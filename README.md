# Custom Firmware for the Wanhao Duplicator i3 v2.1, by Bot-In-a-Box
## Based on Marlin Firmware 1.1.9

A big thank-you is in order to everyone who's contributed to the Marlin Firmware over the years; because of their support Marlin has become a state-of-the-art universal firmware for 3D Printers everywhere. 

The 1.1.x branch is home to all tagged releases of Marlin 1.1 (final version 1.1.9 – August 2018).
For more information about the Marlin firmware head to the [Marlin Homepage - marlinfw.org](http://marlinfw.org/).
Check out Marlin's [Github repo](https://github.com/MarlinFirmware/Marlin/issues) as well.

## About this Firmware

I realized the default firmware that came with my Wanhao Duplicator i3 was, frankly, not great. It was slow, unstable, clunky, and all-around unideal. However, once I realized that it was based on Marlin, I knew I could do better. Besides, Octoprint warned me that the firmware didn't even have built-in thermal protection! But by reading pages upon pages of documentation, example code, and forum posts, I was able to piece together exactly how I needed to alter the Marlin 1.1.9 source code to get it to work with my printer. I'd especially like to point out the posts I found most useful:

[https://www.reddit.com/r/3Dprinting/comments/8o3wg8/installing_marlin_on_maker_select_v2/](https://www.reddit.com/r/3Dprinting/comments/8o3wg8/installing_marlin_on_maker_select_v2/)
[https://www.thingiverse.com/thing:2450111](https://www.thingiverse.com/thing:2450111)

- [Sincerely, Matthew Piercey](https://matthewpiercey.ml)

## Some Features

..* Custom "Chippy" Bootscreen by [Bot-In-a-Box](https://botinabox.ca)
..* Built-in Thermal Runway Protection
..* Change Settings and Save/Load them from EEPROM
..* Printing over SD Micro/USB Mini Support
..* Bed-Leveling Wizard
..* Change Temperature/Position/Extrusion On-the-Fly
..* **TO-DO:** TEMPERATURE SETTINGS ARE A BIT OFF (NOZZLE SHOWS 35C WHEN IT'S 15 INSIDE)
	
## How to Install

	1. Flash the Optiboot Bootloader on your Melzi board after taking it out of the box (I used my Raspberry Pi to do it):[https://www.fission3d.com/guides/flash-bootloader-and-install-firmware-with-raspberry-pi](https://www.fission3d.com/guides/flash-bootloader-and-install-firmware-with-raspberry-pi)
	2. Auto Build the Firmware with Platform.io in Atom [http://marlinfw.org/docs/basics/install_platformio.html](http://marlinfw.org/docs/basics/install_platformio.html)
	3. Auto Upload the Firmware with Platform.io in Atom (After connecting the Melzi to your computer via USB Mini)

## License

Marlin is published under the GPL License, and a copy of that license is included in the source code. It's worth noting that the license explicitly states that any software licensed under it is offered with "NO WARRANTY... OF ANY KIND, EITHER EXPRESSED OR IMPLIED." I'm offering this firmware open-source in the hopes that it might prove helpful to someone else, but I'm not responsible if anything goes wrong with your printer or anything else because of it; it's AS-IS.


