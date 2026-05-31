# IoT-Based-Smart-Environmental-Monitoring-System-for-Underground-Mines
IoT-based environmental monitoring system for underground mines using ESP32, MQTT, Flask, SQLite, and real-time safety alerts for gas, temperature, humidity, noise, and worker health monitoring.

# IoT-Based Smart Environmental Monitoring System for Underground Mines

## Overview

The IoT-Based Smart Environmental Monitoring System for Underground Mines is a real-time safety monitoring platform designed to improve worker safety and environmental awareness in underground mining operations.

The system continuously monitors critical environmental and health-related parameters such as gas concentration, temperature, humidity, noise levels, and heart rate using IoT sensors connected to an ESP32 microcontroller. The collected data is transmitted through MQTT, processed by a Flask-based backend, stored in a database, and visualized through a web dashboard.

When unsafe conditions are detected, the system generates instant alerts to help prevent accidents and ensure timely intervention.

---

## Problem Statement

Underground mining environments are highly hazardous due to the presence of toxic gases, poor ventilation, extreme temperatures, excessive noise, and worker health risks. Traditional monitoring approaches may not provide continuous real-time visibility into environmental conditions.

This project addresses these challenges by providing an automated IoT-based monitoring solution capable of detecting dangerous conditions and generating real-time alerts.

---

## Objectives

- Monitor environmental conditions in underground mines.
- Detect hazardous gas concentrations.
- Track temperature and humidity levels.
- Monitor noise pollution levels.
- Observe worker health parameters.
- Generate alerts during unsafe conditions.
- Store and visualize historical data for analysis.

---

## Features

### Real-Time Monitoring
- Gas Detection (MQ2 Sensor)
- Carbon Monoxide Monitoring (MQ9 Sensor)
- Temperature Monitoring
- Humidity Monitoring
- Noise Level Monitoring
- Heart Rate Monitoring

### Safety Alerts
- Real-Time Hazard Detection
- Email Notifications
- Telegram Notifications
- Emergency Warning Alerts

### Dashboard
- Live Sensor Data Display
- Environmental Status Indicators
- Historical Data Visualization
- Interactive Charts and Graphs
- Responsive Web Interface

### Data Management
- MQTT-Based Data Transmission
- SQLite Database Storage
- Historical Data Logging
- Real-Time Data Updates

---

## Technology Stack

### Hardware
- ESP32 Development Board
- MQ2 Gas Sensor
- MQ9 Gas Sensor
- DHT11 Temperature and Humidity Sensor
- Heart Rate Sensor
- Sound/Noise Sensor

### Software
- Python
- Flask
- MQTT (HiveMQ Cloud)
- SQLite
- HTML
- CSS
- JavaScript
- Bootstrap
- Chart.js

---

## System Architecture

```text
Sensors
   │
   ▼
ESP32 Microcontroller
   │
   ▼
MQTT Broker (HiveMQ Cloud)
   │
   ▼
Flask Backend Server
   │
   ├── SQLite Database
   ├── Alert System
   └── Data Processing
   │
   ▼
Web Dashboard
```

---

## Project Structure

```text
project/
│
├── app.py
├── run.py
├── requirements.txt
├── sensor_data.db
│
├── static/
│   ├── css/
│   ├── js/
│   └── images/
│
├── templates/
│   └── index.html
│
├── sms_alerts.py
├── email_configuration_info.py
├── test_connection.py
│
└── README.md
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/iot-smart-environmental-monitoring-underground-mines.git
```

### Navigate to Project Folder

```bash
cd iot-smart-environmental-monitoring-underground-mines
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run the Application

```bash
python run.py
```

### Access Dashboard

```text
http://localhost:5000
```

---

## Workflow

1. Sensors collect environmental and worker health data.
2. ESP32 reads sensor values.
3. Data is transmitted to the MQTT broker.
4. Flask backend subscribes to MQTT topics.
5. Sensor readings are stored in SQLite.
6. Dashboard displays live updates.
7. Alert system notifies users when thresholds are exceeded.

---

## Applications

- Underground Coal Mines
- Metal Mining Operations
- Tunnel Construction Projects
- Industrial Safety Monitoring
- Hazardous Work Environments

---

## Future Enhancements

- AI-Based Hazard Prediction
- Mobile Application Support
- GPS-Based Worker Tracking
- Predictive Maintenance Analytics
- Multi-Site Monitoring
- Cloud Deployment

---

## Results

- Continuous environmental monitoring
- Early detection of hazardous conditions
- Improved worker safety
- Real-time alert generation
- Historical data analysis support

---

## Contributors

- MV Siddardha
- Team Members

---

## License

This project is developed for educational, research, and hackathon purposes.
