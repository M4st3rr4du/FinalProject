FinalProject
Simple Games on ATmega328P
Introduction
What it does: This project implements a set of simple games (e.g., Snake, Blocks) on an ATmega328P microcontroller, using an LED matrix and an LCD screen for display.
Purpose: To provide an interactive and educational platform for demonstrating basic game development on embedded systems.
Idea behind it: Combining creativity and technology to build retro-style games on a low-power microcontroller.
Why it’s useful: It showcases fundamental principles of game logic and embedded programming in a fun and engaging way.
General Description
Block diagram of the project:

ATmega328P - Central processing unit handling game logic and user input.
LED Matrix - Displays game visuals, such as Snake's movement or falling blocks.
LCD Screen - Displays scores, game options, and messages.
Buttons:
Direction buttons for game control.
Start/Select button to navigate menus or restart games.
Hardware Design
List of Components
ATmega328P microcontroller
LED matrix module (e.g., 8x8)
16x2 LCD with I2C adapter
Buttons (5-6 for navigation and control)
Resistors, jumper wires, breadboard/PCB
Electrical Schematics
Include:

Connections between ATmega328P, LED matrix, LCD, and buttons.
Proper pull-up resistors for buttons and connections for I2C communication with the LCD.
![Electrical Schematic](images/schemelectric.png)

Software Design
Development Environment: PlatformIO
Libraries used:
Adafruit_GFX for LED matrix graphics
Adafruit_LED_Backpack for LED matrix control
LiquidCrystal_I2C.h for LCD interaction
Implemented Games and Features
Snake:
The player controls a growing snake to collect food, avoiding walls and itself.
Blocks:
A Tetris-inspired game where the player arranges falling blocks to clear lines.
Functions Implemented
Game selection menu
Real-time game updates and rendering
Input handling for navigation and gameplay
Score tracking and display
Results
The system successfully runs both games:
Smooth and responsive gameplay.
Scores are displayed in real-time on the LCD.
The design demonstrates efficient use of microcontroller resources.
Conclusions
This project highlights how embedded systems can power interactive applications, showcasing both hardware design and software logic. It's an excellent example of retro gaming combined with modern microcontroller programming.

Source Code and Other Resources to Include on GitHub
Organize files as follows:
src/: Source code.
hardware/: Electrical schematics.
images/: Photos and diagrams (block diagram, electrical schematics).
README.md: This document.





