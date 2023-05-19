# Implementation of Logic Gates using Verilog HDL
## Aim
To implement and to verify the truth table in Verilog HDL for the following logic gates 
1.	AND gate
2.	 OR gate
3.	 NOT gate 
4.	 NAND gate
5.	 NOR gate
6.	 Ex-OR gate
7.	 Ex-NOR gates 

## Components Required:
1.	Laptop with Quartus software and modelsim software

## Theory
## Introduction
Logic gates are the basic building blocks of any digital system. Logic gates are electronic circuits having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic. 


1) AND gate
The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB
	Y= A.B
![image](https://github.com/rvinifa/ex1final/assets/133735746/0b3bb617-91e2-48cb-b076-0ee1a72e0479)

  





2) OR gate
The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation.

  Y= A+B

![image](https://github.com/rvinifa/ex1final/assets/133735746/68debf78-a4f1-47a5-9dba-0220a8c3f537)
 




3) NOT gate

The NOT gate is an electronic circuit that produces an inverted version of the input at its output. It is also known as an inverter. If the input variable is A, the inverted output is known as NOT A. This is also shown as A' or A with a bar over the top, as shown at the outputs.

Y= A'
![image](https://github.com/rvinifa/ex1final/assets/133735746/bfb047a9-0077-4164-bd7d-3972a1b5f997)


 




4) NAND gate
This is a NOT-AND gate which is equal to an AND gate followed by a NOT gate. The outputs of all NAND gates are high if any of the inputs are low. The symbol is an AND gate with a small circle on the output. The small circle represents inversion.

Y= (AB)’
![image](https://github.com/rvinifa/ex1final/assets/133735746/f103398b-56bf-43d0-a454-c611aa79ce1e)



 



5) NOR gate

This is a NOT-OR gate which is equal to an OR gate followed by a NOT gate. The outputs of all NOR gates are low if any of the inputs are high. The symbol is an OR gate with a small circle on the output. The small circle represents inversion.


Logic Symbol							Truth Table
Y= (A+B)’

 ![image](https://github.com/rvinifa/ex1final/assets/133735746/22a03cab-dc44-4a49-a293-b03dfd4b586e)





6) Ex-OR gate

The 'Exclusive-OR' gate is a circuit which will give a high output if either, but not both of its two inputs are high. An encircled plus sign (⊕) is used to show the Ex-OR operation.


Logic Symbol							Truth Table
Y= A⊕B
![image](https://github.com/rvinifa/ex1final/assets/133735746/cf18ea9e-7d95-4416-bd1d-350141b010c2)

 











7) Ex-NOR gate

The 'Exclusive-NOR' gate circuit does the opposite to the EX-OR gate. It will give a low output if either, but not both of its two inputs are high. The symbol is an EX-OR gate with a small circle on the output. The small circle represents inversion.


Logic Symbol						Truth Table
Y= A⊕B

![image](https://github.com/rvinifa/ex1final/assets/133735746/f5fc7782-e4a7-47d1-b596-394835324213)
 






## Procedure:
1.	Type the program in Quartus software.
2.	Compile and run the program.
3.	Generate the RTL schematic and save the logic diagram.
4.	Create nodes for inputs and outputs to generate the timing diagram.
5.	For different input combinations, generate the timing diagram.

## Program:
module Exp1(a,b,andgate,notgate,orgate,nandgate,norgate,xorgate,xnorgate);
input a,b;
output andgate,orgate,notgate,norgate,nandgate,xorgate,xnorgate;
and(andgate,a,b);
or(orgate,a,b);
not(notgate,a);
nand(nandgate,a,b);
nor(norgate,a,b);
xor(xorgate,a,b);
xnor(xnorgate,a,b);
endmodule



## RTL Schematic:
![exp1 (2)](https://github.com/ragavanayyadurai/exp1/assets/118749557/e43b0c61-07d9-493e-a2e5-6dd2206af97e)

## Timing Diagram:
![exp1](https://github.com/ragavanayyadurai/exp1/assets/118749557/7c048271-6b19-4f4d-bfd9-9a7731cd013a)



## Result:

Thus the different logic gates are implemented in Verilog HDL and the truth table are verified.



