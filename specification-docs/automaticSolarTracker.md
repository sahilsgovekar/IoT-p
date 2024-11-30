# Solar Tracking System Using Arduino

## Description

The **Solar Tracking System** is an IoT-based project designed to enhance the efficiency of solar panels by aligning them with the sun's position throughout the day. By utilizing an Arduino UNO, a servo motor, and LDR sensors, the system automatically adjusts the solar panel to capture maximum sunlight, optimizing energy collection.


## Components Used

- **Arduino UNO**: 
- **Small Solar Panel**: 
- **Servo Motor**: Rotates the solar panel to align with sunlight.
- **Two LDR Sensors**: Detect the intensity of sunlight on each side of the panel.
- **Male-to-Male Jumper Wires (10)**: Establish electrical connections.
- **9V Battery**: Provides power to the system.
- **9V Battery Cap**: Connects the 9V battery to the power circuit.
- **Power Jack**: Connects the battery to the Arduino.

## System Design

### Working Principle

1. **Sunlight Detection**: 
   - Two LDR sensors are positioned on opposite sides of the solar panel.
   - The sensors measure sunlight intensity and send the data to the Arduino.

2. **Signal Processing**: 
   - The Arduino UNO reads the analog signals from the LDR sensors.
   - It compares the readings to determine the direction of the sun.

3. **Servo Motor Control**: 
   - Based on the difference in sensor readings, the Arduino adjusts the servo motor to rotate the panel toward the brighter light source.

4. **Continuous Tracking**: 
   - The process repeats at regular intervals to ensure the panel stays aligned with the sun as it moves.


### Software Design

The Arduino sketch includes:
- Reading LDR values from analog pins.
- Calculating the difference in light intensity between the two sensors.
- Sending a PWM signal to control the servo motor.
- A loop function for continuous tracking.

---

This project is a basic demonstration of a solar tracking system, showcasing how IoT and automation can significantly improve the efficiency of solar energy collection. Perfect for beginners in Arduino and IoT!

