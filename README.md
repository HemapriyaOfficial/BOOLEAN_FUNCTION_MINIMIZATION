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

Developed by:Hemapriya.K 

RegisterNumber:212223040066
```
module Booleanexpressionmin(a,b,c,d,w,x,y,z,f1,f2); 
input a,b,c,d,w,x,y,z; 
output f1,f2; 
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u; 
not(adash,a); 
not(bdash,b); 
not(cdash,c); 
not(ddash,d); 
not(ydash,y); 
and(p,bdash,ddash); 
and(q,adash,b,d); 
and(r,a,b,cdash); 
or(f1,p,q,r); 
and(s,ydash,z); 
and(t,x,y); 
and(u,w,y); 
or(f2,s,t,u); 
endmodule
```

**RTL realization**

![322416806-a86b8a88-9cfd-46f7-a430-98227cff9fc4](https://github.com/HemapriyaOfficial/BOOLEAN_FUNCTION_MINIMIZATION/assets/147114275/b530c10e-1c34-4070-9f52-d23d3f1ffe08)

**Output:**
![Screenshot (54)](https://github.com/HemapriyaOfficial/BOOLEAN_FUNCTION_MINIMIZATION/assets/147114275/b5daa90e-6aea-483b-9aee-ad8fbbe55d9a)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

