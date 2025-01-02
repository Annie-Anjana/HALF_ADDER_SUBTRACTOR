# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**
FULL ADDER 
![image](https://github.com/user-attachments/assets/bab07b4f-fa9b-4f21-a77b-12ca88cfdee9)

FULL SUBTRACTOR
![image](https://github.com/user-attachments/assets/b9e958d5-cfb4-4971-9dba-19603af10d90)




**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

```
HALFSUBTRACTOR 
module HALFSUBTRACTORANDADDER(a,b,dif,bor);
 input a,b;
 output dif,bor;
 assign dif=a^b;
 assign x=~a;
 assign bor=b&x;
 endmodule 
HALFADDER
 module adder(a,b,v,j);
 input a,b;
 output v,j;
 assign v=a^b;
 assign j=a&b;
 endmodule
```

Developed by: ANNIE ANJANA A RegisterNumber:24010978

**RTL Schematic**
FULL ADDER
![image](https://github.com/user-attachments/assets/04927a85-028c-424e-b3e9-3d59ee6a9924)

FULL SUBTRACTOR
![image](https://github.com/user-attachments/assets/d1d73635-9057-4674-9725-51bce5e62acf)


**Output/TIMING Waveform**
FULL ADDER
![image](https://github.com/user-attachments/assets/25001916-7770-4b0d-8f44-f27c257babd2)

FULL SUBTRACTOR

![image](https://github.com/user-attachments/assets/0fa06dbc-b7de-4d6d-a498-452768b907c8)



**Result:**
Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is
 verified using Quartus software
