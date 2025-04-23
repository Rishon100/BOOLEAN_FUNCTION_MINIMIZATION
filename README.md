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
```
module exp2(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire w1,w2,w3;
assign w1=(~B)&(~D);
assign w2=(~A)&(B)&(~C);
assign w3=(A)&(B)&(~C);
assign F1=w1|w2|w3;
endmodule
```

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/


**RTL realization Output:**
![Screenshot 2025-04-11 143553](https://github.com/user-attachments/assets/2c14d749-6ab6-4ba1-8a66-a9ff40e289b7)

**RTL**
![Screenshot 2025-04-11 143713](https://github.com/user-attachments/assets/0e459015-f1f2-4e20-9608-34322c68a0ec)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

