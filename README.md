<div align="center">

# PCB Design for an Attitude and Heading Reference System (AHRS)

### A custom 4-layer PCB featuring an STM32 MCU and a 9-axis IMU, developed during a research internship at the Indian Institute of Technology, Kanpur.

![KiCad](https://img.shields.io/badge/KiCad-v6.x-blue?style=for-the-badge&logo=kicad)
![LTspice](https://img.shields.io/badge/LTspice-Simulation-orange?style=for-the-badge&logo=linear-technology)
![Hardware](https://img.shields.io/badge/Hardware-STM32-blueviolet?style=for-the-badge)

</div>

---

Welcome to the official repository for my AHRS project. This project documents the complete hardware design cycle—from component selection and circuit simulation to final PCB layout—for a custom Attitude and Heading Reference System. It was developed as the primary focus of my six-week internship in the Department of Electrical Engineering at IIT Kanpur.

> The goal of this project was to apply theoretical knowledge of electronics and embedded systems to a practical challenge: creating a compact, reliable, and manufacturable PCB for high-performance orientation sensing in robotics and navigation applications.

---

## Table of Contents
1.  [Key Features](#-key-features)
2.  [Repository Structure](#-repository-structure)
3.  [Technical Specifications](#-technical-specifications)
4.  [Challenges & Solutions](#-challenges--solutions)
5.  [Contact & Acknowledgments](#-contact--acknowledgments)

---

## ✨ Key Features

-   **High-Performance Sensing**: Integrates the `LSM9DS1` 9-axis IMU, which includes a 3-axis accelerometer, 3-axis gyroscope, and 3-axis magnetometer on a single chip.
-   **Powerful Processing**: Driven by an `STM32F401RET6` ARM Cortex-M4 microcontroller, providing ample computational power for real-time sensor fusion algorithms.
-   **Stable Power Management**: Features an onboard `TPS62172` buck converter to efficiently step down 5V from USB to a clean 3.3V supply, validated through LTspice simulations.
-   **Robust Connectivity**: Equipped with a `CP2102` USB-to-UART bridge for straightforward data streaming, programming, and debugging.
-   **Optimized 4-Layer PCB**: The layout is designed for a compact form factor while maintaining excellent signal integrity and noise immunity through dedicated ground and power planes.

---

## 📂 Repository Structure

The project files are organized into two primary directories, separating the hardware design from the circuit simulation.

```
AHRS-PCB-Design/
├── PCB + Schematics/
│   ├── AHRSNEW.kicad_pro
│   ├── AHRSNEW.kicad_sch
│   └── AHRSNEW.kicad_pcb
│
└── Power Supply Simulation/
    └── Draft1.asc
```
-   **`PCB + Schematics/`**: This directory contains the complete KiCad project, including all source files for the schematic design and the final 4-layer PCB layout.
-   **`Power Supply Simulation/`**: This directory holds the LTspice simulation files used to validate the power supply circuit before finalizing the hardware design.

---

## 🛠️ Technical Specifications

### Hardware Components

| Component         | Part Number       | Description                                                 |
| :---------------- | :---------------- | :---------------------------------------------------------- |
| **Microcontroller** | `STM32F401RET6`     | ARM Cortex-M4 MCU for processing sensor data.               |
| **IMU Sensor** | `LSM9DS1`         | 9-axis motion sensor (accelerometer, gyroscope, magnetometer). |
| **Buck Converter** | `TPS62172`        | Efficiently steps down 5V USB power to a stable 3.3V.       |
| **USB-UART Bridge** | `CP2102`          | Provides a communication interface with a host computer.    |

### Software & Tools

-   **PCB Design**: KiCad (Schematic Capture & PCB Layout)
-   **Circuit Simulation**: LTspice (Power Supply Validation)

---

## 🧠 Challenges & Solutions

-   **Interpreting Complex Datasheets**
    -   *Solution*: Adopted a structured approach, breaking down datasheets section-by-section and cross-referencing with application notes and online forums.

-   **Achieving a Stable Power Supply**
    -   *Solution*: The power supply circuit was simulated in LTspice to validate component choices and ensure stable operation before hardware implementation.

-   **PCB Layout & Signal Integrity**
    -   *Solution*: Followed standard PCB best practices, including using differential pair routing for USB, keeping high-speed traces short, and utilizing ground planes to shield signals.

---

## 📬 Contact & Acknowledgments

This project was completed under the expert supervision of Prof. Yatindra Nath Singh at IIT Kanpur. I extend my sincere gratitude to my mentors, Mr. Nagendra Kumar and Mr. Rahul Bhattacharyya, for their continuous technical guidance and support.

Feel free to connect with me to discuss this project or other topics in embedded systems and robotics.

-   **LinkedIn**: [My LinkedIn Profile URL](https://www.linkedin.com/in/prakhar-sharma-75b998347/)
-   **GitHub**: [My GitHub Profile URL](https://github.com/Prakhar730)
-   **Email**: [My Mail](sprakhar2005@gmail.com)
