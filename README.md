# Arduino Nano AC Switch & Home Automation Node

A compact, modular PCB designed for controlling AC appliances using an Arduino Nano. This project integrates sensor inputs (IR/Proximity) with a relay driver stage to create a standalone home automation unit.

## 🚀 Project Overview
This board simplifies the wiring mess of breadboard prototypes by consolidating the power supply, microcontroller, and switching logic into a single, robust PCB. It is designed to switch mains voltage loads safely based on sensor triggers.

### 🛠 Key Technical Features
* **Microcontroller:** Socket for **Arduino Nano (ATmega328P)**.
* **Power Stage:** * Accepts **12V DC Input**.
    * Onboard **5V Regulator** (LM7805 or AMS1117) to power the Nano and sensors.
* **Switching Logic:** * Dedicated **Relay Header** with transistor driver circuit.
    * Flyback diode protection for inductive loads.
* **Sensor Interface:** * 3-pin Header for **IR / Proximity Sensors** (VCC, GND, Signal).
* **User Interface:** * Power Indication LED.
    * Status LED (connected to a GPIO for debugging).

## 📂 Repository Structure
* `/Schematics`: Circuit diagrams and PDF exports.
* `/PCB_Design`: EasyEDA source files and Gerber manufacturing data.
* `/Code`: Arduino sketch (`.ino`) for basic IR switching logic.
* `/Images`: Photos of the assembled board.

## 🔌 How It Works
1.  **Input:** The IR sensor detects a signal (e.g., a hand wave or remote button press).
2.  **Processing:** The Arduino Nano reads the signal and debounces the input.
3.  **Output:** The Nano triggers the relay driver transistor, switching the AC load ON/OFF.
4.  **Power:** The board takes 12V from a standard adapter and regulates it down for the logic components.

## 📸 Visuals
![Board Top View](path-to-your-image.png)
*(Replace this text with the path to your actual image, e.g., `images/board_render.png`)*

## 🔮 Future Improvements
* Adding an ESP8266 header for Wi-Fi control.
* Implementing zero-crossing detection for smoother AC switching.

---
**Author:** [Your Name]  
**Role:** 2nd Year ECE Student @ SGBAU  
**Tools Used:** EasyEDA, Arduino IDE

