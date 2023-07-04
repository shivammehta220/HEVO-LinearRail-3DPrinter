# HEVO 3D-Printer with Linear Rails
## About This Project
This project is an adaptation and build of the HyperCube Evolution (HEVO) project by SCOTT_3D. The goal was to build a modified version of the HEVO printer with increased height for a larger build volume in the Z-axis, as well as incorporating a compartment for housing the electronics at the lower section. Additionally the kinematics of the printer where upgraded from the orginal linear rods to MGN Linear rails. In the repository, the CAD files, STLs used, BOMs and Marlin files can be found.     

## Electronics
The electronics used in this project differ from the original design and are in the compartment at the lower section of the frame. For the mainboard, the BIGTREETECH SKR PRO V1.1 Control Board with TMC2209 drivers was chosen since it has alot of room for expandability and future upgrades. To board is running Marlin 2.0, and the fork can be found here. Paired with that 

- BIGTREETECH SKR PRO V1.1 Control Board with TMC2209 drivers
- BIGTREETECH TFT35 V3.0 LCD Touch Screen with WiFi Board
- Trianglelab BMG extruder + V6 Hotend
- 300x300 Magnetic Heated Bed
- BLTOUCH Auto Bed Leveling Sensor
- Nema17 Stepper Motors

## Frame
The frame for this printer was purchased and laser cut from MISUMI, with overall dimensions of 700x450x440mm. The frame is designed to provide stability and support for the printer components.

## Linear Rail Upgrade
To improve the printer's performance, the linear rod rails used in the original design were upgraded to linear rails. This upgrade was implemented using a project found at [https://www.thingiverse.com/thing:2839395]. Additionally, a custom bracket was designed to mount the Trianglelab BMG extruder + V6 Hotend. The CAD files for these upgrades are available in the repository.

## Quality of Life Upgrades
Several quality of life upgrades were implemented to enhance the overall usability of the printer. These include:

- OctoPrint: A web interface for controlling and monitoring the printer remotely.
- Filament stand: A stand or holder for storing filament spools near the printer.
- Filament runout sensor: A sensor that detects when the filament runs out during a print.
- RepRap display: A display unit for providing real-time information about the printer's status.
- TFT screen: A touch screen interface for easy control and navigation of printer settings.

## Repository Structure
The repository is organized into the following folders:

- CAD Files: Contains the CAD files for the printer components, including the frame, linear rail upgrades, and extruder bracket.
- STLs: Contains the STL files ready for 3D printing.
- Marlin File: Contains the Marlin firmware configuration file specific to the printer.
- BOMs: Contains the Bill of Materials, listing all the necessary components for building the printer.
- Images: Contains images showcasing the printer, its components, and upgrades.

Please refer to the respective folders for specific files and documentation related to each section of the project.

## Acknowledgements
This project is based on and adapted from the HyperCube Evolution project by SCOTT_3D. We would like to express our gratitude to SCOTT_3D for providing the inspiration and foundation for this project.

## License
The design files and documentation in this repository are licensed under [INSERT LICENSE HERE]. Please review the license file for more information.

Feel free to explore the repository and make use of the resources provided to build and customize your own version of the printer. If you have any questions or suggestions, please don't hesitate to reach out. Happy printing!
