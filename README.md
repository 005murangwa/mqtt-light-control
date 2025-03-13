# Assignment 005: MQTT-Based Light Control

A web-based application to control a simulated IoT light via MQTT, featuring a simple HTML interface with 'Turn ON' and 'Turn OFF' buttons that publish to `/student_group/light_control`. Includes a Python script simulating an ESP8266, subscribing to the topic and printing the light's status using the `test.mosquitto.org` broker.

## Files
- **index.html**: A minimal webpage with "Turn ON" and "Turn OFF" buttons, using MQTT.js to send "ON" or "OFF" messages to `/student_group/light_control` via WebSockets.
- **light_simulation.py**: A Python script acting as an ESP8266 IoT device, subscribing to `/student_group/light_control` and printing "💡 Light is TURNED ON" or "💡 Light is TURNED OFF" based on messages.
- **README.md**: You're reading it!

## Features
- Real-time light control simulation over MQTT.
- Uses a public broker (`test.mosquitto.org`)—no local server setup needed!
- Lightweight and easy to test with just a browser and Python.

## How to Clone and Run
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/005murangwa/mqtt-light-control.git
   cd mqtt-light-control
