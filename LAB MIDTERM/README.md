This laboratory activity shows how an Arduino can be used to create a simple smart lighting system using a photoresistor. The activity focuses on detecting light intensity from the environment and turning ON LEDs based on the amount of light detected.

The objectives of this activity are to:
- Read light intensity using a photoresistor
- Control LEDs based on light levels
- Switch between manual and automatic modes
- Use serial commands to control the system

In this activity, a photoresistor is connected to the Arduino to sense the surrounding light. The Arduino reads the sensor value and converts it into a percentage. Depending on the light intensity, one of the three LEDs (green, yellow, or red) turns ON to indicate whether the environment is dark, normal, or bright.

The system works in two modes. In manual mode, the LEDs turn ON based on fixed threshold values that can be changed through the Serial Monitor. In automatic mode, the Arduino automatically determines the lighting condition (cloudy, normal, or bright sunlight) and activates the correct LED. The current light intensity, active LED, and mode are displayed in the Serial Monitor.

Code Explanation
- The setup() function sets the LED pins as OUTPUT and the photoresistor as INPUT. It also starts the serial communication so the user can view data and send commands.
- The loop() function continuously reads the light value from the photoresistor and converts it into a percentage. Based on the selected mode, the program turns ON the appropriate LED. It also prints the light intensity and system status to the Serial Monitor.
- The program accepts serial commands to switch between MANUAL and AUTO modes and to adjust the light thresholds in manual mode. This allows the user to interact with and control the system in real time.

Hardware Components Used
- Arduino board
- Photoresistor
- LEDs (Green, Yellow, Red)
- Breadboard
- USB cable
