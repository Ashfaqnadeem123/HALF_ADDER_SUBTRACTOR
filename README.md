**EXP3: HALF ADDER AND SUBTRACTOR**

Name: Mohamed Ashfaq Nadeem A

reg no: 24000199

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

**Half Adder**

![Screenshot 2024-11-20 183951](https://github.com/user-attachments/assets/bfe3322f-77d3-44f4-8105-a260e97f9fbf)


**Half Subtractor**

![Screenshot 2024-11-20 184040](https://github.com/user-attachments/assets/9455457a-652e-4211-8f96-f41c8c83d0d2)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

**Half Adder**

module halfadd (
input a,b,    
output s,c   
);
xor gate_xor (s, a, b);  
and gate_and (c, a, b);  
endmodule

**Half Subtractor**

module halfsub(diff,borr,a,b);

input a,b;

output diff,borr;

wire w1;

xor g1(diff,a,b);

not g2(w1,a);

and g3(borr,w1,b);

endmodule


/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.



**RTL Schematic**

**Half Adder**

![Screenshot 2024-11-20 182026](https://github.com/user-attachments/assets/020300bc-bb95-44e9-b5b8-7ad564afea40)

**Half Subtractor**

![WhatsApp Image 2024-11-20 at 14 38 27_c12ad3e7](https://github.com/user-attachments/assets/48f926ca-ed06-47a9-b52b-c04a31fee761)



**Output/TIMING Waveform**

**Half Adder**

![Screenshot 2024-11-20 182148](https://github.com/user-attachments/assets/fdaac5fb-ce8c-4e3e-8b2b-299166f03bda)

**Half Subtractor**

![WhatsApp Image 2024-11-20 at 14 38 21_d76e3ae1](https://github.com/user-attachments/assets/4e259e24-3923-46e2-925b-8762cf8dd5e5)



**Result:**
Therefore  half adder and half subtractor circuit is studied and verified
