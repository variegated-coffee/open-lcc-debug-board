# How to order and assemble

## PCB and PCBA manufacturer

This directory contains Gerber files for the PCB, a BOM file with LCSC numbers for ordering with JLCPCB, and a CPL file.

### Orientations

Be careful with the orientation of the FPC connector on both this and the main board. Pin 1 is indicated on the board. When placed correctly on both the Open LCC and Debug board, you should use an FPC cable with *connectors on opposite sides*. If for some reason the connector is incorrectly oriented, you'll still be able to use the boards, but you may need an FPC cable with connectors on the *same* side. 

Orientations in general are a bit of a pain. I recommend checking the "Confirm production files" option on JLCPCB, to be able to verify that the orientations of all the components match the PCB and schematic.

## Parts you'll need from other vendors

The BOM in the file isn't complete; you'll need a few other parts, all of which are hand soldered. Below is a table, including links to Digikey when the item is available there.

| Designator  | Part name                     | Notes                                                            | URL (for one vendor, usually there are others)                                            |
|-------------|-------------------------------|------------------------------------------------------------------|-------------------------------------------------------------------------------------------|
| J8, J9      | 2x10 pin IDC Male header      | Optional, intended to be used with J-Link                        | https://www.digikey.se/en/products/detail/sullins-connector-solutions/SBH11-PBPC-D10-ST-BK/1990065 |
| SW3-SW5     | Omron B3S-1000                |                                                                  | https://www.digikey.se/en/products/detail/omron-electronics-inc-emc-div/B3S-1000/20686    |
| SW1         | 2x DIP switch                 |                                                                  | https://www.digikey.se/en/products/detail/grayhill-inc/78B02T/726239 |
| SW2         | 2.54 mm SPDT switch           | Can be replaced with a 2 or 3 pin header and a jumper            | https://www.digikey.se/en/products/detail/eao/09-03290-01/8733106 |
| R2          |                               | Current limiting resistor for RP2040 RESETn | |
| U2          | PTN04050C Boost module        | Optional, supplies 12V to main board VIN instead of 5V.          | https://www.digikey.se/en/products/detail/texas-instruments/PTN04050CAD/864519 |
| R7          | 1K33 Resistor                 | Only required when using PTN0405C                                | https://www.digikey.se/en/products/detail/yageo/MFR-25FBF52-1K33/13036 |
| C5, C6      | 100 µF, 16 V electrolytic cap | Only required when using PTN04050C                               | https://www.digikey.se/en/products/detail/panasonic-electronic-components/EEA-GA1C101/2504576 |