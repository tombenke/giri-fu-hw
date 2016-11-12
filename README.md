giri-fu-hw
==========

The hardware module of giri-fu functional unit, that is asimple relay board, with an MCU unit.

The v1.0.0 version is just documenting [the early prototype](docs/images/prototype.jpg?raw=true "giri-fu-hw prototype"),
that was made on a raster panel.

The PCB layout was intentionally designed very simple, in order to make it easy to reproduce with DIY technologies.

The top layer can be substituted with simple, straight jumper wires.

![Alt text](docs/images/prototype.jpg?raw=true "giri-fu-hw prototype")

## Features:

- Standalone MCU (ATMega328P, 16MHz)
- 6 relays to switch 24V AC current (for magnetic valves)
- 12V AC input for Power supply

Dimensions: 3.6 x 2.15 x 0.5 inch

Boxing: The minimum required internal size of box: 4.75 x 3 x 1.5 inch

Mounting: N.A.

## Artifacts

The `src` folder holds the EAGLE files:

- `src/giri-fu-hw.sch`
- `src/giri-fu-hw.brd`

The `dist` folder contains the final products for manufacturing:

- [The schematic diagram](dist/giri-hw_brd.pdf)
- [The PCB layout](dist/giri-hw_sch.pdf)
- [PCB top layer (to print)](dist/giri-hw_top.pdf)
- [PCB bottom layer (to print)](dist/giri-hw_bottom.pdf)


## References:

- [ATMega328P](http://www.atmel.com/Images/Atmel-42735-8-bit-AVR-Microcontroller-ATmega328-328P_datasheet.pdf)
- [Rayex RSY-5 relay](docs/datasheets/RSY-5G5V1K5V1_EN.pdf)
- [Making of PCBs at home, DIY using inexpenive materials](https://www.youtube.com/watch?v=mv7Y0A9YeUc)
