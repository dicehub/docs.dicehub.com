---
title: Installation
type: guide
order: 2
---

### Get DICE

Download DICE from the <https://dicehub.com> website in the getDice-section:

<a class="button" href="https://dicehub.com/getdice/current" target="_blank">Download DICE here</a><span class="light info">Linux/Windows</span>

### Linux

There are always two different versions for DICE: `development` and `stable release`. The development version is the build of the latest commit and the archive contains the string `latest-dev`. The versioning for the stable release follows the [CalVer](http://calver.org/) convention:
<img src="https://img.shields.io/badge/calver-YY.0M.MICRO-22bfda.svg">

DICE has been tested on the following OS:

| OS | DICE | DPM |
| --- | ---
| **(K)Ubuntu 16.04 (xenial)** | ✓ | ✓ |
| **(K)Ubuntu 16.10 (yakkety)** | ✓ | ✓ |
| **(K)Ubuntu 17.04 (zesty)** | ✓ | ✓ |
| **Windows 7** | ✓ | ✓ |
| **Windows 10** | ✓ | ✓ |

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

### Windows

#### Download DICE

Before starting DICE you will need to install the `Visual C++ Redistributable for Visual Studio 2015` library:

<a class="button" href="https://www.microsoft.com/en-us/download/details.aspx?id=48145" target="_blank">MSVC R 2015</a><span class="light info">From Microsoft</span>

Download the archive, extract it and execute: `DICE.bat`
