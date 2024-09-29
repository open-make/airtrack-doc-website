# Electronics part 2: Uploading of scripts to the Arduino Uno





Within this section you're going to upload the scripts to the [Arduino Uno](electronic.yml#Arduino_Uno).


## Source of the code
https://github.com/open-make/code-airtrack

## Setup of the Arduino Uno 

1. Install the Arduino IDE: Download and install the Arduino IDE from the official Arduino website (https://www.arduino.cc/en/software).
2. Install the Pixy2 Library (download at Pixycam.com; guide on the website).
3. Download the "airtrack" folder from the Github repository
4. Open "airtrack.ino" with the Arduino IDE and the other files inside the folder should automatically open along the airtrack.ino file (definitions.h, leds.h, mpr.h, sensor.h, acuator.h and pins.h). 
5. Connect the Arduino: Connect your Arduino board to your computer by using a USB cable.
6. Select the Arduino board and port: In the Arduino IDE, go to "Tools" > "Board" and select the appropriate Arduino board (e.g., "Arduino Uno"). Then, go to "Tools" > "Port" and select the port corresponding to your connected Arduino board.
7. Compile, check for errors and upload the code to your Arduino board.



## Saving of the output

In the Arduino IDE output section are continuously print outputs in the serial monitor tab while running the experiment. These prints can be saved in a text file to store the experimental data. 


>i **Note** 
>i
>i The scripts for PixyCam1 are also included in the Github


