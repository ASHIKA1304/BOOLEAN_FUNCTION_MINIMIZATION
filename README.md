BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean Algebra is a branch of algebra that deals with boolean values-true and false.It is fundamental to digital logic design and computer science,providing a mathamatical framework for describing logical operation and expressions.

**Logic Diagram**
![image](https://github.com/user-attachments/assets/a719d34c-9d03-4c54-a46e-9750f06be6b3)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:ASHIKA TR
RegisterNumber:24900481
```
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```

```
module funct2(w,x,y,z,f2);
intput w,x,y,z;
output f2;
assign f2=((~y & z)|(w & y)|(x &y));
endmodule
```

**Output:**

**RTL**

Boolean function minimization f1

![WhatsApp Image 2024-12-10 at 20 48 09_63d2ef5a](https://github.com/user-attachments/assets/fcd0e1f9-b197-4436-8282-352acff21e5a)


Bollean function minimization f2

![WhatsApp Image 2024-12-10 at 20 48 16_de2ef258](https://github.com/user-attachments/assets/1cdb0fba-53ec-498b-9b1e-6eacd7d4802a)


**Timing Diagram**

Boolean function minimization f1

![WhatsApp Image 2024-12-10 at 20 40 29_84a69ba6](https://github.com/user-attachments/assets/41904ea2-1b71-457f-afe7-74efa689da51)


Boolen function minimization f2

![WhatsApp Image 2024-12-10 at 20 48 20_26d6e794](https://github.com/user-attachments/assets/4c9e2ce8-0fd5-4360-acd1-100d6cad3ef7)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

