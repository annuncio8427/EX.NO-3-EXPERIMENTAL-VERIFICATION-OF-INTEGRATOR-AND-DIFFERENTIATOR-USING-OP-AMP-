3. ##**EX.NO:
** 3  EXPERIMENTAL VERIFICATION OF INTEGRATOR AND DIFFERENTIATOR USING OP-AMP 
            
**DATE:**  
             3A INTEGRATOR
---

## AIM
To design and test the performance of integrator and differentiator circuits using Op-amp

---

## APPARATUS REQUIRED

| S.No | Name of the Apparatus | Range | Quantity |
|------|------------------------|--------|-----------|
| 1 | Function Generator | 3 MHz | 1 |
| 2 | DSO | 30 MHz | 1 |
| 3 | Dual RPS | (0 – 30) V | 1 |
| 4 | Op-Amp | µA741 | 1 |
| 5 | Bread Board | — | 1 |
| 6 | Resistors | 1K,10K,100K  | 2 |
| 7 | capacitors | 0.1µF,0.01µF | 1 |
| 8 | Connecting wires and probes | As required | — |

---

## THEORY
INTEGRATOR
A circuit in which the output voltage waveform is the integral of the input voltage waveform is the integrator. Such a circuit is obtained by using a basic inverting amplifier configuration if the feedback resistor Rf is replaced by a capacitor Cf . The expression for the output voltage is given as,
Vo = - (1/Rf C1 ) ∫ Vi dt

Here the negative sign indicates that the output voltage is 180 0 out of phase with the input signal. Normally between fa and fb the circuit acts as an integrator. Generally, the value of fa < fb . The input signal will be integrated properly if the Time period T of the signal is larger than or equal to Rf Cf . That is,
T ≥ Rf Cf

The integrator is most commonly used in analog computers and ADC and signal-wave shaping circuits.
CIRCUIT DIAGRAM
## CIRCUIT DIAGRAM
![WhatsApp Image 2025-11-28 at 2 18 12 PM](https://github.com/user-attachments/assets/0b927f4c-261f-4a66-96a7-0a98f755597c)


## MODEL GRAPH

![WhatsApp Image 2025-11-28 at 2 19 31 PM](https://github.com/user-attachments/assets/d290967f-c590-45f5-a090-e12d48e119f8)


---

## DESIGN

To obtain the output of an Integrator circuit with component values R1Cf = 0.1ms , Rf = 10 R1 and Cf = 0.01 µF and also if 1 V peak square wave at 1000Hz is applied as input.
We know the frequency at which the gain is 0 dB, fb = 1 / (2π R1 Cf) Therefore fb = 	 Since fb = 10 fa , and also the gain limiting frequency fa = 1 / (2π Rf Cf)
We get , R1 =	and hence Rf = 	

## PROCEDURE

1.	Connections are given as per the circuit diagram
2. + Vcc and - Vcc supply is given to the power supply terminal of the Op-Amp IC.
3.	By adjusting the amplitude and frequency knobs of the function generator, appropriate input voltage is applied to the inverting input terminal of the Op- Amp.
4.	The output voltage is obtained in the CRO and the input and output voltage waveforms are plotted in a graph sheet.


## TABULATION

![WhatsApp Image 2025-11-28 at 2 24 22 PM](https://github.com/user-attachments/assets/fc473679-ea64-4815-99ae-f27e629a131f)

---

## OUT PUT WAVEFORM AND DISCUSSION 

![WhatsApp Image 2025-11-28 at 2 23 32 PM](https://github.com/user-attachments/assets/bab973f4-9396-48c7-abaf-ac02c17a5bd7)
![WhatsApp Image 2025-11-28 at 2 26 03 PM](https://github.com/user-attachments/assets/bc033ead-9ac4-42a5-98b5-e56ce7e177df)

---
**DATE:**  
             3 B DIFFERENTIATOR
---

## AIM
To design and test the performance of integrator and differentiator circuits using Op-amp

---

## APPARATUS REQUIRED

| S.No | Name of the Apparatus | Range | Quantity |
|------|------------------------|--------|-----------|
| 1 | Function Generator | 3 MHz | 1 |
| 2 | DSO | 30 MHz | 1 |
| 3 | Dual RPS | (0 – 30) V | 1 |
| 4 | Op-Amp | µA741 | 1 |
| 5 | Bread Board | — | 1 |
| 6 | Resistors | 1K,10K,100K  | 2 |
| 7 | capacitors | 0.1µF,0.01µF | 1 |
| 8 | Connecting wires and probes | As required | — |

---

## THEORY
DIFFEERENTIATOR:
The differentiator circuit performs the mathematical operation of differentiation; that is, the output waveform is the derivative of the input waveform. The differentiator may be constructed from a basic inverting amplifier if an input resistor R1 is replaced by a capacitor C1 . The expression for the output voltage is given as,
Vo = - Rf C1 ( dVi /dt )

Here the negative sign indicates that the output voltage is 180 0 out of phase with the input signal. A resistor Rcomp = Rf is normally connected to the non-inverting input terminal of the op-amp to compensate for the input bias current. A workable differentiator can be designed by implementing the following steps:
1.	Select fa equal to the highest frequency of the input signal to be differentiated. Then, assuming a value of C1 < 1 µF, calculate the value of Rf.
2.	Choose fb = 20 fa and calculate the values of R1 and Cf so that R1C1 = Rf Cf.

The differentiator is most commonly used in wave shaping circuits to detect high frequency components in an input signal and also as a rate–of–change detector in FM modulators.

## CIRCUIT DIAGRAM

![WhatsApp Image 2025-11-28 at 2 29 29 PM](https://github.com/user-attachments/assets/13a1934a-edba-4cbc-b878-45d0957cb6b0)



## MODEL GRAPH

(i)	 SINE WAVE INPUT

<img width="687" height="479" alt="image" src="https://github.com/user-attachments/assets/c89226c0-c2bb-4544-b355-27fc0d923f1a" />
---

AND

(ii) SQUARE WAVE INPUT

<img width="758" height="447" alt="image" src="https://github.com/user-attachments/assets/cda33b00-c40c-490f-a9bd-e06107119c25" />


---

## DESIGN

Design an op-amp differentiator that will differentiate an input signal with fmax = 100HZ Select fa = fmax = 100 HZ = 1 / 2πRFC1
Let C1 = 0.1μF
Then RF = 1 / 2π(102)(10-7)
= 15.9KΩ
Now choose fb = 10fa = 1 / 2πR1C1 Therefore, R1 = 1 / 2π(103)(10-7)
= 1.59KΩ Since RFCF = R1C1
We get, CF = (1.59*103*10-7) / 15.9*103
= 0.01μF

![WhatsApp Image 2025-11-28 at 2 31 38 PM](https://github.com/user-attachments/assets/17ad9b9d-ae88-446b-bfa9-51eadff2b73b)

## PROCEDURE

1.	Connections are given as per the circuit diagram
2. + Vcc and - Vcc supply is given to the power supply terminal of the Op-Amp IC.
3.	By adjusting the amplitude and frequency knobs of the function generator, appropriate input voltage is applied to the inverting input terminal of the Op- Amp.
4.	The output voltage is obtained in the CRO and the input and output voltage waveforms are plotted in a graph sheet.

 ## TABULATION
 ![WhatsApp Image 2025-11-28 at 2 33 20 PM](https://github.com/user-attachments/assets/4622272a-0c5c-409b-947a-b56f4e1b9152)


## OUT PUT WAVEFORM AND DISCUSSION 

![WhatsApp Image 2025-11-28 at 2 30 16 PM](https://github.com/user-attachments/assets/e800a411-9478-4703-9332-43d683bac9b6)

---

RESULT:
Thus an Integrator and Differentiator using op-amp are designed and their performance was successfully tested using op-amp IC 741.
---

![WhatsApp Image 2025-11-28 at 2 34 05 PM](https://github.com/user-attachments/assets/be23333e-d05c-4a7a-aed9-e7d6606bcd2b)


