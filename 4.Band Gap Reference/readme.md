# 1.2V Band gap reference

With Regards Bishal Paudel ;)

Band gap reference is a circuit which will give constant output voltage with respect to temperature and supply variations. It is a major building block of any IC. Although there are other parameters like process variation also which might effect VREF. 

[PTAT](https://github.com/Bishal1022/Analog-IC-Design/tree/main/4.Band%20Gap%20Reference/2.PTAT%20Design)
[CTAT](https://github.com/Bishal1022/Analog-IC-Design/tree/main/4.Band%20Gap%20Reference/1.CTAT%20Design)

## 1.Principle

<p align="center">
<img width="400" alt="Schematic Diagram" src="https://user-images.githubusercontent.com/62088646/213187225-1e94b946-b910-4185-9be3-1f44b86db7b1.png">
</p>

## 2. Schematic Diagram:
In CMOS technology the bipolar junction transistor (BJT) behaves like a diode when its base and collector terminal are shorted to ground. In our design, we have implemented diode using a BJT(pnp) with the current source in the emitter terminal replicating the proposed circuit.  

  ![1 Schematic diagram of BGR_Currentmirror](https://user-images.githubusercontent.com/62088646/213197758-10154544-686e-44c2-b452-f5abb7db7a52.png)


To implement the practically realizable circuit, we will be replacing the ideal current source by a current mirror while designing bandgap refernce circuit. Nevertheless to understand the characteristics of CTAT, ideal current source is good enough.

## 3. Result:

![3 Temperature variation of PTAT,CTAT and VREF](https://user-images.githubusercontent.com/62088646/213197857-0fccb30a-1c76-4fe1-9c9f-153763dd8d93.jpg)

From the above figure we observed that as temperature increases, voltage decreases. Hence, we can conclude that CTAT is realized. Additionally, the slope of voltage w.r.t temperature (blue graph) is approximately -1.6mV/°C with variations from -1.5mV/°C to 1.78mV/°C.

For more accurate and comprehensive analysis do check out the Cookbook.

