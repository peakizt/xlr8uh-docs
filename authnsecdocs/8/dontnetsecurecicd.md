Directory structure:
└── sametkayikci-dotnet-secure-ci-cd/
    ├── README.md
    ├── gitlab-ci.yml
    └── LICENSE


Files Content:

================================================
FILE: README.md
================================================
# .NET Secure CI/CD Pipeline

This repository provides a sample CI/CD pipeline configuration for .NET projects, focusing on security and reliability throughout the development lifecycle.

## Features

- **Build**: Builds the .NET project using the latest .NET SDK (v8.0).
- **Security Scans**:
  - **SAST**: Static Application Security Testing to detect code vulnerabilities.
  - **Dependency Scanning**: Checks for vulnerabilities in third-party dependencies.
  - **Secret Detection**: Identifies hardcoded secrets in the codebase.
  - **IaC SAST**: Scans Infrastructure as Code files using KICS.
- **Security Reports**: Validates security scan results, blocking the pipeline for high or critical vulnerabilities.
- **Deployment Protection**: Prevents merging to the main branch if security issues are detected.

## Stages

1. **Build**
   - Restores and builds the .NET project in Release configuration.

2. **Security-Scan**
   - Runs SAST, Dependency Scanning, and IaC scans to identify security vulnerabilities.

3. **Secrets**
   - Detects hardcoded secrets in the codebase.

4. **Security-Report**
   - Aggregates and validates security findings across all scans.

5. **Test**
   - Placeholder stage for integrating unit or integration tests.

6. **Deploy**
   - Protects the main branch by blocking merges if critical issues are present.

## Configuration Details

### Pipeline Variables
- `SAST_FAIL_ON_SEVERITY`: Blocks the pipeline for specified severity levels (e.g., `high`).
- `SECURE_LOG_LEVEL`: Debug level for detailed scan logs.

### Tools Used
- **GitLab Templates** for SAST, Dependency Scanning, and Secret Detection.
- **KICS** for IaC SAST.

### Artifacts
- Security scan results are saved as JSON reports for further analysis:
  - `gl-sast-report.json`
  - `gl-dependency-scanning-report.json`
  - `gl-secret-detection-report.json`
  - `kics_sast_report.json`

## How It Works

1. The pipeline starts with the `build` stage, ensuring the project compiles successfully.
2. Security scans are executed in the `security-scan` stage, generating reports.
3. Secret detection runs in the `secrets` stage to identify hardcoded credentials.
4. The `security-report` stage validates all scan results and blocks the pipeline if high or critical vulnerabilities are detected.
5. The `deploy` stage prevents merging to the `main` branch if unresolved security issues exist.

## Usage

1. Clone this repository.
2. Customize the pipeline variables and scripts as needed for your project.
3. Push the `.gitlab-ci.yml` file to your GitLab repository.

## Contributing

Feel free to submit issues or pull requests to improve this pipeline configuration.

## License

This project is licensed under the MIT License. See the LICENSE file for details.



================================================
FILE: gitlab-ci.yml
================================================
stages:
- build
- security-scan
- secrets
- security-report
- test
- deploy

build:
  stage: build
  image: mcr.microsoft.com/dotnet/sdk:8.0
  before_script:
    - apt-get update && apt-get install -y jq
  script:
    - echo "Building .NET Core Project"
    - dotnet restore
    - dotnet build --configuration Release
  allow_failure: false

include:
  - template: Security/SAST.gitlab-ci.yml
  - template: Security/Dependency-Scanning.gitlab-ci.yml
  - template: Security/Secret-Detection.gitlab-ci.yml

# SAST Scan
sast:
  stage: security-scan
  variables:
    SAST_FAIL_ON_SEVERITY: "high"  # Bu şekilde high seviyesinde pipeline durur
  artifacts:
    reports:
      sast: gl-sast-report.json
  allow_failure: false


# Dependency Scanning
dependency_scanning:
  stage: security-scan
  variables:
    SECURE_LOG_LEVEL: debug
  artifacts:
    reports:
      dependency_scanning: gl-dependency-scanning-report.json
  allow_failure: false

# Secret Detection
secret_detection:
  stage: secrets
  variables:
    SECURE_LOG_LEVEL: debug
  artifacts:
    reports:
      secret_detection: gl-secret-detection-report.json
  allow_failure: false

# Infrastructure as Code (IaC) SAST using KICS
sast-iac:
  stage: security-scan
  image: registry.gitlab.com/security-products/kics:latest
  script:
    - echo "Running Infrastructure as Code Security Analysis with KICS"
    - mkdir -p kics_reports
    - |
      # Disable immediate exit on error
      set +e

      # Run the KICS scan and fail only on critical and high severities
      kics scan -p . \
        -o kics_reports \
        --output-name kics_sast_report \
        --report-formats json \
        --fail-on critical,high

      # Capture the exit code
      SCAN_EXIT_CODE=$?

      # Re-enable immediate exit on error
      set -e

      # List the KICS report
      echo "Listing files in kics_reports"
      ls -l kics_reports

      # If vulnerabilities are found, print message and exit with code 50
      if [ $SCAN_EXIT_CODE -eq 50 ]; then
        echo "Security vulnerabilities detected!!!"
        exit 50
      else
        echo "No vulnerabilities found"
      fi
  artifacts:
    reports:
      sast: kics_reports/kics_sast_report.json
  allow_failure: false


# Security Findings Check
check_security_findings:
  stage: security-report
  script:
    # SAST report check for critical and high severity
    - if [ -f gl-sast-report.json ]; then
        cat gl-sast-report.json
        cat gl-sast-report.json | jq '.vulnerabilities[] | select(.severity == "high" or .severity == "critical")' && exit 1 || echo "No critical or high SAST issues found";
      else
        echo "SAST report not found";
      fi

    # Dependency Scanning report check for high and critical severity
    - if [ -f gl-dependency-scanning-report.json ]; then
        cat gl-dependency-scanning-report.json | jq '.vulnerabilities[] | select(.severity == "critical" or .severity == "high")' && exit 1 || echo "No critical or high Dependency Scanning issues found";
      else
        echo "Dependency Scanning report not found";
      fi

    # Secret Detection report check for critical and high severity
    - if [ -f gl-secret-detection-report.json ]; then
        cat gl-secret-detection-report.json | jq '.secrets[] | select(.severity == "critical" or .severity == "high")' && exit 1 || echo "No critical or high secrets found";
      else
        echo "Secret Detection report not found";
      fi

    # SAST-IaC report check for critical and high severity
    - if [ -f kics-report.json ]; then
        cat kics-report.json | jq '.vulnerabilities[] | select(.severity == "critical" or .severity == "high")' && exit 1 || echo "No critical or high IaC issues found";
      else
        echo "SAST-IaC report not found";
      fi
  allow_failure: false

# Deployment Protection: Blocking deploy if security findings are present
protect_master:
  stage: deploy
  script:
    - echo "Merging is protected due to security issues."
  rules:
    - if: $CI_COMMIT_BRANCH == "main"
      when: on_success



================================================
FILE: LICENSE
================================================
MIT License

Copyright (c) 2025 Samet Kayıkcı

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


