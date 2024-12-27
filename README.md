# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean function minimization is the process of simplifying a Boolean expression to use the fewest number of logic gates, variables, and operators. 

**Logic Diagram**

![TT](https://github.com/user-attachments/assets/642be207-4bc2-4ca3-a21d-3530d3926a6e)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. */
```
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule

```
```
Developed by: JOANN ELIZABETH SAMUEL
RegisterNumber: 24900609
```



**RTL realization**

![exp 2(1)](https://github.com/user-attachments/assets/da12accb-6dd8-40bb-bef8-8a2ae3044a00)
![exp 2(2)](https://github.com/user-attachments/assets/cef87916-7ff9-422c-a283-1894e2bcfbcd)



**Output:**

**RTL**

![image](https://github.com/user-attachments/assets/d6e9ffdf-76a1-46f3-99b1-2356a60dcea4)
![image](https://github.com/user-attachments/assets/ddaf0cb4-eeae-4336-9a11-aeb4969db9dd)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

