# Laser Induced Fluorescence(LIF) Detection System
This is part of my current project. Our long term goal is to develop a portable, point-of-care device for on-site pathagen detection. I have built a few Laser Induced Fluorescence(LIF) prototypes for this project. 
## Hardware
Here is a minimal setup for LIF. Notice the CPS1 battery pack - this system powered by rechargable battery which make it possible to be portable.
![LIF setup](instruments/minilif.JPG)
A more powerful system was also built. This system has multiple lasers installed on a manual wheel (left side) and an automatical filter wheel which can be controlled by the data acquisition program. A multiple channel relay circuit was include to control the power of the lasers.
![LIFpro setup](instruments/minilifpro2.JPG)
Here is a close-up of the setup.
![LIFpro close-up](instruments/minilifpro3.JPG)
## Software
The software was written in VB.net. Here is a screenshot of the main GUI of the software:
![LIF program](images/yxLiFpro.png)
The channels can be set as:
![Channel Selection](images/lifchannel.png)
## Connect to Smart Phone
A LIF prototype with the capability of sending reading result to a smart phone was developed. The system is webpage based, so users can use any smart phone to connect to the device, control the on/off of the laser and  start the reading process. Then the result will be returned to the phone. This capability is enssential for a POC device to report detected positive case to the disease control center. The disease control center then will have the realtime data to monitor the epidemiological distribution of given disease.
![The device prototype](instruments/rpi1.jpg)
Here are the screenshots of the app on an iphone:
![Screenshot1](images/rpi1.png)
![Screenshot2](images/rpi2.png)