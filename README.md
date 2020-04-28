# Micro-Servo-Control-using-Arduino

In this tutorial we will design a Arduino Uno Micro Servo Control. This is a very basic project. Arduino Uno is programmed to control servo motors. This project will be very useful for beginners. 

**Components Required:**
* Arduino Uno
* Servo Motor (SG 90 – 4 pieces)
* Jumper wires
* Bread Board
* 9V Battery

**Servo Motors:**

  First we talk a bit about Servo Motors. Servo Motors are excessively used when there is a need for accurate shaft movement or position. These are not proposed for high speed applications. Servo motors are proposed for low speed, medium torque and accurate position application. These motors can also be used for designing robotic arm.
	
  Servo motors are available of different sizes and shapes. We are going to use small servo motors, here we have used four SG90 servos. A servo motors will have mainly three wires. One is for positive voltage, another is for ground and last one is for position setting. The Black/Brown wire is connected to ground, Red wire is connected to power and Orange/Yellow wire is connected to signal. In Arduino we have predefined libraries to control the Servo, so it is easy to control servo, which you will learn along with this tutorial.

**Connections:**
* The external battery VCC / GND connects to the breadboard.
*	The Arduino GND connects to the breadboard’s GND input.
*	The servo connections we use in this project are as follows:

       - Orange/Yellow Input – Signal Input
       - Red Input – Power Input (VCC)
       - Brown/Black Input – Ground Input

*	The Servo1 VCC and GND connects to the breadboard’s VCC and GND inputs
*	The Servo1 Signal connects to the Arduino Digital PWM 3
*	The Servo2 VCC and GND connects to the breadboard’s VCC and GND inputs
*	The Servo2 Signal connects to the Arduino Digital PWM 5
*	The Servo3 VCC and GND connects to the breadboard’s VCC and GND inputs
*	The Servo3 Signal connects to the Arduino Digital PWM 6
*	The Servo4 VCC and GND connects to the breadboard’s VCC and GND inputs
*	The Servo4 Signal connects to the Arduino Digital PWM 9

And here your connections are complete.



Now let’s talk about the Servo. Arduino Uno has a feature which enables us to control the servo position just giving the degree value. Say if we want the servo to be at 30, we can directly represent the value in the program. The Servo header (Servo.h) file takes care of all the duty ratio calculations internally. 

```c
#include <Servo.h>
servo servo1;
servo1.attach(3);
servo1.write(degrees);
```

Here first statement represents the header file for controlling the servo motor. Second statement is naming the servo; we leave it as servo1 as we are going to use four motors. Third statement states where the servo signal pin is connected; this must be a PWM pin. Here we are using PIN3 for first servo. Fourth statement gives command for positioning servo motor in degrees. If it is given 30, the servo motor rotates 30 degrees. 

This is how we have controlled the Servos. Check the full code bellow.

**Code:**
**1) If you want your motors to rotate continuously:**

    Please refer servo_continuous file.
    
**2) If you want your motors to run it only once:**

    Please refer servo_once file.

**Video:**

[Micro Servo Control using Arduino Uno Board](https://www.youtube.com/watch?v=M6smHSJ1RP4&t=1s)

You see the connections, code and the output in the video attached.


***HAPPY LEARNING!!***
