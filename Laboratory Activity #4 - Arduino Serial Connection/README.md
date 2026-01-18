This laboratory activity demonstrates how an Arduino can use a photoresistor and serial communication to control the blinking behavior of an LED. The activity focuses on detecting light intensity and allowing the user to stop the LED using a command from the Serial Monitor.

The objectives of this activity are to:
- Measure light intensity using a photoresistor
- Control an LED based on a light threshold
- Use serial input to control program behavior
- Understand basic conditional logic in Arduino

In this activity, a photoresistor is connected to the Arduino to detect the brightness of the surrounding environment. The Arduino reads the light value and converts it into a normalized range. When the brightness reaches or exceeds the set threshold, the LED begins to blink automatically.

The system also allows user interaction through the Serial Monitor. When the user types the command “stop”, the Arduino immediately stops the LED from blinking and turns it OFF. This demonstrates how sensor input and user commands can work together to control an output device.

Code Explanation
- The setup() function initializes serial communication and sets the LED pin as an OUTPUT. It also displays instructions in the Serial Monitor.
- The loop() function continuously reads the brightness value from the photoresistor and checks if it reaches the defined threshold. If the threshold is met, the LED starts blinking. The program also listens for serial input, and when the “stop” command is received, the LED blinking stops.

Hardware Components Used
- Arduino board
- Photoresistor
- LED
- Resistor
- Breadboard
- USB cable
