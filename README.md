# Custom ESP32-S3-MINI-1 Development Board

## Overview
This repository contains the hardware design files for a custom ESP32-S3 development board. Built around the **ESP32-S3-MINI-1** module, this board is designed for flexible IoT development. It integrates onboard environmental sensing and status indicators, making it an excellent foundation for projects like automated smart plant watering systems or custom home automation nodes.

The schematic and PCB layout were designed using **KiCad E.D.A**.

Schematic:
<img width="1198" height="833" alt="image" src="https://github.com/user-attachments/assets/efcbcad6-7cf7-4900-b546-e99f3f077d5b" />

## Hardware Features
This development board includes:
* **Microcontroller:** ESP32-S3-MINI-1 (Wi-Fi & Bluetooth LE).
* **USB Interface:** USB Type-C receptacle with dedicated ESD protection (D3V3XA4B10LP).
* **Power Management:** 5V to 3.3V LDO regulator (TLV75801PDBV) with a dedicated power indicator LED.
* **Onboard Sensors & Outputs:**
  * **ENS210** Temperature and Humidity Sensor (connected via I2C).
  * **WS2812B** Addressable RGB LED for visual status feedback.
* **User Controls:** Physical `BOOT` and `RESET` tactile switches for easy flashing and debugging.
* **Expansion:** Two 22-pin headers breaking out GPIOs, I2C, UART, USB data lines, and power rails for easy breadboarding.

## Acknowledgements & Design Methodology
The design of this custom board was verified and optimized following the hardware design tutorials by **John Teel** at [Predictable Designs](https://predictabledesigns.com/). 

## Related Documents & Resources
For detailed specifications on the core components and reference designs, please consult the following official Espressif documentation:

* [ESP32-S3 Datasheet (PDF)](#)
* [ESP32-S3-MINI-1 & ESP32-S3-MINI-1U Datasheet (PDF)](#)
* [ESP32-S3-DevKitM-1 Schematic (PDF)](#)
* [ESP32-S3-DevKitM-1 PCB layout (PDF)](#)
* [ESP32-S3-DevKitM-1 Dimensions (PDF)](#)
* [ESP32-S3-DevKitM-1 Dimensions source file (DXF)](#) 

## Repository Structure
* `/Hardware` - KiCad project files (`.pro`, `.sch`, `.kicad_pcb`).
* `/Docs` - Exported schematics, BOM, and Gerber files for manufacturing.
* `/Firmware` - Example code for testing the WS2812B LED and ENS210 sensor.
