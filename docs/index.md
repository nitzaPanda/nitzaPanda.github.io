---
title: Welcome
tags:
- tag1
- tag2
---
<center>
<font size= "6">Danitza Datasheet</font><br>
as part of<br>
<font size= "8"> Phoenix Force</font><br>
for<br>
<font size= "5"> Team 315 </font><br>

**Submission: 12, 08, 2025**
</center>

## Introduction

* We were task to help wildfire responders since wildfire has increased over the years. Our TerraGuard is a two board rover with a portable screan that has its own wi-fi to communicate with the rover in real time.

### Project Summary

* The rover has BME688(temperature), MQ-2 gas sensor(detects versatile gases), GPS, and motors for mobility. The screen is CrowPanel EP-32-S3 with led to indicate status of the rover's connection and visual awareness if sensors detect changes to the environment. Full detail of project is in the link [team report.](https://egr314-2025-f-315.github.io/phoenixforce.github.io/)


### My Contribution

* Gas Sensor:
  Detecting early fire indicators is critical for wildfire prevention system, where even a small ignition can rapidly escalate into a destructive wildfire.          Carefully selected sensor that is able to read verious gases and smoke options. Created code and calibrated to detect gasses by using ratios.
  Rs= Sensor resistance when gas is present
  Ro= Sensor resistance in clean air
* Design rover and display cover:
  designed and 3D printed using SolidWorks. 

To review the details listed of the material used to construct the subsection, you can review it in the ["BOM"](https://embedded-systems-design.github.io/EGR304DataSheetTemplate/03-BOM/BOM/) section of the datasheet.

### IndividuaL Assignment

* Component  Selection:
 MQ-2 Sensor Detection has high-quality dual-panel design, with power indicator. TTL output valid signal is Low-level signal when the output light can be directly connected to the microcontroller. Analog output funtions with higher concentration of higher voltage. Sensor does need to be powered in advance because of the internal heat box needs to be warmed up and have stable data reading.

Total of 4 Pins:

Input voltage : DC5V Power consumption ( current ): 150mA

DO output : TTL digital 0 and 1 ( 0.1 and 5V)

AO output :0.1-0 .3 V ( relative to pollution ) , the maximum concentration of a voltage of about 4V

Ground : power supply is negative

["DATASHEET"](https://cdn.sparkfun.com/assets/3/b/0/6/d/MQ-2.pdf)


