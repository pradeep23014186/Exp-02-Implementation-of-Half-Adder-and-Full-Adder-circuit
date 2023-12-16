# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

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
Developed by: Pradeep Kumar.G
RegisterNumber:23014186
```
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

1.Program to design a half adder:
module ex3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=a^b;
assign carry=a&b;
endmodule

1.Program to design a full adder:
module ex31(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=a^b^cin;
assign carry=(a&b)|((a^b)&cin);
endmodule
```
### Output:
### RTL realization:
## HALF ADDER:
![image](https://github.com/pradeep23014186/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152294642/78816ebb-baf5-4004-9429-67bc6b4da357)
## FULL ADDER:
![image](https://github.com/pradeep23014186/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152294642/01805649-55a3-488b-be05-beb218a4ae92)

### TIMING DIAGRAM
## HALF ADDER:
![image](https://github.com/pradeep23014186/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152294642/752b323f-f637-4d7b-850d-2b595ad26a0b)
## FULL ADDER:
![image](https://github.com/pradeep23014186/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152294642/3b9d0e6a-ccdf-452c-ad80-acd9751b0e4b)

### TRUTH TABLE 
## HALF ADDER:
![image](https://github.com/pradeep23014186/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152294642/aa828c97-9df0-4f20-b714-f907084d0897)
## FULL ADDER:
![image](https://github.com/pradeep23014186/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152294642/bb3f3e3a-a3ea-48d9-9b88-e606a87f43e7)


### Result:
Thus the half adder and full adder circuit are designed and the truth table for half adder and full adder are verified.
