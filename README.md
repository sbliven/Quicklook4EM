# Quicklook 4 Electron Microscopy

These plugins all you to quickly inspect three types of EM file formats:

- EM
- MRC
- CCP4

# Functionality
The plugins load each file seperately from disk. Take care when running the plugins over a networked filesystem since that might significantly slow down your user experience when viewing large files. For tomorgrams, only the central slice will be used for display. 

# Requirements
Mac with installed XCode

Git

# Structure
Each format has it's own, independent code stored as a XCode project. You have to build each project seperately to get all plugins.

# Building
Simply clone the repository and run **Archive** in the XCode -> Product menu. This will build the `qlgenerator` file into the open project. Search for it in the XCode project browser.

# Installing
Move the built files `(*qlgenerator)` to `~/Library/QuickLook`. For activating the features you have to reboot / log out and log back in to your OSX session or type `qlmanage -r` in the terminal. You coulds also place the files into `/Library/Quicklook` but that requires administrator rights to that machine.

# License
Released under GNU GPLv3
