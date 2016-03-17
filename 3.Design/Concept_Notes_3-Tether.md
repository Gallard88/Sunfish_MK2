Concept Notes 3.
=======
March 2016

Tether
-----------

An important part of this design is the tether. This is the cable that carries the power down to the ROV. I have run a number of simulations and crunched numbers to try and determine just how large this cable needs to be. The trade offs are as follows:
A larger cable has fewer losses and is more effecient, especially under load. It is more expensive though.
It is however heavier meaning more power is required to pull it. I may need to add float, or something similar in order to try and make the cable neutrally buoyant.

Size
-----------
Without detailed power analysis it's hard to know how much current the system will draw. The worst case estimate is all motors starting at once (which is very unlikely) drawing around 25A. With some clever software a motor might be able to be softstarted reducing the peak current. Alternatively a motor takes around 15-30ms to start. Thrusters could be staggered slightly so the peaks are not cumlative.

The second factor is the static load, i.e. the SBC, microcontroller, LEDs, etc. This is a mostly unchanging load that is contant. I have estimated 5A for my calculations although this is greatly overestimated. This too could be tuned and decreased. uC Sleep modes and power tuning in Linux could reduce this number. 

Working with these details I have determined that I need a cable between 8  & 12 guage. Any larger than 8 and the cable diameter increases past 6mm, meaning it won't fit through a cable penetrator. 8 may or maynot fit. It is normally less than 6, but not by much (5.5) This may make it difficult to pot correctly.

Sourcing
-----------
So far Digi-Key has he best selection. I can purchase a 30.5m (1000') roll of wire for around $100AUD. That's 200 dollar for both power & ground. 

E-Bay has a surprising selection. I have found 8 & 10 Guage cable for around half the price of similar offerings from Digi-Key. I am aware that Digi-Key has larger profit margin than an E-Bay seller but I am not convinced that this may be too good to be true. This may require further investigation later on.

Ethernet
-----------
In addition to power this cable will also carry Ethernet. This will be a standard CAT 5e or 6 cable. The standard dictated a max cable length of 90m which puts a limit on the total length unless other options like fiber optics are considered. At present Fiber is considered too difficult, too exotic and too expensive.

Length
-----------
The final parameter is the cable length. As mentioned above there is a hard limit at 90m. However this much cable becomes very expensive (~$1k). 30m appears to be a nice trade off. There are 30m CAt 5e/6 cable easily available. There are also 30.5m (1000') rolls of wire. 


Conclusion
-----------
The tether will consist of a CAT5e or 6 Ethernet cable & 2 conductors carrying power.
The tether length will be 30m.
The power cables will be 8 - 12 AWG.
