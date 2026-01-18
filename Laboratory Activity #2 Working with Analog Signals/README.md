This laboratory activity demonstrates how an Arduino can control the brightness of multiple LEDs using a potentiometer. The activity focuses on reading analog input values and using them to adjust LED brightness through pulse-width modulation (PWM).

The objectives of this activity are to:
- Read analog input from a potentiometer
- Control LED brightness using PWM
- Apply looping structures in Arduino programming
- Understand the relationship between input values and output brightness

In this activity, a potentiometer is connected to the Arduino’s analog input pin to serve as a brightness control. The Arduino reads the potentiometer value and maps it to a range suitable for controlling LED brightness. Five LEDs connected to digital pins are then turned ON one by one, gradually increasing their brightness based on the potentiometer setting.

After all LEDs are turned ON, the program gradually turns them OFF one by one by decreasing their brightness. Delays are added so that the changes in brightness and LED sequence can be clearly observed. The brightness level of the LEDs changes as the potentiometer is adjusted, allowing the user to interact with the system in real time.

Code Explanation
- The setup() function uses a while loop to set all LED pins as OUTPUT.
- The loop() function reads the potentiometer value using analogRead() and converts it to a usable brightness range using the map() function. The LEDs are then turned ON one at a time with gradually increasing brightness. Afterward, the LEDs are turned OFF one by one by gradually decreasing their brightness. The process repeats continuously.

Hardware Components Used
- Arduino board
- LEDs (5 pieces)
- Potentiometer
- Resistors
- Breadboard
- USB cable
