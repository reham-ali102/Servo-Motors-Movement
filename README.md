# Servo Motors Movement Project using Arduino
This project aims to move six servo motors using an Arduino UNO board to create a walking motion for a robot. The Servo library is used to control the servo motors.

## Required Components
- Arduino UNO board
- Breadboard
- 6 Servo motors
- Jumper wires

## Connections
- Connect servo motor 1 to pin 3 on the Arduino board.
- Connect servo motor 2 to pin 5 on the Arduino board.
- Connect servo motor 3 to pin 6 on the Arduino board.
- Connect servo motor 4 to pin 9 on the Arduino board.
- Connect servo motor 5 to pin 10 on the Arduino board.
- Connect servo motor 6 to pin 11 on the Arduino board.
- Connect the power wires (VCC) from each servo motor to the power line (5V) on the breadboard.
- Connect the ground wires (GND) from each servo motor to the ground line (GND) on the breadboard.

## Code
Use the following code to move the servo motors:

```cpp
#include <Servo.h>

Servo servo1;
Servo servo2;
Servo servo3;
Servo servo4;
Servo servo5;
Servo servo6;

void setup() {
  servo1.attach(3);  // Connect servo 1 to pin 3
  servo2.attach(5);  // Connect servo 2 to pin 5
  servo3.attach(6);  // Connect servo 3 to pin 6
  servo4.attach(9);  // Connect servo 4 to pin 9
  servo5.attach(10); // Connect servo 5 to pin 10
  servo6.attach(11); // Connect servo 6 to pin 11
}

void loop() {
  // Move the servos to create a walking motion for the robot

  // Move servo 1 and 4 to 90 degrees
  servo1.write(90);
  servo4.write(90);
  delay(500);  // Wait for half a second

  // Move servo 2 and 5 to 45 degrees
  servo2.write(45);
  servo5.write(45);
  delay(500);  // Wait for half a second

  // Move servo 3 and 6 to 135 degrees
  servo3.write(135);
  servo6.write(135);
  delay(500);  // Wait for half a second

  // Return servos to original positions
  servo1.write(0);
  servo2.write(0);
  servo3.write(0);
  servo4.write(0);
  servo5.write(0);
  servo6.write(0);

  delay(1000);  // Wait for 1 second
}
```

## Simulation on Tinkercad
1. Create an account on Tinkercad or log in if you already have an account.
2. Click on "Circuits" from the side menu.
3. Click on "Create new Circuit".
4. Add the components and connect them as shown in the image.
5. Copy the code above into the code editor in Tinkercad.
6. Click on "Start Simulation" to run the simulation.

## Contributors
- **Reham Ali** - Main Developer

## Images
Here is an image showing the connections used in the project:
![Project Connections](https://github.com/reham-ali102/Servo-Motors-Movement/blob/main/Servo-Moving.PNG)
![Project Connections](https://github.com/reham-ali102/Servo-Motors-Movement/blob/main/servo.PNG)
```

