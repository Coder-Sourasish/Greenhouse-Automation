🌱 Greenhouse Monitoring & Automation System

A Low-Cost Smart Agriculture Solution

📌 Overview

This project is a low-cost, Arduino-based Greenhouse Automation System designed to automatically maintain ideal conditions for plant growth. It monitors temperature, humidity, soil moisture, and light, and controls irrigation, heating, cooling, and lighting through a 4-channel relay module.

The goal is to create an affordable, sustainable, and accessible smart-farming solution for small and medium-scale farmers.

🚀 Features

🌡️ Automatic temperature control (heating & cooling)

💧 Smart irrigation using soil moisture sensor

☀️ Automatic grow light activation in low-light conditions

🔄 Real-time environmental monitoring

⚡ Low power consumption

🔧 Fully customizable thresholds

🌞 IoT + Solar + AI upgrade-ready

🛠️ Technologies Used

Programming: Arduino C/C++

Microcontroller: Arduino UNO

Components:

DHT11 Sensor (Temperature & Humidity)

Soil Moisture Sensor

LDR (Light Dependent Resistor)

4-Channel Relay Module

Water Pump

Cooling Fan

Heating Pad / Heater

LED Grow Light

Software: Arduino IDE

🔧 Hardware Connections
Component	Arduino Pin
DHT11 Sensor	7
Soil Moisture Sensor	A0
LDR	A1
Relay 1 (Water Pump)	2
Relay 2 (Heater)	3
Relay 3 (Cooling Fan)	4
Relay 4 (Grow Light)	5
Servo / Extra Output	10
🔄 Working Principle

The system works in a continuous loop:

Read input

Temperature

Humidity

Soil moisture

Light level

Process data
Arduino compares values with pre-set thresholds.

Trigger output

Moisture < 60% → Water Pump ON

Temp > 30°C → Cooling Fan ON

Temp < 20°C → Heater ON

Low Light → Grow Light ON

Maintain optimal conditions automatically

📊 Flowchart
[Sensors: DHT11, Moisture, LDR]
          |
          v
[Arduino Processing Unit]
          |
          v
[Check Threshold Values]
   | Temp > 30°C → Fan ON
   | Temp < 20°C → Heater ON
   | Soil Moisture < 60% → Pump ON
   | Light Low → Light ON
          |
          v
[4-Relay Module Activation]
          |
          v
[Repeat Continuously]

📦 Folder Structure
Greenhouse-Automation/
│── src/
│   └── greenhouse.ino
│── images/
│── docs/
│── README.md
└── LICENSE
