EXP 03:HALF_ADDER_SUBTRACTOR

  
NAME:NAVEENKUMAR

REF NO:24900580

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

**Half Subtractor:**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

**HALF SUBTRACTOR:**


![Screenshot 2024-11-15 143300](https://github.com/user-attachments/assets/70beab9b-90b5-4c65-86e6-4c2691961de7)


**HALF ADDER**

![Screenshot 2024-11-15 144408](https://github.com/user-attachments/assets/9ecf5b07-1c99-4523-9337-80a222f88101)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

**HALF SUBTRACTOR:**

module exphs(diff,borr,a,b);

input a,b;

output diff,borr;

wire w1;

xor g1(diff,a,b);

not g2(w1,a);

and g3(borr,w1,b);

endmodule 
**HALF ADDER**

module exphs(Ssum,cout,a,b);

input a,b;

output sum,cout;

xor g1(sum,a,b);

and g3(conta,b);
Developed by: RegisterNumber:249200580

**RTL Schematic:**

**HALF SUBTRACTOR:**
<img src="https://github.com/user-attachments/assets/5947c09e-bd9a-4270-b3e5-bf5db99c63dd" width="600" height="500"/>



**HALF ADDER**
<img src="https://github.com/user-attachments/assets/43dab650-b727-4fed-acdc-3f187779a087" width="600" height="500"/>



**Output/TIMING**

**HALF SUBTRACTOR:**

<img src="https://github.com/user-attachments/assets/c0ec367d-9e54-4c02-b79d-fed3ae9365f6" width="600" height="500"/>


 
 **HALF ADDER**
<img src="https://github.com/user-attachments/assets/c99caf84-60b9-4f34-b104-f4431ee5aa58" width="600" height="500"/>



**Result:**

   Thus to  design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.


