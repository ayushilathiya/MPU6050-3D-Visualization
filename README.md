# MPU6050-3D-Visualization

## Introduction

This project demonstrates how to visualize real-time motion using a tiny sensor and a web interface. By combining the ESP8266 Wi-Fi module with the MPU6050 motion sensor, we capture accelerometer and gyroscope data to create a 3D model that moves as you move the sensor.

## Components

- **ESP8266 NodeMCU** (Wi-Fi-enabled microcontroller)
- **MPU6050** (6-axis motion sensor)
- **Arduino IDE** with the necessary libraries
- **Libraries** used in the project:
  - `ESP8266WiFi` - Enables Wi-Fi functionality for ESP8266
  - `ESPAsyncTCP` - Handles asynchronous TCP communication
  - `ESPAsyncWebServer` - Creates an asynchronous web server
  - `Adafruit MPU6050` - Interfaces with the MPU6050 sensor
  - `Adafruit Sensor` - Provides a unified sensor interface
  - `Arduino_JSON` - Handles JSON formatting for web responses
  - `LittleFS` - Manages file storage on ESP8266

## How It Works

The **MPU6050** sensor captures accelerometer and gyroscope data. The accelerometer detects linear movement in 3 directions (X, Y, Z), while the gyroscope measures rotational motion. This data is processed and sent to a webpage where a 3D model is rendered to represent the sensor's movement in real-time.

### Technologies Used:
- **ESPAsyncWebServer** for real-time communication
- **Three.js** for 3D motion visualization
- **Server-Sent Events (SSE)** for continuous data streaming to the browser
