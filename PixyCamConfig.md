# Electronics part 3: Configuration of the PixyCam 2





The PixyCam needs to be configured in order to work with the scripts on the Arduino. The Pixymon software is able to safe parameters at the PixyCam. 

## Install Arduino library {pagestep}

To use the PixyCam with the Arduino, you need to download the latest library zip-file and import it in the Arduino IDE via Sketch -> Include Library.

The zip-file for the PixyCam2 can be found at "https://pixycam.com/downloads-pixy2/".

The zip-file for the PixyCam1 can be found at "https://pixycam.com/downloads-pixy1/".



## Install Pixymon {pagestep}

Download the Pixymon software (at Pixycam.com)

- Set up a connection to the PixyCam via USB from your Computer

- MacOS users need to disable gatekeeper for first time usage

- You might need to choose "Blocks, video" in the drop down menu "View" to see the recording

## PixyCam orientation {pagestep}

Once again make sure that the lens of the PixyCam is pointing away from the table side where rewards get provided.


## Light settings {pagestep}


>i **Note** 
>i
>i As experiments most likely are done in the dark, extra light sources are needed. Place the light sources at the side and not below the plexiglass book to minimize reflections for PixyCam detection.


Use the lightning settings in the  "Pixy Parameter" submenu to optimize the visibility in the Pixymon viewer. You need to check what works best at your setup place. A better visibility of objects in the viewer will result in better object detection. 


- Within "Tuning" submenu -> "Camera brightness"

- Several settings in "Camera" submenu

- Maybe you need to adjust light sources as the reflections in the air table contribute to the noise.

- Lowering the frames per second can help in low light situations to reduce noise.

- You can enable "Highlight overexposure" in the Pixymon parameters to show areas with poor image recognition properties. 




## Block detection {pagestep}

- Place the floating platform on the air table. The orientation of the colored rectangle should be parallel or orthogonal to the length of the air table.

- In " Pixy parameters" -> "Expert"
    - Set "Max blocks"  to 2, as you only need to detect two connected blocks. 
    - Set "Default program" to "color connected components"
    

- In the drop down menu "Actions"
    - Select "Set CC signature 1" and "Set CC signature 2" to mark the center area of each color on the floating platform


- In " Pixy parameters" -> "Expert"
    - Play with the "Signature teach threshold" to have the hole object detected but not more than it.

- Afterwards in the Pixymon viewer: A box should be visible around both colors at the bottom side of the platform with a "s" and "phi" value. 

The detection configuration will be saved on the PixyCam and can be used with the Arduino scripts.



## Configuration of coordinates {pagestep}

In the definitions.h you need to specify the y-axis minimum and maximum coordinates of the movement of the platform. Further you need to change the y-axis motor threshold which triggers the motor if the mouse is in the lane. As the mouse moves forwards in a lane, the platform moves to the non reward side of the air table. You need to determine the y-axis value when the mouse is deep enough in the lane.

In definitions.h the PixyCam coordinates for our set up are set to:


- this->y_threshold_min = 45
- this->y_threshold_max = 190
- this->y_motor_threshold = 115




>i **Note** 
>i
>i  It's recommend to watch the video and the block detection while running the experiment
>i
>i  **Reminder**
>i
>i  You must have the camera connected to a PC during the usage.




