
# 🌞 Smart Solar Tracking and Irrigation System

This project integrates **solar tracking** and **automatic irrigation** using **Arduino Uno boards**.  
It optimizes solar panel positioning for maximum power generation while monitoring soil moisture levels  
to automate plant watering. The entire system can also be controlled manually using an **IR remote**.

---

## 🧠 Overview

The system combines several smart features:

- 🌤️ **Dual-axis solar tracking** using two servo motors and LDR (light-dependent resistors)
- 💧 **Automatic irrigation** controlled by soil moisture readings
- 🔋 **Solar-powered system** with battery charging and regulation
- 🎮 **IR remote manual control**
- 🧩 **Dual Arduino setup** — one for solar tracking, one for irrigation and control

---

## ⚙️ Components Used

| Component | Quantity | Description |
|------------|-----------|-------------|
| Arduino Uno | 2 | Main microcontrollers |
| Solar Panel | 1 | Provides renewable power |
| Battery Pack (AA 1.5V x3) | 1 | Power storage |
| LDR Sensors | 2 | Detect light intensity |
| Servo Motors | 2 | Control solar panel orientation |
| Soil Moisture Sensor | 1 | Detects soil dryness |
| IR Receiver + Remote | 1 | For remote control input |
| Breadboards | 2 | Circuit prototyping |
| Potentiometers | 2 | Calibration and tuning |
| Resistors & Jumper Wires | — | For circuit connections |

---

## 🔌 Circuit Description

- Solar Tracker Module (Arduino #1):  
  - Two LDRs sense sunlight intensity.  
  - Arduino adjusts servo motors to align the solar panel.  
  - Power from the solar panel is stored in rechargeable batteries.

- Irrigation Module (Arduino #2):
  - Reads soil moisture data.  
  - Activates a pump or relay when soil is dry.  
  - Receives IR remote input for manual override.

- Power Management: 
  - Solar panel charges the battery pack.  
  - Both Arduinos are powered from the regulated battery output.

---

## 🧩 Example Pin Connections

| Module | Arduino Pin | Description |
|---------|--------------|-------------|
| LDR 1 | A0 | Light sensor 1 |
| LDR 2 | A1 | Light sensor 2 |
| Servo X | D9 | Horizontal axis control |
| Servo Y | D10 | Vertical axis control |
| Soil Sensor | A2 | Soil moisture input |
| IR Receiver | D11 | Remote signal input |
| Pump/Relay | D12 | Water control output |

> ⚠️ *Pin assignments may vary depending on your circuit layout.*

---

## 💻 Software

The project includes two Arduino sketches:

1. `solar_tracker.ino` – Controls solar tracking and servos.  
2. `irrigation_system.ino` – Handles moisture sensing and irrigation logic.

---

## 🪛 How to Use

1. Upload `solar_tracker.ino` to Arduino #1.  
2. Upload `irrigation_system.ino` to Arduino #2.  
3. Connect all components as shown in the circuit diagram.  
4. Power the system via solar panel or batteries.  
5. Use the IR remote for manual control.  
6. Monitor LEDs or Serial output for feedback.

---

## 🌿 Features & Future Improvements

✅ Automatic dual-axis solar tracking  
✅ Smart irrigation system  
✅ Solar-powered and energy efficient  
✅ Manual remote control  

## 🔧 Future Improvements:
- IoT connectivity (Wi-Fi/Bluetooth)
- Real-time data display (LCD or web dashboard)
- Improved power management and efficiency

---
### 👨‍💻 Author
Developed as an Arduino-based automation and renewable energy project.  
Feel free to contribute improvements or additional features!

print("✅ README.md file created successfully!")
# Solar-Tracking-and-Cleaning-System
