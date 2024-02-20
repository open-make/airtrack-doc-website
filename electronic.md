# Set up of the electric system

{{BOM}}

## Wiring of devices {pagestep}

- In order to connect the devices you need a circuit board, e.g. this [circuit board](electronic.yml#circuit_board){Qty:1}. 

- Further you need many jumper wires to set up connections accordingly to the following circuit drawing. You need male, female and ordinary wires. 

- To clean up the pathing of cables you can use cable ties like, e.g. these [cable ties](connectors.yml#cable_tie){Qty:many} and fixate with that the cables at the [aluminium strut profile](framework.yml#20x20Rod).

-  You can use a large breadboard to keep a structure between the [Arduino Uno](electronic.yml#Arduino_Uno), [capacitive sensor mpr121](electronic.yml#mpr121){Qty:1}, [Active Buzzer](electronic.yml#Keyes_KY-012){Qty:1} and [H bridge L293D](electronic.yml#L293D){Qty:1}.

#### Wiring configuration
![](images/arduino_schematic.png)


### Component informations:


### [Linear actuator](electronic.yml#LinActuator50mm):

- Orange – Feedback Potentiometer negative reference rail

- Purple – Feedback Potentiometer wiper

- Red – Motor V+ (6V or 12V)

- Black – Motor V- (Ground)

- Yellow – Feedback Potentiometer positive reference rail




## [Capacitive sensor MPR121](electronic.yml#mpr121)  {pagestep}

The left and right sensor in the circuit diagram is meant to be a electrically conductive wire which is attached to each needle.

- The wire needs to be wrapped around the needle multiple times
    - For small changes in the placement of the wire the threshold of the Mpr121 needs to be adjusted. The margin of tolerance is small.



## Not required parts of wiring configuration {pagestep}

The buzzer and LED in the wiring configuration are components of the first use case and may not be required for your set up. 
Because the provided code is also from the first use case, both components still get mentioned here. 


>! **To do ** 
>!
>! SPI cable for pixy - more flexible connecting
