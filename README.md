# Arduino Core for SAMD21 CPU

This repository contains the source code and configuration files of the Arduino Core
for Atmel's SAMD21 processor used on the ZeroSquare32 boards by HITECS SRL.


## Installation on Arduino IDE

ZeroAquare32 board  is an expansion of the Arduino Zero board; therefore, is necessary to install the arduino Zero package first:

    Select Tools > Boards "..." > Boards Manager...
    Select "Arduino SAMD Boards (32-bits ARM Cortex-M0+)"
    Select version 1.6.8 with the small "Select version" box, see the image below.
    Than click on Install
    
    
Must be installed version 1.6.8 becouse ZeroSquare32 board was developed on Package of Arduino Zero Board version 1.6.8.
Using other version board cannot work properly.

After installation of Arduino SAMD Boards (32-bits ARM Cortex-M0+) vers. 1.6.8 is time to install ZeroSquare32 boards package:
 

    Select File­>Preferences.
    Fill in after Additional Boards Manager URLs: https://github.com/gnmas/ZeroSquare32/blob/master/ZeroSquare32.zip?raw=true
    Install the ZeroSquare32 package, the procedure is the same as for the Arduino Zero package.
    Plug in the ZeroSquare32 board.
    Select Tools­>Board­> select ZeroSquare32
    Select Tools­>Port and select the correct COM port.  

Now you are ready to debug your sketch.

 

## Support

There is a dedicated section of the Arduino Forum for general discussion and project assistance:

http://forum.arduino.cc/index.php?board=98.0

## Bugs or Issues

If you find a bug you can submit an issue here on github:

https://github.com/arduino/ArduinoCore-samd/issues

Before posting a new issue, please check if the same problem has been already reported by someone else
to avoid duplicates.

## Contributions

Contributions are always welcome. The preferred way to receive code cotribution is by submitting a 
Pull Request on github.

## Hourly builds

This repository is under a Continuous Integration system that every hour checks if there are updates and
builds a release for testing (the so called "Hourly builds").

The hourly builds are available through Boards Manager. If you want to install them:
  1. Open the **Preferences** of the Arduino IDE.
  2. Add this URL `http://downloads.arduino.cc/Hourly/samd/package_samd-hourly-build_index.json` in the **Additional Boards Manager URLs** field, and click OK.
  3. Open the **Boards Manager** (menu Tools->Board->Board Manager...)
  4. Install **Arduino SAMD core - Hourly build**
  5. Select one of the boards under **SAMD Hourly build XX** in Tools->Board menu
  6. Compile/Upload as usual

If you already installed an hourly build and you want to update it with the latest:
  1. Open the **Boards Manager** (menu Tools->Board->Board Manager...)
  2. Remove **Arduino SAMD core - Hourly build**
  3. Install again **Arduino SAMD core - Hourly build**, the Board Manager will download the latest build replacing the old one.

## License and credits

This core has been developed by Arduino LLC in collaboration with Atmel.

```
  Copyright (c) 2015 Arduino LLC.  All right reserved.

  This library is free software; you can redistribute it and/or
  modify it under the terms of the GNU Lesser General Public
  License as published by the Free Software Foundation; either
  version 2.1 of the License, or (at your option) any later version.

  This library is distributed in the hope that it will be useful,
  but WITHOUT ANY WARRANTY; without even the implied warranty of
  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
  See the GNU Lesser General Public License for more details.

  You should have received a copy of the GNU Lesser General Public
  License along with this library; if not, write to the Free Software
  Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA  02110-1301  USA
```
