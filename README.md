
Abstract—Operational amplifier is consider to be the most imperative electronic device. The procedure inscribed in this paper is to design a two stage CMOS operational amplifier (Opamp) and analyze the effect of various parameters on the characteristics of Opamp design. This paper is mainly concentrating on design of optimized Opamp gain. Keeping this as a main aspect, Opamp specifications are taken into account, i.e., Gain, phase margin, slew rate, power dissipation and others. This work presents a design and implementation of two stage CMOS operational amplifier which operates at ±1V supply voltage and Simulation process is carried out by using an EDA tool cadence virtuoso with 90nm technology. The obtained gain is 
84db with phase margin of 560 and the power dissipation is of 
38.02μW
Keywords—CMOS,opamp,Cadence,90nm opamp, gain 
	I.	INTRODUCTION 
Opamps are the most commonly used devices     in electronic circuits. Their applications are wide. They are used in Filters, Differentiators, Integrators, Digital-Analog convertors and Comparators. The challenge faced in CMOS technology is mainly about scaling these devices to decrease their size and power consumption. Opamps are of two types namely inverting Opamp and non-inverting Opamp with two inputs and single output. The main prospect in this report is to design, optimize the size in order to increase the gain of 90nm technology. The modulation made here leads to better efficiency and operating frequency. The problem lies in design and implementation of two stage CMOS Opamp keeping various parameters into consideration which are constraints. In this paper the specification which becomes the target is the (W/L) ratio which indirectly relates to gain. 
However increase in the gain improves the performance and keeps up the stability of device. 
II.BLOCK DIAGRAM OF TWO STAGE CMOS OPERATIONAL AMPLIFIER
It has two stages, as shown in the block diagram where stage 1 is the differential amplifier and common source amplifier becomes stage 2. 
The differential amplifier has two different voltage inputs vin+ and vin- which amplifies the differences between two input voltages. Since the gain obtained from the first stage is not sufficient, it uses common source amplifier at second stage. Thus, the output of this differential amplifier continues to enter the common source amplifier where further more gain is increased. In order to obtain low gain at high frequencies and maintain the device’ stability, it includes compensation circuit whenever the device is in negative feedback condition. The two-stage CMOS opamp consists of a differential amplifier as the first stage and a common source amplifier as the second stage. 
- Stage 1– Amplifies the difference between two input voltages Vin + and Vin - with high input impedance and good noise rejection. It provides initial gain but often not sufficient for most applications.
- Stage 2 – Boosts the overall gain further and provides low output impedance, making it capable of driving loads effectively.
A compensation circuit is added to ensure stability in feedback conditions, typically using Miller compensation to introduce a dominant pole and prevent oscillations, thereby maintaining proper frequency response.
 ![image](https://github.com/user-attachments/assets/1274cb3d-672f-40f7-9334-44a75957185d)

                    Fig.1.Block diagram of two stage Opamp
 ![image](https://github.com/user-attachments/assets/a88c2daf-f7af-4ac0-a937-b4f7c2f454d0)

Fig.2.Circuit Diagram of Opamp 
	III.	DESIGN PROCEDURE
In the cadence tool we designed a circuit for finding β 
effective and Vth values for NMOS and PMOS 
  
A.	NMOS and PMOS Bias circuit  
For calculating βeff and Vth values, we use the NMOS and PMOS bias circuit. 
To determine μnCox and μpCox for 90nm  
βeff  = μ.Cox(W/L)
Where βeff is the MOSFET transconductance effective factor, μ is the mobility of electrons and Cox is the oxide capacitance. 
 ![image](https://github.com/user-attachments/assets/08d62533-9b1d-4cb2-8aa4-05a84c055a12)
![image](https://github.com/user-attachments/assets/b4eeecfd-df1e-49f5-8b88-21993f7bcea3)

Fig.3.NMOS circuit to find process information 
 ![image](https://github.com/user-attachments/assets/da27b0fb-d9a9-41b3-b7da-efe760a1e9e3)

Fig.4.PMOS circuit to find process information 
Table I. Process information βeff and Vth values of NMOS and PMOS 
device parameters
 ![image](https://github.com/user-attachments/assets/22065f61-de47-4711-9e1b-4264366b063a)

  
B.	Design of Opamp 
The total gain of two stage CMOS Opamp is defined by Av. The corresponding equation is given by the product of Av1 and Av2. 
  
Where Av1 is called as differential amplifier gain and Av2 is called as common source amplifier gain. 
 ![image](https://github.com/user-attachments/assets/a2a827e8-ef43-485b-b1bb-a19ba47b8262)

Table 1 Design Specifications
 ![image](https://github.com/user-attachments/assets/a324dd08-8541-4e66-a25c-94de22012856)

![image](https://github.com/user-attachments/assets/f442874a-bf3a-4fbc-9d9d-f683677c9a01)

  
 
Fig.6.circuit diagram for Opamp using 90nm technology 
![image](https://github.com/user-attachments/assets/6c70167d-021d-4172-b69e-d5dd7e84f64a)

 
Fig.7.Circuit diagram of Opamp test bench in 90nm  

	IV.	RESULTS
The design and optimization of two stages CMOS OPAMP has been done to increase the gain by using 90nm technology in cadence tool. The various parameters in this device are constraints, with few modifications in parameters lead to the improvised gain. By using theoretical values further resizing is done. Furthermore a modification in W/L ratios of MOSFET as shown in table IV and it leads to better improvisation of this two stage CMOS Opamp gain is as shown in Fig.8  
Table IV. Resizing in MOSFETs W /L ratio with reference to theoretical values in table III for a gain of 84dB
To resize the aspect ratios of your MOSFETs to achieve a gain of 84 dB, a phase margin of 56°, and a gain margin greater than 1 dB, we need to make calculated adjustments. Here’s how we can refine the aspect ratios:
1. Adjusting (W/L)(W/L)(W/L) for Gain:
•	The overall gain AvA_vAv is proportional to the transconductance gm1g_{m1}gm1 and gm6g_{m6}gm6. Increasing the aspect ratio (W/L)(W/L)(W/L) for M1, M2, or M6 will increase gm1g_{m1}gm1 and gm6g_{m6}gm6, respectively.
   
2. Calculating New Aspect Ratios

 Let’s update the aspect ratios accordingly and provide the revised values.Here are the updated aspect ratios to achieve the desired gain and phase margin:
 
These adjustments should help achieve a gain of 84 dB, a phase margin of 56°, and a gain margin greater than 1 dB. 
 ![image](https://github.com/user-attachments/assets/f523d4d8-4925-4620-a1af-0ce1d57998eb)

Fig.8.Graph representing frequency response of Opamp at 90nm , 84db gain
TRANSIENT RESPONCE 

![image](https://github.com/user-attachments/assets/7fd613a6-e093-4d22-95c4-1e96ebfa4fe1)

DC RESPOMNCE 
![image](https://github.com/user-attachments/assets/6732d392-d0b5-4155-a5b0-91806b6e22e4)

Table 2 Results
  
Figure 10 CMMRR Calculation
![Uploading image.png…]()

 
CMRR – 100.38 db
Figure 11 CMRR
V.CONCLUSION
The simulation has been carried out using Cadence tool with 90nm technology. The gain has been increased by optimizing the parameters like (W/L) values. Using the design equations, by choosing and carefully sizing the structure of the circuit. The design performs a gain of 84db with phase margin of 87.89 under unity gain feedback configuration and the power dissipation is of 31.02μW, which is not correct we need to improve Miler compensation to control RHP which is responsible for UNITY GAIN BANDWIDHTH  location in bode plot.
VI.REFERENCES
[1]	B. Razavi, “Design of Analog CMOS Integrated Circuits”, New York: Mc-Graw Hill, 2001.  
[2]	.  Allen, P. E., & Holberg, D. R. (2002). CMOS Analog Circuit Design (2nd ed.). Oxford University Press.
[3]	https://www.researchgate.net/publication/320651737_Design_and_implementation_of_two_stage_CMOS_operational_amplifier_using_90nm_technology
