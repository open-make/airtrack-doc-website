# Construction guidance of an Airtrack


This website will guide you through the hole process of building an Airtrack by yourself. This guide is part of the output from the [open.make project](https://www.openmake.de/). This project aims to further establish open hardware in science e.g. by supporting scientist replicating research and providing guides to research hardware. The Airtrack was first published in the paper titled [Air-Track: a real-world floating environment for active sensing in head-fixed mice in Journal of Neurophysiology 1 October 2016 Vol. 116](https://pubmed.ncbi.nlm.nih.gov/27486102/). It was developed within Larkum Lab by Mostafa Nashaat, Hatem Oraby, Robert Sachdev, York Winter and Matthew Larkum as well as Alexander Schill from the Charite Workshop. 
Further Information is provided on the website of the [Airtrack](http://www.neuro-airtrack.com/).




## Table of contents


#### [Construction of the airtable](airtable.md){step}


#### [Construction of the basic framework](basicframework.md){step}


#### [Construction of the head fixation and platform tracking](headandcamera.md){step}


#### [Construction of the rewarding system](rewardsystem.md){step}


#### [Setup of the electronics](electronic.md){step}


#### [List of all necessary components]{BOM}




### About the Airtrack

To investigate the neuronal activities in ordinary behaviour it's eligible to implement modern brain recording equipment. These modern technics frequently require head fixation. The Airtrack is one approach to facilitate analysing natural behaviour in its complexity. Behaviour is depended on permanent sensory feedback from various modalities and to provide the possibility of sensory perception in its totality is a central challenge. The Airtrack aims to facilitate these multiple sensory and motor modality approaches in combination with a simple setup, low costs and less computational processing. The shift from a virtual visual (air ball/ treadmill with VR) to somatosensory modality approach causes a natural tactile representation while having less computational needs besides no errors between perception and movement of the mice and corresponding virtual environment. The virtual environment approaches faces the difficulties of estimating the perceptual experience of the mice or other animals and it's probably impossible to match virtual reality and real world experience. 
The developers conclude that the Airtrack system is ideal for eliciting natural behaviour in concert with virtually any system for monitoring or manipulating brain activity.

The following setup is described in [Air-Track: a real-world floating environment for active sensing in head-fixed mice in Journal of Neurophysiology 1 October 2016 Vol. 116](https://pubmed.ncbi.nlm.nih.gov/27486102/) and is shown in the picture below.
It consists out of a central air table with the possibility of modification. In this version a mouse moves on a floating lightweight plus maze while being head fixed in the center above the platform. Below the table a camera tracks the movement of the plus maze with different coloring on the bottom side and at one side of the table a moveable reward system is placed with two licking spots. To detect with spot was licked a capacitive sensor is used. The Airtrack was used to perform Go/No-Go and two-alternative forced choice tasks with mice. The lanes on the maze are equipped with different features to distinguish them and correspond with the tasks. They can either be smooth or with gratings etched. Further for the performed tasks a LED and buzzer are installed to provide position feedback. The position tracking was done with a Pixy camera (CMUcam5 Image Sensor) by detecting  different colouring on the bottom side of the plus maze. The Pixy camera processes colour information in real time.
The central table consists out of a plexiglass box with air flowing through. On the upper side many holes are placed to create an air cushion on the surface the platform can float on. The table is mounted on aluminium legs to reach the desired height and space for the camera. On the framework is a lot space to place e.g. further tracking devices. The computational tasks are performed with a Arduino Uno microcontroller.

![](airtrack_platform_small.jpg)


Source ???

References: [Nashaat MA, Oraby H, Sachdev RN, Winter Y, Larkum ME. Air-Track: a real-world floating environment for active sensing in head-fixed mice. J Neurophysiol. 116(4):1542-1553, 2016](https://pubmed.ncbi.nlm.nih.gov/27486102/)