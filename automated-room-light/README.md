# PLC – Automated Room Light

## 📌 Project Overview
This project implements a PLC-based system for automated room lighting control based on occupancy detection and ambient light conditions. The system is suitable for spaces such as hallways, garages, storage rooms, or similar environments.

Lighting is controlled using logical conditions derived from motion detection, daylight sensing, and safety mechanisms.

---

## 🚪 Occupancy Detection
The room is assumed to have both entrance and exit doors, each equipped with a PIR (Passive Infrared) motion sensor for detecting movement.

- PIR sensors detect entry and exit events.
- Sensor data is used to determine whether the room is occupied.
- If the room becomes empty, the light turns off automatically after a 10-second delay.
- The delay allows the light to remain on in case of quick re-entry.

For rooms with a single door, PIR sensors can be placed on both sides (entry and exit) to maintain correct occupancy tracking.

---

## 🌙 Day/Night Detection
- A photosensor is used to detect ambient light conditions.
- The lighting system is activated only when nighttime conditions are detected.
- Alternatively, the same functionality can be implemented using a real-time clock (RTC) to control lighting based on predefined time intervals.

---

## 🔐 Safety and Fault Protection
- A relay is integrated as a safety mechanism.
- Under normal operation, the relay remains deactivated, allowing the system to function normally.
- In the event of a detected anomaly or fault, the relay is activated, shutting down the system by disabling the lighting and photosensor.

---

## 🧠 PLC Functionality
- Logical control of lighting based on occupancy and light conditions
- Timed delay handling for light deactivation
- Sensor-based state management
- Safety shutdown using relay logic

---

## 🛠️ Technologies & Tools
- PLC-based control system
- PIR motion sensors
- Photosensor or real-time clock (RTC)
- Relay-based safety circuit

---

## 📄 Notes
This project demonstrates practical PLC logic design for energy-efficient and safe automated lighting systems.
