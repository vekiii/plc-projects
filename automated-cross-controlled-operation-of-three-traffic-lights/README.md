# PLC – Automated Cross-Controlled Operation of Three Traffic Lights  
### Train, Pedestrian, and Vehicle Signals

## 📌 Project Overview
This project implements a PLC-based system for automated and cross-controlled operation of three traffic signal types: train, pedestrian, and vehicle signals. The system is designed with safety and priority handling in mind, ensuring reliable coordination between all traffic participants.

---

## 🔌 Inputs and Outputs

### Inputs
- Train arrival detection switch
- System stop and restart switch

### Outputs
- End-of-cycle indicator
- Train traffic signal
- Pedestrian traffic signals (red and green)
- Vehicle traffic signals (red, yellow, and green)

---

## 🚦 Control Logic and Signal Coordination
- The train signal has the highest priority and activates whenever a train is detected.
- While the train is passing, both pedestrian and vehicle signals are forced into a red state to ensure safe operation.
- Once the train has passed, the system resumes normal traffic control.

Under standard operating conditions:
- Pedestrian and vehicle signals operate alternately.
- When the pedestrian signal is green, the vehicle signal is red, and vice versa.

---

## 🌙 Reduced Operation and Maintenance Mode
- During prolonged cycle repetition or low-traffic periods (e.g., nighttime operation), pedestrian and vehicle signals can be disabled.
- This mode enables system maintenance and reduced power consumption.
- The train signal remains fully operational and can activate at any time, regardless of the status of other signals.

---

## 🧠 PLC Functionality
- Priority-based event handling
- Cross-controlled traffic signal logic
- Manual system stop and restart capability
- Safe state transitions and timing control

---

## 🛠️ Technologies & Tools
- PLC-based control system
- Digital input and output modules
- Timer-based and state-driven control logic

---

## 📄 Notes
This project demonstrates safety-critical PLC control logic for coordinated traffic management with integrated train priority handling.
