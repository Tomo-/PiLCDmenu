PiLCDmenu
=========

Menu for use with standard 16x2 LCD and Raspberry Pi

RaspberryPiLcdMenu
==================

A menu driven application template for the Adafruit LCD Plates on a Raspberry Pi.

It provides a simple way to navigate a nested set of menus, and run various
functions, by pressing the buttons connected to the GPIO pins.  Included is a way
to determine the IP address of the Pi when running
headless.  Also, allows the user to select from a large list of choices (using
List Selector), by cycling through letters vertically and horizontally.
It uses an XML file to configure the menu structure, and processes tags to
enable different options.  XML element support includes:
- folders, for organizing menus.
- widgets, which are really just functions to call in the code.
- run, which allows you to run any command and see the output on the LCD.
- 


Some of the canned menu items are functional, but other are place holders to
spawn ideas.  Such as using gphoto2 to trigger DSLR camera operations, or using
raspistill to capture images from the Pi Camera.  Or using the ephem library to
do astronomy calculations.  Or connecting the Pi to your GPS to auto locate.

To get started, put all these files somewhere.  Then obtain the Adafruit LCD
python code.  From that, copy the Adafruit_CharLCD.py from:
Adafruit-Raspberry-Pi-Python-Code/Adafruit_CharLCD
into the same folder as this code.



Then you should be able to do:
python lcdmenu.py

Enjoy!

===========
Changes:
24-Aug-2014
 - Added support to set date/time
 - Fixed bug to allow backing out of ListSelector
 - Added support for a reboot command
 - Heavily modifed to use standard LCD's rather than Adafruit_LCDPlate //TomoDev

 

GPL v3 license, kindly include text above in any redistribution.
