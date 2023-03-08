MuMeM GPrompt
============================

## Description

A graphical prompt for MUME, done the MUME way.

The prompt displays the vitals in a graphical way (bars) and also displays status information, like environment lightning, weather, riding, weight and the like.

## Vital bar explanation

MUME does not expose detailed vital information all the time. Expecially during combat you do not see your exact values, but instead of this "vital categories" are given. For example "healthy", "wounded", "bad" and so on for your health.

GPrompt displays your vitals in two "layers":

  * The top layer shows you in which "category" you are, e.g. healthy, wounded, and so on. So this is the guaranteed minimum health/mana/move you currently have
  * The middle layer shows:

    * the exact value of your vitals when you are outside of combat
    * the last known value when you are in combat

Now this all sounds very complicated, but it will be easily understandable once you are in the game and see the bars moving.

### GPrompt during combat

![GPrompt during combat](https://github.com/MuMeM/mume/blob/main/Mudlet/MuMeM-GPrompt/doc/GPrompt-Combat.png)

### GPrompt out of combat

![GPrompt out of combat](https://github.com/MuMeM/mume/blob/main/Mudlet/MuMeM-GPrompt/doc/GPrompt-OutOfCombat.png)

## Installation

**WARNING**: MuMeM-GPrompt is conflicting with "mumem_gui". You need to uninstall/disable it first. See below how.

### Via MuMeM Package Manager

Just install [MuMeM Package Manager](https://github.com/MuMeM/mume/tree/main/Mudlet/MuMeM-PkgMgr). You can then install this application with a simple graphical user interfase.

### Manual installation

GPrompt needs the following dependencies. All of these can be found on the MuMeM github page.

  * MuMeM-Core
  * MuMeM-Player
  * MuMeM-Log
  * MuMeM-GMCP

You can download these packages and MuMeM-GPrompt from github and install them via the package manager. You **must restart** Mudlet after installation!

An easier way is to install them via the command line. Follow these instuctions:

  1. Start the client and select your profile (you do not need to login to MUME)
  2. Copy and paste the lines from the codeblock below (one for one!)
  3. See the feedback on the screen (You get [download] and [OK])
  4. restart Mudlet

    lua installPackage"https://github.com/MuMeM/mume/raw/main/Mudlet/MuMeM-Core/MuMeM-Core-latest.mpackage"
    lua installPackage"https://github.com/MuMeM/mume/raw/main/Mudlet/MuMeM-Player/MuMeM-Player-latest.mpackage"
    lua installPackage"https://github.com/MuMeM/mume/raw/main/Mudlet/MuMeM-Log/MuMeM-Log-latest.mpackage"
    lua installPackage"https://github.com/MuMeM/mume/raw/main/Mudlet/MuMeM-GMCP/MuMeM-GMCP-latest.mpackage"
    lua installPackage"https://github.com/MuMeM/mume/raw/main/Mudlet/MuMeM-GPrompt/MuMeM-GPrompt-latest.mpackage"

## Uninstallation

Just use the Mudlet package manager and remove the packages. Then *restart* Mudlet!

## Uninstallation of mume_gui

The default MUME GUI (mume_gui) package is *automatically* installed by Mudlet. There is no way to remove it, as it will reinstall itself. So the only way is to disable it. You can do this by

  1. go to the script edit in Mudlet
  2. select the "mume_gui" folder
  3. select the "mume_gui.lua" file
  4. in the first line *insert*: `if 1 == 1 then return end`

*EXCEPTION*: When play MUME via MMapper, "mume_gui" is not installed by default!