# proxmark3-ble
Controlling Proxmark3 with your BLE devices.

** This is an ongoing project, if you have some brillant idea, create a new `Issue`.

## Software

Developing...

Previous version is deprecared https://github.com/DickyT/proxmark3-ios

## Hardware

**Fritzing does not have a community component, so I use RCS22 to replace Proxmark3 in this chart**

**RCS22 : VCC -> Proxmark3 USB VCC+**

**RCS22 : GND -> Proxmark3 USB GND**

**YOU NEED TO CONNECT Proxmark3 USB D+ AND D- TO RASPBERRY PI's MICRO-USB D+ AND D-**

![1](https://user-images.githubusercontent.com/4535844/68543443-15d47400-0385-11ea-825d-cab4162d4516.png)

The base hardware is Raspberry Pi ZERO W version, it comes with WiFi and Bluetooth module, which makes hardware part easier.

You do not need to use a USB-OTG cable, you can solder your own `Micro-USB - Micro-USB` cable refering my diagram.

Since Proxmark3 do have a hardware reset button, but if you put the whole thing into a case, you cannot touch that button, sometimes Proxmark3 just hangs, you NEED to restart it.

I added a transitor (S8050) with a resistor (3.3k) to the power cable, so we can always reset our Proxmark with Raspberri Pi's GPIO pin.
