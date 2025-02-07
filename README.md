# Basys 3 Root Repository

## Basys 3 Stopwatch Demo

### Description

This branch contains sources for the Basys 3 Stopwatch Demo.

This project is a Vivado demo using the Basys 3's LEDs, pushbuttons, and seven-segment display, written in Verilog. When programmed onto the board, a user can press BTNR to start a timer. The seven segment display begins counting ten times a second and LEDs begin illuminating, right to left. BTNL is used to stop the timer - if the user times it right, and presses the stop button at the moment that all LEDs are illuminated, the LEDs will flash, and the seven segment counter will not be cleared, allowing the user to build up a high score. BTNC can be used to reset the state machine and counters that implement this functionality at any time.
 
| Button | Function               |
| ------ | ---------------------- |
| BTND   | Reset                  |
| BTNR   | Start the Timer        |
| BTNL   | Stop the Timer         |

For more information on the Basys 3 Stopwatch Demo, including setup instructions, visit its [Demo Page](https://digilent.com/reference/programmable-logic/basys-3/demos/stopwatch) on the Digilent Wiki.

For more information on the Basys 3, including other demos that may be available, see its [Resource Center](https://digilent.com/reference/programmable-logic/basys-3/start) on the Digilent Wiki.

### Git Navigation Information

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://digilent.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked above.

To see other demos in this repository, see the master branch's [README](https://github.com/Digilent/Basys-3).

Some demos do not require some submodules, in these cases, they are still provided to ease switching between demos in git. When unused, the submodule folder is largely empty, except for a readme containing only the heading "Root commit". This demo contains the following submodules:

| Submodule | Used by this demo |
|-----------|-------------------|
| HW        | Yes |
| OS        | No |
| SW        | No |

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Basys 3
* Vivado 2024.1 Installation
* MicroUSB Cable