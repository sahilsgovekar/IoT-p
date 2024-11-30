# Smart Notice Board Using GSM Module

## Description
The **Smart Notice Board** is an innovative project that uses an Arduino microcontroller and a GSM module to create a digital notice board controlled via SMS. The system allows users to send text messages from their mobile phones, which are then displayed on an LCD screen connected to the Arduino. This project is ideal for schools, offices, or any environment where quick updates are needed, eliminating the need for manual updates.

---

## Components Required
1. **Arduino Uno** - Microcontroller for processing data.
2. **GSM Module** (e.g., SIM800L or SIM900A) - To receive SMS from mobile devices.
3. **16x2 LCD Display** (with I2C module) - To display the received text messages.
4. **I2C Module** (optional) - For simplified LCD interfacing.
5. **SIM Card** - Activated, with SMS functionality.
6. **10kΩ Potentiometer** (optional) - For adjusting the LCD contrast if I2C is not used.
7. **Breadboard** - For prototyping the circuit.
8. **Connecting Wires** - For connections between components.
9. **Power Supply** - 5V adapter or USB cable to power the Arduino.
10. **Resistors** - 220Ω for the LCD backlight (optional).

---

## System Design

### **Architecture**
1. **Input**:
   - SMS is sent from a mobile phone to the GSM module.
   - The GSM module receives and forwards the message to the Arduino.
   
2. **Processing**:
   - The Arduino extracts the text message from the GSM data.
   - It parses the message and prepares it for display.

3. **Output**:
   - The 16x2 LCD displays the received text.

---

## Features
- **Mobile Controlled**: Update messages on the notice board via SMS.
- **Easy Setup**: Simple connections and minimal components.
- **Real-Time Updates**: Displays messages instantly upon receiving SMS.

---

## Use Cases
- School or college notice boards.
- Office announcements.
- Event updates in public spaces.
