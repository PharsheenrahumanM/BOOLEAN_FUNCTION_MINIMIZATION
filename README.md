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

Developed by: RegisterNumber:*/212224230193
# F1
module booleanfn(a,b,c,d,f1);
 input a,b,c,d;
 output f1;
 assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
 endmodule
# F2

 module booleanfnb(w,x,y,z,f2);
 input w,x,y,z;
 output f2;
 assign f2=((~y & z)|(w & y)|(x & y));
 endmodule


**RTL realization**
**F1**
![DE2F1D](https://github.com/user-attachments/assets/4db0926a-4beb-438f-927e-aa0733fdd006)
**F2**
![DE2BDIA](https://github.com/user-attachments/assets/f614c15b-de9d-47f8-8563-3dd0d3de7be7)

**Output:**
**F1**
![DE2F2OUT](https://github.com/user-attachments/assets/53b66bba-2648-4942-ada4-935eeb16a76f)

**F2**
![EXP2BDEOUT](https://github.com/user-attachments/assets/f1b1259a-6816-44ce-9fda-68938d1c7362)


**RTL**

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

