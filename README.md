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
module de2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule
```


**RTL realization**
<img width="589" height="578" alt="image" src="https://github.com/user-attachments/assets/6359514c-f733-48da-baa3-7caa6b3cebcd" />

**Output:**
**RTL**

<img width="1238" height="618" alt="image" src="https://github.com/user-attachments/assets/3b8251a2-ba81-47a5-9dfd-9371d06a1fdc" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

