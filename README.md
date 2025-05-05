AIM:

To implement Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

SOFTWARE REQUIRED: Quartus prime

THEORY

Encoder 8 To 3

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/user-attachments/assets/8c78ee0d-6e50-4e0f-b71b-9dad5f69156b)


Figure 01 Block Diagram of Encoder 8 * 3

Truth Table

![image](https://github.com/user-attachments/assets/23234a6f-5f44-4fc3-b8e7-67b20be59e4e)



The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/user-attachments/assets/c2c83ad0-48ef-4fa6-9e91-293e47aed82e)


Figure 02 Encoder 8 * 3

Procedure

Step 1: Write the Truth Table

Step 2: Derive Boolean Expressions

Step 3: Write the Module Declaration

Step 4: Implement Dataflow Assignments

Step 5: Verify by Simulation (Optional but Recommended)

PROGRAM

Developed by: Madhumitha.B RegisterNumber:212224050018

Module enc(A0,A1,A2,D0,D1,D2,D3,D4,D5,D6,D7);
input A0,A1,A2;
output D0,D1,D2,D3,D4,D5,D6,D7;
assign A0= ( D4 | D5 | D6 | D7);
assign A1= ( D2 | D3 | D6 | D7);
assign A2= ( D1 | D3 | D5 | D7);
endmodule

![image](https://github.com/user-attachments/assets/7b4dc927-b4f2-46d2-b059-c104c0ab2084)


TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling

![image](https://github.com/user-attachments/assets/0540fcd9-51b1-4ebe-8e77-efb1d5425504)

RESULTS Thus the Encoder 8 To 3 in Dataflow Modelling using verilog are verified and the logic diagrams are designed and the truth table is verified.
