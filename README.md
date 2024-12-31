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

![Screenshot 2024-12-24 123731](https://github.com/user-attachments/assets/89012c12-c6bf-479d-ac24-e7f9be52f5aa)



2.F2

![image](https://github.com/user-attachments/assets/5f6816a1-680a-44bf-bcdd-82807c1386eb)

**Boolean Function Minimization**

1.F1

![WhatsApp Image 2024-12-21 at 03 26 32_16197669](https://github.com/user-attachments/assets/ad9ecd38-0cb9-488a-b529-c4289bc9a09f)

2.F2

![WhatsApp Image 2024-12-21 at 03 26 53_e454fce8](https://github.com/user-attachments/assets/d352442c-2c59-4ae2-8689-a659eab56cb1)


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

![WhatsApp Image 2024-12-24 at 12 44 47_6fc5deeb](https://github.com/user-attachments/assets/71b1076d-f96d-43d7-8493-1528c6fe3906)



2. F2

![WhatsApp Image 2024-12-31 at 09 12 53_7a80457f](https://github.com/user-attachments/assets/c707e4f7-b747-48ca-aa0a-9e6d191606e0)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

