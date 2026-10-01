# 🔌 Circuit Diagram

This folder contains the wiring diagram for the Arduino Obstacle Avoiding Robot Car.

## Components

- Arduino Uno
- HC-SR04 Ultrasonic Sensor
- L298N Motor Driver
- 4 DC Motors
- Battery Pack (7V–12V)

## Circuit Diagram

![Circuit Diagram](circuit_diagram.png)

## Notes

- Use a common GND between the Arduino, L298N motor driver, and battery.
- Connect the HC-SR04 Trigger pin to Arduino D12.
- Connect the HC-SR04 Echo pin to Arduino D13.
- Supply the motors using an external battery pack (7V–12V).
- Do not power the motors directly from the Arduino.

An autonomous robot car that detects nearby obstacles and changes direction using an Arduino Uno, an HC-SR04 ultrasonic sensor, and an L298N motor driver.
The car moves forward while measuring the distance to obstacles. When an obstacle is detected within the configured threshold of 50 cm, it stops, tries turning right, and checks the path again. If the path remains blocked, it turns left before continuing.
📑 Table of Contents
- Features
- Components
- Software
- How It Works
- Pin Connections
- Circuit Diagram
- Project Structure
- Future Improvements
- Author
✨ Features
- Autonomous obstacle detection and avoidance
- Real-time distance measurement with the HC-SR04
- Automatic right- and left-turn behavior
- PWM-based motor speed control
- Four-wheel mobile platform
- Arduino programming in Embedded C
🛠 Components
Component	Quantity
Arduino Uno	1
HC-SR04 ultrasonic sensor	1
L298N motor driver	1
DC motors	4
Wheels	4
Robot chassis	1
Battery pack	1
Jumper wires	As needed


💻 Software
- Arduino IDE
- Arduino programming language (Embedded C/C++)
⚙️ How It Works
1. The car drives forward.
2. The HC-SR04 measures the distance to nearby objects.
3. If an object is detected within 50 cm, the car stops and turns right.
4. It checks the path again. If it remains blocked, the car turns left.
5. The car resumes forward movement and repeats the process.
🔌 Pin Connections
Arduino pin	Connection
D8–D11	Motor driver inputs
D2–D3	Motor driver inputs
D4–D5	Motor driver inputs
A5, A4, A1, A2	Motor driver enable pins
D12	HC-SR04 Trigger
D13	HC-SR04 Echo


Confirm the motor-driver input labels and wiring against your circuit. The original pin list labels these as IN1–IN8 and ENA/ENB front/back, which may not match a typical L298N module.

🔌 Circuit Diagram
The diagram shows the connections between the Arduino Uno, ultrasonic sensor, motor driver, battery, and motors.
📁 Project Structure
Arduino-Obstacle-Avoiding-Robot-Car/
├── Arduino_Code/
├── Circuit/
│   ├── circuit_diagram.png
│   └── README.md
├── Images/
├── Videos/
├── LICENSE
└── README.md
🚀 Future Improvements
- Mount the ultrasonic sensor on a servo for wider scanning
- Add Bluetooth control
- Build a mobile-app interface
- Add ESP32-based Wi-Fi control
- Integrate a camera for visual navigation
👩‍💻 Author
Vani Jain
