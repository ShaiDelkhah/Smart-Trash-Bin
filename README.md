# Smart-Trash-Bin
I created a fully automatic smart trash can that has the ability to open and close its lid autonomously using an Elegoo Uno R3 (Arduino compatible), an Ultrasonic Distance Sensor (HC-SR04), an LED, a Servo Motor, and a couple jumper wires. 

## How it works:
The design uses the Elegoo Uno R3 as the microcontroller, allowing everything to function properly. When the distance sensor detects an object within 20 centimeters, it sends high voltage to the LED pin, lighting it up. Meanwhile, the Servo Motor stays still until the lED is lit. If the LED is lit, then the Servo Motor will rotate 80 degrees, opening the trash can's lid. Once the object moves outside of the 20 centimeters range, then a one second delay will be applied, and the LED will turn off, rotating the Servo Motor back to its original position. 
