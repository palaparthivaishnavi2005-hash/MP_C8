````markdown
# IoT-Based Non-Destructive Invasive Species Suppression System

## Overview

The IoT-Based Non-Destructive Invasive Species Suppression System is a smart aquatic ecosystem monitoring and protection framework designed to detect environmental conditions that promote algae blooms and invasive species growth. The system continuously monitors water quality using multiple sensors connected to an ESP32 microcontroller and automatically performs eco-friendly corrective actions without using harmful chemicals.

The project provides real-time monitoring, risk assessment, automated control, OLED-based visualization, and WhatsApp notifications to support sustainable aquatic ecosystem management.

## Problem Statement

Freshwater ecosystems such as lakes, ponds, and reservoirs are increasingly affected by excessive algae growth, water pollution, reduced dissolved oxygen levels, and invasive species. Traditional monitoring approaches rely on manual sampling, laboratory analysis, chemical treatments, and mechanical cleaning, which are often expensive, time-consuming, environmentally harmful, and unsuitable for continuous monitoring.

This project addresses these limitations through a low-cost IoT-based monitoring and control system capable of continuous environmental assessment and automated intervention.

## Objectives

- Continuously monitor environmental parameters including turbidity, temperature, humidity, light intensity, gas concentration, and water level.
- Detect conditions favorable for algae bloom formation.
- Classify ecosystem health into Low, Medium, and High risk levels.
- Automate environmental control using pumps, fans, and alerts.
- Send real-time WhatsApp notifications for critical conditions.
- Provide a sustainable and non-destructive solution for aquatic ecosystem protection.

## Features

- Real-time environmental monitoring
- Algae bloom risk assessment
- Automated actuator control
- OLED-based status display
- WhatsApp notifications
- Low-cost implementation
- Energy-efficient operation
- Eco-friendly intervention methods
- Scalable architecture

## System Architecture

```text
Sensor Module
    ↓
Signal Conditioning
    ↓
ESP32 Processing
    ↓
Risk Assessment
    ↓
Decision Support Module
    ↓
Actuator Control
    ↓
OLED Display & Notifications
```

## Hardware Components

| Component             | Quantity | Purpose                             |
| --------------------- | -------- | ----------------------------------- |
| ESP32 Microcontroller | 1        | Main controller of the system       |
| Turbidity Sensor      | 1        | Measures water quality and clarity  |
| LDR Sensor            | 1        | Measures light intensity            |
| DHT11 Sensor          | 1        | Measures temperature and humidity   |
| MQ-135 Gas Sensor     | 1        | Detects decomposition-related gases |
| Float Sensor          | 1        | Measures water level                |
| Relay Module          | 1        | Controls actuators                  |
| Water Pump            | 2        | Water circulation and pumping       |
| DC Fan                | 1        | Aeration and cooling                |
| OLED Display          | 1        | Displays system status              |
| Buzzer                | 1        | Generates alerts                    |
| 7.4V Battery          | 1        | ESP32 power supply                  |
| 9V Batteries          | 3        | Actuator power supply               |


## Software Requirements

### Development Environment
- Arduino IDE

### Programming Language
- Embedded C/C++

### Libraries Used
- WiFi.h
- HTTPClient.h
- DHT.h
- Wire.h
- Adafruit_GFX.h
- Adafruit_SSD1306.h

## Methodology

### 1. Sensor Data Collection
The system continuously collects environmental data using turbidity, temperature, humidity, gas, light, and water-level sensors.

### 2. Signal Conditioning
Sensor readings are filtered, calibrated, normalized, and validated before processing.

### 3. ESP32 Processing
The ESP32 analyzes sensor values and evaluates ecosystem conditions.

### 4. Risk Assessment
Sensor readings are compared against predefined thresholds and classified into:
- Low Risk
- Medium Risk
- High Risk

### 5. Monitoring
Real-time information is displayed on the OLED screen and Serial Monitor.

### 6. Automated Intervention
Based on the identified risk level, actuators such as pumps, fans, and buzzers are activated automatically.

## Working Principle

1. Sensors continuously monitor environmental conditions.
2. Data is transmitted to the ESP32 microcontroller.
3. The ESP32 processes sensor readings and calculates risk levels.
4. Results are displayed on the OLED display.
5. Alerts are sent through WhatsApp when abnormal conditions occur.
6. Pumps, fans, and buzzers are activated automatically to maintain ecosystem balance.

## Risk Classification

| Risk Level | Description |
|------------|------------|
| Low | Normal environmental conditions |
| Medium | Slight imbalance requiring monitoring |
| High | Strong possibility of algae bloom formation requiring immediate intervention |

## Advantages

- Continuous real-time monitoring
- Early detection of ecosystem imbalance
- Reduced manual effort
- Cost-effective implementation
- Eco-friendly and non-destructive approach
- Suitable for rural and urban environments
- Easy deployment and maintenance
- Scalable for larger monitoring systems

## Applications

- Lakes
- Ponds
- Reservoirs
- Aquaculture farms
- Community water bodies
- Environmental monitoring projects
- Educational and research applications

## Future Enhancements

- Cloud-based monitoring dashboard
- Mobile application integration
- Solar-powered operation
- AI-based algae bloom prediction
- Camera-based invasive species detection
- Historical data analytics and visualization

## Sustainable Development Goals

This project supports:

- SDG 14: Life Below Water
- SDG 15: Life on Land

## Team Members

- Kopunamoni Pranitha (24251A05E6)
- Maudshetty Sneha (24251A05F1)
- Palaparthi Vaishnavi (24251A05F6)

## Guide

Dr. Jayashree S. Patil  
Associate Professor  
Department of Computer Science and Engineering  
G. Narayanamma Institute of Technology and Science (GNITS)



