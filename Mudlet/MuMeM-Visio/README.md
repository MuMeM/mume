MuMeM Visio
============================

## Description
MuMeM visio is a POC (Proof of Concept) on how to display images of rooms in MUME. In its current form it is very basic and just aims to give an impression of what a solution could look like.

![MuMeM-Visio Screenshot](https://github.com/MuMeM/mume/blob/main/Mudlet/MuMeM-Visio/doc/MuMeM-Visio.png)

## Installation
Download the latest package from this website and install it in Mudlet via the package manager. This will install a "directory" called "MuMeM-Visio" in the scripts section of Mudlet.

To install the image pack, see below.

## Uninstallation
Use the packaged manager of Mudlet to remove the package and restart.

## Image-Pack installation

### "automatic" download
Open "MuMeM-Visio" by typing "visere". Click on the "download images" button in the middle of the interface. Watch the log pane for progress and possible errors.

### Manual installation
You can download the image pack from this website (image-pack.zip). Unzip it and move the **RoomImages** into the directory/folder which is shown in the "Data Directory" at MuMeM-Visio.

### Manual installation (detailed steps)

 1. Download the image pack from this web site (image-pack.zip)
 2. Unzip the file
 3. Lookup the Data Directory in MuMeM-Visio's graphical interface
    * You need to start Mudlet for this!
 4. Create the directory if required (or the missing subpathes)
    * Linux example: `mkdir -p /home/MuMeM/.config/mudlet/profiles/MMaper/MuMeM-Visio`
 5. Copy the RoomImage directory into the Data Directory
    * Linux example: `cp RoomImages /home/MuMeM/.config/mudlet/profiles/MMaper/MuMeM-Visio/`

## Using the package / addon
The package adds a "visere" command. Just type "visere" to open the graphical window. If you close the window (via the x), you can open it again by typing "visere".

Note that the addon will start in "de-activated" state, and thus not draw rooms. To activate the room drawing, just press on "activate" in the GUI of MuMeM-Visio.

**WARNING**: You should deactivate the image display when not using the addon, as it will load images while hidden (need to fix this).

## Currently "mapped" areas in the POC
Only a few rooms around the marketsplace of Black Hill Village are mapped (the street, the market, the inn, smitty, ...).

In addition to this the area at the junction far south of Black Hill Village is also mapped with AI generated images. Thanx to Freyja for providing the images!

**WARNING**: Loading of the images takes around one second! So use the "active"/"de-activate" possiblity of MuMeM-Visio! Aka, only activate if you are in a "mapped" area.

**WARNING2**: Be careful in swim situation due to the long image load times!!!

## Adding your own images
You can simply add your own images by placing the picture into the RoomImages directory in the DataDirectory. The Data Directory is displayed in the user interface. The following conditions apply:

  * The filename must be the Hash of the room
    * The room hash is displayed in the MuMeM-Visio windown while standing in the room
    * Press "print hash" to have the hash printed into log window for easy copy & paste
  * There file must not have an extension (like .jpg or .png). Only the roomhash by itself.
  * The image size is restricted to 400x400. Larger immages will **not** be scaled down.
  * Use "redraw" to see the effects (or do "look" in the room)

**Update**: Since version v0.1.1 you can now use the "import image" button in the user interface, which will directly import the image file you select via the file dialogue and rename it to the hash. You still need to resize the image first though by yourself!

## Caveats / Future
As said above, this is a POC of how something like this could look like. There are many ideas how this can be improved

  * Download the images from the web (technically quite easy)
  * Support query parameters for download (GET is easy, POST bit more difficult)
  * Intelligently cache and download the images
  * Currently hashing is custom lua, which is very slow. Use a different library
  * Add images of people / mobiles in the room
  * Add navigation elements for the exits (e.g. compass like)

In the end a fully graphical, newbie friendly MUME GUI would be the dream...
