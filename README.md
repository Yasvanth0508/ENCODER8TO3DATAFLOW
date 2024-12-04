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

**Procedure**

/* write all the steps invloved */

**PROGRAM**

/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 
```
module enc(a, b, c, y0, y1, y2, y3, y4, y5, y6, y7);
    input a, b, c;
    output y0, y1, y2, y3, y4, y5, y6, y7;

    assign y0 = ~a & ~b & ~c;
    assign y1 = ~a & ~b & c;
    assign y2 = ~a & b & ~c;
    assign y3 = ~a & b & c;
    assign y4 = a & ~b & ~c;
    assign y5 = a & ~b & c;
    assign y6 = a & b & ~c;
    assign y7 = a & b & c;
endmodule



Developed by:Yasvanth RD
RegisterNumber:24900517

```

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**

![WhatsApp Image 2024-12-04 at 14 24 04_48e07f88](https://github.com/user-attachments/assets/802a9128-36b5-4f74-a8b0-9de24db8ff13)

**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**

![WhatsApp Image 2024-12-04 at 14 24 03_9d7ce117](https://github.com/user-attachments/assets/d1e30d57-d32e-45e5-818a-624e479bd730)

**RESULTS**
Thus Encoder 8 to 3 designed and truthtable is verified.



