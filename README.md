# 🏠 Smart Home Automation using ESP32

A simple IoT-based Smart Home Automation system developed using **ESP32, Wokwi Simulation, Sensors, and Firebase Realtime Database**.

The system detects human motion, monitors light intensity, and automatically controls a room light and fan. A push button is also used to control a buzzer. Sensor and device status are transmitted to Firebase and displayed on a real-time web dashboard.

---

## 📌 Project Overview

This project demonstrates how an ESP32 can be used to build a basic smart home system.

The ESP32 collects data from sensors and makes simple automation decisions:

- Detects motion using a PIR sensor.
- Measures light intensity using an LDR.
- Automatically turns ON the light when motion is detected in a dark environment.
- Turns ON the fan when motion is detected.
- Controls a buzzer using a push button.
- Sends sensor and device status to Firebase Realtime Database.
- Displays live data through a web dashboard.

The complete system is simulated using **Wokwi**, so physical hardware is not required for the prototype.

---

## 🎯 Objectives

- Build a simple IoT-based home automation system.
- Learn ESP32 GPIO and sensor interfacing.
- Implement automatic device control.
- Send real-time sensor data to Firebase.
- Create a web-based monitoring dashboard.
- Demonstrate an IoT workflow using simulation.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| ESP32 | Main microcontroller |
| Wokwi | Circuit simulation |
| Arduino C/C++ | ESP32 programming |
| PIR Sensor | Motion detection |
| LDR | Light intensity measurement |
| Push Button | Buzzer control |
| LED | Light and fan simulation |
| Buzzer | Alert/output |
| Firebase Realtime Database | Cloud data storage |
| HTML/CSS/JavaScript | Web dashboard |
| Firebase Hosting | Dashboard deployment |

---

## 🔌 Hardware / Simulation Components

- ESP32 DevKit V1
- PIR Motion Sensor
- LDR / Photoresistor
- Push Button
- 2 × LEDs
- 2 × 220Ω Resistors
- Buzzer
- Jumper Wires
- Power and Ground connections

---

## 📐 Pin Configuration

| Component | ESP32 Pin |
|---|---:|
| PIR OUT | GPIO 27 |
| LDR Analog Output | GPIO 34 |
| Push Button | GPIO 25 |
| Light LED | GPIO 26 |
| Fan LED | GPIO 14 |
| Buzzer | GPIO 33 |

---

## ⚙️ System Working

### 1. Motion Detection

The PIR sensor detects whether movement is present.

```text
Motion detected → ESP32 receives HIGH
No motion → ESP32 receives LOW
