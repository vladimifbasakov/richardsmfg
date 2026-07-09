# Project Overview

## Project Name

**Richards MFG — Industrial Embedded Test & Monitoring Platform**

## Purpose

This project is an industrial embedded test and monitoring platform focused on electrical measurements, sensor data acquisition, remote diagnostics, test automation, and edge AI anomaly detection.

The goal is to build a modular R&D engineering platform that combines microcontrollers, wireless communication, data logging, dashboards, and future FPGA acceleration into one practical system.

## Engineering Problem

Industrial electrical systems often require reliable monitoring, repeatable testing, and early detection of abnormal behavior. Traditional manual measurements are useful, but they are limited when many channels must be monitored continuously.

This project addresses that problem by creating a system that can:

- collect multi-channel sensor and voltage data;
- process signals in real time;
- detect threshold violations;
- send data wirelessly;
- log measurements over time;
- display results in dashboards;
- support future AI-based anomaly detection.

## High-Level Architecture

```text
Industrial Sensors / Voltage Inputs
              ↓
          STM32 MCU
  Real-time acquisition and filtering
              ↓
          ESP32-C6 / ESP32-S3
 Wi-Fi / BLE / Zigbee / OTA / Web UI
              ↓
        Raspberry Pi 5
 MQTT + InfluxDB + Grafana + Python
              ↓
    Edge AI anomaly detection
