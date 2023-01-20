# Cascode LNA
With Regards Bishal Paudel ;) 

In this project we aim to achieve 2.1 GHZ LNA following the steps of cook-book for minimum noise figure. In order to achieve minimum noise figure, the principle of noise matching is being used. Since noise matching is usually a resonant operation it gives us narrow band output. 

Matching network not only have to do NOISE MATCHING for minimizing noise but also it should do IMPEDANCE MATCHING for Maximum Power transfer.

<p align="center">
<img width="510" alt="image" src="https://user-images.githubusercontent.com/62088646/212983107-9312f85b-2293-4077-9732-5fd2ac3ac1c4.png">
</p>


1) Condition for Noise match: While looking back into the matching network we need to see 𝑍𝑜𝑝𝑡 to minimize. 
2) Condition for Power match: While looking into the matching network we need to see 𝑍𝑖𝑛 as conjugate of source impedance. \
Hence, 1) and 2) will only be achieved if 𝑍𝑜𝑝𝑡 is complex conjugate of 𝑍𝑖𝑛.

Any matching network that does both the job simultaneously is known as simultaneous noise matching and power matching.

## 1. Design Requirement: 

A) Technology: UMC 180nm process \
B) Supply Voltage (Vdd) = 1.8 V \
C) |S21| > 15 dB \
D) NF < 2 dB \
E) Power < 10 mW \ 
F) |S11| < -15 dB \
G) |S22| < -15 dB \
H) |S12| < -30 dB (Reverse Isolation)

## 2. Schematic diagram

<p align="center">
<img width="900" alt="1 Schematic Diagram" src="https://user-images.githubusercontent.com/62088646/213182916-09071518-f56a-49c7-892e-d12fa819f7a7.png">
</p>

## 3. Results

1. Noise Figure is as low as 507mdB(0.5dB)

![2 FrequencyVSNoiseplot](https://user-images.githubusercontent.com/62088646/212979413-b6002076-f52b-43bd-a9a2-c21409e976f4.png)

2. The gain is 13.25dB which is just adequate. (Trade-off done between noise matching and power matching)

![7 S21](https://user-images.githubusercontent.com/62088646/212979475-137242e1-374f-4c91-b915-12986b6d32ad.png)

3. The achieved 1-dB Compression point is -25dBm 

![4 1dBcompressionpoint](https://user-images.githubusercontent.com/62088646/212979719-cf5bc9e9-fa2f-4320-80bd-0704468c4d07.png)

4. The stipulated S11 < -15 dB but we are able to achieve -12.3 dB because a trade-off was done between input matching and noise matching to have a better noise performance of LNA, which is the priority.   

![5 S11](https://user-images.githubusercontent.com/62088646/212984528-3b5fde3d-6c5e-4130-8a62-87fd6fdc36c6.png)

5. We are able to achieve S12 = -46 dB at our design frequency. Hence, exemplary reverse isolation is achieved as stipulated by cascode design.

![6 S12](https://user-images.githubusercontent.com/62088646/212985092-eaaa9eaa-6050-4911-9f65-603dfa71c5f8.png)

6. Also, the achieved S22 is -10.3 dB which is decent enough.

![8 S22](https://user-images.githubusercontent.com/62088646/212985175-c1e1385c-642c-47b9-9c1a-7fe50920a146.png)


For more accurate and comprehensive analysis do check out the [Cookbook](https://github.com/Bishal1022/Analog-IC-Design/blob/main/1.Narrowband%202.1GHz%20LNA/Cook-book%20of%20LNA.pdf).
