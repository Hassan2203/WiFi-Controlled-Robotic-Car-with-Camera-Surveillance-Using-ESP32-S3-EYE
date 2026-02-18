📌 Project Overview

This project presents a WiFi-controlled robotic car with real-time camera streaming using the ESP32-S3-EYE development board.
The system integrates motor control, wireless communication, and live video streaming into a single embedded IoT platform.

The robot connects to a WiFi network and is controlled via a web-based interface.

🎯 Objectives

Design a WiFi-controlled robotic platform

Implement real-time camera streaming

Enable four-direction motor control

Develop a web-based control interface

Integrate LED lighting control

🛠 Hardware Components
Component	Description
ESP32-S3-EYE	Microcontroller with camera
OV2640 Camera	2MP camera sensor
Motor Driver (L298N)	Controls DC motors
DC Motors	Movement control
Chassis	Robot body
External Battery	Motor power
USB Power	Board power
🔌 Pin Configuration
Camera Pins (Important – Do Not Modify)

(List camera GPIO table here)

Motor Control Pins
Function	GPIO
Left Forward	GPIO 2
Left Backward	GPIO 1
Right Forward	GPIO 41
Right Backward	GPIO 42
LED	GPIO 21
🏗 System Architecture

The system consists of:

Hardware Layer – ESP32 board, motors, power supply

Firmware Layer – Arduino-based program

Communication Layer – WiFi & Web Server

💻 Software Requirements

Arduino IDE

ESP32 Board Package

WiFi Library

ESP32 Camera Library


🚀 Installation & Setup
1) Open in Arduino IDE

Select Board: ESP32-S3-EYE

Select correct COM Port

2) Update WiFi Credentials
const char* ssid = "Your_WiFi_Name";
const char* password = "Your_Password";

3) Upload Code

After upload:

Open Serial Monitor

Copy IP address

Open in browser

📷 Working Demonstration

Add:

Project Images

Circuit Diagram

Screenshot of Web Interface

Short demo video (optional)

📊 Results

WiFi Connection Time: 2–5 sec

Streaming Resolution: 640x480

Frame Rate: 15–20 fps

Latency: 200–500 ms

Motor Response Time: <100 ms

⚠ Challenges Faced
1️⃣ Camera Pin Conflicts

Solved by reviewing ESP32-S3-EYE datasheet and reassigning motor pins.

2️⃣ Power Stability

Used separate power supplies for motors and board.

3️⃣ Video Latency

Reduced resolution and optimized JPEG quality.

🔮 Future Improvements

Add PWM speed control

Add ultrasonic obstacle detection

Add autonomous mode

Add mobile app control

Add secure authentication
