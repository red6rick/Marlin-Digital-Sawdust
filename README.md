# Marlin for Sapphire Pro

# With 4 x TMC2209 (UART), auto off heat sink fan and optical endstop on Z axis

A few pictures of the hardware side

![Wiring](https://www.thingiverse.com/thing:4344191)

## Marlin 2.0 Bugfix Branch

__Not for production use. Use with caution!__

## Files adapted to Sapphire Pro with TMC2209 (UART)

* pins_MKS_ROBIN_NANO.h
* HAL_LCD_class_defines.h
* u8g_dev_tft_480x320_upscale_from_128x64.cpp
* Conditionals_LCD.h
* ultralcd_DOGM.h
* sdio.h
* Configuration.h
* Configuration_adv.h

Most parts of the changes were copied from https://github.com/porlock/SapphireProMarlin2.0stable

## Sapphire Pro modifications
* 4 x TMC2209 with UART wires to stepper E1 pins and thermocouples pin
* Hotend heat sink fan on HE1 connector (turns off below 50°C)
* Optical endstop on Z axis
* E3D V6 hotend with sock

See the location of the pins here https://github.com/makerbase-mks/MKS-Robin-Nano/blob/master/hardware/MKS%20Robin%20Nano%20V1.2_004/MKS%20Robin%20Nano%20V1.2_004%20PIN.pdf

## License

Marlin is published under the [GPL license](/LICENSE) because we believe in open development. The GPL comes with both rights and obligations. Whether you use Marlin firmware as the driver for your open or closed-source product, you must keep Marlin open, and you must provide your compatible Marlin source code to end users upon request. The most straightforward way to comply with the Marlin license is to make a fork of Marlin on Github, perform your modifications, and direct users to your modified fork.

While we can't prevent the use of this code in products (3D printers, CNC, etc.) that are closed source or crippled by a patent, we would prefer that you choose another firmware or, better yet, make your own.
