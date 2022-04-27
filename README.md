# ENEL300-project
ENEL300-Winter2022

FONIMAKS

CAUTION: 

There are 2 files: voiceModulator-current is the current version of the FONIMAKS software while the voiceModulator-developing is the software file under development and has not been thoroughly tested. Please use the first file for all general uses.

The FONIMAKS software is developed for AVR128DB28 chip with XC8 compiler, other compilers/microcontrollers might not be compatible.

GENERAL INSTRUCTIONS:

Distortion: Adjust the cutoff variable to change the distortion intensity. The range of this cutoff is from 225 to 512, anything outside this range will break the code. This max and min value is already tested for normal human speech, if you wish to change this range, please refer to the datasheet below for more information.

Delay: Adjust the LENGTH variable to adjust the delay time. Larger values will yield a bigger time delay. The maximum of this variable is 9000, anything more than that will exceed the memory capacity of the AVR (this value might decrease as we add more effects into the software so please stay updated with the newest infomation)
If you wish to set the delay time to an exact value, please refer to the datasheet below

Pitch Shift: Adjust samFactor variable for a pitch shift effect. 1 would yield the same frequency as your input voice, while 0.5 would yield 1/2 the frequency and 2 would yield double the frequency. For the harmonizer effect, samFactor is set to 1.5 which is essentially a 5th above your input voice

AVR128DB28 DATASHEET

https://ww1.microchip.com/downloads/en/DeviceDoc/AVR128DB28-32-48-64-DataSheet-DS40002247A.pdf

For questions related to delay time specification, please go to page 92 and 498   

For questions related to distortion, please go to page 500
