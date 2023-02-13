# 1.2V Band gap reference

With Regards Bishal Paudel ;)

Band gap reference is a circuit which will give constant output voltage with respect to temperature and supply variations.  
We can make a constant voltage reference, cancelling the effect of temperature by combining [CTAT](https://github.com/Bishal1022/Analog-IC-Design/tree/main/4.Band%20Gap%20Reference/1.CTAT%20Design) and [PTAT](https://github.com/Bishal1022/Analog-IC-Design/tree/main/4.Band%20Gap%20Reference/2.PTAT%20Design) circuits.

BGR is a major building block of any IC as it is very essential for a circuit to be immune to effect of temperature change. BGR are commonly used in LDO, Buck-boost converter, Regulator, ADC, DAC etc. Although there are other parameters like process variation which might effect V<sub>REF</sub>


## 1. Principle:

As stated above, for obtaining constant voltage we combine  [CTAT](https://github.com/Bishal1022/Analog-IC-Design/tree/main/4.Band%20Gap%20Reference/1.CTAT%20Design) and [PTAT](https://github.com/Bishal1022/Analog-IC-Design/tree/main/4.Band%20Gap%20Reference/2.PTAT%20Design)


![2 CTAT and PTAT collaged](https://user-images.githubusercontent.com/62088646/213234051-5e8018ff-7d71-4f22-9d10-48b07ed4cbea.jpg)


From our design of [CTAT](https://github.com/Bishal1022/Analog-IC-Design/tree/main/4.Band%20Gap%20Reference/1.CTAT%20Design) and [PTAT](https://github.com/Bishal1022/Analog-IC-Design/tree/main/4.Band%20Gap%20Reference/2.PTAT%20Design): 

• [CTAT](https://github.com/Bishal1022/Analog-IC-Design/tree/main/4.Band%20Gap%20Reference/1.CTAT%20Design) slope = -1.6mV/°C 

• [PTAT](https://github.com/Bishal1022/Analog-IC-Design/tree/main/4.Band%20Gap%20Reference/2.PTAT%20Design) slope = 73.29uV/°C

It can be observed that the slope of CTAT and PTAT differs and adding them up will not cancel their nature. Thus, we need to scale the CTAT and PTAT so that they cancels each other as depicted in given block diagram representation:

<p align="center">
<img width="400" alt="Schematic Diagram" src="https://user-images.githubusercontent.com/62088646/213187225-1e94b946-b910-4185-9be3-1f44b86db7b1.png">
</p>


## 2. Schematic Diagram:
The figure below depicts the schematic diagram for band gap reference by combining scaled [CTAT](https://github.com/Bishal1022/Analog-IC-Design/tree/main/4.Band%20Gap%20Reference/1.CTAT%20Design) and [PTAT](https://github.com/Bishal1022/Analog-IC-Design/tree/main/4.Band%20Gap%20Reference/2.PTAT%20Design) using current mirror circuit as current source.

<p align="center">
<img width="900" alt="Schematic Diagram" src="https://user-images.githubusercontent.com/62088646/213197758-10154544-686e-44c2-b452-f5abb7db7a52.png">
</p>





## 3. Result:
#### A. Temperature variation of CTAT, PTAT and V<sub>REF</sub>
Hence, by adding scaled CTAT and PTAT we obtained a band gap reference of ≈ 1.2V

![3 Temperature variation of PTAT,CTAT and VREF](https://user-images.githubusercontent.com/62088646/213210580-63f254be-9add-4b75-820c-b16eb62a5e0c.jpg)

#### B. Bell curve of V<sub>REF</sub>
When I zoomed in the graph of V<sub>REF</sub> , it looked like a bell-shaped curve with maximum variation 981uV. And we are getting such bell-curved because our CTAT and PTAT are not exact staright lines.

![2 Bell_curve_of_VREF](https://user-images.githubusercontent.com/62088646/213239768-16566fbb-032e-42dc-8a0c-1716fdaa38d9.jpg)

#### C. Supply variations on V<sub>REF</sub>
When evaluated with supply variation, we got 41mV deviation over 0.6V.

![4 Supply variations on VREF](https://user-images.githubusercontent.com/62088646/213239951-fe613980-ca95-44e2-bb59-8f4a74d28081.jpg)

Furthermore, if supply voltage and temperature variations is to be reduced, we need to use complex cascode mirror. Yet again using a cascode structure demands for higher supply voltage so trade-off is to be done as your requirement.

For more accurate and comprehensive analysis do check out the [Cookbook](https://github.com/Bishal1022/Analog-IC-Design/blob/main/3.Power_management_designs/1.Band_Gap_Reference/Cook-book_of_Bandgap_voltage_reference.pdf).

