# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: OVIYA P
RegisterNumber:  23013207

## HALFADDER CODE:

module Halfadder(sum,a,b,carry);

input a,b;

output sum,carry;

xor(sum,a,b);

and(carry,a,b);

endmodule

## TRUTH TABLE FOR HALFADDER:

![image](https://github.com/Oviya24032K6/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147139999/b78f1155-a978-4332-87c3-43dc2ad8c540)

## RTL VIEWER FOR HALFADDER:

![image](https://github.com/Oviya24032K6/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147139999/f040d1d6-8d5f-4002-986c-7e764397962b)

## OUTPUT FOR HALFADDER:

![image](https://github.com/Oviya24032K6/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147139999/e43d3836-8bd2-492d-b9bf-64d88da17c59)

## CODE FOR FULLADDER:

module fulladder(a,b,c,sum,carry);

input a,b,c;

output sum,carry;

xor(sum,a,b,c);

assign carry=a&b | b&c| a&c;

endmodule

## TRUTH TABLE FOR FULLADDER:

![image](https://github.com/Oviya24032K6/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147139999/ff754a1c-68e9-4848-9eb4-09b97b81708a)

## RTL VIEWER FOR FULLADDER:

![image](https://github.com/Oviya24032K6/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147139999/5a28cb14-7807-4be8-88c2-9eeba16489bd)

## OUTPUT FOR FULLADDER:
![image](https://github.com/Oviya24032K6/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147139999/0a90102c-f677-425a-a2a5-72a26ac534ed)


### Result:

Thus the given half adder and full adder are verified using verilog programming
