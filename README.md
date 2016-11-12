giri-fu-hw
==========

Hardware module of the giri-fu functional unit, that is a simple relay board, with its own MCU.

It is a proof of concept for a tiny autonomous device, that is able to control 24 VAC magnetic valves in real circumstances:

- wet and dirty environment,
- wide range of temperature,
- mechanical stress.

The [functional block diagram of the unit](docs/images/giri-fu-hw_fbd.png) demonstrates how to connect it into its environment.

![functional block diagram of the unit](docs/images/giri-fu-hw_fbd.png?raw=true)

The v1.0.x version is just documenting [the early prototype](docs/images/prototype.jpg?raw=true "giri-fu-hw prototype"),
that was made on a raster panel. (Note: The PCB design differs from the raster panel version).

The PCB layout was intentionally designed to be very simple, in order to make it easy to reproduce with DIY technologies.

The top layer can be substituted with, straight jumper wires, so it is enought to make a one-sided panel, with the bottom layout.

The firmware implementation can be found in the [giri-fu firmware repository](https://github.com/tombenke/giri-fu).


## Features

- Standalone MCU (ATMega328P, 16MHz)
- High-voltage, high-current darlington transistor array (ULN2003A)
- 6 relays to switch 24V AC current, for magnetic valves (RSY-5)
- 12V AC input for Power supply

Dimensions: 3.6 x 2.15 x 0.5 inch

Boxing: The minimum required internal size of box: 4.75 x 3 x 1.5 inch

Mounting: N.A.

Inputs:

- 12V AC, min: ? A (TBD.)
- 24V AC, min: ? A (TBD.)

Outputs (6x):

- Carry current: 2 A
- Max. operating voltage: 125 VAC, 60 VDC
- Max. operating current: 1 A
- Max. switching capacity: 62.50 VA, 30W
- Min. permissible load: 1 mA, 5 VDC


## Artifacts

The `src` folder holds the EAGLE files:

- `src/giri-fu-hw.sch`
- `src/giri-fu-hw.brd`

The `dist` folder contains the final products for manufacturing:

- [The schematic diagram](dist/giri-fu-hw_sch.pdf)
- [The PCB layout](dist/giri-fu-hw_brd.pdf)
- [PCB top layer (to print)](dist/giri-fu-hw_top.pdf)
- [PCB bottom layer (to print)](dist/giri-fu-hw_bottom.pdf)


## References

- [giri-fu firmware](https://github.com/tombenke/giri-fu)
- [ATMega328P datasheet](http://www.atmel.com/Images/Atmel-42735-8-bit-AVR-Microcontroller-ATmega328-328P_datasheet.pdf)
- [Rayex RSY-5 relay datasheet](docs/datasheets/RSY-5G5V1K5V1_EN.pdf)
- [ULN2003A datsheet](https://www.sparkfun.com/datasheets/IC/ULN2003A.pdf)
- [Making of PCBs at home, DIY using inexpenive materials](https://www.youtube.com/watch?v=mv7Y0A9YeUc)

