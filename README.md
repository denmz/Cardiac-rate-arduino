# Cardiac-rate-arduino
A cardiac rate made for arduino with a programing base on C++


Here is the full description:

Heart Rate Monitoring System with Arduino and KY-039 Sensor
This project presents the design and implementation of a heart rate monitoring system using low-cost electronic components. The system is built around an Arduino Uno microcontroller, a KY-039 optical pulse sensor, and a 16x2 LCD display with an I2C communication module connected through pins A4 (SDA) and A5 (SCL).
The KY-039 sensor works by emitting infrared light through the fingertip and detecting the variation in light intensity caused by blood flow with each heartbeat. This analog signal is read by the Arduino through pin A0, and when the signal exceeds a defined threshold value, the system identifies a heartbeat and calculates the beats per minute (BPM) by measuring the elapsed time between consecutive beats using the formula: BPM = 60000 / interval in milliseconds.
To ensure accurate readings, the code implements a beat detection filter that prevents the same heartbeat from being counted multiple times, as well as a valid range filter that only accepts BPM values between 30 and 220, discarding any readings caused by electrical noise or sudden movements. The calculated BPM value is updated in real time on the LCD screen and simultaneously transmitted through the serial port for monitoring on a computer.
This system represents a practical and educational application of analog signal processing, real-time data display, and embedded programming using the Arduino platform, making it suitable for academic projects, biomedical prototyping, and learning purposes in the fields of electronics and health technology.
