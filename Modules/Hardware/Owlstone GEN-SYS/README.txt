Owlstone GEN-SYS LabVIEW Class

Introduction
------------
The Owlstone Vapour Generator Owlstone GEN-SYS consists of modular components such as
* OVG-4: Owlstone Vapour Generator (2 Eurotherm PID controllers)
* OHG-4: Owlstone Humidity Generator (1 Eurotherm PID controller and 1 Michell Easidew humidity
sensor)
* OFC-1: Owlstone Flow Controller

The LabVIEW Owlstone GEN-SYS class is designed to control a GEN-SYS rack with one OVG-4
and one OHG-4 module. For other configurations, the Owlstone GEN-SYS class will need to 
be adjusted to fit the Owlstone GEN-SYS rack configuration.

A serial connection to the humidity sensor of the OHG-4 has been established, as outlined
in the appendix of the Michell Easidew operation manual.


Dependencies
------------
Copy the "Eurotherm 32xx Series" folder, containing the Eurotherm PID controller support
functions to the LabVIEW instr.lib folder.

Run
---
* Open Test.vi
* enter the addresses of the OVG-4 and OHG-4 PID controllers as determined by Owlstone
* enter VISA name for the connection to the GEN-SYS rack (RS-485)
* enter VISA name for the connection to the Michell Easidew
* Press Run

-> Adjusting the different settings of the GEN-SYS results in different gas output parameters.
While the relative humidity is constantly read out. The gas concentration and flow rate are
derived theoretically from the instrument setpoints.

NOTE: depending on the permeation source you will have, you might need to add your own
permeation source specifications to 
a) Permeation Tube Gas.ctl -> Specify gas compound 
b) Set Tube Parameters.ctl -> Specify molecular weight, calibration temperature and calibrated
permeation rate

Pieter De Beule
23 September 2013