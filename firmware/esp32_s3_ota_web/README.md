# ESP32-S3 OTA Web LED Controller

## Overview

This module is the first ESP32 firmware example for the **Richards MFG — Industrial Embedded Test & Monitoring Platform** repository.

The goal is to build a simple but professional ESP32-S3 project that demonstrates:

- Wi-Fi connectivity;
- web-based device control;
- LED ON/OFF control;
- OTA firmware update support;
- persistent configuration storage;
- basic device status reporting.

This project is intended as a starting point for future industrial IoT gateway features.

---

## Target Hardware

- ESP32-S3 DevKit
- LED connected to GPIO2
- USB cable for programming and serial monitor
- Wi-Fi network for web control and OTA updates

---

## Planned Features

- [ ] Wi-Fi connection
- [ ] Web server
- [ ] Responsive web interface
- [ ] LED ON/OFF control
- [ ] AJAX or WebSocket state update
- [ ] Store LED state in NVS / Preferences
- [ ] Restore LED state after reboot
- [ ] ArduinoOTA support
- [ ] OTA progress in Serial Monitor
- [ ] Device status page
- [ ] Display uptime, IP address, RSSI, and firmware version

---

## Software Stack

Recommended development stack:

- PlatformIO
- Arduino Framework for ESP32
- C++
- ArduinoOTA
- Preferences / NVS
- WebServer or AsyncWebServer

---

## Basic Architecture

```text
Browser / Phone
      ↓
ESP32-S3 Web Server
      ↓
LED Control Logic
      ↓
GPIO2 LED

Wi-Fi Network
      ↓
OTA Firmware Update
