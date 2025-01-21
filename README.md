# CMOS_2STAGE_OPAMP
CMOS_OPAMP_2STAGE
Design and analysis of 2-Stage opamp in 90nm gpdk tech | Analog Ic design | CADENCE
EDA tool : Cadence Virtuoso 
Description: In this project I designed and studied opamp configurations, aim is to design circuit with PM = 60, ICMR ( -1 to 2)v , and power dissipation Pdiss < 2mW., Vout range +- 2v , SR>10V/us , VDD = 2.5, Av > 5000 and study  its CMMR, SR, Power dissipation, stability analysis, PVT variations.
Abstract—Operational amplifier is consider to be the most 
imperative electronic device. The procedure inscribed in this paper is to 
design a two stage CMOS operational amplifier (Opamp) and analyze 
the effect of various parameters on the characteristics of Opamp design. 
This paper is mainly concentrating on design of optimized Opamp gain. 
Keeping this as a main aspect, Opamp specifications are taken into 
account, i.e., Gain, phase margin, slew rate, power dissipation and 
others. This work presents a design and implementation of two stage 
CMOS operational amplifier which operates at ±1V supply voltage and 
Simulation process is carried out by using an EDA tool cadence virtuoso 
with 90nm technology. The obtained gain is  
84db with phase margin of 560 and the power dissipation is of  
38.02μW 
Keywords—CMOS,opamp,Cadence,90nm opamp, gain  
I. 
INTRODUCTION  
Opamps are the most commonly used devices     
in electronic 
circuits. Their applications are wide. They are used in Filters, 
Differentiators, 
Integrators, 
Digital-Analog 
convertors 
and 
Comparators. The challenge faced in CMOS technology is mainly about 
scaling these devices to decrease their size and power consumption. 
Opamps are of two types namely inverting Opamp and non-inverting 
Opamp with two inputs and single output. The main prospect in this 
report is to design, optimize the size in order to increase the gain of 
90nm technology. The modulation made here leads to better efficiency 
and operating frequency. The problem lies in design and 
implementation of two-stage CMOS Opamp keeping various 
parameters into consideration which are constraints. In this paper the 
specification that becomes the target is the (W/L) ratio which 
indirectly relates to gain.  
However increase in the gain improves the performance and keeps 
up the stability of device.  
II.BLOCK DIAGRAM OF TWO STAGE CMOS OPERATIONAL AMPLIFIER 
It has two stages, as shown in the block diagram where stage 1 is the 
differential amplifier and common source amplifier becomes stage 2.  
The differential amplifier has two different voltage inputs vin+ and vin- 
which amplifies the differences between two input voltages. Since the 
gain obtained from the first stage is not sufficient, it uses common 
source amplifier at second stage. Thus, the output of this differential 
amplifier continues to enter the common source amplifier where 
further more gain is increased. In order to obtain low gain at high 
frequencies and maintain the device’ stability, it includes 
compensation circuit whenever the device is in negative feedback 
condition. The two-stage CMOS opamp consists of a differential 
amplifier as the first stage and a common source amplifier as the 
second stage.  - Stage 1– Amplifies the difference between two input voltages Vin + 
and Vin - with high input impedance and good noise rejection. It 
provides initial gain but often not sufficient for most applications. - Stage 2 – Boosts the overall gain further and provides low output 
impedance, making it capable of driving loads effectively. 
A compensation circuit is added to ensure stability in feedback 
conditions, typically using Miller compensation to introduce a
