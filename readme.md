<img src="images/microchiptechnologyinc.png" height="60">

# AVR128DA48 LED Blink with sleep and wake up using a Timer interrupt example

This repository provides an Atmel Studio solution with a bare metal code example for an LED blink and sleep application. The AVR-da is woken up from sleep using TCA0 interrupt.

This example demonstrates simple toggling on a LED connected to PC6 with a period of 1 second. After toggling the LED, the device enters sleep until it gets woken up by an interrupt from TCA0.


## Configurations

- PC6 - configured as digital output (the on-board user LED)
- TCA0:
	* Normal mode
	* Input clock Main Clock (4MHz) /256
	* Overflow interrupt enabled
	* Period 0x2000
- CPUINT:
	* Global interrupt enabled

<img src="images/AVR128DA48_CNANO_instructions.PNG" height="250">

## Required Tools

- Atmel Studio 7.0.2397 or newer
- AVR-Dx 1.0.18 or newer Device Pack
- AVR128DA48 Curiosity Nano (DM164151)

## Compatibility
The source code is compatible with the following devices: AVR128DA28, AVR128DA32, AVR128DA48, and AVR128DA64.

