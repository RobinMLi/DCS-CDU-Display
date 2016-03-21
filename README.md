# DCS-CDU-Display
Proof of concept - A cheap solution to create a DCS A-10C CDU display, using latest release of DCS-BIOS


Hardware:

  Arduino UNO R3 board
  
  3.95 inch tft lcd screen
  
  Both are from aliexpress.com and cost about $10. 
  

Required software:

- DCS-BIOS v0.5.0

- DCS-BIOS arduino library v0.2.0

Arduino display library:

  - MCUFRIEND_kbv library
  
  - Adafruit_GFX library
  
Detail is here: https://forum.arduino.cc/index.php?topic=366304.0


The default 5x7 font has been modified to handle the special character from A-10C CDU display. 

glcdfont_cdu.c is the modified font file, use it to replace the default glcdfont.c font file in Adafruit_GFX library. 
DCS_CDU_DISPLAY.ino is the ardunio sketch.

