Architecture
=======

The System consists of three basic sub-systems:
* The ROSV
* The Surface Control Station (SCS)
* The Tether.

The entire system is designed to fit into a pelican case (Model: TBA). This is to simplify transport and set up. Each sub-system can be divide further into base components.


Surface Control
----+
    |
    +--+
    |  |
----+  |
       |
       | Ethernet/Power
       | Tether
       |
       |     +---------------+
       |     |  ROSV         |/|
       +-----+               | |
             |               |\|
             +---------------+


The ROSV
-----------
This is the submarine itself. It is designed to dive and provide a realtime video feed.
In this generation the craft will receive power from the surface wia the tether. This is in contrast to the previous generation which contained onboard batteries.
The ROSV contains a number of sensors, thrusters for motion and other actuators.


The Surface Control Station
-----------
The SCS contains the power source for the ROSV. It is also the brains for the LAN. The SCS is designed to provide control for the ROSV craft. It will provide a monitor which can display either the camera feed or other dive related information.


The Tether
-----------
This is a cable(s) the connects the ROSV back to the surface. It provides power and LAN connectivity. 
