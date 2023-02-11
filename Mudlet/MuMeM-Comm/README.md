MuMeM Communicaton
============================

## Description

MuMeM Communication is a communication panel for MUME. It captures communication via GMCP, so no "triggers" required and is thus very reliable. The chat messages are stored in a central repository, which can be accessed by various means. For example you can have multiple windows open that filter the messages on channels.

![MuMeM Communication ](https://github.com/MuMeM/mume/blob/main/Mudlet/MuMeM-Comm/doc/MuMeM-Comm.png)
![MuMeM Communication Multi ](https://github.com/MuMeM/mume/blob/main/Mudlet/MuMeM-Comm/doc/MuMeM-Comm-Multi.png)

## Installation

### Via MuMeM Package Manager

Just install [MuMeM Package Manager](https://github.com/MuMeM/mume/tree/main/Mudlet/MuMeM-PkgMgr). You can then install this application with a simple graphical user interfase.

### Via command line (EXPERTS ONLY)

You need to install this package, and all its dependencies

    https://github.com/MuMeM/mume/raw/main/Mudlet/MuMeM-Core/MuMeM-Core-latest.mpackage
    https://github.com/MuMeM/mume/raw/main/Mudlet/MuMeM-Log/MuMeM-Log-latest.mpackage
    https://github.com/MuMeM/mume/raw/main/Mudlet/MuMeM-GMCP/MuMeM-GMCP-latest.mpackage
    https://github.com/MuMeM/mume/raw/main/Mudlet/MuMeM-Comm/MuMeM-Comm-latest.mpackage

## Usage

### Basic

You can add a new window with "`mcomm window create <name>`". The window will then automatically appear.

### Window layout

The window consists of a tab pane on the top and a message pane on the lower part, containing the chat messages.

Buttons have have different meanings, depending on their scope:

  * The light blue buttons, called "Tales", "Says", ... are channel buttons. Left clicking this button enables/disables the channel. Right clicking the button only ables the selected channel (aka disables all others)
  * The "All" button quickly switches the channels on. Left click is switch all channels on, and right click to switch them off
  * The group buttons "Direct", "Local", "Global" build groups of channels. Left clicking such a button adds the related channels to the selection. Right clicking adds only the group and removes the others.

Sounds complicated? Just left and right click the buttons and see what happens. It should be pretty intuitive once you get the hang of it.

### Commands

`mcomm list` - gives a list of all known windows
`mcomm window create <name>` - creates a new window and shows it
`mcomm window show <name>` - shows a previously hidden/closed window
`mcomm window hide <name>` - hides/closes a window. same effect as clicking the "X" on the window title bar

## FAQ

#### How do I update a package?

Use [MuMeM Package Manager](https://github.com/MuMeM/mume/tree/main/Mudlet/MuMeM-PkgMgr).

#### I have many windows open. Does this slow down my system

Every new window will *slightly* slow down due to some overhead. But the storage is central and updates are done via events. You will however copy the UI elements and the chat body as shown in the window.

To summarize: A couple of windows are perfectly fine, but more than 10 might have some impact.

### I want to use this for my own project and extend the classes

It is made to be extendable in the code. Look at the code itself, you can easily extend the classes and tweak them to your liking.