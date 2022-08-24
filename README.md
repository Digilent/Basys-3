# Basys 3 Root Repository

## Basys 3 GPIO Demo

### Description

This branch contains sources for the Basys 3 GPIO Demo.

This project is a Vivado demo using the Basys 3's switches, LEDs, pushbuttons, seven-segment display, VGA connector, USB HID Host port and USB UART bridge, written in VHDL.

When programmed onto the board, all sixteen of the switches are tied to their corresponding LEDs. Every time a switch is toggled, the LED directly above it will toggle with it.

A computer monitor attached to the Basys 3 with a VGA cable displays a series of moving patterns. If a mouse is attached to the USB port when the demo starts running, a cursor is displayed on the screen and can be moved with the mouse.

The seven segment display counts up from 0 to 9 as long as no buttons are pressed. As long as BTNU is pressed, the first digit on the seven segment display is turned off. In the same manner, BTNL turns off the second digit, BTNR turns off the third, and BTND turns off the fourth. BTNC turns off the entire display and resets the counter.
 
To use the USB-UART bridge feature of this demo, the Basys 3 must be connected to a serial terminal on the computer it is connected to over the MicroUSB cable. Whenever the reset button or BTNC is pressed, the Basys 3 sends the line “BASYS3 GPIO/UART DEMO!” to the serial terminal. Whenever one of the D-pad buttons other than BTNC is pressed, the line “Button press detected!” is sent.

| Button | Function                                                          |
| ------ | ----------------------------------------------------------------- |
| BTNC   | Turns off the entire seven-segment display and resets the counter |
|        | Prints "BASYS3 GPIO/UART DEMO!" through theUSB-UART bridge        |
| BTNU   | Turns off the first digit on seven-segment display                |                               
|        | Prints "Button press detected!" through the USB-UART bridge       |
| BTNL   | Turns off the second digit on seven-segment display               |
|        | Prints "Button press detected!" through theUSB-UART bridge        |
| BTNR   | Turns off the third digit on seven-segment display                |
|        | Prints "Button press detected!" through the USB-UART bridge       |
| BTND   | Turns off the fourth digit on seven-segment display               |
|        | Prints "Button press detected!" through the USB-UART bridge       |

For more information on the Basys 3 GPIO Demo, including setup instructions, visit its [Demo Page](https://reference.digilentinc.com/reference/programmable-logic/basys-3/demos/gpio) on the Digilent Wiki.

For more information on the Basys 3, including other demos that may be available, see its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/basys-3/start) on the Digilent Wiki.

### Git Navigation Information

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked above.

To see other demos in this repository, see the master branch's [README](https://github.com/Digilent/Basys-3).

Some demos do not require some submodules, in these cases, they are still provided to ease switching between demos in git. When unused, the submodule folder is largely empty, except for a readme containing only the heading "Root commit". This demo contains the following submodules:

| Submodule | Used by this demo |
|-----------|-------------------|
| HW        | Yes |
| OS        | No |
| SW        | No |

This demo was moved into this repository during 2020.1 updates. Its history prior to these updates can be found in its old repository, linked below:
* https://github.com/Digilent/Basys-3-GPIO

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Basys 3
* Vivado 2022.1 Installation
* MicroUSB Cable
* Serial Terminal Emulator
* VGA Monitor
* VGA Cable
* USB Mouse