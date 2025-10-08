### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**
4 bit synchronous UP Counter

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

image

image

Each flip-flop in this circuit will be clocked at exactly the same time. The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.” Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse. Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time. The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed. However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**
1.Open Quartus software and create a new Verilog file. Paste the code and save it.
2.Compile the program to check for errors.
3.Generate the RTL schematic via the RTL Viewer and save the logic diagram.
4.Use the Waveform Editor to assign nodes for clk, rstn, and out.
5.Simulate the design with different clk and rstn combinations to generate the timing diagram, and save the results.
/* write all the steps invloved */

**PROGRAM**

<img width="475" height="240" alt="Screenshot 2025-10-08 193518" src="https://github.com/user-attachments/assets/6569d8b0-806c-4d99-a85f-e09de548cc4a" />

/* Program for flipflops and verify its truth table in quartus using Verilog programming. 

Developed by: RegisterNumber:J.Ivan Abishek Benhannan

25006144
*/

**RTL LOGIC UP COUNTER**
<img width="1781" height="873" alt="Screenshot 2025-10-08 193503" src="https://github.com/user-attachments/assets/285a646f-407f-413d-b00e-7c5286566391" />


**TIMING DIAGRAM FOR IP COUNTER**
<img width="1028" height="575" alt="Screenshot 2025-10-08 193814" src="https://github.com/user-attachments/assets/13936754-fed2-4785-812d-626723f74009" />


**TRUTH TABLE**

<img width="675" height="338" alt="Screenshot 2025-10-08 194321" src="https://github.com/user-attachments/assets/6d4134ee-d76f-4ac3-9b36-b0392f7f21aa" />


**RESULTS**
Thus the Synchronous 3 bit Up counter is implemeted and verified.
