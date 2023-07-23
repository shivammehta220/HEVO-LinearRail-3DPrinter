# HEVO 3D-Printer with Linear Rails
![Main](/assets/images/Main.png)
## About This Project
This project is an adaptation and build of the HyperCube Evolution (HEVO) project by SCOTT_3D. The objective was to construct a modified version of the HEVO printer with an increased height to achieve a larger build volume in the Z-axis. Additionally, the project aimed to incorporate a compartment for electronics and upgrade the original linear rods to MGN Linear rails.

The repository contains CAD files, documentation, STLs, BOMs, and Marlin files related to this project.    

## [Electronics](/Electronics/README.md)
The electronics used in this project differ from the original design. They are all securely mounted using standoffs in the lower compartment of the frame. For the mainboard, the BIGTREETECH SKR PRO V1.1 Control Board with TMC2209 drivers was selected due to its ample room for expandability and future upgrades. The board is running Marlin 2.0, and the customized fork can be [found here](https://github.com/shivammehta220/Marlin/tree/HEVO).

![Compartment](/assets/images/Compartment.png)

## [Frame](/Design/README.md)
The printer's frame was purchased and laser-cut from MISUMI, with overall dimensions of 440x450x700 mm. The frame is designed to provide stability and support for the printer components. The original build volume of SCOTT_3D's design is 300x300x300 mm, but it has been upgraded to 300x300x450 mm, with an additional 200 mm of extrusion in the lower section for housing the electronics. All printed components are made using PETG filament. The STLs and CAD files for all the components used, as well as the Hypercube configurator for the build layout, can be found in the Design folder of this repository.

## [Linear Rail Upgrade](/Design/README.md)
To enhance the printer's performance, the linear rod rails used in the original design were replaced with linear rails. This upgrade was implemented using a project found at [https://www.thingiverse.com/thing:2839395]. Additionally, a custom bracket was designed to mount the Trianglelab BMG extruder + V6 Hotend. The CAD files for these upgrades are available in the Design folder of this repository.

![Extruder](/assets/images/CAD/Extruder.png)

## [Octoprint](/Octoprint/README.md)
OctoPrint, a web interface for controlling and monitoring the printer remotely, is hosted on a Raspberry Pi 4. To complement the web interface, a 7-inch touch screen LCD is paired with the Pi to access the files. All plugins and settings for OctoPrint can be found in the OctoPrint folder of this repository, along with their corresponding links and documentations.

![Dashboard1](/assets/images/Octoprint/Dashboard1.png)

## Acknowledgements
This project is based on and adapted from the HyperCube Evolution project by SCOTT_3D. I would like to express my gratitude to SCOTT_3D for providing the inspiration and foundation for this project, as well as all the remixes that contributed to making it possible.

## License
The design files and documentation in this repository are licensed under MIT LICENSE. Please review the license file for more information.

Feel free to explore the repository and utilize the resources provided to build and customize your own version of the printer. If you have any questions or suggestions, please don't hesitate to reach out. Happy printing!
