Concept Notes 2.
=======
February 2016

Since the Hammod enclosure depth rating failed a new housing must be found. These should ideally be rated to a depth of at least 10 meters. 

Blue Robotics creates a series of PVC tubes designed specfically for ROVs. These could be used. However the largest tube is only 4" (101mm) in diameter. This is too small for any SLA Battery, meaning power will have to be provided from the shore via a tether. This will require analysis into how much power the system draws and the acceptable power loss. Cost might also be a factor.

There are 2 possible layouts. These are pictured in ROSV_Arch_Idea1 & ROSV_Arch_Idea2.
In both designs the USB Camera could be mounted on a PCB covered in LEDs for lighting. This might be easier than trying to mount external bulbs on the frame.

ROSV_Arch_Idea1
-----------
This design used 2 tubes to house the electronics. One tube houses the sensors, SBC & camera. The other houses power circuitry and motor controllers. This design would use 2x 3" pipes. Each pipe can have a clear end plate, or one with 7 or 4 holes. One plate has to be clear for the camera, which leaves a max of 21 holes in total. Some of these will be used to move power & data beween the 2 tubes, some will be for things like sensors & vacuum seals.

The extra size could be used to hold bulk capacitance, useful for suppling the system during large transients like starting multiple thrusters. However bulk capacitance brings it's own problems.

ROSV_Arch_Idea2
-----------
This design houses everything in a single 4" tube. Some quick sketches suggest that everything can fit in this tube. This is a simpler and cleaner design than Idea1. It uses a single PCB, with a single Micro & single USB port, while the other design uses at least 2. With the wider tube comes an end plate with more holes. This design can have a max of 10 holes. The main problem with this design is the number of cable penetrators required. With out futher information there are a few unknowns. For this to work each penetrator must hold 4 thruster cables. If that is not possible then this design is unfeasable.

 1. Vacuum Seal
 2. Supply In +
 3. Supply In -
 4. NC
 5. Ethernet
 6. Depth Sensor
 7. TC 1 + 2
 8. TC 3 + 4
 9. TC 5 + 6
10. TC 7 + 8


Conclusion
-----------
Idea1 is large and not ideal. It adds significant complexity to the design (cables running back and forth). However it's largest advantage is the space available, and the number of holes for cables. Some of the cable sizes are currenty unknown/undecided. This layout means there are ample holes left over for changes in circumstances or future expansion if required. Quick calculations show that 2x 3" are more buoyant than 1x 4" tube. This Idea1 will require more ballast to make it sink.
Idea2 is prefered if possible, but this design is hinged on fitting 4 cables per penetrator. This will have to be investigated. 
