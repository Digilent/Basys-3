# Basys 3 Root Repository

## Basys 3 Abacus Demo

### Description

This branch contains sources for the Basys 3 Abacus Demo.

This project is a Vivado demo using the Basys 3's switches, LEDs, pushbuttons, and seven-segment display, written in Verilog. When programmed onto the board, the Abacus demo can perform one of four arithmetic functions on two 8-bit numbers. Switches 15-8 represent input A and switches 7-0 represent input B.  

The pushbuttons select between subtraction, multiplication, division, and modulo operations as shown in the table below. The result of the selected operation is displayed on the seven-segment display. Once the operation button is released, the result of the operation scrolls across the seven segment display.
 
| Button | Function               |
| ------ | ---------------------- |
| BTNU   | Subtraction (A-B)      |
| BTND   | Multiplication (A\*B)  |
| BTNR   | Division (A/B)         |
| BTNL   | Modulo/Remainder (A%B) |

For more information on the Basys 3 Abacus Demo, including setup instructions, visit its [Demo Page](https://reference.digilentinc.com/reference/programmable-logic/basys-3/demos/abacus) on the Digilent Wiki.

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
* https://github.com/Digilent/Basys-3-Abacus

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Basys 3
* Vivado 2021.1 Installation
* MicroUSB Cable