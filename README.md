# 328Games

## Simple Games on ATmega328P  

---

### 📘 Introduction  

- **What it does:** This project implements a collection of simple games, such as **Snake** and **Blocks**, on an **ATmega328P microcontroller**. It uses an LED matrix and an LCD screen to provide interactive gameplay.  
- **Purpose:** To create a retro-style gaming experience while demonstrating embedded systems programming.  
- **Idea behind it:** Showcasing the potential of low-power microcontrollers to handle creative and fun applications.  
- **Why it’s useful:** Combines educational value with entertainment, making it an engaging project for learning microcontroller programming.  

---

### 🛠️ General Description  

#### 🔧 Block Diagram  

- **ATmega328P**: Core processor handling game logic, rendering, and user inputs.  
- **LED Matrix**: Displays game visuals such as snake movement or falling blocks.  
- **LCD Screen**: Shows scores, instructions, and menu options.  
- **Buttons:**  
  - **Direction buttons**: Up, down, left, right.  
  - **Start/Select button**: Menu navigation and game restart.  

`![Block Diagram](images/block_diagram.png)`  

---

### 🖥️ Hardware Design  

#### 📋 List of Components  

- **ATmega328P microcontroller**  
- **LED matrix module** (e.g., 8x8 or 16x16)  
- **16x2 LCD with I2C adapter**  
- **Push-buttons** (5 or 6 for controls)  
- **Resistors** for pull-up circuits  
- **Jumper wires**  
- **Breadboard** or **custom PCB**  

#### ⚡ Electrical Schematics  

- Proper wiring between ATmega328P, the LED matrix, and LCD.  
- I2C connections for the LCD.  
- Pull-up resistors for push-buttons.  

`![Electrical Schematic](images/electrical_schematic.png)`  

---

### 🧑‍💻 Software Design  

#### 💻 Development Environment  
- **IDE:** PlatformIO with Arduino Framework.  
- **Programming Language:** C/C++  

#### 📚 Libraries Used  

- **`Adafruit_GFX`**: Graphics library for LED matrix visuals.  
- **`Adafruit_LED_Backpack`**: For controlling the LED matrix.  
- **`LiquidCrystal_I2C`**: Simplifies LCD integration.  

#### 🎮 Implemented Games  

- **Snake**:  
  - Navigate the snake to collect food.  
  - Avoid walls and self-collision to continue growing.  
- **Blocks**:  
  - Arrange falling blocks to clear rows.  
  - Increase difficulty with faster block drops.  

#### 🛠️ Functions Implemented  

- **Game Menu**: Allows the player to select a game.  
- **Rendering System**: Handles real-time updates to the LED matrix.  
- **Input Management**: Reads button presses and processes them into game actions.  
- **Score Display**: Shows the player’s score on the LCD.  

---

### 📊 Results  

- **Snake Game**:  
  - Smooth gameplay with responsive controls.  
  - Dynamic score updates displayed on the LCD.  
- **Blocks Game**:  
  - Blocks move fluidly with increasing speed.  
  - Rows clear and scores increment properly.  
- **System Performance**:  
  - Efficient resource utilization ensures minimal delays.  

---

### 🏁 Conclusions  

- This project successfully demonstrates the capabilities of the **ATmega328P** in handling interactive applications.  
- It provides a fun and educational way to explore microcontroller programming while showcasing efficient use of resources.  

---

### 📁 Repository Structure  

- **`src/`**: Source code for the project.  
- **`hardware/`**: Electrical schematics and PCB designs.  
- **`images/`**: Block diagrams, schematics, and project photos.  
- **README.md**: This document.  

---

### 📷 Visuals  

- Include photos or screenshots of:  
  - The final hardware setup.  
  - The LED matrix during gameplay.  
  - The LCD displaying scores or menus.  

---

### 🔗 Useful References  

- [ATmega328P Datasheet](https://ww1.microchip.com/downloads/en/DeviceDoc/ATmega328P-Complete.pdf)  
- [Adafruit GFX Library](https://github.com/adafruit/Adafruit-GFX-Library)  
