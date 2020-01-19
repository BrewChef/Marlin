# Marlin 3D Printer Firmware for Prusa i3 MK3 + BigTreeTech BTT002/TMC2209s

![GitHub](https://img.shields.io/github/license/marlinfirmware/marlin.svg)
![GitHub contributors](https://img.shields.io/github/contributors/marlinfirmware/marlin.svg)

![image](https://user-images.githubusercontent.com/13375512/71555715-1cc24f00-29e4-11ea-89d4-ad3bfa27b243.png)

# WORK IN PROGRESS! USE AT YOUR OWN RISK!

This firmware is configured for a [Prusa i3 MK3](https://www.prusa3d.com/original-prusa-i3-mk3/) modded with a [BigTreeTech BTT002 motherboard](https://twitter.com/biqu_hope/status/1189807693336236032)/TMC2209s.

Make sure the jumpers under your drivers are set to "TMC2208-UART MODE" since this config is for TMC2209s:
![image](https://user-images.githubusercontent.com/13375512/72644762-b23b6980-3926-11ea-8c01-950351374699.png)

## To-Do
* Tune PID settings since they are causing thermal runaways
* Verify `*_STALL_SENSITIVITY`
* Tune `ADVANCED_PAUSE_FEATURE`
* Verify `LCD_FEEDBACK_FREQUENCY_DURATION_MS`/`LCD_FEEDBACK_FREQUENCY_HZ` settings
* Verify PINDA V2's temperature support/tune thermal probe compensation settings
* Enable/verify `Z_STEPPER_AUTO_ALIGN`

## Known Issues
* Z homing doesn't work correctly on my machine, but does others. Test homing with something metal near the PINDA to see if yours works.
* Probably other settings as well... WORK IN PROGRESS! USE AT YOUR OWN RISK!

Don't forget to Initialize EEPROM through the menu or by sending `M502`, followed by `M500` after updating your firmware.
