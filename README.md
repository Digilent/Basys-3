# Basys 3 Root Repository

## Basys 3 XADC Demo

### Description

This branch contains sources for the Basys 3 XADC Demo.

This project is a Vivado demo using the Basys 3's analog-to-digital converter ciruitry, switches, LEDs, and seven-segment display, written in Verilog. When programmed onto the board, voltage levels between 0 and 1 Volt are read off of the JXADC header. The 16 User LEDs increment from right to left as the voltage difference between the selected channel's pins gets larger. The seven-segment display shows the voltage difference between the selected channel's pins in volts. SW0 and SW1 select which XADC channel is displayed, as shown in the table below. 

| XADC Channel | JXADC Pins             | SW0 Position | SW1 Position |
| ------------ | ---------------------- | ------------ | ------------ |
| AD6          | JXADC1(P) / JXADC7(N)  | Down         | Down         |
| AD14         | JXADC2(P) / JXADC8(N)  | Up           | Down         |
| AD7          | JXADC3(P) / JXADC9(N)  | Down         | Up           |
| AD15         | JXADC4(P) / JXADC10(N) | Up           | Up           |

For more information on the Basys 3 XADC Demo, including setup instructions, visit its [Demo Page](https://reference.digilentinc.com/reference/programmable-logic/basys-3/demos/xadc) on the Digilent Wiki.

For more information on the Basys 3, including other demos that may be available, see its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/basys-3/start) on the Digilent Wiki.

### Git Navigation Information

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked above.

To see other demos in this repository, see the master branch's [README](https://github.com/Digilent/Basys-3).

Some demos do not require some submodules, in these cases, they are still provided to ease switching between demos in git. When unused, the submodule folder is largely empty, except for a readme containing only the heading "Root commit". This demo contains the following submodules:

| Submodule | Used by this demo |
|-----------|-------------------|
| HW        | Yes |

This demo was moved into this repository during 2020.1 updates. Its history prior to these updates can be found in its old repository, linked below:
* https://github.com/Digilent/Basys-3-XADC

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Basys 3
* Vivado 2020.1 Installation
* MicroUSB Cable
* Wires and a circuit to measure