# Arduino code guide

The provided code handles a complex workflow. It tracks the position of the mouse and provides positional feedback and rewards. This process requires several external components which are set up at the start of the script. If errors arise, it's most likely within this section. 

For debugging you need to implement several print messages and check which get outputted and which not.

-  Code example for printing: Serial.print("Start sensor setup  ");




### Capacitive sensor MPR121  {pagestep}

- To test the functionality of the MPR121 use the test.ino provided in the Github repository 

- https://github.com/adafruit/Adafruit_MPR121/blob/master/examples/MPR121test/MPR121test.ino

- Depending on your wiring the MPR121 will register more or less contacts. You might need to change the thresholds.
    - These values can be found in the definitions.h file starting with line 97


### Test Pixycam2 {pagestep}

- To test the Pixycam2 select within the Arduino IDE file -> examples -> Pixy2 -> ccc_hello_world

- The program permanently prints if it detects a specified object and includes the parameters


### Adjust pixel values in code {pagestep}

Depending on the position of your camera you need to adjust the pixel values for the tracked platform in the code.

- The minimal and maximal x and y values specify the pixels in the camera view where the center of the platform is if the mouse is in a lane.
    - These values can be found in the definitions.h file starting with line 111

- Use the "ccc_hello_world" to determine pixel values of the area 


### Linear actuator {pagestep}

- The airtrack code Github repository contains a linear actuator moving file which also can be used to test it

- The default mode of the code is to pull

