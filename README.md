<img width="3024" height="4032" alt="2im1" src="https://github.com/user-attachments/assets/677dc6f8-71fb-4f3d-b9b1-91ee98332256" /># BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**
<img width="3024" height="4032" alt="2im1" src="https://github.com/user-attachments/assets/2f2417b5-b8cf-4b2f-93bd-cd73ddedc85c" />

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
~~~
Developed by:Branzen B V 
RegisterNumber:212225100005
~~~
~~~
Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
module de2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule
~~~



**RTL realization**
<img width="503" height="489" alt="2im2" src="https://github.com/user-attachments/assets/d1d8fa8d-add1-4d28-8f30-44600d91842f" />

**Output:**
<img width="1306" height="643" alt="2im3" src="https://github.com/user-attachments/assets/5eaffed4-8f2e-4a75-81d9-5a1624da14dc" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

