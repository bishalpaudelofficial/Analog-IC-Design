# Wideband LNA
With Regards Bishal Paudel ;) 

We designed a [Narrow Band LNA](https://github.com/Bishal1022/Analog-IC-Design/tree/main/1.RFIC/1.Narrowband_2.1GHz_LNA) at our Design Frequency 2.1 GHz with noise Figure 0.5dB. Having a narrowband LNA in today’s world where mobile devices cover all communication bands to 6 GHz will be requiring multi-LNA solution. \
Hence, we require a single wideband LNA which will be flexible in terms of area, power and costs.

Cascode LNA with LC matching networks at input and output provides good performance but narrow bandwidth. To get wide band with low noise we have to get NF<sub>min</sub> over wide range of frequency.We have lot of Inductors & resonance circuit which is causing a Narrow band hence, we need to
**design an Inductor less Broad Band LNA.**


## NOISE CANCELLING PRINCIPLE:
<ins>Principle:</ins> In a circuit with a two path to the output and which two path are making observation to the input such that signal are correlated and noise anti-correlated hence when combined signal are reinforced and noise has been cancelled. (Magically) Noise cancelling allows input circuit to be designed only for power matching (unlike [noise matching](https://github.com/Bishal1022/Analog-IC-Design/tree/main/1.RFIC/1.Narrowband_2.1GHz_LNA#cascode-lna) in Narrow Band LNA). Noise matching of input circuit is relaxed/eliminated as noise matching is usually a resonant operation. 
Hence, in this way Noise Cancelling Aims to achieve wide-bandwidth operation.Although Noise of the Cancellation circuit remains that is noise cancellation circuit has its own noise.


## Basic Noise-Cancelling Behavioral Model:

<p align="center">
<img width="500" alt="1 Schematic Diagram" src="https://user-images.githubusercontent.com/62088646/219562001-67bf591c-ed1f-4cf9-bb90-f925501fc8da.png"> 
</p>
<p align="center">
  <sub>Figure: Noise-Cancelling Behavioral Model</sub>
</p>  
<sub><sup> ***Ref [1]: D. Murphy et al., "A Blocker-Tolerant, Noise-Cancelling Receiver Suitable for Wideband Wireless Applications," in IEEE 
Journal of Solid-State Circuits, vol. 47, no. 12, pp. 2943-2963, Dec. 2012, doi: 10.1109/JSSC.2012.2217832*** <sup></sub> 
  

  
 *Here*, 𝑅<sub>𝑖𝑛</sub> = 𝑅<sub>𝑠</sub> for impedance/Power matching

Q) Why are we using 𝑅𝑖𝑛 which has its own noise? \
=> Because it’s going to be cancelled out by use of Noise-Cancelling
From the Figure by Applying Circuit Law;

<p align="center">
<img width="220" alt="image" src="https://user-images.githubusercontent.com/62088646/219565712-c260c0eb-4f37-495e-a115-24c80a813596.png">
</p>

We can see from the Equations how noise due to R<sub>in</sub> is anti-correlated and if scaled and added they are going to be cancelled. \
Hence, with this strategy of Noise Cancelling Principle, we are going to achieve wide band, inductor less LNA. 
  
  
  > **THIS PROJECT IS ONGOING PLEASE STAY TUNED FOR UPDATES**
