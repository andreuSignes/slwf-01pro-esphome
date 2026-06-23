## This repository contains ESPHome yaml configs for SLWF-01pro v1.1 and v2.1 devices.

## How to distinguish between versions?
Version v2.1 has an additional Type-C port.

## Version v1.1 and 1.2
First revisions of the USB dongle.<br>
Device update is only possible via OTA (no USB-TTL convertor on board).<br>
No output for "Follow me".

## Version v2.1
Second generation.<br>
Has a "Follow me" pad that can be soldered to the IR receiver output of your AC, in which case you can use IR capabilities.<br>
Has a separate Type-C port through which the device can be updated via USB cable. Convenient tool for updating [https://smlight.tech/flasher/#slwf01proV2](https://smlight.tech/flasher/#slwf01proV2)<br>
[USB driver installation guide](https://learn.sparkfun.com/tutorials/how-to-install-ch340-drivers/all)<br>

To flash the device:
Connect the device to the PC **with the button pressed**.<br>
After the flashing starts, you can release the button.<br>
If the flashing has not started, repeat the first step!