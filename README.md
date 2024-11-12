# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


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


Developed by:**KARTHICK R**

RegisterNumber**24900278**


**RTL realization**
![image](https://github.com/user-attachments/assets/17ff06c2-7377-4e67-b71e-0a3b35fd5d9f)

**TRUTH TABLE**
![image](https://github.com/user-attachments/assets/d5d276cf-fe9c-46e9-8c51-dfa4646e634c)

![image](https://github.com/user-attachments/assets/d0bc7a24-d0aa-43cd-bb9c-5b4469d46849)


**Output:**

![image](https://github.com/user-attachments/assets/c650d007-7b74-458e-9437-e7dff29f0da8)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

