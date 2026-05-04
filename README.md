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
