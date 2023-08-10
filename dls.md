# Dynamic Light Scattering System

Welcome to the Dynamic Light Scattering (DLS) System, a powerful technique for determining the size distribution profile of small particles in suspension or polymers in solution. This cutting-edge technology utilizes the temporal fluctuations of laser light scattering by particles or macro molecules in the solution. By analyzing auto-correlation functions of intensity, we can accurately extract particle size distributions. DLS is also referred to as photon correlation spectroscopy (PCH) or quasi-elastic light scattering. The auto-correlation process is facilitated by a dedicated hardware correlator, while the subsequent fitting procedure involves the intricate "inverse Laplace transform" technique, which I expertly employ using MATLAB. Additionally, I've seamlessly integrated data acquisition into the MATLAB script, resulting in an intuitive GUI akin to commercial software.

## Hardware
The DLS system boasts two essential subsystems: the laser scattering subsystem and the detection subsystem, interconnected by a multimode optical fiber. Here is our laser scattering setup:

![DLS light scattering](images/dls1.jpg)

For reference, a ruler is included in the picture, showcasing the system's compact design centered around a cuvette holder.

This picture shows the detection subsystem. This assembly features an optical fiber coupler, a beam splitter, and a pair of avalanche diodes, a strategic choice that effectively mitigates the afterpulse effect during detection.

![DLS detection system ](images/dls2.jpg)

## Software
The software's GUI is designed with simplicity and user-friendliness in mind, ensuring a smooth and intuitive experience for all users.
![DLS software](images/yxcorr.png)
As the fitting process unfolds, this dialog provides real-time updates on the regression progress:
![DLS software](images/yxcorr-fitting.png)
Presented here is a measured DLS curve, alongside the fitting result for a 42.9nm standard bead:
![DLS software](images/yxcorr-result.png)