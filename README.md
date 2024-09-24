# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

Developed by: P. THIRUMALAI 


RegisterNumber: 24900297


**Program:**

module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);

input A,B,C,D,W,X,Y,Z;

wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;

output F1,F2;

assign x1=(~A)&(~B)&(~C)&(~D);

assign x2=(A)&(~C)&(~D);

assign x3=(~B)&(C)&(~D);

assign x4=(~A)&(B)&(C)&(D);

assign x5=(B)&(~C)&(D);

assign x6=(X)&(~Y)&(Z);

assign x7=(~X)&(~Y)&(Z);

assign x8=(~W)&(X)&(Y);

assign x9=(W)&(~X)&(Y);

assign x10=(W)&(X)&(Y);

assign F1=x1|x2|x3|x4|x5;

assign F2=x6|x7|x8|x9|x10;

endmodule


**RTL realization**

![EX2 LOGIC DIAGRAM (1)](https://github.com/user-attachments/assets/e1134829-3f1f-412e-a721-b3e16835c394)

**Logic symbol & Truthtable:**

![EX2 TABLE F1](https://github.com/user-attachments/assets/8793e451-e24e-4161-91b5-cb22c4ff1b13)
![EX2 TABLE](https://github.com/user-attachments/assets/414c5025-e6e0-443c-a9b1-5c66d19e7a66)

**Output**
![EX 2 OUTPUT DE](https://github.com/user-attachments/assets/667f12d0-eb72-47ef-bae5-2f7b2f975ef5)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

