# Lancer Lumineers MATE ROV Competition Pioneer/Explorer 2023-24

# ROV Hydra Control System 

## Overview
This repository contains the code for a Remotely Operated Vehicle (ROV) control system, utilizing Pygame for the graphical user interface (GUI) and serial communication for hardware interaction. The project is designed to control an ROV through a user-friendly interface, allowing for joystick-based navigation, real-time video feedback, and customizable control widgets.

# Files Description
- `joystickX_test.py`: Script for testing joystick functionality and input handling.
- `main.py`: The main control script integrating joystick input, GUI updates, and hardware control commands.
- `widgets2.py`: Defines custom Pygame widgets for the GUI, including toggles, displays, and sliders.
- `rover-arduino.ino`: Arduino sketch for receiving control signals and managing hardware components like servos and sensors.

# Key Features:
- Pygame GUI: A custom GUI setup that includes a main view area and a sidebar for additional controls and information.
- Joystick Control: Interprets joystick inputs for ROV movement, using mathematical calculations to translate joystick position into commands.
- Serial Communication: Sends commands to the ROV's Arduino controller, allowing for real-time control of the vehicle.
- Live video capture: Three onboard cameras, one main which appears on the pygame and two external auxillary cameras ran by [OBSstudio](https://obsproject.com/download)
- Image Capture: Utilizes Pygame's camera module for capturing images, which can be used for navigation or documentation. (Needs to be configured)
## Future Plans:
- 3D Photogrammetry: With hardware and software upgrades, the ROV can perform 3D photogrammetry underwater. 
- Autonomous movement: With hardware and software upgrades, the ROV can perform autopathing or predefined pathing underwater.
---

# Getting Started
To run the ROV control system, ensure you have Python installed along with the Pygame library and the PySerial module for serial communication. Clone this repository, and run ROV_final.py to start the control interface.

---

# Prerequisites
- Python 3.x
- Pygame library
- PySerial library
  
- Arduino IDE
- "ArduinoJson" by Benoit library
- "Servo" by Michael Margolis library

---
# Installation

## Arduino Installation
1. Get [Arduino Uno IDE](https://www.arduino.cc/en/software)
2. Install ArduinoJson and Servo libraries in IDE
## Python Installation
(Important Note: YOU NEED WINDOWS FOR THIS PROJECT, IT DOESN'T SUPPORT MAC)
1. Here is the [link](https://www.geeksforgeeks.org/how-to-install-python-on-windows/) to install python on your Windows
2. Use any desired IDE, I recommend [VScode](https://code.visualstudio.com/download)
3. Get [pip](https://www.geeksforgeeks.org/how-to-install-pip-on-windows/)
4. After you get pip running, install pygame and pyserial using the following commands in cmd
```
pip install pygame
pip install pyserial
```

# Contributing
Contributions to the ROV control system are welcome. Please feel free to fork the repository, make changes, and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

# License
This project is licensed under the MIT License - see the LICENSE file for details.
Feel free to adjust the content to match your project's specifics or personal preferences better.
