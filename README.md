# 📏 Ultrasonic Sensor – Distance Measurement & Obstacle Detection
## 📌 Overview
The Ultrasonic Sensor (HC-SR04) is widely used for non-contact distance measurement. It works by emitting ultrasonic waves and measuring the time taken for the echo to return after hitting an object.
This repository focuses on the working principle, timing analysis, ESP32 interfacing, and practical engineering applications of ultrasonic sensors.
## 🧠 Working Principle
The ultrasonic sensor uses the **Time-of-Flight (ToF)** principle.
It emits high-frequency sound waves (typically 40 kHz), which travel through air, reflect off an object, and return to the sensor.
The time taken for this round trip is used to calculate the distance.
## ⏱ Distance Calculation
Distance is calculated using:
Distance = (Speed of Sound × Time) / 2
The division by 2 accounts for the forward and return journey of the wave.
## 🔌 Pin Configuration
HC-SR04 has four pins:
* VCC → Power supply (5V)
* Trig → Trigger input
* Echo → Output signal
* GND → Ground
## ⚙️ Signal Operation
### 🔹 Steps:
1. ESP32 sends a 10µs pulse to Trig
2. Sensor emits ultrasonic burst
3. Echo pin goes HIGH
4. Echo stays HIGH until signal returns
5. Duration of HIGH signal = travel time
## 📡 ESP32 Interfacing
ESP32 reads the duration of the Echo signal and calculates distance.
### 🔹 Basic Flow:
* Trigger signal sent  
* Echo signal received  
* Time measured  
* Distance calculated  
* Output displayed or processed
## 🌐 IoT Integration
Ultrasonic sensors can be used in IoT systems for real-time monitoring.
### 🔹 Examples:
* Water level monitoring  
* Smart parking systems  
* Object detection alerts  
* Tank level monitoring  
