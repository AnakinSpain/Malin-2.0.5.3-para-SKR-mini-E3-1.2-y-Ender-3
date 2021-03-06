﻿<img align="right" width=175 src="buildroot/share/pixmaps/logo/marlin-250.png" />

# Marlin 3D Printer Firmware

[![Build Status](https://travis-ci.org/MarlinFirmware/Marlin.svg?branch=2.0.x)](https://travis-ci.org/MarlinFirmware/Marlin)
![GitHub](https://img.shields.io/github/license/marlinfirmware/marlin.svg)
![GitHub contributors](https://img.shields.io/github/contributors/marlinfirmware/marlin.svg)
![GitHub Release Date](https://img.shields.io/github/release-date/marlinfirmware/marlin.svg)

_Marlin_ es un firmware para máquinas RepRap, tambien conocidas como _3D printers_. Este firmware añade suporte para las placas mucho mas rapidas a 32-bit y ARM mejorando las antiguas de 8-bit usando el  "hardware abstraction layer."

Additional documentation can be found at the [Marlin Home Page](http://marlinfw.org/).
Please let us know if Marlin misbehaves in any way. Volunteers are standing by!

### BigTreeTech Actualiza su firmware, consíguelo aquí:
https://github.com/bigtreetech/BIGTREETECH-SKR-mini-E3

## Building Marlin 2.0 (compilando)

Para compilar Marlin necesitarás [Arduino IDE 1.8.8 or newer](https://www.arduino.cc/en/main/software) o [PlatformIO](http://docs.platformio.org/en/latest/ide.html#platformio-ide) con _[Visual Studio Code](https://code.visualstudio.com/download)_.

- [Instalando Marlin (Arduino)](http://marlinfw.org/docs/basics/install_arduino.html)
- [Instalando Marlin (VSCode)](http://marlinfw.org/docs/basics/install_platformio_vscode.html).

Si instalas VSC ejecutando el archivo "marlin para skr 1.2 y ender3.codework debe cargarte con todo en VSC.

## Objetivo actual

Creality Ender-3 wiconth SKR Mini E3 v1.2 y Creality BLTouch 3.1

## Características activadas:

- BLTouch (Bi-Linear Bed Leveling)
- Custom Status Screen (Ender-3 Default)
- Disable Boot Screens
- Disable Info Screen
- Enabled Slim Menus
- Enabled S Curve Acceleration
- Disable ARC Support (Cura does not have arc support anyway)
- Enabled Linear Advance
- Enabled Square Wave Stepping
- Enabled Hybrid Threshold for TMC2209 Stepper Drivers
- Bed Size is 230x230mm
- Enable Menu to Level Bed Corners (and Center)
- Pre-Heat for "PLA" and "PETG"
- Fix for EEPROM saving issue

## BLTouch conexiones

Conectado según la web de ANTCLABS:

<img src="/img/bltouch-wiring.jpeg" />

Ten en cuenta que los colores pueden variar.

## El archivo Binario está en la carpeta BIN.


Para instalarlo solamente tienes que copiar el archivo que decidas en el SD, encender la impresora y esperar hasta que se reinicie.

3 tipos de firmwares explicados en la descripcion. Yo uso el de 512k. BLTouch usa una cama de 5x5 grid to probe, Manual Bed Leveling usa una cama de 3x3, y 512K usa una cama de 3x3.

- [SKR_Mini_E3_v1.2_256K_BLTouch_v3.1](https://raw.githubusercontent.com/damvcoool/Marlin-2.0.x-SKR-Mini-E3-v1.2/master/bin/SKR_Mini_E3_v1.2_256K_BLTouch_v3.1.bin)
- [SKR_Mini_E3_v1.2_256K_Manual_Bed_Level](https://raw.githubusercontent.com/damvcoool/Marlin-2.0.x-SKR-Mini-E3-v1.2/master/bin/SKR_Mini_E3_v1.2_256K_Manual_Bed_Level.bin)
- [SKR_Mini_E3_v1.2_512K_BLTouch_v3.1](https://github.com/AnakinSpain/Malin-2.0.5.3-para-SKR-mini-E3-1.2-y-Ender-3/blob/master/bin/SKR_Mini_E3_v1.2_512K_BLTouch_v3.1.bin)


## Credits

The current Marlin dev team consists of:

- Scott Lahteine [[@thinkyhead](https://github.com/thinkyhead)] - USA &nbsp; [Donate](http://www.thinkyhead.com/donate-to-marlin) / Flattr: [![Flattr Scott](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=thinkyhead&url=https://github.com/MarlinFirmware/Marlin&title=Marlin&language=&tags=github&category=software)
- Roxanne Neufeld [[@Roxy-3D](https://github.com/Roxy-3D)] - USA
- Chris Pepper [[@p3p](https://github.com/p3p)] - UK
- Bob Kuhn [[@Bob-the-Kuhn](https://github.com/Bob-the-Kuhn)] - USA
- João Brazio [[@jbrazio](https://github.com/jbrazio)] - Portugal
- Erik van der Zalm [[@ErikZalm](https://github.com/ErikZalm)] - Netherlands &nbsp; [![Flattr Erik](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=ErikZalm&url=https://github.com/MarlinFirmware/Marlin&title=Marlin&language=&tags=github&category=software)

- I ONLY make one or two changes from original repository from: https://github.com/damvcoool/Marlin-2.0.x-SKR-Mini-E3-v1.2

## License

Marlin is published under the [GPL license](/LICENSE) because we believe in open development. The GPL comes with both rights and obligations. Whether you use Marlin firmware as the driver for your open or closed-source product, you must keep Marlin open, and you must provide your compatible Marlin source code to end users upon request. The most straightforward way to comply with the Marlin license is to make a fork of Marlin on Github, perform your modifications, and direct users to your modified fork.

While we can't prevent the use of this code in products (3D printers, CNC, etc.) that are closed source or crippled by a patent, we would prefer that you choose another firmware or, better yet, make your own.
