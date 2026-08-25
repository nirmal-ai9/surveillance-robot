Autonomous Surveillance and Tracking Robot Car

This project is a six-wheel autonomous surveillance robot designed around an ESP32-CAM. The robot provides both manual remote control and autonomous person-tracking capabilities through a web-based interface.

System Overview

The robot uses an ESP32-CAM as its primary controller and camera module. It creates its own Wi-Fi network and hosts a web server, allowing a mobile device to connect directly to the robot without requiring an external router or internet connection.

Once connected, the mobile device can access a web-based control interface hosted by the robot. Through this interface, the user can:

- Control the robot's movement.
- View the live camera feed.
- Control the camera's position.
- Switch between manual and autonomous operating modes.

Autonomous Person-Tracking Mode

In autonomous mode, the camera system is designed to detect a person within its field of view and track their movement.

The robot can automatically adjust its movement to follow the detected person while continuously updating the camera's orientation. This allows the robot to maintain visual tracking without requiring constant manual control.

Pan-and-Tilt Camera System

The ESP32-CAM is mounted on a two-axis servo mechanism.

The two servo motors provide:

- Horizontal movement (pan) — rotates the camera from side to side.
- Vertical movement (tilt) — moves the camera up and down.

This gives the camera a wider observation range and allows it to track subjects more effectively.

Collision Avoidance and Safety

The robot will also incorporate distance or obstacle-detection sensors to help prevent collisions.

The sensors continuously monitor the area around the vehicle. When an obstacle is detected within a predefined distance, the robot can take appropriate action, such as stopping or changing direction.

This system is intended to improve the robot's reliability during autonomous operation.

Mechanical Platform

The robot is built on a six-wheel vehicle platform, providing improved stability and traction compared with a conventional two- or four-wheel configuration.

The six-wheel chassis will serve as the base for:

- ESP32-CAM
- Pan-and-tilt camera mechanism
- Drive motors
- Motor driver
- Obstacle-detection sensors
- Battery and power-management components
- Control electronics

Know more about required-hardware.md

Operating Modes

The robot is planned to support two primary operating modes:

1. Manual Mode

The user controls the robot remotely through the web interface. The live camera feed provides visual feedback while the user operates the vehicle.

2. Autonomous Tracking Mode

The robot uses its camera and detection system to identify and track a person. The movement of the robot and camera can be adjusted automatically based on the detected person's position.

Project Goal

The primary goal of this project is to create a compact, Wi-Fi-enabled robotic platform that combines remote control, live video streaming, pan-and-tilt camera control, obstacle avoidance, and autonomous person tracking into a single system.

The complete hardware configuration, wiring, component requirements, software setup, and assembly procedure are documented separately in the accompanying Excel setup guide.
