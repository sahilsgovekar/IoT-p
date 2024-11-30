# **Smart Parking System**

## **Description**

The **Smart Parking System** is an IoT-based solution designed to optimize parking management by monitoring parking slot availability and controlling access to the parking area. This system utilizes ultrasonic sensors to detect the presence of vehicles, a servo motor to manage the entry gate, and an LCD display to provide real-time information on parking slot occupancy. If all parking slots are filled, the system prevents entry and notifies the user through a buzzer.

---

## **Components**

### **Hardware**
1. **Microcontroller**:
   - Arduino UNO / ESP32 (optional for cloud integration).
2. **Sensors (x no of parking slots required)**:
   - Ultrasonic Sensors (HC-SR04) for detecting vehicle presence.
3. **LCD Display**:
   - 16x2 LCD with I2C module for displaying parking status.
4. **Servo Motor**:
   - For gate control.
5. **Push Button**:
   - To simulate a car requesting entry.
6. **Buzzer**:
   - To alert users when slots are full.
7. **Power Supply**:
   - 5V adapter or battery pack.
8. **Connecting Wires**:
   - Jumper wires for connections.
9. **Breadboard**:
   - For prototyping.
10. **LEDs**:
   - (Optional) For additional visual indication.

### **Software**
1. **Arduino IDE**:
   - Used to write and upload the code to the microcontroller.
2. **Libraries**:
   - `LiquidCrystal_I2C`: For LCD display.
   - `Servo`: For controlling the servo motor.

---

## **System Design**

### **Workflow**
1. **Slot Detection**:
   - Each parking slot is monitored by an ultrasonic sensor that determines if the slot is occupied based on distance measurements.
2. **Display Status**:
   - The 16x2 LCD displays the number of free and occupied slots in real-time.
3. **Gate Control**:
   - A servo motor opens the gate when a car requests entry, provided slots are available.
   - If no slots are available, the gate remains closed, and a buzzer alerts the user.
4. **Entry Request**:
   - A push button simulates a car requesting entry.

### **Logic**
1. If slots are available:
   - The gate opens for a car to enter.
   - The slot status is updated once the car is parked.
2. If no slots are available:
   - The gate remains closed, and the system alerts users via the buzzer and LCD display.

### **System Connections**
- Ultrasonic sensors detect car presence and send data to the microcontroller.
- The LCD and I2C module are used for displaying slot statuses.
- The servo motor is controlled via a signal pin to open and close the gate.
- The buzzer provides audio alerts, and the push button initiates entry requests.

---

## **How to Use**
1. Assemble the components as per the circuit diagram.
2. Upload the provided Arduino code to the microcontroller.
3. Power on the system.
4. View parking status on the LCD display and test the entry process by pressing the push button.

---

## **Future Enhancements**
1. Cloud-based monitoring using ESP32 for remote access to parking data.
2. Integration with mobile apps for slot booking and notifications.
3. Solar-powered design for energy efficiency.
4. Advanced sensors for higher accuracy in detecting vehicles.

---
