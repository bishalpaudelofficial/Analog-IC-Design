# Complementary to absolute temperature (CTAT) 

With Regards Bishal Paudel ;)

The circuit in which voltage decreases with increase in temperature is called CTAT.
If biased current is applied across a diode, it behaves as a CTAT provided the bias current is constant in nature.

Hence by the definition, if a constant current is passed through a diode then the voltage decreases at the rate of -1.6mV/°C with respect to temperature.


## 1. Proposed circuit:
According to the definition of CTAT, the proposed circuit is sketched.

<p align="center">
  <img width="141" alt="Proposed circuit" src="https://user-images.githubusercontent.com/62088646/213097119-124365a3-c6f3-4e97-b373-a6316f686187.png">
</p>


## 2. Schematic Diagram:
In CMOS technology the bipolar junction transistor (BJT) behaves like a diode when its base and collector terminal are shorted to ground. In our design, we have implemented diode using a BJT(pnp) with the current source in the emitter terminal replicating the proposed circuit.  

<p align="center">
  <img width="535" alt="1 Schematic of CTAT design" src="https://user-images.githubusercontent.com/62088646/213097269-8bc3499e-6954-4ad6-81cf-296264dafb8a.png">
</p>

To implement the practically realizable circuit, we will be replacing the ideal current source by a current mirror while designing bandgap refernce circuit. Nevertheless to understand the characteristics of CTAT, ideal current source is good enough.

## 3. Result:

![2 Voltage variation with temperature and its slope](https://user-images.githubusercontent.com/62088646/213100901-e2f76862-e5b8-44be-aeaa-6d77960a5d9f.jpg)

From the above figure we observed that as temperature increases, voltage decreases. Hence, we can conclude that CTAT is realized. Additionally, the slope of voltage w.r.t temperature (blue graph) is approximately -1.6mV/°C with variations from -1.5mV/°C to 1.78mV/°C.

For more accurate and comprehensive analysis do check out the Cookbook.

