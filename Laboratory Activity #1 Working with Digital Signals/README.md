This laboratory activity demonstrates how an Arduino can control multiple LEDs using digital output pins. The activity focuses on understanding how LEDs can be turned ON and OFF in sequence using loops and timing delays.

The objectives of this activity are to:
- Control multiple LEDs using an Arduino
- Understand how digital output pins work
- Apply looping and timing in Arduino programming
- Observe LED sequencing behavior

In this activity, five LEDs are connected to different digital pins of the Arduino. The Arduino is programmed to turn ON the LEDs one by one with a one-second delay between each LED. After all LEDs are turned ON, the program then turns them OFF one by one using the same delay. This process repeats continuously.

This activity helps students understand how digital signals control output devices and how loops can be used to simplify repetitive tasks in a program.

Code Explanation
- The setup() function sets all the LED pins as OUTPUT so the Arduino can control them.
- The loop() function contains two for loops. The first loop turns ON each LED one at a time with a one-second delay. The second loop turns OFF each LED one at a time, also with a one-second delay. The program runs continuously, creating a repeating LED sequence.

Hardware Components Used
- Arduino board
- LEDs
- Resistors
- Breadboard
- USB cable
