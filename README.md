# Battery Management System Master Board (BMS Master)

![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/york-fs/bms-master/ci.yml?label=DRC)
![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fyork-fs.github.io%2Fbms-master%2Finfo.json&query=%24.pad_count&label=Pad%20Count)
![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fyork-fs.github.io%2Fbms-master%2Finfo.json&query=%24.via_count&label=Via%20Count)

The BMS master board which connects to a daisy chain of distributed segment boards and continuously checks all
critical values. Two linear hall effect current sensors are sampled to measure the main DC battery current.

## Features

* **I2C Communication to Distributed Segment Boards**
* **Current Sensing**
  * On both battery poles
  * Uses a linear hall effect current sensor
* **CAN Communication**
  * Periodically sends telemetry data
* **Shutdown and Charge Enable Outputs**
* **EEPROM Config**

![Preview Render](https://york-fs.github.io/bms-master/preview.jpg)

## Cloning

A recursive clone must be used to download the `kicad-library` repository:

    git clone --recursive https://github.com/york-fs/bms-master.git
