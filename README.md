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

**Truth table**

1.F1

![image](https://github.com/user-attachments/assets/2566cd5d-e645-4df4-bd3e-6222a20a397f)

2.F2

![image](https://github.com/user-attachments/assets/5f6816a1-680a-44bf-bcdd-82807c1386eb)

**Boolean Function Minimization**

1.F1

![WhatsApp Image 2024-12-21 at 03 26 32_16197669](https://github.com/user-attachments/assets/ad9ecd38-0cb9-488a-b529-c4289bc9a09f)

2.F2

![WhatsApp Image 2024-12-21 at 03 26 45_2b131323](https://github.com/user-attachments/assets/af8088e0-0789-4ff4-9e0d-06bd2fec0789)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

F1

```
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```

F2

```
module funct2(w,x,y,z,f2);
intput w,x,y,z;
output f2;
assign f2=((~y & z)|(w & y)|(x &y));
endmodule
```

Developed by:ASHIKA TR
RegisterNumber:24900481


**RTL**

1.F1

![WhatsApp Image 2024-12-10 at 20 48 09_63d2ef5a](https://github.com/user-attachments/assets/fcd0e1f9-b197-4436-8282-352acff21e5a)


2.F2

![WhatsApp Image 2024-12-10 at 20 48 16_de2ef258](https://github.com/user-attachments/assets/1cdb0fba-53ec-498b-9b1e-6eacd7d4802a)


**Timing Diagram**

1.F1

![WhatsApp Image 2024-12-10 at 20 40 29_84a69ba6](https://github.com/user-attachments/assets/41904ea2-1b71-457f-afe7-74efa689da51)


2. F2

![WhatsApp Image 2024-12-10 at 20 48 20_26d6e794](https://github.com/user-attachments/assets/4c9e2ce8-0fd5-4360-acd1-100d6cad3ef7)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

