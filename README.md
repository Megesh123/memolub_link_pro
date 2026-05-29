# Link Pro Timer

Industrial lubrication timer powered by ESP32-S3 with local scheduling, motor control, remote connectivity, and firmware update capabilities.

## Overview

Link Pro Timer is an intelligent lubrication controller designed for automated lubrication systems. The device provides configurable lubrication schedules, reliable motor control, status monitoring, and connectivity through Wi-Fi and GSM networks.

Built on the ESP32-S3 platform, the system combines industrial reliability with modern connectivity features, making it suitable for a wide range of lubrication applications.

---

## Key Features

* Configurable lubrication scheduling
* ESP32-S3 based control platform
* Motor control using MOSFET driver circuitry
* Proximity sensor monitoring
* Real-Time Clock (RTC) for accurate scheduling
* Graphical user interface through SINDA display
* Wi-Fi connectivity
* GSM communication using A7672G module
* Over-the-Air (OTA) firmware update support
* Remote diagnostics and maintenance capabilities
* Industrial-grade operation

---

## Hardware Components

| Component         | Description               |
| ----------------- | ------------------------- |
| MCU               | ESP32-S3                  |
| Display           | SINDA Display             |
| RTC               | Real-Time Clock Module    |
| Communication     | Wi-Fi + A7672G GSM Module |
| Motor Driver      | MOSFET-Based Control      |
| Sensor            | Proximity Sensor          |
| Firmware Platform | PlatformIO                |

---

## System Architecture

The Link Pro Timer consists of the following functional blocks:

* User Interface Layer

  * Display management
  * User configuration
  * Status visualization

* Control Layer

  * Lubrication scheduling
  * Motor control
  * Safety monitoring

* Communication Layer

  * Wi-Fi connectivity
  * GSM connectivity
  * Remote diagnostics

* Firmware Management

  * OTA update handling
  * Version management
  * Recovery mechanisms

---

## Lubrication Scheduling

The controller allows users to configure lubrication intervals according to application requirements.

Features include:

* Adjustable lubrication cycles
* RTC-based timing accuracy
* Persistent schedule storage
* Automatic operation after power restoration

---

## Connectivity

### Wi-Fi

Wi-Fi connectivity enables:

* Device configuration
* Firmware updates
* Diagnostic access
* Development and testing support

### GSM (A7672G)

The integrated GSM module provides:

* Remote communication
* Network-independent operation
* Field deployment flexibility

---

## OTA Firmware Updates

The firmware supports Over-the-Air (OTA) updates using GitHub Releases.

> Note: OTA functionality is currently intended for development, validation, and testing purposes. Production deployment procedures may differ depending on customer requirements.

OTA benefits include:

* Remote firmware deployment
* Reduced maintenance effort
* Faster bug fixes and feature validation
* Version-controlled releases

---

## Repository Structure

```text
memolub_link_pro/
├── include/
├── lib/
├── src/
├── test/
├── platformio.ini
└── README.md
```

### Directory Description

* `src/` - Application source code
* `include/` - Header files
* `lib/` - Custom and third-party libraries
* `test/` - Unit and integration tests
* `platformio.ini` - PlatformIO project configuration

---

## Development Environment

### Requirements

* PlatformIO
* Visual Studio Code
* ESP32 Platform Support

### Build

```bash
pio run
```

### Upload

```bash
pio run --target upload
```

### Serial Monitor

```bash
pio device monitor
```

---

## Applications

Link Pro Timer is suitable for:

* Automated lubrication systems
* Industrial machinery
* Manufacturing equipment
* Conveyor systems
* Bearings and chain lubrication systems
* Preventive maintenance applications

---

## Reliability Features

* RTC-backed scheduling
* Sensor-based monitoring
* Remote firmware maintenance
* Industrial communication support
* Robust ESP32-S3 platform

---

## Support

For technical support, feature requests, or issue reporting, please contact the Memolub engineering team.

---

## License

Copyright © Memolub.

All rights reserved.
