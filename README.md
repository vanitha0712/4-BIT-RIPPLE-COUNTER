# 4-BIT-RIPPLE-COUNTER

**AIM:**

To implement  4 Bit Ripple Counter using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 Bit Ripple Counter**

A binary ripple counter consists of a series connection of complementing flip-flops (T or JK type), with the output of each flip-flop connected to the Clock Pulse input of the next higher-order flip-flop. The flip-flop holding the least significant bit receives the incoming count pulses. The diagram of a 4-bit binary ripple counter is shown in Fig. below.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/cb4b74d4-31ab-4359-95d0-d22e67daba13)

In timing diagram Q0 is changing as soon as the negative edge of clock pulse is encountered, Q1 is changing when negative edge of Q0 is encountered(because Q0 is like clock pulse for second flip flop) and so on.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/a573a7d6-014e-4e54-93e6-e2ac9530960b)

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/85e1958a-2fc1-49bb-9a9f-d58ccbf3663c)

**Procedure**

/* write all the steps invloved */

**PROGRAM**

/* Program for 4 Bit Ripple Counter and verify its truth table in quartus using Verilog programming.

 Developed by:B.VANITHA RegisterNumber:25014805
*/
module exp_6(out,clk,rst); 
 input clk,rst; 
 output reg [3:0]out; 
 always @ (posedge clk)
 begin 
 if(rst) 
 out<=0; 
 else 
 out <= out-1; 
 end endmodule

**RTL LOGIC FOR 4 Bit Ripple Counter**
<img width="1395" height="777" alt="Screenshot 2026-03-12 111934" src="https://github.com/user-attachments/assets/5240d49c-42d2-49b0-888b-fb7011b80c7b" />

**TIMING DIGRAMS FOR 4 Bit Ripple Counter**
<img width="1392" height="731" alt="Screenshot 2026-03-12 112058" src="https://github.com/user-attachments/assets/a124950e-564b-473d-96e0-e1a65590b60e" />

**RESULTS**
