<div align="center">

# PCB Design for an Attitude and Heading Reference System (AHRS)

### Complete hardware design files for a custom AHRS board developed during an internship at IIT Kanpur.

![KiCad](https://img.shields.io/badge/KiCad-v6.x-blue?style=for-the-badge&logo=kicad)
![LTspice](https://img.shields.io/badge/LTspice-Simulation-orange?style=for-the-badge&logo=linear-technology)
![Hardware](https://img.shields.io/badge/Hardware-STM32-blueviolet?style=for-the-badge)

</div>

---

Welcome to the repository for my AHRS PCB project. [cite_start]This project was undertaken as part of a six-week internship at the Indian Institute of Technology Kanpur (IIT Kanpur)[cite: 18, 55]. [cite_start]It contains all the necessary design files, from circuit schematics and power supply simulations to the final 4-layer PCB layout[cite: 27, 86].

> [cite_start]The goal of this project was to design a compact and reliable Printed Circuit Board (PCB) for an Attitude and Heading Reference System (AHRS)—a system that determines an object's orientation in space using inertial sensors[cite: 85].

---

## 📂 Repository Structure

The project is organized into two main directories: one for the KiCad PCB and schematic files, and another for the power supply circuit simulations.

.
├── PCB + Schematics/
│   ├── AHRSNEW.kicad_pro         # Main KiCad project file
│   ├── AHRSNEW.kicad_sch         # Top-level schematic file
│   └── AHRSNEW.kicad_pcb         # PCB layout file
│
└── Power Supply Simulation/
   └── Draft1.asc                # LTspice simulation schematic


-   [cite_start]`PCB + Schematics/`: Contains the complete **KiCad** project, including the schematic design, PCB layout, symbol libraries, and custom footprints[cite: 81, 96, 98].
-   [cite_start]`Power Supply Simulation/`: Contains **LTspice** files used to simulate and validate the onboard buck converter, ensuring a stable 3.3V power supply for the microcontroller and sensors[cite: 82, 94].

---

## ✨ Featured Hardware & Tools

### Core Components

| Component           | Part Number       | Description                                                  |
| :------------------ | :---------------- | :----------------------------------------------------------- |
| Microcontroller     | `STM32F401RET6`   | [cite_start]ARM Cortex-M4 MCU for processing sensor data[cite: 91].         |
| IMU Sensor          | `LSM9DS1`         | [cite_start]9-axis motion sensor (accelerometer, gyroscope, magnetometer)[cite: 91]. |
| Buck Converter      | `TPS62172`        | [cite_start]Efficiently steps down 5V USB power to a stable 3.3V[cite: 106]. |
| USB-UART Bridge     | `CP2102`          | Provides a communication interface with a host computer.     |

### Design & Simulation Software

-   [cite_start]**KiCad**: Used for the end-to-end schematic capture and 4-layer PCB layout design[cite: 81].
-   [cite_start]**LTspice**: Used for simulating the power supply circuit to ensure stable operation under various loads[cite: 82, 94].


***3D Visualization of the Assembled PCB***

---

## 📬 Contact & Acknowledgments

This project would not have been possible without the guidance and support from my mentors.

A special thanks to **Prof. Yatindra Nath Singh**, **Mr. Nagendra Kumar**, and **Mr. [cite_start]Rahul Bhattacharyya** from IIT Kanpur for their invaluable mentorship during this internship[cite: 11, 19, 21].

Feel free to connect with me:

-   **LinkedIn**: [Your LinkedIn Profile URL]
-   **Email**: [your.email@example.com]








this shit is broken rearead everything and write a proper one



Show thinking
Of course. I have re-read your internship report and analyzed your file structure to create a comprehensive and professional README.md. This version includes more detail, highlights the key technical features of your design, and better reflects the work you documented.

Here is the complete, copy-and-pasteable code for your README.md file.

Markdown

<div align="center">

# PCB Design for an Attitude and Heading Reference System (AHRS)

### A custom 4-layer PCB featuring an STM32 MCU and a 9-axis IMU, developed during a research internship at the Indian Institute of Technology, Kanpur.

![KiCad](https://img.shields.io/badge/KiCad-v6.x-blue?style=for-the-badge&logo=kicad)
![LTspice](https://img.shields.io/badge/LTspice-Simulation-orange?style=for-the-badge&logo=linear-technology)
![Hardware](https://img.shields.io/badge/Hardware-STM32-blueviolet?style=for-the-badge)

</div>

---

Welcome to the official repository for my AHRS project. This project documents the complete hardware design cycle—from component selection and circuit simulation to final PCB layout—for a custom Attitude and Heading Reference System. [cite_start]It was developed as the primary focus of my six-week internship in the Department of Electrical Engineering at IIT Kanpur[cite: 10, 55].

> [cite_start]The goal of this project was to apply theoretical knowledge of electronics and embedded systems to a practical challenge: creating a compact, reliable, and manufacturable PCB for high-performance orientation sensing in robotics and navigation applications[cite: 57, 59, 85].

---

## ✨ Key Features

-   [cite_start]**High-Performance Sensing**: Integrates the `LSM9DS1` 9-axis IMU, which includes a 3-axis accelerometer, 3-axis gyroscope, and 3-axis magnetometer on a single chip[cite: 91].
-   [cite_start]**Powerful Processing**: Driven by an `STM32F401RET6` ARM Cortex-M4 microcontroller, providing ample computational power for real-time sensor fusion algorithms[cite: 91].
-   [cite_start]**Stable Power Management**: Features an onboard `TPS62172` buck converter to efficiently step down 5V from USB to a clean 3.3V supply, validated through LTspice simulations[cite: 91, 94, 106].
-   [cite_start]**Robust Connectivity**: Equipped with a `CP2102` USB-to-UART bridge for straightforward data streaming, programming, and debugging[cite: 96].
-   [cite_start]**Optimized 4-Layer PCB**: The layout is designed for a compact form factor while maintaining excellent signal integrity and noise immunity through dedicated ground and power planes[cite: 98, 108].

---

## 📂 Repository Structure

The project files are organized into two main folders, separating the PCB design from the circuit simulation work.

.
├── PCB + Schematics/
│   ├── AHRSNEW.kicad_pro         # The main KiCad project file
│   ├── AHRSNEW.kicad_sch         # Top-level schematic file for the AHRS board
│   ├── AHRSNEW.kicad_pcb         # 4-layer PCB layout file
│   └── Library.pretty/           # Folder containing custom KiCad footprints
│
└── Power Supply Simulation/
   └── Draft1.asc                # LTspice simulation schematic for the TPS62172 buck converter


-   `PCB + Schematics/`: Contains the complete **KiCad** project, including schematics, PCB layout, project settings, and custom libraries.
-   `Power Supply Simulation/`: Contains the **LTspice** files used to simulate and validate the power supply circuit before its inclusion in the final design.

---

## 🛠️ Technical Specifications

### Hardware Components

| Component           | Part Number       | Description                                                  |
| :------------------ | :---------------- | :----------------------------------------------------------- |
| Microcontroller     | `STM32F401RET6`   | [cite_start]ARM Cortex-M4 MCU for processing sensor data[cite: 91].         |
| IMU Sensor          | `LSM9DS1`         | [cite_start]9-axis motion sensor (accelerometer, gyroscope, magnetometer)[cite: 91]. |
| Buck Converter      | `TPS62172`        | [cite_start]Efficiently steps down 5V USB power to a stable 3.3V[cite: 91, 106]. |
| USB-UART Bridge     | `CP2102`          | [cite_start]Provides a communication interface with a host computer[cite: 96].     |

### Software & Tools

-   [cite_start]**PCB Design**: **KiCad** (Schematic Capture & PCB Layout)[cite: 81].
-   [cite_start]**Circuit Simulation**: **LTspice** (Power Supply Validation)[cite: 82].

---

## 📬 Contact & Acknowledgments

This project was completed under the expert supervision of **Prof. Yatindra Nath Singh** at IIT Kanpur. I extend my sincere gratitude to my mentors, **Mr. Nagendra Kumar** and **Mr. [cite_start]Rahul Bhattacharyya**, for their continuous technical guidance and support[cite: 19, 21].

Feel free to connect with me to discuss this project or other topics in embedded systems and robotics.

-   **LinkedIn**: [[Your LinkedIn Profile URL](https://www.linkedin.com/in/prakhar-sharma-75b998347/)]
-   **GitHub**: [[My GitHub Profile URL](https://github.com/Prakhar730)]
-   **Email**: [My Email](sprakhar2005@gmail.com)]
