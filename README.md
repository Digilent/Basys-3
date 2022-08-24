# Basys 3 Root Repository

## Basys 3 Keyboard Demo

### Description

This branch contains sources for the Basys 3 Keyboard Demo.

This project is a Vivado demo using the Basys 3's USB HID Host port and USB UART bridge, written in Verilog. When programmed onto the board, whenever the user presses a key on a keyboard connected to the USB HID port (J2, labeled "USB"), a scan code is sent to the Basys3 through a PS/2 interface. This scan code is read and transmitted to the computer via the USB-UART bridge. When the key is released, a scan code of 0xF0XX is transmitted, indicating that the key with PS/2 code "XX" has been released.

To use this demo, the Basys 3 must be connected to a serial terminal on the computer it is connected to over the MicroUSB cable.

For example: If the user presses the space bar on a keyboard connected to the Basys 3, the scan code "29" will be sent to the computer.  When the space bar is released, "F0 29" will be printed.

For more information on the Basys 3 Keyboard Demo, including setup instructions, visit its [Demo Page](https://reference.digilentinc.com/reference/programmable-logic/basys-3/demos/keyboard) on the Digilent Wiki.

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
* https://github.com/Digilent/Basys-3-Keyboard

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Basys 3
* Vivado 2022.1 Installation
* MicroUSB Cable
* Serial Terminal Emulator
* USB Keyboard