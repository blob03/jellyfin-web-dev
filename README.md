This branch is the Merging of all branches with the most uptodate Jellyfin-web client available.<br/>
Releases ('PatchBundle') are produced from this.

## Installation

As a prerequisite you need nodejs and npm to be installed in your system.<br/>
This can be achieved on Ubuntu systems using a simple command line like #sudo apt install nodejs.

Clone this repository<br/>
#cd into its main directory<br/>
#npm install<br/>
#npm run build:production (or development)<br/>
#sudo mv /usr/share/jellyfin/web /usr/share/jellyfin/web.orig<br/>
#sudo cp -rf dist /usr/share/jellyfin/web

To test, connect jellyfin with your browser as usual  (SRV IP address:8096 by default).<br/>
Flush your browser's cache if necessary.


## Patch Bundle details

### RelocateAccessSchedule
Relocate the "Access Schedule" settings into the access tab.

### AutoLogoutScreenSaver
Add a screen saver to automatically sign users out to keep their account safe.

### FixLogoScreenSaver
Fix screensaver 'Logo' appearing behind the top toolbar and the footer frames.<br/>
Fix screensaver 'Logo' incorrectly centered.

### FixScreenSaverManager
Fix mousewheel and middle/right click events not handled by the screensaver manager.<br/>
Fix keypress events not resetting the screensaver manager internal timer.<br/>
Fix event propagating to the UI when leaving a screensaver.

### ImproveDisplayModeTV
Remove margins of section Libraries which caused the screen to scroll horizontally when navigating using arrow keys.

### ThemeHalloween
Introduce a new Halloween style theme filled with terror.

### ImproveQuickConnect
Place the QuickConnect page content at the center of its frame. This is consistent with how other pages are rendered.

### Adjustable Clock
Allow the clock to be disabled from the display settings in TV mode.<br/>
The clock can now display the date of the day.<br/>
Provide several date and time formats that users can select by repeatedly clicking on the clock.

### FixAddMediaToPlaylistsAndCollections
Allow Lg TVs and TV mode to access “Add to Collection” and “Add to Playlist” through the contextual menu available in the detail page.<br/>
Allow Lg TVs and TV mode to access the management menu of playlists and collections list view, thus allowing the removal of items individually.<br/>
Allow TV mode to use the drag handle in list view.

### ShuffleAndPlayAllButtonsForSeriesLibs
Add Shuffle and 'Play All' buttons to the series library browser in Shows and Episodes views.

### FixSubmitDisplaySettingsOnTV
Prevent corruption of the layout parameters in use and the subsequent break of the web Client after the submission<br/>
of the display settings from a TV device.




