# Smart-Trash-Bin
I created a fully automatic smart trash can that has the ability to open and close its lid autonomously using an Elegoo Uno R3 (Arduino compatible), an Ultrasonic Distance Sensor (HC-SR04), an LED, a Servo Motor, and a couple jumper wires. 

## How it works:
The design uses the Elegoo Uno R3 as the microcontroller, allowing everything to function properly. When the distance sensor detects an object within 15 centimeters, it sends high voltage to the LED pin, lighting it up. Meanwhile, the Servo Motor stays still until the LED is lit. If the LED is lit, then the Servo Motor will rotate 50 degrees, opening the trash can's lid. Once the object moves outside of the 20 centimeters range, then a one second delay will be applied, and the LED will turn off, rotating the Servo Motor back to its original position. 

## Components used: 
Elegoo Uno R3 (Arduino Compatible)
Breadboard
HC-SR04 Ultrasonic Distance Sensor
Servo Motor
Jumper Wires
1 LED
220 Ohms Resistor 

## The Code
The Code features a C++ language type written on the Arduino IDE software. It uses the LED as a primary indicator for the Servo Motor, using numerous if else statements. The distance sensor's Trigger Pin sends out ultrasonic pulses that help it detect how far an object  The Echo pin then recieves this signal and measures the distance. If a distance is within 15 centimeters, then the LED will turn on. If distance is greater than 15 centimeters, then LED stays off. If the LED is lit, then the servo motor will rotate 50 degrees. If the LED is off, then the servo motor rotates 0 degrees. 

## The Arduino Code for this project can be found below:
See the [full Arduino sketch](./Smart_Trash_Bin/Smart_Trash_Bin.ino)
