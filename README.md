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

**Minimization**
**F1**
![jo 1](https://github.com/user-attachments/assets/5290d5f2-b7ff-4233-8d9c-50c0a5d4bceb)

**F2**
![jo2](https://github.com/user-attachments/assets/00e83349-95fd-41bd-8202-96f5a908624b)

**Truth table**

![JO3](https://github.com/user-attachments/assets/41794594-a6f8-4a3b-9c88-48b65c72ca38)

![JO4](https://github.com/user-attachments/assets/768428a6-871b-45ff-b3dd-b30fd3318a1b)



**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
```
module funct1(a,b,c,d,f1);
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

Developed by:JOANN ELIZABETH SAMUEL
RegisterNumber: 24900609


**RTL**

![Screenshot 2024-12-28 192105](https://github.com/user-attachments/assets/1dcf3336-b2fb-4415-b0de-6f33a39753cb)


**Output**

![jo5](https://github.com/user-attachments/assets/56501447-f145-4162-9f23-ddbcf045bd88)

![jo6](https://github.com/user-attachments/assets/f2be49ab-c51c-4131-89b8-ffbcbfcb4b15)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


