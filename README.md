# Bluetooth Controlled Robotic Car Using Arduino

## Objective
To design and implement a **Bluetooth-controlled robotic car** using an **Arduino microcontroller**, where motor movements are controlled through **serial commands received via a Bluetooth module**.

---

## Components Used
- Arduino UNO / Nano
- Bluetooth Module (HC-05 / HC-06)
- Motor Driver Module (L293D / L298N)
- 2 × DC Motors
- Robot Chassis
- Battery / Power Supply
- Jumper Wires

---

## Pin Configuration

### Motor Driver Connections
| Motor | Arduino Pin |
|------|-------------|
| Motor 1 IN1 | 9 |
| Motor 1 IN2 | 10 |
| Motor 2 IN1 | 11 |
| Motor 2 IN2 | 12 |

---

## Working Principle
- Control commands are sent from a **mobile application** via Bluetooth.
- The Bluetooth module communicates with Arduino using **serial communication (9600 baud rate)**.
- Arduino reads incoming character commands and interprets them.
- Based on the received command, Arduino controls the motor driver pins to move the car in the desired direction.

---

## System Flow
Mobile App → Bluetooth Module → Arduino → Motor Driver → DC Motors

---

## Control Commands

| Command | Action |
|--------|--------|
| `F` | Move Forward |
| `B` | Move Backward |
| `L` | Turn Left |
| `R` | Turn Right |
| `S` | Stop |
| `I` | Forward Right |
| `G` | Forward Left |
| `J` | Backward Right |
| `H` | Backward Left |

---

## Software & Communication
- Programmed using **Arduino IDE**
- Serial communication at **9600 baud rate**
- Character-based command decoding
- Directional motor control using digital outputs

---

## How to Operate
1. Assemble the circuit and connect motors and Bluetooth module.
2. Upload the Arduino code to the board.
3. Pair the mobile phone with the Bluetooth module.
4. Open a Bluetooth control app.
5. Send control commands (`F`, `B`, `L`, `R`, etc.).
6. The robotic car moves according to the received command.

---

## Learning Outcomes
- Understanding serial communication in embedded systems
- Interfacing Bluetooth modules with Arduino
- Direction control of DC motors using motor drivers
- Real-time wireless control of robotic systems

---

## Limitations
- No speed control (PWM not implemented)
- Communication range limited by Bluetooth
- No obstacle detection

---

## Future Enhancements
- Add PWM-based speed control
- Implement obstacle avoidance using sensors
- Develop a custom Android application
- Integrate voice control

---

## Author
**Neeraj Kumar Bairwa**  
B.E. Electronics & Electrical Engineering  
MBM University, Jodhpur
