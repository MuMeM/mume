### 20230318

  * Global class function update

### 20230311

  * Fixed main window params
  * Fixed CHANGELOG version numbering

### 20230228

  * Sneak-Preview: action bar
  * global inheritances changes

### 20230223

  * Mobiles are now "sorted" (kind of)
  * Bugfixes

### 20230219

  * Import of mobiles added
  * Mobiles can now be selected (currently only used for import)
  * Main console background fixed
  * Housekeeping and minor refactoring

### 20230218

  * Added a compass (and again, awesome art by Freyja!)
  * Replaced stock images (kudos again to Freyja!)
  * Redesigned the layout ("menu" bar at top, room layer, action bar, ...)
  * Extra functions now in own sub window ("More...")
  * Room exits are updating (e.g. door status)
  * Enlarged the image
  * [internal] Complete overhaul and refactoring

### 20230211

  * Cleaning up image-pack.zip after download
  * Room image import fixed
  * Startup message removed
  * replaced showWindow(obj) by obj:show() (MacOS 13 bugfix)

### 20230203

  * Clickable exists: When clicking on the exit, you move to that direction
  * Clickable doors: Clicking will open the door, right click brings door-manipulation window
  * Mobiles added to the interface (download resource-pack.zip!)
  * Mobiles auto-update on mobiles entering or leaving the room
  * Rebased on MuMeM support modules (which are now a requirement!)

### v0.1.1

  * Updated image pack, now all rooms include (thanx Freyja!)
  * **Clickable** exits added (work in progress, no "open doors" or the like)
  * **Preview** Background image in main console
  * "background" button toggles modes: off, full screen, center, tiled
  * "Import Image" added. You can now import a single image from your local drive
  * Room name now colored (green) and using different "coloring" (due to widget change)
  * Fixed a bug when Room.Info.desc was not know ("pitch black") (thanx nuzo!)
  * Removed double calculation of roomHash at redraw (redraw now twice as fast!)
  * [Internal] Changed RoomInfo visual from Label to MiniConsole

### v0.1.0

  * **BREAKING** New image file location ("data dir"/RoomImages)
  * You can now easily download the images in the MuMeM Visio interface
  * Redraw duration now also shows
    * hashing duration (time it took to calculate the has)
    * gui duraton (time it took to do the visual redraw)
  * Room image background now black (instead of grey)
  * Main window docking now defaults to "true"
  * Main window now has a title

### v0.0.2-alpha

  * Updated image-pack with images of Freya
  * Now starts in "de-activated" mode
  * New image if image is not found
  * Updated README.md
  * Minor bugfixes

### v0.0.1-alpha

  * Initial Releaase
