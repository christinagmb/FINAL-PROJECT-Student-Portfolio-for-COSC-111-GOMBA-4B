This laboratory activity demonstrates how an Arduino can control multiple LEDs using both physical buttons and a web-based API. The activity focuses on turning LEDs ON and OFF individually or all at once, using button presses and HTTP requests sent through a FastAPI server.

The objectives of this activity are to:
- Control multiple LEDs using physical buttons
- Control LEDs remotely using a web API
- Understand serial communication between Arduino and a computer
- Learn how software and hardware can work together in real time

In this activity, three LEDs (red, green, and blue) are connected to the Arduino along with three push buttons. When a button is pressed, the Arduino toggles the corresponding LED and sends a status message via the serial port. The Arduino also listens for commands from a Python program running FastAPI. Users can send HTTP requests to toggle individual LEDs or turn all LEDs ON or OFF, and the Arduino responds accordingly. This demonstrates both local (button) and remote (web API) control of hardware.

Code Explanation
- The Arduino program sets up the LED pins as OUTPUT and button pins as INPUT_PULLUP.
- The loop() function calls two main functions:
	- handleSerialInput() reads commands from the serial port to toggle individual LEDs or turn all LEDs ON/OFF.
	- handleButtons() detects button presses and toggles the corresponding LED while sending a status message over serial.
- The FastAPI Python program runs a web server that allows users to send HTTP GET requests to toggle LEDs or control all LEDs. The server communicates with the Arduino via the serial port by sending the correct commands.

Hardware Components Used
- Arduino board
- LEDs (Red, Green, Blue)
- Push buttons
- Resistors
- Breadboard
- USB cable
