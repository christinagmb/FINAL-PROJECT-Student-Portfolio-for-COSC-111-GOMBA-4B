This laboratory activity demonstrates how an Arduino can control multiple LEDs using physical buttons and a Python program. The activity focuses on detecting button presses, sending signals over serial communication, and toggling LEDs based on both button input and commands from the computer.

The objectives of this activity are to:
- Detect button presses using digital input pins
- Toggle LEDs ON and OFF based on input
- Use serial communication between Arduino and a computer
- Learn how hardware and software can work together to control devices

In this activity, three LEDs (red, green, and blue) are connected to the Arduino along with three push buttons. When a button is pressed, the Arduino sends a signal to the Python program via the serial port. The Python program receives the signal and sends back a command to the Arduino to toggle the corresponding LED. This allows students to see how pressing a physical button can control a device and how software can interact with hardware in real time.

Code Explanation
- The Arduino program sets up the LED pins as OUTPUT and the button pins as INPUT_PULLUP. The loop() function calls two sub-functions: handleButtons() checks if a button is pressed and sends a corresponding character over serial, and handleSerial() reads incoming serial commands from the Python program to toggle the LEDs. Debouncing is handled with a small delay to avoid multiple triggers from a single press.
- The Python program continuously listens to the serial port for signals from the Arduino. When it receives a signal (R, G, or B), it sends back a command (1, 2, or 3) to toggle the corresponding LED. It also prints messages to indicate which button was pressed and which LED is toggled.

Hardware Components Used
- Arduino board
- LEDs (Red, Green, Blue)
- Push buttons
- Resistors
- Breadboard
- USB cable
