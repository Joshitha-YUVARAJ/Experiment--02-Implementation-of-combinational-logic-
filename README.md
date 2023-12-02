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
A combinational circuit in which the output depends on the present combination of inputs.Comdinational circuit are made up of logic gates. The output of each logic gate is determined by its logic function.Combinational circuits can be made using various logic gates ,such as AND gates,OR gates and NOT gates.
 


## Program:

/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

Developed by:YUVARAJ JOSHITHA

RegisterNumber:  23011447

```
module verilog1(a,b,c,d,w,x,y,z,F1,F2);
input a,b,c,d,w,x,y,z;
output F1,F2;
wire A1,A2,A3,A4,A5,B1,B2,B3,B4,B5;
assign A1=(~a&(~b)&(~C)&(~d));
assign A2=(a&c&(~d));
assign A3=((~b)&c&(~d));
assign A4=(~a&b&c&d);
assign A5=(b&(~c)&d);
assign F1=A1|A2|A3|A4|A5;
assign B1=(x&(~y)&z);
assign B2=(~x&(~y)&z);
assign B3=(~w&x&y);
assign B4=(w&(~x)&y);
assign B5=(w&y&z);
assign F2=B1|B2|B3|B4|B5;
endmodule
```

*/

## Output:

## Truth Table

![Screenshot 2023-12-02 214727](https://github.com/Joshitha-YUVARAJ/Experiment--02-Implementation-of-combinational-logic-/assets/145742770/7df34acb-d7dc-491e-9d5e-f02582e2b895)

![Screenshot 2023-12-02 214752](https://github.com/Joshitha-YUVARAJ/Experiment--02-Implementation-of-combinational-logic-/assets/145742770/15e586f7-fc68-4fa7-b81a-76110299e373)



## RTL realization

![Screenshot 2023-12-02 214812](https://github.com/Joshitha-YUVARAJ/Experiment--02-Implementation-of-combinational-logic-/assets/145742770/a48f0310-0271-49ef-bdf2-b9ad91e70ad4)



## Timing Diagram

![Screenshot 2023-12-02 214831](https://github.com/Joshitha-YUVARAJ/Experiment--02-Implementation-of-combinational-logic-/assets/145742770/731b643e-acd7-433c-8803-44a94fb0f8c7)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
