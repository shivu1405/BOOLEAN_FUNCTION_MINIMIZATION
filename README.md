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
i)
module DE2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

ii)
module DE2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:SHIVASRI S
RegisterNumber:24006106


**RTL realization**
![image](https://github.com/user-attachments/assets/94ada76c-8c62-41de-a10e-cea52b46387e)
![image](https://github.com/user-attachments/assets/9940c4f6-069e-4ff8-9ae7-abb518184dfb)


**WAVEFORM**
![image](https://github.com/user-attachments/assets/c2aa78fd-313b-452c-b7fd-0b573bda6e5b)
![image](https://github.com/user-attachments/assets/2577a12b-1996-4b93-9b8f-95faf6eb6e6a)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
