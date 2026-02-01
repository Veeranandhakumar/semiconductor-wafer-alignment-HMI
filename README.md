# semiconductor-wafer-alignment-HMI
This project simulates an automated semiconductor wafer alignment and counting system using Raspberry Pi logic in Proteus and a real-time HMI dashboard built with Node-RED. The system detects wafer alignment using a laser–LDR sensor setup, controls a motor for correction, and displays live status, alarms, and wafer count .

🧠 Wafer Alignment & Counting System with HMI
Raspberry Pi (Simulation) + Proteus + Node-RED Dashboard

📌 Project Overview

This project presents a simulation-based semiconductor wafer alignment and counting system integrated with a Human-Machine Interface (HMI). The system detects wafer alignment using a laser–LDR sensor setup, corrects misalignment using motor control logic, and provides real-time monitoring, counting, and alarms through a Node-RED dashboard.

The complete system is designed and tested in a virtual environment using Proteus, making it ideal for learning industrial automation concepts without physical hardware.

🚀 Key Features

🔍 Wafer alignment detection using laser and LDR sensor simulation
⚙️ Automatic motor control for wafer position correction
🔢 Real-time wafer counting system
🟢🔴 Visual status indicators (Aligned / Misaligned)
🖥 Live HMI dashboard using Node-RED
🚨 Alarm system for repeated misalignment
🔁 Reset and manual control options from HMI
🔌 Serial communication between Proteus simulation and Node-RED
🧩 Fully modular, scalable system design
🏭 Industrial Relevance

- Wafer handling and alignment are critical processes in semiconductor manufacturing. This project demonstrates:
- Embedded system design for industrial automation
- Human-Machine Interface (HMI) integration
- Real-time monitoring and control logic
- Fault detection and alarm handling
- This mirrors real-world semiconductor equipment control systems.

🏗 System Architecture

- The system consists of four major subsystems:
- Sensing System – Laser emitter and LDR detect wafer alignment
- Control System – Raspberry Pi GPIO logic controls motor and indicators
- Actuation System – DC motor driven through L293D motor driver
- HMI System – Node-RED dashboard displays status and allows control

📷 Functional Block Diagram image 
![WhatsApp Image 2026-02-01 at 7 04 19 PM](https://github.com/user-attachments/assets/956ba284-289b-4e7a-84c9-1b9e91e6e387)



⚙️ Technologies Used
🔧 Simulation & Embedded

- Proteus 8 Professional
- Raspberry Pi (GPIO simulation)
- MCP3208 ADC (Analog-to-Digital Conversion)
- L293D Motor Driver
- Laser + LDR alignment sensing

🖥 HMI & Communication
- Node-RED Dashboard
- UART Serial Communication
- COMPIM Module (Proteus)
- Virtual Serial Port (com0com / VSPE)

🔄 System Working

- A laser beam is aimed at an LDR sensor.
- If the beam is uninterrupted, the wafer is properly aligned.
- If the beam is blocked, the wafer is misaligned.
- The Raspberry Pi control logic:
- Stops motor if aligned
- Rotates motor to correct position if misaligned
- Alignment status is shown using:
      🟢 Green LED → Aligned
      🔴 Red LED → Misaligned
- Each successful alignment increases the wafer count.
- Status and count are sent to Node-RED via serial communication.
- The HMI dashboard displays:
- Alignment status
- Total wafer count
- Alarm warnings
- If repeated misalignment occurs, an alarm is triggered.

🖥 HMI Dashboard Features

- Live alignment status indicator
- Wafer counter display
- Alarm notifications
- Reset button for wafer count
- Manual motor control option

📷Node-Red Dashboard


🧪 Simulation Environment

- All hardware is simulated in Proteus, including:
- Raspberry Pi GPIO behavior
- Motor driver and DC motor
- Laser + LDR alignment sensing
- LCD status display
- Serial communication via COMPIM

📷 Schematic on Proteus
![Capture](https://github.com/user-attachments/assets/84171923-f654-4316-bc11-8f62f7ada150)


🎓 Key Learnings

- Embedded system simulation using Proteus
- Designing control logic for sensor-based automation
- Serial communication between embedded systems and HMI
- Developing real-time dashboards using Node-RED
- Implementing alarm and fault detection mechanisms
- System-level thinking for industrial automation design

🔮 Future Improvements

- Deploy system on real Raspberry Pi hardware
- Add vision-based alignment detection
- Cloud data logging and analytics
- Predictive maintenance using AI/ML
- Multi-wafer handling automation


👨‍💻 Author

Veeranandhakumar G
Electronics & Communication Engineering
Embedded Systems | Automation | HMI Systems
