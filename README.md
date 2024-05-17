```markdown
# Colour-Based Product Sorting

In today's fast-paced manufacturing environments, efficient sorting of products is crucial for streamlined operations. Manual sorting methods are not only time-consuming but also prone to errors, leading to inefficiencies in production lines. To address this challenge, this project introduces an innovative solution. By harnessing IoT technology and servo motors, the system accurately identifies the color of objects and efficiently directs them to their designated bins. Real-time monitoring capabilities further enhance control and oversight, ensuring seamless integration into production lines.

## Hardware and Software Required:
- NodeMCU ESP8266 
- TCS3200 Colour Sensor 
- Servo Motor 
- Jumper Wires
- Cardboard
- USB cable for power
- ThingSpeak
- Arduino IDE

## Procedure:

### ThingSpeak Channel Setup:
1. Create an account on ThingSpeak ([ThingSpeak](https://thingspeak.com)).
2. Establish a new channel and designate fields:
   - One field for colour data 
   - Another field for object count 

### Hardware Assembly:
1. Following the TCS3200 colour sensor's datasheet, connect it to the ESP8266 board.
2. Connect the two servo motors to the ESP8266 according to their respective specifications.
3. Construct a sorting mechanism using cardboard. This entails designing a path for objects to travel and designated chutes or compartments for sorted colours.

### ESP8266 Code Development:
1. Employ the Arduino IDE to write code for the ESP8266.
2. The code must incorporate libraries for the colour sensor and servo motors.
3. The program should follow this general structure:
   - Read colour data from the sensor.
   - Analyze sensor readings to identify the colour.
   - Control the servo motors to move the sorting mechanism based on the detected colour, directing the object to the designated chute.
   - Transmit the detected colour and a count of 1 to the ThingSpeak channel via the WiFi connection.

### Code Upload and System Testing:
1. Upload the developed code to ESP8266 board.
2. Test the system functionality by placing objects of various colours on the sorting path.
3. Observe the sorted objects and monitor the ThingSpeak channel to verify the accuracy of colour data and count updates.

### Hardware and Software Output:
Once the code and hardware are ready, set up the colour sorting mechanism and mount both the servo motors and colour sensor. Now upload the code to the NodeMCU-ESP8266 board, and the setup is ready to sort the balls of different colours. The number of products for each colour will be displayed on ThingSpeak.

## Result:
The automation introduced by the IoT-based Colour Sorting Machine simplified object sorting based on colour. Using the TCS3200 Colour Sensor and servo motors, objects were efficiently directed into respective bins, reducing manual efforts. This automation not only saved time but also improved accuracy, minimizing human error. Integration with ThingSpeak allowed real-time monitoring of sorting progress, facilitating informed decision-making. Overall, the system streamlined operations, enhancing efficiency and reducing labor costs in manufacturing or industrial settings.
```
