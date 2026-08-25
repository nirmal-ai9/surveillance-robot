Hardware Requirements

The following hardware components are required to construct the autonomous surveillance robot:

Power System

- 4 × AA Battery Holder — auxiliary power source
- 2S 5A BMS — battery protection and management for the sensor/control power system
- 2S 10A BMS — battery protection and management for the motor power system
- LM2596 Buck Converter — regulated voltage conversion for low-voltage electronics
- Battery 1: 4 × lithium-ion cells arranged in a 2S2P configuration
- Battery 2: 2 × lithium-ion cells arranged in a 2S configuration

Control & Processing

- ESP32-S3-CAM — primary microcontroller and camera module
- PCA9685 16-Channel PWM Driver — servo control and PWM signal management

Motor & Motion Control

- 2 × L298N Motor Driver Modules — control of the six-wheel drive motors
- 3 × Servo Motors
  - 2 servos for the camera's pan-and-tilt mechanism
  - 1 servo for an additional mechanism, if required

Sensors

- 2 × HC-SR04 Ultrasonic Sensors — obstacle and distance detection

Wiring & Connectivity

- Connecting wires
- Jumper wires
- Header pins
- Required connectors and miscellaneous wiring accessories

«Note: The final power distribution and voltage requirements should be verified before assembly to ensure that the batteries, BMS units, buck converter, motor drivers, ESP32-S3-CAM, sensors, and servos operate within their specified electrical limits.»
