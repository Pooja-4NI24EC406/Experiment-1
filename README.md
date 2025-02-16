# Experiment-1  
<body>
<center>
  <font color="pink">

 <h1>DC, TRANSIENT AND AC ANALYSIS ON COMMON SOURCE AMPLIFIER USING MOSFET</h1>
 </font>
 </center>
 </body>
 <br>
 <h2> INTRODUCTION </h2>  </br> 
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
 power supply(VDD) - 12V,
 drain resistor(RD)-1K,
 mosfet(CMOSN)-NMOS4,
 input voltage<VIN) - AC signal,
 ground-0v.
 </p>

   <h3>CALCULATIONS</h3>



   
  <h3>WORKING PRINCIPLE</h3>
<h4>Operating Regions of MOSFET</h4>
A MOSFET has three major operating regions:
<br>1. Cutoff Region (Vgs<Vth) – No current flows.</br>
<br>2. Saturation Region ((Vgs>Vth and Vds>Vgs-Vth) – Amplification mode.</br>
<br>3. Ohmic/Linear Region ((Vgs>Vth and Vds<Vgs-Vth) – Acts as a resistor.</br>
For amplification, the MOSFET must operate in the saturation region.

 <h3>SOME IMP EQUATIONS/KEY EQUATIONS</h3> 

1. Overdrive Voltage

V_{OV} = V_{GS} - V_{Th},    VGS = Gate-Source Voltage,      VTH = Threshold Voltage

2. Drain Current in Saturation Region,     I_D = 1/2kn(Vgs-Vth)^2      I_D = Drain current      kn= Process transconductance parameter

3. Voltage Gain (Av)     A_v = - g_m R_D     gm=kn(V_{GS} - V_{Th}
 (Transconductance)    R_D = Drain resistor

<h3>Steps for LTSpice Simulation</h3>

<br>Step 1: Design the circuit in LTSpice</br>

<br>Step 2: Set the input voltage as an AC source.</br>

<br>Step 3: Run a DC, Transient, and AC Analysis to observe current and signal amplification.</br>

<br>Step 4: Verify the current and phase inversion in the waveform.</br>

<h3>DC ANALYSIS</h3>
![DC Analysis](https://github.com/user-attachments/assets/01ee2d9f-a943-4943-b484-2d63cd7a4095)



<h3> TRANSIENT ANALYSIS</h3>
![transient analysis 11](https://github.com/user-attachments/assets/38deecdd-d963-449b-82f1-cd57f570572d)
![transient anasysis111](https://github.com/user-attachments/assets/744fd8d5-cf29-47e7-869f-f8537cd2f8d7)




<h3>AC ANALYSIS</h3>
![AC Analysis](https://github.com/user-attachments/assets/e2d11372-e388-4a51-ac51-9d647d97937f)



<h3>RESULT</h3>
After designing, analyzing, and simulating this circuit, the following results were observed:
<br>1. Voltage Gain ():
<p>The circuit provided a significant voltage amplification.
The gain was calculated using  and verified using LTSpice simulation.</p></br>
<br>2. Phase Inversion:
<p>The output waveform was inverted with respect to the input, confirming the expected behavior of a common-source amplifier.</p><br>
<br>3. Current Characteristics:
<p>The drain current () followed the quadratic relationship in the saturation region:
 I_D = 1/2kn(Vgs-Vth)^2</p></br>
 <br>4. Simulation Results (LTSpice Analysis):
<p>The transient analysis showed a clear amplification of the input AC signal.
The output voltage amplitude was higher than the input, confirming the amplifier's functionality.</p></br>

<h3>INFERENCE</h3>
<br>Based on the experimental and simulation results, the following conclusions were drawn:

The Common Source MOSFET Amplifier successfully amplifies small AC signals, making it ideal for analog signal processing.

The output is phase-inverted, which aligns with theoretical expectations

The voltage gain depends on the transconductance () and the drain resistor (), allowing for design flexibility.

The MOSFET operates in the saturation region, ensuring a stable amplification process.

The LTSpice simulation results match theoretical calculations, confirming the circuit's validity.</br>

<h3>Final Conclusion</h3>
<p>This experiment demonstrated the working of a Common Source MOSFET Amplifier and verified its performance through mathematical analysis and circuit simulation. The results show that this amplifier configuration is effective for voltage amplification in electronic circuits.</p>






    
