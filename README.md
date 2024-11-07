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
Developed by:Hemakesh G 
RegisterNumber:212223040064
```
```
module de_exp_2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d) | (a & b & ~c) | (~a & b & d));
endmodule
```
```
module proj23(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2= ((~y&z)|(w&y)|(x&y));
endmodule
```

**Truth Table:**

*F1*

![2 1 truth table](https://github.com/user-attachments/assets/6a3f7a61-4175-4183-bb22-e91ce1e5bfea)

*F2*

![2 2 truth table](https://github.com/user-attachments/assets/a94b9962-e99c-4028-a265-5c906cca8121)


**RTL:**

*F1*
![Screenshot 2024-09-13 093739](https://github.com/user-attachments/assets/14fd6235-76f8-4953-b16d-cb6df525c75e)
*F2*
![image](https://github.com/user-attachments/assets/e48183a0-2f82-432d-86b7-556d8b32b9dd)



**Timing Diagram:**

*F1*
![Screenshot 2024-09-13 095350](https://github.com/user-attachments/assets/1b416323-e578-499c-9147-a1f2514fbbcb)
*F2*
![image](https://github.com/user-attachments/assets/5ad1ecc7-e1e3-4352-9f83-298cd33bb95b)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

