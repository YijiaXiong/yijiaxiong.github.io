# Fluorescence Correlation Spectroscopy System
Welcome to the world of Fluorescence Correlation Spectroscopy (FCS), a sophisticated analysis technique that explores the fluctuations in fluorescence intensity. This technique serves as a gateway to unraveling the physical and chemical properties of molecules. In the realm of biochemical research, FCS finds its prowess in studying protein-fused fluorescent proteins and fluorescent dye-labeled biomolecules such as proteins and DNA/RNAs. Our FCS system, built by me in both hardware and software, began as a simple single-sample setup and evolved into a versatile platform equipped with an automated stage, enabling microplate measurements. Allow me to guide you through the intricacies of our FCS system:

## Hardware
Our FCS system is built around a Nikon TE300 inverted microscope, roughly divided into three subsystems: the laser launch subsystem, the inverted microscope, and the detection subsystem. These subsystems are linked by an optical fiber, ensuring a flexible and efficient setup. This modularity allows for independent alignment and troubleshooting, enhancing the overall robustness of the system. Behold an overview of our setup, complete with controllers adorning the roof shelf.

### Laser Launcher
The laser launcher system boasts three lasers: a 532nm Diode-pumped solid-state laser, a 632nm He-Ne laser, and a multi-line Argon laser (with major lines at 488nm and 514nm). Through an intricate assembly of mirrors, prisms, beam splitters, and flip-flop mounts, I've built the system that allows manual selection of any of the four lasers. The laser is then coupled into the optical fiber, and connects to the microscope. The image below showcases the optics with all lasers illuminated, exemplifying the beauty of precision engineering.

![Fcs Launcher](instruments/fcs-launcher.JPG)

### Microscope
Our microscope, the Nikon TE300, stands adorned with a 100X objective lens (S Fluo100, Nikon). A notable upgrade involves the integration of a LUDL automatic microplate stage, which is computer-controlled through RS232 communication.

![Fcs2](instruments/fcs2.JPG)

### Detection Subsystem
The heart of our detection subsystem is shown in this image.
![Fcs1](instruments/fcs1.JPG)

In the top-left corner, you'll discover the collimator for the laser optical fiber, orchestrating the passage of collimated laser light into the microscope. The fluorescence, collected through the objective lens, is coupled into the orange multimode optical fiber and then sent through the optical fiber to a beam splitter selector (either 50/50 splitter for single color FCS or dichroic for cross-correlation experiment). A pair of SPCM-AQR-14 avalanche photodiodes(APDs) are used to detect the fluorescence and the output signals are fed into a Flex01-05D multi-tau correlator.

## Software
The program was written in VB6. This program orchestrates parameter configuration for data acquisition, microplate stage control, and real-time correlation curve visualization. A couple of snapshots of this software in action are presented below:

![Corr](images/corr.PNG)

#### The interface for microplate well setting.
![Setwell](images/setwell.PNG)
Furthermore, I write another program written in MATLAB or R for data analysis. This program operates independently, allowing data analysis for binding affinity measurement. The main program integrates the scripts, simplifying the workflow and enabling quick results through just a few clicks.

#### Overlap all fcs curves
![Fitall1](images/fitall1.PNG)

#### Fit all fcs curves automatically
![Fitall3](images/fitall3.PNG)

#### Generate the binding curve and fit it with two models for selection
![Fitall4](images/fitall4.PNG)

Yet another VB.net program was written to organize and analyze the FCS experiment data:
![Fcsdata](images/fcsdata.PNG)


## Sample Result
Allow me to present the fruits of our labor, extracted from my publication:
*Xiong, Y.; et al. High-Affinity and Cooperative Binding of Oxidized Calmodulin by Methionine Sulfoxide Reductase. Biochemistry 2006, 45, (49), 14642-14654.*

The upper figure shows a group of the fluorescence correlation curves of one protein, oxidized Calmodulin, binding to various concentrations of another protein, Methionine Sulfoxide Reductase. The lower figure shows the binding curve and fitting. 
![MsrA](figs/msrA.png)
