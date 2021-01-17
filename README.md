# ORIO2
Open Robot IO Controller Version 2 Rev 2.

A [PDF of the schematic can be found here](2060-ORIO2.pdf).

This project contains 
[KiCad 5](https://kicad.org/) 
design files for a 
[Rasbperry PI](https://www.raspberrypi.org/products/)
add-on module that can be used to operate a robot such as those used in 
[First Robotics Competition](https://www.firstinspires.org/robotics/frc).

The ORIO2 adds the following I/O ports to a Raspberry PI:

* 10 5V tolerant LVTTL quadrature inputs with 3.3v or 5v power
* 8 5V tolerant LVTTL digital inputs with 3.3v or 5v power
* 8 LVTTL digital outputs with 3.3v or 5v power
* 16 direct-FPGA GPIO pins on header with 3.3v power
* 1 Power LED
* 8 User LED outputs
* 8 User switch (binary inputs)
* 2 User push-button (binary inputs)
* 8 ADC inputs 0-5V (w/jumper on port 0 to monitor battery voltage)
* 16 PWM outputs w/6V, 3A power
* 1 12V RSL light output
* 8 24V solenoid outputs
* 1 12V air-compressor relay control output
* 1 Raspberry PI I2C pinout with 3.3V power supply & pullup resistors

All I/O is controlled with a Lattice ICE40HX4K-TQ144 FPGA that 
communicates with the PI using the PI's SPI port.

The FPGA and Raspberry PI source code is open-source and managed 
using a github repo here: 
[ORIO2-software](https://github.com/johnwinans/ORIO2-software)

![PCB Image](2060-ORIO2.png)
