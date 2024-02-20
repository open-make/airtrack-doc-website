# Configuration of the PixyCam 2

>i **Note** 
>i
>i  It's recommend to: 
>i
>i - Upload the preferences to the PixyCam before connecting it
>i 
>i - Watch the video and the block detection while running the experiment

The PixyCam needs to be configured in order to work with the scripts on the Arduino. The Pixymon software is able to safe parameters at the PixyCam. 

## Install Pixymon {pagestep}

Download the Pixymon software (at Pixycam.com)

- Set up a connection to the PixyCam via USB from your Computer

- MacOS users need to disable gatekeeper for first time usage

- You might need to choose "Blocks, video" in the drop down menu "View" to see the recording


## Light settings {pagestep}

Use the lightning settings in the  "Pixy Parameter" submenu to optimize the visibility in the Pixymon viewer. You need to check what works best at your setup place. 


- Within "Tuning" submenu -> "Camera brightness"

- Several settings in "Camera" submenu


## Block detection {pagestep}

- Place the floating platform on the air table. The orientation of the colored rectangle should be parallel or orthogonal to the length of the air table.

- In " Pixy parameters" -> "Expert"
    - Set "Max blocks"  to 1, as you only need to detect one connected block. 
    - Set "Default program" to "color connected components"

- In the drop down menu "Actions"
    - Select "Set CC signature 1" and "Set CC signature 2" to mark the center area of both colors on the floating platform

- Afterwards should a box be visible around both colors at the bottom side of the platform with a "s" and "phi" value. 

The detection configuration will be saved on the PixyCam and can be used with the Arduino scripts.








