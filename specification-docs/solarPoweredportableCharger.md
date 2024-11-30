# Solar-Powered Portable Charger with Battery Storage (IoT Project)

## Description

This project aims to build a **solar-powered portable charger with battery storage**, capable of charging mobile phones using renewable solar energy. The charger utilizes a **solar panel**, **lithium-ion battery**, and **boost converter** to charge a mobile device. Additionally, the system is enhanced with **IoT capabilities**, allowing for remote monitoring of the battery's status through a cloud platform (ThingSpeak, Blynk, or AWS IoT).

By integrating IoT, this system not only charges the phone but also collects and sends real-time data such as battery voltage to a cloud platform for monitoring and analysis. This allows users to keep track of the system's performance and receive alerts for battery status or low energy levels.

---

## Components

### 1. **Solar Panel (5V, 3-6W)**
   - Converts sunlight into electrical energy to charge the battery.
   
### 2. **Lithium-ion Battery (3.7V, 2000mAh or higher)**
   - Stores the energy collected from the solar panel for later use.

### 3. **TP4056 Battery Charging Module**
   - Provides safe charging and discharging protection for the lithium-ion battery.
   
### 4. **Boost Converter (5V Output)**
   - Steps up the battery voltage to 5V, which is suitable for charging mobile phones.
   
### 5. **USB Output Port**
   - Allows users to connect their mobile device and charge it using the stored energy.

### 6. **Microcontroller (ESP32)**
   - Handles the IoT functionality, including Wi-Fi connectivity and sending data to the cloud platform.
   
### 7. **Voltage Sensor**
   - Monitors the battery voltage to ensure it stays within a safe range.

### 8. **Current Sensor (Optional)**
   - Measures the current being drawn by the battery or mobile device (useful for advanced monitoring).
   
### 9. **Wi-Fi Module (Built-in ESP32 - not additional buy)**
   - Enables the microcontroller to connect to the internet for cloud data transmission.

### 11. **Diodes (Schottky Diodes)**
   - Prevent reverse current flow to protect the components.
   
### 12. **Resistors and Capacitors**
   - Used for filtering, stabilizing, and protecting signals in the circuit.

### 13. **Enclosure**
   - A casing to house all the components and protect them from external elements.

---

## System Design

The system consists of multiple interconnected modules that work together to capture solar energy, store it in a battery, charge a phone, and send data to the cloud. Below is a high-level overview of the design:

### **Power Generation and Storage**
1. **Solar Panel**: Captures solar energy and converts it to DC voltage.
2. **TP4056 Charging Module**: Charges the lithium-ion battery safely by managing the input from the solar panel.
3. **Lithium-ion Battery**: Stores the energy collected by the solar panel for later use.
4. **Boost Converter**: Converts the stored 3.7V battery voltage to 5V, which is required for charging mobile phones.

### **IoT Integration**
1. **Microcontroller (ESP32)**: The heart of the IoT system, which connects to Wi-Fi and sends data to the cloud. It communicates with the **voltage sensor** to measure the battery's voltage and relay that information to the cloud platform.
2. **Voltage Sensor**: Monitors the battery voltage to ensure the system works within safe operating limits and helps prevent overcharging or deep discharging.

### **Cloud Platform (e.g., ThingSpeak, Blynk, or AWS IoT)**
   - Stores and displays data from the charger, such as battery voltage and status, in real-time.
   
---


