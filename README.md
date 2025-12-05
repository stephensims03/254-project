# 254-project

the 4 main steps to this prject are listed below. I mainly worked on #1,3, and 4.

1. Hardware Assembly
We built a compact demo door using a small DC motor mounted to wooded rod. the woden rod spun a string that open the door (plywood). The motor is driven by an Arduino Uno (see wiring diagram). We then mounted a small camara to the door.

2. TensorFlow
We made a TensorFlow object detection model. The model continuously watches the camera and sees the car we used. Once the model detects the car, VS code send a command to the Arduino to activate the door.

3. Arduino Motor Control
The Arduino was programmed to listen for “1” (open) command over USB serial. When an “1” command is received, the motor lifts the demo door. 


4. Testing

After wiring and programming, the VS code and Arduino were fully combined. During testing, the camera successfully used the TensorFlow model, which sent commands to the Arduino. The door moved consistently to detections, completing the AIassisted garage.

parts used:
:elego smart car
:Small dc motor
:Ardiuno uno
:tensorflow
:pyserial
:VS code
:Arduino IDE

The most diffucult part of this project was connecting Arduino IDE to the tensorflow model. We had lots of trouble getting the pyserial to work on anyones computer but nolans. 

this is a short video explaning the process of building the garage.

https://youtu.be/ISsgWm5NaLM
