# BOOLEAN_FUNCTION_MINIMIZATION

**Develope4d by:**V Rishon Anand

**RegisterNumber:**212224240135

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
module boolean(A,B,C,D,F2);
input A,B,C,D;
output F2;
wire w1,w2,w3;
assign w1=(~B)&(~D);
assign w2=(~A)&(B)&(~C);
assign w3=(A)&(B)&(~C);
assign F2=w1|w2|w3;
endmodule
```
```
module boolean(W,X,Y,Z,F2);
input W,X,Y,Z;
output F2;
wire w1,w2,w3;
assign w1=(~Y)&(Z);
assign w2=(X)&(Y);
assign w3=(W)&(Y);
assign F2=w1|w2|w3;
endmodule
```


/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 




**RTL realization output:**

![Screenshot 2025-04-11 143553](https://github.com/user-attachments/assets/ffc57109-8f71-4cc1-8127-bcbf62dcdbb1)

![Screenshot 2025-04-23 141913](https://github.com/user-attachments/assets/64f5865e-3298-4e49-af98-0db7217feaaa)

**RTL**

![Screenshot 2025-04-11 143713](https://github.com/user-attachments/assets/8520d757-5d6c-4463-bee9-170c3c6868e7)

![Screenshot 2025-04-23 142433](https://github.com/user-attachments/assets/40c205d2-1448-4865-b048-4310e20e2ff5)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

