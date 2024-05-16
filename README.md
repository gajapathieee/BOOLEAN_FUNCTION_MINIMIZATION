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


Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
Developed by: j.gajapathi
RegisterNumber: 2122223002
```
```
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
```
## Logic symbol & Truthtable:
![exp 2 truth table 1](https://github.com/23003250/BOOLEAN_FUNCTION_MINIMIZATION/assets/139331462/a6b8101c-bd3c-4b64-bc4a-f4a8962ac13a)
![exp 2 truth table 2](https://github.com/23003250/BOOLEAN_FUNCTION_MINIMIZATION/assets/139331462/348e89c8-b4d6-4c9e-8783-541ac0829105)

## RTL realization Output:
![RTL OUTPUT 2](https://github.com/23003250/BOOLEAN_FUNCTION_MINIMIZATION/assets/139331462/be51436b-369d-4d09-b411-d66fb1a3d375)

## RTL
![waveform exp 2](https://github.com/23003250/BOOLEAN_FUNCTION_MINIMIZATION/assets/139331462/b42d8d42-def2-4ec7-a4a0-baeb043c7949)

## Result:
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

