# Open LCC Debug Board

Schematics and PCB files for the Open LCC debug board. Licensed under the CERN OHL-P license.

The Debug Board exposes SWD, JTAG, USB and Reset/GPIO0/Bootsel for the RP2040 and ESP32-S3 on the Open LCC Main Board.

It also has an optional boost converter to provide 12V instead of 5V as VIN to the Open LCC Main board. When using the color TFT, this doesn't matter at all. When using the OLED, the OLED is dimmer when powered using 5V. You probably don't need this boost converter.

## Disclaimer

Anything you do with this, you do at your own risk. Components have been fried already during the course of this project. Your machine uses both line voltage power, high pressured hot water, steam and other dangerous components. Risks include but are not limited to, damaging the machine, personal injury, property damage and summoning dead Cthulhu from his sleep at R'lyeh.