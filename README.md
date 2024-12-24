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
![384846756-52062f5d-0af3-425d-9e67-15bf399c40d6](https://github.com/user-attachments/assets/17ef44b9-6cc3-496f-85fd-10a721aff333)
![384847121-2ce86520-018e-4e38-b8c4-f7e9e23ad23c](https://github.com/user-attachments/assets/56965040-823b-4497-a77b-e8c7605513fc)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

```
module ex03(a,b,cy, sm, df,bo);
input a,b;
output sm,cy, df, bo;
xor(sm,a,b);
and(cy,a,b);
xor(df,a,b);
and (bo,~a,b);
endmodule
```
Developed by: RegisterNumber:*/24005701

**RTL Schematic**
![384845325-91131b39-f8d4-4a44-a4c5-d42a6c545db0](https://github.com/user-attachments/assets/e47c1394-7975-43ce-bf2d-3c8ee3ea90f1)

**Output/TIMING Waveform**
![384845794-c21117da-14d5-40f5-b056-5a00ce2d03cb](https://github.com/user-attachments/assets/5321db78-f4c1-4797-bef0-e0b48d293e06)

**Result:**
Thus the Half Adder and Half Subtractor circuits are designed and the truth tables is verified using Quartus software.
