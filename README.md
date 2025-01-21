CMOS OPAMP 2 STAGE 



Abstract— Operational amplifier is consider to be the most imperative electronic device. The procedure inscribed in this paper is to design a two stage CMOS operational amplifier (Opamp) and analyze the effect of various parameters on the characteristics of Opamp design. This paper is mainly concentrating on design of optimized Opamp gain. Keeping this as a main aspect, Opamp specifications are taken into account, i.e., Gain, phase margin, slew rate, power dissipation and others. This work presents a design and implementation of two stage CMOS operational amplifier which operates at ±1V supply voltage and Simulation process is carried out by using an EDA tool cadence virtuoso with 90nm technology. The obtained gain is 
84db with phase margin of 560 and the power dissipation is of 
38.02μW
Keywords—CMOS,opamp, Cadence,90nm opamp, gain 

BLOCK DIAGRAM


![image](https://github.com/user-attachments/assets/880b8647-374c-4b88-b32a-3d8cb1cf2f02)

CIRCUIT

![image](https://github.com/user-attachments/assets/f53ee111-be8f-4243-b7c9-9ed75a48ebad)

Fig.circuit diagram for Opamp using 90nm technology 

![image](https://github.com/user-attachments/assets/a8e29bd5-a33d-463a-b1a7-4492c666f994)

Fig.Circuit diagram of Opamp test bench in 90nm  

INTRODUCTION 
Opamps are the most commonly used devices     in electronic circuits. Their applications are wide. They are used in Filters, Differentiators, Integrators, Digital-Analog convertors and Comparators. The challenge faced in CMOS technology is mainly about scaling these devices to decrease their size and power consumption. Opamps are of two types namely inverting Opamp and non-inverting Opamp with two inputs and single output. The main prospect in this report is to design, optimize the size in order to increase the gain of 90nm technology. The modulation made here leads to better efficiency and operating frequency. The problem lies in design and implementation of two stage CMOS Opamp keeping various parameters into consideration which are constraints. In this paper the specification which becomes the target is the (W/L) ratio which indirectly relates to gain. 
However increase in the gain improves the performance and keeps up the stability of device. 
II.BLOCK DIAGRAM OF TWO STAGE CMOS OPERATIONAL AMPLIFIER
It has two stages, as shown in the block diagram where stage 1 is the differential amplifier and common source amplifier becomes stage 2. 
The differential amplifier has two different voltage inputs vin+ and vin- which amplifies the differences between two input voltages. Since the gain obtained from the first stage is not sufficient, it uses common source amplifier at second stage. Thus, the output of this differential amplifier continues to enter the common source amplifier where further more gain is increased. In order to obtain low gain at high frequencies and maintain the device’ stability, it includes compensation circuit whenever the device is in negative feedback condition. The two-stage CMOS opamp consists of a differential amplifier as the first stage and a common source amplifier as the second stage. 
- Stage 1– Amplifies the difference between two input voltages Vin + and Vin - with high input impedance and good noise rejection. It provides initial gain but often not sufficient for most applications.
- Stage 2 – Boosts the overall gain further and provides low output impedance, making it capable of driving loads effectively.
A compensation circuit is added to ensure stability in feedback conditions, typically using Miller compensation to introduce a dominant pole and prevent oscillations, thereby maintaining proper frequency response.

V.CONCLUSION
The simulation has been carried out using Cadence tool with 90nm technology. The gain has been increased by optimizing the parameters like (W/L) values. Using the design equations, by choosing and carefully sizing the structure of the circuit. The design performs a gain of 84db with phase margin of 87.89 under unity gain feedback configuration and the power dissipation is of 31.02μW, which is not correct we need to improve Miler compensation to control RHP which is responsible for UNITY GAIN BANDWIDHTH  location in bode plot.

VI.REFERENCES
[1]	B. Razavi, “Design of Analog CMOS Integrated Circuits”, New York: Mc-Graw Hill, 2001.  
[2]	.  Allen, P. E., & Holberg, D. R. (2002). CMOS Analog Circuit Design (2nd ed.). Oxford University Press.
[3]	https://www.researchgate.net/publication/320651737_Design_and_implementation_of_two_stage_CMOS_operational_amplifier_using_90nm_technology
