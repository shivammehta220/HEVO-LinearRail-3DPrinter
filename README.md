# HEVO 3D-Printer with Linear Rails
![/images/main.png]
## About This Project
This project is an adaptation and build of the HyperCube Evolution (HEVO) project by SCOTT_3D. The goal was to build a modified version of the HEVO printer with increased height for a larger build volume in the Z-axis, as well as incorporating a compartment for housing the electronics at the lower section. Additionally the kinematics of the printer have been upgraded from the orginal linear rods to MGN Linear rails. In the repository, the CAD files, documentation, STLs, BOMs and Marlin files can be found.     

## Electronics
The electronics used in this project differ from the original design and are in the compartment at the lower section of the frame. For the mainboard, the BIGTREETECH SKR PRO V1.1 Control Board with TMC2209 drivers was chosen since it has alot of room for expandability and future upgrades. The board is running Marlin 2.0, and the fork can be [found here](https://github.com/shivammehta220/Marlin/tree/HEVO).

| Component  | Description | Link |
| ------------- | ------------- | ------------- |
| BIGTREETECH SKR PRO V1.1 Control Board  | Content Cell  | Link |
| Trianglelab BMG extruder  | Content Cell  | Link |
| Trianglelab V6 Hotend  | Content Cell  | Link |
| 300x300 Magnetic Heated Bed  | Content Cell  | Link |
| BLTOUCH Auto Bed Leveling Sensor | Content Cell  | Link |
| 2 × NEMA17 0.9 Degree Stepper Motor - 40mm  | Content Cell  | Link |
| BIGTREETECH Smart Filament Sensor Break Detection Module BTT SFS V1.0 Monitor | Content Cell  | Link |
| 2 × NEMA17 Stepper Motor With Attached Lead Screw- 40mm  | Content Cell  | Link |

## Frame
The frame for this printer was purchased and laser cut from MISUMI, with overall dimensions of 440x450x700(mm). The frame is designed to provide stability and support for the printer components. The orginal build volume of SCOTT_3D design is 300x300x300(mm), and has been upgraded to 300x300x450(mm), with additional 200mm of extrustion in the lower compartment for the electroincs using the HEVO excel configurator.

| Extrution (mm) | Type | Quantity |
| ------------- | ------------- | ------------- |
| 420 | 3030 Black Alu profiles | 6 |
| 410 | 3030 Black Alu profiles | 8 |
| 700 | 3030 Black Alu profiles | 4 |
| 415 | 2020 Black Alu profiles | 2 |
| 235 | 2020 Black Alu profiles | 2 |

## Linear Rail Upgrade
To improve the printer's performance, the linear rod rails used in the original design were upgraded to linear rails. This upgrade was implemented using a project found at [https://www.thingiverse.com/thing:2839395]. Additionally, a custom bracket was designed to mount the Trianglelab BMG extruder + V6 Hotend. The CAD files for these upgrades are available in the repository.

## Octoprint
OctoPrint is a web interface for controlling and monitoring the printer remotely, and is hosted on a Raspberry Pi 4. To compliment the web interface, a 7-inch touch screen LCD is paired with the Pi to access the files using OctoDock. The following plugins are being used:

## Quality of Life Upgrades
Several quality of life upgrades were implemented to enhance the overall usability of the printer. These include:

- OctoPrint: A web interface for controlling and monitoring the printer remotely.
- Filament stand: A stand or holder for storing filament spools near the printer.
- Filament runout sensor: A sensor that detects when the filament runs out during a print.
- RepRap display: A display unit for providing real-time information about the printer's status.
- TFT screen: A touch screen interface for easy control and navigation of printer settings.

## Acknowledgements
This project is based on and adapted from the HyperCube Evolution project by SCOTT_3D. We would like to express our gratitude to SCOTT_3D for providing the inspiration and foundation for this project.

## License
The design files and documentation in this repository are licensed under [INSERT LICENSE HERE]. Please review the license file for more information.

Feel free to explore the repository and make use of the resources provided to build and customize your own version of the printer. If you have any questions or suggestions, please don't hesitate to reach out. Happy printing!
