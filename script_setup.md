# Uploading of scripts to the Arduino Uno


>i **Note** 
>i
>i It's recommend to upload the scripts to the Arduino Uno before connecting it. 


{{BOM}}

Within this section you're going to upload the scripts to the [Arduino Uno](electronic.yml#Arduino_Uno){Qty:1}.


## Source of the code
https://github.com/larkum-lab/airtrack

## Setup of the Arduino Uno 

1. Install the Arduino IDE: Download and install the Arduino IDE from the official Arduino website (https://www.arduino.cc/en/software).
2. Install the Pixy2 Library (download at Pixycam.com; guide on the website).
3. Create a new Arduino sketch: Open the Arduino IDE, and create a new sketch by clicking "File" > "New". 
4. Save the sketch in the project related folder and add the header files: definitions.h, leds.h, mpr.h, sensor.h, acuator.h and pins.h) inside the folder. 
5. Further add the airtrack.ino file in the same folder (a download for an updated airtrack.ino file for PixyCam2 is at the bottom of this page).
6. Connect the Arduino: Connect your Arduino board to your computer by using a USB cable.
7. Select the Arduino board and port: In the Arduino IDE, go to "Tools" > "Board" and select the appropriate Arduino board (e.g., "Arduino Uno"). Then, go to "Tools" > "Port" and select the port corresponding to your connected Arduino board.
8. Compile, check for errors and upload the code to your Arduino board.



## Saving of the output

In the Arduino IDE output section are continuously print outputs while running the experiment. These prints can be saved in a text file to store the experimental data. 

>!! **Warning** 
>!!
>!! Need test of file



>i **Note** 
>i
>i The airtrack.ino file of the Github repository was made for the PixyCam.
>i
>i [Download the updated airtrack.ino for PixyCam2](airtrack.ino.zip){zip, pattern:"*.ino"}


