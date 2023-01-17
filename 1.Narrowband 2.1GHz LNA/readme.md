# Cascode LNA
With Regards Bishal Paudel ;) 

The given LNA is designed at 2.1GHz. I have uploaded the Schematic design snap and the results obtained using the same. 

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
      2. The gain is 13.25dB which is just adequate. (Trade-off done between noise matching and power matching)
      3. And other S parameter plots are uploded in repo. Which can be adjusted as per the requirement with the cost of trade off with other parameter. 
      
In this design I have done a trade off with Power(Input) match which can be descripted as:

<img width="473" alt="Screenshot 2022-11-11 134052" src="https://user-images.githubusercontent.com/62088646/201296789-a1aa720c-ad44-456b-9679-1e212bd4c7c9.png">

