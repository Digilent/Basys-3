# Basys 3 Root Repository

This repository contains all demos for the Basys 3.

For more information about the Basys 3, visit its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/basys-3/start) on the Digilent Wiki.

Each demo contained in this repository is documented on the Digilent Wiki, links in the table below.

| Wiki Link | Demo Master Branch | Submodules Used |
|-----------|--------------------|-----------------|
| [Basys 3 Abacus Demo](https://reference.digilentinc.com/reference/programmable-logic/basys-3/demos/abacus) | Abacus/master | HW |
| [Basys 3 General I/O Demo](https://reference.digilentinc.com/reference/programmable-logic/basys-3/demos/gpio) | GPIO/master | HW |
| [Basys 3 Keyboard Demo](https://reference.digilentinc.com/reference/programmable-logic/basys-3/demos/keyboard) | Keyboard/master | HW |
| [Basys 3 XADC Analog to Digital Converter Demo](https://reference.digilentinc.com/reference/programmable-logic/basys-3/demos/xadc) | XADC/master | HW |

## Repository Description

This repository is designed to offer a unified and comprehensive approach to all of the aspects of the demos that we provide for the Basys 3, across multiple tools. By cloning this repo recursively you will receive the repositories for Vivado projects (HW), Vitis workspaces (SW), and Petalinux projects (OS). Each submodule may have its own submodule dependencies which will also be pulled when cloning. An important aspect of this structure is the fact that the SW and OS heavily depend on hardware hand-off files from the HW repository.

This repository also provides releases containing project and image files used by the various tools involved. Releases provide files that are directly usable, without requiring the use git or any scripting systems. Documentation of each demo, as well as instructions for using their releases, can be found by visiting the corresponding pages on the Digilent Wiki, links below. All releases in this repository can be found in this repository's [releases page](https://github.com/Digilent/Basys-3/releases), however, use of the wiki pages to find specific well-tested releases is advised.

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked in the table of demos, above.

Demos were moved into this repository during 2020.1 updates. History of these demos prior to these updates can be found in their old repositories, linked below:
* https://github.com/Digilent/Basys-3-Abacus
* https://github.com/Digilent/Basys-3-GPIO
* https://github.com/Digilent/Basys-3-Keyboard
* https://github.com/Digilent/Basys-3-XADC
