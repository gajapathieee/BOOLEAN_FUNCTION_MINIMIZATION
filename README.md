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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming.


Developed by: j.gajapathi
RegisterNumber:212222053004
Department: AIDS
```
module ex02(a,b,c,d,w,x,y,z,f1,f2); 
input a,b,c,d,w,x,y,z;
output f1,f2; 
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u; 
not(adash,a); not(bdash,b); not(cdash,c);
 not(ddash,d);
 and(p,bdash,ddash);
 and(q,adash,b,d);
 and(r,a,b,cdash); 
 or(f1,p,q,r);
 not(ydash,y); 
 and(s,ydash,z); 
 and(t,x,y);
 and(u,w,y); 
 or(f2,s,t,u);
 endmodule
 ```


**RTL realization**
![321126891-6165149e-5930-46f3-97f2-4ef97728ce65](https://github.com/23008859/BOOLEAN_FUNCTION_MINIMIZATION/assets/139117979/b1ea3887-5333-47de-92d8-a30f47240bd1)

**Output:**
![321126914-a1aacc77-a0d6-4887-8d75-f4e34f93b122](https://github.com/23008859/BOOLEAN_FUNCTION_MINIMIZATION/assets/139117979/619349cf-9261-468c-b105-426bcfa9b849)

**RTL**
![image](https://github.com/23008859/BOOLEAN_FUNCTION_MINIMIZATION/assets/139117979/923cfcf3-b058-4405-a7d4-7a1c21869366)


**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

