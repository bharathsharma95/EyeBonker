# EyeBonker
Screws up eyes of an intruder (safely of course)

* Inputs:- Passive Infrared Sensors at 9 columns in the basement, preferrably covering most area
* Outputs:- Strobe style light effect with LEDs in zones associated to those columns we mentioned
* 8 Narrow field PIR sensors to cover the peripheri of the house
* 5 Wide angle(>=120 degrees) Sensors covering most interior parts of the basement

## System Design
Peripheral sensors shall be polled for every 50ms (or perhaps a tunable knob so that this can be changed later), to save power
Once there is movement detected at a certain edge, power is turned ON for those wide angle sensors in the same region as the edge sensors
If there is movement registered here too (which shall be a flag that will be set) (to be reset after 1 minute - configurable time)
Lights shall be powered ON in all the regions with a strobe pattern

![image](https://user-images.githubusercontent.com/32398444/183305303-505bcefe-ba3c-4933-b11e-8d104cc2444b.png)
