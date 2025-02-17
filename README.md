# Experiment-1  
<body>
<center>
  <font color="black">

 <h1>DC, TRANSIENT AND AC ANALYSIS ON COMMON SOURCE AMPLIFIER USING MOSFET</h1>
 </font>
 </center>
 </body>
 <br>
 <h2>THEORY/INTRODUCTION </h2>  </br> 
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
<br> power supply(VDD) - 12V,
 drain resistor(RD)-1K,
 mosfet(CMOSN)-NMOS4,
 input voltage<VIN) - AC signal,
 ground-0v.</br>
 </p>

  <h3>Working principle</h3>
<h4>Operating Regions of MOSFET</h4>
A MOSFET has three major operating regions:
<br>1. Cutoff Region (Vgs<Vth) – No current flows.</br>
<br>2. Saturation Region ((Vgs>Vth and Vds>Vgs-Vth) – Amplification mode.</br>
<br>3. Ohmic/Linear Region ((Vgs>Vth and Vds<Vgs-Vth) – Acts as a resistor.</br>
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
   <br>Given
   Vdd=1.8v
   R1=1.3k
   Vs=0v
   Vg=0.9v

   FROM DC ANALYSIS OUTPUT:
   Vd(Vout)=
   Vg=0.9v
   Vs=0v
   Vgs=Vg-Vs
   Vgs=0.9v-0v=0.9v
   Vth=
   Vov=Vgs-Vth
   Vov=
   

<h3> TRANSIENT ANALYSIS</h3>

![transient analysis 11](https://github.com/user-attachments/assets/38deecdd-d963-449b-82f1-cd57f570572d)

![transient anasysis111](https://github.com/user-attachments/assets/744fd8d5-cf29-47e7-869f-f8537cd2f8d7)




<h3>AC ANALYSIS</h3>

![AC Analysis](https://github.com/user-attachments/assets/e2d11372-e388-4a51-ac51-9d647d97937f)




<h3>RESULT</h3>
Drain current is theoritical=55.5uA and practically in LTspice=54.44uA
Vov=       Vout=     Vth=
AC Gain=
The output waveform was inverted with respect to the input, here we observed the behavior of a common-source amplifier.
After designing, analyzing, and simulating this circuit, the following results were observed:
Current is calculated , theorical value is 55.5uA, after simulating in LTspice we get or setted as 54.44uA.The circuit provided a significant voltage amplification.
The gain was calculated and verified using LTSpice simulation.
The output waveform was inverted with respect to the input, here we observed the behavior of a common-source amplifier.
 I_D = 1/2kn(Vgs-Vth)^2
 <br>4. Simulation Results (LTSpice Analysis):
<p>The transient analysis showed a clear amplification of the input AC signal.
The output voltage amplitude was higher than the input, confirming the amplifier's functionality.</p></br>

<h3>INFERENCE</h3>
<br>After designing, analyzing, and simulating this circuit,
Current is calculated , theorical value is 55.5uA, after simulating in LTspice we get or setted as 54.44uA.The circuit provided a significant voltage amplification.
The gain was calculated and verified using LTSpice simulation.
The output waveform was inverted with respect to the input, here we observed the behavior of a common-source amplifier.
The current is calculated by using formula, Power is given,so P=V*I, for amplifieng current is always in saturation region I_D = 1/2kn(Vgs-Vth)^2
The voltage gain gepends on the transconductance and drain resistor Av=-Gm*Rd. LTSpice simulation results match with theoretical calculations.</br>


<h3>Final Conclusion</h3>
<p>This experirement demonstrated the working of a common source amplifier and verified it circuit by analyzing and simulating. The result shows that this amplifier is effective for voltage amplication. Hence proved by simulating in LTSpice.</p>






    
