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

 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:212223230079
//Program to compute the function f1=a'b'c'd'+ac'd'+b'cd'+a'bcd+bc'd
//f2=xy'z+x'y'z+w'xy+wx'y+wxy
module boolean(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1 = (~A)&(~B)&(~C)&(~D);
assign x2 = (A)&(~C)&(~D);
assign x3 = (~B)&(C)&(~D);
assign x4 = (~A)&(B)&(C)&(D);
assign x5 = (B)&(~C)&(D);
assign F1 = x1|x2|x3|x4|x5;
endmodule 

```
![Screenshot 2024-03-18 045749](https://github.com/hindhujanaki/BOOLEAN_FUNCTION_MINIMIZATION/assets/148514666/e44321b4-5d6b-4ff9-94a8-b06024dcb2ac)

**RTL realization**
![Screenshot 2024-03-18 045846](https://github.com/hindhujanaki/BOOLEAN_FUNCTION_MINIMIZATION/assets/148514666/55c71391-e729-450c-862e-32fc28bb56bf)

**Output:**

![Screenshot 2024-03-18 050814](https://github.com/hindhujanaki/BOOLEAN_FUNCTION_MINIMIZATION/assets/148514666/74614d8b-3b8a-42b0-9232-cdec511be4c4)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

