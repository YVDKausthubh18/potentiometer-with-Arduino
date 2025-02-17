 Potentiometer with Arduino

Overview
This project demonstrates how to control the brightness of an LED using a potentiometer (analog sensor) with an Arduino. The potentiometer’s value is read by the Arduino and mapped to control the brightness of an LED. The values are also displayed in the Serial Monitor.

 Components Required
- Arduino Board (e.g., Arduino Uno)
- LED (connected to pin 3)
- Potentiometer (connected to analog pin A0)
- Resistor (220 ohm for the LED)
- Breadboard and Jumper Wires

 Wiring Diagram
- LED: The anode (longer leg) is connected to pin 3, and the cathode (shorter leg) is connected to ground through a 220-ohm resistor.
- Potentiometer: One end is connected to 5V, the other end to ground, and the middle pin (wiper) is connected to analog pin A0 on the Arduino.

Working Principle
- The potentiometer's value is read using the `analogRead()` function, which returns values between 0 and 1023.
- The `map()` function is used to scale the potentiometer’s value to a range that suits the LED brightness (1 to 255).
- The LED’s brightness is controlled with `analogWrite()`, which varies the voltage to the LED based on the potentiometer’s value.
- The sensor value and corresponding LED brightness are printed to the Serial Monitor.

How to Use
1. Connect the components according to the wiring diagram.
2. Upload the code to your Arduino board using the Arduino IDE.
3. Open the Serial Monitor to view the potentiometer value and LED brightness.
4. Adjust the potentiometer to see the LED brightness change accordingly.

Conclusion
This simple project is an introduction to reading analog sensors and controlling outputs based on the sensor's value using Arduino. You can use this setup as the foundation for more complex projects that involve sensor input and output control.
