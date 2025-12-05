# 254-project
Our team will be using Arduino to create a functioning (small) garage door that has recognition software built in to detect an automated car. We will be using Arduino uno and a small servo motor. along with a pre built car.  

the 4 main steps to this prject are listed below. I have highlighted what I did.

1. Hardware Assembly
We built a compact demo door using a small DC motor mounted to wooded rod. the woden rod spun a string that open the door (plywood). The motor is driven by an Arduino Uno (see wiring diagram). We then mounted a small camara to the door.

2. TensorFlow
We made a TensorFlow object detection model. The model continuously watches the camera and sees the car we used. Once the model detects the car, VS code send a command to the Arduino to activate the door.

3. Arduino Motor Control
The Arduino was programmed to listen for “1” (open) command over USB serial. When an “1” command is received, the motor lifts the demo door. 


4. Testing

After wiring and programming, the VS code and Arduino were fully combined. During testing, the camera successfully used the TensorFlow model, which sent commands to the Arduino. The door moved consistently to detections, completing the AIassisted garage.
