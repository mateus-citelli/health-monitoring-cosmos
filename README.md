# Health Monitoring Cosmos

Health Monitoring Cosmos is a wearable health monitoring project designed for astronauts during space missions.

The goal is to collect and process physiological data efficiently using embedded systems, with a focus on low power consumption, reliability, and real-time monitoring.

## Main Features

- Heart rate monitoring
- Blood oxygen saturation (SpO₂)
- Skin temperature monitoring
- Heart Rate Variability (HRV)
- Motion and activity detection
- Signal filtering and processing
- Individual health baseline
- Anomaly detection
- Bluetooth Low Energy communication
- Power management for low-energy operation

## Technologies

The firmware is developed primarily in **C** using the **ESP-IDF** framework.

Main technologies and components:

- ESP-IDF
- FreeRTOS
- NimBLE / Bluetooth Low Energy
- I2C communication
- Embedded signal processing
- Low-power firmware techniques

## Firmware Architecture

```text
ESP-IDF
   │
   ├── FreeRTOS
   │
   ├── I2C Drivers
   │      ├── MAX30102
   │      ├── TMP117
   │      └── IMU
   │
   ├── Signal Processing
   │      ├── Filters
   │      ├── Heart Rate
   │      ├── SpO₂
   │      └── HRV
   │
   ├── Health Analysis
   │      ├── Baseline
   │      └── Anomaly Detection
   │
   ├── NimBLE
   │
   └── Power Management