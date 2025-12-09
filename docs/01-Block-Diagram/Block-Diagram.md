---
title: Individual Subsystem Block Diagram – Gas Sensor 
tags:
  - air-quality
  - ESP32
  - gas-sensor
---

# Gas Sensor Subsystem – Block Diagram Overview

This document describes the hardware connection of gas sensing node used in our project.

![Gas Sensor Subsystem Block Diagram](block_diagram.png)

## Key Features
- Fully wireless (Wi-Fi + Bluetooth) operation  
- Integrated GPS for geolocation  
- Local OLED display for real-time readings  
- Long battery life using efficient power conversion  
- Expandable via upstream/downstream connectors  

## Main Components

| Component              | Description                                                                                   | Key Details                          |
|-----------------------|------------------------------------------------------------------------------------------------|--------------------------------------|
| **Microcontroller**   | ESP32-S2 (or ESP32-S3 variant)                                                                | Wi-Fi/BLE, ADC, UART, GPIO control   |
| **Gas Sensor**        | Multi-gas sensor module (PN: 701715455504)                                                    | Analog output, 5V heater + 3.3V logic|
| **Wireless**          | Built-in ESP32 radio + external antenna                                                       | u.FL connector for improved range    |
| **GPS Module**        |        NEO-6M                                                                                 | UART interface, 5V/3.3V compatible   |
| **Display**           | Integrated OLED screen (likely 0.96" or 1.3" SSD1306/SH1106)                                  | Driven directly by ESP32             |
| **Power Supply**      | Single-cell LiPo/Li-ion battery (3.7–4.2 V) → DC/DC converters                                | Outputs: regulated 5V and 3.3V rails |
| **Connectors**        | 2× 8-pin (4x2) headers + battery connector                                                    | Upstream/downstream chaining, debug  |


