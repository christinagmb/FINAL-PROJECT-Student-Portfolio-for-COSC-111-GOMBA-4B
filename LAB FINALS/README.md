This laboratory activity demonstrates the integration of a microcontroller with a software application to control a network-based system. It focuses on using a physical push button connected to an Arduino to trigger actions in a remote LED control system through serial communication and a RESTful API.

The objectives of this activity are to:
- Detect user input using a digital push button
- Apply debouncing techniques to ensure reliable input detection
- Transmit data from Arduino to a computer using serial communication
- Trigger an API to control the LED

In this activity, a push button is connected to an Arduino and configured using an internal pull-up resistor. When the button is pressed, the Arduino detects the input change and applies a debounce delay to prevent multiple triggers caused by mechanical noise. Once a valid press is confirmed, the Arduino sends a predefined group number through the serial port.

A Python program running on the computer continuously listens for incoming serial data from the Arduino. Upon receiving the group number, the program validates the data and sends an HTTP request to a specific API endpoint. This endpoint is responsible for toggling the state of an LED group, allowing the physical button press to control LEDs over a network connection.

This activity demonstrates how hardware input devices can be used to interact with software systems and web services, reflecting a common architecture used in Internet of Things (IoT) applications.

Code Explanation
- The Arduino setup() function initializes the button pin and serial communication.
- The loop() function monitors the button state, applies debounce logic, and sends data only when a valid button press occurs.
- The Python script establishes a serial connection and continuously listens for data from the Arduino.
- Once valid input is received, the Python program sends an API request to toggle the assigned LED group.

Hardware Components Used:
- Arduino board
- Push button
- USB cable


