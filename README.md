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

**TRUTHTABLE**

![WhatsApp Image 2024-12-21 at 09 37 45_a2a231c4](https://github.com/user-attachments/assets/9ce1b53f-158f-49f7-b869-1c1ba3bc598e)

![WhatsApp Image 2024-12-21 at 09 36 50_733f2661](https://github.com/user-attachments/assets/f0fccd7b-76f4-4785-864c-cdb03e29d17e)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

i)HALF ADDER

module ha(a,b,sum,carry);

input a,b;

output sum,carry;

assign sum= (a ^ b);

assign carry= ( a & b);

endmodule

ii)HALF SUBTRACTOR

module hs(a,b,difference,borrow);

input a,b;

output difference,borrow;

assign difference= (a ^ b);

assign borrow= ( ~a & b);

endmodule


Developed by: Kaviya.V.M

RegisterNumber: 24900714

**RTL Schematic**

i.)HALF ADDER RTL

![half adder](https://github.com/user-attachments/assets/5deba570-6ec9-4aa3-8b80-98fa2b105f67)

ii.)HALF SUBRACTOR RTL

![subractor](https://github.com/user-attachments/assets/3897c95f-ecb2-408f-b6d3-ae66f856e099)


**Output**

i.)HALF ADDER WAVEFORM

![half adder waveform](https://github.com/user-attachments/assets/dad190ad-2ea6-46f0-a845-c3b96688dac0)

ii.)HALF SUBRACTOR WAVEFORM

![subractor waveform](https://github.com/user-attachments/assets/8e629f5e-9494-4d56-b779-ae1ec656b81f)


**Result:**

Thus the given half adder and half subtractor circuit is verified its truth table in Quartus using Verilog programming.
