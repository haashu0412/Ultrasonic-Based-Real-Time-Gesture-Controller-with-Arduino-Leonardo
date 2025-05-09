# Ultrasonic-Based Real-Time Gesture Controller with Arduino Leonardo

A lightweight, real-time gesture controller built using Arduino Leonardo and ultrasonic sensors. This project allows for hands-free device interaction through swipe and tap gestures, offering a plug-and-play HID interface.

---

## Overview

This system enables gesture-based human-computer interaction without the need for cameras or expensive equipment. Using HC-SR04 ultrasonic sensors, it accurately detects hand positions and maps them to HID-compatible inputs (e.g., keyboard/mouse commands).

---

## Key Features

- **Real-time Response**: Sub-100ms latency from gesture to action
- **High Accuracy**: >90% recognition accuracy under controlled conditions
- **Multi-Gesture Recognition**: Supports 4+ gesture types (e.g., left/right swipe, push, hover tap)
- **Plug-and-Play**: USB HID device—no drivers required
- **Affordable**: Built with low-cost open-source components

---

## Hardware Components

- Arduino Leonardo (ATmega32u4 with built-in USB HID support)
- 2x HC-SR04 Ultrasonic Sensors
- Jumper wires and breadboard
- USB cable (for power and data)

---

## How It Works

1. Two ultrasonic sensors measure the distance of a user's hand from fixed points.
2. A gesture recognition algorithm processes these distances.
3. Each gesture (e.g., swipe, push) is mapped to a specific HID command (e.g., arrow keys).
4. Commands are transmitted over USB to control devices.

---

## Setup Instructions

1. **Wiring**
   - Left Sensor: TRIG -> D9, ECHO -> D10
   - Right Sensor: TRIG -> D12, ECHO -> D11
   - VCC -> 5V, GND -> GND

2. **Programming**
   - Use Arduino IDE
   - Include `Keyboard.h` for HID functions
   - Upload sketch via USB

3. **Calibration**
   - Tune distance thresholds (e.g., 10–15cm = Tap, 20–25cm = Swipe)
   - Use serial monitor to test distance outputs

---

## Use Cases

- Contactless PC control for accessibility
- Interactive kiosks or public displays
- Prototyping for smart home and IoT interfaces

---

## Performance Metrics

| Metric                    | Value                  |
|--------------------------|------------------------|
| Gesture Recognition Rate | 90%+                   |
| Response Time            | < 100ms                |
| Power Consumption        | < 500mA via USB        |
| Distance Accuracy        | ±1 cm                  |

---

## References

- [Arduino Leonardo Overview](https://www.arduino.cc/en/Main/ArduinoBoardLeonardo)
- [HC-SR04 Datasheet](https://components101.com/sensors/hc-sr04-ultrasonic-sensor)
- [Arduino Keyboard Library](https://www.arduino.cc/reference/en/language/functions/usb/keyboard/)

---

## Architecture 
- Component Architecture
  ![image](https://github.com/user-attachments/assets/f55b8de8-e3f1-49b5-b383-e29b4ec36495)
  ![image](https://github.com/user-attachments/assets/8a1e95fe-e10e-421b-9b40-bb3b7741e497)
   ![image](https://github.com/user-attachments/assets/c676ab2d-289f-41f5-a3ac-4811931e6a02)
  ![image](https://github.com/user-attachments/assets/0feffcff-165d-42cb-b555-01f1717973b0)
  ![image](https://github.com/user-attachments/assets/86c601f0-c9ec-465f-b122-30116c7c4591)

## Implementation
- Adrino IDE
  ![image](https://github.com/user-attachments/assets/a22288ce-6485-4369-bca5-dec7a159ce9a)
  ![image](https://github.com/user-attachments/assets/afd42b33-f71c-458e-bfdb-3c68f407277c)

## Video Demo Link 

- link : https://drive.google.com/file/d/1aigNY-lnmNoe-cObmuhN2eWZIro9-9ED/view?usp=drive_link
