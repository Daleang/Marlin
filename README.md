# Marlin 3D Printer Firmware for the Creality Ender-3
<img align="right" src="../../raw/1.1.x/buildroot/share/pixmaps/logo/marlin-250.png" />

## Additional Information

This firmware is configured for the Creality Ender-3 with a Biqu/BigTreeTech SKR 1.3 and TMC5160s *with* Linear Advance enabled ([demo](https://youtu.be/DplBQubcGCM)) as well as the following mods:
* 1/32 microstepping
* Bondtech BMG/E3D V6 in direct drive ([Petsfang](https://www.thingiverse.com/thing:2963434))
* 0.9 LDO pancake stepper
* Copper block + Slice Engineering vanadium nozzle
* BLTouch
* Anycubic AC-3D651/Busheng 17HD40005-22B, 1.8 degree stepper on Y-axis
* Creality 42-40/JKong Motor JK42HS40-1004A-02F 1.8 degree stepper on X-axis (formerally used as the extruder motor)
* Custom Keenovo AC-powered bed w/ removable spring steel sheet
* Linear rail on Y
* Pi/OctoPrint (SD card changes were to allow for remote firmware updates)


After flashing, make sure you run `M502`, then `M500` to pull default settings from the firmware.
You'll also need to disable StealthChop on X, Y, & E through the TMC Settings menu or send `M569 S0 X Y E` and `M500` in order to use Linear Advance and to not skip steps.
