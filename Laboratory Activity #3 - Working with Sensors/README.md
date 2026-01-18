This laboratory activity demonstrates how an Arduino can use multiple sensors to create a simple alert system. The activity focuses on monitoring temperature and light intensity and activating an LED and buzzer when both conditions reach a set limit.

The objectives of this activity are to:
- Read temperature using a thermistor
- Detect light intensity using a photoresistor
- Use conditional statements to trigger an alert
- Control an LED and buzzer using a single output pin

In this activity, a thermistor and a photoresistor are connected to the Arduino to measure temperature and brightness. The Arduino continuously reads the values from both sensors. The temperature value is calculated in degrees Celsius, while the brightness value represents the amount of light detected by the photoresistor.

When the temperature exceeds the set threshold and the brightness level is also high, the Arduino activates an LED and buzzer connected to the same output pin. The LED and buzzer turn ON and OFF repeatedly to act as a warning signal. If either the temperature or brightness is below the threshold, the alert remains OFF.

Code Explanation
- The setup() function sets the LED and buzzer pin as an OUTPUT.
- The loop() function reads the temperature from the thermistor and the brightness from the photoresistor. It then checks if both values exceed their respective thresholds. If the conditions are met, the Arduino blinks the LED and buzzer. Otherwise, the output remains OFF.

Hardware Components Used
- Arduino board
- Thermistor
- Photoresistor
- LED
- Buzzer
- Resistors
- Breadboard
- USB cable
