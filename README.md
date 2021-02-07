# EasyFlash3-Core

## Introduction

This is the EasyFlash 3 CPLD Core. It is used to configure the CPLD
to define the behavior of the hardware.

## Website, Repository and Issue Tracker

EasyFlash website: https://skoe.de/easyflash/

Official repository and issue tracker:
https://gitlab.com/easyflash/easyflash3-core/.

Other EasyFlash related repositories:
https://gitlab.com/easyflash/

Source repository mirror:
https://github.com/easyflash-mirror/easyflash3-core/.

## License

(C) Thomas 'skoe' Giesel

Refer to [LICENSE.md](./LICENSE.md).

## Changes

Version 1.1.1 - 18.08.2012

- Re-enabled AR/RR-mode, which I forgot in 1.0.0 *fp*

Version 1.1.0 - 17.08.2012

- Improved compatibility of KERNAL implementation

Version 1.0.0 - 06.06.2012

- USB and I/O2 RAM are also active in KERNAL mode
  - Allows USB-related features in a special KERNAL currently being
    developed
- KERNAL implementation uses a cleaner timing now
- CPLD Version register added ($de08)
  - Will be displayed in the next menu version, not release yet
- Improved C128 support
  - 2 MHz mode works in EasyFlash mode (needed for PoP)
  - Added a way to leave to C64 mode or to C128 mode
    - Will need a menu update, not release yet
  - Still NO external KERNAL on C128!
- Many optimizations to get all this crap into the CPLD

Some of the features will need a software update which is not release yet.
Do not try to start an external KERNAL on the C128, it will crash.

Version 0.9.2 - 09.01.2012

- LED implemented
  - In EasyFlash mode: LED controlled by software
  - In AR/RR/NP/SS5 mode: On when cartridge is active, off when it is inactive

Version 0.9.1 - 19.12.2011

- Weird glitch in A14 fixed

Version 0.9.0 - 18.12.2011

- First pre-release
- Known limitation: No or only very limited support for C128
- USB not tested
