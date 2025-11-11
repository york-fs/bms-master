# Battery Management System Master Board (BMS Master)

![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/york-fs/bms-master/ci.yml?label=DRC)
![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fyork-fs.github.io%2Fbms-master%2Finfo.json&query=%24.pad_count&label=Pad%20Count)
![Dynamic JSON Badge](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fyork-fs.github.io%2Fbms-master%2Finfo.json&query=%24.via_count&label=Via%20Count)

The BMS master board which connects to a daisy chain of distributed segment boards and continuously checks all
critical values. Two linear hall effect current sensors are sampled to measure the main DC battery current.

## Features

* **I2C Communication to Distributed Segment Boards**
* **Dual-Pole Current Sensing**
  * Uses open-loop hall effect current sensors
* **CAN Communication**
* **Active-High Open-Drain Shutdown Output**
  * Driven high to ~10.9 volts to indicate healthy state
  * High impedance in a fault state
  * Matches the Bender ISOMETER IR155-3204 IMD
* **eFuse and TVS Protected LVS Input**
  * Designed for 12 volt nominal input
  * Overvoltage lockout at ~16.7 volts
* **Microcontroller Watchdog with 3V3 Rail Monitoring**
* **EEPROM Config**

![Preview Render](https://york-fs.github.io/bms-master/preview.jpg)

## Cloning

A recursive clone must be used to download the `kicad-library` repository:

    git clone --recursive https://github.com/york-fs/bms-master.git
