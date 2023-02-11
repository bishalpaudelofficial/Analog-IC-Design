# Two-Stage Op-Amp

With Regards Bishal Paudel ;)

This project is about designing a Two-Stage Op-Amp that aims to provide a cookbook for choosing the device parameters according to the design requirements provided to you. This project is designed in Cadence virtuoso using 180nm PDK.

## 1. Design Requirements:

A) Technology: UMC 180nm process \
B) Supply Voltage (Vdd) = 1.8 V \
C) Voltage gain (Av) = 1000 (60dB) \
D) Load Capacitor (CL) = 2pF \
E) Input Common mode range (ICMR) = Max: +1.6V & Min: -0.8V \
F) Slew Rate (SR) = 20V/usec \
G) Power Dissipation < 300uW \
H) Gain Bandwidth Product (GBW) = 30MHz \
I) Phase Margin > 60°


## 2. Schematic diagram

<p align="center">
<img width="850" alt="Schematic Diagram" src="https://user-images.githubusercontent.com/62088646/218270192-169a3bfa-6f42-4607-b4f1-f2b749494161.png">
</p>


## 3. Results

<p align="center">
<img width="900" alt="Schematic Diagram" src="https://user-images.githubusercontent.com/62088646/212559710-30275fc0-3828-42fc-9c49-ce2754865304.jpg">
</p>


Hence \
Voltage gain (Av) ≈ 70dB \
Gain Bandwidth Product (GBW) = 30 MHz \
Phase Margin (PM) = 59.38° ≈ 60° \
Power Dissipation = 271.7 u W \
Also, the other defined design requirement were met.

For more accurate and comprehensive analysis do check out the [Cookbook](https://github.com/Bishal1022/Analog-IC-Design/blob/main/2.Analog_baseband_circuits/2.Two-stage_Op-Amp/Cook-book_of_two_stage_op_amp.pdf).
