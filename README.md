# Phendrana
Repository for the Phendrana Keyboard - a split keyboard based on the nrf52840 and ZMK
## Photos
![Photo1](/Photos/20230405_115505.jpg)
## Demo

## Features
- Longer Battery Life
- Multiple Bluetooth Connections
- Single-colour Backlight
- Cherry MX and Kailh Choc compatible
- Hotswap Switches, Battery, and MCU

## Firmware
Firmware can be found [here:](https://github.com/LegoRocket/Phendrana-ZMK)

### Compiling
To compile firmware for Phendrana
0. Ensure the .UF2 bootloader is installed from here: (to be added later) (Version * currently works)
1. Download the Phendrana Firmware repo
2. Follow the [ZMK Toolchain Setup](https://zmk.dev/docs/development/setup) Guide Local Build Guide
3. Place the Phendrana files in the zmk/app/boards/shields/Phendrana folder (you will need to make the folder)
  - It should look like below:
4. Open the zmk/app folder in terminal
5. Use the command "west build -b -p nrf52840 --DSHIELD=phendrana_left" to build the left half firmware
6. Use the command "west build -b -p nrf52840 --DSHIELD=phendrana_right" to build the right firmware
7. Upload both firmwares, to their respective halves, attempt to powerup at a similar time (The halves should automatically connect to each other)

## Inspirations
- [The Sanctuary](https://github.com/LegoRocket/Sanctuary-Keyboard-Hardware)
- [ZMK](https://zmk.dev/)
- [Quefrency](https://keeb.io/collections/quefrency-split-staggered-65-keyboard)

## Versions
Rev 1.0.0 - Initial Release - Small errors, requiring 1 wire for USB connection, as well as other small wires to fix small trace errors
