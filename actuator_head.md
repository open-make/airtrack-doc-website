# Construction of the linear actuator front


## Preparation: 3D prints {pagestep}

- Print all following parts, some need to be printed twice.


### Core components
![](models/rewards_center_01.stl){color: grey}
![](models/rewards_center_02.stl){color: grey}

### Moveable needle hold (2x)
![](models/rewards_moveable_needle_hold.stl){color: grey}

### Needle fixation (2x)
![](models/rewards_needle_fixation.stl){color: grey}




### Print settings

Print settings used for testing with a good result at a Creality Ender-3 V2

- Layer height: 0.12 mm
- Infill: 70%
- Nuzzle temperatur: 200°C
- Support: Yes, automatic from PrusaSlicer
- Raft: No

### After printing

- Use sandpaper to smooth both parts of the ball joint.
- Clean the holes inside the parts from blocking print artifacts, e.g. with a small drill.




### An overview of all combined 3D printed parts

![](models/rewards_all.stl){color: grey}




## Combine the 3D prints

Use the overview as an orientation. 

- Use a [M2 screw](screws.yml#m2x16mm_screw){Qty: 1} and a [M2 hexagon nuts](screws.yml#m2_hexagon_nuts){Qty: 1} to combine both core parts. 

    - Before tighten the screw place both moveable needle holds with the ball inside. These should point sidewards and not to the front as shown in the file.

    - Remember to loosen the screws before repositioning the moveable needle holds.



>i Note
>i
>i If the movable needle hold is to unstable for your purposes, at the bottom this page are the two ending parts of the movable needle hold which can be combined by a long M2 screw with a small head.



## Attaching at the Linear actuator {pagestep}


- Use a [M2 screw](screws.yml#m2x16mm_screw){Qty: 1} and a [M2 hexagon nuts](screws.yml#m2_hexagon_nuts){Qty: 1} to combine the 3D printed component to the [linear actuator](electronic.yml#LinActuator50mm). 
    - The screw needs to go through the hole in the bigger core 3D part and the front hole of the moveable part of the linear actuator.

>! Picture


- Choose one long side of the U-formation framework and drill a [1/4" thread]


## Appendix - moveable needle hold parts:


![](models/rewards_mnh_end_01001.stl){color: grey}
![](models/rewards_mnh_end_02001.stl){color: grey}



