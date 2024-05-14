# Electronics part 3: Configuration of the PixyCam 2



The PixyCam needs to be configured in order to work with the scripts on the Arduino. The Pixymon software is able to safe parameters at the PixyCam. 

## Install Pixymon {pagestep}

Download the Pixymon software (at Pixycam.com)

- Set up a connection to the PixyCam via USB from your Computer

- MacOS users need to disable gatekeeper for first time usage

- You might need to choose "Blocks, video" in the drop down menu "View" to see the recording


## Light settings {pagestep}

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


>i **Note** 
>i
>i  It's recommend to watch the video and the block detection while running the experiment
>i
>i  **Reminder**
>i
>i  You must have the camera connected to a PC during the usage.




