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
```
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: MANOJ G
RegisterNumber:  2122222240060
*/

Half adder program:

module fulladd (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule

Full adder program:

module fulladd (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
```
Logic symbol & Truthtable
RTL realization

### Output:
### RTL
HALF ADDER
![image](https://user-images.githubusercontent.com/69635071/234767065-6290c6c9-7191-44a2-873c-f346f6645fc2.png)

FULL ADDER
![image](https://user-images.githubusercontent.com/69635071/234767150-42fab4a7-79fd-4122-9c9d-095889e43ce8.png)

### TIMING DIAGRAM
HALF ADDER
![image](https://user-images.githubusercontent.com/69635071/234767347-6cccbb43-17aa-4d5d-8dac-5d5d6974c6da.png)

FULL ADDER
![image](https://user-images.githubusercontent.com/69635071/234767428-5417f145-a1bd-4392-a097-1710c6c291e9.png)



### TRUTH TABLE 
HALF ADDER

![image](https://user-images.githubusercontent.com/69635071/234767533-018261f1-229d-43d3-b172-f48681826210.png)


FULL ADDER
![image](https://user-images.githubusercontent.com/69635071/234767606-a14e13cb-03db-48f2-aaed-9893f7cd38e6.png)


### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
