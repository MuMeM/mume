MuMeM Prompt
============================

## Description

A graphical prompt for MUME, done the MUME way.

The prompt displays the vitals in a graphical way (bars) and also displays status information, like environment lightning, weather, riding, weight and the like.

## Vital bar explanation

MUME does not expose detailed vital information all the time. Expecially during combat you do not see your exact values, but instead of this "vital categories" are given. For example "healthy", "wounded", "bad" and so on for your health.

Prompt displays your vitals in two "layers":

  * The top layer shows you in which "category" you are, e.g. healthy, wounded, and so on. So this is the guaranteed minimum health/mana/move you currently have
  * The middle layer shows:

    * the exact value of your vitals when you are outside of combat
    * the last known value when you are in combat

Now this all sounds very complicated, but it will be easily understandable once you are in the game and see the bars moving.

### Prompt during combat

![Prompt during combat](https://github.com/MuMeM/mume/blob/main/Mudlet/MuMeM-Prompt/doc/Prompt-Combat.png)

### Prompt out of combat

![Prompt out of combat](https://github.com/MuMeM/mume/blob/main/Mudlet/MuMeM-Prompt/doc/Prompt-OutOfCombat.png)

## Installation

**WARNING**: MuMeM-Prompt is conflicting with "mumem_gui". You need to uninstall/disable it first. See below how.

### Via MuMeM Package Manager

Just install [MuMeM Package Manager](https://github.com/MuMeM/mume/tree/main/Mudlet/MuMeM-PkgMgr). You can then install this application with a simple graphical user interfase.

### Manual installation

See the toplevel file for dependencies. Install the package together with the dependencies.

## Uninstallation

Just use the MuMeM package manager and remove the packages. Then *restart* Mudlet!

## Uninstallation of mume_gui

The default MUME GUI (mume_gui) package is *automatically* installed by Mudlet. There is no way to remove it, as it will reinstall itself. So the only way is to disable it. You can do this by

  1. go to the script edit in Mudlet
  2. select the "mume_gui" folder
  3. select the "mume_gui.lua" file
  4. in the first line *insert*: `if 1 == 1 then return end`

*EXCEPTION*: When play MUME via MMapper, "mume_gui" is not installed by default!
