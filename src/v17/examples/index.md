---
title: Minimal Package
type: examples
order: 0
---

> Simple package with minimal configuration.

Let's go step by step and create a simple DICE package with minimal configuration. The basic requirements are just an editor (Vim, Kate, Sublime, ...) and latest DICE which also comes with the dice package manager (dpm). The following steps are being performed on a Linux OS.

First of all we create a directory for DICE packages, for example in your home directory:

```bash
mkdir -p ~/dice-packages
```

Next we create a directory for our package with the name `examples-dev`:

```bash
mkdir -p ~/examples-dev
cd ~/example-dev
```

Inside what we need to tell DICE that this is a package. That's why we will create the file `package.yaml` with the following content:

```yaml
version: '1'

name: 'Examples'
description: |
  'Example package'
release: '17.09.0'
```

This package is currently empty. To be able to see this package in the packages treeView in DICE, we need to add our directory with packages to the `dice packages search path`. This can be done by going to `Settings > Packages search paths` and adding our packages directory path:

<p style="text-align: center">
  <img style="width:700px" src="/images/packages_dirs.png" alt="packages, dice">
</p>


 <p class="tip">You can also edit the entry `packages_dirs` in the `~/.DICE/config/dice.json` configuration file.</p>

 Now you can see the package in the treeView for packages on the DICE desk.


<p style="text-align: center">
  <img style="width:700px" src="/images/packages_treeView_1.png" alt="wvc, dice">
</p>

Resulting directory structure:

```
examples-dev
|- package.yaml
```
