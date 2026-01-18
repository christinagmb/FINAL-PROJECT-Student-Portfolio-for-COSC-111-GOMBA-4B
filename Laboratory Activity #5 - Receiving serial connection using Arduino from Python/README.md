This laboratory activity demonstrates how an Arduino can control multiple LEDs using both an embedded program and a Python-based serial interface. The activity focuses on using digital output pins to turn LEDs ON and OFF individually or all at once, and shows how a computer can communicate with Arduino through the Serial Monitor.

The objectives of this activity are to:
- Control multiple LEDs individually and collectively
- Use a Python program to send commands to Arduino
- Understand serial communication between Arduino and a computer
- Apply functions and modular programming in Arduino

In this activity, three LEDs (red, green, and yellow) are connected to the Arduino. The Arduino program defines functions to toggle each LED and to turn all LEDs ON or OFF. The program listens for serial commands from the computer and executes the corresponding action. Using the Python interface, the user can type commands to control the LEDs in real time. This allows students to see how software commands can directly control hardware outputs.

Code Explanation
- The Arduino program uses the LedFunctions.h library to define LED pins, track their states, and provide functions to toggle or control all LEDs.
- The setup() function initializes the LED pins as OUTPUT and starts serial communication. The loop() function continuously checks for serial input and executes the appropriate function based on the command received (R, G, Y, A, O).
- The Python program provides a simple menu for the user to type commands. It sends the corresponding command to the Arduino over the serial port, waits briefly, and prints Arduino’s response. This allows the user to interactively control the LEDs from the computer.

Hardware Components Used
- Arduino board
- LEDs (Red, Green, Yellow)
- Resistors
- Breadboard
- USB cable
