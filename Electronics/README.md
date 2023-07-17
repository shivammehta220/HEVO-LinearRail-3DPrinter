# Electronics
In this section, you can find the manuals and repositories related to the electronics used in the project. The complete list of electronics can be found in the BOM Excel sheet, but here are some of the main components:

| Component |
| ------------- |
| BIGTREETECH SKR PRO V1.1 Control Board  | 
| Trianglelab BMG extruder  | 
| Trianglelab V6 Hotend  | 
| 300x300 Magnetic Heated Bed  | 
| BLTOUCH Auto Bed Leveling Sensor | 
| 2 × NEMA17 0.9 Degree Stepper Motor - 40mm  | 
| BIGTREETECH Smart Filament Sensor Break Detection Module BTT SFS V1.0 Monitor | 
| 2 × NEMA17 Stepper Motor With Attached Lead Screw- 40mm  | 

## Electronics Compartment
The electronics compartment houses all the printer's electronics. It is enclosed with printed side panels and features cutouts for the power outlet, Ethernet, and both the RepRap display and the display for OctoPrint.

![/assets/images/Electronics/Power_outlet.png]
![/assets/images/Electronics/Displays.png]

## RGBW LED, 12V Regulator and Controller
To provide visualization of the print bed during prints and indicate the print status, RGBW LEDs are mounted on the 3030 extrusion frame. The LED strips themselves cannot be controlled by the SKR PRO V1.1 Control Board directly, so a basic MOSFET control circuit is used to turn the LEDs on and off. Additionally, since the power supply unit (PSU) operates at 24V, a 12V regulator is added to power the LEDs and other accessories (fans).

![/assets/images/Electronics/LEDS.png]
![/assets/images/Electronics/LEDS_Controller.png]

The LEDs are connected to unused pins on the SKR PRO V1.1 Control Board, and the corresponding lines in the Marlin firmware are enabled to support LED control.
```
/**
 * RGB LED / LED Strip Control
 *
 * Enable support for an RGB LED connected to 5V digital pins, or
 * an RGB Strip connected to MOSFETs controlled by digital pins.
 *
 * Adds the M150 command to set the LED (or LED strip) color.
 * If pins are PWM capable (e.g., 4, 5, 6, 11) then a range of
 * luminance values can be set from 0 to 255.
 * For NeoPixel LED an overall brightness parameter is also available.
 *
 * *** CAUTION ***
 *  LED Strips require a MOSFET Chip between PWM lines and LEDs,
 *  as the Arduino cannot handle the current the LEDs will require.
 *  Failure to follow this precaution can destroy your Arduino!
 *  NOTE: A separate 5V power supply is required! The NeoPixel LED needs
 *  more current than the Arduino 5V linear regulator can produce.
 * *** CAUTION ***
 *
 * LED Type. Enable only one of the following two options.
 */
//#define RGB_LED
#define RGBW_LED

#if EITHER(RGB_LED, RGBW_LED)
  #define RGB_LED_R_PIN PD0
  #define RGB_LED_G_PIN PD2
  #define RGB_LED_B_PIN PD5
  #define RGB_LED_W_PIN PE0
#endif
```
## Smart Filament Sensor
The BIGTREETECH Smart Filament Sensor is not your typical mechanical or optical sensor. It is capable of detecting filament movement, allowing it to prevent false positives in case of filament breakage.

![/assets/images/Electronics/Filament_Sensor.png]
