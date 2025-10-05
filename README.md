# Battery Management System Master Board (BMS Master)

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

## Cloning

A recursive clone must be used to download the `kicad-library` repository:

    git clone --recursive https://github.com/york-fs/bms-master.git
