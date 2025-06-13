# Universal WLED PCB Documentation

Universal WLED is a circuit board designed to support a wide range of use cases of the open source LED driver Firmware WLED.

It features:
- an ESP32S3 microcontroller in N16R8 configuration (16MB Flash, 8MB PSRAM in Octa-SPI configuration)
- a USB-C programming interface for the ESP with backfeed protection from the DC/DC
- screw terminal for LED power input, supporting a range from 5V to 24V DC
- a DC/DC converter to power the ESP32S3 from the LED supply, also supporting 5-24V DC
- 2 5V-level shifters to drive addressable LED strip data to a dedicated screw terminal block
- 5 LED PWM channels with very low RDS_on N-MOSFETS in DPAK cases with lots of margin for larger setups
- a female pin header for easy installation of standard IR remote-control sensors
- large screw terminals for the PWM and adressable LED strip interfaces
- one 10-pin and one 12-pin 2.54mm pin header to expose the remaining ESP GPIOs for arbitrary extensions
- indicator LEDs for the 3.3V and 5V supply rails
- on-board PDM microphone (see note for that below, currently not working with WLED audioreactive yet, help wanted!)