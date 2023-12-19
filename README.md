# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:

Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: ARAVIND R
RegisterNumber: 23005371
~~~
module exp2(a,b,c,d,f1,f2);
input a,b,c,d;
output f1,f2;
wire adash,bdash,cdash,ddash,x,y,z,p,q,r;
not(avdash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
and(x,bdash,ddash);
and(z,a,b,cdash);
and(y,adash,b,d);
or(f1,x,y,z);
and(p,cdash,d);
and(q,a,c);
and(r,b,c);
or(f2,p,q,r);
endmodule
~~~
## RTL realization
![image](https://github.com/ARAVIND23005370/Experiment--02-Implementation-of-combinational-logic-/assets/148514836/a33d324e-7ce3-4f03-84ac-41cd80efaf11)

## Output:
![image](https://github.com/ARAVIND23005370/Experiment--02-Implementation-of-combinational-logic-/assets/148514836/aff1796e-510b-4736-848d-b17d4734ac8b)

## Timing Diagram
## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
