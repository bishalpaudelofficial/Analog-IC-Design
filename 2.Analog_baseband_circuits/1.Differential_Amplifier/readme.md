# Differential Amplifier

With Regards Bishal Paudel ;)

This project is about designing a differential amplifier that aims to provide a cookbook for choosing the device parameters according to the design requirements provided to you. This project is designed in Cadence virtuoso using 180nm PDK.

## 1. Design Requirement: 

A) Technology: UMC 180nm process \
B) Supply Voltage (V<sub>dd</sub>) = 1.8 V \
C) Voltage gain (A<sub>v</sub>) = 100 (40dB) \
D) Load Capacitor (C<sub>L</sub>) = 10pF \
E) Input Common mode range (ICMR) = Max: +1.6V & Min: -0.8V \
F) Slew Rate (SR) = 5V/usec \
G) Power Dissipation < 3mW \
H) Gain Bandwidth Product (GBW) = 5MHz 

## 2. Schematic diagram
There are different types of differential amplifier topology available which have scope to achieve the set design requirement. This project is using 5 transistor OTA which provides better gain compared to other. As this project aims to have higher gain than specified in design requirement, 5 transistor OTA is preferred. 

<p align="center">
<img width="900" alt="Schematic Diagram" src="https://user-images.githubusercontent.com/62088646/212534694-775215bb-b2a0-4e26-a0d7-4aa08d6f3bc9.png">
</p>


## 3. Results
Bode plot is adopted which effectively depicts the design parameters: 

![3 BodePlot_after_increasing_width](https://user-images.githubusercontent.com/62088646/212535500-a4ffb4f3-c77d-459a-a637-91e7ca3809a0.jpg)

Hence \
Voltage gain (A<sub>v</sub>) = 39.4729dB ≈ 40dB \
Gain Bandwidth Product (GBW) ≈ 5 MHz \
Power Dissipation = 122 u W \
Also, the other defined design requirement were met.

For more accurate and comprehensive analysis do check out the [Cookbook](/Cook-Book_of_Differential_Amplifier.pdf).
