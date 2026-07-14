# Custom-PCB
# Custom PCB Design for IoT Platform - ESP32-S3

## Project Overview

This project presents the design of a custom printed circuit board (PCB) developed for an IoT monitoring and control platform. The board is built around the ESP32-S3-WROOM-1-N16R8 module, combining artificial intelligence and IoT capabilities in a single compact solution.

> **Important Note:** This design was created for educational and demonstration purposes only and has not been sent for production.

---

## Objectives

- Design a custom PCB integrating an ESP32-S3 module for IoT applications
- Provide multiple connectivity options (Ethernet, USB, Wi-Fi, Bluetooth)
- Include a TFT display for local data visualization
- Implement robust power management with multiple supply options
- Create a versatile platform for AI and machine learning applications

---

## Microcontroller Selection

The ESP32-S3-WROOM-1-N16R8 module was chosen for its exceptional capabilities:

- **Processor:** Dual-core Xtensa LX7 @ up to 240 MHz
- **Flash Memory:** 16 MB
- **AI Acceleration:** Native support (ESP-DSP, ESP-ML)
- **Connectivity:** Wi-Fi 802.11 b/g/n, Bluetooth 5.0 (LE)
- **GPIOs:** 44 programmable pins
- **Security:** Hardware acceleration for encryption

Reference: ESP32-S3 Series Datasheet - Espressif Systems [13]

---

## PCB Architecture

The PCB is organized into three main functional blocks:

### Block 1: MCU & Power Management

**Components:**
- ESP32-S3-WROOM-1-N16R8 module
- TL1963A-33DCYR voltage regulator (3.3V, 1.5A)
- USB-C connector (power input and programming)
- CP2102 USB-to-UART converter (serial communication)
- RESET and BOOT buttons
- Status LEDs (Power, Activity)
- Power selection circuit (automatic switching)
- GPIO headers for expansion

### Block 2: Ethernet Connectivity

**Components:**
- W5500 Ethernet controller chip (hardwired TCP/IP stack)
- RJ45 connector with integrated magnetics
- SPI interface for communication with ESP32-S3
- 10/100 Mbps Ethernet support

### Block 3: TFT Display

**Components:**
- 3.5-inch TFT LCD display
- Resolution: 320 × 480 pixels
- SPI interface (4-wire)
- Optional touchscreen support

---

## Tools Used

- **Altium Designer** — PCB schematic design, layout, and routing
- **Altium 3D View** — Mechanical validation and 3D visualization
- **Octopart / Mouser** — Component selection and sourcing

---

## Repository Structure
