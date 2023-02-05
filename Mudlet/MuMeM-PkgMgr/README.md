MuMeM Package Manager
============================

## Description

MuMeM Package Manager (MuMeM-PkgMgr) is a graphical package manager to easily install, upgrade and uninstall MuMeM packages.

You can easily use the package manager in Mudlet by typing `mpkgmgr`.

![MuMeM Package Manager](https://github.com/MuMeM/mume/blob/main/Mudlet/MuMeM-PkgMgr/doc/MuMeM-PkgMgr.png)

## Installation

### Via Mudlet Package Manager

Download the latest package of MuMeM Package Manager from github. The package is called `MuMeM-PkgMgr-latest.mpackage`. Open the Mudlet package manager and install the package. **Restart** Mudlet!

To install additional MuMeM packages via the MuMeM Package Manager, type `mpkgmgr`.

### Via command line

After starting Mudlet, type below line and thereafter **restart** Mudlet.

    lua installPackage"https://github.com/MuMeM/mume/raw/main/Mudlet/MuMeM-PkgMgr/MuMeM-PkgMgr-latest.mpackage"

You do not have to be logged into the mud for this, just starting Mudlet is sufficient.

To install additional MuMeM packages via the MuMeM Package Manager, type `mpkgmgr`.

## Usage

The graphical interface is pretty much self explanatory. Here are some conventions:

  * When you install a package that is already instaleld, it is first removed and then installed again (aka re-install or update)
  * When you install packages, all dependencies will be (re-)installed automatically
  * "Remove all" will not remove MuMeM Package Manager (MuMeM-PkgMgr)
  * "Install all" will not install/update MuMeM Package Manager (MuMeM-PkgMgr)

## FAQ

#### How do I update a package?

Select the package and click "install". The package will be removed and the latest version installed.

#### How do I update MuMeM Package Manager (MeMeM-PkgMgr)

Select MuMeM Package manager and click "install". MuMeM Package Manager will be updated (removed and installed again).

**NOTE**: When upgrading MuMeM Package Manager, **immediately** restart Mudlet before proceeding!