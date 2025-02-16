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

<th>
  <tr>
    <td>component</td>
  </tr>

 <tr>
   <td>power supply
   </td>
 </tr>

 <h3> COMPONENTS(SYMBOLS) with VALUE/SPECIFICATIONS </h3>
 <p>
 power supply(VDD) - 12V,
 drain resistor(RD)-1K,
 mosfet(CMOSN)-NMOS4,
 input voltage<VIN) - AC signal,
 ground-0v.
 </p>
 4. Working Principle

<h3>Operating Regions of MOSFET</h3>
<h4>A MOSFET has three major operating regions:</h4>
<br>1. Cutoff Region (Vgs<Vth) – No current flows.</br>
<br>2. Saturation Region ((Vgs>Vth and Vds>Vgs-Vth) – Amplification mode.</br>
<br>3. Ohmic/Linear Region ((Vgs>Vth and Vds<Vgs-Vth) – Acts as a resistor.</br>
For amplification, the MOSFET must operate in the saturation region.

    
