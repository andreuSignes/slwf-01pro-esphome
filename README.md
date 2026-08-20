## This repository contains ESPHome yaml configs for SLWF-01pro v1.1 and v2.1 devices.

## Automatic firmware updates via Home Assistant

Both `slwf01pro_v2.1.yaml` and `slwf01pro_v1.1.yaml` are configured with the ESPHome
[`update: http_request`](https://esphome.io/components/update/http_request/) component.
Once a device is added to Home Assistant, it polls the manifest at the repo root
every 6 hours and surfaces an "Update available" badge in
**Settings → Devices & Services → SLWF-01Pro → Update** whenever a new release ships.
Click install and HA flashes the firmware over HTTP — no manual reflash required.

The web flasher and USB-C flashing paths below remain available as fallbacks.

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