# Custom ESP32-S3-MINI-1 Development Board

## Overview
This repository contains the hardware design files for a custom ESP32-S3 4 layer development board. Built around the **ESP32-S3-MINI-1** module, this board is designed for flexible IoT development. 

The schematic and PCB layout were designed using **KiCad V6 E.D.A**.

**Schematic:**

<img width="1198" height="833" alt="image" src="https://github.com/user-attachments/assets/efcbcad6-7cf7-4900-b546-e99f3f077d5b" />

**PCB:**

<img width="537" height="763" alt="image" src="https://github.com/user-attachments/assets/77f13435-8566-4349-ba66-a49200195562" />
<img width="523" height="772" alt="image" src="https://github.com/user-attachments/assets/bbfd6591-d9d9-4ae9-8870-f7a88c7fe318" />

**Layers:**

<img width="371" height="857" alt="image" src="https://github.com/user-attachments/assets/38476eeb-6866-48b2-99e3-80cc236d0dc6" />

<img width="368" height="861" alt="image" src="https://github.com/user-attachments/assets/5377ce9c-0289-403e-a2ea-8557695463e2" />

<img width="368" height="861" alt="image" src="https://github.com/user-attachments/assets/31ec5dd8-0270-42f6-8e5d-6bf97868840c" />

<img width="350" height="844" alt="image" src="https://github.com/user-attachments/assets/1b146fd5-8457-478c-9647-7610f43fb4da" />

**3D View:**

<img width="505" height="864" alt="image" src="https://github.com/user-attachments/assets/bc2a83a8-5bf2-4953-ac95-5f64ce7373b7" />

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
