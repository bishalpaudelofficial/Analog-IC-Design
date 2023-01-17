# Cascode LNA
With Regards Bishal Paudel ;) 

In this project we aim to achieve 2.1 GHZ LNA following the steps of cook-book for minimum noise figure. In order to achieve minimum noise figure, the principle of noise matching is being used. Since noise matching is usually a resonant operation it gives us narrow band output. 

Matching network not only have to do NOISE MATCHING for minimizing noise but also it should do IMPEDANCE MATCHING for Maximum Power transfer.

<img width="710" alt="image" src="https://user-images.githubusercontent.com/62088646/212983107-9312f85b-2293-4077-9732-5fd2ac3ac1c4.png">

1) Condition for Noise match: While looking back into the matching network we need to see 𝑍𝑜𝑝𝑡 to minimize. \
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

![1 Schematic Diagram](https://user-images.githubusercontent.com/62088646/212977058-0dc3096e-d469-443d-b151-9b59b1b61019.png)

## 3. Results

1. Noise Figure is as low as 507mdB(0.5dB)

![2 FrequencyVSNoiseplot](https://user-images.githubusercontent.com/62088646/212979413-b6002076-f52b-43bd-a9a2-c21409e976f4.png)

2. The gain is 13.25dB which is just adequate. (Trade-off done between noise matching and power matching)

![7 S21](https://user-images.githubusercontent.com/62088646/212979475-137242e1-374f-4c91-b915-12986b6d32ad.png)

3. The achieved 1-dB Compression point is -25dBm 

![4 1dBcompressionpoint](https://user-images.githubusercontent.com/62088646/212979719-cf5bc9e9-fa2f-4320-80bd-0704468c4d07.png)

      


For more accurate and comprehensive analysis do check out the Cookbook.
