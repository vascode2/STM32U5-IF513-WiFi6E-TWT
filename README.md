# STM32U5 Wi-Fi 6E & TWT Integration (Sona IF513)

**A low-power reference integration enabling Wi-Fi 6E connectivity and Target Wake Time (TWT) on the STM32U575I-EV board.**

![Project Status](https://img.shields.io/badge/Status-Finished-success)
![Hardware](https://img.shields.io/badge/Hardware-STM32U575I--EV-blue)
![Connectivity](https://img.shields.io/badge/Module-Sona_IF513_(WiFi_6E)-orange)

## 📖 Overview
This project demonstrates the integration of the **Ezurio (Laird Connectivity) Sona IF513 (Wi-Fi 6E / Bluetooth 5.4)** module with the ultra-low power **STM32U575I-EV** evaluation board.

Because the STM32U575I-EV lacks a native M.2 slot, this project details the hardware bridge (M.2 to Micro-SD adapter) and the specific software configurations required to drive the AIROC™ CYW55573 chipset via SDIO. Key features demonstrated include **Target Wake Time (TWT)**, which significantly reduces power consumption for battery-operated IoT devices.

## 🛠️ Tech Stack
* **MCU:** STM32U575 (Cortex-M33 Ultra-low power)
* **Wireless:** Sona IF513 (Infineon CYW55573)
* **Interface:** SDIO (4-bit)
* **Key Feature:** 802.11ax Target Wake Time (TWT)
* **Tools:** STM32CubeIDE, STM32CubeMX, Infineon AIROC Expansion Pack v1.7.0

## 📂 Documentation
The full step-by-step application note is hosted in this repository and also published online. It covers hardware modification, driver patching, and TWT validation.

### 🌐 [View the Official Published Guide](https://lairdcp.github.io/guides/IF513-STM32U575I-TWT/1.0/IF513-STM32U575I-TWT.html)

You can also view the local version in the `docs` folder:

### [👉 Read the Local Integration Guide](docs/IF513-STM32U575I-TWT.md)

* **Hardware Setup:** M.2 to Micro-SD bridge configuration.
* **Driver Patching:** Applying critical patches to the Infineon expansion pack.
* **TWT Validation:** Analyzing power-save modes using RF traces.

## 📦 Resources
* **Patches & Traces:** Available in [`docs/files`](docs/files/)
* **Source Code:** Derived from Infineon AIROC STM32 Expansion Pack v1.7.0

---
*Disclaimer: This project serves as a reference implementation. Please refer to the official Ezurio documentation for hardware specifications.*
