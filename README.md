# OpenOCRCorrect
This project belongs to [@rohitsaluja22](https://github.com/rohitsaluja22/OpenOCRCorrect). I have just added the requested feature.

## Ubuntu and Qt version
Compiled and tested on Ubuntu 20.04 with Qt 5.14.2

## Installation
1. Install Qt 5
  - $ sudo apt-get install qt5-default
2. Open terminal in OpenOCRCorrect folder and run the following commands
  - $ qmake qpadfinal.pro
  - $ make
 
## How to run the code?
To execute the file in QOpenOCRCorrect folder  
  - $ ./qpadfinal
  
## What has been done?
Bold/ un-bold of an individual text has been added.

## Issues
- Loading the dictionary before opening any final crashes the app after a right-click in the textBrowser window.
- Type in slp1 format and press “Cntrl+d” to change the text under cursor to Devanagari. There are some issues in the format. Eg: % -> ॐ instead of ऩ् as mentioned in the application's slp1 guide.

## Challenges
The bold feature is present under the menubar item 'Edit'. The challenge I faced was that when after creating a slot for bold and building the code, it showed the following error: **Class Ui_MainWindow has no such member actionBold**.
**Solution:** I deleted the file ui_mainwindow.h and then in the projects panel in QtCreator I unchecked/checked the shadow build checkbox.

## Features
The following two features are added
  - **Bold:**
    Selected text can be made bold/ un-bold using Ctrl+B or using Edit->Bold
    
## References

- https://www.youtube.com/watch?v=x858_WCtl_Y
- https://stackoverflow.com/questions/22824528/qt-creator-not-showing-ui-changes-when-run







