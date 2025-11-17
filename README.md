# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean function minimization is the process of simplifying complex Boolean expressions to their most efficient form while preserving their logical function. The goal is to reduce the number of logic gates, literals, and wiring needed for implementation in digital circuits, leading to lower costs, improved speed, and reduced power consumption.

**Logic Diagram**

<img width="800" height="241" alt="image" src="https://github.com/user-attachments/assets/24d10dc4-b8d3-4863-a61b-005f89422bbb" />


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
~~~
module DAY5(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
~~~
**RTL realization**

**Output:**

**RTL**
<img width="1920" height="1080" alt="Screenshot (60)" src="https://github.com/user-attachments/assets/690cfd1e-d944-4f93-879b-b88a153c2cee" />

**Timing Diagram**
<img width="1920" height="1080" alt="Screenshot (61)" src="https://github.com/user-attachments/assets/96216a6b-4111-4b01-b870-adc0da217d6a" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

