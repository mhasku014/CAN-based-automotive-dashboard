🚗 CAN-Based Automotive Dashboard System
A real-time automotive dashboard system built using the CAN (Controller Area Network) protocol, simulating a functional vehicle instrument cluster with multiple ECUs communicating over the CAN bus.

📌 Project Overview
This project replicates a real-world automotive dashboard by establishing a multi-node CAN network using three ECUs. Vehicle parameters such as speed, RPM, gear position, and turn indicators are acquired, transmitted, and displayed in real-time on a Character LCD (CLCD), demonstrating the working of an embedded automotive communication system.

⚙️ System Architecture
ECURoleParameters HandledECU 1Transmitter Node 1Vehicle Speed, Gear PositionECU 2Transmitter Node 2Engine RPM, Turn IndicatorsECU 3Receiver / Display NodeReceives all data & displays on CLCD

🔧 Features

Real-time display of Vehicle Speed and Engine RPM simulated via potentiometers
Gear Position monitoring and display
Turn Indicator status display (Left / Right)
Multi-node CAN bus communication between three ECUs
Live data rendering on Character LCD (CLCD)


🛠️ Technologies & Tools Used

Embedded C — Core programming language
CAN Protocol — Inter-ECU communication
ECU (Electronic Control Unit) — Three-node embedded architecture
Potentiometer — Analog signal simulation for Speed & RPM
Character LCD (CLCD) — Real-time data display
CAN Transceiver — Physical layer communication
ADC (Analog to Digital Converter) — Analog signal processing


📂 Project Structure
CAN-Automotive-Dashboard/
│
├── ECU1_Speed_Gear/          # ECU 1 - Speed & Gear Position transmitter code
├── ECU2_RPM_Indicator/       # ECU 2 - RPM & Turn Indicator transmitter code
├── ECU3_Display/             # ECU 3 - Receiver & CLCD display code
├── Docs/                     # Circuit diagrams & documentation
└── README.md

🔌 Hardware Requirements

3x Microcontroller boards (ECUs)
CAN Transceiver modules
Potentiometers (x2) — for Speed & RPM simulation
Character LCD (16x2 or 20x4)
Connecting wires & breadboard


🚀 How It Works

ECU 1 reads analog values from a potentiometer for speed and monitors gear position, then transmits both over the CAN bus.
ECU 2 reads analog values for RPM and monitors the turn indicator state, transmitting over the CAN bus.
ECU 3 receives all CAN messages, decodes the data, and displays Vehicle Speed, RPM, Gear Position, and Turn Indicator status in real-time on the CLCD.


📸 Output

Vehicle Speed | Engine RPM | Gear Position | Turn Indicator — all displayed live on Character LCD.


🧠 Key Learnings

Multi-node CAN network design and bus arbitration
ECU-level embedded C programming
Real-time data acquisition and display
CAN message framing, ID prioritization, and decoding
Hardware-software integration on embedded platforms


👤 Author
[Mhasku Kumbharkar]
Embedded Systems Engineer | https://www.linkedin.com/in/mhasku-kumbharkar.
