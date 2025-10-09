### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

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

/* write all the steps invloved */

**PROGRAM**

/* Program for flipflops and verify its truth table in quartus using Verilog programming. 

Developed by: RegisterNumber:
*/

**RTL LOGIC UP COUNTER**

**TIMING DIAGRAM FOR IP COUNTER**

**TRUTH TABLE**

**RESULTS**
<img width="1920" height="1080" alt="exe6(1)" src="https://github.com/user-attachments/assets/2e0f0f69-b66b-49e8-a569-3ac669537ded" />
![ex6(2)](https://github.com/user-attachments/assets/70ac1547-e685-434a-acb3-2693a33ffd9e)
![ex6(3)](https://github.com/user-attachments/assets/06808dc5-9e01-48b3-8271-53d19a93a329)
<img width="1920" height="1080" alt="exe6(1)" src="https://github.com/user-attachments/assets/9e90001a-4d38-409c-9d13-18f99631528b" />
<img width="1920" height="1080" alt="exe6(1)" src="https://github.com/user-attachments/assets/65ba5dd9-1f0b-4155-90f4-cc221cdd4609" />
