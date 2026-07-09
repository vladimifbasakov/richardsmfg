# Richards MFG — Industrial Embedded Test & Monitoring Platform

## Overview

This repository is dedicated to the development of an industrial embedded test and monitoring platform for electrical and electronic systems.

The project focuses on combining **STM32**, **ESP32**, **Raspberry Pi 5**, sensor acquisition, wireless communication, OTA firmware updates, data logging, dashboards, and anomaly detection into one practical R&D engineering platform.

The goal is to build a modular system that can be used for:

* industrial sensor monitoring;
* voltage and current measurement;
* embedded test automation;
* equipment diagnostics;
* remote data logging;
* IoT dashboards;
* anomaly detection using edge AI.

---

## Project Purpose

The main purpose of this project is to demonstrate a complete R&D engineering workflow:

```text
Idea
↓
Hardware concept
↓
Firmware development
↓
Sensor acquisition
↓
Communication protocol
↓
Data logging
↓
Dashboard visualization
↓
Testing and validation
↓
Industrial application
```

This project is intended to be useful as both a technical prototype and a professional portfolio project.

---

## Main Technologies

### Microcontrollers

* STM32G431 / STM32F303 / STM32F405
* ESP32-C6
* ESP32-S3

### Embedded Development

* STM32CubeIDE
* ESP-IDF
* PlatformIO
* Arduino Framework
* C / C++
* MicroPython

### Communication

* Wi-Fi
* BLE
* Zigbee
* MQTT
* CAN / CAN FD
* UART
* SPI
* I2C

### Sensors and Data Acquisition

* ADS1115 ADC
* Multi-channel voltage measurement
* Digital inputs
* PWM outputs
* Encoder counters
* Industrial sensor interfaces

### Data and Visualization

* Raspberry Pi 5
* Python
* MQTT broker
* InfluxDB
* Grafana
* CSV logging
* Web dashboard

### Future Expansion

* FPGA / CPLD acceleration
* Verilog
* Microchip IGLOO2 / SmartFusion2 / PolarFire
* Altium Designer PCB design
* Edge AI anomaly detection
* LSTM Autoencoder on Raspberry Pi 5

---

## Planned System Architecture

```text
Industrial Sensors / Voltage Inputs
              ↓
          STM32 MCU
  Real-time acquisition and filtering
              ↓
          ESP32-C6
 Wi-Fi / Zigbee / BLE / OTA / Web UI
              ↓
        Raspberry Pi 5
 MQTT + InfluxDB + Grafana + Python
              ↓
    AI-based anomaly detection
```

---

## Main Project Modules

### 1. STM32 Data Acquisition

Planned features:

* multi-channel ADC acquisition;
* real-time filtering;
* threshold detection;
* PWM generation;
* encoder input support;
* CAN / CAN FD communication;
* UART debug interface.

### 2. ESP32 IoT Gateway

Planned features:

* Wi-Fi connection;
* BLE support;
* Zigbee support for ESP32-C6;
* OTA firmware update;
* web dashboard;
* MQTT data publishing;
* non-volatile configuration storage.

### 3. Raspberry Pi 5 Dashboard

Planned features:

* MQTT broker;
* Python data collector;
* InfluxDB time-series database;
* Grafana dashboard;
* CSV export;
* alarm history;
* anomaly detection experiments.

### 4. Edge AI Anomaly Detection

Planned features:

* voltage pattern analysis;
* moving average and RMS features;
* anomaly detection using LSTM Autoencoder;
* alarm classification;
* visualization of abnormal events.

### 5. FPGA / CPLD Expansion

Future FPGA module:

```text
STM32G431
    ↓ SPI
FPGA / CPLD
    ├── high-speed counters
    ├── PWM generator
    ├── encoder counters
    ├── FIFO buffer
    └── simple digital filters
```

This module will be useful for high-speed digital acquisition and real-time preprocessing.

---

## Suggested Repository Structure

```text
richardsmfg/
├── README.md
├── docs/
│   ├── project_overview.md
│   ├── hardware.md
│   ├── firmware.md
│   ├── communication.md
│   ├── dashboard.md
│   └── test_results.md
├── firmware/
│   ├── stm32/
│   ├── esp32/
│   └── fpga/
├── hardware/
│   ├── schematics/
│   ├── pcb/
│   └── wiring/
├── software/
│   ├── raspberry_pi/
│   ├── mqtt/
│   ├── influxdb/
│   └── grafana/
├── images/
├── tests/
└── LICENSE
```

---

## Current Development Status

This project is currently in the early development stage.

Planned first milestones:

* [ ] Create basic repository structure
* [ ] Add STM32 firmware example
* [ ] Add ESP32-C6 Wi-Fi / OTA example
* [ ] Add MQTT communication example
* [ ] Add Raspberry Pi 5 Python data logger
* [ ] Add Grafana dashboard screenshots
* [ ] Add test results and measurements
* [ ] Add hardware wiring diagrams
* [ ] Add FPGA learning module

---

## Example Use Cases

### Industrial Monitoring

Monitor voltage, current, temperature, vibration, or digital signals from industrial equipment.

### Embedded Test Bench

Use STM32 and ESP32 boards as a flexible test platform for sensors, drivers, relays, and communication interfaces.

### Remote Diagnostics

Send measurements to Raspberry Pi 5 and display them in Grafana dashboards.

### Predictive Maintenance

Use historical sensor data and anomaly detection to identify unusual behavior before failure.

### Engineering Portfolio

Demonstrate practical skills in:

* embedded systems;
* STM32 firmware;
* ESP32 IoT;
* industrial communication;
* test automation;
* data logging;
* dashboards;
* edge AI;
* PCB and FPGA expansion.

---

## Hardware Used

Planned or supported hardware:

* STM32G431 Nucleo
* STM32F303RE Nucleo
* STM32F405RE Nucleo
* ESP32-C6 development board
* ESP32-S3 development board
* Raspberry Pi 5
* ADS1115 ADC modules
* CAN / CAN FD transceivers
* MCP2515 CAN module
* sensors and test fixtures
* oscilloscope
* multimeter
* ST-Link / J-Link programmer

---

## Software Tools

* STM32CubeIDE
* STM32CubeProgrammer
* ESP-IDF
* PlatformIO
* Arduino IDE
* VS Code
* Python
* Git
* InfluxDB
* Grafana
* Altium Designer
* Libero SoC Design Suite

---

## Professional Focus

This project reflects the work of an R&D Embedded Systems Engineer specializing in:

* embedded firmware development;
* industrial test systems;
* microcontroller-based control;
* IoT communication;
* sensor data acquisition;
* hardware debugging;
* edge AI experiments;
* PCB and system-level prototyping.

---

## Author

**Vladimif Basakov**
R&D Embedded Systems Engineer
GitHub: [@vladimifbasakov](https://github.com/vladimifbasakov)

---

## License

This project is intended for educational, research, and portfolio purposes.

A license file will be added later.
Add initial project README
