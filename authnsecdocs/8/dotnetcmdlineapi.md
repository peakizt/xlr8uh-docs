Directory structure:
└── dotnet-command-line-api/
    ├── README.md
    ├── build.cmd
    ├── build.sh
    ├── CODE-OF-CONDUCT.md
    ├── CONTRIBUTING.md
    ├── Directory.Build.props
    ├── Directory.Build.rsp
    ├── Directory.Build.targets
    ├── Directory.Packages.props
    ├── global.json
    ├── LICENSE.md
    ├── NuGet.config
    ├── repack.ps1
    ├── SECURITY.md
    ├── System.CommandLine.sln
    ├── System.CommandLine.v3.ncrunchsolution
    ├── .editorconfig
    ├── .vsts-ci-official.yml
    ├── .vsts-ci.yml
    ├── docs/
    │   ├── readme.md
    │   ├── dotnet-suggest.md
    │   ├── Functional-goals.md
    │   ├── History.md
    │   └── Technical-motivations.md
    ├── eng/
    │   ├── DotNetBuild.props
    │   ├── Publishing.props
    │   ├── Version.Details.xml
    │   ├── Versions.props
    │   └── common/
    │       ├── README.md
    │       ├── build.cmd
    │       ├── build.ps1
    │       ├── build.sh
    │       ├── CIBuild.cmd
    │       ├── cibuild.sh
    │       ├── darc-init.ps1
    │       ├── darc-init.sh
    │       ├── dotnet-install.cmd
    │       ├── dotnet-install.ps1
    │       ├── dotnet-install.sh
    │       ├── enable-cross-org-publishing.ps1
    │       ├── generate-locproject.ps1
    │       ├── generate-sbom-prep.ps1
    │       ├── generate-sbom-prep.sh
    │       ├── helixpublish.proj
    │       ├── init-tools-native.cmd
    │       ├── init-tools-native.ps1
    │       ├── init-tools-native.sh
    │       ├── internal-feed-operations.ps1
    │       ├── internal-feed-operations.sh
    │       ├── msbuild.ps1
    │       ├── msbuild.sh
    │       ├── pipeline-logging-functions.ps1
    │       ├── pipeline-logging-functions.sh
    │       ├── PSScriptAnalyzerSettings.psd1
    │       ├── retain-build.ps1
    │       ├── sdk-task.ps1
    │       ├── SetupNugetSources.ps1
    │       ├── SetupNugetSources.sh
    │       ├── template-guidance.md
    │       ├── tools.ps1
    │       ├── tools.sh
    │       ├── BuildConfiguration/
    │       │   └── build-configuration.json
    │       ├── core-templates/
    │       │   ├── job/
    │       │   │   ├── job.yml
    │       │   │   ├── onelocbuild.yml
    │       │   │   ├── publish-build-assets.yml
    │       │   │   ├── source-build.yml
    │       │   │   └── source-index-stage1.yml
    │       │   ├── jobs/
    │       │   │   ├── codeql-build.yml
    │       │   │   ├── jobs.yml
    │       │   │   └── source-build.yml
    │       │   ├── post-build/
    │       │   │   ├── common-variables.yml
    │       │   │   ├── post-build.yml
    │       │   │   └── setup-maestro-vars.yml
    │       │   ├── steps/
    │       │   │   ├── component-governance.yml
    │       │   │   ├── enable-internal-runtimes.yml
    │       │   │   ├── enable-internal-sources.yml
    │       │   │   ├── generate-sbom.yml
    │       │   │   ├── get-delegation-sas.yml
    │       │   │   ├── get-federated-access-token.yml
    │       │   │   ├── publish-build-artifacts.yml
    │       │   │   ├── publish-logs.yml
    │       │   │   ├── publish-pipeline-artifacts.yml
    │       │   │   ├── retain-build.yml
    │       │   │   ├── send-to-helix.yml
    │       │   │   └── source-build.yml
    │       │   └── variables/
    │       │       └── pool-providers.yml
    │       ├── cross/
    │       │   ├── build-android-rootfs.sh
    │       │   ├── build-rootfs.sh
    │       │   ├── tizen-build-rootfs.sh
    │       │   ├── tizen-fetch.sh
    │       │   ├── toolchain.cmake
    │       │   ├── arm/
    │       │   │   └── tizen/
    │       │   │       └── tizen.patch
    │       │   ├── arm64/
    │       │   │   └── tizen/
    │       │   │       └── tizen.patch
    │       │   ├── armel/
    │       │   │   ├── armel.jessie.patch
    │       │   │   └── tizen/
    │       │   │       └── tizen.patch
    │       │   ├── riscv64/
    │       │   │   └── tizen/
    │       │   │       └── tizen.patch
    │       │   └── x86/
    │       │       └── tizen/
    │       │           └── tizen.patch
    │       ├── internal/
    │       │   ├── Directory.Build.props
    │       │   ├── NuGet.config
    │       │   └── Tools.csproj
    │       ├── loc/
    │       │   └── P22DotNetHtmlLocalization.lss
    │       ├── native/
    │       │   ├── common-library.sh
    │       │   ├── CommonLibrary.psm1
    │       │   ├── init-compiler.sh
    │       │   ├── init-distro-rid.sh
    │       │   ├── init-os-and-arch.sh
    │       │   ├── install-cmake-test.sh
    │       │   ├── install-cmake.sh
    │       │   └── install-tool.ps1
    │       ├── post-build/
    │       │   ├── check-channel-consistency.ps1
    │       │   ├── nuget-validation.ps1
    │       │   ├── nuget-verification.ps1
    │       │   ├── publish-using-darc.ps1
    │       │   ├── redact-logs.ps1
    │       │   ├── sourcelink-validation.ps1
    │       │   └── symbols-validation.ps1
    │       ├── sdl/
    │       │   ├── configure-sdl-tool.ps1
    │       │   ├── execute-all-sdl-tools.ps1
    │       │   ├── extract-artifact-archives.ps1
    │       │   ├── extract-artifact-packages.ps1
    │       │   ├── init-sdl.ps1
    │       │   ├── NuGet.config
    │       │   ├── packages.config
    │       │   ├── run-sdl.ps1
    │       │   ├── sdl.ps1
    │       │   └── trim-assets-version.ps1
    │       ├── templates/
    │       │   ├── job/
    │       │   │   ├── job.yml
    │       │   │   ├── onelocbuild.yml
    │       │   │   ├── publish-build-assets.yml
    │       │   │   ├── source-build.yml
    │       │   │   └── source-index-stage1.yml
    │       │   ├── jobs/
    │       │   │   ├── codeql-build.yml
    │       │   │   ├── jobs.yml
    │       │   │   └── source-build.yml
    │       │   ├── post-build/
    │       │   │   ├── common-variables.yml
    │       │   │   ├── post-build.yml
    │       │   │   └── setup-maestro-vars.yml
    │       │   ├── steps/
    │       │   │   ├── component-governance.yml
    │       │   │   ├── enable-internal-runtimes.yml
    │       │   │   ├── enable-internal-sources.yml
    │       │   │   ├── generate-sbom.yml
    │       │   │   ├── get-delegation-sas.yml
    │       │   │   ├── get-federated-access-token.yml
    │       │   │   ├── publish-build-artifacts.yml
    │       │   │   ├── publish-logs.yml
    │       │   │   ├── publish-pipeline-artifacts.yml
    │       │   │   ├── retain-build.yml
    │       │   │   ├── send-to-helix.yml
    │       │   │   └── source-build.yml
    │       │   └── variables/
    │       │       └── pool-providers.yml
    │       └── templates-official/
    │           ├── job/
    │           │   ├── job.yml
    │           │   ├── onelocbuild.yml
    │           │   ├── publish-build-assets.yml
    │           │   ├── source-build.yml
    │           │   └── source-index-stage1.yml
    │           ├── jobs/
    │           │   ├── codeql-build.yml
    │           │   ├── jobs.yml
    │           │   └── source-build.yml
    │           ├── post-build/
    │           │   ├── common-variables.yml
    │           │   ├── post-build.yml
    │           │   └── setup-maestro-vars.yml
    │           ├── steps/
    │           │   ├── component-governance.yml
    │           │   ├── enable-internal-runtimes.yml
    │           │   ├── enable-internal-sources.yml
    │           │   ├── generate-sbom.yml
    │           │   ├── get-delegation-sas.yml
    │           │   ├── get-federated-access-token.yml
    │           │   ├── publish-build-artifacts.yml
    │           │   ├── publish-logs.yml
    │           │   ├── publish-pipeline-artifacts.yml
    │           │   ├── retain-build.yml
    │           │   ├── send-to-helix.yml
    │           │   └── source-build.yml
    │           └── variables/
    │               ├── pool-providers.yml
    │               └── sdl-variables.yml
    ├── src/
    │   ├── System.Diagnostics.CodeAnalysis.cs
    │   ├── Common/
    │   │   ├── ArgumentBuilder.cs
    │   │   └── OptionBuilder.cs
    │   ├── System.CommandLine/
    │   │   ├── AliasSet.cs
    │   │   ├── Argument.cs
    │   │   ├── ArgumentArity.cs
    │   │   ├── ArgumentValidation.cs
    │   │   ├── Argument{T}.cs
    │   │   ├── ChildSymbolList{T}.cs
    │   │   ├── Command.cs
    │   │   ├── CommandLineConfiguration.cs
    │   │   ├── CommandLineConfigurationException.cs
    │   │   ├── CompletionSourceExtensions.cs
    │   │   ├── ConsoleHelpers.cs
    │   │   ├── Directive.cs
    │   │   ├── EnumerableExtensions.cs
    │   │   ├── EnvironmentVariablesDirective.cs
    │   │   ├── LocalizationResources.cs
    │   │   ├── Option.cs
    │   │   ├── OptionValidation.cs
    │   │   ├── Option{T}.cs
    │   │   ├── ParseDiagramDirective.cs
    │   │   ├── ParseResult.cs
    │   │   ├── RootCommand.cs
    │   │   ├── Symbol.cs
    │   │   ├── SymbolNode.cs
    │   │   ├── System.CommandLine.Config.cs
    │   │   ├── System.CommandLine.csproj
    │   │   ├── VersionOption.cs
    │   │   ├── Binding/
    │   │   │   ├── ArgumentConversionResult.cs
    │   │   │   ├── ArgumentConversionResultType.cs
    │   │   │   ├── ArgumentConverter.cs
    │   │   │   ├── ArgumentConverter.DefaultValues.cs
    │   │   │   ├── ArgumentConverter.StringConverters.cs
    │   │   │   ├── TryConvertArgument.cs
    │   │   │   └── TypeExtensions.cs
    │   │   ├── Completions/
    │   │   │   ├── CompletionAction.cs
    │   │   │   ├── CompletionContext.cs
    │   │   │   ├── CompletionItem.cs
    │   │   │   ├── SuggestDirective.cs
    │   │   │   └── TextCompletionContext.cs
    │   │   ├── Help/
    │   │   │   ├── HelpAction.cs
    │   │   │   ├── HelpBuilder.cs
    │   │   │   ├── HelpBuilder.Default.cs
    │   │   │   ├── HelpBuilderExtensions.cs
    │   │   │   ├── HelpContext.cs
    │   │   │   ├── HelpOption.cs
    │   │   │   └── TwoColumnHelpRow.cs
    │   │   ├── Invocation/
    │   │   │   ├── AnonymousAsynchronousCommandLineAction.cs
    │   │   │   ├── AnonymousSynchronousCommandLineAction.cs
    │   │   │   ├── AsynchronousCommandLineAction.cs
    │   │   │   ├── CommandLineAction.cs
    │   │   │   ├── InvocationPipeline.cs
    │   │   │   ├── ParseErrorAction.cs
    │   │   │   ├── ProcessTerminationHandler.cs
    │   │   │   └── SynchronousCommandLineAction.cs
    │   │   ├── Parsing/
    │   │   │   ├── ArgumentResult.cs
    │   │   │   ├── CommandLineParser.cs
    │   │   │   ├── CommandResult.cs
    │   │   │   ├── DirectiveResult.cs
    │   │   │   ├── OptionResult.cs
    │   │   │   ├── ParseDiagramAction.cs
    │   │   │   ├── ParseError.cs
    │   │   │   ├── ParseOperation.cs
    │   │   │   ├── StringExtensions.cs
    │   │   │   ├── SymbolResult.cs
    │   │   │   ├── SymbolResultExtensions.cs
    │   │   │   ├── SymbolResultTree.cs
    │   │   │   ├── Token.cs
    │   │   │   ├── TokenType.cs
    │   │   │   └── TryReplaceToken.cs
    │   │   ├── Properties/
    │   │   │   ├── Resources.Designer.cs
    │   │   │   ├── Resources.resx
    │   │   │   └── xlf/
    │   │   │       ├── Resources.cs.xlf
    │   │   │       ├── Resources.de.xlf
    │   │   │       ├── Resources.es.xlf
    │   │   │       ├── Resources.fr.xlf
    │   │   │       ├── Resources.it.xlf
    │   │   │       ├── Resources.ja.xlf
    │   │   │       ├── Resources.ko.xlf
    │   │   │       ├── Resources.pl.xlf
    │   │   │       ├── Resources.pt-BR.xlf
    │   │   │       ├── Resources.ru.xlf
    │   │   │       ├── Resources.tr.xlf
    │   │   │       ├── Resources.zh-Hans.xlf
    │   │   │       └── Resources.zh-Hant.xlf
    │   │   ├── System.Diagnostics.CodeAnalysis/
    │   │   │   ├── DynamicallyAccessedMembersAttribute.cs
    │   │   │   ├── DynamicallyAccessedMemberTypes.cs
    │   │   │   └── UnconditionalSuppressMessageAttribute.cs
    │   │   └── System.Runtime.CompilerServices/
    │   │       └── IsExternalInit.cs
    │   ├── System.CommandLine.ApiCompatibility.Tests/
    │   │   ├── ApiCompatibilityApprovalTests.cs
    │   │   ├── ApiCompatibilityApprovalTests.System_CommandLine_api_is_not_changed.approved.txt
    │   │   ├── ApiContract.cs
    │   │   ├── LocalizationTests.cs
    │   │   └── System.CommandLine.ApiCompatibility.Tests.csproj
    │   ├── System.CommandLine.Benchmarks/
    │   │   ├── Categories.cs
    │   │   ├── Program.cs
    │   │   ├── RecommendedConfig.cs
    │   │   ├── System.CommandLine.Benchmarks.csproj
    │   │   ├── System.CommandLine.Benchmarks.net5.0.v3.ncrunchproject
    │   │   ├── System.CommandLine.Benchmarks.v3.ncrunchproject
    │   │   ├── CommandLine/
    │   │   │   ├── Perf_Parser_CustomScenarios.cs
    │   │   │   ├── Perf_Parser_Directives_Suggest.cs
    │   │   │   ├── Perf_Parser_NestedCommands.cs
    │   │   │   ├── Perf_Parser_Options_Bare.cs
    │   │   │   ├── Perf_Parser_Options_With_Arguments.cs
    │   │   │   ├── Perf_Parser_ParseResult.cs
    │   │   │   ├── Perf_Parser_Simple.cs
    │   │   │   ├── Perf_Parser_TypoCorrection.cs
    │   │   │   └── Perf_Suggestions.cs
    │   │   ├── Helpers/
    │   │   │   ├── BdnParam.cs
    │   │   │   ├── NullStreamWriter.cs
    │   │   │   └── Utils.cs
    │   │   └── Input/
    │   │       └── Sample1.Main.cs
    │   ├── System.CommandLine.Suggest/
    │   │   ├── build-and-install.ps1
    │   │   ├── CombineSuggestionRegistration.cs
    │   │   ├── dotnet-suggest-shim.bash
    │   │   ├── dotnet-suggest-shim.ps1
    │   │   ├── dotnet-suggest-shim.zsh
    │   │   ├── dotnet-suggest.csproj
    │   │   ├── DotnetMuxer.cs
    │   │   ├── DotnetProfileDirectory.cs
    │   │   ├── FileEnumerator.cs
    │   │   ├── FileSuggestionRegistration.cs
    │   │   ├── GlobalToolsSuggestionRegistration.cs
    │   │   ├── ISuggestionRegistration.cs
    │   │   ├── ISuggestionStore.cs
    │   │   ├── PathExtensions.cs
    │   │   ├── Program.cs
    │   │   ├── RegistrationPair.cs
    │   │   ├── ShellType.cs
    │   │   ├── StringExtensions.cs
    │   │   ├── SuggestionDispatcher.cs
    │   │   ├── SuggestionShellScriptException.cs
    │   │   ├── SuggestionShellScriptHandler.cs
    │   │   └── SuggestionStore.cs
    │   ├── System.CommandLine.Suggest.Tests/
    │   │   ├── dotnet-suggest.Tests.csproj
    │   │   ├── DotnetSuggestEndToEndTests.cs
    │   │   ├── FileEnumeratorTests.cs
    │   │   ├── FileSuggestionProviderTests.cs
    │   │   ├── GlobalToolsSuggestionRegistrationTests.cs
    │   │   ├── SuggestionDispatcherTests.cs
    │   │   ├── SuggestionRegistrationTest.cs
    │   │   ├── SuggestionShellScriptHandlerTest.cs
    │   │   ├── TestSuggestionRegistration.cs
    │   │   ├── TestSuggestionRegistrationTests.cs
    │   │   └── EndToEndTestApp/
    │   │       ├── EndToEndTestApp.csproj
    │   │       └── Program.cs
    │   └── System.CommandLine.Tests/
    │       ├── ArgumentTests.cs
    │       ├── CommandLineConfigurationTests.cs
    │       ├── CommandTests.cs
    │       ├── CompilationTests.cs
    │       ├── CompletionContextTests.cs
    │       ├── CompletionTests.cs
    │       ├── CustomParsingTests.cs
    │       ├── DirectiveTests.cs
    │       ├── EnvironmentVariableDirectiveTests.cs
    │       ├── GetValueByNameParserTests.cs
    │       ├── GlobalOptionTests.cs
    │       ├── HelpOptionTests.cs
    │       ├── OptionTests.cs
    │       ├── OptionTests.MultipleArgumentsPerToken.cs
    │       ├── ParseDiagramTests.cs
    │       ├── ParseDirectiveTests.cs
    │       ├── ParseErrorReportingTests.cs
    │       ├── ParseResultTests.cs
    │       ├── ParserTests.cs
    │       ├── ParserTests.DoubleDash.cs
    │       ├── ParserTests.MultipleArguments.cs
    │       ├── ParserTests.MultiplePositions.cs
    │       ├── ParserTests.RootCommandAndArg0.cs
    │       ├── ParserTests.SetupErrors.cs
    │       ├── ParsingValidationTests.cs
    │       ├── ResponseFileTests.cs
    │       ├── RootCommandTests.cs
    │       ├── SplitCommandLineTests.cs
    │       ├── SuggestDirectiveTests.cs
    │       ├── System.CommandLine.Tests.csproj
    │       ├── TestCliActions.cs
    │       ├── TokenReplacementTests.cs
    │       ├── UseExceptionHandlerTests.cs
    │       ├── VersionOptionTests.cs
    │       ├── Binding/
    │       │   ├── TestModels.cs
    │       │   └── TypeConversionTests.cs
    │       ├── Help/
    │       │   ├── ApprovalTests.Config.cs
    │       │   ├── CustomHelpAction.cs
    │       │   ├── HelpBuilderExtensions.cs
    │       │   ├── HelpBuilderTests.Approval.cs
    │       │   ├── HelpBuilderTests.cs
    │       │   ├── HelpBuilderTests.Customization.cs
    │       │   └── Approvals/
    │       │       └── HelpBuilderTests.Help_layout_has_not_changed.approved.txt
    │       ├── Invocation/
    │       │   ├── CancelOnProcessTerminationTests.cs
    │       │   ├── InvocationTests.cs
    │       │   └── TypoCorrectionTests.cs
    │       ├── Parsing/
    │       │   └── CommandLineStringSplitterTests.cs
    │       ├── TestApps/
    │       │   ├── NativeAOT/
    │       │   │   ├── NativeAOT.csproj
    │       │   │   └── Program.cs
    │       │   └── Trimming/
    │       │       ├── Program.cs
    │       │       └── Trimming.csproj
    │       └── Utility/
    │           ├── AssertionExtensions.cs
    │           ├── LinuxOnlyTheory.cs
    │           ├── NonWindowsOnlyFactAttribute.cs
    │           ├── ParseResultExtensions.cs
    │           ├── Process.cs
    │           ├── ReleaseBuildOnlyFactAttribute.cs
    │           ├── ReleaseBuildOnlyTheoryAttribute.cs
    │           ├── RemoteExecution.cs
    │           ├── RemoteExecutor.cs
    │           └── WindowsOnlyFactAttribute.cs
    └── .config/
        └── tsaoptions.json


Files Content:

(Files content cropped to 300k characters, download full ingest to see more)
================================================
FILE: README.md
================================================


[![Build Status](https://dev.azure.com/dnceng-public/public/_apis/build/status/dotnet/command-line-api/command-line-api?branchName=main)](https://dev.azure.com/dnceng-public/public/_build?definitionId=175&branchName=main) [![Join the chat at https://gitter.im/dotnet/command-line-api](https://badges.gitter.im/dotnet/command-line-api.svg)](https://gitter.im/dotnet/command-line-api?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

This repository contains the code for the System.CommandLine libraries and the `dotnet-suggest` global tool.

## Packages

Package                          | Version                                                                                                                                     | Description
---------------------------------| ------------------------------------------------------------------------------------------------------------------------------------------- | -----------------------------
`System.CommandLine`             | [![Nuget](https://img.shields.io/nuget/v/System.CommandLine.svg)](https://nuget.org/packages/System.CommandLine)                            | Command line parser, model binding, invocation, shell completions
`dotnet-suggest`                 | [![Nuget](https://img.shields.io/nuget/v/dotnet-suggest.svg)](https://nuget.org/packages/dotnet-suggest)                                    | A command-line tool to provide shell completions for apps built using `System.CommandLine`.

### Daily Builds

Daily builds are available if you add this feed to your nuget.config: `https://pkgs.dev.azure.com/dnceng/public/_packaging/dotnet-libraries/nuget/v3/index.json`

Versions are listed at: https://dev.azure.com/dnceng/public/_artifacts/feed/dotnet-libraries/NuGet/System.CommandLine/versions

## Documentation

The System.CommandLine documentation can now be found at [Microsoft Learn](https://learn.microsoft.com/en-us/dotnet/standard/commandline/).

## Code of Conduct

This project has adopted the code of conduct defined by the [Contributor Covenant](https://www.contributor-covenant.org/) to clarify expected behavior in our community. For more information, see the [.NET Foundation Code of Conduct](https://www.dotnetfoundation.org/code-of-conduct)

## Contributing

See the [Contributing guide](CONTRIBUTING.md) for developer documentation.

## License

This project is licensed under the [MIT license](LICENSE.md).

## .NET Foundation

.NET is a [.NET Foundation](http://www.dotnetfoundation.org/projects) project.



================================================
FILE: build.cmd
================================================
@echo off
powershell -NoLogo -NoProfile -ExecutionPolicy ByPass %~dp0eng\common\build.ps1 -build -restore %*
exit /b %ErrorLevel%



================================================
FILE: build.sh
================================================
#!/usr/bin/env bash

source="${BASH_SOURCE[0]}"

# resolve $SOURCE until the file is no longer a symlink
while [[ -h $source ]]; do
  scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"
  source="$(readlink "$source")"

  # if $source was a relative symlink, we need to resolve it relative to the path where the
  # symlink file was located
  [[ $source != /* ]] && source="$scriptroot/$source"
done

scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"
"$scriptroot/eng/common/build.sh" --build --restore $@



================================================
FILE: CODE-OF-CONDUCT.md
================================================
# Code of Conduct

This project has adopted the code of conduct defined by the Contributor Covenant
to clarify expected behavior in our community.

For more information, see the [.NET Foundation Code of Conduct](https://dotnetfoundation.org/code-of-conduct).



================================================
FILE: CONTRIBUTING.md
================================================
Contributing
============

Please read [.NET Guidelines](https://github.com/dotnet/runtime/blob/master/CONTRIBUTING.md) for more general information about coding styles, source structure, making pull requests, and more.

## Developer guide

This project can be developed on any platform. To get started, follow instructions for your OS.

### Prerequisites

This project depends on .NET 7. Before working on the project, check that the [.NET SDK](https://dotnet.microsoft.com/en-us/download) is installed.

### Visual Studio

This project supports [Visual Studio 2022](https://visualstudio.com). Any version, including the free Community Edition, should be sufficient.

This project also supports using
[Visual Studio Code](https://code.visualstudio.com). Install the [C# Dev Kit](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csdevkit).

### Command line scripts

This project can be built on the command line using the `build.cmd`/`build.sh` scripts.

Run `.\build.cmd -help` or `./build.sh --help` to see more options.

### Compile

Windows:

    > .\build.cmd

macOS/Linux

    $ ./build.sh

### Running tests

To build **and** run tests:

Windows:

    > .\build.cmd -test

macOS/Linux:

    $ ./build.sh --test




================================================
FILE: Directory.Build.props
================================================
<Project>

  <Import Project="Sdk.props"
          Sdk="Microsoft.DotNet.Arcade.Sdk"
          Condition="'$(DisableArcade)' != '1'" />

  <PropertyGroup>
    <NoWarn>$(NoWarn);NU5125;CS0618</NoWarn>
    <PackageLicenseExpression>MIT</PackageLicenseExpression>
    <LangVersion>13.0</LangVersion>
    <PackageProjectUrl>https://github.com/dotnet/command-line-api</PackageProjectUrl>
  </PropertyGroup>

  <PropertyGroup>
    <TargetFrameworkForNETSDK Condition="'$(DotNetBuildSourceOnly)' == 'true'">$(NetCurrent)</TargetFrameworkForNETSDK>
    <TargetFrameworkForNETSDK Condition="'$(DotNetBuildSourceOnly)' != 'true'">net8.0</TargetFrameworkForNETSDK>
  </PropertyGroup>

</Project>



================================================
FILE: Directory.Build.rsp
================================================
# This file intentionally left blank to avoid accidental import during build.



================================================
FILE: Directory.Build.targets
================================================
<Project>

  <Import Project="Sdk.targets"
          Sdk="Microsoft.DotNet.Arcade.Sdk"
          Condition="'$(DisableArcade)' != '1'" />

  <PropertyGroup Condition="'$(DisableArcade)' == '1' and $(MSBuildProjectName.EndsWith('.Tests'))">
    <DefaultExcludesInProjectFolder>$(DefaultExcludesInProjectFolder);TestResults\**</DefaultExcludesInProjectFolder>
    <IsPackable>false</IsPackable>
  </PropertyGroup>

  <ItemGroup Condition="'$(DisableArcade)' == '1' and $(MSBuildProjectName.EndsWith('.Tests'))">
    <PackageReference Include="xunit" />
    <PackageReference Include="xunit.runner.visualstudio" />
  </ItemGroup>

	<Target Name="PublishAfterBuild"
         AfterTargets="Build"
         DependsOnTargets="Publish"
         Condition="'$(PublishAfterBuild)' == 'true'" />

</Project>



================================================
FILE: Directory.Packages.props
================================================
<Project>

  <PropertyGroup>
    <ManagePackageVersionsCentrally>true</ManagePackageVersionsCentrally>
    <CentralPackageTransitivePinningEnabled>false</CentralPackageTransitivePinningEnabled>
    <!-- Using multiple feeds isn't supported by Maestro: https://github.com/dotnet/arcade/issues/14155. -->
    <NoWarn>$(NoWarn);NU1507</NoWarn>
  </PropertyGroup>

  <ItemGroup>
    <!-- Roslyn dependencies -->
    <PackageVersion Include="Microsoft.CodeAnalysis" Version="4.0.1" />
    <PackageVersion Include="Microsoft.CodeAnalysis.Analyzers" Version="3.3.3" />
    <PackageVersion Include="Microsoft.CodeAnalysis.CSharp" Version="4.0.1" />
    <PackageVersion Include="Microsoft.CodeAnalysis.CSharp.Scripting" Version="4.0.1" />
    <!-- Runtime dependencies -->
    <PackageVersion Include="Microsoft.Extensions.Configuration.CommandLine" Version="8.0.0" />
    <PackageVersion Include="Microsoft.Extensions.DependencyInjection.Abstractions" Version="8.0.2" />
    <PackageVersion Include="Microsoft.Extensions.Hosting" Version="8.0.1" />
    <!-- external dependencies -->
    <PackageVersion Include="ApprovalTests" Version="7.0.0-beta.3" />
    <PackageVersion Include="BenchmarkDotNet" Version="0.13.1" />
    <PackageVersion Include="AwesomeAssertions" Version="8.1.0" />
    <PackageVersion Include="Microsoft.CSharp" Version="4.7.0" />
    <PackageVersion Include="Microsoft.DotNet.PlatformAbstractions" Version="3.1.6" />
    <PackageVersion Include="Newtonsoft.Json" Version="13.0.3" />
    <PackageVersion Include="System.Memory" Version="4.5.4" />
    <PackageVersion Include="system.reactive.core" Version="6.0.0" />
  </ItemGroup>

  <ItemGroup Condition="'$(DisableArcade)' == '1'">
    <!-- The xunit version should be kept in sync with the one that Arcade promotes -->
    <PackageVersion Include="xunit" Version="2.4.2" />
    <PackageVersion Include="xunit.runner.visualstudio" Version="2.4.3" />
  </ItemGroup>

</Project>



================================================
FILE: global.json
================================================
{
  "tools": {
    "dotnet": "9.0.106",
    "runtimes": {
      "dotnet": [
        "8.0.12"
      ]
    }
  },
  "msbuild-sdks": {
    "Microsoft.DotNet.Arcade.Sdk": "9.0.0-beta.25302.2"
  }
}



================================================
FILE: LICENSE.md
================================================
The MIT License (MIT)

Copyright © .NET Foundation and Contributors

All rights reserved.

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



================================================
FILE: NuGet.config
================================================
<?xml version="1.0" encoding="utf-8"?>
<configuration>
  <!-- Only specify feed for Arcade SDK (see https://github.com/Microsoft/msbuild/issues/2982) -->
  <packageSources>
    <clear />
    <add key="dotnet-public" value="https://pkgs.dev.azure.com/dnceng/public/_packaging/dotnet-public/nuget/v3/index.json" />
    <add key="dotnet5" value="https://pkgs.dev.azure.com/dnceng/public/_packaging/dotnet5/nuget/v3/index.json" />
    <add key="dotnet5-transport" value="https://pkgs.dev.azure.com/dnceng/public/_packaging/dotnet5-transport/nuget/v3/index.json" />
    <add key="dotnet-eng" value="https://pkgs.dev.azure.com/dnceng/public/_packaging/dotnet-eng/nuget/v3/index.json" />
    <add key="dotnet-tools" value="https://pkgs.dev.azure.com/dnceng/public/_packaging/dotnet-tools/nuget/v3/index.json" />
    <add key="dotnet-libraries" value="https://pkgs.dev.azure.com/dnceng/public/_packaging/dotnet-libraries/nuget/v3/index.json" />
    <add key="dotnet8" value="https://pkgs.dev.azure.com/dnceng/public/_packaging/dotnet8/nuget/v3/index.json" />
  </packageSources>
  <disabledPackageSources />
</configuration>



================================================
FILE: repack.ps1
================================================

# clean up the previously-cached NuGet packages
Remove-Item -Recurse ~\.nuget\packages\System.CommandLine* -Force

# build and pack dotnet-interactive
dotnet clean
dotnet pack  /p:PackageVersion=2.0.0-dev

# copy the dotnet-interactive packages to the temp directory
Get-ChildItem -Recurse -Filter *.nupkg | Copy-Item -Destination c:\temp -Force




================================================
FILE: SECURITY.md
================================================
# Security Policy

## Supported Versions

The .NET Core and ASP.NET Core support policy, including supported versions can be found at the [.NET Core Support Policy Page](https://dotnet.microsoft.com/platform/support/policy/dotnet-core).

## Reporting a Vulnerability

Security issues and bugs should be reported privately to the Microsoft Security Response Center (MSRC), either by emailing secure@microsoft.com or via the portal at https://msrc.microsoft.com.
You should receive a response within 24 hours. If for some reason you do not, please follow up via email to ensure we received your
original message. Further information, including the MSRC PGP key, can be found in the [MSRC Report an Issue FAQ](https://www.microsoft.com/en-us/msrc/faqs-report-an-issue).

Reports via MSRC may qualify for the .NET Core Bug Bounty. Details of the .NET Core Bug Bounty including terms and conditions are at [https://aka.ms/corebounty](https://aka.ms/corebounty).

Please do not open issues for anything you think might have a security implication.


================================================
FILE: System.CommandLine.sln
================================================
﻿
Microsoft Visual Studio Solution File, Format Version 12.00
# Visual Studio Version 17
VisualStudioVersion = 17.0.31714.462
MinimumVisualStudioVersion = 10.0.40219.1
Project("{2150E333-8FDC-42A3-9474-1A3956D46DE8}") = "Solution Items", "Solution Items", "{5BBF2B6C-2655-4B53-A3FA-21A901662C0D}"
	ProjectSection(SolutionItems) = preProject
		.editorconfig = .editorconfig
		.gitattributes = .gitattributes
		.gitignore = .gitignore
		build.cmd = build.cmd
		build.sh = build.sh
		Directory.Build.props = Directory.Build.props
		Directory.Build.rsp = Directory.Build.rsp
		Directory.Build.targets = Directory.Build.targets
		Directory.Packages.props = Directory.Packages.props
		global.json = global.json
		LICENSE.md = LICENSE.md
		README.md = README.md
		restore.cmd = restore.cmd
		restore.sh = restore.sh
		test.cmd = test.cmd
		test.sh = test.sh
	EndProjectSection
EndProject
Project("{2150E333-8FDC-42A3-9474-1A3956D46DE8}") = "src", "src", "{E5B1EC71-0FC4-4FAA-9C65-32D5016FBC45}"
EndProject
Project("{9A19103F-16F7-4668-BE54-9A1E7A4F7556}") = "System.CommandLine", "src\System.CommandLine\System.CommandLine.csproj", "{0BE8E56E-7580-4526-BE24-D304E1779724}"
EndProject
Project("{9A19103F-16F7-4668-BE54-9A1E7A4F7556}") = "System.CommandLine.Tests", "src\System.CommandLine.Tests\System.CommandLine.Tests.csproj", "{F843CCCA-4CC9-422C-A881-3AE6A998B53F}"
EndProject
Project("{9A19103F-16F7-4668-BE54-9A1E7A4F7556}") = "dotnet-suggest", "src\System.CommandLine.Suggest\dotnet-suggest.csproj", "{E23C760E-B826-4B4F-BE76-916D86BAD2DB}"
EndProject
Project("{9A19103F-16F7-4668-BE54-9A1E7A4F7556}") = "dotnet-suggest.Tests", "src\System.CommandLine.Suggest.Tests\dotnet-suggest.Tests.csproj", "{E41F0471-B14D-4FA0-9D8B-1E7750695AE9}"
EndProject
Project("{9A19103F-16F7-4668-BE54-9A1E7A4F7556}") = "System.CommandLine.ApiCompatibility.Tests", "src\System.CommandLine.ApiCompatibility.Tests\System.CommandLine.ApiCompatibility.Tests.csproj", "{A54EE328-D456-4BAF-A180-84E77E6409AC}"
EndProject
Global
	GlobalSection(SolutionConfigurationPlatforms) = preSolution
		Debug|Any CPU = Debug|Any CPU
		Debug|x64 = Debug|x64
		Debug|x86 = Debug|x86
		Release|Any CPU = Release|Any CPU
		Release|x64 = Release|x64
		Release|x86 = Release|x86
	EndGlobalSection
	GlobalSection(ProjectConfigurationPlatforms) = postSolution
		{0BE8E56E-7580-4526-BE24-D304E1779724}.Debug|Any CPU.ActiveCfg = Debug|Any CPU
		{0BE8E56E-7580-4526-BE24-D304E1779724}.Debug|Any CPU.Build.0 = Debug|Any CPU
		{0BE8E56E-7580-4526-BE24-D304E1779724}.Debug|x64.ActiveCfg = Debug|Any CPU
		{0BE8E56E-7580-4526-BE24-D304E1779724}.Debug|x64.Build.0 = Debug|Any CPU
		{0BE8E56E-7580-4526-BE24-D304E1779724}.Debug|x86.ActiveCfg = Debug|Any CPU
		{0BE8E56E-7580-4526-BE24-D304E1779724}.Debug|x86.Build.0 = Debug|Any CPU
		{0BE8E56E-7580-4526-BE24-D304E1779724}.Release|Any CPU.ActiveCfg = Release|Any CPU
		{0BE8E56E-7580-4526-BE24-D304E1779724}.Release|Any CPU.Build.0 = Release|Any CPU
		{0BE8E56E-7580-4526-BE24-D304E1779724}.Release|x64.ActiveCfg = Release|Any CPU
		{0BE8E56E-7580-4526-BE24-D304E1779724}.Release|x64.Build.0 = Release|Any CPU
		{0BE8E56E-7580-4526-BE24-D304E1779724}.Release|x86.ActiveCfg = Release|Any CPU
		{0BE8E56E-7580-4526-BE24-D304E1779724}.Release|x86.Build.0 = Release|Any CPU
		{F843CCCA-4CC9-422C-A881-3AE6A998B53F}.Debug|Any CPU.ActiveCfg = Debug|Any CPU
		{F843CCCA-4CC9-422C-A881-3AE6A998B53F}.Debug|Any CPU.Build.0 = Debug|Any CPU
		{F843CCCA-4CC9-422C-A881-3AE6A998B53F}.Debug|x64.ActiveCfg = Debug|Any CPU
		{F843CCCA-4CC9-422C-A881-3AE6A998B53F}.Debug|x64.Build.0 = Debug|Any CPU
		{F843CCCA-4CC9-422C-A881-3AE6A998B53F}.Debug|x86.ActiveCfg = Debug|Any CPU
		{F843CCCA-4CC9-422C-A881-3AE6A998B53F}.Debug|x86.Build.0 = Debug|Any CPU
		{F843CCCA-4CC9-422C-A881-3AE6A998B53F}.Release|Any CPU.ActiveCfg = Release|Any CPU
		{F843CCCA-4CC9-422C-A881-3AE6A998B53F}.Release|Any CPU.Build.0 = Release|Any CPU
		{F843CCCA-4CC9-422C-A881-3AE6A998B53F}.Release|x64.ActiveCfg = Release|Any CPU
		{F843CCCA-4CC9-422C-A881-3AE6A998B53F}.Release|x64.Build.0 = Release|Any CPU
		{F843CCCA-4CC9-422C-A881-3AE6A998B53F}.Release|x86.ActiveCfg = Release|Any CPU
		{F843CCCA-4CC9-422C-A881-3AE6A998B53F}.Release|x86.Build.0 = Release|Any CPU
		{E23C760E-B826-4B4F-BE76-916D86BAD2DB}.Debug|Any CPU.ActiveCfg = Debug|Any CPU
		{E23C760E-B826-4B4F-BE76-916D86BAD2DB}.Debug|Any CPU.Build.0 = Debug|Any CPU
		{E23C760E-B826-4B4F-BE76-916D86BAD2DB}.Debug|x64.ActiveCfg = Debug|Any CPU
		{E23C760E-B826-4B4F-BE76-916D86BAD2DB}.Debug|x64.Build.0 = Debug|Any CPU
		{E23C760E-B826-4B4F-BE76-916D86BAD2DB}.Debug|x86.ActiveCfg = Debug|Any CPU
		{E23C760E-B826-4B4F-BE76-916D86BAD2DB}.Debug|x86.Build.0 = Debug|Any CPU
		{E23C760E-B826-4B4F-BE76-916D86BAD2DB}.Release|Any CPU.ActiveCfg = Release|Any CPU
		{E23C760E-B826-4B4F-BE76-916D86BAD2DB}.Release|Any CPU.Build.0 = Release|Any CPU
		{E23C760E-B826-4B4F-BE76-916D86BAD2DB}.Release|x64.ActiveCfg = Release|Any CPU
		{E23C760E-B826-4B4F-BE76-916D86BAD2DB}.Release|x64.Build.0 = Release|Any CPU
		{E23C760E-B826-4B4F-BE76-916D86BAD2DB}.Release|x86.ActiveCfg = Release|Any CPU
		{E23C760E-B826-4B4F-BE76-916D86BAD2DB}.Release|x86.Build.0 = Release|Any CPU
		{E41F0471-B14D-4FA0-9D8B-1E7750695AE9}.Debug|Any CPU.ActiveCfg = Debug|Any CPU
		{E41F0471-B14D-4FA0-9D8B-1E7750695AE9}.Debug|Any CPU.Build.0 = Debug|Any CPU
		{E41F0471-B14D-4FA0-9D8B-1E7750695AE9}.Debug|x64.ActiveCfg = Debug|Any CPU
		{E41F0471-B14D-4FA0-9D8B-1E7750695AE9}.Debug|x64.Build.0 = Debug|Any CPU
		{E41F0471-B14D-4FA0-9D8B-1E7750695AE9}.Debug|x86.ActiveCfg = Debug|Any CPU
		{E41F0471-B14D-4FA0-9D8B-1E7750695AE9}.Debug|x86.Build.0 = Debug|Any CPU
		{E41F0471-B14D-4FA0-9D8B-1E7750695AE9}.Release|Any CPU.ActiveCfg = Release|Any CPU
		{E41F0471-B14D-4FA0-9D8B-1E7750695AE9}.Release|Any CPU.Build.0 = Release|Any CPU
		{E41F0471-B14D-4FA0-9D8B-1E7750695AE9}.Release|x64.ActiveCfg = Release|Any CPU
		{E41F0471-B14D-4FA0-9D8B-1E7750695AE9}.Release|x64.Build.0 = Release|Any CPU
		{E41F0471-B14D-4FA0-9D8B-1E7750695AE9}.Release|x86.ActiveCfg = Release|Any CPU
		{E41F0471-B14D-4FA0-9D8B-1E7750695AE9}.Release|x86.Build.0 = Release|Any CPU
		{A54EE328-D456-4BAF-A180-84E77E6409AC}.Debug|Any CPU.ActiveCfg = Debug|Any CPU
		{A54EE328-D456-4BAF-A180-84E77E6409AC}.Debug|Any CPU.Build.0 = Debug|Any CPU
		{A54EE328-D456-4BAF-A180-84E77E6409AC}.Debug|x64.ActiveCfg = Debug|Any CPU
		{A54EE328-D456-4BAF-A180-84E77E6409AC}.Debug|x64.Build.0 = Debug|Any CPU
		{A54EE328-D456-4BAF-A180-84E77E6409AC}.Debug|x86.ActiveCfg = Debug|Any CPU
		{A54EE328-D456-4BAF-A180-84E77E6409AC}.Debug|x86.Build.0 = Debug|Any CPU
		{A54EE328-D456-4BAF-A180-84E77E6409AC}.Release|Any CPU.ActiveCfg = Release|Any CPU
		{A54EE328-D456-4BAF-A180-84E77E6409AC}.Release|Any CPU.Build.0 = Release|Any CPU
		{A54EE328-D456-4BAF-A180-84E77E6409AC}.Release|x64.ActiveCfg = Release|Any CPU
		{A54EE328-D456-4BAF-A180-84E77E6409AC}.Release|x64.Build.0 = Release|Any CPU
		{A54EE328-D456-4BAF-A180-84E77E6409AC}.Release|x86.ActiveCfg = Release|Any CPU
		{A54EE328-D456-4BAF-A180-84E77E6409AC}.Release|x86.Build.0 = Release|Any CPU
	EndGlobalSection
	GlobalSection(SolutionProperties) = preSolution
		HideSolutionNode = FALSE
	EndGlobalSection
	GlobalSection(NestedProjects) = preSolution
		{0BE8E56E-7580-4526-BE24-D304E1779724} = {E5B1EC71-0FC4-4FAA-9C65-32D5016FBC45}
		{F843CCCA-4CC9-422C-A881-3AE6A998B53F} = {E5B1EC71-0FC4-4FAA-9C65-32D5016FBC45}
		{E23C760E-B826-4B4F-BE76-916D86BAD2DB} = {E5B1EC71-0FC4-4FAA-9C65-32D5016FBC45}
		{E41F0471-B14D-4FA0-9D8B-1E7750695AE9} = {E5B1EC71-0FC4-4FAA-9C65-32D5016FBC45}
		{A54EE328-D456-4BAF-A180-84E77E6409AC} = {E5B1EC71-0FC4-4FAA-9C65-32D5016FBC45}
	EndGlobalSection
	GlobalSection(ExtensibilityGlobals) = postSolution
		SolutionGuid = {5C159F93-800B-49E7-9905-EE09F8B8434A}
	EndGlobalSection
EndGlobal



================================================
FILE: System.CommandLine.v3.ncrunchsolution
================================================
﻿<SolutionConfiguration>
  <Settings>
    <AllowParallelTestExecution>True</AllowParallelTestExecution>
    <CustomBuildProperties>
      <Value>TargetFrameworks = net8.0</Value>
      <Value>TargetFramework = net8.0</Value>
    </CustomBuildProperties>
    <EnableRDI>False</EnableRDI>
    <RdiConfigured>True</RdiConfigured>
    <SolutionConfigured>True</SolutionConfigured>
  </Settings>
</SolutionConfiguration>


================================================
FILE: .editorconfig
================================================

[*.{c,c++,cc,cp,cpp,cu,cuh,cxx,h,hh,hpp,hxx,inc,inl,ino,ipp,mpp,proto,tpp}]
indent_style=tab
indent_size=tab
tab_width=4

[*.{asax,ascx,aspx,cs,cshtml,css,htm,html,js,jsx,master,razor,skin,ts,tsx,vb,xaml,xamlx,xoml}]
indent_style=space
indent_size=4
tab_width=4

[*.{appxmanifest,build,config,csproj,dbml,discomap,dtd,json,jsproj,lsproj,njsproj,nuspec,proj,props,resjson,resw,resx,StyleCop,targets,tasks,vbproj,xml,xsd}]
indent_style=space
indent_size=2
tab_width=2

[*]

# Microsoft .NET properties
csharp_new_line_before_members_in_object_initializers=false
csharp_preferred_modifier_order=public, private, protected, internal, new, abstract, virtual, sealed, override, static, readonly, extern, unsafe, volatile, async:suggestion
csharp_style_var_elsewhere=true:hint
csharp_style_var_for_built_in_types=true:hint
csharp_style_var_when_type_is_apparent=true:hint
dotnet_style_predefined_type_for_locals_parameters_members=true:hint
dotnet_style_predefined_type_for_member_access=true:hint
dotnet_style_qualification_for_event=false:warning
dotnet_style_qualification_for_field=false:warning
dotnet_style_qualification_for_method=false:warning
dotnet_style_qualification_for_property=false:warning
dotnet_style_require_accessibility_modifiers=for_non_interface_members:hint



================================================
FILE: .vsts-ci-official.yml
================================================
variables:
  - name: _TeamName
    value: DotNetCore
  - name: _DotNetArtifactsCategory
    value: .NETCore
  - name: Codeql.Enabled
    value: true
  # CodeQL3000 needs this plumbed along as a variable to enable TSA.
  - name: Codeql.TSAEnabled
    value: true
  - name: Codeql.TSAOptionsPath
    value: '$(Build.SourcesDirectory)/.config/tsaoptions.json'

# CI and PR triggers
trigger:
  batch: true
  branches:
    include:
    - main
    - internal/release/*
    - validation/*

pr:
  autoCancel: false
  branches:
    include:
    - '*'

resources:
  repositories:
  - repository: 1ESPipelineTemplates
    type: git
    name: 1ESPipelineTemplates/1ESPipelineTemplates
    ref: refs/tags/release

extends:
  template: v1/1ES.Official.PipelineTemplate.yml@1ESPipelineTemplates
  parameters:
    pool:
      name: NetCore1ESPool-Svc-Internal
      image: 1es-windows-2022
      os: windows
    customBuildTags:
    - ES365AIMigrationTooling
    sdl:
      policheck:
        enabled: true
      tsa:
        enabled: true
    stages:
    - stage: build
      displayName: Build and Test
      jobs:
      - template: /eng/common/templates-official/jobs/jobs.yml@self
        parameters:
          enableMicrobuild: true
          enablePublishBuildArtifacts: true
          enablePublishUsingPipelines: true
          enablePublishTestResults: true
          enablePublishBuildAssets: true
          enableTelemetry: true
          enableSourceBuild: true
          helixRepo: dotnet/command-line-api
          timeoutInMinutes: 180 # increase timeout since BAR publishing might wait a long time
          jobs:
          - job: Windows
            pool:
              name: NetCore1ESPool-Internal
              demands: ImageOverride -equals windows.vs2022.amd64
            variables:
            - ${{ if notin(variables['Build.Reason'], 'PullRequest') }}:
              # Publish-Build-Assets provides: MaestroAccessToken, BotAccount-dotnet-maestro-bot-PAT
              - group: DotNet-Symbol-Server-Pats
              - group: Publish-Build-Assets
              - name: _OfficialBuildArgs
                value: /p:DotNetSignType=$(_SignType)
                      /p:TeamName=$(_TeamName)
                      /p:DotNetPublishUsingPipelines=$(_PublishUsingPipelines)
                      /p:DotNetArtifactsCategory=$(_DotNetArtifactsCategory)
                      /p:OfficialBuildId=$(BUILD.BUILDNUMBER)
                      /p:PublishToSymbolServer=true
                      /p:DotNetSymbolServerTokenMsdl=$(microsoft-symbol-server-pat)
                      /p:DotNetSymbolServerTokenSymWeb=$(symweb-symbol-server-pat)
              - name: _PublishUsingPipelines
                value: true
            # else
            - ${{ if in(variables['Build.Reason'], 'PullRequest') }}:
              - name: _OfficialBuildArgs
                value: ''
            strategy:
              matrix:
                ${{ if in(variables['Build.Reason'], 'PullRequest') }}:
                  Debug:
                    _BuildConfig: Debug
                    _SignType: test
                    _BuildArgs:

                Release:
                  _BuildConfig: Release
                  # PRs are not signed.
                  ${{ if in(variables['Build.Reason'], 'PullRequest') }}:
                    _SignType: test
                  ${{ if notin(variables['Build.Reason'], 'PullRequest') }}:
                    _SignType: real
                    _BuildArgs: $(_OfficialBuildArgs)
            templateContext:
              sdl:
                binskim:
                  analyzeTargetGlob: +:f|artifacts\bin\**\*.dll;+:f|artifacts\bin\**\*.exe;-:f|artifacts\bin\**\xunit*.dll;-:f|artifacts\bin\**\verify*.dll;
              outputs:
              - output: pipelineArtifact
                displayName: Upload package artifacts
                condition: and(eq(variables['system.pullrequest.isfork'], false), eq(variables['_BuildConfig'], 'Release'))
                targetPath: artifacts/packages/
                artifactName: artifacts
              - output: pipelineArtifact
                displayName: Publish Artifact Symbols
                condition: and(eq(variables['system.pullrequest.isfork'], false), eq(variables['_BuildConfig'], 'Release'))
                targetPath: '$(Build.SourcesDirectory)\artifacts\SymStore\$(_BuildConfig)'
                artifactName: 'NativeSymbols'
            # WORKAROUND: BinSkim requires the folder exist prior to scanning.
            preSteps:
            - powershell: New-Item -ItemType Directory -Path $(Build.SourcesDirectory)/artifacts/bin -Force
              displayName: Create artifacts/bin directory
            steps:
            - checkout: self
              clean: true
            - script: eng\common\cibuild.cmd
                -configuration $(_BuildConfig)
                -prepareMachine
                $(_BuildArgs)
              displayName: Build and Publish

          - job: Ubuntu
            displayName: Ubuntu
            pool:
              name: NetCore1ESPool-Svc-Internal
              demands: ImageOverride -equals 1es-ubuntu-2004
              os: linux
            strategy:
              matrix:
                ${{ if in(variables['Build.Reason'], 'PullRequest') }}:
                  Debug:
                    _BuildConfig: Debug
                    _SignType: none
                Release:
                  _BuildConfig: Release
                  _SignType: none
            steps:
            - checkout: self
              clean: true
            - bash: |
                wget -O - https://apt.llvm.org/llvm-snapshot.gpg.key | sudo apt-key add -
                sudo apt-add-repository "deb https://apt.llvm.org/focal/ llvm-toolchain-focal-9 main"
                sudo apt-get update
            - bash: |
                sudo apt-get install cmake clang-9 libicu66 uuid-dev libcurl4-openssl-dev zlib1g-dev libkrb5-dev
            - script: eng/common/cibuild.sh
                --configuration $(_BuildConfig)
                --prepareMachine
              displayName: Build

          - job: MacOS
            displayName: MacOS
            pool:
              name: Azure Pipelines
              image: macOS-latest
              os: macOS
            strategy:
              matrix:
                ${{ if in(variables['Build.Reason'], 'PullRequest') }}:
                  Debug:
                    _BuildConfig: Debug
                    _SignType: none
                    _DotNetPublishToBlobFeed: false
                Release:
                  _BuildConfig: Release
                  _SignType: none
                  _DotNetPublishToBlobFeed: false
            steps:
            - checkout: self
              clean: true
            - script: eng/common/cibuild.sh
                --configuration $(_BuildConfig)
                --prepareMachine
              displayName: Build

    - ${{ if notin(variables['Build.Reason'], 'PullRequest') }}:
      - template: /eng/common/templates-official/post-build/post-build.yml@self



================================================
FILE: .vsts-ci.yml
================================================
variables:
  - name: _TeamName
    value: DotNetCore
  - name: _DotNetArtifactsCategory
    value: .NETCore
  - name: Codeql.Enabled
    value: true

# CI and PR triggers
trigger:
  batch: true
  branches:
    include:
    - main

pr:
  autoCancel: false
  branches:
    include:
    - '*'

stages:
- stage: build
  displayName: Build and Test
  jobs:
  - template: /eng/common/templates/jobs/jobs.yml
    parameters:
      enableMicrobuild: true
      enablePublishBuildArtifacts: true
      enablePublishUsingPipelines: true
      enablePublishTestResults: true
      enablePublishBuildAssets: true
      enableTelemetry: true
      enableSourceBuild: true
      helixRepo: dotnet/command-line-api
      timeoutInMinutes: 180 # increase timeout since BAR publishing might wait a long time
      jobs:
      - job: Windows
        pool:
          name: NetCore-Public
          demands: ImageOverride -equals windows.vs2022.amd64.open
        variables:
        - name: _OfficialBuildArgs
          value: ''
        strategy:
          matrix:
            ${{ if in(variables['Build.Reason'], 'PullRequest') }}:
              Debug:
                _BuildConfig: Debug
                _SignType: test
                _BuildArgs:

            Release:
              _BuildConfig: Release
              _SignType: test
        steps:
        - checkout: self
          clean: true
        - script: eng\common\cibuild.cmd
            -configuration $(_BuildConfig)
            -prepareMachine
            $(_BuildArgs)
          displayName: Build and Publish
        - task: PublishBuildArtifacts@1
          displayName: Upload package artifacts
          condition: and(eq(variables['system.pullrequest.isfork'], false), eq(variables['_BuildConfig'], 'Release'))
          inputs:
            pathtoPublish: artifacts/packages/
            artifactName: artifacts
            artifactType: Container
            parallel: true
        - task: PublishBuildArtifacts@1
          displayName: Publish Artifact Symbols
          condition: and(eq(variables['system.pullrequest.isfork'], false), eq(variables['_BuildConfig'], 'Release'))
          inputs:
            PathtoPublish: '$(Build.SourcesDirectory)\artifacts\SymStore\$(_BuildConfig)'
            ArtifactName: 'NativeSymbols'

      - job: Ubuntu
        displayName: Ubuntu
        pool:
          name: NetCore-Svc-Public
          demands: ImageOverride -equals 1es-ubuntu-2004-open
        strategy:
          matrix:
            ${{ if in(variables['Build.Reason'], 'PullRequest') }}:
              Debug:
                _BuildConfig: Debug
                _SignType: none
            Release:
              _BuildConfig: Release
              _SignType: none
        steps:
        - checkout: self
          clean: true
        - bash: |
            wget -O - https://apt.llvm.org/llvm-snapshot.gpg.key | sudo apt-key add -
            sudo apt-add-repository "deb https://apt.llvm.org/focal/ llvm-toolchain-focal-9 main"
            sudo apt-get update
        - bash: |
            sudo apt-get install cmake clang-9 libicu66 uuid-dev libcurl4-openssl-dev zlib1g-dev libkrb5-dev
        - script: eng/common/cibuild.sh
            --configuration $(_BuildConfig)
            --prepareMachine
          displayName: Build

      - job: MacOS
        displayName: MacOS
        pool:
          vmImage: macOS-latest
        strategy:
          matrix:
            ${{ if in(variables['Build.Reason'], 'PullRequest') }}:
              Debug:
                _BuildConfig: Debug
                _SignType: none
                _DotNetPublishToBlobFeed : false
            Release:
              _BuildConfig: Release
              _SignType: none
              _DotNetPublishToBlobFeed : false
        steps:
        - checkout: self
          clean: true
        - script: eng/common/cibuild.sh
            --configuration $(_BuildConfig)
            --prepareMachine
          displayName: Build



================================================
FILE: docs/readme.md
================================================
The System.CommandLine documentation can now be found at [Microsoft Docs](https://docs.microsoft.com/en-us/dotnet/standard/commandline/).



================================================
FILE: docs/dotnet-suggest.md
================================================
# dotnet-suggest

Command line apps built using `System.CommandLine` have built-in support for tab completion.

![t-rex-suggestions](https://user-images.githubusercontent.com/547415/50387753-ef4c1280-06b8-11e9-90c8-89466d0bb406.gif)

On the machine where you'd like to enable completion, you'll need to do two things.

1. Install the `dotnet-suggest` global tool:

```sh
dotnet tool install -g dotnet-suggest
```

2. Install the completion script.

### bash
```sh
dotnet-suggest script bash >~/.dotnet-suggest-shim.bash
echo '. ~/.dotnet-suggest-shim.bash' >>~/.bashrc
```

### zsh
```sh
dotnet-suggest script zsh >~/.dotnet-suggest-shim.zsh
echo '. ~/.dotnet-suggest-shim.zsh' >>~/.zshrc
```

### PowerShell

Add the contents of [dotnet-suggest-shim.ps1](https://github.com/dotnet/command-line-api/blob/master/src/System.CommandLine.Suggest/dotnet-suggest-shim.ps1) to your PowerShell profile. You can find the expected path to your PowerShell profile by running the following in your console:

```console
> echo $profile
```

(For other shells, please [look for](https://github.com/dotnet/command-line-api/issues?q=is%3Aissue+is%3Aopen+label%3A%22shell+suggestion%22) or open an [issue](https://github.com/dotnet/command-line-api/issues).)



================================================
FILE: docs/Functional-goals.md
================================================
# Functional goals

The high level goals for `System.CommandLine` support our idea that creating great command line experiences for your users can be easy. We have not yet met all of these goals.

## Goals for the end user's experience

* Help should be clear and consistent
  * I should not have to know the right syntax to get help. Just make all variations work.
* Tab suggestion should just work with as little setup as possible.

## Goals for the programmer's experience

* Help

  * Creating some version of help should be automated, requiring no work.
  * Help should be informative if descriptions are supplied.
  * Help localization should be straightforward.

* Tab suggestion

  * It should just work with no effort on the programmer's part.
  * It should provide support for enums.
  * It should have a mechanism for dynamic values.
  * It should stay out of the way of shell suggestions for files and folders.
  * Dynamic suggestions should be extensible for other things I might do.

* Validation

  * If there are parse errors, it should fail before my application code is called.
  * It should check the number and type of arguments.
  * It should generally fail if there are unmatched tokens, but I should be able to allow it to pass through.
  * It should provide default responses for the user on validation issues.
  * I should be able to customize the validation messages.

* Debugging and testing

  * I should not have to turn a string into an array to interact programmatically.
  * I should be able to get a visualization of how a string is parsed.
  * It should be easy to test parsing in isolation from the application.
  * It should be easy to test the application in isolation from parsing.
  * I should be able to specify at the command line that I want to attach a debugger.

* Acting on parser results

  * Argument results should be strongly typed.
  * For advanced scenarios, I can alter and re-parse input.
  * It should be simple for me to manage exceptions, output, and exit codes.

* Rendering

  * Provide ways to reason about layout rather than just text.
  * Hide Windows/Linux/Mac differences for me.
  * Take advantage of new Windows 10 console capabilities.
  * Hide non-ANSI/ANSI differences for me.
  * Make output look correct when redirected to a file.

* Extensibility

  * I can compose cross-cutting behaviors using packages.




================================================
FILE: docs/History.md
================================================
# History

The new `System.CommandLine`'s lineage can be traced through the experiences of various teams at Microsoft building .NET command line applications. Some of its ideas have been expressed in the `dotnet` CLI  and `CommandLineUtils` originally created in ASP.NET with a [popular fork](https://github.com/natemcmaster/CommandLineUtils) by @natemcmaster.

This project is called the "new" `System.CommandLine` because Microsoft also had a `System.CommandLine` project in CoreFxLab that has been retired because it did not meet the current needs.

`System.CommandLine` is not a "Microsoft project." It is a community project with both Microsoft employees and community members as contributors. We've been working with folks on the CoreFx team so that we are aligned for inclusion in .NET Core if `System.CommandLine` meets the quality bar of the community and Microsoft. This relationship also allows us to work within the `dotnet` organization on GitHub. A few teams at Microsft have been early adopters, avoiding one-off parsers and trying to be consistent across `dotnet` CLI experiences.

The addition of global tools to the `dotnet` ecosystem meant the creation of more mini-CLIs. It is quite easy to set out to build a global tool and then spend more time building its CLI than on writing the code for the actual problem you were trying to solve. And if you aren't forward-looking, you can easily create a system where the functionality of the tool and the command line parsing cannot be separately tested.

Parsing is a deceptively complex problem. With folks on the team that have been involved in writing complex and successful CLIs, we can work in the other direction, focusing first on a solid core and then working outward toward the functionality and API surface. We're building the foundation that the folks who wrote and worked on the `dotnet` CLI wish they had been able to use. We ran this part of the project in private to ensure the core was solid, and as an all-volunteer effort this phase took painfully long.

The next layer, the API over the core functionality, has undergone a rewrite, and we are fairly happy with how you explicitly define your CLI. Explicitly defining a syntax feels like too much work for many scenarios and we've put a lot of thought and discussion into the idea of "app models" that infer the structure of your CLI from something that is natural to write.

App models have two aspects: defining the CLI's structure and bridging between parse results and your application.

As an example, one approach is to bind to a method, which is executed with parameters matching the options and arguments your user provided. This method binding works well when mapped one-to-one between the command and the invoked method. You can find this as the basis for the experimental "DragonFruit" model. DragonFruit takes this idea one step furher by wrapping your `Program.Main` entry point and just letting your `Main` method have normal parameters that just happen to be able to be of types other than `string`. We have not yet found a way we like to do subcommands with the DragonFruit model.

Other approaches to binding include binding to classes. A fundamental aspect of `System.CommandLine` is top-level support for app models and binders. These may reside outside `System.CommandLine` and we hope it will be a framework that people with other ideas can build on. The goal is that app models will interoperate with one another allowing many choices for programmers.

## Rendering

We've also done preliminary work on rendering. This is another area where `System.Console` is showing its age. In particular, `System.Console` does not supporting ANSI terminals easily. While `ncurses` has long addressed differing terminal capabilities in the non-Windows world, .NET programmers could benefit from something that works consistently on Windows, Linux, and Mac.

And with the new Windows Terminal and Windows 10 bringing [virtual terminal capabilities](https://blogs.msdn.microsoft.com/commandline/2018/06/27/windows-command-line-the-evolution-of-the-windows-command-line/) to the Windows console, we think there's an opportunity for .NET APIs that these benefits to users.




================================================
FILE: docs/Technical-motivations.md
================================================
# Technical motivations

* Provide a parser that's independent of binding and invocation.

  * You can create your own conventions and your own API surface.
  * Parsing can easily be tested independently from other application logic.
  * The syntax abstraction opens up use cases such as an extensible completions model.
  * Features such as syntax validation can be customized independent of your API.
  * Grammars can be serialized for interpretation by other tools.
  * Different APIs using this base layer can interoperate easily.
  * Don't always assume a console app entry point: provide `Main(string[])`-equivalent string splitting.

* Make the end user command line experience consistent and inclusive.

  * Support both POSIX and Windows syntax conventions.
  * Make help easy to find by defaulting into all common conventions (`-h`, `--help`, `/h` `/?`, `-?`).
  * Make completions work by default, so that they become the norm.
  * Make it possible to write completion providers for non-.NET command line applications.
  * Localization support for all messages that the library emits.
  * Parse diagramming, to help people understand a program's syntax without invoking it, is available by default.

* A composable chain of responsibility for subcommand routing, middleware, directives, etc.

  * An invocation model that allows for short-circuiting and interception, with access to the parser, meaning cross-cutting behaviors can be composed into your app via NuGet packages.
  * Simplify debugging by providing an interception hook in the middleware pipeline.
  * Support for handling process cancellation.
  * Directive syntax provides a consistent extensibility point that does not interfere with your app's syntax.
  * Supports command line API versioning via directives.

* Rich, adapative output rendering

  * Write output code once and render it correctly based on the presence or absence of a terminal as well as terminal capabilities.
  * Support for higher-level layouts, tables, event-based re-rendering, and animation.
  * Support for standard render mode hints via directives.

* Other things:

  * Support arbitrarily deep nesting of subcommands.
  * Support response files.
  * Restore console state after application exit.




================================================
FILE: eng/DotNetBuild.props
================================================
<!-- When altering this file, include @dotnet/product-construction as a reviewer. -->
<Project>

  <!-- TODO: Remove this file when command-line-api upgrades to Arcade 10 -->
  <PropertyGroup>
    <GitHubRepositoryName>command-line-api</GitHubRepositoryName>
    <SourceBuildManagedOnly>true</SourceBuildManagedOnly>
    <ReportPrebuiltUsage Condition="'$(DotNetBuildSourceOnly)' == 'true'">$(DotNetBuildFromVMR)</ReportPrebuiltUsage>
    <SetUpSourceBuildIntermediateNupkgCache>false</SetUpSourceBuildIntermediateNupkgCache>
    <CreateIntermediatePackage>false</CreateIntermediatePackage>
  </PropertyGroup>

</Project>



================================================
FILE: eng/Publishing.props
================================================
<Project>

  <PropertyGroup>
    <ProducesDotNetReleaseShippingAssets>true</ProducesDotNetReleaseShippingAssets>
  </PropertyGroup>

   <!-- Update all Artifacts with Kind=Package to have additional metadata item Category="LibraryPackage".
        This will mean that in VMR builds, command line api packages can get published to a different feed depending on
        the channel configuration -->
   <ItemGroup>
     <Artifact Update="@(Artifact->WithMetadataValue('Kind', 'Package'))" Category="LibraryPackage" />
   </ItemGroup>

</Project>



================================================
FILE: eng/Version.Details.xml
================================================
<?xml version="1.0" encoding="utf-8"?>
<Dependencies>
  <Source Uri="https://github.com/dotnet/dotnet" Mapping="command-line-api" Sha="445fb3a55b402cbe3a43576105e6fdc6686c8e4c" BarId="269352" />
  <ProductDependencies>
  </ProductDependencies>
  <ToolsetDependencies>
    <Dependency Name="Microsoft.DotNet.Arcade.Sdk" Version="9.0.0-beta.25302.2">
      <Uri>https://github.com/dotnet/arcade</Uri>
      <Sha>0d52a8b262d35fa2fde84e398cb2e791b8454bd2</Sha>
    </Dependency>
  </ToolsetDependencies>
</Dependencies>



================================================
FILE: eng/Versions.props
================================================
<Project>
  <!-- Repo Version Information -->
  <PropertyGroup>
    <VersionPrefix>2.0.0</VersionPrefix>
    <PreReleaseVersionLabel>beta7</PreReleaseVersionLabel>
    <AutoGenerateAssemblyVersion>false</AutoGenerateAssemblyVersion>
  </PropertyGroup>
</Project>



================================================
FILE: eng/common/README.md
================================================
# Don't touch this folder

                uuuuuuuuuuuuuuuuuuuu
              u" uuuuuuuuuuuuuuuuuu "u
            u" u$$$$$$$$$$$$$$$$$$$$u "u
          u" u$$$$$$$$$$$$$$$$$$$$$$$$u "u
        u" u$$$$$$$$$$$$$$$$$$$$$$$$$$$$u "u
      u" u$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$u "u
    u" u$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$u "u
    $ $$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$ $
    $ $$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$ $
    $ $$$" ... "$...  ...$" ... "$$$  ... "$$$ $
    $ $$$u `"$$$$$$$  $$$  $$$$$  $$  $$$  $$$ $
    $ $$$$$$uu "$$$$  $$$  $$$$$  $$  """ u$$$ $
    $ $$$""$$$  $$$$  $$$u "$$$" u$$  $$$$$$$$ $
    $ $$$$....,$$$$$..$$$$$....,$$$$..$$$$$$$$ $
    $ $$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$ $
    "u "$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$" u"
      "u "$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$" u"
        "u "$$$$$$$$$$$$$$$$$$$$$$$$$$$$" u"
          "u "$$$$$$$$$$$$$$$$$$$$$$$$" u"
            "u "$$$$$$$$$$$$$$$$$$$$" u"
              "u """""""""""""""""" u"
                """"""""""""""""""""

!!! Changes made in this directory are subject to being overwritten by automation !!!

The files in this directory are shared by all Arcade repos and managed by automation. If you need to make changes to these files, open an issue or submit a pull request to https://github.com/dotnet/arcade first.



================================================
FILE: eng/common/build.cmd
================================================
@echo off
powershell -ExecutionPolicy ByPass -NoProfile -command "& """%~dp0build.ps1""" %*"
exit /b %ErrorLevel%



================================================
FILE: eng/common/build.ps1
================================================
[CmdletBinding(PositionalBinding=$false)]
Param(
  [string][Alias('c')]$configuration = "Debug",
  [string]$platform = $null,
  [string] $projects,
  [string][Alias('v')]$verbosity = "minimal",
  [string] $msbuildEngine = $null,
  [bool] $warnAsError = $true,
  [bool] $nodeReuse = $true,
  [switch][Alias('r')]$restore,
  [switch] $deployDeps,
  [switch][Alias('b')]$build,
  [switch] $rebuild,
  [switch] $deploy,
  [switch][Alias('t')]$test,
  [switch] $integrationTest,
  [switch] $performanceTest,
  [switch] $sign,
  [switch] $pack,
  [switch] $publish,
  [switch] $clean,
  [switch][Alias('pb')]$productBuild,
  [switch][Alias('bl')]$binaryLog,
  [switch][Alias('nobl')]$excludeCIBinarylog,
  [switch] $ci,
  [switch] $prepareMachine,
  [string] $runtimeSourceFeed = '',
  [string] $runtimeSourceFeedKey = '',
  [switch] $excludePrereleaseVS,
  [switch] $nativeToolsOnMachine,
  [switch] $help,
  [Parameter(ValueFromRemainingArguments=$true)][String[]]$properties
)

# Unset 'Platform' environment variable to avoid unwanted collision in InstallDotNetCore.targets file
# some computer has this env var defined (e.g. Some HP)
if($env:Platform) {
  $env:Platform=""
}
function Print-Usage() {
  Write-Host "Common settings:"
  Write-Host "  -configuration <value>  Build configuration: 'Debug' or 'Release' (short: -c)"
  Write-Host "  -platform <value>       Platform configuration: 'x86', 'x64' or any valid Platform value to pass to msbuild"
  Write-Host "  -verbosity <value>      Msbuild verbosity: q[uiet], m[inimal], n[ormal], d[etailed], and diag[nostic] (short: -v)"
  Write-Host "  -binaryLog              Output binary log (short: -bl)"
  Write-Host "  -help                   Print help and exit"
  Write-Host ""

  Write-Host "Actions:"
  Write-Host "  -restore                Restore dependencies (short: -r)"
  Write-Host "  -build                  Build solution (short: -b)"
  Write-Host "  -rebuild                Rebuild solution"
  Write-Host "  -deploy                 Deploy built VSIXes"
  Write-Host "  -deployDeps             Deploy dependencies (e.g. VSIXes for integration tests)"
  Write-Host "  -test                   Run all unit tests in the solution (short: -t)"
  Write-Host "  -integrationTest        Run all integration tests in the solution"
  Write-Host "  -performanceTest        Run all performance tests in the solution"
  Write-Host "  -pack                   Package build outputs into NuGet packages and Willow components"
  Write-Host "  -sign                   Sign build outputs"
  Write-Host "  -publish                Publish artifacts (e.g. symbols)"
  Write-Host "  -clean                  Clean the solution"
  Write-Host "  -productBuild           Build the solution in the way it will be built in the full .NET product (VMR) build (short: -pb)"
  Write-Host ""

  Write-Host "Advanced settings:"
  Write-Host "  -projects <value>       Semi-colon delimited list of sln/proj's to build. Globbing is supported (*.sln)"
  Write-Host "  -ci                     Set when running on CI server"
  Write-Host "  -excludeCIBinarylog     Don't output binary log (short: -nobl)"
  Write-Host "  -prepareMachine         Prepare machine for CI run, clean up processes after build"
  Write-Host "  -warnAsError <value>    Sets warnaserror msbuild parameter ('true' or 'false')"
  Write-Host "  -msbuildEngine <value>  Msbuild engine to use to run build ('dotnet', 'vs', or unspecified)."
  Write-Host "  -excludePrereleaseVS    Set to exclude build engines in prerelease versions of Visual Studio"
  Write-Host "  -nativeToolsOnMachine   Sets the native tools on machine environment variable (indicating that the script should use native tools on machine)"
  Write-Host ""

  Write-Host "Command line arguments not listed above are passed thru to msbuild."
  Write-Host "The above arguments can be shortened as much as to be unambiguous (e.g. -co for configuration, -t for test, etc.)."
}

. $PSScriptRoot\tools.ps1

function InitializeCustomToolset {
  if (-not $restore) {
    return
  }

  $script = Join-Path $EngRoot 'restore-toolset.ps1'

  if (Test-Path $script) {
    . $script
  }
}

function Build {
  $toolsetBuildProj = InitializeToolset
  InitializeCustomToolset

  $bl = if ($binaryLog) { '/bl:' + (Join-Path $LogDir 'Build.binlog') } else { '' }
  $platformArg = if ($platform) { "/p:Platform=$platform" } else { '' }

  if ($projects) {
    # Re-assign properties to a new variable because PowerShell doesn't let us append properties directly for unclear reasons.
    # Explicitly set the type as string[] because otherwise PowerShell would make this char[] if $properties is empty.
    [string[]] $msbuildArgs = $properties

    # Resolve relative project paths into full paths
    $projects = ($projects.Split(';').ForEach({Resolve-Path $_}) -join ';')

    $msbuildArgs += "/p:Projects=$projects"
    $properties = $msbuildArgs
  }

  MSBuild $toolsetBuildProj `
    $bl `
    $platformArg `
    /p:Configuration=$configuration `
    /p:RepoRoot=$RepoRoot `
    /p:Restore=$restore `
    /p:DeployDeps=$deployDeps `
    /p:Build=$build `
    /p:Rebuild=$rebuild `
    /p:Deploy=$deploy `
    /p:Test=$test `
    /p:Pack=$pack `
    /p:DotNetBuildRepo=$productBuild `
    /p:IntegrationTest=$integrationTest `
    /p:PerformanceTest=$performanceTest `
    /p:Sign=$sign `
    /p:Publish=$publish `
    @properties
}

try {
  if ($clean) {
    if (Test-Path $ArtifactsDir) {
      Remove-Item -Recurse -Force $ArtifactsDir
      Write-Host 'Artifacts directory deleted.'
    }
    exit 0
  }

  if ($help -or (($null -ne $properties) -and ($properties.Contains('/help') -or $properties.Contains('/?')))) {
    Print-Usage
    exit 0
  }

  if ($ci) {
    if (-not $excludeCIBinarylog) {
      $binaryLog = $true
    }
    $nodeReuse = $false
  }

  if ($nativeToolsOnMachine) {
    $env:NativeToolsOnMachine = $true
  }
  if ($restore) {
    InitializeNativeTools
  }

  Build
}
catch {
  Write-Host $_.ScriptStackTrace
  Write-PipelineTelemetryError -Category 'InitializeToolset' -Message $_
  ExitWithExitCode 1
}

ExitWithExitCode 0



================================================
FILE: eng/common/build.sh
================================================
#!/usr/bin/env bash

# Stop script if unbound variable found (use ${var:-} if intentional)
set -u

# Stop script if command returns non-zero exit code.
# Prevents hidden errors caused by missing error code propagation.
set -e

usage()
{
  echo "Common settings:"
  echo "  --configuration <value>    Build configuration: 'Debug' or 'Release' (short: -c)"
  echo "  --verbosity <value>        Msbuild verbosity: q[uiet], m[inimal], n[ormal], d[etailed], and diag[nostic] (short: -v)"
  echo "  --binaryLog                Create MSBuild binary log (short: -bl)"
  echo "  --help                     Print help and exit (short: -h)"
  echo ""

  echo "Actions:"
  echo "  --restore                  Restore dependencies (short: -r)"
  echo "  --build                    Build solution (short: -b)"
  echo "  --sourceBuild              Source-build the solution (short: -sb)"
  echo "                             Will additionally trigger the following actions: --restore, --build, --pack"
  echo "                             If --configuration is not set explicitly, will also set it to 'Release'"
  echo "  --productBuild             Build the solution in the way it will be built in the full .NET product (VMR) build (short: -pb)"
  echo "                             Will additionally trigger the following actions: --restore, --build, --pack"
  echo "                             If --configuration is not set explicitly, will also set it to 'Release'"
  echo "  --rebuild                  Rebuild solution"
  echo "  --test                     Run all unit tests in the solution (short: -t)"
  echo "  --integrationTest          Run all integration tests in the solution"
  echo "  --performanceTest          Run all performance tests in the solution"
  echo "  --pack                     Package build outputs into NuGet packages and Willow components"
  echo "  --sign                     Sign build outputs"
  echo "  --publish                  Publish artifacts (e.g. symbols)"
  echo "  --clean                    Clean the solution"
  echo ""

  echo "Advanced settings:"
  echo "  --projects <value>       Project or solution file(s) to build"
  echo "  --ci                     Set when running on CI server"
  echo "  --excludeCIBinarylog     Don't output binary log (short: -nobl)"
  echo "  --prepareMachine         Prepare machine for CI run, clean up processes after build"
  echo "  --nodeReuse <value>      Sets nodereuse msbuild parameter ('true' or 'false')"
  echo "  --warnAsError <value>    Sets warnaserror msbuild parameter ('true' or 'false')"
  echo ""
  echo "Command line arguments not listed above are passed thru to msbuild."
  echo "Arguments can also be passed in with a single hyphen."
}

source="${BASH_SOURCE[0]}"

# resolve $source until the file is no longer a symlink
while [[ -h "$source" ]]; do
  scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"
  source="$(readlink "$source")"
  # if $source was a relative symlink, we need to resolve it relative to the path where the
  # symlink file was located
  [[ $source != /* ]] && source="$scriptroot/$source"
done
scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"

restore=false
build=false
source_build=false
product_build=false
rebuild=false
test=false
integration_test=false
performance_test=false
pack=false
publish=false
sign=false
public=false
ci=false
clean=false

warn_as_error=true
node_reuse=true
binary_log=false
exclude_ci_binary_log=false
pipelines_log=false

projects=''
configuration=''
prepare_machine=false
verbosity='minimal'
runtime_source_feed=''
runtime_source_feed_key=''

properties=''
while [[ $# > 0 ]]; do
  opt="$(echo "${1/#--/-}" | tr "[:upper:]" "[:lower:]")"
  case "$opt" in
    -help|-h)
      usage
      exit 0
      ;;
    -clean)
      clean=true
      ;;
    -configuration|-c)
      configuration=$2
      shift
      ;;
    -verbosity|-v)
      verbosity=$2
      shift
      ;;
    -binarylog|-bl)
      binary_log=true
      ;;
    -excludecibinarylog|-nobl)
      exclude_ci_binary_log=true
      ;;
    -pipelineslog|-pl)
      pipelines_log=true
      ;;
    -restore|-r)
      restore=true
      ;;
    -build|-b)
      build=true
      ;;
    -rebuild)
      rebuild=true
      ;;
    -pack)
      pack=true
      ;;
    -sourcebuild|-sb)
      build=true
      source_build=true
      product_build=true
      restore=true
      pack=true
      ;;
    -productBuild|-pb)
      build=true
      product_build=true
      restore=true
      pack=true
      ;;
    -test|-t)
      test=true
      ;;
    -integrationtest)
      integration_test=true
      ;;
    -performancetest)
      performance_test=true
      ;;
    -sign)
      sign=true
      ;;
    -publish)
      publish=true
      ;;
    -preparemachine)
      prepare_machine=true
      ;;
    -projects)
      projects=$2
      shift
      ;;
    -ci)
      ci=true
      ;;
    -warnaserror)
      warn_as_error=$2
      shift
      ;;
    -nodereuse)
      node_reuse=$2
      shift
      ;;
    -runtimesourcefeed)
      runtime_source_feed=$2
      shift
      ;;
     -runtimesourcefeedkey)
      runtime_source_feed_key=$2
      shift
      ;;
    *)
      properties="$properties $1"
      ;;
  esac

  shift
done

if [[ -z "$configuration" ]]; then
  if [[ "$source_build" = true ]]; then configuration="Release"; else configuration="Debug"; fi
fi

if [[ "$ci" == true ]]; then
  pipelines_log=true
  node_reuse=false
  if [[ "$exclude_ci_binary_log" == false ]]; then
    binary_log=true
  fi
fi

. "$scriptroot/tools.sh"

function InitializeCustomToolset {
  local script="$eng_root/restore-toolset.sh"

  if [[ -a "$script" ]]; then
    . "$script"
  fi
}

function Build {
  InitializeToolset
  InitializeCustomToolset

  if [[ ! -z "$projects" ]]; then
    properties="$properties /p:Projects=$projects"
  fi

  local bl=""
  if [[ "$binary_log" == true ]]; then
    bl="/bl:\"$log_dir/Build.binlog\""
  fi

  MSBuild $_InitializeToolset \
    $bl \
    /p:Configuration=$configuration \
    /p:RepoRoot="$repo_root" \
    /p:Restore=$restore \
    /p:Build=$build \
    /p:DotNetBuildRepo=$product_build \
    /p:ArcadeBuildFromSource=$source_build \
    /p:DotNetBuildSourceOnly=$source_build \
    /p:Rebuild=$rebuild \
    /p:Test=$test \
    /p:Pack=$pack \
    /p:IntegrationTest=$integration_test \
    /p:PerformanceTest=$performance_test \
    /p:Sign=$sign \
    /p:Publish=$publish \
    $properties

  ExitWithExitCode 0
}

if [[ "$clean" == true ]]; then
  if [ -d "$artifacts_dir" ]; then
    rm -rf $artifacts_dir
    echo "Artifacts directory deleted."
  fi
  exit 0
fi

if [[ "$restore" == true ]]; then
  InitializeNativeTools
fi

Build



================================================
FILE: eng/common/CIBuild.cmd
================================================
@echo off
powershell -ExecutionPolicy ByPass -NoProfile -command "& """%~dp0Build.ps1""" -restore -build -test -sign -pack -publish -ci %*"


================================================
FILE: eng/common/cibuild.sh
================================================
#!/usr/bin/env bash

source="${BASH_SOURCE[0]}"

# resolve $SOURCE until the file is no longer a symlink
while [[ -h $source ]]; do
  scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"
  source="$(readlink "$source")"

  # if $source was a relative symlink, we need to resolve it relative to the path where
  # the symlink file was located
  [[ $source != /* ]] && source="$scriptroot/$source"
done
scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"

. "$scriptroot/build.sh" --restore --build --test --pack --publish --ci $@


================================================
FILE: eng/common/darc-init.ps1
================================================
param (
    $darcVersion = $null,
    $versionEndpoint = 'https://maestro.dot.net/api/assets/darc-version?api-version=2020-02-20',
    $verbosity = 'minimal',
    $toolpath = $null
)

. $PSScriptRoot\tools.ps1

function InstallDarcCli ($darcVersion, $toolpath) {
  $darcCliPackageName = 'microsoft.dotnet.darc'

  $dotnetRoot = InitializeDotNetCli -install:$true
  $dotnet = "$dotnetRoot\dotnet.exe"
  $toolList = & "$dotnet" tool list -g

  if ($toolList -like "*$darcCliPackageName*") {
    & "$dotnet" tool uninstall $darcCliPackageName -g
  }

  # If the user didn't explicitly specify the darc version,
  # query the Maestro API for the correct version of darc to install.
  if (-not $darcVersion) {
    $darcVersion = $(Invoke-WebRequest -Uri $versionEndpoint -UseBasicParsing).Content
  }

  $arcadeServicesSource = 'https://pkgs.dev.azure.com/dnceng/public/_packaging/dotnet-eng/nuget/v3/index.json'

  Write-Host "Installing Darc CLI version $darcVersion..."
  Write-Host 'You may need to restart your command window if this is the first dotnet tool you have installed.'
  if (-not $toolpath) {
    Write-Host "'$dotnet' tool install $darcCliPackageName --version $darcVersion --add-source '$arcadeServicesSource' -v $verbosity -g"
    & "$dotnet" tool install $darcCliPackageName --version $darcVersion --add-source "$arcadeServicesSource" -v $verbosity -g
  }else {
    Write-Host "'$dotnet' tool install $darcCliPackageName --version $darcVersion --add-source '$arcadeServicesSource' -v $verbosity --tool-path '$toolpath'"
    & "$dotnet" tool install $darcCliPackageName --version $darcVersion --add-source "$arcadeServicesSource" -v $verbosity --tool-path "$toolpath"
  }
}

try {
  InstallDarcCli $darcVersion $toolpath
}
catch {
  Write-Host $_.ScriptStackTrace
  Write-PipelineTelemetryError -Category 'Darc' -Message $_
  ExitWithExitCode 1
}


================================================
FILE: eng/common/darc-init.sh
================================================
#!/usr/bin/env bash

source="${BASH_SOURCE[0]}"
darcVersion=''
versionEndpoint='https://maestro.dot.net/api/assets/darc-version?api-version=2020-02-20'
verbosity='minimal'

while [[ $# > 0 ]]; do
  opt="$(echo "$1" | tr "[:upper:]" "[:lower:]")"
  case "$opt" in
    --darcversion)
      darcVersion=$2
      shift
      ;;
    --versionendpoint)
      versionEndpoint=$2
      shift
      ;;
    --verbosity)
      verbosity=$2
      shift
      ;;
    --toolpath)
      toolpath=$2
      shift
      ;;
    *)
      echo "Invalid argument: $1"
      usage
      exit 1
      ;;
  esac

  shift
done

# resolve $source until the file is no longer a symlink
while [[ -h "$source" ]]; do
  scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"
  source="$(readlink "$source")"
  # if $source was a relative symlink, we need to resolve it relative to the path where the
  # symlink file was located
  [[ $source != /* ]] && source="$scriptroot/$source"
done
scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"

. "$scriptroot/tools.sh"

if [ -z "$darcVersion" ]; then
  darcVersion=$(curl -X GET "$versionEndpoint" -H "accept: text/plain")
fi

function InstallDarcCli {
  local darc_cli_package_name="microsoft.dotnet.darc"

  InitializeDotNetCli true
  local dotnet_root=$_InitializeDotNetCli

  if [ -z "$toolpath" ]; then
    local tool_list=$($dotnet_root/dotnet tool list -g)
    if [[ $tool_list = *$darc_cli_package_name* ]]; then
      echo $($dotnet_root/dotnet tool uninstall $darc_cli_package_name -g)
    fi
  else
    local tool_list=$($dotnet_root/dotnet tool list --tool-path "$toolpath")
    if [[ $tool_list = *$darc_cli_package_name* ]]; then
      echo $($dotnet_root/dotnet tool uninstall $darc_cli_package_name --tool-path "$toolpath")
    fi
  fi

  local arcadeServicesSource="https://pkgs.dev.azure.com/dnceng/public/_packaging/dotnet-tools/nuget/v3/index.json"

  echo "Installing Darc CLI version $darcVersion..."
  echo "You may need to restart your command shell if this is the first dotnet tool you have installed."
  if [ -z "$toolpath" ]; then
    echo $($dotnet_root/dotnet tool install $darc_cli_package_name --version $darcVersion --add-source "$arcadeServicesSource" -v $verbosity -g)
  else
    echo $($dotnet_root/dotnet tool install $darc_cli_package_name --version $darcVersion --add-source "$arcadeServicesSource" -v $verbosity --tool-path "$toolpath")
  fi
}

InstallDarcCli



================================================
FILE: eng/common/dotnet-install.cmd
================================================
@echo off
powershell -ExecutionPolicy ByPass -NoProfile -command "& """%~dp0dotnet-install.ps1""" %*"


================================================
FILE: eng/common/dotnet-install.ps1
================================================
[CmdletBinding(PositionalBinding=$false)]
Param(
  [string] $verbosity = 'minimal',
  [string] $architecture = '',
  [string] $version = 'Latest',
  [string] $runtime = 'dotnet',
  [string] $RuntimeSourceFeed = '',
  [string] $RuntimeSourceFeedKey = ''
)

. $PSScriptRoot\tools.ps1

$dotnetRoot = Join-Path $RepoRoot '.dotnet'

$installdir = $dotnetRoot
try {
    if ($architecture -and $architecture.Trim() -eq 'x86') {
        $installdir = Join-Path $installdir 'x86'
    }
    InstallDotNet $installdir $version $architecture $runtime $true -RuntimeSourceFeed $RuntimeSourceFeed -RuntimeSourceFeedKey $RuntimeSourceFeedKey
}
catch {
  Write-Host $_.ScriptStackTrace
  Write-PipelineTelemetryError -Category 'InitializeToolset' -Message $_
  ExitWithExitCode 1
}

ExitWithExitCode 0



================================================
FILE: eng/common/dotnet-install.sh
================================================
#!/usr/bin/env bash

source="${BASH_SOURCE[0]}"
# resolve $source until the file is no longer a symlink
while [[ -h "$source" ]]; do
  scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"
  source="$(readlink "$source")"
  # if $source was a relative symlink, we need to resolve it relative to the path where the
  # symlink file was located
  [[ $source != /* ]] && source="$scriptroot/$source"
done
scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"

. "$scriptroot/tools.sh"

version='Latest'
architecture=''
runtime='dotnet'
runtimeSourceFeed=''
runtimeSourceFeedKey=''
while [[ $# > 0 ]]; do
  opt="$(echo "$1" | tr "[:upper:]" "[:lower:]")"
  case "$opt" in
    -version|-v)
      shift
      version="$1"
      ;;
    -architecture|-a)
      shift
      architecture="$1"
      ;;
    -runtime|-r)
      shift
      runtime="$1"
      ;;
    -runtimesourcefeed)
      shift
      runtimeSourceFeed="$1"
      ;;
    -runtimesourcefeedkey)
      shift
      runtimeSourceFeedKey="$1"
      ;;
    *)
      Write-PipelineTelemetryError -Category 'Build' -Message "Invalid argument: $1"
      exit 1
      ;;
  esac
  shift
done

# Use uname to determine what the CPU is, see https://en.wikipedia.org/wiki/Uname#Examples
cpuname=$(uname -m)
case $cpuname in
  arm64|aarch64)
    buildarch=arm64
    if [ "$(getconf LONG_BIT)" -lt 64 ]; then
        # This is 32-bit OS running on 64-bit CPU (for example Raspberry Pi OS)
        buildarch=arm
    fi
    ;;
  loongarch64)
    buildarch=loongarch64
    ;;
  amd64|x86_64)
    buildarch=x64
    ;;
  armv*l)
    buildarch=arm
    ;;
  i[3-6]86)
    buildarch=x86
    ;;
  riscv64)
    buildarch=riscv64
    ;;
  *)
    echo "Unknown CPU $cpuname detected, treating it as x64"
    buildarch=x64
    ;;
esac

dotnetRoot="${repo_root}.dotnet"
if [[ $architecture != "" ]] && [[ $architecture != $buildarch ]]; then
  dotnetRoot="$dotnetRoot/$architecture"
fi

InstallDotNet "$dotnetRoot" $version "$architecture" $runtime true $runtimeSourceFeed $runtimeSourceFeedKey || {
  local exit_code=$?
  Write-PipelineTelemetryError -Category 'InitializeToolset' -Message "dotnet-install.sh failed (exit code '$exit_code')." >&2
  ExitWithExitCode $exit_code
}

ExitWithExitCode 0



================================================
FILE: eng/common/enable-cross-org-publishing.ps1
================================================
param(
  [string] $token
)


. $PSScriptRoot\pipeline-logging-functions.ps1

# Write-PipelineSetVariable will no-op if a variable named $ci is not defined
# Since this script is only ever called in AzDO builds, just universally set it
$ci = $true

Write-PipelineSetVariable -Name 'VSS_NUGET_ACCESSTOKEN' -Value $token -IsMultiJobVariable $false
Write-PipelineSetVariable -Name 'VSS_NUGET_URI_PREFIXES' -Value 'https://dnceng.pkgs.visualstudio.com/;https://pkgs.dev.azure.com/dnceng/;https://devdiv.pkgs.visualstudio.com/;https://pkgs.dev.azure.com/devdiv/' -IsMultiJobVariable $false



================================================
FILE: eng/common/generate-locproject.ps1
================================================
Param(
    [Parameter(Mandatory=$true)][string] $SourcesDirectory,     # Directory where source files live; if using a Localize directory it should live in here
    [string] $LanguageSet = 'VS_Main_Languages',                # Language set to be used in the LocProject.json
    [switch] $UseCheckedInLocProjectJson,                       # When set, generates a LocProject.json and compares it to one that already exists in the repo; otherwise just generates one
    [switch] $CreateNeutralXlfs                                 # Creates neutral xlf files. Only set to false when running locally
)

# Generates LocProject.json files for the OneLocBuild task. OneLocBuildTask is described here:
# https://ceapex.visualstudio.com/CEINTL/_wiki/wikis/CEINTL.wiki/107/Localization-with-OneLocBuild-Task

Set-StrictMode -Version 2.0
$ErrorActionPreference = "Stop"
. $PSScriptRoot\pipeline-logging-functions.ps1

$exclusionsFilePath = "$SourcesDirectory\eng\Localize\LocExclusions.json"
$exclusions = @{ Exclusions = @() }
if (Test-Path -Path $exclusionsFilePath)
{
    $exclusions = Get-Content "$exclusionsFilePath" | ConvertFrom-Json
}

Push-Location "$SourcesDirectory" # push location for Resolve-Path -Relative to work

# Template files
$jsonFiles = @()
$jsonTemplateFiles = Get-ChildItem -Recurse -Path "$SourcesDirectory" | Where-Object { $_.FullName -Match "\.template\.config\\localize\\.+\.en\.json" } # .NET templating pattern
$jsonTemplateFiles | ForEach-Object {
    $null = $_.Name -Match "(.+)\.[\w-]+\.json" # matches '[filename].[langcode].json

    $destinationFile = "$($_.Directory.FullName)\$($Matches.1).json"
    $jsonFiles += Copy-Item "$($_.FullName)" -Destination $destinationFile -PassThru
}

$jsonWinformsTemplateFiles = Get-ChildItem -Recurse -Path "$SourcesDirectory" | Where-Object { $_.FullName -Match "en\\strings\.json" } # current winforms pattern

$wxlFiles = Get-ChildItem -Recurse -Path "$SourcesDirectory" | Where-Object { $_.FullName -Match "\\.+\.wxl" -And -Not( $_.Directory.Name -Match "\d{4}" ) } # localized files live in four digit lang ID directories; this excludes them
if (-not $wxlFiles) {
    $wxlEnFiles = Get-ChildItem -Recurse -Path "$SourcesDirectory" | Where-Object { $_.FullName -Match "\\1033\\.+\.wxl" } #  pick up en files (1033 = en) specifically so we can copy them to use as the neutral xlf files
    if ($wxlEnFiles) {
      $wxlFiles = @()
      $wxlEnFiles | ForEach-Object {
        $destinationFile = "$($_.Directory.Parent.FullName)\$($_.Name)"
        $wxlFiles += Copy-Item "$($_.FullName)" -Destination $destinationFile -PassThru
      }
    }
}

$macosHtmlEnFiles = Get-ChildItem -Recurse -Path "$SourcesDirectory" | Where-Object { $_.FullName -Match "en\.lproj\\.+\.html$" } # add installer HTML files
$macosHtmlFiles = @()
if ($macosHtmlEnFiles) {
    $macosHtmlEnFiles | ForEach-Object {
        $destinationFile = "$($_.Directory.Parent.FullName)\$($_.Name)"
        $macosHtmlFiles += Copy-Item "$($_.FullName)" -Destination $destinationFile -PassThru
    }
}

$xlfFiles = @()

$allXlfFiles = Get-ChildItem -Recurse -Path "$SourcesDirectory\*\*.xlf"
$langXlfFiles = @()
if ($allXlfFiles) {
    $null = $allXlfFiles[0].FullName -Match "\.([\w-]+)\.xlf" # matches '[langcode].xlf'
    $firstLangCode = $Matches.1
    $langXlfFiles = Get-ChildItem -Recurse -Path "$SourcesDirectory\*\*.$firstLangCode.xlf"
}
$langXlfFiles | ForEach-Object {
    $null = $_.Name -Match "(.+)\.[\w-]+\.xlf" # matches '[filename].[langcode].xlf

    $destinationFile = "$($_.Directory.FullName)\$($Matches.1).xlf"
    $xlfFiles += Copy-Item "$($_.FullName)" -Destination $destinationFile -PassThru
}

$locFiles = $jsonFiles + $jsonWinformsTemplateFiles + $xlfFiles

$locJson = @{
    Projects = @(
        @{
            LanguageSet = $LanguageSet
            LocItems = @(
                $locFiles | ForEach-Object {
                    $outputPath = "$(($_.DirectoryName | Resolve-Path -Relative) + "\")"
                    $continue = $true
                    foreach ($exclusion in $exclusions.Exclusions) {
                        if ($_.FullName.Contains($exclusion))
                        {
                            $continue = $false
                        }
                    }
                    $sourceFile = ($_.FullName | Resolve-Path -Relative)
                    if (!$CreateNeutralXlfs -and $_.Extension -eq '.xlf') {
                        Remove-Item -Path $sourceFile
                    }
                    if ($continue)
                    {
                        if ($_.Directory.Name -eq 'en' -and $_.Extension -eq '.json') {
                            return @{
                                SourceFile = $sourceFile
                                CopyOption = "LangIDOnPath"
                                OutputPath = "$($_.Directory.Parent.FullName | Resolve-Path -Relative)\"
                            }
                        } else {
                            return @{
                                SourceFile = $sourceFile
                                CopyOption = "LangIDOnName"
                                OutputPath = $outputPath
                            }
                        }
                    }
                }
            )
        },
        @{
            LanguageSet = $LanguageSet
            CloneLanguageSet = "WiX_CloneLanguages"
            LssFiles = @( "wxl_loc.lss" )
            LocItems = @(
                $wxlFiles | ForEach-Object {
                    $outputPath = "$($_.Directory.FullName | Resolve-Path -Relative)\"
                    $continue = $true
                    foreach ($exclusion in $exclusions.Exclusions) {
                        if ($_.FullName.Contains($exclusion)) {
                            $continue = $false
                        }
                    }
                    $sourceFile = ($_.FullName | Resolve-Path -Relative)
                    if ($continue)
                    {
                        return @{
                            SourceFile = $sourceFile
                            CopyOption = "LangIDOnPath"
                            OutputPath = $outputPath
                        }
                    }
                }
            )
        },
        @{
            LanguageSet = $LanguageSet
            CloneLanguageSet = "VS_macOS_CloneLanguages"
            LssFiles = @( ".\eng\common\loc\P22DotNetHtmlLocalization.lss" )
            LocItems = @(
                $macosHtmlFiles | ForEach-Object {
                    $outputPath = "$($_.Directory.FullName | Resolve-Path -Relative)\"
                    $continue = $true
                    foreach ($exclusion in $exclusions.Exclusions) {
                        if ($_.FullName.Contains($exclusion)) {
                            $continue = $false
                        }
                    }
                    $sourceFile = ($_.FullName | Resolve-Path -Relative)
                    $lciFile = $sourceFile + ".lci"
                    if ($continue) {
                        $result = @{
                            SourceFile = $sourceFile
                            CopyOption = "LangIDOnPath"
                            OutputPath = $outputPath
                        }
                        if (Test-Path $lciFile -PathType Leaf) {
                            $result["LciFile"] = $lciFile
                        }
                        return $result
                    }
                }
            )
        }
    )
}

$json = ConvertTo-Json $locJson -Depth 5
Write-Host "LocProject.json generated:`n`n$json`n`n"
Pop-Location

if (!$UseCheckedInLocProjectJson) {
    New-Item "$SourcesDirectory\eng\Localize\LocProject.json" -Force # Need this to make sure the Localize directory is created
    Set-Content "$SourcesDirectory\eng\Localize\LocProject.json" $json
}
else {
    New-Item "$SourcesDirectory\eng\Localize\LocProject-generated.json" -Force # Need this to make sure the Localize directory is created
    Set-Content "$SourcesDirectory\eng\Localize\LocProject-generated.json" $json

    if ((Get-FileHash "$SourcesDirectory\eng\Localize\LocProject-generated.json").Hash -ne (Get-FileHash "$SourcesDirectory\eng\Localize\LocProject.json").Hash) {
        Write-PipelineTelemetryError -Category "OneLocBuild" -Message "Existing LocProject.json differs from generated LocProject.json. Download LocProject-generated.json and compare them."

        exit 1
    }
    else {
        Write-Host "Generated LocProject.json and current LocProject.json are identical."
    }
}



================================================
FILE: eng/common/generate-sbom-prep.ps1
================================================
Param(
    [Parameter(Mandatory=$true)][string] $ManifestDirPath    # Manifest directory where sbom will be placed
)

. $PSScriptRoot\pipeline-logging-functions.ps1

# Normally - we'd listen to the manifest path given, but 1ES templates will overwrite if this level gets uploaded directly
# with their own overwriting ours. So we create it as a sub directory of the requested manifest path.
$ArtifactName = "${env:SYSTEM_STAGENAME}_${env:AGENT_JOBNAME}_SBOM"
$SafeArtifactName = $ArtifactName -replace '["/:<>\\|?@*"() ]', '_'
$SbomGenerationDir = Join-Path $ManifestDirPath $SafeArtifactName

Write-Host "Artifact name before : $ArtifactName"
Write-Host "Artifact name after : $SafeArtifactName"

Write-Host "Creating dir $ManifestDirPath"

# create directory for sbom manifest to be placed
if (!(Test-Path -path $SbomGenerationDir))
{
  New-Item -ItemType Directory -path $SbomGenerationDir
  Write-Host "Successfully created directory $SbomGenerationDir"
}
else{
  Write-PipelineTelemetryError -category 'Build'  "Unable to create sbom folder."
}

Write-Host "Updating artifact name"
Write-Host "##vso[task.setvariable variable=ARTIFACT_NAME]$SafeArtifactName"



================================================
FILE: eng/common/generate-sbom-prep.sh
================================================
#!/usr/bin/env bash

source="${BASH_SOURCE[0]}"

# resolve $SOURCE until the file is no longer a symlink
while [[ -h $source ]]; do
  scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"
  source="$(readlink "$source")"

  # if $source was a relative symlink, we need to resolve it relative to the path where the
  # symlink file was located
  [[ $source != /* ]] && source="$scriptroot/$source"
done
scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"
. $scriptroot/pipeline-logging-functions.sh


# replace all special characters with _, some builds use special characters like : in Agent.Jobname, that is not a permissible name while uploading artifacts.
artifact_name=$SYSTEM_STAGENAME"_"$AGENT_JOBNAME"_SBOM"
safe_artifact_name="${artifact_name//["/:<>\\|?@*$" ]/_}"
manifest_dir=$1

# Normally - we'd listen to the manifest path given, but 1ES templates will overwrite if this level gets uploaded directly
# with their own overwriting ours. So we create it as a sub directory of the requested manifest path.
sbom_generation_dir="$manifest_dir/$safe_artifact_name"

if [ ! -d "$sbom_generation_dir" ] ; then
  mkdir -p "$sbom_generation_dir"
  echo "Sbom directory created." $sbom_generation_dir
else
  Write-PipelineTelemetryError -category 'Build'  "Unable to create sbom folder."
fi

echo "Artifact name before : "$artifact_name
echo "Artifact name after : "$safe_artifact_name
export ARTIFACT_NAME=$safe_artifact_name
echo "##vso[task.setvariable variable=ARTIFACT_NAME]$safe_artifact_name"

exit 0



================================================
FILE: eng/common/helixpublish.proj
================================================
<!-- Licensed to the .NET Foundation under one or more agreements. The .NET Foundation licenses this file to you under the MIT license. -->
<Project Sdk="Microsoft.DotNet.Helix.Sdk" DefaultTargets="Test">

  <PropertyGroup>
    <Language>msbuild</Language>
  </PropertyGroup>

  <ItemGroup>
    <HelixCorrelationPayload Include="$(CorrelationPayloadDirectory)">
      <PayloadDirectory>%(Identity)</PayloadDirectory>
    </HelixCorrelationPayload>
  </ItemGroup>

  <ItemGroup>
    <HelixWorkItem Include="WorkItem" Condition="'$(WorkItemDirectory)' != ''">
      <PayloadDirectory>$(WorkItemDirectory)</PayloadDirectory>
      <Command>$(WorkItemCommand)</Command>
      <Timeout Condition="'$(WorkItemTimeout)' != ''">$(WorkItemTimeout)</Timeout>
    </HelixWorkItem>
  </ItemGroup>

  <ItemGroup>
    <XUnitProject Include="$(XUnitProjects.Split(';'))">
      <Arguments />
    </XUnitProject>
  </ItemGroup>
</Project>



================================================
FILE: eng/common/init-tools-native.cmd
================================================
@echo off
powershell -NoProfile -NoLogo -ExecutionPolicy ByPass -command "& """%~dp0init-tools-native.ps1""" %*"
exit /b %ErrorLevel%


================================================
FILE: eng/common/init-tools-native.ps1
================================================
<#
.SYNOPSIS
Entry point script for installing native tools

.DESCRIPTION
Reads $RepoRoot\global.json file to determine native assets to install
and executes installers for those tools

.PARAMETER BaseUri
Base file directory or Url from which to acquire tool archives

.PARAMETER InstallDirectory
Directory to install native toolset.  This is a command-line override for the default
Install directory precedence order:
- InstallDirectory command-line override
- NETCOREENG_INSTALL_DIRECTORY environment variable
- (default) %USERPROFILE%/.netcoreeng/native

.PARAMETER Clean
Switch specifying to not install anything, but cleanup native asset folders

.PARAMETER Force
Clean and then install tools

.PARAMETER DownloadRetries
Total number of retry attempts

.PARAMETER RetryWaitTimeInSeconds
Wait time between retry attempts in seconds

.PARAMETER GlobalJsonFile
File path to global.json file

.PARAMETER PathPromotion
Optional switch to enable either promote native tools specified in the global.json to the path (in Azure Pipelines)
or break the build if a native tool is not found on the path (on a local dev machine)

.NOTES
#>
[CmdletBinding(PositionalBinding=$false)]
Param (
  [string] $BaseUri = 'https://netcorenativeassets.blob.core.windows.net/resource-packages/external',
  [string] $InstallDirectory,
  [switch] $Clean = $False,
  [switch] $Force = $False,
  [int] $DownloadRetries = 5,
  [int] $RetryWaitTimeInSeconds = 30,
  [string] $GlobalJsonFile,
  [switch] $PathPromotion
)

if (!$GlobalJsonFile) {
  $GlobalJsonFile = Join-Path (Get-Item $PSScriptRoot).Parent.Parent.FullName 'global.json'
}

Set-StrictMode -version 2.0
$ErrorActionPreference='Stop'

. $PSScriptRoot\pipeline-logging-functions.ps1
Import-Module -Name (Join-Path $PSScriptRoot 'native\CommonLibrary.psm1')

try {
  # Define verbose switch if undefined
  $Verbose = $VerbosePreference -Eq 'Continue'

  $EngCommonBaseDir = Join-Path $PSScriptRoot 'native\'
  $NativeBaseDir = $InstallDirectory
  if (!$NativeBaseDir) {
    $NativeBaseDir = CommonLibrary\Get-NativeInstallDirectory
  }
  $Env:CommonLibrary_NativeInstallDir = $NativeBaseDir
  $InstallBin = Join-Path $NativeBaseDir 'bin'
  $InstallerPath = Join-Path $EngCommonBaseDir 'install-tool.ps1'

  # Process tools list
  Write-Host "Processing $GlobalJsonFile"
  If (-Not (Test-Path $GlobalJsonFile)) {
    Write-Host "Unable to find '$GlobalJsonFile'"
    exit 0
  }
  $NativeTools = Get-Content($GlobalJsonFile) -Raw |
                    ConvertFrom-Json |
                    Select-Object -Expand 'native-tools' -ErrorAction SilentlyContinue
  if ($NativeTools) {
    if ($PathPromotion -eq $True) {
      $ArcadeToolsDirectory = "$env:SYSTEMDRIVE\arcade-tools"
      if (Test-Path $ArcadeToolsDirectory) { # if this directory exists, we should use native tools on machine
        $NativeTools.PSObject.Properties | ForEach-Object {
          $ToolName = $_.Name
          $ToolVersion = $_.Value
          $InstalledTools = @{}

          if ((Get-Command "$ToolName" -ErrorAction SilentlyContinue) -eq $null) {
            if ($ToolVersion -eq "latest") {
              $ToolVersion = ""
            }
            $ToolDirectories = (Get-ChildItem -Path "$ArcadeToolsDirectory" -Filter "$ToolName-$ToolVersion*" | Sort-Object -Descending)
            if ($ToolDirectories -eq $null) {
              Write-Error "Unable to find directory for $ToolName $ToolVersion; please make sure the tool is installed on this image."
              exit 1
            }
            $ToolDirectory = $ToolDirectories[0]
            $BinPathFile = "$($ToolDirectory.FullName)\binpath.txt"
            if (-not (Test-Path -Path "$BinPathFile")) {
              Write-Error "Unable to find binpath.txt in '$($ToolDirectory.FullName)' ($ToolName $ToolVersion); artifact is either installed incorrectly or is not a bootstrappable tool."
              exit 1
            }
            $BinPath = Get-Content "$BinPathFile"
            $ToolPath = Convert-Path -Path $BinPath
            Write-Host "Adding $ToolName to the path ($ToolPath)..."
            Write-Host "##vso[task.prependpath]$ToolPath"
            $env:PATH = "$ToolPath;$env:PATH"
            $InstalledTools += @{ $ToolName = $ToolDirectory.FullName }
          }
        }
        return $InstalledTools
      } else {
        $NativeTools.PSObject.Properties | ForEach-Object {
          $ToolName = $_.Name
          $ToolVersion = $_.Value

          if ((Get-Command "$ToolName" -ErrorAction SilentlyContinue) -eq $null) {
            Write-PipelineTelemetryError -Category 'NativeToolsBootstrap' -Message "$ToolName not found on path. Please install $ToolName $ToolVersion before proceeding."
            Write-PipelineTelemetryError -Category 'NativeToolsBootstrap' -Message "If this is running on a build machine, the arcade-tools directory was not found, which means there's an error with the image."
          }
        }
        exit 0
      }
    } else {
      $NativeTools.PSObject.Properties | ForEach-Object {
        $ToolName = $_.Name
        $ToolVersion = $_.Value
        $LocalInstallerArguments =  @{ ToolName = "$ToolName" }
        $LocalInstallerArguments += @{ InstallPath = "$InstallBin" }
        $LocalInstallerArguments += @{ BaseUri = "$BaseUri" }
        $LocalInstallerArguments += @{ CommonLibraryDirectory = "$EngCommonBaseDir" }
        $LocalInstallerArguments += @{ Version = "$ToolVersion" }

        if ($Verbose) {
          $LocalInstallerArguments += @{ Verbose = $True }
        }
        if (Get-Variable 'Force' -ErrorAction 'SilentlyContinue') {
          if($Force) {
            $LocalInstallerArguments += @{ Force = $True }
          }
        }
        if ($Clean) {
          $LocalInstallerArguments += @{ Clean = $True }
        }

        Write-Verbose "Installing $ToolName version $ToolVersion"
        Write-Verbose "Executing '$InstallerPath $($LocalInstallerArguments.Keys.ForEach({"-$_ '$($LocalInstallerArguments.$_)'"}) -join ' ')'"
        & $InstallerPath @LocalInstallerArguments
        if ($LASTEXITCODE -Ne "0") {
          $errMsg = "$ToolName installation failed"
          if ((Get-Variable 'DoNotAbortNativeToolsInstallationOnFailure' -ErrorAction 'SilentlyContinue') -and $DoNotAbortNativeToolsInstallationOnFailure) {
              $showNativeToolsWarning = $true
              if ((Get-Variable 'DoNotDisplayNativeToolsInstallationWarnings' -ErrorAction 'SilentlyContinue') -and $DoNotDisplayNativeToolsInstallationWarnings) {
                  $showNativeToolsWarning = $false
              }
              if ($showNativeToolsWarning) {
                  Write-Warning $errMsg
              }
              $toolInstallationFailure = $true
          } else {
              # We cannot change this to Write-PipelineTelemetryError because of https://github.com/dotnet/arcade/issues/4482
              Write-Host $errMsg
              exit 1
          }
        }
      }

      if ((Get-Variable 'toolInstallationFailure' -ErrorAction 'SilentlyContinue') -and $toolInstallationFailure) {
          # We cannot change this to Write-PipelineTelemetryError because of https://github.com/dotnet/arcade/issues/4482
          Write-Host 'Native tools bootstrap failed'
          exit 1
      }
    }
  }
  else {
    Write-Host 'No native tools defined in global.json'
    exit 0
  }

  if ($Clean) {
    exit 0
  }
  if (Test-Path $InstallBin) {
    Write-Host 'Native tools are available from ' (Convert-Path -Path $InstallBin)
    Write-Host "##vso[task.prependpath]$(Convert-Path -Path $InstallBin)"
    return $InstallBin
  }
  elseif (-not ($PathPromotion)) {
    Write-PipelineTelemetryError -Category 'NativeToolsBootstrap' -Message 'Native tools install directory does not exist, installation failed'
    exit 1
  }
  exit 0
}
catch {
  Write-Host $_.ScriptStackTrace
  Write-PipelineTelemetryError -Category 'NativeToolsBootstrap' -Message $_
  ExitWithExitCode 1
}



================================================
FILE: eng/common/init-tools-native.sh
================================================
#!/usr/bin/env bash

source="${BASH_SOURCE[0]}"
scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"

base_uri='https://netcorenativeassets.blob.core.windows.net/resource-packages/external'
install_directory=''
clean=false
force=false
download_retries=5
retry_wait_time_seconds=30
global_json_file="$(dirname "$(dirname "${scriptroot}")")/global.json"
declare -a native_assets

. $scriptroot/pipeline-logging-functions.sh
. $scriptroot/native/common-library.sh

while (($# > 0)); do
  lowerI="$(echo $1 | tr "[:upper:]" "[:lower:]")"
  case $lowerI in
    --baseuri)
      base_uri=$2
      shift 2
      ;;
    --installdirectory)
      install_directory=$2
      shift 2
      ;;
    --clean)
      clean=true
      shift 1
      ;;
    --force)
      force=true
      shift 1
      ;;
    --donotabortonfailure)
      donotabortonfailure=true
      shift 1
      ;;
    --donotdisplaywarnings)
      donotdisplaywarnings=true
      shift 1
      ;;
    --downloadretries)
      download_retries=$2
      shift 2
      ;;
    --retrywaittimeseconds)
      retry_wait_time_seconds=$2
      shift 2
      ;;
    --help)
      echo "Common settings:"
      echo "  --installdirectory                  Directory to install native toolset."
      echo "                                      This is a command-line override for the default"
      echo "                                      Install directory precedence order:"
      echo "                                          - InstallDirectory command-line override"
      echo "                                          - NETCOREENG_INSTALL_DIRECTORY environment variable"
      echo "                                          - (default) %USERPROFILE%/.netcoreeng/native"
      echo ""
      echo "  --clean                             Switch specifying not to install anything, but cleanup native asset folders"
      echo "  --donotabortonfailure               Switch specifiying whether to abort native tools installation on failure"
      echo "  --donotdisplaywarnings              Switch specifiying whether to display warnings during native tools installation on failure"
      echo "  --force                             Clean and then install tools"
      echo "  --help                              Print help and exit"
      echo ""
      echo "Advanced settings:"
      echo "  --baseuri <value>                   Base URI for where to download native tools from"
      echo "  --downloadretries <value>           Number of times a download should be attempted"
      echo "  --retrywaittimeseconds <value>      Wait time between download attempts"
      echo ""
      exit 0
      ;;
  esac
done

function ReadGlobalJsonNativeTools {
  # happy path: we have a proper JSON parsing tool `jq(1)` in PATH!
  if command -v jq &> /dev/null; then

    # jq: read each key/value pair under "native-tools" entry and emit:
    #   KEY="<entry-key>" VALUE="<entry-value>"
    # followed by a null byte.
    #
    # bash: read line with null byte delimeter and push to array (for later `eval`uation).

    while IFS= read -rd '' line; do
      native_assets+=("$line")
    done < <(jq -r '. |
        select(has("native-tools")) |
        ."native-tools" |
        keys[] as $k |
        @sh "KEY=\($k) VALUE=\(.[$k])\u0000"' "$global_json_file")

    return
  fi

  # Warning: falling back to manually parsing JSON, which is not recommended.

  # Following routine matches the output and escaping logic of jq(1)'s @sh formatter used above.
  # It has been tested with several weird strings with escaped characters in entries (key and value)
  # and results were compared with the output of jq(1) in binary representation using xxd(1);
  # just before the assignment to 'native_assets' array (above and below).

  # try to capture the section under "native-tools".
  if [[ ! "$(cat "$global_json_file")" =~ \"native-tools\"[[:space:]\:\{]*([^\}]+) ]]; then
    return
  fi

  section="${BASH_REMATCH[1]}"

  parseStarted=0
  possibleEnd=0
  escaping=0
  escaped=0
  isKey=1

  for (( i=0; i<${#section}; i++ )); do
    char="${section:$i:1}"
    if ! ((parseStarted)) && [[ "$char" =~ [[:space:],:] ]]; then continue; fi

    if ! ((escaping)) && [[ "$char" == "\\" ]]; then
      escaping=1
    elif ((escaping)) && ! ((escaped)); then
      escaped=1
    fi

    if ! ((parseStarted)) && [[ "$char" == "\"" ]]; then
      parseStarted=1
      possibleEnd=0
    elif [[ "$char" == "'" ]]; then
      token="$token'\\\''"
      possibleEnd=0
    elif ((escaping)) || [[ "$char" != "\"" ]]; then
      token="$token$char"
      possibleEnd=1
    fi

    if ((possibleEnd)) && ! ((escaping)) && [[ "$char" == "\"" ]]; then
      # Use printf to unescape token to match jq(1)'s @sh formatting rules.
      # do not use 'token="$(printf "$token")"' syntax, as $() eats the trailing linefeed.
      printf -v token "'$token'"

      if ((isKey)); then
        KEY="$token"
        isKey=0
      else
        line="KEY=$KEY VALUE=$token"
        native_assets+=("$line")
        isKey=1
      fi

      # reset for next token
      parseStarted=0
      token=
    elif ((escaping)) && ((escaped)); then
      escaping=0
      escaped=0
    fi
  done
}

native_base_dir=$install_directory
if [[ -z $install_directory ]]; then
  native_base_dir=$(GetNativeInstallDirectory)
fi

install_bin="${native_base_dir}/bin"
installed_any=false

ReadGlobalJsonNativeTools

if [[ ${#native_assets[@]} -eq 0 ]]; then
  echo "No native tools defined in global.json"
  exit 0;
else
  native_installer_dir="$scriptroot/native"
  for index in "${!native_assets[@]}"; do
    eval "${native_assets["$index"]}"

    installer_path="$native_installer_dir/install-$KEY.sh"
    installer_command="$installer_path"
    installer_command+=" --baseuri $base_uri"
    installer_command+=" --installpath $install_bin"
    installer_command+=" --version $VALUE"
    echo $installer_command

    if [[ $force = true ]]; then
      installer_command+=" --force"
    fi

    if [[ $clean = true ]]; then
      installer_command+=" --clean"
    fi

    if [[ -a $installer_path ]]; then
      $installer_command
      if [[ $? != 0 ]]; then
        if [[ $donotabortonfailure = true ]]; then
          if [[ $donotdisplaywarnings != true ]]; then
            Write-PipelineTelemetryError -category 'NativeToolsBootstrap' "Execution Failed"
          fi
        else
          Write-PipelineTelemetryError -category 'NativeToolsBootstrap' "Execution Failed"
          exit 1
        fi
      else
        $installed_any = true
      fi
    else
      if [[ $donotabortonfailure == true ]]; then
        if [[ $donotdisplaywarnings != true ]]; then
          Write-PipelineTelemetryError -category 'NativeToolsBootstrap' "Execution Failed: no install script"
        fi
      else
        Write-PipelineTelemetryError -category 'NativeToolsBootstrap' "Execution Failed: no install script"
        exit 1
      fi
    fi
  done
fi

if [[ $clean = true ]]; then
  exit 0
fi

if [[ -d $install_bin ]]; then
  echo "Native tools are available from $install_bin"
  echo "##vso[task.prependpath]$install_bin"
else
  if [[ $installed_any = true ]]; then
    Write-PipelineTelemetryError -category 'NativeToolsBootstrap' "Native tools install directory does not exist, installation failed"
    exit 1
  fi
fi

exit 0



================================================
FILE: eng/common/internal-feed-operations.ps1
================================================
param(
  [Parameter(Mandatory=$true)][string] $Operation,
  [string] $AuthToken,
  [string] $CommitSha,
  [string] $RepoName,
  [switch] $IsFeedPrivate
)

$ErrorActionPreference = 'Stop'
Set-StrictMode -Version 2.0
. $PSScriptRoot\tools.ps1

# Sets VSS_NUGET_EXTERNAL_FEED_ENDPOINTS based on the "darc-int-*" feeds defined in NuGet.config. This is needed
# in build agents by CredProvider to authenticate the restore requests to internal feeds as specified in
# https://github.com/microsoft/artifacts-credprovider/blob/0f53327cd12fd893d8627d7b08a2171bf5852a41/README.md#environment-variables. This should ONLY be called from identified
# internal builds
function SetupCredProvider {
  param(
    [string] $AuthToken
  )

  # Install the Cred Provider NuGet plugin
  Write-Host 'Setting up Cred Provider NuGet plugin in the agent...'
  Write-Host "Getting 'installcredprovider.ps1' from 'https://github.com/microsoft/artifacts-credprovider'..."

  $url = 'https://raw.githubusercontent.com/microsoft/artifacts-credprovider/master/helpers/installcredprovider.ps1'

  Write-Host "Writing the contents of 'installcredprovider.ps1' locally..."
  Invoke-WebRequest $url -OutFile installcredprovider.ps1

  Write-Host 'Installing plugin...'
  .\installcredprovider.ps1 -Force

  Write-Host "Deleting local copy of 'installcredprovider.ps1'..."
  Remove-Item .\installcredprovider.ps1

  if (-Not("$env:USERPROFILE\.nuget\plugins\netcore")) {
    Write-PipelineTelemetryError -Category 'Arcade' -Message 'CredProvider plugin was not installed correctly!'
    ExitWithExitCode 1
  }
  else {
    Write-Host 'CredProvider plugin was installed correctly!'
  }

  # Then, we set the 'VSS_NUGET_EXTERNAL_FEED_ENDPOINTS' environment variable to restore from the stable
  # feeds successfully

  $nugetConfigPath = Join-Path $RepoRoot "NuGet.config"

  if (-Not (Test-Path -Path $nugetConfigPath)) {
    Write-PipelineTelemetryError -Category 'Build' -Message 'NuGet.config file not found in repo root!'
    ExitWithExitCode 1
  }

  $endpoints = New-Object System.Collections.ArrayList
  $nugetConfigPackageSources = Select-Xml -Path $nugetConfigPath -XPath "//packageSources/add[contains(@key, 'darc-int-')]/@value" | foreach{$_.Node.Value}

  if (($nugetConfigPackageSources | Measure-Object).Count -gt 0 ) {
    foreach ($stableRestoreResource in $nugetConfigPackageSources) {
      $trimmedResource = ([string]$stableRestoreResource).Trim()
      [void]$endpoints.Add(@{endpoint="$trimmedResource"; password="$AuthToken"})
    }
  }

  if (($endpoints | Measure-Object).Count -gt 0) {
      $endpointCredentials = @{endpointCredentials=$endpoints} | ConvertTo-Json -Compress

     # Create the environment variables the AzDo way
      Write-LoggingCommand -Area 'task' -Event 'setvariable' -Data $endpointCredentials -Properties @{
        'variable' = 'VSS_NUGET_EXTERNAL_FEED_ENDPOINTS'
        'issecret' = 'false'
      }

      # We don't want sessions cached since we will be updating the endpoints quite frequently
      Write-LoggingCommand -Area 'task' -Event 'setvariable' -Data 'False' -Properties @{
        'variable' = 'NUGET_CREDENTIALPROVIDER_SESSIONTOKENCACHE_ENABLED'
        'issecret' = 'false'
      }
  }
  else
  {
    Write-Host 'No internal endpoints found in NuGet.config'
  }
}

#Workaround for https://github.com/microsoft/msbuild/issues/4430
function InstallDotNetSdkAndRestoreArcade {
  $dotnetTempDir = Join-Path $RepoRoot "dotnet"
  $dotnetSdkVersion="2.1.507" # After experimentation we know this version works when restoring the SDK (compared to 3.0.*)
  $dotnet = "$dotnetTempDir\dotnet.exe"
  $restoreProjPath = "$PSScriptRoot\restore.proj"

  Write-Host "Installing dotnet SDK version $dotnetSdkVersion to restore Arcade SDK..."
  InstallDotNetSdk "$dotnetTempDir" "$dotnetSdkVersion"

  '<Project Sdk="Microsoft.DotNet.Arcade.Sdk"/>' | Out-File "$restoreProjPath"

  & $dotnet restore $restoreProjPath

  Write-Host 'Arcade SDK restored!'

  if (Test-Path -Path $restoreProjPath) {
    Remove-Item $restoreProjPath
  }

  if (Test-Path -Path $dotnetTempDir) {
    Remove-Item $dotnetTempDir -Recurse
  }
}

try {
  Push-Location $PSScriptRoot

  if ($Operation -like 'setup') {
    SetupCredProvider $AuthToken
  }
  elseif ($Operation -like 'install-restore') {
    InstallDotNetSdkAndRestoreArcade
  }
  else {
    Write-PipelineTelemetryError -Category 'Arcade' -Message "Unknown operation '$Operation'!"
    ExitWithExitCode 1
  }
}
catch {
  Write-Host $_.ScriptStackTrace
  Write-PipelineTelemetryError -Category 'Arcade' -Message $_
  ExitWithExitCode 1
}
finally {
  Pop-Location
}



================================================
FILE: eng/common/internal-feed-operations.sh
================================================
#!/usr/bin/env bash

set -e

# Sets VSS_NUGET_EXTERNAL_FEED_ENDPOINTS based on the "darc-int-*" feeds defined in NuGet.config. This is needed
# in build agents by CredProvider to authenticate the restore requests to internal feeds as specified in
# https://github.com/microsoft/artifacts-credprovider/blob/0f53327cd12fd893d8627d7b08a2171bf5852a41/README.md#environment-variables.
# This should ONLY be called from identified internal builds
function SetupCredProvider {
  local authToken=$1

  # Install the Cred Provider NuGet plugin
  echo "Setting up Cred Provider NuGet plugin in the agent..."...
  echo "Getting 'installcredprovider.ps1' from 'https://github.com/microsoft/artifacts-credprovider'..."

  local url="https://raw.githubusercontent.com/microsoft/artifacts-credprovider/master/helpers/installcredprovider.sh"

  echo "Writing the contents of 'installcredprovider.ps1' locally..."
  local installcredproviderPath="installcredprovider.sh"
  if command -v curl > /dev/null; then
    curl $url > "$installcredproviderPath"
  else
    wget -q -O "$installcredproviderPath" "$url"
  fi

  echo "Installing plugin..."
  . "$installcredproviderPath"

  echo "Deleting local copy of 'installcredprovider.sh'..."
  rm installcredprovider.sh

  if [ ! -d "$HOME/.nuget/plugins" ]; then
    Write-PipelineTelemetryError -category 'Build' 'CredProvider plugin was not installed correctly!'
    ExitWithExitCode 1
  else
    echo "CredProvider plugin was installed correctly!"
  fi

  # Then, we set the 'VSS_NUGET_EXTERNAL_FEED_ENDPOINTS' environment variable to restore from the stable
  # feeds successfully

  local nugetConfigPath="{$repo_root}NuGet.config"

  if [ ! "$nugetConfigPath" ]; then
    Write-PipelineTelemetryError -category 'Build' "NuGet.config file not found in repo's root!"
    ExitWithExitCode 1
  fi

  local endpoints='['
  local nugetConfigPackageValues=`cat "$nugetConfigPath" | grep "key=\"darc-int-"`
  local pattern="value=\"(.*)\""

  for value in $nugetConfigPackageValues
  do
    if [[ $value =~ $pattern ]]; then
      local endpoint="${BASH_REMATCH[1]}"
      endpoints+="{\"endpoint\": \"$endpoint\", \"password\": \"$authToken\"},"
    fi
  done

  endpoints=${endpoints%?}
  endpoints+=']'

  if [ ${#endpoints} -gt 2 ]; then
      local endpointCredentials="{\"endpointCredentials\": "$endpoints"}"

      echo "##vso[task.setvariable variable=VSS_NUGET_EXTERNAL_FEED_ENDPOINTS]$endpointCredentials"
      echo "##vso[task.setvariable variable=NUGET_CREDENTIALPROVIDER_SESSIONTOKENCACHE_ENABLED]False"
  else
    echo "No internal endpoints found in NuGet.config"
  fi
}

# Workaround for https://github.com/microsoft/msbuild/issues/4430
function InstallDotNetSdkAndRestoreArcade {
  local dotnetTempDir="$repo_root/dotnet"
  local dotnetSdkVersion="2.1.507" # After experimentation we know this version works when restoring the SDK (compared to 3.0.*)
  local restoreProjPath="$repo_root/eng/common/restore.proj"

  echo "Installing dotnet SDK version $dotnetSdkVersion to restore Arcade SDK..."
  echo "<Project Sdk=\"Microsoft.DotNet.Arcade.Sdk\"/>" > "$restoreProjPath"

  InstallDotNetSdk "$dotnetTempDir" "$dotnetSdkVersion"

  local res=`$dotnetTempDir/dotnet restore $restoreProjPath`
  echo "Arcade SDK restored!"

  # Cleanup
  if [ "$restoreProjPath" ]; then
    rm "$restoreProjPath"
  fi

  if [ "$dotnetTempDir" ]; then
    rm -r $dotnetTempDir
  fi
}

source="${BASH_SOURCE[0]}"
operation=''
authToken=''
repoName=''

while [[ $# > 0 ]]; do
  opt="$(echo "$1" | tr "[:upper:]" "[:lower:]")"
  case "$opt" in
    --operation)
      operation=$2
      shift
      ;;
    --authtoken)
      authToken=$2
      shift
      ;;
    *)
      echo "Invalid argument: $1"
      usage
      exit 1
      ;;
  esac

  shift
done

while [[ -h "$source" ]]; do
  scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"
  source="$(readlink "$source")"
  # if $source was a relative symlink, we need to resolve it relative to the path where the
  # symlink file was located
  [[ $source != /* ]] && source="$scriptroot/$source"
done
scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"

. "$scriptroot/tools.sh"

if [ "$operation" = "setup" ]; then
  SetupCredProvider $authToken
elif [ "$operation" = "install-restore" ]; then
  InstallDotNetSdkAndRestoreArcade
else
  echo "Unknown operation '$operation'!"
fi



================================================
FILE: eng/common/msbuild.ps1
================================================
[CmdletBinding(PositionalBinding=$false)]
Param(
  [string] $verbosity = 'minimal',
  [bool] $warnAsError = $true,
  [bool] $nodeReuse = $true,
  [switch] $ci,
  [switch] $prepareMachine,
  [switch] $excludePrereleaseVS,
  [string] $msbuildEngine = $null,
  [Parameter(ValueFromRemainingArguments=$true)][String[]]$extraArgs
)

. $PSScriptRoot\tools.ps1

try {
  if ($ci) {
    $nodeReuse = $false
  }

  MSBuild @extraArgs
}
catch {
  Write-Host $_.ScriptStackTrace
  Write-PipelineTelemetryError -Category 'Build' -Message $_
  ExitWithExitCode 1
}

ExitWithExitCode 0


================================================
FILE: eng/common/msbuild.sh
================================================
#!/usr/bin/env bash

source="${BASH_SOURCE[0]}"

# resolve $source until the file is no longer a symlink
while [[ -h "$source" ]]; do
  scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"
  source="$(readlink "$source")"
  # if $source was a relative symlink, we need to resolve it relative to the path where the
  # symlink file was located
  [[ $source != /* ]] && source="$scriptroot/$source"
done
scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"

verbosity='minimal'
warn_as_error=true
node_reuse=true
prepare_machine=false
extra_args=''

while (($# > 0)); do
  lowerI="$(echo $1 | tr "[:upper:]" "[:lower:]")"
  case $lowerI in
    --verbosity)
      verbosity=$2
      shift 2
      ;;
    --warnaserror)
      warn_as_error=$2
      shift 2
      ;;
    --nodereuse)
      node_reuse=$2
      shift 2
      ;;
    --ci)
      ci=true
      shift 1
      ;;
    --preparemachine)
      prepare_machine=true
      shift 1
      ;;
      *)
      extra_args="$extra_args $1"
      shift 1
      ;;
  esac
done

. "$scriptroot/tools.sh"

if [[ "$ci" == true ]]; then
  node_reuse=false
fi

MSBuild $extra_args
ExitWithExitCode 0



================================================
FILE: eng/common/pipeline-logging-functions.ps1
================================================
# Source for this file was taken from https://github.com/microsoft/azure-pipelines-task-lib/blob/11c9439d4af17e6475d9fe058e6b2e03914d17e6/powershell/VstsTaskSdk/LoggingCommandFunctions.ps1 and modified.

# NOTE: You should not be calling these method directly as they are likely to change.  Instead you should be calling the Write-Pipeline* functions defined in tools.ps1

$script:loggingCommandPrefix = '##vso['
$script:loggingCommandEscapeMappings = @( # TODO: WHAT ABOUT "="? WHAT ABOUT "%"?
    New-Object psobject -Property @{ Token = ';' ; Replacement = '%3B' }
    New-Object psobject -Property @{ Token = "`r" ; Replacement = '%0D' }
    New-Object psobject -Property @{ Token = "`n" ; Replacement = '%0A' }
    New-Object psobject -Property @{ Token = "]" ; Replacement = '%5D' }
)
# TODO: BUG: Escape % ???
# TODO: Add test to verify don't need to escape "=".

# Specify "-Force" to force pipeline formatted output even if "$ci" is false or not set
function Write-PipelineTelemetryError {
    [CmdletBinding()]
    param(
        [Parameter(Mandatory = $true)]
        [string]$Category,
        [Parameter(Mandatory = $true)]
        [string]$Message,
        [Parameter(Mandatory = $false)]
        [string]$Type = 'error',
        [string]$ErrCode,
        [string]$SourcePath,
        [string]$LineNumber,
        [string]$ColumnNumber,
        [switch]$AsOutput,
        [switch]$Force)

    $PSBoundParameters.Remove('Category') | Out-Null

    if ($Force -Or ((Test-Path variable:ci) -And $ci)) {
        $Message = "(NETCORE_ENGINEERING_TELEMETRY=$Category) $Message"
    }
    $PSBoundParameters.Remove('Message') | Out-Null
    $PSBoundParameters.Add('Message', $Message)
    Write-PipelineTaskError @PSBoundParameters
}

# Specify "-Force" to force pipeline formatted output even if "$ci" is false or not set
function Write-PipelineTaskError {
    [CmdletBinding()]
    param(
        [Parameter(Mandatory = $true)]
        [string]$Message,
        [Parameter(Mandatory = $false)]
        [string]$Type = 'error',
        [string]$ErrCode,
        [string]$SourcePath,
        [string]$LineNumber,
        [string]$ColumnNumber,
        [switch]$AsOutput,
        [switch]$Force
    )

    if (!$Force -And (-Not (Test-Path variable:ci) -Or !$ci)) {
        if ($Type -eq 'error') {
            Write-Host $Message -ForegroundColor Red
            return
        }
        elseif ($Type -eq 'warning') {
            Write-Host $Message -ForegroundColor Yellow
            return
        }
    }

    if (($Type -ne 'error') -and ($Type -ne 'warning')) {
        Write-Host $Message
        return
    }
    $PSBoundParameters.Remove('Force') | Out-Null
    if (-not $PSBoundParameters.ContainsKey('Type')) {
        $PSBoundParameters.Add('Type', 'error')
    }
    Write-LogIssue @PSBoundParameters
}

function Write-PipelineSetVariable {
    [CmdletBinding()]
    param(
        [Parameter(Mandatory = $true)]
        [string]$Name,
        [string]$Value,
        [switch]$Secret,
        [switch]$AsOutput,
        [bool]$IsMultiJobVariable = $true)

    if ((Test-Path variable:ci) -And $ci) {
        Write-LoggingCommand -Area 'task' -Event 'setvariable' -Data $Value -Properties @{
            'variable' = $Name
            'isSecret' = $Secret
            'isOutput' = $IsMultiJobVariable
        } -AsOutput:$AsOutput
    }
}

function Write-PipelinePrependPath {
    [CmdletBinding()]
    param(
        [Parameter(Mandatory = $true)]
        [string]$Path,
        [switch]$AsOutput)

    if ((Test-Path variable:ci) -And $ci) {
        Write-LoggingCommand -Area 'task' -Event 'prependpath' -Data $Path -AsOutput:$AsOutput
    }
}

function Write-PipelineSetResult {
    [CmdletBinding()]
    param(
        [ValidateSet("Succeeded", "SucceededWithIssues", "Failed", "Cancelled", "Skipped")]
        [Parameter(Mandatory = $true)]
        [string]$Result,
        [string]$Message)
    if ((Test-Path variable:ci) -And $ci) {
        Write-LoggingCommand -Area 'task' -Event 'complete' -Data $Message -Properties @{
            'result' = $Result
        }
    }
}

<########################################
# Private functions.
########################################>
function Format-LoggingCommandData {
    [CmdletBinding()]
    param([string]$Value, [switch]$Reverse)

    if (!$Value) {
        return ''
    }

    if (!$Reverse) {
        foreach ($mapping in $script:loggingCommandEscapeMappings) {
            $Value = $Value.Replace($mapping.Token, $mapping.Replacement)
        }
    }
    else {
        for ($i = $script:loggingCommandEscapeMappings.Length - 1 ; $i -ge 0 ; $i--) {
            $mapping = $script:loggingCommandEscapeMappings[$i]
            $Value = $Value.Replace($mapping.Replacement, $mapping.Token)
        }
    }

    return $Value
}

function Format-LoggingCommand {
    [CmdletBinding()]
    param(
        [Parameter(Mandatory = $true)]
        [string]$Area,
        [Parameter(Mandatory = $true)]
        [string]$Event,
        [string]$Data,
        [hashtable]$Properties)

    # Append the preamble.
    [System.Text.StringBuilder]$sb = New-Object -TypeName System.Text.StringBuilder
    $null = $sb.Append($script:loggingCommandPrefix).Append($Area).Append('.').Append($Event)

    # Append the properties.
    if ($Properties) {
        $first = $true
        foreach ($key in $Properties.Keys) {
            [string]$value = Format-LoggingCommandData $Properties[$key]
            if ($value) {
                if ($first) {
                    $null = $sb.Append(' ')
                    $first = $false
                }
                else {
                    $null = $sb.Append(';')
                }

                $null = $sb.Append("$key=$value")
            }
        }
    }

    # Append the tail and output the value.
    $Data = Format-LoggingCommandData $Data
    $sb.Append(']').Append($Data).ToString()
}

function Write-LoggingCommand {
    [CmdletBinding(DefaultParameterSetName = 'Parameters')]
    param(
        [Parameter(Mandatory = $true, ParameterSetName = 'Parameters')]
        [string]$Area,
        [Parameter(Mandatory = $true, ParameterSetName = 'Parameters')]
        [string]$Event,
        [Parameter(ParameterSetName = 'Parameters')]
        [string]$Data,
        [Parameter(ParameterSetName = 'Parameters')]
        [hashtable]$Properties,
        [Parameter(Mandatory = $true, ParameterSetName = 'Object')]
        $Command,
        [switch]$AsOutput)

    if ($PSCmdlet.ParameterSetName -eq 'Object') {
        Write-LoggingCommand -Area $Command.Area -Event $Command.Event -Data $Command.Data -Properties $Command.Properties -AsOutput:$AsOutput
        return
    }

    $command = Format-LoggingCommand -Area $Area -Event $Event -Data $Data -Properties $Properties
    if ($AsOutput) {
        $command
    }
    else {
        Write-Host $command
    }
}

function Write-LogIssue {
    [CmdletBinding()]
    param(
        [ValidateSet('warning', 'error')]
        [Parameter(Mandatory = $true)]
        [string]$Type,
        [string]$Message,
        [string]$ErrCode,
        [string]$SourcePath,
        [string]$LineNumber,
        [string]$ColumnNumber,
        [switch]$AsOutput)

    $command = Format-LoggingCommand -Area 'task' -Event 'logissue' -Data $Message -Properties @{
        'type'         = $Type
        'code'         = $ErrCode
        'sourcepath'   = $SourcePath
        'linenumber'   = $LineNumber
        'columnnumber' = $ColumnNumber
    }
    if ($AsOutput) {
        return $command
    }

    if ($Type -eq 'error') {
        $foregroundColor = $host.PrivateData.ErrorForegroundColor
        $backgroundColor = $host.PrivateData.ErrorBackgroundColor
        if ($foregroundColor -isnot [System.ConsoleColor] -or $backgroundColor -isnot [System.ConsoleColor]) {
            $foregroundColor = [System.ConsoleColor]::Red
            $backgroundColor = [System.ConsoleColor]::Black
        }
    }
    else {
        $foregroundColor = $host.PrivateData.WarningForegroundColor
        $backgroundColor = $host.PrivateData.WarningBackgroundColor
        if ($foregroundColor -isnot [System.ConsoleColor] -or $backgroundColor -isnot [System.ConsoleColor]) {
            $foregroundColor = [System.ConsoleColor]::Yellow
            $backgroundColor = [System.ConsoleColor]::Black
        }
    }

    Write-Host $command -ForegroundColor $foregroundColor -BackgroundColor $backgroundColor
}



================================================
FILE: eng/common/pipeline-logging-functions.sh
================================================
#!/usr/bin/env bash

function Write-PipelineTelemetryError {
  local telemetry_category=''
  local force=false
  local function_args=()
  local message=''
  while [[ $# -gt 0 ]]; do
    opt="$(echo "${1/#--/-}" | tr "[:upper:]" "[:lower:]")"
    case "$opt" in
      -category|-c)
        telemetry_category=$2
        shift
        ;;
      -force|-f)
        force=true
        ;;
      -*)
        function_args+=("$1 $2")
        shift
        ;;
      *)
        message=$*
        ;;
    esac
    shift
  done

  if [[ $force != true ]] && [[ "$ci" != true ]]; then
    echo "$message" >&2
    return
  fi

  if [[ $force == true ]]; then
    function_args+=("-force")
  fi
  message="(NETCORE_ENGINEERING_TELEMETRY=$telemetry_category) $message"
  function_args+=("$message")
  Write-PipelineTaskError ${function_args[@]}
}

function Write-PipelineTaskError {
  local message_type="error"
  local sourcepath=''
  local linenumber=''
  local columnnumber=''
  local error_code=''
  local force=false

  while [[ $# -gt 0 ]]; do
    opt="$(echo "${1/#--/-}" | tr "[:upper:]" "[:lower:]")"
    case "$opt" in
      -type|-t)
        message_type=$2
        shift
        ;;
      -sourcepath|-s)
        sourcepath=$2
        shift
        ;;
      -linenumber|-ln)
        linenumber=$2
        shift
        ;;
      -columnnumber|-cn)
        columnnumber=$2
        shift
        ;;
      -errcode|-e)
        error_code=$2
        shift
        ;;
      -force|-f)
        force=true
        ;;
      *)
        break
        ;;
    esac

    shift
  done

  if [[ $force != true ]] && [[ "$ci" != true ]]; then
    echo "$@" >&2
    return
  fi

  local message="##vso[task.logissue"

  message="$message type=$message_type"

  if [ -n "$sourcepath" ]; then
    message="$message;sourcepath=$sourcepath"
  fi

  if [ -n "$linenumber" ]; then
    message="$message;linenumber=$linenumber"
  fi

  if [ -n "$columnnumber" ]; then
    message="$message;columnnumber=$columnnumber"
  fi

  if [ -n "$error_code" ]; then
    message="$message;code=$error_code"
  fi

  message="$message]$*"
  echo "$message"
}

function Write-PipelineSetVariable {
  if [[ "$ci" != true ]]; then
    return
  fi

  local name=''
  local value=''
  local secret=false
  local as_output=false
  local is_multi_job_variable=true

  while [[ $# -gt 0 ]]; do
    opt="$(echo "${1/#--/-}" | tr "[:upper:]" "[:lower:]")"
    case "$opt" in
      -name|-n)
        name=$2
        shift
        ;;
      -value|-v)
        value=$2
        shift
        ;;
      -secret|-s)
        secret=true
        ;;
      -as_output|-a)
        as_output=true
        ;;
      -is_multi_job_variable|-i)
        is_multi_job_variable=$2
        shift
        ;;
    esac
    shift
  done

  value=${value/;/%3B}
  value=${value/\\r/%0D}
  value=${value/\\n/%0A}
  value=${value/]/%5D}

  local message="##vso[task.setvariable variable=$name;isSecret=$secret;isOutput=$is_multi_job_variable]$value"

  if [[ "$as_output" == true ]]; then
    $message
  else
    echo "$message"
  fi
}

function Write-PipelinePrependPath {
  local prepend_path=''

  while [[ $# -gt 0 ]]; do
    opt="$(echo "${1/#--/-}" | tr "[:upper:]" "[:lower:]")"
    case "$opt" in
      -path|-p)
        prepend_path=$2
        shift
        ;;
    esac
    shift
  done

  export PATH="$prepend_path:$PATH"

  if [[ "$ci" == true ]]; then
    echo "##vso[task.prependpath]$prepend_path"
  fi
}

function Write-PipelineSetResult {
  local result=''
  local message=''

  while [[ $# -gt 0 ]]; do
    opt="$(echo "${1/#--/-}" | tr "[:upper:]" "[:lower:]")"
    case "$opt" in
      -result|-r)
        result=$2
        shift
        ;;
      -message|-m)
        message=$2
        shift
        ;;
    esac
    shift
  done

  if [[ "$ci" == true ]]; then
    echo "##vso[task.complete result=$result;]$message"
  fi
}



================================================
FILE: eng/common/PSScriptAnalyzerSettings.psd1
================================================
@{
    IncludeRules=@('PSAvoidUsingCmdletAliases',
                   'PSAvoidUsingWMICmdlet',
                   'PSAvoidUsingPositionalParameters',
                   'PSAvoidUsingInvokeExpression',
                   'PSUseDeclaredVarsMoreThanAssignments',
                   'PSUseCmdletCorrectly',
                   'PSStandardDSCFunctionsInResource',
                   'PSUseIdenticalMandatoryParametersForDSC',
                   'PSUseIdenticalParametersForDSC')
}


================================================
FILE: eng/common/retain-build.ps1
================================================

Param(
[Parameter(Mandatory=$true)][int] $buildId,
[Parameter(Mandatory=$true)][string] $azdoOrgUri,
[Parameter(Mandatory=$true)][string] $azdoProject,
[Parameter(Mandatory=$true)][string] $token
)

$ErrorActionPreference = 'Stop'
Set-StrictMode -Version 2.0

function Get-AzDOHeaders(
    [string] $token)
{
    $base64AuthInfo = [Convert]::ToBase64String([Text.Encoding]::ASCII.GetBytes(":${token}"))
    $headers = @{"Authorization"="Basic $base64AuthInfo"}
    return $headers
}

function Update-BuildRetention(
    [string] $azdoOrgUri,
    [string] $azdoProject,
    [int] $buildId,
    [string] $token)
{
    $headers = Get-AzDOHeaders -token $token
    $requestBody = "{
        `"keepForever`": `"true`"
    }"

    $requestUri = "${azdoOrgUri}/${azdoProject}/_apis/build/builds/${buildId}?api-version=6.0"
    write-Host "Attempting to retain build using the following URI: ${requestUri} ..."

    try {
        Invoke-RestMethod -Uri $requestUri -Method Patch -Body $requestBody -Header $headers -contentType "application/json"
        Write-Host "Updated retention settings for build ${buildId}."
    }
    catch {
        Write-Error "Failed to update retention settings for build: $_.Exception.Response.StatusDescription"
        exit 1
    }
}

Update-BuildRetention -azdoOrgUri $azdoOrgUri -azdoProject $azdoProject -buildId $buildId -token $token
exit 0



================================================
FILE: eng/common/sdk-task.ps1
================================================
[CmdletBinding(PositionalBinding=$false)]
Param(
  [string] $configuration = 'Debug',
  [string] $task,
  [string] $verbosity = 'minimal',
  [string] $msbuildEngine = $null,
  [switch] $restore,
  [switch] $prepareMachine,
  [switch] $help,
  [Parameter(ValueFromRemainingArguments=$true)][String[]]$properties
)

$ci = $true
$binaryLog = $true
$warnAsError = $true

. $PSScriptRoot\tools.ps1

function Print-Usage() {
  Write-Host "Common settings:"
  Write-Host "  -task <value>           Name of Arcade task (name of a project in SdkTasks directory of the Arcade SDK package)"
  Write-Host "  -restore                Restore dependencies"
  Write-Host "  -verbosity <value>      Msbuild verbosity: q[uiet], m[inimal], n[ormal], d[etailed], and diag[nostic]"
  Write-Host "  -help                   Print help and exit"
  Write-Host ""

  Write-Host "Advanced settings:"
  Write-Host "  -prepareMachine         Prepare machine for CI run"
  Write-Host "  -msbuildEngine <value>  Msbuild engine to use to run build ('dotnet', 'vs', or unspecified)."
  Write-Host ""
  Write-Host "Command line arguments not listed above are passed thru to msbuild."
}

function Build([string]$target) {
  $logSuffix = if ($target -eq 'Execute') { '' } else { ".$target" }
  $log = Join-Path $LogDir "$task$logSuffix.binlog"
  $outputPath = Join-Path $ToolsetDir "$task\"

  MSBuild $taskProject `
    /bl:$log `
    /t:$target `
    /p:Configuration=$configuration `
    /p:RepoRoot=$RepoRoot `
    /p:BaseIntermediateOutputPath=$outputPath `
    /v:$verbosity `
    @properties
}

try {
  if ($help -or (($null -ne $properties) -and ($properties.Contains('/help') -or $properties.Contains('/?')))) {
    Print-Usage
    exit 0
  }

  if ($task -eq "") {
    Write-PipelineTelemetryError -Category 'Build' -Message "Missing required parameter '-task <value>'"
    Print-Usage
    ExitWithExitCode 1
  }

  if( $msbuildEngine -eq "vs") {
    # Ensure desktop MSBuild is available for sdk tasks.
    if( -not ($GlobalJson.tools.PSObject.Properties.Name -contains "vs" )) {
      $GlobalJson.tools | Add-Member -Name "vs" -Value (ConvertFrom-Json "{ `"version`": `"16.5`" }") -MemberType NoteProperty
    }
    if( -not ($GlobalJson.tools.PSObject.Properties.Name -match "xcopy-msbuild" )) {
      $GlobalJson.tools | Add-Member -Name "xcopy-msbuild" -Value "17.12.0" -MemberType NoteProperty
    }
    if ($GlobalJson.tools."xcopy-msbuild".Trim() -ine "none") {
        $xcopyMSBuildToolsFolder = InitializeXCopyMSBuild $GlobalJson.tools."xcopy-msbuild" -install $true
    }
    if ($xcopyMSBuildToolsFolder -eq $null) {
      throw 'Unable to get xcopy downloadable version of msbuild'
    }

    $global:_MSBuildExe = "$($xcopyMSBuildToolsFolder)\MSBuild\Current\Bin\MSBuild.exe"
  }

  $taskProject = GetSdkTaskProject $task
  if (!(Test-Path $taskProject)) {
    Write-PipelineTelemetryError -Category 'Build' -Message "Unknown task: $task"
    ExitWithExitCode 1
  }

  if ($restore) {
    Build 'Restore'
  }

  Build 'Execute'
}
catch {
  Write-Host $_.ScriptStackTrace
  Write-PipelineTelemetryError -Category 'Build' -Message $_
  ExitWithExitCode 1
}

ExitWithExitCode 0



================================================
FILE: eng/common/SetupNugetSources.ps1
================================================
# This script adds internal feeds required to build commits that depend on internal package sources. For instance,
# dotnet6-internal would be added automatically if dotnet6 was found in the nuget.config file. In addition also enables
# disabled internal Maestro (darc-int*) feeds.
#
# Optionally, this script also adds a credential entry for each of the internal feeds if supplied.
#
# See example call for this script below.
#
#  - task: PowerShell@2
#    displayName: Setup Private Feeds Credentials
#    condition: eq(variables['Agent.OS'], 'Windows_NT')
#    inputs:
#      filePath: $(Build.SourcesDirectory)/eng/common/SetupNugetSources.ps1
#      arguments: -ConfigFile $(Build.SourcesDirectory)/NuGet.config -Password $Env:Token
#    env:
#      Token: $(dn-bot-dnceng-artifact-feeds-rw)
#
# Note that the NuGetAuthenticate task should be called after SetupNugetSources.
# This ensures that:
# - Appropriate creds are set for the added internal feeds (if not supplied to the scrupt)
# - The credential provider is installed.
#
# This logic is also abstracted into enable-internal-sources.yml.

[CmdletBinding()]
param (
    [Parameter(Mandatory = $true)][string]$ConfigFile,
    $Password
)

$ErrorActionPreference = "Stop"
Set-StrictMode -Version 2.0
[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12

. $PSScriptRoot\tools.ps1

# Add source entry to PackageSources
function AddPackageSource($sources, $SourceName, $SourceEndPoint, $creds, $Username, $pwd) {
    $packageSource = $sources.SelectSingleNode("add[@key='$SourceName']")

    if ($packageSource -eq $null)
    {
        $packageSource = $doc.CreateElement("add")
        $packageSource.SetAttribute("key", $SourceName)
        $packageSource.SetAttribute("value", $SourceEndPoint)
        $sources.AppendChild($packageSource) | Out-Null
    }
    else {
        Write-Host "Package source $SourceName already present."
    }

    AddCredential -Creds $creds -Source $SourceName -Username $Username -pwd $pwd
}

# Add a credential node for the specified source
function AddCredential($creds, $source, $username, $pwd) {
    # If no cred supplied, don't do anything.
    if (!$pwd) {
        return;
    }

    # Looks for credential configuration for the given SourceName. Create it if none is found.
    $sourceElement = $creds.SelectSingleNode($Source)
    if ($sourceElement -eq $null)
    {
        $sourceElement = $doc.CreateElement($Source)
        $creds.AppendChild($sourceElement) | Out-Null
    }

    # Add the <Username> node to the credential if none is found.
    $usernameElement = $sourceElement.SelectSingleNode("add[@key='Username']")
    if ($usernameElement -eq $null)
    {
        $usernameElement = $doc.CreateElement("add")
        $usernameElement.SetAttribute("key", "Username")
        $sourceElement.AppendChild($usernameElement) | Out-Null
    }
    $usernameElement.SetAttribute("value", $Username)

    # Add the <ClearTextPassword> to the credential if none is found.
    # Add it as a clear text because there is no support for encrypted ones in non-windows .Net SDKs.
    #   -> https://github.com/NuGet/Home/issues/5526
    $passwordElement = $sourceElement.SelectSingleNode("add[@key='ClearTextPassword']")
    if ($passwordElement -eq $null)
    {
        $passwordElement = $doc.CreateElement("add")
        $passwordElement.SetAttribute("key", "ClearTextPassword")
        $sourceElement.AppendChild($passwordElement) | Out-Null
    }

    $passwordElement.SetAttribute("value", $pwd)
}

function InsertMaestroPrivateFeedCredentials($Sources, $Creds, $Username, $pwd) {
    $maestroPrivateSources = $Sources.SelectNodes("add[contains(@key,'darc-int')]")

    Write-Host "Inserting credentials for $($maestroPrivateSources.Count) Maestro's private feeds."

    ForEach ($PackageSource in $maestroPrivateSources) {
        Write-Host "`tInserting credential for Maestro's feed:" $PackageSource.Key
        AddCredential -Creds $creds -Source $PackageSource.Key -Username $Username -pwd $pwd
    }
}

function EnablePrivatePackageSources($DisabledPackageSources) {
    $maestroPrivateSources = $DisabledPackageSources.SelectNodes("add[contains(@key,'darc-int')]")
    ForEach ($DisabledPackageSource in $maestroPrivateSources) {
        Write-Host "`tEnsuring private source '$($DisabledPackageSource.key)' is enabled by deleting it from disabledPackageSource"
        # Due to https://github.com/NuGet/Home/issues/10291, we must actually remove the disabled entries
        $DisabledPackageSources.RemoveChild($DisabledPackageSource)
    }
}

if (!(Test-Path $ConfigFile -PathType Leaf)) {
  Write-PipelineTelemetryError -Category 'Build' -Message "Eng/common/SetupNugetSources.ps1 returned a non-zero exit code. Couldn't find the NuGet config file: $ConfigFile"
  ExitWithExitCode 1
}

# Load NuGet.config
$doc = New-Object System.Xml.XmlDocument
$filename = (Get-Item $ConfigFile).FullName
$doc.Load($filename)

# Get reference to <PackageSources> or create one if none exist already
$sources = $doc.DocumentElement.SelectSingleNode("packageSources")
if ($sources -eq $null) {
    $sources = $doc.CreateElement("packageSources")
    $doc.DocumentElement.AppendChild($sources) | Out-Null
}

$creds = $null
if ($Password) {
    # Looks for a <PackageSourceCredentials> node. Create it if none is found.
    $creds = $doc.DocumentElement.SelectSingleNode("packageSourceCredentials")
    if ($creds -eq $null) {
        $creds = $doc.CreateElement("packageSourceCredentials")
        $doc.DocumentElement.AppendChild($creds) | Out-Null
    }
}

# Check for disabledPackageSources; we'll enable any darc-int ones we find there
$disabledSources = $doc.DocumentElement.SelectSingleNode("disabledPackageSources")
if ($disabledSources -ne $null) {
    Write-Host "Checking for any darc-int disabled package sources in the disabledPackageSources node"
    EnablePrivatePackageSources -DisabledPackageSources $disabledSources
}

$userName = "dn-bot"

# Insert credential nodes for Maestro's private feeds
InsertMaestroPrivateFeedCredentials -Sources $sources -Creds $creds -Username $userName -pwd $Password

# 3.1 uses a different feed url format so it's handled differently here
$dotnet31Source = $sources.SelectSingleNode("add[@key='dotnet3.1']")
if ($dotnet31Source -ne $null) {
    AddPackageSource -Sources $sources -SourceName "dotnet3.1-internal" -SourceEndPoint "https://pkgs.dev.azure.com/dnceng/_packaging/dotnet3.1-internal/nuget/v2" -Creds $creds -Username $userName -pwd $Password
    AddPackageSource -Sources $sources -SourceName "dotnet3.1-internal-transport" -SourceEndPoint "https://pkgs.dev.azure.com/dnceng/_packaging/dotnet3.1-internal-transport/nuget/v2" -Creds $creds -Username $userName -pwd $Password
}

$dotnetVersions = @('5','6','7','8','9')

foreach ($dotnetVersion in $dotnetVersions) {
    $feedPrefix = "dotnet" + $dotnetVersion;
    $dotnetSource = $sources.SelectSingleNode("add[@key='$feedPrefix']")
    if ($dotnetSource -ne $null) {
        AddPackageSource -Sources $sources -SourceName "$feedPrefix-internal" -SourceEndPoint "https://pkgs.dev.azure.com/dnceng/internal/_packaging/$feedPrefix-internal/nuget/v2" -Creds $creds -Username $userName -pwd $Password
        AddPackageSource -Sources $sources -SourceName "$feedPrefix-internal-transport" -SourceEndPoint "https://pkgs.dev.azure.com/dnceng/internal/_packaging/$feedPrefix-internal-transport/nuget/v2" -Creds $creds -Username $userName -pwd $Password
    }
}

$doc.Save($filename)



================================================
FILE: eng/common/SetupNugetSources.sh
================================================
#!/usr/bin/env bash

# This script adds internal feeds required to build commits that depend on internal package sources. For instance,
# dotnet6-internal would be added automatically if dotnet6 was found in the nuget.config file. In addition also enables
# disabled internal Maestro (darc-int*) feeds.
#
# Optionally, this script also adds a credential entry for each of the internal feeds if supplied.
#
# See example call for this script below.
#
#  - task: Bash@3
#    displayName: Setup Internal Feeds
#    inputs:
#      filePath: $(Build.SourcesDirectory)/eng/common/SetupNugetSources.sh
#      arguments: $(Build.SourcesDirectory)/NuGet.config
#    condition: ne(variables['Agent.OS'], 'Windows_NT')
#  - task: NuGetAuthenticate@1
#
# Note that the NuGetAuthenticate task should be called after SetupNugetSources.
# This ensures that:
# - Appropriate creds are set for the added internal feeds (if not supplied to the scrupt)
# - The credential provider is installed.
#
# This logic is also abstracted into enable-internal-sources.yml.

ConfigFile=$1
CredToken=$2
NL='\n'
TB='    '

source="${BASH_SOURCE[0]}"

# resolve $source until the file is no longer a symlink
while [[ -h "$source" ]]; do
  scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"
  source="$(readlink "$source")"
  # if $source was a relative symlink, we need to resolve it relative to the path where the
  # symlink file was located
  [[ $source != /* ]] && source="$scriptroot/$source"
done
scriptroot="$( cd -P "$( dirname "$source" )" && pwd )"

. "$scriptroot/tools.sh"

if [ ! -f "$ConfigFile" ]; then
    Write-PipelineTelemetryError -Category 'Build' "Error: Eng/common/SetupNugetSources.sh returned a non-zero exit code. Couldn't find the NuGet config file: $ConfigFile"
    ExitWithExitCode 1
fi

if [[ `uname -s` == "Darwin" ]]; then
    NL=$'\\\n'
    TB=''
fi

# Ensure there is a <packageSources>...</packageSources> section.
grep -i "<packageSources>" $ConfigFile
if [ "$?" != "0" ]; then
    echo "Adding <packageSources>...</packageSources> section."
    ConfigNodeHeader="<configuration>"
    PackageSourcesTemplate="${TB}<packageSources>${NL}${TB}</packageSources>"

    sed -i.bak "s|$ConfigNodeHeader|$ConfigNodeHeader${NL}$PackageSourcesTemplate|" $ConfigFile
fi

# Ensure there is a <packageSourceCredentials>...</packageSourceCredentials> section.
grep -i "<packageSourceCredentials>" $ConfigFile
if [ "$?" != "0" ]; then
    echo "Adding <packageSourceCredentials>...</packageSourceCredentials> section."

    PackageSourcesNodeFooter="</packageSources>"
    PackageSourceCredentialsTemplate="${TB}<packageSourceCredentials>${NL}${TB}</packageSourceCredentials>"

    sed -i.bak "s|$PackageSourcesNodeFooter|$PackageSourcesNodeFooter${NL}$PackageSourceCredentialsTemplate|" $ConfigFile
fi

PackageSources=()

# Ensure dotnet3.1-internal and dotnet3.1-internal-transport are in the packageSources if the public dotnet3.1 feeds are present
grep -i "<add key=\"dotnet3.1\"" $ConfigFile
if [ "$?" == "0" ]; then
    grep -i "<add key=\"dotnet3.1-internal\"" $ConfigFile
    if [ "$?" != "0" ]; then
        echo "Adding dotnet3.1-internal to the packageSources."
        PackageSourcesNodeFooter="</packageSources>"
        PackageSourceTemplate="${TB}<add key=\"dotnet3.1-internal\" value=\"https://pkgs.dev.azure.com/dnceng/_packaging/dotnet3.1-internal/nuget/v2\" />"

        sed -i.bak "s|$PackageSourcesNodeFooter|$PackageSourceTemplate${NL}$PackageSourcesNodeFooter|" $ConfigFile
    fi
    PackageSources+=('dotnet3.1-internal')

    grep -i "<add key=\"dotnet3.1-internal-transport\">" $ConfigFile
    if [ "$?" != "0" ]; then
        echo "Adding dotnet3.1-internal-transport to the packageSources."
        PackageSourcesNodeFooter="</packageSources>"
        PackageSourceTemplate="${TB}<add key=\"dotnet3.1-internal-transport\" value=\"https://pkgs.dev.azure.com/dnceng/_packaging/dotnet3.1-internal-transport/nuget/v2\" />"

        sed -i.bak "s|$PackageSourcesNodeFooter|$PackageSourceTemplate${NL}$PackageSourcesNodeFooter|" $ConfigFile
    fi
    PackageSources+=('dotnet3.1-internal-transport')
fi

DotNetVersions=('5' '6' '7' '8' '9')

for DotNetVersion in ${DotNetVersions[@]} ; do
    FeedPrefix="dotnet${DotNetVersion}";
    grep -i "<add key=\"$FeedPrefix\"" $ConfigFile
    if [ "$?" == "0" ]; then
        grep -i "<add key=\"$FeedPrefix-internal\"" $ConfigFile
        if [ "$?" != "0" ]; then
            echo "Adding $FeedPrefix-internal to the packageSources."
            PackageSourcesNodeFooter="</packageSources>"
            PackageSourceTemplate="${TB}<add key=\"$FeedPrefix-internal\" value=\"https://pkgs.dev.azure.com/dnceng/internal/_packaging/$FeedPrefix-internal/nuget/v2\" />"

            sed -i.bak "s|$PackageSourcesNodeFooter|$PackageSourceTemplate${NL}$PackageSourcesNodeFooter|" $ConfigFile
        fi
        PackageSources+=("$FeedPrefix-internal")

        grep -i "<add key=\"$FeedPrefix-internal-transport\">" $ConfigFile
        if [ "$?" != "0" ]; then
            echo "Adding $FeedPrefix-internal-transport to the packageSources."
            PackageSourcesNodeFooter="</packageSources>"
            PackageSourceTemplate="${TB}<add key=\"$FeedPrefix-internal-transport\" value=\"https://pkgs.dev.azure.com/dnceng/internal/_packaging/$FeedPrefix-internal-transport/nuget/v2\" />"

            sed -i.bak "s|$PackageSourcesNodeFooter|$PackageSourceTemplate${NL}$PackageSourcesNodeFooter|" $ConfigFile
        fi
        PackageSources+=("$FeedPrefix-internal-transport")
    fi
done

# I want things split line by line
PrevIFS=$IFS
IFS=$'\n'
PackageSources+="$IFS"
PackageSources+=$(grep -oh '"darc-int-[^"]*"' $ConfigFile | tr -d '"')
IFS=$PrevIFS

if [ "$CredToken" ]; then
    for FeedName in ${PackageSources[@]} ; do
        # Check if there is no existing credential for this FeedName
        grep -i "<$FeedName>" $ConfigFile
        if [ "$?" != "0" ]; then
            echo "Adding credentials for $FeedName."

            PackageSourceCredentialsNodeFooter="</packageSourceCredentials>"
            NewCredential="${TB}${TB}<$FeedName>${NL}<add key=\"Username\" value=\"dn-bot\" />${NL}<add key=\"ClearTextPassword\" value=\"$CredToken\" />${NL}</$FeedName>"

            sed -i.bak "s|$PackageSourceCredentialsNodeFooter|$NewCredential${NL}$PackageSourceCredentialsNodeFooter|" $ConfigFile
        fi
    done
fi

# Re-enable any entries in disabledPackageSources where the feed name contains darc-int
grep -i "<disabledPackageSources>" $ConfigFile
if [ "$?" == "0" ]; then
    DisabledDarcIntSources=()
    echo "Re-enabling any disabled \"darc-int\" package sources in $ConfigFile"
    DisabledDarcIntSources+=$(grep -oh '"darc-int-[^"]*" value="true"' $ConfigFile  | tr -d '"')
    for DisabledSourceName in ${DisabledDarcIntSources[@]} ; do
        if [[ $DisabledSourceName == darc-int* ]]
            then
                OldDisableValue="<add key=\"$DisabledSourceName\" value=\"true\" />"
                NewDisableValue="<!-- Reenabled for build : $DisabledSourceName -->"
                sed -i.bak "s|$OldDisableValue|$NewDisableValue|" $ConfigFile
                echo "Neutralized disablePackageSources entry for '$DisabledSourceName'"
        fi
    done
fi



================================================
FILE: eng/common/template-guidance.md
================================================
# Overview

Arcade provides templates for public (`/templates`) and 1ES pipeline templates (`/templates-official`) scenarios.  Pipelines which are required to be managed by 1ES pipeline templates should reference `/templates-offical`, all other pipelines may reference `/templates`.

## How to use

Basic guidance is:

- 1ES Pipeline Template or 1ES Microbuild template runs should reference `eng/common/templates-official`. Any internal production-graded pipeline should use these templates.

- All other runs should reference `eng/common/templates`.

See [azure-pipelines.yml](../../azure-pipelines.yml) (templates-official example) or [azure-pipelines-pr.yml](../../azure-pipelines-pr.yml) (templates example) for examples.

#### The `templateIs1ESManaged` parameter

The `templateIs1ESManaged` is available on most templates and affects which of the variants is used for nested templates. See [Development Notes](#development-notes) below for more information on the `templateIs1ESManaged1 parameter.

- For templates under `job/`, `jobs/`, `steps`, or `post-build/`, this parameter must be explicitly set.

## Multiple outputs

1ES pipeline templates impose a policy where every publish artifact execution results in additional security scans being injected into your pipeline.  When using `templates-official/jobs/jobs.yml`, Arcade reduces the number of additional security injections by gathering all publishing outputs into the [Build.ArtifactStagingDirectory](https://learn.microsoft.com/en-us/azure/devops/pipelines/build/variables?view=azure-devops&tabs=yaml#build-variables-devops-services), and utilizing the [outputParentDirectory](https://eng.ms/docs/cloud-ai-platform/devdiv/one-engineering-system-1es/1es-docs/1es-pipeline-templates/features/outputs#multiple-outputs) feature of 1ES pipeline templates.  When implementing your pipeline, if you ensure publish artifacts are located in the `$(Build.ArtifactStagingDirectory)`, and utilize the 1ES provided template context, then you can reduce the number of security scans for your pipeline.

Example:
``` yaml
# azure-pipelines.yml
extends:
  template: azure-pipelines/MicroBuild.1ES.Official.yml@MicroBuildTemplate
  parameters:
    stages:
    - stage: build
      jobs:
      - template: /eng/common/templates-official/jobs/jobs.yml@self
        parameters:
          # 1ES makes use of outputs to reduce security task injection overhead
          templateContext:
            outputs:
            - output: pipelineArtifact
              displayName: 'Publish logs from source'
              continueOnError: true
              condition: always()
              targetPath: $(Build.ArtifactStagingDirectory)/artifacts/log
              artifactName: Logs
          jobs:
          - job: Windows
            steps:
            - script: echo "friendly neighborhood" > artifacts/marvel/spiderman.txt
          # copy build outputs to artifact staging directory for publishing
          - task: CopyFiles@2
              displayName: Gather build output
              inputs:
                SourceFolder: '$(Build.SourcesDirectory)/artifacts/marvel'
                Contents: '**'
                TargetFolder: '$(Build.ArtifactStagingDirectory)/artifacts/marvel'
```

Note: Multiple outputs are ONLY applicable to 1ES PT publishing (only usable when referencing `templates-official`).

## Development notes

**Folder / file structure**

``` text
eng\common\
    [templates || templates-official]\
        job\
            job.yml                          (shim + artifact publishing logic)
            onelocbuild.yml                  (shim)
            publish-build-assets.yml         (shim)
            source-build.yml                 (shim)
            source-index-stage1.yml          (shim)
        jobs\
            codeql-build.yml                 (shim)
            jobs.yml                         (shim)
            source-build.yml                 (shim)
        post-build\
            post-build.yml                   (shim)
            common-variabls.yml              (shim)
            setup-maestro-vars.yml           (shim)
        steps\
            publish-build-artifacts.yml      (logic)
            publish-pipeline-artifacts.yml   (logic)
            component-governance.yml         (shim)
            generate-sbom.yml                (shim)
            publish-logs.yml                 (shim)
            retain-build.yml                 (shim)
            send-to-helix.yml                (shim)
            source-build.yml                 (shim)
        variables\
            pool-providers.yml               (logic + redirect) # templates/variables/pool-providers.yml will redirect to templates-official/variables/pool-providers.yml if you are running in the internal project
            sdl-variables.yml                (logic)
    core-templates\
        job\
            job.yml                          (logic)
            onelocbuild.yml                  (logic)
            publish-build-assets.yml         (logic)
            source-build.yml                 (logic)
            source-index-stage1.yml          (logic)
        jobs\
            codeql-build.yml                 (logic)
            jobs.yml                         (logic)
            source-build.yml                 (logic)
        post-build\
            common-variabls.yml              (logic)
            post-build.yml                   (logic)
            setup-maestro-vars.yml           (logic)
        steps\
            component-governance.yml         (logic)
            generate-sbom.yml                (logic)
            publish-build-artifacts.yml      (redirect)
            publish-logs.yml                 (logic)
            publish-pipeline-artifacts.yml   (redirect)
            retain-build.yml                 (logic)
            send-to-helix.yml                (logic)
            source-build.yml                 (logic)
        variables\
            pool-providers.yml               (redirect)
```

In the table above, a file is designated as "shim", "logic", or "redirect".

- shim - represents a yaml file which is an intermediate step between pipeline logic and .Net Core Engineering's templates (`core-templates`) and defines the `is1ESPipeline` parameter value.

- logic - represents actual base template logic.

- redirect- represents a file in `core-templates` which redirects to the "logic" file in either `templates` or `templates-official`.

Logic for Arcade's templates live **primarily** in the `core-templates` folder.  The exceptions to the location of the logic files are around artifact publishing, which is handled differently between 1es pipeline templates and standard templates.  `templates` and `templates-official` provide shim entry points which redirect to `core-templates` while also defining the `is1ESPipeline` parameter.  If a shim is referenced in `templates`, then `is1ESPipeline` is set to `false`.  If a shim is referenced in `templates-official`, then `is1ESPipeline` is set to `true`.

Within `templates` and `templates-official`, the templates at the "stages", and "jobs" / "job" level have been replaced with shims.  Templates at the "steps" and "variables" level are typically too granular to be replaced with shims and instead persist logic which is directly applicable to either scenario.

Within `core-templates`, there are a handful of places where logic is dependent on which shim entry point was used.  In those places, we redirect back to the respective logic file in `templates` or `templates-official`.



================================================
FILE: eng/common/tools.ps1
================================================
# Initialize variables if they aren't already defined.
# These may be defined as parameters of the importing script, or set after importing this script.

# CI mode - set to true on CI server for PR validation build or official build.
[bool]$ci = if (Test-Path variable:ci) { $ci } else { $false }

# Build configuration. Common values include 'Debug' and 'Release', but the repository may use other names.
[string]$configuration = if (Test-Path variable:configuration) { $configuration } else { 'Debug' }

# Set to true to opt out of outputting binary log while running in CI
[bool]$excludeCIBinarylog = if (Test-Path variable:excludeCIBinarylog) { $excludeCIBinarylog } else { $false }

# Set to true to output binary log from msbuild. Note that emitting binary log slows down the build.
[bool]$binaryLog = if (Test-Path variable:binaryLog) { $binaryLog } else { $ci -and !$excludeCIBinarylog }

# Set to true to use the pipelines logger which will enable Azure logging output.
# https://github.com/Microsoft/azure-pipelines-tasks/blob/master/docs/authoring/commands.md
# This flag is meant as a temporary opt-opt for the feature while validate it across
# our consumers. It will be deleted in the future.
[bool]$pipelinesLog = if (Test-Path variable:pipelinesLog) { $pipelinesLog } else { $ci }

# Turns on machine preparation/clean up code that changes the machine state (e.g. kills build processes).
[bool]$prepareMachine = if (Test-Path variable:prepareMachine) { $prepareMachine } else { $false }

# True to restore toolsets and dependencies.
[bool]$restore = if (Test-Path variable:restore) { $restore } else { $true }

# Adjusts msbuild verbosity level.
[string]$verbosity = if (Test-Path variable:verbosity) { $verbosity } else { 'minimal' }

# Set to true to reuse msbuild nodes. Recommended to not reuse on CI.
[bool]$nodeReuse = if (Test-Path variable:nodeReuse) { $nodeReuse } else { !$ci }

# Configures warning treatment in msbuild.
[bool]$warnAsError = if (Test-Path variable:warnAsError) { $warnAsError } else { $true }

# Specifies which msbuild engine to use for build: 'vs', 'dotnet' or unspecified (determined based on presence of tools.vs in global.json).
[string]$msbuildEngine = if (Test-Path variable:msbuildEngine) { $msbuildEngine } else { $null }

# True to attempt using .NET Core already that meets requirements specified in global.json
# installed on the machine instead of downloading one.
[bool]$useInstalledDotNetCli = if (Test-Path variable:useInstalledDotNetCli) { $useInstalledDotNetCli } else { $true }

# Enable repos to use a particular version of the on-line dotnet-install scripts.
#    default URL: https://builds.dotnet.microsoft.com/dotnet/scripts/v1/dotnet-install.ps1
[string]$dotnetInstallScriptVersion = if (Test-Path variable:dotnetInstallScriptVersion) { $dotnetInstallScriptVersion } else { 'v1' }

# True to use global NuGet cache instead of restoring packages to repository-local directory.
[bool]$useGlobalNuGetCache = if (Test-Path variable:useGlobalNuGetCache) { $useGlobalNuGetCache } else { !$ci }

# True to exclude prerelease versions Visual Studio during build
[bool]$excludePrereleaseVS = if (Test-Path variable:excludePrereleaseVS) { $excludePrereleaseVS } else { $false }

# An array of names of processes to stop on script exit if prepareMachine is true.
$processesToStopOnExit = if (Test-Path variable:processesToStopOnExit) { $processesToStopOnExit } else { @('msbuild', 'dotnet', 'vbcscompiler') }

$disableConfigureToolsetImport = if (Test-Path variable:disableConfigureToolsetImport) { $disableConfigureToolsetImport } else { $null }

set-strictmode -version 2.0
$ErrorActionPreference = 'Stop'
[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12

# If specifies, provides an alternate path for getting .NET Core SDKs and Runtimes. This script will still try public sources first.
[string]$runtimeSourceFeed = if (Test-Path variable:runtimeSourceFeed) { $runtimeSourceFeed } else { $null }
# Base-64 encoded SAS token that has permission to storage container described by $runtimeSourceFeed
[string]$runtimeSourceFeedKey = if (Test-Path variable:runtimeSourceFeedKey) { $runtimeSourceFeedKey } else { $null }

# True if the build is a product build
[bool]$productBuild = if (Test-Path variable:productBuild) { $productBuild } else { $false }

[String[]]$properties = if (Test-Path variable:properties) { $properties } else { @() }

function Create-Directory ([string[]] $path) {
    New-Item -Path $path -Force -ItemType 'Directory' | Out-Null
}

function Unzip([string]$zipfile, [string]$outpath) {
  Add-Type -AssemblyName System.IO.Compression.FileSystem
  [System.IO.Compression.ZipFile]::ExtractToDirectory($zipfile, $outpath)
}

# This will exec a process using the console and return it's exit code.
# This will not throw when the process fails.
# Returns process exit code.
function Exec-Process([string]$command, [string]$commandArgs) {
  $startInfo = New-Object System.Diagnostics.ProcessStartInfo
  $startInfo.FileName = $command
  $startInfo.Arguments = $commandArgs
  $startInfo.UseShellExecute = $false
  $startInfo.WorkingDirectory = Get-Location

  $process = New-Object System.Diagnostics.Process
  $process.StartInfo = $startInfo
  $process.Start() | Out-Null

  $finished = $false
  try {
    while (-not $process.WaitForExit(100)) {
      # Non-blocking loop done to allow ctr-c interrupts
    }

    $finished = $true
    return $global:LASTEXITCODE = $process.ExitCode
  }
  finally {
    # If we didn't finish then an error occurred or the user hit ctrl-c.  Either
    # way kill the process
    if (-not $finished) {
      $process.Kill()
    }
  }
}

# Take the given block, print it, print what the block probably references from the current set of
# variables using low-effort string matching, then run the block.
#
# This is intended to replace the pattern of manually copy-pasting a command, wrapping it in quotes,
# and printing it using "Write-Host". The copy-paste method is more readable in build logs, but less
# maintainable and less reliable. It is easy to make a mistake and modify the command without
# properly updating the "Write-Host" line, resulting in misleading build logs. The probability of
# this mistake makes the pattern hard to trust when it shows up in build logs. Finding the bug in
# existing source code can also be difficult, because the strings are not aligned to each other and
# the line may be 300+ columns long.
#
# By removing the need to maintain two copies of the command, Exec-BlockVerbosely avoids the issues.
#
# In Bash (or any posix-like shell), "set -x" prints usable verbose output automatically.
# "Set-PSDebug" appears to be similar at first glance, but unfortunately, it isn't very useful: it
# doesn't print any info about the variables being used by the command, which is normally the
# interesting part to diagnose.
function Exec-BlockVerbosely([scriptblock] $block) {
  Write-Host "--- Running script block:"
  $blockString = $block.ToString().Trim()
  Write-Host $blockString

  Write-Host "--- List of variables that might be used:"
  # For each variable x in the environment, check the block for a reference to x via simple "$x" or
  # "@x" syntax. This doesn't detect other ways to reference variables ("${x}" nor "$variable:x",
  # among others). It only catches what this function was originally written for: simple
  # command-line commands.
  $variableTable = Get-Variable |
    Where-Object {
      $blockString.Contains("`$$($_.Name)") -or $blockString.Contains("@$($_.Name)")
    } |
    Format-Table -AutoSize -HideTableHeaders -Wrap |
    Out-String
  Write-Host $variableTable.Trim()

  Write-Host "--- Executing:"
  & $block
  Write-Host "--- Done running script block!"
}

# createSdkLocationFile parameter enables a file being generated under the toolset directory
# which writes the sdk's location into. This is only necessary for cmd --> powershell invocations
# as dot sourcing isn't possible.
function InitializeDotNetCli([bool]$install, [bool]$createSdkLocationFile) {
  if (Test-Path variable:global:_DotNetInstallDir) {
    return $global:_DotNetInstallDir
  }

  # Don't resolve runtime, shared framework, or SDK from other locations to ensure build determinism
  $env:DOTNET_MULTILEVEL_LOOKUP=0

  # Disable first run since we do not need all ASP.NET packages restored.
  $env:DOTNET_NOLOGO=1

  # Disable telemetry on CI.
  if ($ci) {
    $env:DOTNET_CLI_TELEMETRY_OPTOUT=1
  }

  # Find the first path on %PATH% that contains the dotnet.exe
  if ($useInstalledDotNetCli -and (-not $globalJsonHasRuntimes) -and ($env:DOTNET_INSTALL_DIR -eq $null)) {
    $dotnetExecutable = GetExecutableFileName 'dotnet'
    $dotnetCmd = Get-Command $dotnetExecutable -ErrorAction SilentlyContinue

    if ($dotnetCmd -ne $null) {
      $env:DOTNET_INSTALL_DIR = Split-Path $dotnetCmd.Path -Parent
    }
  }

  $dotnetSdkVersion = $GlobalJson.tools.dotnet

  # Use dotnet installation specified in DOTNET_INSTALL_DIR if it contains the required SDK version,
  # otherwise install the dotnet CLI and SDK to repo local .dotnet directory to avoid potential permission issues.
  if ((-not $globalJsonHasRuntimes) -and (-not [string]::IsNullOrEmpty($env:DOTNET_INSTALL_DIR)) -and (Test-Path(Join-Path $env:DOTNET_INSTALL_DIR "sdk\$dotnetSdkVersion"))) {
    $dotnetRoot = $env:DOTNET_INSTALL_DIR
  } else {
    $dotnetRoot = Join-Path $RepoRoot '.dotnet'

    if (-not (Test-Path(Join-Path $dotnetRoot "sdk\$dotnetSdkVersion"))) {
      if ($install) {
        InstallDotNetSdk $dotnetRoot $dotnetSdkVersion
      } else {
        Write-PipelineTelemetryError -Category 'InitializeToolset' -Message "Unable to find dotnet with SDK version '$dotnetSdkVersion'"
        ExitWithExitCode 1
      }
    }

    $env:DOTNET_INSTALL_DIR = $dotnetRoot
  }

  # Creates a temporary file under the toolset dir.
  # The following code block is protecting against concurrent access so that this function can
  # be called in parallel.
  if ($createSdkLocationFile) {
    do {
      $sdkCacheFileTemp = Join-Path $ToolsetDir $([System.IO.Path]::GetRandomFileName())
    }
    until (!(Test-Path $sdkCacheFileTemp))
    Set-Content -Path $sdkCacheFileTemp -Value $dotnetRoot

    try {
      Move-Item -Force $sdkCacheFileTemp (Join-Path $ToolsetDir 'sdk.txt')
    } catch {
      # Somebody beat us
      Remove-Item -Path $sdkCacheFileTemp
    }
  }

  # Add dotnet to PATH. This prevents any bare invocation of dotnet in custom
  # build steps from using anything other than what we've downloaded.
  # It also ensures that VS msbuild will use the downloaded sdk targets.
  $env:PATH = "$dotnetRoot;$env:PATH"

  # Make Sure that our bootstrapped dotnet cli is available in future steps of the Azure Pipelines build
  Write-PipelinePrependPath -Path $dotnetRoot

  Write-PipelineSetVariable -Name 'DOTNET_MULTILEVEL_LOOKUP' -Value '0'
  Write-PipelineSetVariable -Name 'DOTNET_NOLOGO' -Value '1'

  return $global:_DotNetInstallDir = $dotnetRoot
}

function Retry($downloadBlock, $maxRetries = 5) {
  $retries = 1

  while($true) {
    try {
      & $downloadBlock
      break
    }
    catch {
      Write-PipelineTelemetryError -Category 'InitializeToolset' -Message $_
    }

    if (++$retries -le $maxRetries) {
      $delayInSeconds = [math]::Pow(2, $retries) - 1 # Exponential backoff
      Write-Host "Retrying. Waiting for $delayInSeconds seconds before next attempt ($retries of $maxRetries)."
      Start-Sleep -Seconds $delayInSeconds
    }
    else {
      Write-PipelineTelemetryError -Category 'InitializeToolset' -Message "Unable to download file in $maxRetries attempts."
      break
    }
  }
}

function GetDotNetInstallScript([string] $dotnetRoot) {
  $installScript = Join-Path $dotnetRoot 'dotnet-install.ps1'
  if (!(Test-Path $installScript)) {
    Create-Directory $dotnetRoot
    $ProgressPreference = 'SilentlyContinue' # Don't display the console progress UI - it's a huge perf hit
    $uri = "https://builds.dotnet.microsoft.com/dotnet/scripts/$dotnetInstallScriptVersion/dotnet-install.ps1"

    Retry({
      Write-Host "GET $uri"
      Invoke-WebRequest $uri -OutFile $installScript
    })
  }

  return $installScript
}

function InstallDotNetSdk([string] $dotnetRoot, [string] $version, [string] $architecture = '', [switch] $noPath) {
  InstallDotNet $dotnetRoot $version $architecture '' $false $runtimeSourceFeed $runtimeSourceFeedKey -noPath:$noPath
}

function InstallDotNet([string] $dotnetRoot,
  [string] $version,
  [string] $architecture = '',
  [string] $runtime = '',
  [bool] $skipNonVersionedFiles = $false,
  [string] $runtimeSourceFeed = '',
  [string] $runtimeSourceFeedKey = '',
  [switch] $noPath) {

  $dotnetVersionLabel = "'sdk v$version'"

  if ($runtime -ne '' -and $runtime -ne 'sdk') {
    $runtimePath = $dotnetRoot
    $runtimePath = $runtimePath + "\shared"
    if ($runtime -eq "dotnet") { $runtimePath = $runtimePath + "\Microsoft.NETCore.App" }
    if ($runtime -eq "aspnetcore") { $runtimePath = $runtimePath + "\Microsoft.AspNetCore.App" }
    if ($runtime -eq "windowsdesktop") { $runtimePath = $runtimePath + "\Microsoft.WindowsDesktop.App" }
    $runtimePath = $runtimePath + "\" + $version

    $dotnetVersionLabel = "runtime toolset '$runtime/$architecture v$version'"

    if (Test-Path $runtimePath) {
      Write-Host "  Runtime toolset '$runtime/$architecture v$version' already installed."
      $installSuccess = $true
      Exit
    }
  }

  $installScript = GetDotNetInstallScript $dotnetRoot
  $installParameters = @{
    Version = $version
    InstallDir = $dotnetRoot
  }

  if ($architecture) { $installParameters.Architecture = $architecture }
  if ($runtime) { $installParameters.Runtime = $runtime }
  if ($skipNonVersionedFiles) { $installParameters.SkipNonVersionedFiles = $skipNonVersionedFiles }
  if ($noPath) { $installParameters.NoPath = $True }

  $variations = @()
  $variations += @($installParameters)

  $dotnetBuilds = $installParameters.Clone()
  $dotnetbuilds.AzureFeed = "https://ci.dot.net/public"
  $variations += @($dotnetBuilds)

  if ($runtimeSourceFeed) {
    $runtimeSource = $installParameters.Clone()
    $runtimeSource.AzureFeed = $runtimeSourceFeed
    if ($runtimeSourceFeedKey) {
      $decodedBytes = [System.Convert]::FromBase64String($runtimeSourceFeedKey)
      $decodedString = [System.Text.Encoding]::UTF8.GetString($decodedBytes)
      $runtimeSource.FeedCredential = $decodedString
    }
    $variations += @($runtimeSource)
  }

  $installSuccess = $false
  foreach ($variation in $variations) {
    if ($variation | Get-Member AzureFeed) {
      $location = $variation.AzureFeed
    } else {
      $location = "public location";
    }
    Write-Host "  Attempting to install $dotnetVersionLabel from $location."
    try {
      & $installScript @variation
      $installSuccess = $true
      break
    }
    catch {
      Write-Host "  Failed to install $dotnetVersionLabel from $location."
    }
  }
  if (-not $installSuccess) {
    Write-PipelineTelemetryError -Category 'InitializeToolset' -Message "Failed to install $dotnetVersionLabel from any of the specified locations."
    ExitWithExitCode 1
  }
}

#
# Locates Visual Studio MSBuild installation.
# The preference order for MSBuild to use is as follows:
#
#   1. MSBuild from an active VS command prompt
#   2. MSBuild from a compatible VS installation
#   3. MSBuild from the xcopy tool package
#
# Returns full path to msbuild.exe.
# Throws on failure.
#
function InitializeVisualStudioMSBuild([bool]$install, [object]$vsRequirements = $null) {
  if (-not (IsWindowsPlatform)) {
    throw "Cannot initialize Visual Studio on non-Windows"
  }

  if (Test-Path variable:global:_MSBuildExe) {
    return $global:_MSBuildExe
  }

  # Minimum VS version to require.
  $vsMinVersionReqdStr = '17.7'
  $vsMinVersionReqd = [Version]::new($vsMinVersionReqdStr)

  # If the version of msbuild is going to be xcopied,
  # use this version. Version matches a package here:
  # https://dev.azure.com/dnceng/public/_artifacts/feed/dotnet-eng/NuGet/Microsoft.DotNet.Arcade.MSBuild.Xcopy/versions/17.12.0
  $defaultXCopyMSBuildVersion = '17.12.0'

  if (!$vsRequirements) {
    if (Get-Member -InputObject $GlobalJson.tools -Name 'vs') {
      $vsRequirements = $GlobalJson.tools.vs
    }
    else {
      $vsRequirements = New-Object PSObject -Property @{ version = $vsMinVersionReqdStr }
    }
  }
  $vsMinVersionStr = if ($vsRequirements.version) { $vsRequirements.version } else { $vsMinVersionReqdStr }
  $vsMinVersion = [Version]::new($vsMinVersionStr)

  # Try msbuild command available in the environment.
  if ($env:VSINSTALLDIR -ne $null) {
    $msbuildCmd = Get-Command 'msbuild.exe' -ErrorAction SilentlyContinue
    if ($msbuildCmd -ne $null) {
      # Workaround for https://github.com/dotnet/roslyn/issues/35793
      # Due to this issue $msbuildCmd.Version returns 0.0.0.0 for msbuild.exe 16.2+
      $msbuildVersion = [Version]::new((Get-Item $msbuildCmd.Path).VersionInfo.ProductVersion.Split([char[]]@('-', '+'))[0])

      if ($msbuildVersion -ge $vsMinVersion) {
        return $global:_MSBuildExe = $msbuildCmd.Path
      }

      # Report error - the developer environment is initialized with incompatible VS version.
      throw "Developer Command Prompt for VS $($env:VisualStudioVersion) is not recent enough. Please upgrade to $vsMinVersionStr or build from a plain CMD window"
    }
  }

  # Locate Visual Studio installation or download x-copy msbuild.
  $vsInfo = LocateVisualStudio $vsRequirements
  if ($vsInfo -ne $null) {
    # Ensure vsInstallDir has a trailing slash
    $vsInstallDir = Join-Path $vsInfo.installationPath "\"
    $vsMajorVersion = $vsInfo.installationVersion.Split('.')[0]

    InitializeVisualStudioEnvironmentVariables $vsInstallDir $vsMajorVersion
  } else {
    if (Get-Member -InputObject $GlobalJson.tools -Name 'xcopy-msbuild') {
      $xcopyMSBuildVersion = $GlobalJson.tools.'xcopy-msbuild'
      $vsMajorVersion = $xcopyMSBuildVersion.Split('.')[0]
    } else {
      #if vs version provided in global.json is incompatible (too low) then use the default version for xcopy msbuild download
      if($vsMinVersion -lt $vsMinVersionReqd){
        Write-Host "Using xcopy-msbuild version of $defaultXCopyMSBuildVersion since VS version $vsMinVersionStr provided in global.json is not compatible"
        $xcopyMSBuildVersion = $defaultXCopyMSBuildVersion
        $vsMajorVersion = $xcopyMSBuildVersion.Split('.')[0]
      }
      else{
        # If the VS version IS compatible, look for an xcopy msbuild package
        # with a version matching VS.
        # Note: If this version does not exist, then an explicit version of xcopy msbuild
        # can be specified in global.json. This will be required for pre-release versions of msbuild.
        $vsMajorVersion = $vsMinVersion.Major
        $vsMinorVersion = $vsMinVersion.Minor
        $xcopyMSBuildVersion = "$vsMajorVersion.$vsMinorVersion.0"
      }
    }

    $vsInstallDir = $null
    if ($xcopyMSBuildVersion.Trim() -ine "none") {
        $vsInstallDir = InitializeXCopyMSBuild $xcopyMSBuildVersion $install
        if ($vsInstallDir -eq $null) {
            throw "Could not xcopy msbuild. Please check that package 'Microsoft.DotNet.Arcade.MSBuild.Xcopy @ $xcopyMSBuildVersion' exists on feed 'dotnet-eng'."
        }
    }
    if ($vsInstallDir -eq $null) {
      throw 'Unable to find Visual Studio that has required version and components installed'
    }
  }

  $msbuildVersionDir = if ([int]$vsMajorVersion -lt 16) { "$vsMajorVersion.0" } else { "Current" }

  $local:BinFolder = Join-Path $vsInstallDir "MSBuild\$msbuildVersionDir\Bin"
  $local:Prefer64bit = if (Get-Member -InputObject $vsRequirements -Name 'Prefer64bit') { $vsRequirements.Prefer64bit } else { $false }
  if ($local:Prefer64bit -and (Test-Path(Join-Path $local:BinFolder "amd64"))) {
    $global:_MSBuildExe = Join-Path $local:BinFolder "amd64\msbuild.exe"
  } else {
    $global:_MSBuildExe = Join-Path $local:BinFolder "msbuild.exe"
  }

  return $global:_MSBuildExe
}

function InitializeVisualStudioEnvironmentVariables([string] $vsInstallDir, [string] $vsMajorVersion) {
  $env:VSINSTALLDIR = $vsInstallDir
  Set-Item "env:VS$($vsMajorVersion)0COMNTOOLS" (Join-Path $vsInstallDir "Common7\Tools\")

  $vsSdkInstallDir = Join-Path $vsInstallDir "VSSDK\"
  if (Test-Path $vsSdkInstallDir) {
    Set-Item "env:VSSDK$($vsMajorVersion)0Install" $vsSdkInstallDir
    $env:VSSDKInstall = $vsSdkInstallDir
  }
}

function InstallXCopyMSBuild([string]$packageVersion) {
  return InitializeXCopyMSBuild $packageVersion -install $true
}

function InitializeXCopyMSBuild([string]$packageVersion, [bool]$install) {
  $packageName = 'Microsoft.DotNet.Arcade.MSBuild.Xcopy'
  $packageDir = Join-Path $ToolsDir "msbuild\$packageVersion"
  $packagePath = Join-Path $packageDir "$packageName.$packageVersion.nupkg"

  if (!(Test-Path $packageDir)) {
    if (!$install) {
      return $null
    }

    Create-Directory $packageDir

    Write-Host "Downloading $packageName $packageVersion"
    $ProgressPreference = 'SilentlyContinue' # Don't display the console progress UI - it's a huge perf hit
    Retry({
      Invoke-WebRequest "https://pkgs.dev.azure.com/dnceng/public/_packaging/dotnet-eng/nuget/v3/flat2/$packageName/$packageVersion/$packageName.$packageVersion.nupkg" -OutFile $packagePath
    })

    if (!(Test-Path $packagePath)) {
      Write-PipelineTelemetryError -Category 'InitializeToolset' -Message "See https://dev.azure.com/dnceng/internal/_wiki/wikis/DNCEng%20Services%20Wiki/1074/Updating-Microsoft.DotNet.Arcade.MSBuild.Xcopy-WAS-RoslynTools.MSBuild-(xcopy-msbuild)-generation?anchor=troubleshooting for help troubleshooting issues with XCopy MSBuild"
      throw
    }
    Unzip $packagePath $packageDir
  }

  return Join-Path $packageDir 'tools'
}

#
# Locates Visual Studio instance that meets the minimal requirements specified by tools.vs object in global.json.
#
# The following properties of tools.vs are recognized:
#   "version": "{major}.{minor}"
#       Two part minimal VS version, e.g. "15.9", "16.0", etc.
#   "components": ["componentId1", "componentId2", ...]
#       Array of ids of workload components that must be available in the VS instance.
#       See e.g. https://docs.microsoft.com/en-us/visualstudio/install/workload-component-id-vs-enterprise?view=vs-2017
#
# Returns JSON describing the located VS instance (same format as returned by vswhere),
# or $null if no instance meeting the requirements is found on the machine.
#
function LocateVisualStudio([object]$vsRequirements = $null){
  if (-not (IsWindowsPlatform)) {
    throw "Cannot run vswhere on non-Windows platforms."
  }

  if (Get-Member -InputObject $GlobalJson.tools -Name 'vswhere') {
    $vswhereVersion = $GlobalJson.tools.vswhere
  } else {
    $vswhereVersion = '2.5.2'
  }

  $vsWhereDir = Join-Path $ToolsDir "vswhere\$vswhereVersion"
  $vsWhereExe = Join-Path $vsWhereDir 'vswhere.exe'

  if (!(Test-Path $vsWhereExe)) {
    Create-Directory $vsWhereDir
    Write-Host 'Downloading vswhere'
    Retry({
      Invoke-WebRequest "https://netcorenativeassets.blob.core.windows.net/resource-packages/external/windows/vswhere/$vswhereVersion/vswhere.exe" -OutFile $vswhereExe
    })
  }

  if (!$vsRequirements) { $vsRequirements = $GlobalJson.tools.vs }
  $args = @('-latest', '-format', 'json', '-requires', 'Microsoft.Component.MSBuild', '-products', '*')

  if (!$excludePrereleaseVS) {
    $args += '-prerelease'
  }

  if (Get-Member -InputObject $vsRequirements -Name 'version') {
    $args += '-version'
    $args += $vsRequirements.version
  }

  if (Get-Member -InputObject $vsRequirements -Name 'components') {
    foreach ($component in $vsRequirements.components) {
      $args += '-requires'
      $args += $component
    }
  }

  $vsInfo =& $vsWhereExe $args | ConvertFrom-Json

  if ($lastExitCode -ne 0) {
    return $null
  }

  # use first matching instance
  return $vsInfo[0]
}

function InitializeBuildTool() {
  if (Test-Path variable:global:_BuildTool) {
    # If the requested msbuild parameters do not match, clear the cached variables.
    if($global:_BuildTool.Contains('ExcludePrereleaseVS') -and $global:_BuildTool.ExcludePrereleaseVS -ne $excludePrereleaseVS) {
      Remove-Item variable:global:_BuildTool
      Remove-Item variable:global:_MSBuildExe
    } else {
      return $global:_BuildTool
    }
  }

  if (-not $msbuildEngine) {
    $msbuildEngine = GetDefaultMSBuildEngine
  }

  # Initialize dotnet cli if listed in 'tools'
  $dotnetRoot = $null
  if (Get-Member -InputObject $GlobalJson.tools -Name 'dotnet') {
    $dotnetRoot = InitializeDotNetCli -install:$restore
  }

  if ($msbuildEngine -eq 'dotnet') {
    if (!$dotnetRoot) {
      Write-PipelineTelemetryError -Category 'InitializeToolset' -Message "/global.json must specify 'tools.dotnet'."
      ExitWithExitCode 1
    }
    $dotnetPath = Join-Path $dotnetRoot (GetExecutableFileName 'dotnet')

    # Use override if it exists - commonly set by source-build
    if ($null -eq $env:_OverrideArcadeInitializeBuildToolFramework) {
      $initializeBuildToolFramework="net9.0"
    } else {
      $initializeBuildToolFramework=$env:_OverrideArcadeInitializeBuildToolFramework
    }

    $buildTool = @{ Path = $dotnetPath; Command = 'msbuild'; Tool = 'dotnet'; Framework = $initializeBuildToolFramework }
  } elseif ($msbuildEngine -eq "vs") {
    try {
      $msbuildPath = InitializeVisualStudioMSBuild -install:$restore
    } catch {
      Write-PipelineTelemetryError -Category 'InitializeToolset' -Message $_
      ExitWithExitCode 1
    }

    $buildTool = @{ Path = $msbuildPath; Command = ""; Tool = "vs"; Framework = "net472"; ExcludePrereleaseVS = $excludePrereleaseVS }
  } else {
    Write-PipelineTelemetryError -Category 'InitializeToolset' -Message "Unexpected value of -msbuildEngine: '$msbuildEngine'."
    ExitWithExitCode 1
  }

  return $global:_BuildTool = $buildTool
}

function GetDefaultMSBuildEngine() {
  # Presence of tools.vs indicates the repo needs to build using VS msbuild on Windows.
  if (Get-Member -InputObject $GlobalJson.tools -Name 'vs') {
    return 'vs'
  }

  if (Get-Member -InputObject $GlobalJson.tools -Name 'dotnet') {
    return 'dotnet'
  }

  Write-PipelineTelemetryError -Category 'InitializeToolset' -Message "-msbuildEngine must be specified, or /global.json must specify 'tools.dotnet' or 'tools.vs'."
  ExitWithExitCode 1
}

function GetNuGetPackageCachePath() {
  if ($env:NUGET_PACKAGES -eq $null) {
    # Use local cache on CI to ensure deterministic build.
    # Avoid using the http cache as workaround for https://github.com/NuGet/Home/issues/3116
    # use global cache in dev builds to avoid cost of downloading packages.
    # For directory normalization, see also: https://github.com/NuGet/Home/issues/7968
    if ($useGlobalNuGetCache) {
      $env:NUGET_PACKAGES = Join-Path $env:UserProfile '.nuget\packages\'
    } else {
      $env:NUGET_PACKAGES = Join-Path $RepoRoot '.packages\'
      $env:RESTORENOHTTPCACHE = $true
    }
  }

  return $env:NUGET_PACKAGES
}

# Returns a full path to an Arcade SDK task project file.
function GetSdkTaskProject([string]$taskName) {
  return Join-Path (Split-Path (InitializeToolset) -Parent) "SdkTasks\$taskName.proj"
}

function InitializeNativeTools() {
  if (-Not (Test-Path variable:DisableNativeToolsetInstalls) -And (Get-Member -InputObject $GlobalJson -Name "native-tools")) {
    $nativeArgs= @{}
    if ($ci) {
      $nativeArgs = @{
        InstallDirectory = "$ToolsDir"
      }
    }
    if ($env:NativeToolsOnMachine) {
      Write-Host "Variable NativeToolsOnMachine detected, enabling native tool path promotion..."
      $nativeArgs += @{ PathPromotion = $true }
    }
    & "$PSScriptRoot/init-tools-native.ps1" @nativeArgs
  }
}

function Read-ArcadeSdkVersion() {
  return $GlobalJson.'msbuild-sdks'.'Microsoft.DotNet.Arcade.Sdk'
}

function InitializeToolset() {
  # For Unified Build/Source-build support, check whether the environment variable is
  # set. If it is, then use this as the toolset build project.
  if ($env:_InitializeToolset -ne $null) {
    return $global:_InitializeToolset = $env:_InitializeToolset
  }

  if (Test-Path variable:global:_InitializeToolset) {
    return $global:_InitializeToolset
  }

  $nugetCache = GetNuGetPackageCachePath

  $toolsetVersion = Read-ArcadeSdkVersion
  $toolsetLocationFile = Join-Path $ToolsetDir "$toolsetVersion.txt"

  if (Test-Path $toolsetLocationFile) {
    $path = Get-Content $toolsetLocationFile -TotalCount 1
    if (Test-Path $path) {
      return $global:_InitializeToolset = $path
    }
  }

  if (-not $restore) {
    Write-PipelineTelemetryError -Category 'InitializeToolset' -Message "Toolset version $toolsetVersion has not been restored."
    ExitWithExitCode 1
  }

  $buildTool = InitializeBuildTool

  $proj = Join-Path $ToolsetDir 'restore.proj'
  $bl = if ($binaryLog) { '/bl:' + (Join-Path $LogDir 'ToolsetRestore.binlog') } else { '' }

  '<Project Sdk="Microsoft.DotNet.Arcade.Sdk"/>' | Set-Content $proj

  MSBuild-Core $proj $bl /t:__WriteToolsetLocation /clp:ErrorsOnly`;NoSummary /p:__ToolsetLocationOutputFile=$toolsetLocationFile

  $path = Get-Content $toolsetLocationFile -Encoding UTF8 -TotalCount 1
  if (!(Test-Path $path)) {
    throw "Invalid toolset path: $path"
  }

  return $global:_InitializeToolset = $path
}

function ExitWithExitCode([int] $exitCode) {
  if ($ci -and $prepareMachine) {
    Stop-Processes
  }
  exit $exitCode
}

# Check if $LASTEXITCODE is a nonzero exit code (NZEC). If so, print a Azure Pipeline error for
# diagnostics, then exit the script with the $LASTEXITCODE.
function Exit-IfNZEC([string] $category = "General") {
  Write-Host "Exit code $LASTEXITCODE"
  if ($LASTEXITCODE -ne 0) {
    $message = "Last command failed with exit code $LASTEXITCODE."
    Write-PipelineTelemetryError -Force -Category $category -Message $message
    ExitWithExitCode $LASTEXITCODE
  }
}

function Stop-Processes() {
  Write-Host 'Killing running build processes...'
  foreach ($processName in $processesToStopOnExit) {
    Get-Process -Name $processName -ErrorAction SilentlyContinue | Stop-Process
  }
}

#
# Executes msbuild (or 'dotnet msbuild') with arguments passed to the function.
# The arguments are automatically quoted.
# Terminates the script if the build fails.
#
function MSBuild() {
  if ($pipelinesLog) {
    $buildTool = InitializeBuildTool

    if ($ci -and $buildTool.Tool -eq 'dotnet') {
      $env:NUGET_PLUGIN_HANDSHAKE_TIMEOUT_IN_SECONDS = 20
      $env:NUGET_PLUGIN_REQUEST_TIMEOUT_IN_SECONDS = 20
      Write-PipelineSetVariable -Name 'NUGET_PLUGIN_HANDSHAKE_TIMEOUT_IN_SECONDS' -Value '20'
      Write-PipelineSetVariable -Name 'NUGET_PLUGIN_REQUEST_TIMEOUT_IN_SECONDS' -Value '20'
    }

    Enable-Nuget-EnhancedRetry

    $toolsetBuildProject = InitializeToolset
    $basePath = Split-Path -parent $toolsetBuildProject
    $possiblePaths = @(
      # new scripts need to work with old packages, so we need to look for the old names/versions
      (Join-Path $basePath (Join-Path $buildTool.Framework 'Microsoft.DotNet.ArcadeLogging.dll')),
      (Join-Path $basePath (Join-Path $buildTool.Framework 'Microsoft.DotNet.Arcade.Sdk.dll')),
      (Join-Path $basePath (Join-Path net7.0 'Microsoft.DotNet.ArcadeLogging.dll')),
      (Join-Path $basePath (Join-Path net7.0 'Microsoft.DotNet.Arcade.Sdk.dll')),
      (Join-Path $basePath (Join-Path net8.0 'Microsoft.DotNet.ArcadeLogging.dll')),
      (Join-Path $basePath (Join-Path net8.0 'Microsoft.DotNet.Arcade.Sdk.dll'))
    )
    $selectedPath = $null
    foreach ($path in $possiblePaths) {
      if (Test-Path $path -PathType Leaf) {
        $selectedPath = $path
        break
      }
    }
    if (-not $selectedPath) {
      Write-PipelineTelemetryError -Category 'Build' -Message 'Unable to find arcade sdk logger assembly.'
      ExitWithExitCode 1
    }
    $args += "/logger:$selectedPath"
  }

  MSBuild-Core @args
}

#
# Executes msbuild (or 'dotnet msbuild') with arguments passed to the function.
# The arguments are automatically quoted.
# Terminates the script if the build fails.
#
function MSBuild-Core() {
  if ($ci) {
    if (!$binaryLog -and !$excludeCIBinarylog) {
      Write-PipelineTelemetryError -Category 'Build' -Message 'Binary log must be enabled in CI build, or explicitly opted-out from with the -excludeCIBinarylog switch.'
      ExitWithExitCode 1
    }

    if ($nodeReuse) {
      Write-PipelineTelemetryError -Category 'Build' -Message 'Node reuse must be disabled in CI build.'
      ExitWithExitCode 1
    }
  }

  Enable-Nuget-EnhancedRetry

  $buildTool = InitializeBuildTool

  $cmdArgs = "$($buildTool.Command) /m /nologo /clp:Summary /v:$verbosity /nr:$nodeReuse /p:ContinuousIntegrationBuild=$ci"

  if ($warnAsError) {
    $cmdArgs += ' /warnaserror /p:TreatWarningsAsErrors=true'
  }
  else {
    $cmdArgs += ' /p:TreatWarningsAsErrors=false'
  }

  foreach ($arg in $args) {
    if ($null -ne $arg -and $arg.Trim() -ne "") {
      if ($arg.EndsWith('\')) {
        $arg = $arg + "\"
      }
      $cmdArgs += " `"$arg`""
    }
  }

  # Be sure quote the path in case there are spaces in the dotnet installation location.
  $env:ARCADE_BUILD_TOOL_COMMAND = "`"$($buildTool.Path)`" $cmdArgs"

  $exitCode = Exec-Process $buildTool.Path $cmdArgs

  if ($exitCode -ne 0) {
    # We should not Write-PipelineTaskError here because that message shows up in the build summary
    # The build already logged an error, that's the reason it failed. Producing an error here only adds noise.
    Write-Host "Build failed with exit code $exitCode. Check errors above." -ForegroundColor Red

    $buildLog = GetMSBuildBinaryLogCommandLineArgument $args
    if ($null -ne $buildLog) {
      Write-Host "See log: $buildLog" -ForegroundColor DarkGray
    }

    # When running on Azure Pipelines, override the returned exit code to avoid double logging.
    # Skip this when the build is a child of the VMR orchestrator build.
    if ($ci -and $env:SYSTEM_TEAMPROJECT -ne $null -and !$productBuild -and -not($properties -like "*DotNetBuildRepo=true*")) {
      Write-PipelineSetResult -Result "Failed" -Message "msbuild execution failed."
      # Exiting with an exit code causes the azure pipelines task to log yet another "noise" error
      # The above Write-PipelineSetResult will cause the task to be marked as failure without adding yet another error
      ExitWithExitCode 0
    } else {
      ExitWithExitCode $exitCode
    }
  }
}

function GetMSBuildBinaryLogCommandLineArgument($arguments) {
  foreach ($argument in $arguments) {
    if ($argument -ne $null) {
      $arg = $argument.Trim()
      if ($arg.StartsWith('/bl:', "OrdinalIgnoreCase")) {
        return $arg.Substring('/bl:'.Length)
      }

      if ($arg.StartsWith('/binaryLogger:', 'OrdinalIgnoreCase')) {
        return $arg.Substring('/binaryLogger:'.Length)
      }
    }
  }

  return $null
}

function GetExecutableFileName($baseName) {
  if (IsWindowsPlatform) {
    return "$baseName.exe"
  }
  else {
    return $baseName
  }
}

function IsWindowsPlatform() {
  return [environment]::OSVersion.Platform -eq [PlatformID]::Win32NT
}

function Get-Darc($version) {
  $darcPath  = "$TempDir\darc\$([guid]::NewGuid())"
  if ($version -ne $null) {
    & $PSScriptRoot\darc-init.ps1 -toolpath $darcPath -darcVersion $version | Out-Host
  } else {
    & $PSScriptRoot\darc-init.ps1 -toolpath $darcPath | Out-Host
  }
  return "$darcPath\darc.exe"
}

. $PSScriptRoot\pipeline-logging-functions.ps1

$RepoRoot = Resolve-Path (Join-Path $PSScriptRoot '..\..\')
$EngRoot = Resolve-Path (Join-Path $PSScriptRoot '..')
$ArtifactsDir = Join-Path $RepoRoot 'artifacts'
$ToolsetDir = Join-Path $ArtifactsDir 'toolset'
$ToolsDir = Join-Path $RepoRoot '.tools'
$LogDir = Join-Path (Join-Path $ArtifactsDir 'log') $configuration
$TempDir = Join-Path (Join-Path $ArtifactsDir 'tmp') $configuration
$GlobalJson = Get-Content -Raw -Path (Join-Path $RepoRoot 'global.json') | ConvertFrom-Json
# true if global.json contains a "runtimes" section
$globalJsonHasRuntimes = if ($GlobalJson.tools.PSObject.Properties.Name -Match 'runtimes') { $true } else { $false }

Create-Directory $ToolsetDir
Create-Directory $TempDir
Create-Directory $LogDir

Write-PipelineSetVariable -Name 'Artifacts' -Value $ArtifactsDir
Write-PipelineSetVariable -Name 'Artifacts.Toolset' -Value $ToolsetDir
Write-PipelineSetVariable -Name 'Artifacts.Log' -Value $LogDir
Write-PipelineSetVariable -Name 'TEMP' -Value $TempDir
Write-PipelineSetVariable -Name 'TMP' -Value $TempDir

# Import custom tools configuration, if present in the repo.
# Note: Import in global scope so that the script set top-level variables without qualification.
if (!$disableConfigureToolsetImport) {
  $configureToolsetScript = Join-Path $EngRoot 'configure-toolset.ps1'
  if (Test-Path $configureToolsetScript) {
    . $configureToolsetScript
    if ((Test-Path variable:failOnConfigureToolsetError) -And $failOnConfigureToolsetError) {
      if ((Test-Path variable:LastExitCode) -And ($LastExitCode -ne 0)) {
        Write-PipelineTelemetryError -Category 'Build' -Message 'configure-toolset.ps1 returned a non-zero exit code'
        ExitWithExitCode $LastExitCode
      }
    }
  }
}

#
# If $ci flag is set, turn on (and log that we did) special environment variables for improved Nuget client retry logic.
#
function Enable-Nuget-EnhancedRetry() {
    if ($ci) {
      Write-Host "Setting NUGET enhanced retry environment variables"
      $env:NUGET_ENABLE_ENHANCED_HTTP_RETRY = 'true'
      $env:NUGET_ENHANCED_MAX_NETWORK_TRY_COUNT = 6
      $env:NUGET_ENHANCED_NETWORK_RETRY_DELAY_MILLISECONDS = 1000
      $env:NUGET_RETRY_HTTP_429 = 'true'
      Write-PipelineSetVariable -Name 'NUGET_ENABLE_ENHANCED_HTTP_RETRY' -Value 'true'
      Write-PipelineSetVariable -Name 'NUGET_ENHANCED_MAX_NETWORK_TRY_COUNT' -Value '6'
      Write-PipelineSetVariable -Name 'NUGET_ENHANCED_NETWORK_RETRY_DELAY_MILLISECONDS' -Value '1000'
      Write-PipelineSetVariable -Name 'NUGET_RETRY_HTTP_429' -Value 'true'
    }
}



================================================
FILE: eng/common/tools.sh
================================================
#!/usr/bin/env bash

# Initialize variables if they aren't already defined.

# CI mode - set to true on CI server for PR validation build or official build.
ci=${ci:-false}

# Set to true to use the pipelines logger which will enable Azure logging output.
# https://github.com/Microsoft/azure-pipelines-tasks/blob/master/docs/authoring/commands.md
# This flag is meant as a temporary opt-opt for the feature while validate it across
# our consumers. It will be deleted in the future.
if [[ "$ci" == true ]]; then
  pipelines_log=${pipelines_log:-true}
else
  pipelines_log=${pipelines_log:-false}
fi

# Build configuration. Common values include 'Debug' and 'Release', but the repository may use other names.
configuration=${configuration:-'Debug'}

# Set to true to opt out of outputting binary log while running in CI
exclude_ci_binary_log=${exclude_ci_binary_log:-false}

if [[ "$ci" == true && "$exclude_ci_binary_log" == false ]]; then
  binary_log_default=true
else
  binary_log_default=false
fi

# Set to true to output binary log from msbuild. Note that emitting binary log slows down the build.
binary_log=${binary_log:-$binary_log_default}

# Turns on machine preparation/clean up code that changes the machine state (e.g. kills build processes).
prepare_machine=${prepare_machine:-false}

# True to restore toolsets and dependencies.
restore=${restore:-true}

# Adjusts msbuild verbosity level.
verbosity=${verbosity:-'minimal'}

# Set to true to reuse msbuild nodes. Recommended to not reuse on CI.
if [[ "$ci" == true ]]; then
  node_reuse=${node_reuse:-false}
else
  node_reuse=${node_reuse:-true}
fi

# Configures warning treatment in msbuild.
warn_as_error=${warn_as_error:-true}

# True to attempt using .NET Core already that meets requirements specified in global.json
# installed on the machine instead of downloading one.
use_installed_dotnet_cli=${use_installed_dotnet_cli:-true}

# Enable repos to use a particular version of the on-line dotnet-install scripts.
#    default URL: https://builds.dotnet.microsoft.com/dotnet/scripts/v1/dotnet-install.sh
dotnetInstallScriptVersion=${dotnetInstallScriptVersion:-'v1'}

# True to use global NuGet cache instead of restoring packages to repository-local directory.
if [[ "$ci" == true ]]; then
  use_global_nuget_cache=${use_global_nuget_cache:-false}
else
  use_global_nuget_cache=${use_global_nuget_cache:-true}
fi

# Used when restoring .NET SDK from alternative feeds
runtime_source_feed=${runtime_source_feed:-''}
runtime_source_feed_key=${runtime_source_feed_key:-''}

# True if the build is a product build
product_build=${product_build:-false}

# Resolve any symlinks in the given path.
function ResolvePath {
  local path=$1

  while [[ -h $path ]]; do
    local dir="$( cd -P "$( dirname "$path" )" && pwd )"
    path="$(readlink "$path")"

    # if $path was a relative symlink, we need to resolve it relative to the path where the
    # symlink file was located
    [[ $path != /* ]] && path="$dir/$path"
  done

  # return value
  _ResolvePath="$path"
}

# ReadVersionFromJson [json key]
function ReadGlobalVersion {
  local key=$1

  if command -v jq &> /dev/null; then
    _ReadGlobalVersion="$(jq -r ".[] | select(has(\"$key\")) | .\"$key\"" "$global_json_file")"
  elif [[ "$(cat "$global_json_file")" =~ \"$key\"[[:space:]\:]*\"([^\"]+) ]]; then
    _ReadGlobalVersion=${BASH_REMATCH[1]}
  fi

  if [[ -z "$_ReadGlobalVersion" ]]; then
    Write-PipelineTelemetryError -category 'Build' "Error: Cannot find \"$key\" in $global_json_file"
    ExitWithExitCode 1
  fi
}

function InitializeDotNetCli {
  if [[ -n "${_InitializeDotNetCli:-}" ]]; then
    return
  fi

  local install=$1

  # Don't resolve runtime, shared framework, or SDK from other locations to ensure build determinism
  export DOTNET_MULTILEVEL_LOOKUP=0

  # Disable first run since we want to control all package sources
  export DOTNET_NOLOGO=1

  # Disable telemetry on CI
  if [[ $ci == true ]]; then
    export DOTNET_CLI_TELEMETRY_OPTOUT=1
  fi

  # LTTNG is the logging infrastructure used by Core CLR. Need this variable set
  # so it doesn't output warnings to the console.
  export LTTNG_HOME="$HOME"

  # Find the first path on $PATH that contains the dotnet.exe
  if [[ "$use_installed_dotnet_cli" == true && $global_json_has_runtimes == false && -z "${DOTNET_INSTALL_DIR:-}" ]]; then
    local dotnet_path=`command -v dotnet`
    if [[ -n "$dotnet_path" ]]; then
      ResolvePath "$dotnet_path"
      export DOTNET_INSTALL_DIR=`dirname "$_ResolvePath"`
    fi
  fi

  ReadGlobalVersion "dotnet"
  local dotnet_sdk_version=$_ReadGlobalVersion
  local dotnet_root=""

  # Use dotnet installation specified in DOTNET_INSTALL_DIR if it contains the required SDK version,
  # otherwise install the dotnet CLI and SDK to repo local .dotnet directory to avoid potential permission issues.
  if [[ $global_json_has_runtimes == false && -n "${DOTNET_INSTALL_DIR:-}" && -d "$DOTNET_INSTALL_DIR/sdk/$dotnet_sdk_version" ]]; then
    dotnet_root="$DOTNET_INSTALL_DIR"
  else
    dotnet_root="${repo_root}.dotnet"

    export DOTNET_INSTALL_DIR="$dotnet_root"

    if [[ ! -d "$DOTNET_INSTALL_DIR/sdk/$dotnet_sdk_version" ]]; then
      if [[ "$install" == true ]]; then
        InstallDotNetSdk "$dotnet_root" "$dotnet_sdk_version"
      else
        Write-PipelineTelemetryError -category 'InitializeToolset' "Unable to find dotnet with SDK version '$dotnet_sdk_version'"
        ExitWithExitCode 1
      fi
    fi
  fi

  # Add dotnet to PATH. This prevents any bare invocation of dotnet in custom
  # build steps from using anything other than what we've downloaded.
  Write-PipelinePrependPath -path "$dotnet_root"

  Write-PipelineSetVariable -name "DOTNET_MULTILEVEL_LOOKUP" -value "0"
  Write-PipelineSetVariable -name "DOTNET_NOLOGO" -value "1"

  # return value
  _InitializeDotNetCli="$dotnet_root"
}

function InstallDotNetSdk {
  local root=$1
  local version=$2
  local architecture="unset"
  if [[ $# -ge 3 ]]; then
    architecture=$3
  fi
  InstallDotNet "$root" "$version" $architecture 'sdk' 'true' $runtime_source_feed $runtime_source_feed_key
}

function InstallDotNet {
  local root=$1
  local version=$2
  local runtime=$4

  local dotnetVersionLabel="'$runtime v$version'"
  if [[ -n "${4:-}" ]] && [ "$4" != 'sdk' ]; then
    runtimePath="$root"
    runtimePath="$runtimePath/shared"
    case "$runtime" in
      dotnet)
        runtimePath="$runtimePath/Microsoft.NETCore.App"
        ;;
      aspnetcore)
        runtimePath="$runtimePath/Microsoft.AspNetCore.App"
        ;;
      windowsdesktop)
        runtimePath="$runtimePath/Microsoft.WindowsDesktop.App"
        ;;
      *)
        ;;
    esac
    runtimePath="$runtimePath/$version"

    dotnetVersionLabel="runtime toolset '$runtime/$architecture v$version'"

    if [ -d "$runtimePath" ]; then
      echo "  Runtime toolset '$runtime/$architecture v$version' already installed."
      local installSuccess=1
      return
    fi
  fi

  GetDotNetInstallScript "$root"
  local install_script=$_GetDotNetInstallScript

  local installParameters=(--version $version --install-dir "$root")

  if [[ -n "${3:-}" ]] && [ "$3" != 'unset' ]; then
    installParameters+=(--architecture $3)
  fi
  if [[ -n "${4:-}" ]] && [ "$4" != 'sdk' ]; then
    installParameters+=(--runtime $4)
  fi
  if [[ "$#" -ge "5" ]] && [[ "$5" != 'false' ]]; then
    installParameters+=(--skip-non-versioned-files)
  fi

  local variations=() # list of variable names with parameter arrays in them

  local public_location=("${installParameters[@]}")
  variations+=(public_location)

  local dotnetbuilds=("${installParameters[@]}" --azure-feed "https://ci.dot.net/public")
  variations+=(dotnetbuilds)

  if [[ -n "${6:-}" ]]; then
    variations+=(private_feed)
    local private_feed=("${installParameters[@]}" --azure-feed $6)
    if [[ -n "${7:-}" ]]; then
      # The 'base64' binary on alpine uses '-d' and doesn't support '--decode'
      # '-d'. To work around this, do a simple detection and switch the parameter
      # accordingly.
      decodeArg="--decode"
      if base64 --help 2>&1 | grep -q "BusyBox"; then
          decodeArg="-d"
      fi
      decodedFeedKey=`echo $7 | base64 $decodeArg`
      private_feed+=(--feed-credential $decodedFeedKey)
    fi
  fi

  local installSuccess=0
  for variationName in "${variations[@]}"; do
    local name="$variationName[@]"
    local variation=("${!name}")
    echo "  Attempting to install $dotnetVersionLabel from $variationName."
    bash "$install_script" "${variation[@]}" && installSuccess=1
    if [[ "$installSuccess" -eq 1 ]]; then
      break
    fi

    echo "  Failed to install $dotnetVersionLabel from $variationName."
  done

  if [[ "$installSuccess" -eq 0 ]]; then
    Write-PipelineTelemetryError -category 'InitializeToolset' "Failed to install $dotnetVersionLabel from any of the specified locations."
    ExitWithExitCode 1
  fi
}

function with_retries {
  local maxRetries=5
  local retries=1
  echo "Trying to run '$@' for maximum of $maxRetries attempts."
  while [[ $((retries++)) -le $maxRetries ]]; do
    "$@"

    if [[ $? == 0 ]]; then
      echo "Ran '$@' successfully."
      return 0
    fi

    timeout=$((3**$retries-1))
    echo "Failed to execute '$@'. Waiting $timeout seconds before next attempt ($retries out of $maxRetries)." 1>&2
    sleep $timeout
  done

  echo "Failed to execute '$@' for $maxRetries times." 1>&2

  return 1
}

function GetDotNetInstallScript {
  local root=$1
  local install_script="$root/dotnet-install.sh"
  local install_script_url="https://builds.dotnet.microsoft.com/dotnet/scripts/$dotnetInstallScriptVersion/dotnet-install.sh"

  if [[ ! -a "$install_script" ]]; then
    mkdir -p "$root"

    echo "Downloading '$install_script_url'"

    # Use curl if available, otherwise use wget
    if command -v curl > /dev/null; then
      # first, try directly, if this fails we will retry with verbose logging
      curl "$install_script_url" -sSL --retry 10 --create-dirs -o "$install_script" || {
        if command -v openssl &> /dev/null; then
          echo "Curl failed; dumping some information about dotnet.microsoft.com for later investigation"
          echo | openssl s_client -showcerts -servername dotnet.microsoft.com  -connect dotnet.microsoft.com:443 || true
        fi
        echo "Will now retry the same URL with verbose logging."
        with_retries curl "$install_script_url" -sSL --verbose --retry 10 --create-dirs -o "$install_script" || {
          local exit_code=$?
          Write-PipelineTelemetryError -category 'InitializeToolset' "Failed to acquire dotnet install script (exit code '$exit_code')."
          ExitWithExitCode $exit_code
        }
      }
    else
      with_retries wget -v -O "$install_script" "$install_script_url" || {
        local exit_code=$?
        Write-PipelineTelemetryError -category 'InitializeToolset' "Failed to acquire dotnet install script (exit code '$exit_code')."
        ExitWithExitCode $exit_code
      }
    fi
  fi
  # return value
  _GetDotNetInstallScript="$install_script"
}

function InitializeBuildTool {
  if [[ -n "${_InitializeBuildTool:-}" ]]; then
    return
  fi

  InitializeDotNetCli $restore

  # return values
  _InitializeBuildTool="$_InitializeDotNetCli/dotnet"
  _InitializeBuildToolCommand="msbuild"
  # use override if it exists - commonly set by source-build
  if [[ "${_OverrideArcadeInitializeBuildToolFramework:-x}" == "x" ]]; then
    _InitializeBuildToolFramework="net9.0"
  else
    _InitializeBuildToolFramework="${_OverrideArcadeInitializeBuildToolFramework}"
  fi
}

# Set RestoreNoHttpCache as a workaround for https://github.com/NuGet/Home/issues/3116
function GetNuGetPackageCachePath {
  if [[ -z ${NUGET_PACKAGES:-} ]]; then
    if [[ "$use_global_nuget_cache" == true ]]; then
      export NUGET_PACKAGES="$HOME/.nuget/packages/"
    else
      export NUGET_PACKAGES="$repo_root/.packages/"
      export RESTORENOHTTPCACHE=true
    fi
  fi

  # return value
  _GetNuGetPackageCachePath=$NUGET_PACKAGES
}

function InitializeNativeTools() {
  if [[ -n "${DisableNativeToolsetInstalls:-}" ]]; then
    return
  fi
  if grep -Fq "native-tools" $global_json_file
  then
    local nativeArgs=""
    if [[ "$ci" == true ]]; then
      nativeArgs="--installDirectory $tools_dir"
    fi
    "$_script_dir/init-tools-native.sh" $nativeArgs
  fi
}

function InitializeToolset {
  if [[ -n "${_InitializeToolset:-}" ]]; then
    return
  fi

  GetNuGetPackageCachePath

  ReadGlobalVersion "Microsoft.DotNet.Arcade.Sdk"

  local toolset_version=$_ReadGlobalVersion
  local toolset_location_file="$toolset_dir/$toolset_version.txt"

  if [[ -a "$toolset_location_file" ]]; then
    local path=`cat "$toolset_location_file"`
    if [[ -a "$path" ]]; then
      # return value
      _InitializeToolset="$path"
      return
    fi
  fi

  if [[ "$restore" != true ]]; then
    Write-PipelineTelemetryError -category 'InitializeToolset' "Toolset version $toolset_version has not been restored."
    ExitWithExitCode 2
  fi

  local proj="$toolset_dir/restore.proj"

  local bl=""
  if [[ "$binary_log" == true ]]; then
    bl="/bl:$log_dir/ToolsetRestore.binlog"
  fi

  echo '<Project Sdk="Microsoft.DotNet.Arcade.Sdk"/>' > "$proj"
  MSBuild-Core "$proj" $bl /t:__WriteToolsetLocation /clp:ErrorsOnly\;NoSummary /p:__ToolsetLocationOutputFile="$toolset_location_file"

  local toolset_build_proj=`cat "$toolset_location_file"`

  if [[ ! -a "$toolset_build_proj" ]]; then
    Write-PipelineTelemetryError -category 'Build' "Invalid toolset path: $toolset_build_proj"
    ExitWithExitCode 3
  fi

  # return value
  _InitializeToolset="$toolset_build_proj"
}

function ExitWithExitCode {
  if [[ "$ci" == true && "$prepare_machine" == true ]]; then
    StopProcesses
  fi
  exit $1
}

function StopProcesses {
  echo "Killing running build processes..."
  pkill -9 "dotnet" || true
  pkill -9 "vbcscompiler" || true
  return 0
}

function MSBuild {
  local args=( "$@" )
  if [[ "$pipelines_log" == true ]]; then
    InitializeBuildTool
    InitializeToolset

    if [[ "$ci" == true ]]; then
      export NUGET_PLUGIN_HANDSHAKE_TIMEOUT_IN_SECONDS=20
      export NUGET_PLUGIN_REQUEST_TIMEOUT_IN_SECONDS=20
      Write-PipelineSetVariable -name "NUGET_PLUGIN_HANDSHAKE_TIMEOUT_IN_SECONDS" -value "20"
      Write-PipelineSetVariable -name "NUGET_PLUGIN_REQUEST_TIMEOUT_IN_SECONDS" -value "20"
    fi

    local toolset_dir="${_InitializeToolset%/*}"
    # new scripts need to work with old packages, so we need to look for the old names/versions
    local selectedPath=
    local possiblePaths=()
    possiblePaths+=( "$toolset_dir/$_InitializeBuildToolFramework/Microsoft.DotNet.ArcadeLogging.dll" )
    possiblePaths+=( "$toolset_dir/$_InitializeBuildToolFramework/Microsoft.DotNet.Arcade.Sdk.dll" )
    possiblePaths+=( "$toolset_dir/net7.0/Microsoft.DotNet.ArcadeLogging.dll" )
    possiblePaths+=( "$toolset_dir/net7.0/Microsoft.DotNet.Arcade.Sdk.dll" )
    possiblePaths+=( "$toolset_dir/net8.0/Microsoft.DotNet.ArcadeLogging.dll" )
    possiblePaths+=( "$toolset_dir/net8.0/Microsoft.DotNet.Arcade.Sdk.dll" )
    for path in "${possiblePaths[@]}"; do
      if [[ -f $path ]]; then
        selectedPath=$path
        break
      fi
    done
    if [[ -z "$selectedPath" ]]; then
      Write-PipelineTelemetryError -category 'Build'  "Unable to find arcade sdk logger assembly."
      ExitWithExitCode 1
    fi
    args+=( "-logger:$selectedPath" )
  fi

  MSBuild-Core "${args[@]}"
}

function MSBuild-Core {
  if [[ "$ci" == true ]]; then
    if [[ "$binary_log" != true && "$exclude_ci_binary_log" != true ]]; then
      Write-PipelineTelemetryError -category 'Build'  "Binary log must be enabled in CI build, or explicitly opted-out from with the -noBinaryLog switch."
      ExitWithExitCode 1
    fi

    if [[ "$node_reuse" == true ]]; then
      Write-PipelineTelemetryError -category 'Build'  "Node reuse must be disabled in CI build."
      ExitWithExitCode 1
    fi
  fi

  InitializeBuildTool

  local warnaserror_switch=""
  if [[ $warn_as_error == true ]]; then
    warnaserror_switch="/warnaserror"
  fi

  function RunBuildTool {
    export ARCADE_BUILD_TOOL_COMMAND="$_InitializeBuildTool $@"

    "$_InitializeBuildTool" "$@" || {
      local exit_code=$?
      # We should not Write-PipelineTaskError here because that message shows up in the build summary
      # The build already logged an error, that's the reason it failed. Producing an error here only adds noise.
      echo "Build failed with exit code $exit_code. Check errors above."

      # When running on Azure Pipelines, override the returned exit code to avoid double logging.
      # Skip this when the build is a child of the VMR orchestrator build.
      if [[ "$ci" == true && -n ${SYSTEM_TEAMPROJECT:-} && "$product_build" != true && "$properties" != *"DotNetBuildRepo=true"* ]]; then
        Write-PipelineSetResult -result "Failed" -message "msbuild execution failed."
        # Exiting with an exit code causes the azure pipelines task to log yet another "noise" error
        # The above Write-PipelineSetResult will cause the task to be marked as failure without adding yet another error
        ExitWithExitCode 0
      else
        ExitWithExitCode $exit_code
      fi
    }
  }

  RunBuildTool "$_InitializeBuildToolCommand" /m /nologo /clp:Summary /v:$verbosity /nr:$node_reuse $warnaserror_switch /p:TreatWarningsAsErrors=$warn_as_error /p:ContinuousIntegrationBuild=$ci "$@"
}

function GetDarc {
    darc_path="$temp_dir/darc"
    version="$1"

    if [[ -n "$version" ]]; then
      version="--darcversion $version"
    fi

    "$eng_root/common/darc-init.sh" --toolpath "$darc_path" $version
}

ResolvePath "${BASH_SOURCE[0]}"
_script_dir=`dirname "$_ResolvePath"`

. "$_script_dir/pipeline-logging-functions.sh"

eng_root=`cd -P "$_script_dir/.." && pwd`
repo_root=`cd -P "$_script_dir/../.." && pwd`
repo_root="${repo_root}/"
artifacts_dir="${repo_root}artifacts"
toolset_dir="$artifacts_dir/toolset"
tools_dir="${repo_root}.tools"
log_dir="$artifacts_dir/log/$configuration"
temp_dir="$artifacts_dir/tmp/$configuration"

global_json_file="${repo_root}global.json"
# determine if global.json contains a "runtimes" entry
global_json_has_runtimes=false
if command -v jq &> /dev/null; then
  if jq -e '.tools | has("runtimes")' "$global_json_file" &> /dev/null; then
    global_json_has_runtimes=true
  fi
elif [[ "$(cat "$global_json_file")" =~ \"runtimes\"[[:space:]\:]*\{ ]]; then
  global_json_has_runtimes=true
fi

# HOME may not be defined in some scenarios, but it is required by NuGet
if [[ -z $HOME ]]; then
  export HOME="${repo_root}artifacts/.home/"
  mkdir -p "$HOME"
fi

mkdir -p "$toolset_dir"
mkdir -p "$temp_dir"
mkdir -p "$log_dir"

Write-PipelineSetVariable -name "Artifacts" -value "$artifacts_dir"
Write-PipelineSetVariable -name "Artifacts.Toolset" -value "$toolset_dir"
Write-PipelineSetVariable -name "Artifacts.Log" -value "$log_dir"
Write-PipelineSetVariable -name "Temp" -value "$temp_dir"
Write-PipelineSetVariable -name "TMP" -value "$temp_dir"

# Import custom tools configuration, if present in the repo.
if [ -z "${disable_configure_toolset_import:-}" ]; then
  configure_toolset_script="$eng_root/configure-toolset.sh"
  if [[ -a "$configure_toolset_script" ]]; then
    . "$configure_toolset_script"
  fi
fi

# TODO: https://github.com/dotnet/arcade/issues/1468
# Temporary workaround to avoid breaking change.
# Remove once repos are updated.
if [[ -n "${useInstalledDotNetCli:-}" ]]; then
  use_installed_dotnet_cli="$useInstalledDotNetCli"
fi



================================================
FILE: eng/common/BuildConfiguration/build-configuration.json
================================================
{
  "RetryCountLimit": 1,
  "RetryByAnyError": false
}



================================================
FILE: eng/common/core-templates/job/job.yml
================================================
parameters:
# Job schema parameters - https://docs.microsoft.com/en-us/azure/devops/pipelines/yaml-schema?view=vsts&tabs=schema#job
  cancelTimeoutInMinutes: ''
  condition: ''
  container: ''
  continueOnError: false
  dependsOn: ''
  displayName: ''
  pool: ''
  steps: []
  strategy: ''
  timeoutInMinutes: ''
  variables: []
  workspace: ''
  templateContext: {}

# Job base template specific parameters
  # See schema documentation - https://github.com/dotnet/arcade/blob/master/Documentation/AzureDevOps/TemplateSchema.md
  # publishing defaults
  artifacts: ''
  enableMicrobuild: false
  enablePublishBuildArtifacts: false
  enablePublishBuildAssets: false
  enablePublishTestResults: false
  enablePublishUsingPipelines: false
  enableBuildRetry: false
  mergeTestResults: false
  testRunTitle: ''
  testResultsFormat: ''
  name: ''
  componentGovernanceSteps: []
  preSteps: []
  artifactPublishSteps: []
  runAsPublic: false

# 1es specific parameters
  is1ESPipeline: ''

jobs:
- job: ${{ parameters.name }}

  ${{ if ne(parameters.cancelTimeoutInMinutes, '') }}:
    cancelTimeoutInMinutes: ${{ parameters.cancelTimeoutInMinutes }}

  ${{ if ne(parameters.condition, '') }}:
    condition: ${{ parameters.condition }}

  ${{ if ne(parameters.container, '') }}:
    container: ${{ parameters.container }}

  ${{ if ne(parameters.continueOnError, '') }}:
    continueOnError: ${{ parameters.continueOnError }}

  ${{ if ne(parameters.dependsOn, '') }}:
    dependsOn: ${{ parameters.dependsOn }}

  ${{ if ne(parameters.displayName, '') }}:
    displayName: ${{ parameters.displayName }}

  ${{ if ne(parameters.pool, '') }}:
    pool: ${{ parameters.pool }}

  ${{ if ne(parameters.strategy, '') }}:
    strategy: ${{ parameters.strategy }}

  ${{ if ne(parameters.timeoutInMinutes, '') }}:
    timeoutInMinutes: ${{ parameters.timeoutInMinutes }}

  ${{ if ne(parameters.templateContext, '') }}:
    templateContext: ${{ parameters.templateContext }}

  variables:
  - ${{ if ne(parameters.enableTelemetry, 'false') }}:
    - name: DOTNET_CLI_TELEMETRY_PROFILE
      value: '$(Build.Repository.Uri)'
  - ${{ if eq(parameters.enableRichCodeNavigation, 'true') }}:
    - name: EnableRichCodeNavigation
      value: 'true'
  # Retry signature validation up to three times, waiting 2 seconds between attempts.
  # See https://learn.microsoft.com/en-us/nuget/reference/errors-and-warnings/nu3028#retry-untrusted-root-failures
  - name: NUGET_EXPERIMENTAL_CHAIN_BUILD_RETRY_POLICY
    value: 3,2000
  - ${{ each variable in parameters.variables }}:
    # handle name-value variable syntax
    # example:
    # - name: [key]
    #   value: [value]
    - ${{ if ne(variable.name, '') }}:
      - name: ${{ variable.name }}
        value: ${{ variable.value }}

    # handle variable groups
    - ${{ if ne(variable.group, '') }}:
      - group: ${{ variable.group }}

    # handle template variable syntax
    # example:
    # - template: path/to/template.yml
    #   parameters:
    #     [key]: [value]
    - ${{ if ne(variable.template, '') }}:
      - template: ${{ variable.template }}
        ${{ if ne(variable.parameters, '') }}:
          parameters: ${{ variable.parameters }}

    # handle key-value variable syntax.
    # example:
    # - [key]: [value]
    - ${{ if and(eq(variable.name, ''), eq(variable.group, ''), eq(variable.template, '')) }}:
      - ${{ each pair in variable }}:
        - name: ${{ pair.key }}
          value: ${{ pair.value }}

  # DotNet-HelixApi-Access provides 'HelixApiAccessToken' for internal builds
  - ${{ if and(eq(parameters.enableTelemetry, 'true'), eq(parameters.runAsPublic, 'false'), ne(variables['System.TeamProject'], 'public'), notin(variables['Build.Reason'], 'PullRequest')) }}:
    - group: DotNet-HelixApi-Access

  ${{ if ne(parameters.workspace, '') }}:
    workspace: ${{ parameters.workspace }}

  steps:
  - ${{ if eq(parameters.is1ESPipeline, '') }}:
    - 'Illegal entry point, is1ESPipeline is not defined. Repository yaml should not directly reference templates in core-templates folder.': error

  - ${{ if ne(parameters.preSteps, '') }}:
    - ${{ each preStep in parameters.preSteps }}:
      - ${{ preStep }}

  - ${{ if and(eq(parameters.runAsPublic, 'false'), ne(variables['System.TeamProject'], 'public'), notin(variables['Build.Reason'], 'PullRequest')) }}:
    - ${{ if eq(parameters.enableMicrobuild, 'true') }}:
      - task: MicroBuildSigningPlugin@4
        displayName: Install MicroBuild plugin
        inputs:
          signType: $(_SignType)
          zipSources: false
          feedSource: https://dnceng.pkgs.visualstudio.com/_packaging/MicroBuildToolset/nuget/v3/index.json
        env:
          TeamName: $(_TeamName)
          MicroBuildOutputFolderOverride: '$(Agent.TempDirectory)'
        continueOnError: ${{ parameters.continueOnError }}
        condition: and(succeeded(), in(variables['_SignType'], 'real', 'test'), eq(variables['Agent.Os'], 'Windows_NT'))

  - ${{ if and(eq(parameters.runAsPublic, 'false'), eq(variables['System.TeamProject'], 'internal')) }}:
    - task: NuGetAuthenticate@1

  - ${{ if and(ne(parameters.artifacts.download, 'false'), ne(parameters.artifacts.download, '')) }}:
    - task: DownloadPipelineArtifact@2
      inputs:
        buildType: current
        artifactName: ${{ coalesce(parameters.artifacts.download.name, 'Artifacts_$(Agent.OS)_$(_BuildConfig)') }}
        targetPath: ${{ coalesce(parameters.artifacts.download.path, 'artifacts') }}
        itemPattern: ${{ coalesce(parameters.artifacts.download.pattern, '**') }}

  - ${{ each step in parameters.steps }}:
    - ${{ step }}

  - ${{ if eq(parameters.enableRichCodeNavigation, true) }}:
    - task: RichCodeNavIndexer@0
      displayName: RichCodeNav Upload
      inputs:
        languages: ${{ coalesce(parameters.richCodeNavigationLanguage, 'csharp') }}
        environment: ${{ coalesce(parameters.richCodeNavigationEnvironment, 'internal') }}
        richNavLogOutputDirectory: $(Build.SourcesDirectory)/artifacts/bin
        uploadRichNavArtifacts: ${{ coalesce(parameters.richCodeNavigationUploadArtifacts, false) }}
      continueOnError: true

  - ${{ each step in parameters.componentGovernanceSteps }}:
    - ${{ step }}

  - ${{ if eq(parameters.enableMicrobuild, 'true') }}:
    - ${{ if and(eq(parameters.runAsPublic, 'false'), ne(variables['System.TeamProject'], 'public'), notin(variables['Build.Reason'], 'PullRequest')) }}:
      - task: MicroBuildCleanup@1
        displayName: Execute Microbuild cleanup tasks
        condition: and(always(), in(variables['_SignType'], 'real', 'test'), eq(variables['Agent.Os'], 'Windows_NT'))
        continueOnError: ${{ parameters.continueOnError }}
        env:
          TeamName: $(_TeamName)

  # Publish test results
  - ${{ if or(and(eq(parameters.enablePublishTestResults, 'true'), eq(parameters.testResultsFormat, '')), eq(parameters.testResultsFormat, 'xunit')) }}:
    - task: PublishTestResults@2
      displayName: Publish XUnit Test Results
      inputs:
        testResultsFormat: 'xUnit'
        testResultsFiles: '*.xml'
        searchFolder: '$(Build.SourcesDirectory)/artifacts/TestResults/$(_BuildConfig)'
        testRunTitle: ${{ coalesce(parameters.testRunTitle, parameters.name, '$(System.JobName)') }}-xunit
        mergeTestResults: ${{ parameters.mergeTestResults }}
      continueOnError: true
      condition: always()
  - ${{ if or(and(eq(parameters.enablePublishTestResults, 'true'), eq(parameters.testResultsFormat, '')), eq(parameters.testResultsFormat, 'vstest')) }}:
    - task: PublishTestResults@2
      displayName: Publish TRX Test Results
      inputs:
        testResultsFormat: 'VSTest'
        testResultsFiles: '*.trx'
        searchFolder: '$(Build.SourcesDirectory)/artifacts/TestResults/$(_BuildConfig)'
        testRunTitle: ${{ coalesce(parameters.testRunTitle, parameters.name, '$(System.JobName)') }}-trx
        mergeTestResults: ${{ parameters.mergeTestResults }}
      continueOnError: true
      condition: always()

  # gather artifacts
  - ${{ if ne(parameters.artifacts.publish, '') }}:
    - ${{ if and(ne(parameters.artifacts.publish.artifacts, 'false'), ne(parameters.artifacts.publish.artifacts, '')) }}:
      - task: CopyFiles@2
        displayName: Gather binaries for publish to artifacts
        inputs:
          SourceFolder: 'artifacts/bin'
          Contents: '**'
          TargetFolder: '$(Build.ArtifactStagingDirectory)/artifacts/bin'
      - task: CopyFiles@2
        displayName: Gather packages for publish to artifacts
        inputs:
          SourceFolder: 'artifacts/packages'
          Contents: '**'
          TargetFolder: '$(Build.ArtifactStagingDirectory)/artifacts/packages'
    - ${{ if and(ne(parameters.artifacts.publish.logs, 'false'), ne(parameters.artifacts.publish.logs, '')) }}:
      - task: CopyFiles@2
        displayName: Gather logs for publish to artifacts
        inputs:
          SourceFolder: 'artifacts/log'
          Contents: '**'
          TargetFolder: '$(Build.ArtifactStagingDirectory)/artifacts/log'
        continueOnError: true
        condition: always()

  - ${{ if eq(parameters.enablePublishBuildArtifacts, 'true') }}:
    - task: CopyFiles@2
      displayName: Gather logs for publish to artifacts
      inputs:
        SourceFolder: 'artifacts/log/$(_BuildConfig)'
        Contents: '**'
        TargetFolder: '$(Build.ArtifactStagingDirectory)/artifacts/log/$(_BuildConfig)'
      continueOnError: true
      condition: always()
  - ${{ if eq(parameters.enableBuildRetry, 'true') }}:
    - task: CopyFiles@2
      displayName: Gather buildconfiguration for build retry
      inputs:
        SourceFolder: '$(Build.SourcesDirectory)/eng/common/BuildConfiguration'
        Contents: '**'
        TargetFolder: '$(Build.ArtifactStagingDirectory)/eng/common/BuildConfiguration'
      continueOnError: true
      condition: always()
  - ${{ each step in parameters.artifactPublishSteps }}:
    - ${{ step }}



================================================
FILE: eng/common/core-templates/job/onelocbuild.yml
================================================
parameters:
  # Optional: dependencies of the job
  dependsOn: ''

  # Optional: A defined YAML pool - https://docs.microsoft.com/en-us/azure/devops/pipelines/yaml-schema?view=vsts&tabs=schema#pool
  pool: ''

  CeapexPat: $(dn-bot-ceapex-package-r) # PAT for the loc AzDO instance https://dev.azure.com/ceapex
  GithubPat: $(BotAccount-dotnet-bot-repo-PAT)

  SourcesDirectory: $(Build.SourcesDirectory)
  CreatePr: true
  AutoCompletePr: false
  ReusePr: true
  UseLfLineEndings: true
  UseCheckedInLocProjectJson: false
  SkipLocProjectJsonGeneration: false
  LanguageSet: VS_Main_Languages
  LclSource: lclFilesInRepo
  LclPackageId: ''
  RepoType: gitHub
  GitHubOrg: dotnet
  MirrorRepo: ''
  MirrorBranch: main
  condition: ''
  JobNameSuffix: ''
  is1ESPipeline: ''
jobs:
- job: OneLocBuild${{ parameters.JobNameSuffix }}

  dependsOn: ${{ parameters.dependsOn }}

  displayName: OneLocBuild${{ parameters.JobNameSuffix }}

  variables:
    - group: OneLocBuildVariables # Contains the CeapexPat and GithubPat
    - name: _GenerateLocProjectArguments
      value: -SourcesDirectory ${{ parameters.SourcesDirectory }}
        -LanguageSet "${{ parameters.LanguageSet }}"
        -CreateNeutralXlfs
    - ${{ if eq(parameters.UseCheckedInLocProjectJson, 'true') }}:
      - name: _GenerateLocProjectArguments
        value: ${{ variables._GenerateLocProjectArguments }} -UseCheckedInLocProjectJson
    - template: /eng/common/core-templates/variables/pool-providers.yml
      parameters:
        is1ESPipeline: ${{ parameters.is1ESPipeline }}

  ${{ if ne(parameters.pool, '') }}:
    pool: ${{ parameters.pool }}
  ${{ if eq(parameters.pool, '') }}:
    pool:
      # We don't use the collection uri here because it might vary (.visualstudio.com vs. dev.azure.com)
      ${{ if eq(variables['System.TeamProject'], 'DevDiv') }}:
        name: AzurePipelines-EO
        image: 1ESPT-Windows2022
        demands: Cmd
        os: windows
      # If it's not devdiv, it's dnceng
      ${{ if ne(variables['System.TeamProject'], 'DevDiv') }}:
        name: $(DncEngInternalBuildPool)
        image: 1es-windows-2022
        os: windows

  steps:
    - ${{ if eq(parameters.is1ESPipeline, '') }}:
      - 'Illegal entry point, is1ESPipeline is not defined. Repository yaml should not directly reference templates in core-templates folder.': error

    - ${{ if ne(parameters.SkipLocProjectJsonGeneration, 'true') }}:
      - task: Powershell@2
        inputs:
          filePath: $(Build.SourcesDirectory)/eng/common/generate-locproject.ps1
          arguments: $(_GenerateLocProjectArguments)
        displayName: Generate LocProject.json
        condition: ${{ parameters.condition }}

    - task: OneLocBuild@2
      displayName: OneLocBuild
      env:
        SYSTEM_ACCESSTOKEN: $(System.AccessToken)
      inputs:
        locProj: eng/Localize/LocProject.json
        outDir: $(Build.ArtifactStagingDirectory)
        lclSource: ${{ parameters.LclSource }}
        lclPackageId: ${{ parameters.LclPackageId }}
        isCreatePrSelected: ${{ parameters.CreatePr }}
        isAutoCompletePrSelected: ${{ parameters.AutoCompletePr }}
        ${{ if eq(parameters.CreatePr, true) }}:
          isUseLfLineEndingsSelected: ${{ parameters.UseLfLineEndings }}
          ${{ if eq(parameters.RepoType, 'gitHub') }}:
            isShouldReusePrSelected: ${{ parameters.ReusePr }}
        packageSourceAuth: patAuth
        patVariable: ${{ parameters.CeapexPat }}
        ${{ if eq(parameters.RepoType, 'gitHub') }}:
          repoType: ${{ parameters.RepoType }}
          gitHubPatVariable: "${{ parameters.GithubPat }}"
        ${{ if ne(parameters.MirrorRepo, '') }}:
          isMirrorRepoSelected: true
          gitHubOrganization: ${{ parameters.GitHubOrg }}
          mirrorRepo: ${{ parameters.MirrorRepo }}
          mirrorBranch: ${{ parameters.MirrorBranch }}
      condition: ${{ parameters.condition }}

    - template: /eng/common/core-templates/steps/publish-build-artifacts.yml
      parameters:
        is1ESPipeline: ${{ parameters.is1ESPipeline }}
        args:
          displayName: Publish Localization Files
          pathToPublish: '$(Build.ArtifactStagingDirectory)/loc'
          publishLocation: Container
          artifactName: Loc
          condition: ${{ parameters.condition }}

    - template: /eng/common/core-templates/steps/publish-build-artifacts.yml
      parameters:
        is1ESPipeline: ${{ parameters.is1ESPipeline }}
        args:
          displayName: Publish LocProject.json
          pathToPublish: '$(Build.SourcesDirectory)/eng/Localize/'
          publishLocation: Container
          artifactName: Loc
          condition: ${{ parameters.condition }}


================================================
FILE: eng/common/core-templates/job/publish-build-assets.yml
================================================
parameters:
  configuration: 'Debug'

  # Optional: condition for the job to run
  condition: ''

  # Optional: 'true' if future jobs should run even if this job fails
  continueOnError: false

  # Optional: dependencies of the job
  dependsOn: ''

  # Optional: Include PublishBuildArtifacts task
  enablePublishBuildArtifacts: false

  # Optional: A defined YAML pool - https://docs.microsoft.com/en-us/azure/devops/pipelines/yaml-schema?view=vsts&tabs=schema#pool
  pool: {}

  # Optional: should run as a public build even in the internal project
  #           if 'true', the build won't run any of the internal only steps, even if it is running in non-public projects.
  runAsPublic: false

  # Optional: whether the build's artifacts will be published using release pipelines or direct feed publishing
  publishUsingPipelines: false

  # Optional: whether the build's artifacts will be published using release pipelines or direct feed publishing
  publishAssetsImmediately: false

  artifactsPublishingAdditionalParameters: ''

  signingValidationAdditionalParameters: ''

  is1ESPipeline: ''

jobs:
- job: Asset_Registry_Publish

  dependsOn: ${{ parameters.dependsOn }}
  timeoutInMinutes: 150

  ${{ if eq(parameters.publishAssetsImmediately, 'true') }}:
    displayName: Publish Assets
  ${{ else }}:
    displayName: Publish to Build Asset Registry

  variables:
  - template: /eng/common/core-templates/variables/pool-providers.yml
    parameters:
      is1ESPipeline: ${{ parameters.is1ESPipeline }}
  - ${{ if and(eq(parameters.runAsPublic, 'false'), ne(variables['System.TeamProject'], 'public'), notin(variables['Build.Reason'], 'PullRequest')) }}:
    - group: Publish-Build-Assets
    - group: AzureDevOps-Artifact-Feeds-Pats
    - name: runCodesignValidationInjection
      value: false
    # unconditional - needed for logs publishing (redactor tool version)
    - template: /eng/common/core-templates/post-build/common-variables.yml

  pool:
    # We don't use the collection uri here because it might vary (.visualstudio.com vs. dev.azure.com)
    ${{ if eq(variables['System.TeamProject'], 'DevDiv') }}:
      name: AzurePipelines-EO
      image: 1ESPT-Windows2022
      demands: Cmd
      os: windows
    # If it's not devdiv, it's dnceng
    ${{ if ne(variables['System.TeamProject'], 'DevDiv') }}:
      name: NetCore1ESPool-Publishing-Internal
      image: windows.vs2019.amd64
      os: windows
  steps:
  - ${{ if eq(parameters.is1ESPipeline, '') }}:
    - 'Illegal entry point, is1ESPipeline is not defined. Repository yaml should not directly reference templates in core-templates folder.': error

  - ${{ if and(eq(parameters.runAsPublic, 'false'), ne(variables['System.TeamProject'], 'public'), notin(variables['Build.Reason'], 'PullRequest')) }}:
    - checkout: self
      fetchDepth: 3
      clean: true

    - task: DownloadBuildArtifacts@0
      displayName: Download artifact
      inputs:
        artifactName: AssetManifests
        downloadPath: '$(Build.StagingDirectory)/Download'
        checkDownloadedFiles: true
      condition: ${{ parameters.condition }}
      continueOnError: ${{ parameters.continueOnError }}

    - task: NuGetAuthenticate@1

    - task: AzureCLI@2
      displayName: Publish Build Assets
      inputs:
        azureSubscription: "Darc: Maestro Production"
        scriptType: ps
        scriptLocation: scriptPath
        scriptPath: $(Build.SourcesDirectory)/eng/common/sdk-task.ps1
        arguments: -task PublishBuildAssets -restore -msbuildEngine dotnet
          /p:ManifestsPath='$(Build.StagingDirectory)/Download/AssetManifests'
          /p:MaestroApiEndpoint=https://maestro.dot.net
          /p:PublishUsingPipelines=${{ parameters.publishUsingPipelines }}
          /p:OfficialBuildId=$(Build.BuildNumber)
      condition: ${{ parameters.condition }}
      continueOnError: ${{ parameters.continueOnError }}

    - task: powershell@2
      displayName: Create ReleaseConfigs Artifact
      inputs:
        targetType: inline
        script: |
          New-Item -Path "$(Build.StagingDirectory)/ReleaseConfigs" -ItemType Directory -Force
          $filePath = "$(Build.StagingDirectory)/ReleaseConfigs/ReleaseConfigs.txt"
          Add-Content -Path $filePath -Value $(BARBuildId)
          Add-Content -Path $filePath -Value "$(DefaultChannels)"
          Add-Content -Path $filePath -Value $(IsStableBuild)

          $symbolExclusionfile = "$(Build.SourcesDirectory)/eng/SymbolPublishingExclusionsFile.txt"
          if (Test-Path -Path $symbolExclusionfile)
          {
            Write-Host "SymbolExclusionFile exists"
            Copy-Item -Path $symbolExclusionfile -Destination "$(Build.StagingDirectory)/ReleaseConfigs"
          }

    - template: /eng/common/core-templates/steps/publish-build-artifacts.yml
      parameters:
        is1ESPipeline: ${{ parameters.is1ESPipeline }}
        args:
          displayName: Publish ReleaseConfigs Artifact
          pathToPublish: '$(Build.StagingDirectory)/ReleaseConfigs'
          publishLocation: Container
          artifactName: ReleaseConfigs

    - ${{ if eq(parameters.publishAssetsImmediately, 'true') }}:
      - template: /eng/common/core-templates/post-build/setup-maestro-vars.yml
        parameters:
          BARBuildId: ${{ parameters.BARBuildId }}
          PromoteToChannelIds: ${{ parameters.PromoteToChannelIds }}
          is1ESPipeline: ${{ parameters.is1ESPipeline }}

      - task: AzureCLI@2
        displayName: Publish Using Darc
        inputs:
          azureSubscription: "Darc: Maestro Production"
          scriptType: ps
          scriptLocation: scriptPath
          scriptPath: $(Build.SourcesDirectory)/eng/common/post-build/publish-using-darc.ps1
          arguments: >
            -BuildId $(BARBuildId)
            -PublishingInfraVersion 3
            -AzdoToken '$(System.AccessToken)'
            -WaitPublishingFinish true
            -ArtifactsPublishingAdditionalParameters '${{ parameters.artifactsPublishingAdditionalParameters }}'
            -SymbolPublishingAdditionalParameters '${{ parameters.symbolPublishingAdditionalParameters }}'

    - ${{ if eq(parameters.enablePublishBuildArtifacts, 'true') }}:
      - template: /eng/common/core-templates/steps/publish-logs.yml
        parameters:
          is1ESPipeline: ${{ parameters.is1ESPipeline }}
          JobLabel: 'Publish_Artifacts_Logs'



================================================
FILE: eng/common/core-templates/job/source-build.yml
================================================
parameters:
  # This template adds arcade-powered source-build to CI. The template produces a server job with a
  # default ID 'Source_Build_Complete' to put in a dependency list if necessary.

  # Specifies the prefix for source-build jobs added to pipeline. Use this if disambiguation needed.
  jobNamePrefix: 'Source_Build'

  # Defines the platform on which to run the job. By default, a linux-x64 machine, suitable for
  # managed-only repositories. This is an object with these properties:
  #
  # name: ''
  #   The name of the job. This is included in the job ID.
  # targetRID: ''
  #   The name of the target RID to use, instead of the one auto-detected by Arcade.
  # nonPortable: false
  #   Enables non-portable mode. This means a more specific RID (e.g. fedora.32-x64 rather than
  #   linux-x64), and compiling against distro-provided packages rather than portable ones.
  # skipPublishValidation: false
  #   Disables publishing validation.  By default, a check is performed to ensure no packages are
  #   published by source-build.
  # container: ''
  #   A container to use. Runs in docker.
  # pool: {}
  #   A pool to use. Runs directly on an agent.
  # buildScript: ''
  #   Specifies the build script to invoke to perform the build in the repo. The default
  #   './build.sh' should work for typical Arcade repositories, but this is customizable for
  #   difficult situations.
  # buildArguments: ''
  #   Specifies additional build arguments to pass to the build script.
  # jobProperties: {}
  #   A list of job properties to inject at the top level, for potential extensibility beyond
  #   container and pool.
  platform: {}

  is1ESPipeline: ''

  # If set to true and running on a non-public project,
  # Internal nuget and blob storage locations will be enabled.
  # This is not enabled by default because many repositories do not need internal sources
  # and do not need to have the required service connections approved in the pipeline.
  enableInternalSources: false

jobs:
- job: ${{ parameters.jobNamePrefix }}_${{ parameters.platform.name }}
  displayName: Source-Build (${{ parameters.platform.name }})

  ${{ each property in parameters.platform.jobProperties }}:
    ${{ property.key }}: ${{ property.value }}

  ${{ if ne(parameters.platform.container, '') }}:
    container: ${{ parameters.platform.container }}

  ${{ if eq(parameters.platform.pool, '') }}:
    # The default VM host AzDO pool. This should be capable of running Docker containers: almost all
    # source-build builds run in Docker, including the default managed platform.
    # /eng/common/core-templates/variables/pool-providers.yml can't be used here (some customers declare variables already), so duplicate its logic
    ${{ if eq(parameters.is1ESPipeline, 'true') }}:
      pool:
        ${{ if eq(variables['System.TeamProject'], 'public') }}:
          name: $[replace(replace(eq(contains(coalesce(variables['System.PullRequest.TargetBranch'], variables['Build.SourceBranch'], 'refs/heads/main'), 'release'), 'true'), True, 'NetCore-Svc-Public' ), False, 'NetCore-Public')]
          demands: ImageOverride -equals build.ubuntu.2004.amd64
        ${{ if eq(variables['System.TeamProject'], 'internal') }}:
          name: $[replace(replace(eq(contains(coalesce(variables['System.PullRequest.TargetBranch'], variables['Build.SourceBranch'], 'refs/heads/main'), 'release'), 'true'), True, 'NetCore1ESPool-Svc-Internal'), False, 'NetCore1ESPool-Internal')]
          image: 1es-mariner-2
          os: linux
    ${{ else }}:
      pool:
        ${{ if eq(variables['System.TeamProject'], 'public') }}:
          name: $[replace(replace(eq(contains(coalesce(variables['System.PullRequest.TargetBranch'], variables['Build.SourceBranch'], 'refs/heads/main'), 'release'), 'true'), True, 'NetCore-Svc-Public' ), False, 'NetCore-Public')]
          demands: ImageOverride -equals Build.Ubuntu.2204.Amd64.Open
        ${{ if eq(variables['System.TeamProject'], 'internal') }}:
          name: $[replace(replace(eq(contains(coalesce(variables['System.PullRequest.TargetBranch'], variables['Build.SourceBranch'], 'refs/heads/main'), 'release'), 'true'), True, 'NetCore1ESPool-Svc-Internal'), False, 'NetCore1ESPool-Internal')]
          demands: ImageOverride -equals Build.Ubuntu.2204.Amd64
  ${{ if ne(parameters.platform.pool, '') }}:
    pool: ${{ parameters.platform.pool }}

  workspace:
    clean: all

  steps:
  - ${{ if eq(parameters.is1ESPipeline, '') }}:
    - 'Illegal entry point, is1ESPipeline is not defined. Repository yaml should not directly reference templates in core-templates folder.': error

  - ${{ if eq(parameters.enableInternalSources, true) }}:
    - template: /eng/common/core-templates/steps/enable-internal-sources.yml
      parameters:
        is1ESPipeline: ${{ parameters.is1ESPipeline }}
    - template: /eng/common/core-templates/steps/enable-internal-runtimes.yml
      parameters:
        is1ESPipeline: ${{ parameters.is1ESPipeline }}
  - template: /eng/common/core-templates/steps/source-build.yml
    parameters:
      is1ESPipeline: ${{ parameters.is1ESPipeline }}
      platform: ${{ parameters.platform }}



================================================
FILE: eng/common/core-templates/job/source-index-stage1.yml
================================================
parameters:
  runAsPublic: false
  sourceIndexUploadPackageVersion: 2.0.0-20250425.2
  sourceIndexProcessBinlogPackageVersion: 1.0.1-20250425.2
  sourceIndexPackageSource: https://pkgs.dev.azure.com/dnceng/public/_packaging/dotnet-tools/nuget/v3/index.json
  sourceIndexBuildCommand: powershell -NoLogo -NoProfile -ExecutionPolicy Bypass -Command "eng/common/build.ps1 -restore -build -binarylog -ci"
  preSteps: []
  binlogPath: artifacts/log/Debug/Build.binlog
  condition: ''
  dependsOn: ''
  pool: ''
  is1ESPipeline: ''

jobs:
- job: SourceIndexStage1
  dependsOn: ${{ parameters.dependsOn }}
  condition: ${{ parameters.condition }}
  variables:
  - name: SourceIndexUploadPackageVersion
    value: ${{ parameters.sourceIndexUploadPackageVersion }}
  - name: SourceIndexProcessBinlogPackageVersion
    value: ${{ parameters.sourceIndexProcessBinlogPackageVersion }}
  - name: SourceIndexPackageSource
    value: ${{ parameters.sourceIndexPackageSource }}
  - name: BinlogPath
    value: ${{ parameters.binlogPath }}
  - template: /eng/common/core-templates/variables/pool-providers.yml
    parameters:
      is1ESPipeline: ${{ parameters.is1ESPipeline }}

  ${{ if ne(parameters.pool, '') }}:
    pool: ${{ parameters.pool }}
  ${{ if eq(parameters.pool, '') }}:
    pool:
      ${{ if eq(variables['System.TeamProject'], 'public') }}:
        name: $(DncEngPublicBuildPool)
        image: 1es-windows-2022-open
        os: windows
      ${{ if eq(variables['System.TeamProject'], 'internal') }}:
        name: $(DncEngInternalBuildPool)
        image: 1es-windows-2022
        os: windows

  steps:
  - ${{ if eq(parameters.is1ESPipeline, '') }}:
    - 'Illegal entry point, is1ESPipeline is not defined. Repository yaml should not directly reference templates in core-templates folder.': error

  - ${{ each preStep in parameters.preSteps }}:
    - ${{ preStep }}

  - task: UseDotNet@2
    displayName: Use .NET 8 SDK
    inputs:
      packageType: sdk
      version: 8.0.x
      installationPath: $(Agent.TempDirectory)/dotnet
      workingDirectory: $(Agent.TempDirectory)

  - script: |
      $(Agent.TempDirectory)/dotnet/dotnet tool install BinLogToSln --version $(sourceIndexProcessBinlogPackageVersion) --add-source $(SourceIndexPackageSource) --tool-path $(Agent.TempDirectory)/.source-index/tools
      $(Agent.TempDirectory)/dotnet/dotnet tool install UploadIndexStage1 --version $(sourceIndexUploadPackageVersion) --add-source $(SourceIndexPackageSource) --tool-path $(Agent.TempDirectory)/.source-index/tools
    displayName: Download Tools
    # Set working directory to temp directory so 'dotnet' doesn't try to use global.json and use the repo's sdk.
    workingDirectory: $(Agent.TempDirectory)

  - script: ${{ parameters.sourceIndexBuildCommand }}
    displayName: Build Repository

  - script: $(Agent.TempDirectory)/.source-index/tools/BinLogToSln -i $(BinlogPath) -r $(Build.SourcesDirectory) -n $(Build.Repository.Name) -o .source-index/stage1output
    displayName: Process Binlog into indexable sln

  - ${{ if and(eq(parameters.runAsPublic, 'false'), ne(variables['System.TeamProject'], 'public'), notin(variables['Build.Reason'], 'PullRequest')) }}:
    - task: AzureCLI@2
      displayName: Log in to Azure and upload stage1 artifacts to source index
      inputs:
        azureSubscription: 'SourceDotNet Stage1 Publish'
        addSpnToEnvironment: true
        scriptType: 'ps'
        scriptLocation: 'inlineScript'
        inlineScript: |
          $(Agent.TempDirectory)/.source-index/tools/UploadIndexStage1 -i .source-index/stage1output -n $(Build.Repository.Name) -s netsourceindexstage1 -b stage1



================================================
FILE: eng/common/core-templates/jobs/codeql-build.yml
================================================
parameters:
  # See schema documentation in /Documentation/AzureDevOps/TemplateSchema.md
  continueOnError: false
  # Required: A collection of jobs to run - https://docs.microsoft.com/en-us/azure/devops/pipelines/yaml-schema?view=vsts&tabs=schema#job
  jobs: []
  # Optional: if specified, restore and use this version of Guardian instead of the default.
  overrideGuardianVersion: ''
  is1ESPipeline: ''

jobs:
- template: /eng/common/core-templates/jobs/jobs.yml
  parameters:
    is1ESPipeline: ${{ parameters.is1ESPipeline }}
    enableMicrobuild: false
    enablePublishBuildArtifacts: false
    enablePublishTestResults: false
    enablePublishBuildAssets: false
    enablePublishUsingPipelines: false
    enableTelemetry: true

    variables:
      - group: Publish-Build-Assets
      # The Guardian version specified in 'eng/common/sdl/packages.config'. This value must be kept in
      # sync with the packages.config file.
      - name: DefaultGuardianVersion
        value: 0.109.0
      - name: GuardianPackagesConfigFile
        value: $(Build.SourcesDirectory)\eng\common\sdl\packages.config
      - name: GuardianVersion
        value: ${{ coalesce(parameters.overrideGuardianVersion, '$(DefaultGuardianVersion)') }}

    jobs: ${{ parameters.jobs }}




================================================
FILE: eng/common/core-templates/jobs/jobs.yml
================================================
parameters:
  # See schema documentation in /Documentation/AzureDevOps/TemplateSchema.md
  continueOnError: false

  # Optional: Include PublishBuildArtifacts task
  enablePublishBuildArtifacts: false

  # Optional: Enable publishing using release pipelines
  enablePublishUsingPipelines: false

  # Optional: Enable running the source-build jobs to build repo from source
  enableSourceBuild: false

  # Optional: Parameters for source-build template.
  #           See /eng/common/core-templates/jobs/source-build.yml for options
  sourceBuildParameters: []

  graphFileGeneration:
    # Optional: Enable generating the graph files at the end of the build
    enabled: false
    # Optional: Include toolset dependencies in the generated graph files
    includeToolset: false

  # Required: A collection of jobs to run - https://docs.microsoft.com/en-us/azure/devops/pipelines/yaml-schema?view=vsts&tabs=schema#job
  jobs: []

  # Optional: Override automatically derived dependsOn value for "publish build assets" job
  publishBuildAssetsDependsOn: ''

  # Optional: Publish the assets as soon as the publish to BAR stage is complete, rather doing so in a separate stage.
  publishAssetsImmediately: false

  # Optional: If using publishAssetsImmediately and additional parameters are needed, can be used to send along additional parameters (normally sent to post-build.yml)
  artifactsPublishingAdditionalParameters: ''
  signingValidationAdditionalParameters: ''

  # Optional: should run as a public build even in the internal project
  #           if 'true', the build won't run any of the internal only steps, even if it is running in non-public projects.
  runAsPublic: false

  enableSourceIndex: false
  sourceIndexParams: {}

  artifacts: {}
  is1ESPipeline: ''

# Internal resources (telemetry, microbuild) can only be accessed from non-public projects,
# and some (Microbuild) should only be applied to non-PR cases for internal builds.

jobs:
- ${{ each job in parameters.jobs }}:
  - ${{ if eq(parameters.is1ESPipeline, 'true') }}:
    - template: /eng/common/templates-official/job/job.yml
      parameters:
        # pass along parameters
        ${{ each parameter in parameters }}:
          ${{ if ne(parameter.key, 'jobs') }}:
            ${{ parameter.key }}: ${{ parameter.value }}

        # pass along job properties
        ${{ each property in job }}:
          ${{ if ne(property.key, 'job') }}:
            ${{ property.key }}: ${{ property.value }}

        name: ${{ job.job }}

  - ${{ else }}:
    - template: /eng/common/templates/job/job.yml
      parameters:
        # pass along parameters
        ${{ each parameter in parameters }}:
          ${{ if ne(parameter.key, 'jobs') }}:
            ${{ parameter.key }}: ${{ parameter.value }}

        # pass along job properties
        ${{ each property in job }}:
          ${{ if ne(property.key, 'job') }}:
            ${{ property.key }}: ${{ property.value }}

        name: ${{ job.job }}

- ${{ if eq(parameters.enableSourceBuild, true) }}:
  - template: /eng/common/core-templates/jobs/source-build.yml
    parameters:
      is1ESPipeline: ${{ parameters.is1ESPipeline }}
      allCompletedJobId: Source_Build_Complete
      ${{ each parameter in parameters.sourceBuildParameters }}:
        ${{ parameter.key }}: ${{ parameter.value }}

- ${{ if eq(parameters.enableSourceIndex, 'true') }}:
  - template: ../job/source-index-stage1.yml
    parameters:
      is1ESPipeline: ${{ parameters.is1ESPipeline }}
      runAsPublic: ${{ parameters.runAsPublic }}
      ${{ each parameter in parameters.sourceIndexParams }}:
        ${{ parameter.key }}: ${{ parameter.value }}

- ${{ if and(eq(parameters.runAsPublic, 'false'), ne(variables['System.TeamProject'], 'public'), notin(variables['Build.Reason'], 'PullRequest')) }}:
  - ${{ if or(eq(parameters.enablePublishBuildAssets, true), eq(parameters.artifacts.publish.manifests, 'true'), ne(parameters.artifacts.publish.manifests, '')) }}:
    - template: ../job/publish-build-assets.yml
      parameters:
        is1ESPipeline: ${{ parameters.is1ESPipeline }}
        continueOnError: ${{ parameters.continueOnError }}
        dependsOn:
        - ${{ if ne(parameters.publishBuildAssetsDependsOn, '') }}:
          - ${{ each job in parameters.publishBuildAssetsDependsOn }}:
            - ${{ job.job }}
        - ${{ if eq(parameters.publishBuildAssetsDependsOn, '') }}:
          - ${{ each job in parameters.jobs }}:
            - ${{ job.job }}
        - ${{ if eq(parameters.enableSourceBuild, true) }}:
          - Source_Build_Complete

        runAsPublic: ${{ parameters.runAsPublic }}
        publishUsingPipelines: ${{ parameters.enablePublishUsingPipelines }}
        publishAssetsImmediately: ${{ parameters.publishAssetsImmediately }}
        enablePublishBuildArtifacts: ${{ parameters.enablePublishBuildArtifacts }}
        artifactsPublishingAdditionalParameters: ${{ parameters.artifactsPublishingAdditionalParameters }}
        signingValidationAdditionalParameters: ${{ parameters.signingValidationAdditionalParameters }}



================================================
FILE: eng/common/core-templates/jobs/source-build.yml
================================================
parameters:
  # This template adds arcade-powered source-build to CI. A job is created for each platform, as
  # well as an optional server job that completes when all platform jobs complete.

  # The name of the "join" job for all source-build platforms. If set to empty string, the job is
  # not included. Existing repo pipelines can use this job depend on all source-build jobs
  # completing without maintaining a separate list of every single job ID: just depend on this one
  # server job. By default, not included. Recommended name if used: 'Source_Build_Complete'.
  allCompletedJobId: ''

  # See /eng/common/core-templates/job/source-build.yml
  jobNamePrefix: 'Source_Build'

  # This is the default platform provided by Arcade, intended for use by a managed-only repo.
  defaultManagedPlatform:
    name: 'Managed'
    container: 'mcr.microsoft.com/dotnet-buildtools/prereqs:centos-stream9'

  # Defines the platforms on which to run build jobs. One job is created for each platform, and the
  # object in this array is sent to the job template as 'platform'. If no platforms are specified,
  # one job runs on 'defaultManagedPlatform'.
  platforms: []

  is1ESPipeline: ''

  # If set to true and running on a non-public project,
  # Internal nuget and blob storage locations will be enabled.
  # This is not enabled by default because many repositories do not need internal sources
  # and do not need to have the required service connections approved in the pipeline.
  enableInternalSources: false

jobs:

- ${{ if ne(parameters.allCompletedJobId, '') }}:
  - job: ${{ parameters.allCompletedJobId }}
    displayName: Source-Build Complete
    pool: server
    dependsOn:
    - ${{ each platform in parameters.platforms }}:
      - ${{ parameters.jobNamePrefix }}_${{ platform.name }}
    - ${{ if eq(length(parameters.platforms), 0) }}:
      - ${{ parameters.jobNamePrefix }}_${{ parameters.defaultManagedPlatform.name }}

- ${{ each platform in parameters.platforms }}:
  - template: /eng/common/core-templates/job/source-build.yml
    parameters:
      is1ESPipeline: ${{ parameters.is1ESPipeline }}
      jobNamePrefix: ${{ parameters.jobNamePrefix }}
      platform: ${{ platform }}
      enableInternalSources: ${{ parameters.enableInternalSources }}

- ${{ if eq(length(parameters.platforms), 0) }}:
  - template: /eng/common/core-templates/job/source-build.yml
    parameters:
      is1ESPipeline: ${{ parameters.is1ESPipeline }}
      jobNamePrefix: ${{ parameters.jobNamePrefix }}
      platform: ${{ parameters.defaultManagedPlatform }}
      enableInternalSources: ${{ parameters.enableInternalSources }}



================================================
FILE: eng/common/core-templates/post-build/common-variables.yml
================================================
variables:
  - group: Publish-Build-Assets

  # Whether the build is internal or not
  - name: IsInternalBuild
    value: ${{ and(ne(variables['System.TeamProject'], 'public'), contains(variables['Build.SourceBranch'], 'internal')) }}

  # Default Maestro++ API Endpoint and API Version
  - name: MaestroApiEndPoint
    value: "https://maestro.dot.net"
  - name: MaestroApiVersion
    value: "2020-02-20"

  - name: SourceLinkCLIVersion
    value: 3.0.0
  - name: SymbolToolVersion
    value: 1.0.1
  - name: BinlogToolVersion
    value: 1.0.11

  - name: runCodesignValidationInjection
    value: false



================================================
FILE: eng/common/core-templates/post-build/post-build.yml
================================================
parameters:
  # Which publishing infra should be used. THIS SHOULD MATCH THE VERSION ON THE BUILD MANIFEST.
  # Publishing V1 is no longer supported
  # Publishing V2 is no longer supported
  # Publishing V3 is the default
  - name: publishingInfraVersion
    displayName: Which version of publishing should be used to promote the build definition?
    type: number
    default: 3
    values:
    - 3

  - name: BARBuildId
    displayName: BAR Build Id
    type: number
    default: 0

  - name: PromoteToChannelIds
    displayName: Channel to promote BARBuildId to
    type: string
    default: ''

  - name: enableSourceLinkValidation
    displayName: Enable SourceLink validation
    type: boolean
    default: false

  - name: enableSigningValidation
    displayName: Enable signing validation
    type: boolean
    default: true

  - name: enableSymbolValidation
    displayName: Enable symbol validation
    type: boolean
    default: false

  - name: enableNugetValidation
    displayName: Enable NuGet validation
    type: boolean
    default: true

  - name: publishInstallersAndChecksums
    displayName: Publish installers and checksums
    type: boolean
    default: true

  - name: requireDefaultChannels
    displayName: Fail the build if there are no default channel(s) registrations for the current build
    type: boolean
    default: false

  - name: SDLValidationParameters
    type: object
    default:
      enable: false
      publishGdn: false
      continueOnError: false
      params: ''
      artifactNames: ''
      downloadArtifacts: true

  # These parameters let the user customize the call to sdk-task.ps1 for publishing
  # symbols & general artifacts as well as for signing validation
  - name: symbolPublishingAdditionalParameters
    displayName: Symbol publishing additional parameters
    type: string
    default: ''

  - name: artifactsPublishingAdditionalParameters
    displayName: Artifact publishing additional parameters
    type: string
    default: ''

  - name: signingValidationAdditionalParameters
    displayName: Signing validation additional parameters
    type: string
    default: ''

  # Which stages should finish execution before post-build stages start
  - name: validateDependsOn
    type: object
    default:
    - build

  - name: publishDependsOn
    type: object
    default:
    - Validate

  # Optional: Call asset publishing rather than running in a separate stage
  - name: publishAssetsImmediately
    type: boolean
    default: false

  - name: is1ESPipeline
    type: boolean
    default: false

stages:
- ${{ if or(eq( parameters.enableNugetValidation, 'true'), eq(parameters.enableSigningValidation, 'true'), eq(parameters.enableSourceLinkValidation, 'true'), eq(parameters.SDLValidationParameters.enable, 'true')) }}:
  - stage: Validate
    dependsOn: ${{ parameters.validateDependsOn }}
    displayName: Validate Build Assets
    variables:
      - template: /eng/common/core-templates/post-build/common-variables.yml
      - template: /eng/common/core-templates/variables/pool-providers.yml
        parameters:
          is1ESPipeline: ${{ parameters.is1ESPipeline }}
    jobs:
    - job:
      displayName: NuGet Validation
      condition: and(succeededOrFailed(), eq( ${{ parameters.enableNugetValidation }}, 'true'))
      pool:
        # We don't use the collection uri here because it might vary (.visualstudio.com vs. dev.azure.com)
        ${{ if eq(variables['System.TeamProject'], 'DevDiv') }}:
          name: AzurePipelines-EO
          image: 1ESPT-Windows2022
          demands: Cmd
          os: windows
        # If it's not devdiv, it's dnceng
        ${{ else }}:
          ${{ if eq(parameters.is1ESPipeline, true) }}:
            name: $(DncEngInternalBuildPool)
            image: windows.vs2022.amd64
            os: windows
          ${{ else }}:
            name: $(DncEngInternalBuildPool)
            demands: ImageOverride -equals windows.vs2022.amd64

      steps:
        - template: /eng/common/core-templates/post-build/setup-maestro-vars.yml
          parameters:
            BARBuildId: ${{ parameters.BARBuildId }}
            PromoteToChannelIds: ${{ parameters.PromoteToChannelIds }}
            is1ESPipeline: ${{ parameters.is1ESPipeline }}

        - task: DownloadBuildArtifacts@0
          displayName: Download Package Artifacts
          inputs:
            buildType: specific
            buildVersionToDownload: specific
            project: $(AzDOProjectName)
            pipeline: $(AzDOPipelineId)
            buildId: $(AzDOBuildId)
            artifactName: PackageArtifacts
            checkDownloadedFiles: true

        - task: PowerShell@2
          displayName: Validate
          inputs:
            filePath: $(Build.SourcesDirectory)/eng/common/post-build/nuget-validation.ps1
            arguments: -PackagesPath $(Build.ArtifactStagingDirectory)/PackageArtifacts/

    - job:
      displayName: Signing Validation
      condition: and( eq( ${{ parameters.enableSigningValidation }}, 'true'), ne( variables['PostBuildSign'], 'true'))
      pool:
        # We don't use the collection uri here because it might vary (.visualstudio.com vs. dev.azure.com)
        ${{ if eq(variables['System.TeamProject'], 'DevDiv') }}:
          name: AzurePipelines-EO
          image: 1ESPT-Windows2022
          demands: Cmd
          os: windows
        # If it's not devdiv, it's dnceng
        ${{ else }}:
          ${{ if eq(parameters.is1ESPipeline, true) }}:
            name: $(DncEngInternalBuildPool)
            image: 1es-windows-2022
            os: windows
          ${{ else }}:
            name: $(DncEngInternalBuildPool)
            demands: ImageOverride -equals windows.vs2022.amd64
      steps:
        - template: /eng/common/core-templates/post-build/setup-maestro-vars.yml
          parameters:
            BARBuildId: ${{ parameters.BARBuildId }}
            PromoteToChannelIds: ${{ parameters.PromoteToChannelIds }}
            is1ESPipeline: ${{ parameters.is1ESPipeline }}

        - task: DownloadBuildArtifacts@0
          displayName: Download Package Artifacts
          inputs:
            buildType: specific
            buildVersionToDownload: specific
            project: $(AzDOProjectName)
            pipeline: $(AzDOPipelineId)
            buildId: $(AzDOBuildId)
            artifactName: PackageArtifacts
            checkDownloadedFiles: true
            itemPattern: |
              **
              !**/Microsoft.SourceBuild.Intermediate.*.nupkg

        # This is necessary whenever we want to publish/restore to an AzDO private feed
        # Since sdk-task.ps1 tries to restore packages we need to do this authentication here
        # otherwise it'll complain about accessing a private feed.
        - task: NuGetAuthenticate@1
          displayName: 'Authenticate to AzDO Feeds'

        # Signing validation will optionally work with the buildmanifest file which is downloaded from
        # Azure DevOps above.
        - task: PowerShell@2
          displayName: Validate
          inputs:
            filePath: eng\common\sdk-task.ps1
            arguments: -task SigningValidation -restore -msbuildEngine vs
              /p:PackageBasePath='$(Build.ArtifactStagingDirectory)/PackageArtifacts'
              /p:SignCheckExclusionsFile='$(Build.SourcesDirectory)/eng/SignCheckExclusionsFile.txt'
              ${{ parameters.signingValidationAdditionalParameters }}

        - template: /eng/common/core-templates/steps/publish-logs.yml
          parameters:
            is1ESPipeline: ${{ parameters.is1ESPipeline }}
            StageLabel: 'Validation'
            JobLabel: 'Signing'
            BinlogToolVersion: $(BinlogToolVersion)

    - job:
      displayName: SourceLink Validation
      condition: eq( ${{ parameters.enableSourceLinkValidation }}, 'true')
      pool:
        # We don't use the collection uri here because it might vary (.visualstudio.com vs. dev.azure.com)
        ${{ if eq(variables['System.TeamProject'], 'DevDiv') }}:
          name: AzurePipelines-EO
          image: 1ESPT-Windows2022
          demands: Cmd
          os: windows
        # If it's not devdiv, it's dnceng
        ${{ else }}:
          ${{ if eq(parameters.is1ESPipeline, true) }}:
            name: $(DncEngInternalBuildPool)
            image: 1es-windows-2022
            os: windows
          ${{ else }}:
            name: $(DncEngInternalBuildPool)
            demands: ImageOverride -equals windows.vs2022.amd64
      steps:
        - template: /eng/common/core-templates/post-build/setup-maestro-vars.yml
          parameters:
            BARBuildId: ${{ parameters.BARBuildId }}
            PromoteToChannelIds: ${{ parameters.PromoteToChannelIds }}
            is1ESPipeline: ${{ parameters.is1ESPipeline }}

        - task: DownloadBuildArtifacts@0
          displayName: Download Blob Artifacts
          inputs:
            buildType: specific
            buildVersionToDownload: specific
            project: $(AzDOProjectName)
            pipeline: $(AzDOPipelineId)
            buildId: $(AzDOBuildId)
            artifactName: BlobArtifacts
            checkDownloadedFiles: true

        - task: PowerShell@2
          displayName: Validate
          inputs:
            filePath: $(Build.SourcesDirectory)/eng/common/post-build/sourcelink-validation.ps1
            arguments: -InputPath $(Build.ArtifactStagingDirectory)/BlobArtifacts/
              -ExtractPath $(Agent.BuildDirectory)/Extract/
              -GHRepoName $(Build.Repository.Name)
              -GHCommit $(Build.SourceVersion)
              -SourcelinkCliVersion $(SourceLinkCLIVersion)
          continueOnError: true

- ${{ if ne(parameters.publishAssetsImmediately, 'true') }}:
  - stage: publish_using_darc
    ${{ if or(eq(parameters.enableNugetValidation, 'true'), eq(parameters.enableSigningValidation, 'true'), eq(parameters.enableSourceLinkValidation, 'true'), eq(parameters.SDLValidationParameters.enable, 'true')) }}:
      dependsOn: ${{ parameters.publishDependsOn }}
    ${{ else }}:
      dependsOn: ${{ parameters.validateDependsOn }}
    displayName: Publish using Darc
    variables:
      - template: /eng/common/core-templates/post-build/common-variables.yml
      - template: /eng/common/core-templates/variables/pool-providers.yml
        parameters:
          is1ESPipeline: ${{ parameters.is1ESPipeline }}
    jobs:
    - job:
      displayName: Publish Using Darc
      timeoutInMinutes: 120
      pool:
        # We don't use the collection uri here because it might vary (.visualstudio.com vs. dev.azure.com)
        ${{ if eq(variables['System.TeamProject'], 'DevDiv') }}:
          name: AzurePipelines-EO
          image: 1ESPT-Windows2022
          demands: Cmd
          os: windows
        # If it's not devdiv, it's dnceng
        ${{ else }}:
          ${{ if eq(parameters.is1ESPipeline, true) }}:
            name: NetCore1ESPool-Publishing-Internal
            image: windows.vs2019.amd64
            os: windows
          ${{ else }}:
            name: NetCore1ESPool-Publishing-Internal
            demands: ImageOverride -equals windows.vs2019.amd64
      steps:
        - template: /eng/common/core-templates/post-build/setup-maestro-vars.yml
          parameters:
            BARBuildId: ${{ parameters.BARBuildId }}
            PromoteToChannelIds: ${{ parameters.PromoteToChannelIds }}
            is1ESPipeline: ${{ parameters.is1ESPipeline }}

        - task: NuGetAuthenticate@1

        - task: AzureCLI@2
          displayName: Publish Using Darc
          inputs:
            azureSubscription: "Darc: Maestro Production"
            scriptType: ps
            scriptLocation: scriptPath
            scriptPath: $(Build.SourcesDirectory)/eng/common/post-build/publish-using-darc.ps1
            arguments: >
              -BuildId $(BARBuildId)
              -PublishingInfraVersion ${{ parameters.publishingInfraVersion }}
              -AzdoToken '$(System.AccessToken)'
              -WaitPublishingFinish true
              -RequireDefaultChannels ${{ parameters.requireDefaultChannels }}
              -ArtifactsPublishingAdditionalParameters '${{ parameters.artifactsPublishingAdditionalParameters }}'
              -SymbolPublishingAdditionalParameters '${{ parameters.symbolPublishingAdditionalParameters }}'



================================================
FILE: eng/common/core-templates/post-build/setup-maestro-vars.yml
================================================
parameters:
  BARBuildId: ''
  PromoteToChannelIds: ''
  is1ESPipeline: ''

steps:
  - ${{ if eq(parameters.is1ESPipeline, '') }}:
    - 'Illegal entry point, is1ESPipeline is not defined. Repository yaml should not directly reference templates in core-templates folder.': error

  - ${{ if eq(coalesce(parameters.PromoteToChannelIds, 0), 0) }}:
    - task: DownloadBuildArtifacts@0
      displayName: Download Release Configs
      inputs:
        buildType: current
        artifactName: ReleaseConfigs
        checkDownloadedFiles: true

  - task: AzureCLI@2
    name: setReleaseVars
    displayName: Set Release Configs Vars
    inputs:
      azureSubscription: "Darc: Maestro Production"
      scriptType: pscore
      scriptLocation: inlineScript
      inlineScript: |
        try {
          if (!$Env:PromoteToMaestroChannels -or $Env:PromoteToMaestroChannels.Trim() -eq '') {
            $Content = Get-Content $(Build.StagingDirectory)/ReleaseConfigs/ReleaseConfigs.txt

            $BarId = $Content | Select -Index 0
            $Channels = $Content | Select -Index 1
            $IsStableBuild = $Content | Select -Index 2

            $AzureDevOpsProject = $Env:System_TeamProject
            $AzureDevOpsBuildDefinitionId = $Env:System_DefinitionId
            $AzureDevOpsBuildId = $Env:Build_BuildId
          }
          else {
            . $(Build.SourcesDirectory)\eng\common\tools.ps1
            $darc = Get-Darc
            $buildInfo = & $darc get-build `
              --id ${{ parameters.BARBuildId }} `
              --extended `
              --output-format json `
              --ci `
              | convertFrom-Json

            $BarId = ${{ parameters.BARBuildId }}
            $Channels = $Env:PromoteToMaestroChannels -split ","
            $Channels = $Channels -join "]["
            $Channels = "[$Channels]"

            $IsStableBuild = $buildInfo.stable
            $AzureDevOpsProject = $buildInfo.azureDevOpsProject
            $AzureDevOpsBuildDefinitionId = $buildInfo.azureDevOpsBuildDefinitionId
            $AzureDevOpsBuildId = $buildInfo.azureDevOpsBuildId
          }

          Write-Host "##vso[task.setvariable variable=BARBuildId]$BarId"
          Write-Host "##vso[task.setvariable variable=TargetChannels]$Channels"
          Write-Host "##vso[task.setvariable variable=IsStableBuild]$IsStableBuild"

          Write-Host "##vso[task.setvariable variable=AzDOProjectName]$AzureDevOpsProject"
          Write-Host "##vso[task.setvariable variable=AzDOPipelineId]$AzureDevOpsBuildDefinitionId"
          Write-Host "##vso[task.setvariable variable=AzDOBuildId]$AzureDevOpsBuildId"
        }
        catch {
          Write-Host $_
          Write-Host $_.Exception
          Write-Host $_.ScriptStackTrace
          exit 1
        }
    env:
      PromoteToMaestroChannels: ${{ parameters.PromoteToChannelIds }}



================================================
FILE: eng/common/core-templates/steps/component-governance.yml
================================================
parameters:
  disableComponentGovernance: false
  componentGovernanceIgnoreDirectories: ''
  is1ESPipeline: false
  displayName: 'Component Detection'

steps:
- ${{ if eq(parameters.disableComponentGovernance, 'true') }}:
  - script: echo "##vso[task.setvariable variable=skipComponentGovernanceDetection]true"
    displayName: Set skipComponentGovernanceDetection variable
- ${{ if ne(parameters.disableComponentGovernance, 'true') }}:
  - task: ComponentGovernanceComponentDetection@0
    continueOnError: true
    displayName: ${{ parameters.displayName }}
    inputs:
      ignoreDirectories: ${{ parameters.componentGovernanceIgnoreDirectories }}



================================================
FILE: eng/common/core-templates/steps/enable-internal-runtimes.yml
================================================
# Obtains internal runtime download credentials and populates the 'dotnetbuilds-internal-container-read-token-base64'
# variable with the base64-encoded SAS token, by default

parameters:
- name: federatedServiceConnection
  type: string
  default: 'dotnetbuilds-internal-read'
- name: outputVariableName
  type: string
  default: 'dotnetbuilds-internal-container-read-token-base64'
- name: expiryInHours
  type: number
  default: 1
- name: base64Encode
  type: boolean
  default: true
- name: is1ESPipeline
  type: boolean
  default: false

steps:
- ${{ if ne(variables['System.TeamProject'], 'public') }}:
  - template: /eng/common/core-templates/steps/get-delegation-sas.yml
    parameters:
      federatedServiceConnection: ${{ parameters.federatedServiceConnection }}
      outputVariableName: ${{ parameters.outputVariableName }}
      expiryInHours: ${{ parameters.expiryInHours }}
      base64Encode: ${{ parameters.base64Encode }}
      storageAccount: dotnetbuilds
      container: internal
      permissions: rl
      is1ESPipeline: ${{ parameters.is1ESPipeline }}


================================================
FILE: eng/common/core-templates/steps/enable-internal-sources.yml
================================================
parameters:
# This is the Azure federated service connection that we log into to get an access token.
- name: nugetFederatedServiceConnection
  type: string
  default: 'dnceng-artifacts-feeds-read'
- name: is1ESPipeline
  type: boolean
  default: false
# Legacy parameters to allow for PAT usage
- name: legacyCredential
  type: string
  default: ''

steps:
- ${{ if ne(variables['System.TeamProject'], 'public') }}:
  - ${{ if ne(parameters.legacyCredential, '') }}:
    - task: PowerShell@2
      displayName: Setup Internal Feeds
      inputs:
        filePath: $(Build.SourcesDirectory)/eng/common/SetupNugetSources.ps1
        arguments: -ConfigFile $(Build.SourcesDirectory)/NuGet.config -Password $Env:Token
      env:
        Token: ${{ parameters.legacyCredential }}
  # If running on dnceng (internal project), just use the default behavior for NuGetAuthenticate.
  # If running on DevDiv, NuGetAuthenticate is not really an option. It's scoped to a single feed, and we have many feeds that
  # may be added. Instead, we'll use the traditional approach (add cred to nuget.config), but use an account token.
  - ${{ else }}:
    - ${{ if eq(variables['System.TeamProject'], 'internal') }}:
      - task: PowerShell@2
        displayName: Setup Internal Feeds
        inputs:
          filePath: $(Build.SourcesDirectory)/eng/common/SetupNugetSources.ps1
          arguments: -ConfigFile $(Build.SourcesDirectory)/NuGet.config
    - ${{ else }}:
      - template: /eng/common/templates/steps/get-federated-access-token.yml
        parameters:
          federatedServiceConnection: ${{ parameters.nugetFederatedServiceConnection }}
          outputVariableName: 'dnceng-artifacts-feeds-read-access-token'
      - task: PowerShell@2
        displayName: Setup Internal Feeds
        inputs:
          filePath: $(Build.SourcesDirectory)/eng/common/SetupNugetSources.ps1
          arguments: -ConfigFile $(Build.SourcesDirectory)/NuGet.config -Password $(dnceng-artifacts-feeds-read-access-token)
  # This is required in certain scenarios to install the ADO credential provider.
  # It installed by default in some msbuild invocations (e.g. VS msbuild), but needs to be installed for others
  # (e.g. dotnet msbuild).
  - task: NuGetAuthenticate@1



================================================
FILE: eng/common/core-templates/steps/generate-sbom.yml
================================================
# BuildDropPath - The root folder of the drop directory for which the manifest file will be generated.
# PackageName - The name of the package this SBOM represents.
# PackageVersion - The version of the package this SBOM represents.
# ManifestDirPath - The path of the directory where the generated manifest files will be placed
# IgnoreDirectories - Directories to ignore for SBOM generation. This will be passed through to the CG component detector.

parameters:
  PackageVersion: 9.0.0
  BuildDropPath: '$(Build.SourcesDirectory)/artifacts'
  PackageName: '.NET'
  ManifestDirPath: $(Build.ArtifactStagingDirectory)/sbom
  IgnoreDirectories: ''
  sbomContinueOnError: true
  is1ESPipeline: false
  # disable publishArtifacts if some other step is publishing the artifacts (like job.yml).
  publishArtifacts: true

steps:
- task: PowerShell@2
  displayName: Prep for SBOM generation in (Non-linux)
  condition: or(eq(variables['Agent.Os'], 'Windows_NT'), eq(variables['Agent.Os'], 'Darwin'))
  inputs:
    filePath: ./eng/common/generate-sbom-prep.ps1
    arguments: ${{parameters.manifestDirPath}}

# Chmodding is a workaround for https://github.com/dotnet/arcade/issues/8461
- script: |
    chmod +x ./eng/common/generate-sbom-prep.sh
    ./eng/common/generate-sbom-prep.sh ${{parameters.manifestDirPath}}
  displayName: Prep for SBOM generation in (Linux)
  condition: eq(variables['Agent.Os'], 'Linux')
  continueOnError: ${{ parameters.sbomContinueOnError }}

- task: AzureArtifacts.manifest-generator-task.manifest-generator-task.ManifestGeneratorTask@0
  displayName: 'Generate SBOM manifest'
  continueOnError: ${{ parameters.sbomContinueOnError }}
  inputs:
      PackageName: ${{ parameters.packageName }}
      BuildDropPath: ${{ parameters.buildDropPath }}
      PackageVersion: ${{ parameters.packageVersion }}
      ManifestDirPath: ${{ parameters.manifestDirPath }}/$(ARTIFACT_NAME)
      ${{ if ne(parameters.IgnoreDirectories, '') }}:
        AdditionalComponentDetectorArgs: '--IgnoreDirectories ${{ parameters.IgnoreDirectories }}'

- ${{ if eq(parameters.publishArtifacts, 'true')}}:
  - template: /eng/common/core-templates/steps/publish-pipeline-artifacts.yml
    parameters:
      is1ESPipeline: ${{ parameters.is1ESPipeline }}
      args:
        displayName: Publish SBOM manifest
        continueOnError: ${{parameters.sbomContinueOnError}}
        targetPath: '${{ parameters.manifestDirPath }}'
        artifactName: $(ARTIFACT_NAME)




================================================
FILE: eng/common/core-templates/steps/get-delegation-sas.yml
================================================
parameters:
- name: federatedServiceConnection
  type: string
- name: outputVariableName
  type: string
- name: expiryInHours
  type: number
  default: 1
- name: base64Encode
  type: boolean
  default: false
- name: storageAccount
  type: string
- name: container
  type: string
- name: permissions
  type: string
  default: 'rl'
- name: is1ESPipeline
  type: boolean
  default: false

steps:
- task: AzureCLI@2
  displayName: 'Generate delegation SAS Token for ${{ parameters.storageAccount }}/${{ parameters.container }}'
  inputs:
    azureSubscription: ${{ parameters.federatedServiceConnection }}
    scriptType: 'pscore'
    scriptLocation: 'inlineScript'
    inlineScript: |
      # Calculate the expiration of the SAS token and convert to UTC
      $expiry = (Get-Date).AddHours(${{ parameters.expiryInHours }}).ToUniversalTime().ToString("yyyy-MM-ddTHH:mm:ssZ")

      # Temporarily work around a helix issue where SAS tokens with / in them will cause incorrect downloads
      # of correlation payloads. https://github.com/dotnet/dnceng/issues/3484
      $sas = ""
      do {
        $sas = az storage container generate-sas --account-name ${{ parameters.storageAccount }} --name ${{ parameters.container }} --permissions ${{ parameters.permissions }} --expiry $expiry --auth-mode login --as-user -o tsv
        if ($LASTEXITCODE -ne 0) {
          Write-Error "Failed to generate SAS token."
          exit 1
        }
      } while($sas.IndexOf('/') -ne -1)

      if ($LASTEXITCODE -ne 0) {
        Write-Error "Failed to generate SAS token."
        exit 1
      }

      if ('${{ parameters.base64Encode }}' -eq 'true') {
        $sas = [Convert]::ToBase64String([System.Text.Encoding]::UTF8.GetBytes($sas))
      }

      Write-Host "Setting '${{ parameters.outputVariableName }}' with the access token value"
      Write-Host "##vso[task.setvariable variable=${{ parameters.outputVariableName }};issecret=true]$sas"



================================================
FILE: eng/common/core-templates/steps/get-federated-access-token.yml
================================================
parameters:
- name: federatedServiceConnection
  type: string
- name: outputVariableName
  type: string
- name: is1ESPipeline
  type: boolean
- name: stepName
  type: string
  default: 'getFederatedAccessToken'
- name: condition
  type: string
  default: ''
# Resource to get a token for. Common values include:
# - '499b84ac-1321-427f-aa17-267ca6975798' for Azure DevOps
# - 'https://storage.azure.com/' for storage
# Defaults to Azure DevOps
- name: resource
  type: string
  default: '499b84ac-1321-427f-aa17-267ca6975798'
- name: isStepOutputVariable
  type: boolean
  default: false

steps:
- task: AzureCLI@2
  displayName: 'Getting federated access token for feeds'
  name: ${{ parameters.stepName }}
  ${{ if ne(parameters.condition, '') }}:
    condition: ${{ parameters.condition }}
  inputs:
    azureSubscription: ${{ parameters.federatedServiceConnection }}
    scriptType: 'pscore'
    scriptLocation: 'inlineScript'
    inlineScript: |
      $accessToken = az account get-access-token --query accessToken --resource ${{ parameters.resource }} --output tsv
      if ($LASTEXITCODE -ne 0) {
        Write-Error "Failed to get access token for resource '${{ parameters.resource }}'"
        exit 1
      }
      Write-Host "Setting '${{ parameters.outputVariableName }}' with the access token value"
      Write-Host "##vso[task.setvariable variable=${{ parameters.outputVariableName }};issecret=true;isOutput=${{ parameters.isStepOutputVariable }}]$accessToken"


================================================
FILE: eng/common/core-templates/steps/publish-build-artifacts.yml
================================================
parameters:
- name: is1ESPipeline
  type: boolean
  default: false
- name: args
  type: object
  default: {}
steps:
- ${{ if ne(parameters.is1ESPipeline, true) }}:
  - template: /eng/common/templates/steps/publish-build-artifacts.yml
    parameters:
      is1ESPipeline: ${{ parameters.is1ESPipeline }}
      ${{ each parameter in parameters.args }}:
        ${{ parameter.key }}: ${{ parameter.value }}
- ${{ else }}:
  - template: /eng/common/templates-official/steps/publish-build-artifacts.yml
    parameters:
      is1ESPipeline: ${{ parameters.is1ESPipeline }}
      ${{ each parameter in parameters.args }}:
        ${{ parameter.key }}: ${{ parameter.value }}


================================================
FILE: eng/common/core-templates/steps/publish-logs.yml
================================================
parameters:
  StageLabel: ''
  JobLabel: ''
  CustomSensitiveDataList: ''
  # A default - in case value from eng/common/core-templates/post-build/common-variables.yml is not passed
  BinlogToolVersion: '1.0.11'
  is1ESPipeline: false

steps:
- task: Powershell@2
  displayName: Prepare Binlogs to Upload
  inputs:
    targetType: inline
    script: |
      New-Item -ItemType Directory $(Build.SourcesDirectory)/PostBuildLogs/${{parameters.StageLabel}}/${{parameters.JobLabel}}/
      Move-Item -Path $(Build.SourcesDirectory)/artifacts/log/Debug/* $(Build.SourcesDirectory)/PostBuildLogs/${{parameters.StageLabel}}/${{parameters.JobLabel}}/
  continueOnError: true
  condition: always()

- task: PowerShell@2
  displayName: Redact Logs
  inputs:
    filePath: $(Build.SourcesDirectory)/eng/common/post-build/redact-logs.ps1
    # For now this needs to have explicit list of all sensitive data. Taken from eng/publishing/v3/publish.yml
    # Sensitive data can as well be added to $(Build.SourcesDirectory)/eng/BinlogSecretsRedactionFile.txt'
    #  If the file exists - sensitive data for redaction will be sourced from it
    #  (single entry per line, lines starting with '# ' are considered comments and skipped)
    arguments: -InputPath '$(Build.SourcesDirectory)/PostBuildLogs'
      -BinlogToolVersion ${{parameters.BinlogToolVersion}}
      -TokensFilePath '$(Build.SourcesDirectory)/eng/BinlogSecretsRedactionFile.txt'
      '$(publishing-dnceng-devdiv-code-r-build-re)'
      '$(MaestroAccessToken)'
      '$(dn-bot-all-orgs-artifact-feeds-rw)'
      '$(akams-client-id)'
      '$(microsoft-symbol-server-pat)'
      '$(symweb-symbol-server-pat)'
      '$(dn-bot-all-orgs-build-rw-code-rw)'
      ${{parameters.CustomSensitiveDataList}}
  continueOnError: true
  condition: always()

- task: CopyFiles@2
  displayName: Gather post build logs
  inputs:
    SourceFolder: '$(Build.SourcesDirectory)/PostBuildLogs'
    Contents: '**'
    TargetFolder: '$(Build.ArtifactStagingDirectory)/PostBuildLogs'

- template: /eng/common/core-templates/steps/publish-build-artifacts.yml
  parameters:
    is1ESPipeline: ${{ parameters.is1ESPipeline }}
    args:
      displayName: Publish Logs
      pathToPublish: '$(Build.ArtifactStagingDirectory)/PostBuildLogs'
      publishLocation: Container
      artifactName: PostBuildLogs
      continueOnError: true
      condition: always()



================================================
FILE: eng/common/core-templates/steps/publish-pipeline-artifacts.yml
================================================
parameters:
- name: is1ESPipeline
  type: boolean
  default: false

- name: args
  type: object
  default: {}

steps:
- ${{ if ne(parameters.is1ESPipeline, true) }}:
  - template: /eng/common/templates/steps/publish-pipeline-artifacts.yml
    parameters:
      ${{ each parameter in parameters }}:
        ${{ parameter.key }}: ${{ parameter.value }}
- ${{ else }}:
  - template: /eng/common/templates-official/steps/publish-pipeline-artifacts.yml
    parameters:
      ${{ each parameter in parameters }}:
        ${{ parameter.key }}: ${{ parameter.value }}



================================================
FILE: eng/common/core-templates/steps/retain-build.yml
================================================
parameters:
  # Optional azure devops PAT with build execute permissions for the build's organization,
  # only needed if the build that should be retained ran on a different organization than
  # the pipeline where this template is executing from
  Token: ''
  # Optional BuildId to retain, defaults to the current running build
  BuildId: ''
  # Azure devops Organization URI for the build in the https://dev.azure.com/<organization> format.
  # Defaults to the organization the current pipeline is running on
  AzdoOrgUri: '$(System.CollectionUri)'
  # Azure devops project for the build. Defaults to the project the current pipeline is running on
  AzdoProject: '$(System.TeamProject)'

steps:
  - task: powershell@2
    inputs:
      targetType: 'filePath'
      filePath: eng/common/retain-build.ps1
      pwsh: true
      arguments: >
        -AzdoOrgUri: ${{parameters.AzdoOrgUri}}
        -AzdoProject ${{parameters.AzdoProject}}
        -Token ${{coalesce(parameters.Token, '$env:SYSTEM_ACCESSTOKEN') }}
        -BuildId ${{coalesce(parameters.BuildId, '$env:BUILD_ID')}}
    displayName: Enable permanent build retention
    env:
      SYSTEM_ACCESSTOKEN: $(System.AccessToken)
      BUILD_ID: $(Build.BuildId)


================================================
FILE: eng/common/core-templates/steps/send-to-helix.yml
================================================
# Please remember to update the documentation if you make changes to these parameters!
parameters:
  HelixSource: 'pr/default'              # required -- sources must start with pr/, official/, prodcon/, or agent/
  HelixType: 'tests/default/'            # required -- Helix telemetry which identifies what type of data this is; should include "test" for clarity and must end in '/'
  HelixBuild: $(Build.BuildNumber)       # required -- the build number Helix will use to identify this -- automatically set to the AzDO build number
  HelixTargetQueues: ''                  # required -- semicolon-delimited list of Helix queues to test on; see https://helix.dot.net/ for a list of queues
  HelixAccessToken: ''                   # required -- access token to make Helix API requests; should be provided by the appropriate variable group
  HelixProjectPath: 'eng/common/helixpublish.proj'  # optional -- path to the project file to build relative to BUILD_SOURCESDIRECTORY
  HelixProjectArguments: ''              # optional -- arguments passed to the build command
  HelixConfiguration: ''                 # optional -- additional property attached to a job
  HelixPreCommands: ''                   # optional -- commands to run before Helix work item execution
  HelixPostCommands: ''                  # optional -- commands to run after Helix work item execution
  WorkItemDirectory: ''                  # optional -- a payload directory to zip up and send to Helix; requires WorkItemCommand; incompatible with XUnitProjects
  WorkItemCommand: ''                    # optional -- a command to execute on the payload; requires WorkItemDirectory; incompatible with XUnitProjects
  WorkItemTimeout: ''                    # optional -- a timeout in TimeSpan.Parse-ready value (e.g. 00:02:00) for the work item command; requires WorkItemDirectory; incompatible with XUnitProjects
  CorrelationPayloadDirectory: ''        # optional -- a directory to zip up and send to Helix as a correlation payload
  XUnitProjects: ''                      # optional -- semicolon-delimited list of XUnitProjects to parse and send to Helix; requires XUnitRuntimeTargetFramework, XUnitPublishTargetFramework, XUnitRunnerVersion, and IncludeDotNetCli=true
  XUnitWorkItemTimeout: ''               # optional -- the workitem timeout in seconds for all workitems created from the xUnit projects specified by XUnitProjects
  XUnitPublishTargetFramework: ''        # optional -- framework to use to publish your xUnit projects
  XUnitRuntimeTargetFramework: ''        # optional -- framework to use for the xUnit console runner
  XUnitRunnerVersion: ''                 # optional -- version of the xUnit nuget package you wish to use on Helix; required for XUnitProjects
  IncludeDotNetCli: false                # optional -- true will download a version of the .NET CLI onto the Helix machine as a correlation payload; requires DotNetCliPackageType and DotNetCliVersion
  DotNetCliPackageType: ''               # optional -- either 'sdk', 'runtime' or 'aspnetcore-runtime'; determines whether the sdk or runtime will be sent to Helix; see https://raw.githubusercontent.com/dotnet/core/main/release-notes/releases-index.json
  DotNetCliVersion: ''                   # optional -- version of the CLI to send to Helix; based on this: https://raw.githubusercontent.com/dotnet/core/main/release-notes/releases-index.json
  WaitForWorkItemCompletion: true        # optional -- true will make the task wait until work items have been completed and fail the build if work items fail. False is "fire and forget."
  IsExternal: false                      # [DEPRECATED] -- doesn't do anything, jobs are external if HelixAccessToken is empty and Creator is set
  HelixBaseUri: 'https://helix.dot.net/' # optional -- sets the Helix API base URI (allows targeting https://helix.int-dot.net )
  Creator: ''                            # optional -- if the build is external, use this to specify who is sending the job
  DisplayNamePrefix: 'Run Tests'         # optional -- rename the beginning of the displayName of the steps in AzDO
  condition: succeeded()                 # optional -- condition for step to execute; defaults to succeeded()
  continueOnError: false                 # optional -- determines whether to continue the build if the step errors; defaults to false

steps:
  - powershell: 'powershell "$env:BUILD_SOURCESDIRECTORY\eng\common\msbuild.ps1 $env:BUILD_SOURCESDIRECTORY/${{ parameters.HelixProjectPath }} /restore /p:TreatWarningsAsErrors=false ${{ parameters.HelixProjectArguments }} /t:Test /bl:$env:BUILD_SOURCESDIRECTORY\artifacts\log\$env:BuildConfig\SendToHelix.binlog"'
    displayName: ${{ parameters.DisplayNamePrefix }} (Windows)
    env:
      BuildConfig: $(_BuildConfig)
      HelixSource: ${{ parameters.HelixSource }}
      HelixType: ${{ parameters.HelixType }}
      HelixBuild: ${{ parameters.HelixBuild }}
      HelixConfiguration:  ${{ parameters.HelixConfiguration }}
      HelixTargetQueues: ${{ parameters.HelixTargetQueues }}
      HelixAccessToken: ${{ parameters.HelixAccessToken }}
      HelixPreCommands: ${{ parameters.HelixPreCommands }}
      HelixPostCommands: ${{ parameters.HelixPostCommands }}
      WorkItemDirectory: ${{ parameters.WorkItemDirectory }}
      WorkItemCommand: ${{ parameters.WorkItemCommand }}
      WorkItemTimeout: ${{ parameters.WorkItemTimeout }}
      CorrelationPayloadDirectory: ${{ parameters.CorrelationPayloadDirectory }}
      XUnitProjects: ${{ parameters.XUnitProjects }}
      XUnitWorkItemTimeout: ${{ parameters.XUnitWorkItemTimeout }}
      XUnitPublishTargetFramework: ${{ parameters.XUnitPublishTargetFramework }}
      XUnitRuntimeTargetFramework: ${{ parameters.XUnitRuntimeTargetFramework }}
      XUnitRunnerVersion: ${{ parameters.XUnitRunnerVersion }}
      IncludeDotNetCli: ${{ parameters.IncludeDotNetCli }}
      DotNetCliPackageType: ${{ parameters.DotNetCliPackageType }}
      DotNetCliVersion: ${{ parameters.DotNetCliVersion }}
      WaitForWorkItemCompletion: ${{ parameters.WaitForWorkItemCompletion }}
      HelixBaseUri: ${{ parameters.HelixBaseUri }}
      Creator: ${{ parameters.Creator }}
      SYSTEM_ACCESSTOKEN: $(System.AccessToken)
    condition: and(${{ parameters.condition }}, eq(variables['Agent.Os'], 'Windows_NT'))
    continueOnError: ${{ parameters.continueOnError }}
  - script: $BUILD_SOURCESDIRECTORY/eng/common/msbuild.sh $BUILD_SOURCESDIRECTORY/${{ parameters.HelixProjectPath }} /restore /p:TreatWarningsAsErrors=false ${{ parameters.HelixProjectArguments }} /t:Test /bl:$BUILD_SOURCESDIRECTORY/artifacts/log/$BuildConfig/SendToHelix.binlog
    displayName: ${{ parameters.DisplayNamePrefix }} (Unix)
    env:
      BuildConfig: $(_BuildConfig)
      HelixSource: ${{ parameters.HelixSource }}
      HelixType: ${{ parameters.HelixType }}
      HelixBuild: ${{ parameters.HelixBuild }}
      HelixConfiguration:  ${{ parameters.HelixConfiguration }}
      HelixTargetQueues: ${{ parameters.HelixTargetQueues }}
      HelixAccessToken: ${{ parameters.HelixAccessToken }}
      HelixPreCommands: ${{ parameters.HelixPreCommands }}
      HelixPostCommands: ${{ parameters.HelixPostCommands }}
      WorkItemDirectory: ${{ parameters.WorkItemDirectory }}
      WorkItemCommand: ${{ parameters.WorkItemCommand }}
      WorkItemTimeout: ${{ parameters.WorkItemTimeout }}
      CorrelationPayloadDirectory: ${{ parameters.CorrelationPayloadDirectory }}
      XUnitProjects: ${{ parameters.XUnitProjects }}
      XUnitWorkItemTimeout: ${{ parameters.XUnitWorkItemTimeout }}
      XUnitPublishTargetFramework: ${{ parameters.XUnitPublishTargetFramework }}
      XUnitRuntimeTargetFramework: ${{ parameters.XUnitRuntimeTargetFramework }}
      XUnitRunnerVersion: ${{ parameters.XUnitRunnerVersion }}
      IncludeDotNetCli: ${{ parameters.IncludeDotNetCli }}
      DotNetCliPackageType: ${{ parameters.DotNetCliPackageType }}
      DotNetCliVersion: ${{ parameters.DotNetCliVersion }}
      WaitForWorkItemCompletion: ${{ parameters.WaitForWorkItemCompletion }}
      HelixBaseUri: ${{ parameters.HelixBaseUri }}
      Creator: ${{ parameters.Creator }}
      SYSTEM_ACCESSTOKEN: $(System.AccessToken)
    condition: and(${{ parameters.condition }}, ne(variables['Agent.Os'], 'Windows_NT'))
    continueOnError: ${{ parameters.continueOnError }}



================================================
FILE: eng/common/core-templates/steps/source-build.yml
================================================
parameters:
  # This template adds arcade-powered source-build to CI.

  # This is a 'steps' template, and is intended for advanced scenarios where the existing build
  # infra has a careful build methodology that must be followed. For example, a repo
  # (dotnet/runtime) might choose to clone the GitHub repo only once and store it as a pipeline
  # artifact for all subsequent jobs to use, to reduce dependence on a strong network connection to
  # GitHub. Using this steps template leaves room for that infra to be included.

  # Defines the platform on which to run the steps. See 'eng/common/core-templates/job/source-build.yml'
  # for details. The entire object is described in the 'job' template for simplicity, even though
  # the usage of the properties on this object is split between the 'job' and 'steps' templates.
  platform: {}
  is1ESPipeline: false

steps:
# Build. Keep it self-contained for simple reusability. (No source-build-specific job variables.)
- script: |
    set -x
    df -h

    # If file changes are detected, set CopyWipIntoInnerSourceBuildRepo to copy the WIP changes into the inner source build repo.
    internalRestoreArgs=
    if ! git diff --quiet; then
      internalRestoreArgs='/p:CopyWipIntoInnerSourceBuildRepo=true'
      # The 'Copy WIP' feature of source build uses git stash to apply changes from the original repo.
      # This only works if there is a username/email configured, which won't be the case in most CI runs.
      git config --get user.email
      if [ $? -ne 0 ]; then
        git config user.email dn-bot@microsoft.com
        git config user.name dn-bot
      fi
    fi

    # If building on the internal project, the internal storage variable may be available (usually only if needed)
    # In that case, add variables to allow the download of internal runtimes if the specified versions are not found
    # in the default public locations.
    internalRuntimeDownloadArgs=
    if [ '$(dotnetbuilds-internal-container-read-token-base64)' != '$''(dotnetbuilds-internal-container-read-token-base64)' ]; then
      internalRuntimeDownloadArgs='/p:DotNetRuntimeSourceFeed=https://dotnetbuilds.blob.core.windows.net/internal /p:DotNetRuntimeSourceFeedKey=$(dotnetbuilds-internal-container-read-token-base64) --runtimesourcefeed https://dotnetbuilds.blob.core.windows.net/internal --runtimesourcefeedkey $(dotnetbuilds-internal-container-read-token-base64)'
    fi

    buildConfig=Release
    # Check if AzDO substitutes in a build config from a variable, and use it if so.
    if [ '$(_BuildConfig)' != '$''(_BuildConfig)' ]; then
      buildConfig='$(_BuildConfig)'
    fi

    officialBuildArgs=
    if [ '${{ and(ne(variables['System.TeamProject'], 'public'), notin(variables['Build.Reason'], 'PullRequest')) }}' = 'True' ]; then
      officialBuildArgs='/p:DotNetPublishUsingPipelines=true /p:OfficialBuildId=$(BUILD.BUILDNUMBER)'
    fi

    targetRidArgs=
    if [ '${{ parameters.platform.targetRID }}' != '' ]; then
      targetRidArgs='/p:TargetRid=${{ parameters.platform.targetRID }}'
    fi

    runtimeOsArgs=
    if [ '${{ parameters.platform.runtimeOS }}' != '' ]; then
      runtimeOsArgs='/p:RuntimeOS=${{ parameters.platform.runtimeOS }}'
    fi

    baseOsArgs=
    if [ '${{ parameters.platform.baseOS }}' != '' ]; then
      baseOsArgs='/p:BaseOS=${{ parameters.platform.baseOS }}'
    fi

    publishArgs=
    if [ '${{ parameters.platform.skipPublishValidation }}' != 'true' ]; then
      publishArgs='--publish'
    fi

    assetManifestFileName=SourceBuild_RidSpecific.xml
    if [ '${{ parameters.platform.name }}' != '' ]; then
      assetManifestFileName=SourceBuild_${{ parameters.platform.name }}.xml
    fi

    ${{ coalesce(parameters.platform.buildScript, './build.sh') }} --ci \
      --configuration $buildConfig \
      --restore --build --pack $publishArgs -bl \
      ${{ parameters.platform.buildArguments }} \
      $officialBuildArgs \
      $internalRuntimeDownloadArgs \
      $internalRestoreArgs \
      $targetRidArgs \
      $runtimeOsArgs \
      $baseOsArgs \
      /p:SourceBuildNonPortable=${{ parameters.platform.nonPortable }} \
      /p:ArcadeBuildFromSource=true \
      /p:DotNetBuildSourceOnly=true \
      /p:DotNetBuildRepo=true \
      /p:AssetManifestFileName=$assetManifestFileName
  displayName: Build

# Upload build logs for diagnosis.
- task: CopyFiles@2
  displayName: Prepare BuildLogs staging directory
  inputs:
    SourceFolder: '$(Build.SourcesDirectory)'
    Contents: |
      **/*.log
      **/*.binlog
      artifacts/sb/prebuilt-report/**
    TargetFolder: '$(Build.StagingDirectory)/BuildLogs'
    CleanTargetFolder: true
  continueOnError: true
  condition: succeededOrFailed()

- template: /eng/common/core-templates/steps/publish-pipeline-artifacts.yml
  parameters:
    is1ESPipeline: ${{ parameters.is1ESPipeline }}
    args:
      displayName: Publish BuildLogs
      targetPath: '$(Build.StagingDirectory)/BuildLogs'
      artifactName: BuildLogs_SourceBuild_${{ parameters.platform.name }}_Attempt$(System.JobAttempt)
      continueOnError: true
      condition: succeededOrFailed()
      sbomEnabled: false  # we don't need SBOM for logs

# Manually inject component detection so that we can ignore the source build upstream cache, which contains
# a nupkg cache of input packages (a local feed).
# This path must match the upstream cache path in property 'CurrentRepoSourceBuiltNupkgCacheDir'
# in src\Microsoft.DotNet.Arcade.Sdk\tools\SourceBuild\SourceBuildArcade.targets
- template: /eng/common/core-templates/steps/component-governance.yml
  parameters:
    displayName: Component Detection (Exclude upstream cache)
    is1ESPipeline: ${{ parameters.is1ESPipeline }}
    componentGovernanceIgnoreDirectories: '$(Build.SourcesDirectory)/artifacts/sb/src/artifacts/obj/source-built-upstream-cache'
    disableComponentGovernance: ${{ eq(variables['System.TeamProject'], 'public') }}



================================================
FILE: eng/common/core-templates/variables/pool-providers.yml
================================================
parameters:
  is1ESPipeline: false

variables:
  - ${{ if eq(parameters.is1ESPipeline, 'true') }}:
    - template: /eng/common/templates-official/variables/pool-providers.yml
  - ${{ else }}:
    - template: /eng/common/templates/variables/pool-providers.yml


================================================
FILE: eng/common/cross/build-android-rootfs.sh
================================================
#!/usr/bin/env bash
set -e
__NDK_Version=r21

usage()
{
    echo "Creates a toolchain and sysroot used for cross-compiling for Android."
    echo
    echo "Usage: $0 [BuildArch] [ApiLevel]"
    echo
    echo "BuildArch is the target architecture of Android. Currently only arm64 is supported."
    echo "ApiLevel is the target Android API level. API levels usually m