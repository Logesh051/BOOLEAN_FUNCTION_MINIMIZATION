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
Developed by: Logesh.N.A
RegisterNumber: 212223240078
*/
```
module booleanfunction(A,B,C,D,F1); 
input A,B,C,D; 
output F1; 
wire x1,x2,x3,x4,x5; 
assign x1=(~A)&(~B)&(~C)&(~D); 
assign x2=(A)&(~C)&(~D); 
assign x3=(~B)&(C)&(~D); 
assign x4=(~A)&(B)&(C)&(D); 
assign x5=(B)&(~C)&(D); 
assign F1=x1|x2|x3|x4|x5; 
endmodule 
```
![Screenshot 2024-04-27 104902](https://github.com/Logesh051/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979188/ec458d28-0128-4943-946a-7107acc0d77f)

**RTL realization**
![Screenshot 2024-04-27 104825](https://github.com/Logesh051/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979188/463e8bc1-eb4a-4b76-aab8-29cff37b0de0)

**Timing Diagram**
![316327286-79278d5e-3b0c-4a4a-9430-a2d49b7d385e](https://github.com/Logesh051/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979188/52552769-8352-40dc-a362-72a6317c382b)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

