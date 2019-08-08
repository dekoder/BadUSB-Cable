# BadUSB-Cable
BadUSB cable based on Attiny85 microcontroller (gerbers, design and schematic).

**Idea:** Joel Serna & Ernesto Sánchez

**Development and implementation:** Joel Serna & Ernesto Sánchez

**PCB design:** Rev0: Jorge Mata, Rev1 and Rev2: Ignacio Díaz Álvarez

1. History
2. Acknowledgement
3. Electronic components
4. BadUSB Cable without USB connector
	* Rev0 (only for reference)
	* Rev1 (only for reference)
	* Rev2 (final version)
5. Assembly, bootloader and testing

# History

* Start of the project and first BadUSB cable on breadboard (November 2017):

![BadUSB Cable Breadboard](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/badusb-cable-breadboard.jpg)



* First BadUSB cable with USB connector (December 2017):

![BadUSB Cable with USB connector](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/badusb-cable-usb-1.jpg)

![BadUSB Cable with USB connector](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/badusb-cable-usb-2.jpg)



* Finished proof of concept (January 2018):

![BadUSB Cable final test](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/badusb-cable-final-test.jpg)



* Technical presentation of BadUSB cable and first PCB design (Rev0) presented at Hackplayers Conference (February 2018):

![Design 1](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/first-version-1.png)

![Design 1-1](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/first-version-2.jpg)



* Rev1 of BadUSB cable design (January 2019):

![Rev1](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/revision-1_6*12mm.jpeg)

**NOTE:** More information in Rev1 section.



* Rev2 of BadUSB cable design (May 2019):

![Rev2](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/revision-2_6*10mm.png)

**NOTE:** More information in Rev2 section.



* First PCBs (July 2019):

![First PCBs](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/first-pcbs-3.jpeg)

![First PCBs](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/multi1.jpeg)

![First PCBs](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/multi2.jpeg)

![First PCBs](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/multi3.jpeg)

* BadUSB Cable (August 2019):

![0](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/finalcable0.jpeg)

![1](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/finalcable1.jpeg)

![2](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/finalcable2.jpeg)

# Acknowledgement

**PCB design first version:** Jorge Mata & Innovart

	* Jorge Mata: @jor_mata

	* Innovart: @innovart_cc

	* https://innovart.cc

**PCB design final version:** Ignacio Díaz & ForensicSecurity

	* Ignacio Díaz: @Ignacio Díaz Álvarez

	* Forensic & Security: @ForensicSec

	* https://forensic-security.com

# Electronic components

**Rev0:**
* ATTINY85 microcontroller
* 2 x 3.6V zener diode
* 2 x 68 ohm resistor
* 1 x 1.5k resistor

**Rev1-Rev2:**
* ATTINY85 microcontroller (8-soic)
* 1 x 3.6V zener diode common anode (SOT23)
* 2 x 68 ohm resistor (0402)
* 1 x 1.5k resistor (0402)

Electronic components have been bought in: https://www.digikey.com/

# Rev0
**NOTE:** This Rev0 is included for reference purposes only, Rev2 is the final and full tested version.

![BadUSB Cable Rev0](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/first-version-1.png)

![BadUSB Cable Rev0](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/first-version-2.jpg)

# Rev1
**NOTE:** This Rev1 is included for reference purposes only, Rev2 is the final and full tested version.

![BadUSB Cable Rev1](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/revision-1.jpg)

![BadUSB Cable Rev1](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/revision-1_6*12mm.jpeg)


# Rev2 (Final version)
Implementation of BadUSB cable based on Attiny85 microcontroller.

![BadUSB Cable revision-2](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/revision-2_6*10mm.png)

![BadUSB Cable final-1](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/revision-3-graph1.png)

![BadUSB Cable final-2](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/revision-3-graph2.jpg)

## Import the project
There is a custom built library footprints for this project, remember to import it.

## Introduction
You can order the necessary components with the gerber files in the gerber directory and de BOM (Bill Of Materials).

# Assembly, bootloader and testing
## Pinout

* **Black:** GND
* **Green:** D+
* **White:** D-
* **Red:** VDD

![Pinout](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/pinout.png)

## Hardware needed

To burn the bootloader you can use diferent techniques, for the one we use you will need:

* TEST CLIP SOIC 8 (2 X 4)  
* TINY AVR PROGRAMMER 

![clip](https://media.digikey.com/Photos/Pomona%20Photos/5250.JPG)
![programmer](https://media.digikey.com/Photos/Sparkfun%20Elec%20%20Photos/MFG_PGM-11801_sml.jpg)

## Download bootloader

* Download Micronucleus bootloader for ATTINY85: https://github.com/micronucleus

* You can find the bootloader file at micronucleus-t85\firmware\releases folder

* Use "t85_default.hex" for the bootloader

## Burning bootloader for ATTINY85

You must use the correct fuses bit for the bootloader:

* **Extended:** 0xFE
* **High:** 0xDD
* **Low:** 0xE1

AVRISP MKll In System Programmer and AVR Studio software for burning bootloader

![AVRDUDESS](https://github.com/joelsernamoreno/BadUSB-Cable-Gerbers/blob/master/images/avrdudess.png)

## Installing Digispark USB Driver

1. Download Arduino for Digispark which come with USB driver: http://sourceforge.net/projects/digistump/files/

2. Extract the file (DigisparkArduino-Win32-1.0.4-March29.zip) to any folder

3. Execute DigisparkArduino-Win32\DigisparkWindowsDriver\InstallDriver.exe to start installing the USB driver

## Payloads

You can get payloads in the following repository:

https://github.com/joelsernamoreno/badusb_examples/tree/master/attiny85_digispark