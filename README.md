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
module logic_functions(
input  a, b, c, d,
input  w, x, y, z,
output f1, f2
);

assign f1 = (~b & ~d) |
            (a & b & ~c) |
            (~a & b & d);

assign f2 = (~y & z) | (w & y);
endmodule


```




Developed by: A Amal Tony Charles RegisterNumber:25016419

logic symbol and truth table 

<img width="805" height="442" alt="image" src="https://github.com/user-attachments/assets/591f866e-a2d9-403d-96ca-ce75eef75779" />
<img width="797" height="421" alt="image" src="https://github.com/user-attachments/assets/9dc4a816-f1d2-4adb-8cbe-c98be48d7dbf" />




**RTL realization**
<img width="1607" height="866" alt="Screenshot 2025-12-02 105446" src="https://github.com/user-attachments/assets/4eeafaa3-151a-4239-8549-98cc53bed43f" />


**Output:**
<img width="1920" height="1080" alt="Screenshot 2025-12-02 110557" src="https://github.com/user-attachments/assets/d95a9314-f075-464a-912b-06dea24d86bf" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

