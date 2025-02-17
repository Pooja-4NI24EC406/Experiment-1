# Experiment-1  
<body>
<center>
  <font color="black">
<h1> Problem 1</h1>
 <h2>DC, TRANSIENT AND AC ANALYSIS ON COMMON SOURCE AMPLIFIER USING MOSFET</h2>
 </font>
 </center>
 </body>
 <br>
 <h3>THEORY/INTRODUCTION </h3>  </br> 
     <br>
   AC, DC and transient analysis of common source amplifier. The circuit is designed using a MOSFET transistor, which operates in the saturation region to provide amplification.      
The Common Source (CS) MOSFET amplifier is one of the most widely used configurations in analog circuit design. It is used for voltage amplification and is commonly found in audio systems, RF amplifiers, and signal processing circuits.</br>
<br>
This report explains the theory, working, mathematical equations, and practical implementation on dc ac and transient analysis of this circuit.
</br>
<h3>CIRCUIT DAIGRAM</h3>

![1st circuit](https://github.com/user-attachments/assets/e782bc5f-df49-4a4e-840a-5448a22dd3d3)



 <h3> COMPONENTS(SYMBOLS) with VALUE/SPECIFICATIONS </h3>
 <p>
<br> power supply(VDD) - 12V,</br>
<br>  drain resistor(RD)-1k,</br>
 <br> mosfet(CMOSN)-NMOS4,</br>
 <br> input voltage(VIN)- ac signal</br>
 <br> ground-0v.</br>
 </p>



  <h3>Working principle</h3>
<h4>Operating Regions of MOSFET</h4>
A MOSFET has three major operating regions:
<br>1. Cutoff Region (Vgs < Vth ) ></Vth>– No current flows.    </br>
<br>2. Saturation Region ((Vgs>Vth and Vds>Vgs-Vth) – Amplification mode.</br>
<br>3. Ohmic/Linear Region ((Vgs>Vth and Vds<Vgs-Vth) ></Vgs-Vth>– Acts as a resistor.  </br>
For amplification, the MOSFET must operate in the saturation region.



 <h3>SOME IMP EQUATIONS/KEY EQUATIONS</h3> 

1. Overdrive Voltage

Vov=Vgs-Vth,    VGS = Gate-Source Voltage,      VTH = Threshold Voltage

2. Drain Current in Saturation Region,     I_D = 1/2kn(Vgs-Vth)^2      I_D = Drain current      kn= Process transconductance parameter

3. Voltage Gain (Av)     A_v = -Gm*Rd     gm=kn(Vgs-Vth)
 (Transconductance)    R_D = Drain resistor



<h3>Steps for LTSpice Simulation</h3>

<br>Step 1: Design the circuit in LTSpice</br>
<br>Step 2: Set the input voltage as an AC source.</br>
<br>Step 3: Run a DC, Transient, and AC Analysis to observe current and signal amplification.</br>
<br>Step 4: Verify the current and phase inversion in the waveform.</br>

<h3>DC ANALYSIS</h3>

![DC Analysis](https://github.com/user-attachments/assets/01ee2d9f-a943-4943-b484-2d63cd7a4095)

 <h3>CALCULATIONS</h3>
   <br>Given</br>
  <br> Vdd=1.8v</br>
   <br>R1=1.3k</br>
   <br>Vs=0v</br>
   <br>Vin(Vg)=0.9v</br>
   <br>P=100uW</br>
   <br>theoritical:</br>
   <br>P=V*I</br>
   <br>100uW=0.9v*I</br>
   <br>I=55.5uA</br>
   

   <br>FROM DC ANALYSIS OUTPUT:</br>
  <br> Vd(Vout)=1.73v
   Vg=0.9v
   Vs=0v
   Vgs=Vg-Vs
   Vgs=0.9v-0v=0.9v
   Vth=0.36V
   Vov=Vgs-Vth
   Vov=0.9-0.36=0.54V
   

<h3> TRANSIENT ANALYSIS</h3>

![transient analysis 11](https://github.com/user-attachments/assets/38deecdd-d963-449b-82f1-cd57f570572d)

![transient anasysis111](https://github.com/user-attachments/assets/744fd8d5-cf29-47e7-869f-f8537cd2f8d7)




<h3>AC ANALYSIS</h3>

![image](https://github.com/user-attachments/assets/d4fc52f5-d907-43de-a419-580e9fe24ed7)



<br>Av=Vout/Vin</br>
<br>Av=1.73/0.9</br>
<br>Av=1.92</br>
<br> practically: 2 dB</br>



<h3>RESULT</h3>
<br>Drain current is theoritical=55.5uA and practically in LTspice=55.5uA</br>
<br>Vov=0.54v      Vout=1.73v     Vth=0.36v
<br>AC Gain=1.92v
<br>The output waveform was inverted with respect to the input, here we observed the behavior of a common-source amplifier.</br>



<h3>INFERENCE</h3>
<br>After designing, analyzing, and simulating this circuit,</br>
<br>Current is calculated , theorical value is 55.5uA, after simulating in LTspice we get or setted as 55.54uA.The circuit provided a significant voltage amplification.</br>
<br>The gain was calculated and verified using LTSpice simulation.</br>
<br>The output waveform was inverted with respect to the input, here we observed the behavior of a common-source amplifier.</br>
<br>The current is calculated by using formula, Power is given,so P=V*I, for amplifieng current is always in saturation region I_D = 1/2kn(Vgs-Vth)^2.</br>
<br>The voltage gain gepends on the transconductance and drain resistor Av=-Gm*Rd. LTSpice simulation results match with theoretical calculations.</br>


<h3>Final Conclusion</h3>
<p>This experirement demonstrated the working of a common source amplifier and verified it circuit by analyzing and simulating. The result shows that this amplifier is effective for voltage amplication. Hence proved by simulating in LTSpice.</p>


<h2>PROBLEM 2</h2>
<h3> Theory</h3>
<p> Analysis of cmos inverter( PMOS and CMOS) this circuit consist both CMOS transistor and PMOS transistor CMOS inverter is the fundamental of logic gates.</p>
<h3>CIRCUIT DAIGRAM</h3>

![image](https://github.com/user-attachments/assets/b4ad8698-9859-4bf2-9d7c-f908b7aae2ba)

<h3>Simulation</h3>

<br>Step 1: Design the circuit in LTSpice</br>
<br>Step 2: Set the input voltage as an AC source.</br>
<br>Step 3: Run a DC, Transient, and AC Analysis to observe current and signal amplification.</br>
<br>Step 4: Verify the current and phase inversion in the waveform.</br>


<h3>DC ANALYSIS</h3>

![image](https://github.com/user-attachments/assets/c748f36f-0023-474a-8f3f-a81ee41b9f07)

 <h3>CALCULATIONS</h3>
   <br>Given</br>
  <br> Vdd=1.8v</br>
   <br>V1(Vb)=0.48v</br>
   <br>Vs=0v</br>
   <br>V2=0.9v</br>
   <br>P=100uW</br>
   <br>theoritical:</br>
   <br>P=V*I</br>
   <br>100uW=0.9v*I</br>
   <br>I=55.5uA</br>
   

   <br>FROM DC ANALYSIS OUTPUT:</br>
  <br> Vd(Vout)=1.73v
   Vg=0.9v
   Vs=0v
   Vgs=Vg-Vs
   Vgs=0.9v-0v=0.9v
   Vtn=0.36V
   Vtp=-0.39v
   Vov=Vgs-Vtn
   Vov(NMOS)=0.9-0.36=0.54V
   Vov=Vsg-Vtp
   Vov(PMOS)=0-0.9=-0.9v</ br>

<h3>TRANSIENT ANALYSIS</h3>

![image](https://github.com/user-attachments/assets/c17543a3-0276-4666-b4ac-a574b3d9c08e)



![image](https://github.com/user-attachments/assets/4c93dae8-2785-4169-8ec3-155302cb7f04)

<h3>AC ANALYSIS</h3>

![image](https://github.com/user-attachments/assets/561b4fef-c36a-4441-a07e-c85c81c12bfd)

<br>Av=Vout/Vin</br>
Av= 3.7 dB


<h3>RESULT </h3>
<br>Drain current is theoritical=55.5uA and practically in LTspice=55.54uA</br>
<br>Vov=0.54v      Vout=1.73v     Vth=0.36v</br>
<br>AC Gain=3.7dB
<br>The output waveform was inverted with respect to the input,and observed amplified signal</br>

<h3>INFERENCE</h3>
<br>designed and analyzed and also simulated two MOSFET circuit,</br>
<br>Caculated current is same because of same power, theorical value is 55.5uA,practically or setted as 55.54uA by adjusting or changing the length (L) value. output is amplified with respect to input.</br>
<br>The gain was calculated and verified using LTSpice simulation.
here practically gain is 3.74 dB</br>
<br>The output waveform was inverted with respect to the input in transient analysis</br>

<h3>COMPARISON BETWEEN PROBLEM 1 and PROBLEM 2</h3>
<br> Common source with Rd and two MOSFETS's</br>
| Common source with Rd | Two MOSFET' |
|-----------------------|--------------------|
| A single MOSFET with a drain resistor RD in the drain branch | two MOSFET's configured in a common source |
|Id=55.5uA|Id=55.5uA|
|single MOSFET for amplification|two mosfets one May act as a cascade or a load|
|Power=100uA|Here power is taken as same 100uA|
|W=180nV and L=0.2uV|W=180nV L=0.3uV|
|Practically Av=2dB| Av=3.7dB|
|it is mainly used for basic analog amplification audio signals|it is used for high frequency amplification and RF circuits and low noise amplification|




    
