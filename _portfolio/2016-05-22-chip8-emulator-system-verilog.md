---
title: "Chip8 Emulator on an FPGA"
excerpt: "A Chip8 emulator written to run on an Altera SoCKit Cyclone V FPGA board. "
collection: portfolio
---

# Chip8-SystemVerilog
Implemented a Chip8 Emulator in SystemVerilog meant to run on an Altera SoCKit Cyclone V board

## Software
- [Quartus 13.1](https://dl.altera.com/13.1/?edition=web)
- [Cyclone V Device Drivers](https://dl.altera.com/13.1/?edition=web)
- [Linaro Linux](https://rocketboards.org/foswiki/view/Projects/SoCKitLinaroLinuxDesktop#A_42Run_the_demo_using_the_provided_SD_Card_Image_42)

## Setup
Follow the following two tutorials to get linux running on the SoCKit board
- [Linaro Linux Setup](https://rocketboards.org/foswiki/view/Projects/SoCKitLinaroLinuxDesktop#A_42Run_the_demo_using_the_provided_SD_Card_Image_42)
- [Creating u-boot-scr](https://rocketboards.org/foswiki/view/Documentation/GSRD141ProgrammingFPGAArrowSoCKitEdition)

Then copy the code in chip8-sw to the device and compile it there by calling make. Open Quartus and compile the Chip8.qpf project. Using the programmar load the sockit_top.sof file onto the device and boot the version of linux installed on the sd card. To install the chip8-sw:
```bash
make
insmod chip8.ko
./chip8 <chip8_file>
```
Where a chip8 file is a .chip8 rom file found on many websites. 

## Running
The controls for the chip8 are:
```txt
+---------+
| 1 2 3 4 |
| q w e r |
| a s d f |
| z x c v |
+---------+
```
The display will be outputted via the VGA port on the SoCKit board and is controlled using a USB Keyboard plugged into the board. To pause the game press 'p', to start a rom file press 'enter', and to load a new file press 'l'. 

<div class="github-card" data-github="davidwatkins/Chip8-SystemVerilog" data-width="400" data-height="150" data-theme="default"></div>
<script src="//cdn.jsdelivr.net/github-cards/latest/widget.js"></script>
