INL LabVIEW Repository

0) Installation Guidelines
------------------------------------------------------------------------------------------------------

In order to load the INL LabVIEW repository, one needs to install third party drivers. 
To achieve this, copy the instrumentation drivers located in "INL LabVIEW Repository\3rd Party\*.*"
to "c:\Program Files\National Instruments\LabVIEW 20xx\instr.lib".
This will install the drivers for
1) Standford Research PS300 Series power supply
2) Keithley 24XX power supply
3) Agilent 3458 multimeter
4) NMR Dynamic Link Library
5) ...


1) Introduction
------------------------------------------------------------------------------------------------------

The INL LabVIEW repository consists of several projects...
* Template -> start here
* PID Control Centre -> example for photoionization detection based on the template

... that rely on several VIs common to all projects:
* Controls
* Modules
	* About
	* Analysis
	* Data
	* Display
	* Error
	* File -> Configuration, TDMS
	* Hardware -> Power Supply, Mass Flow Controller, Detector,...
	* Menu
	* Timing
* Shared
* Test	


Pieter De Beule
03-09-2012
Modified 26-11-2012

