# OLed-PCB-control

OLed-PCB-control is a custom PCB project for controlling an SSD1306 OLED display using an Arduino Nano and 3 user buttons, including an on/off latch power circuit. The project provides all necessary KiCad design files and manufacturing outputs for easy assembly and use.

## Features

- SSD1306 OLED screen interface (I2C)
- 3 user input buttons
- On/off latch power circuit for energy efficiency
- Designed for Arduino Nano integration
- Easy-to-manufacture PCB (tested with JLCPCB)
- Includes schematic, PCB layout,  manufacturing outputs (Gerbers, BOM), and component list such as the custom and assigned footrprints

## Example Applications

- Menu navigation for embedded devices
- Educational electronics projects
- Portable or battery-powered interfaces


## Hardware Details

- **SSD1306 OLED Display:**
  - Standard 128x64 pixel OLED panel.
  - I2C interface for easy microcontroller communication.
  - 4-pin header (VCC, GND, SCL, SDA) for simple connection to the PCB.
  - Powered directly from the board’s regulated supply.
  - Compatible with most Arduino SSD1306 libraries.

- **PMOS Power Switch:**
  - Power latch circuit uses a PMOS transistor for efficient on/off control of the board and display.
  - Allows the user to toggle power using a push-button.
  - Reduces power consumption by fully disconnecting supply when off.
  - PMOS footprint provided in the PCB design for easy assembly.
  - Typical part: SI2333DS or equivalent SOT-23 PMOS (refer to schematic/BOM for exact part).

- **NPN Transistor Footprint:**
  - Custom through-hole footprint for robust switching and control applications.
  - Used within the latch circuit for reliable logic-level operation.

- **Standard Connectors:**
  - Easy-to-source headers for Arduino Nano and OLED display.
  - All signal and power lines clearly labeled in silkscreen.


## Credits

Created by [Shelleynguy](https://github.com/Shelleynguy)  
PCB manufactured with [JLCPCB](https://jlcpcb.com)

Feel free to customize this draft further with details specific to your project.
