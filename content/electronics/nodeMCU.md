[[electronics]]

# NodeMCU v3

This module is sold under many names for around $6.50 on AliExpress and it’s one of the cheapest, fully integrated ESP8266 solutions.

It’s an open hardware design with an ESP-12E core and 4 MB of SPI flash.
According to the manufacturer, “with a micro USB cable, you can connect NodeMCU devkit to your laptop and flash it without any trouble”. This is more or less true: the board comes with a CP2102 onboard USB to serial adapter which just works, well, the majority of the time. Sometimes flashing fails and you have to reset the board by holding down FLASH + RST, then releasing FLASH, then releasing RST. This forces the CP2102 device to power cycle and to be re-numbered by Linux.

The board also features a NCP1117 voltage regulator, a blue LED on GPIO16 and a 220k/100k Ohm voltage divider on the ADC input pin. The ESP-12E usually has a led connected on GPIO2.

Full pinout and PDF schematics can be found here [^1]

RST button turns power off
FLASH chip into flashing mode — ready to import code or firmware

Hold FLASH while clicking RST

VIN = 5V

Some pins are HIGH (3V3) at boot [^2]

[^1] https://medium.com/@bass.pj/nodemcu-esp8266-getting-started-with-arduino-on-macos-1cdc61565496
[^2] https://randomnerdtutorials.com/esp8266-pwm-arduino-ide/