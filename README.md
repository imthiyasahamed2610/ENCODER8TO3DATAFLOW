### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

**Proceduer**
1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.

PROGRAM

**PROGRAM**
module enc(a,b,c,y0,y1,y2,y3,y4,y5,y6,y7);

input y0,y1,y2,y3,y4,y5,y6,y7;

output a,b,c

assign a= ( y4 | y5 | y6 | y7);

assign b= ( y2 | y3 | y6 | y7);

assign c= ( y1 | y3 | y5 | y7);

endmodule




Developed by:imthiyas ahamed .m RegisterNumber:212224050012
*/

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**
![389431286-4a77680c-9d91-4796-9aa8-4eabe2be70be](https://github.com/user-attachments/assets/73c1c3f6-d842-4fb6-909a-96beeefa8617)

**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**
![389431336-953e0aa0-527c-44e7-8ef4-e226901b1a4b](https://github.com/user-attachments/assets/9111386c-7423-45b8-ad93-4e793a5f05b7)

**RESULTS**

 Thus the ENCODER 8TO3 DATAFLOW Modelling are studied and the truth tables are verified.




