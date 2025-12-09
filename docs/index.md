---
title: Welcome
tags:
  - tag1
  - tag2
---

<center>
<font size="6">Danitza Datasheet</font><br>
as part of<br>
<font size="8"><b>Phoenix Force</b></font><br>
for<br>
<font size="5"><b>Team 315</b></font><br>
<strong>Submission: December 08, 2025</strong>
</center>

## Introduction
Our team was tasked with assisting wildfire responders, as wildfires have significantly increased in frequency and intensity in recent years. **TerraGuard** is a two-board autonomous rover paired with a portable display screen that creates its own Wi-Fi hotspot, enabling real-time communication with the rover.

### Project Summary
The rover is equipped with:
- BME688 (temperature, humidity, pressure, and gas sensor)
- MQ-2 gas sensor (detects smoke and multiple combustible gases)
- GPS module
- DC motors for mobility

The portable display is a **CrowPanel ESP32-S3** with status LEDs to indicate rover connection and visual alerts when sensors detect environmental changes.

Full project details and team report: [Phoenix Force Team Report](https://egr314-2025-f-315.github.io/phoenixforce.github.io/)

### My Contribution

#### Gas Sensor Integration (MQ-2)
Early detection of fire indicators is critical for wildfire prevention. Even small ignitions can rapidly escalate into large-scale fires.  
I selected the MQ-2 sensor for its ability to detect a wide range of combustible gases and smoke. I developed and calibrated the detection code using the Rs/Ro ratio method:

- **Rs** = Sensor resistance in the presence of target gas  
- **Ro** = Sensor resistance in clean air  

This ratio-based approach provides reliable gas concentration readings.

#### Rover Chassis & Display Cover Design
Designed and 3D-printed the rover chassis and display protective cover using SolidWorks.  
For a complete list of materials and components, see the ["Bill of Materials (BOM)"](https://embedded-systems-design.github.io/EGR304DataSheetTemplate/03-BOM/BOM/) section.

### Individual Assignment – Component Selection: MQ-2 Smoke/Gas Sensor
**Key Features:**
- High-quality dual-panel design with power and status indicators
- TTL digital output (LOW when gas detected) – can be directly connected to a microcontroller
- Analog output (0.1–4 V) proportional to gas concentration
- Requires pre-heating (~60 seconds) for stable readings due to internal heating element

**Specifications:**
- Input voltage: DC 5V
- Power consumption: ~150 mA
- DO output: TTL digital 0 and 1 (0.1V / 5V)
- AO output: 0.1–0.3 V (clean air), up to ~4 V at maximum concentration

[Official MQ-2 Datasheet (PDF)](https://cdn.sparkfun.com/assets/3/b/0/6/d/MQ-2.pdf)

### Photos

| Rover (Front View) | Rover (Back View) | Display Screen | Gas Sensor Setup |
|--------------------|-------------------|----------------|------------------|
| ![Rover Front](Rover.png) | ![Rover Side](Rover2.png) | ![Screen](Screen.png) | ![Gas Sensor](GAS_sensor.png) |

---
*EGR 314 – Embedded Systems Design | Fall 2025 | Team 315 – Phoenix Force*
