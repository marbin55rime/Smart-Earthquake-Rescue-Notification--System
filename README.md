Prototype

A low-cost Arduino Uno prototype that detects earthquake shaking with an MPU6050, then scans three zones (PIR, sound and temperature sensors) for one minute and shows which zone to search first on a 16x2 LCD.

Course: CSE360: Computer Interfacing, BRAC University | Group: 02 | Section: 10

How it works
Normal: green LED, monitoring for shaking.
Warning: first shake, yellow LED and one beep.
Alert: second shake, red LED and 5 beeps, then a 60-second scan of all three zones.
Result: 2 beeps, and the LCD shows Zone X Priority with the Temp/PIR/Sound breakdown.

Each zone scores +1 for PIR motion, +1 for sound and -1 for heat. The highest score wins. A push button resets the system.

Hardware

Arduino Uno, MPU6050, 3x PIR, 3x sound sensor, 3x temperature sensor, 16x2 I2C LCD, 3 LEDs, active buzzer, push button, breadboards, 2 batteries.
