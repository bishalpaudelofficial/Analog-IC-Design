# Proportional to absolute temperature (PTAT) 

With Regards Bishal Paudel ;)

The circuit in which voltage increases with increase in temperature is called PTAT.

Since we have [CTAT](https://github.com/Bishal1022/Analog-IC-Design/tree/main/4.Band%20Gap%20Reference/1.CTAT%20Design) which voltage decreases with temperature now in pursue of getting a band gap reference(BGR) we need a PTAT circuit in which voltage increases with increase in temperature. Combining both the circuit with proper scaling, we obtain a near constant reference voltage(BGR).

## 1. Proposed circuit:
According to the definition of PTAT, the proposed circuit is sketched.

<p align="center">
  <img width="400" alt="Proposed circuit" src="https://user-images.githubusercontent.com/62088646/213192579-fc5988f3-bbe8-4156-bdc1-da7158093a42.png">
</p>


## 2. Schematic Diagram:  
In CMOS technology the bipolar junction transistor (BJT) behaves like a diode when its base and collector terminal are shorted to ground. In our design, we have implemented diode using a BJT(pnp) with the current source in the emitter terminal replicating the proposed circuit. To implement the practically realizable circuit, I have replaced the ideal current source by a current mirror while designing schematic of PTAT.

<p align="center">
<img width="720" alt="Schematic Diagram" src="https://user-images.githubusercontent.com/62088646/213105464-ff27fec3-b870-4d69-b0a0-c3d3f13c2b81.jpg">
</p>


## 3. Result:

![10 Third_cut-design_PTAT(R2) plot and its slope](https://user-images.githubusercontent.com/62088646/213193147-0b4c6d5d-480a-48fb-8420-8e62e859affc.png)

From the above figure we observed that as temperature increases, voltage increases. Hence, we can conclude that PTAT is realized. Additionally, the slope of voltage w.r.t temperature (blue graph) is approximately 73.29uV/°C with variations from 71uV/°C to 77uV/°C.

For more accurate and comprehensive analysis do check out the Cookbook.


