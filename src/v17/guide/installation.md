---
title: Installation
type: guide
order: 2
---

### Get DICE

Latest Version: **v17.09.0** (includes dpm 17.09.0)

| Linux | v17.09.0 | latest-dev |
| --- | --- | --- | --- |
| **Linux Binaries (.tar.gz)** | [64-bit][1.1] | [64-bit][1.2]
| **Linux Binaries (.tar.xz)** | [64-bit][1.3] | [64-bit][1.4]
| **Linux Installer (.run)** | [64-bit][1.5] | [64-bit][1.6]

| Windows | v17.09.0 | latest-dev |
| --- | --- | --- | --- |
| **Windows Installer (.exe)** | [64-bit][2.1] | [64-bit][2.2]
| **Windows Binaries (.zip)** | [64-bit][2.3] | [64-bit][2.3]

[1.1]:http://backup1.foxcloud.net/mcubcsro/dice/releases/dice/17.09/17.09.0/dice-linux-x64-17.09.0.tar.gz
[1.2]:http://backup1.foxcloud.net/mcubcsro/public/dice/releases/dice/latest-dev/dice-linux-x64-latest-dev.tar.gz
[1.3]:http://backup1.foxcloud.net/mcubcsro/dice/releases/dice/17.09/17.09.0/dice-linux-x64-17.09.0.tar.xz
[1.4]:http://backup1.foxcloud.net/mcubcsro/public/dice/releases/dice/latest-dev/dice-linux-x64-latest-dev.tar.xz
[1.5]:http://backup1.foxcloud.net/mcubcsro/dice/releases/dice/17.09/17.09.0/dice-linux-x64-17.09.0.run
[1.6]:http://backup1.foxcloud.net/mcubcsro/public/dice/releases/dice/latest-dev/dice-linux-x64-latest-dev.run

[2.1]:http://backup1.foxcloud.net/mcubcsro/public/dice/releases/dice/latest-dev/DICE_Installer_latest-dev.exe
[2.2]:http://backup1.foxcloud.net/mcubcsro/public/dice/releases/dice/latest-dev/DICE_Installer_latest-dev.exe
[2.3]:http://backup1.foxcloud.net/mcubcsro/dice/releases/dice/latest-dev/dice-win-x64-latest-dev.zip
[2.4]:http://backup1.foxcloud.net/mcubcsro/dice/releases/dice/latest-dev/dice-win-x64-latest-dev.zip

There are always two different versions for DICE: `development` and `stable release`. The development version is the build of the latest commit and the archive contains the string `latest-dev`. The versioning for the stable release follows the [CalVer](http://calver.org/) convention:
<img src="https://img.shields.io/badge/calver-YY.0M.MICRO-22bfda.svg">

### Compatibility

DICE has been tested on the following OS:

| OS | DICE | DPM |
| --- | ---
| **(K)Ubuntu 16.04 (xenial)** | ✓ | ✓ |
| **(K)Ubuntu 16.10 (yakkety)** | ✓ | ✓ |
| **(K)Ubuntu 17.04 (zesty)** | ✓ | ✓ |
| **Windows 7** | ✓ | ✓ |
| **Windows 10** | ✓ | ✓ |

DICE can also be downloaded from the <https://dicehub.com> website in the getDice-section:

<a class="button" href="https://dicehub.com/getdice/current" target="_blank">Download DICE here</a><span class="light info">Linux/Windows</span>

### Quick start on Linux



#### Download DICE

```bash
wget https://download.dicehub.com/dice/release/17.04.0/Linux%2064-bit/tar.xz
```

#### Extract Archive

```bash
tar -xvf dice-linux-x64-latest-dev.tar.xz
```

#### Start DICE

```bash
cd dice-latest-dev
./DICE.sh
```

### Quick start on Windows

#### Download DICE

Before starting DICE you will need to install the `Visual C++ Redistributable for Visual Studio 2015` library:

<a class="button" href="https://www.microsoft.com/en-us/download/details.aspx?id=48145" target="_blank">MSVC R 2015</a><span class="light info">From Microsoft</span>

Download the archive, extract it and execute: `DICE.bat`
