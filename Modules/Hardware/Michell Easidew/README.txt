The Michell Easidew LabVIEW class provides a readout of the dew point supplied to a 
Michell Instruments Easidew hygrometer.

The RS232 protocol is used to provide readout of the hygromter, as outlined in Appendix C
of the Easidew manual. The readout command is outlined in "RS232 Commands.pdf".

The Test.vi provides a test program to check functionality of your device.

The dew point in Celcius or Fahrenheit, as set on the Easidew display, are read out.
From this value the relative humidity is derived assuming that the gas has a standard
laboratory temperature of 20 degrees Celcius. The Arden Bruk equation relating the relative
humidity at a certain temperature to the dew point has been inverted to obtain the relative
humidity in function of the dew point at 20 degrees Celcius. This inversion leeds to a simple
relationship and has been derived in Mathematica. 

Code functionality tested on 6 September 2013.

Pieter De Beule
International Iberian Nanotechnology Laboratory
6 September 2013