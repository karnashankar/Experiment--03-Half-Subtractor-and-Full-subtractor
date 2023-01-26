# Experiment--03-Half-Subtractor-and-Full-subtractor
## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory
Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.

## Half Subtractor Full Subtractor
## Half Subtractor
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.
![half-subtractor9](https://user-images.githubusercontent.com/36288975/166112538-58c3bc7c-ee5d-4e6a-ac8d-8e8328efe27a.png)


Sum = X'Y+XY' = X ⊕ Y
Carry=X'Y

## Full Subtractor
A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow. 
![full-subtractor6](https://user-images.githubusercontent.com/36288975/166112541-24c68359-3de8-4674-ae22-8272ffc385ed.png)


Diff = A ⊕ B ⊕ Bin B = A'Bin + A'B + BBin

## Procedure
##### 1.Use module projname(input,output) to start the Verilog programmming.
##### 2.Assign inputs and outputs using the word input and output respectively.
##### 3.Use defined keywords like wire,assign and required logic gates to represent the boolean expression.
##### 4.Use each output to represnt onre for differnce and the other for borrow.
##### 5.End the verilog program using keyword endmodule.


## Program:

##### Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
##### Developed by: karna s
##### RegisterNumber: 22008977 



<img width="579" alt="image" src="https://user-images.githubusercontent.com/121109150/214821753-d96d4ab2-8d77-4a6e-a233-211dcaf9df3f.png">

## Output:

## Truthtable
#### Half Subtractor Truth Table:
![image](https://user-images.githubusercontent.com/121109150/214821929-5ba5f304-de22-4797-bf0f-20a97c211e87.png)
#### Full subtractor truth table:
![image](https://user-images.githubusercontent.com/121109150/214822004-d96ccf55-a34c-4d8f-9a0f-321733107ae3.png)

##  RTL realization
#### Half subtractor:
![image](https://user-images.githubusercontent.com/121109150/214822123-2904bb9c-09be-4c9c-bb2f-381e867b51b6.png)

#### Full subtractor:
![image](https://user-images.githubusercontent.com/121109150/214822192-fd1c7919-9f02-4828-9aa4-329cf74acec5.png)

## Timing diagram 
#### Half subtractor:
![image](https://user-images.githubusercontent.com/121109150/214822315-66f18562-6cf0-489c-bee0-b85cb5103679.png)
#### Full subtractor:
![image](https://user-images.githubusercontent.com/121109150/214822414-841f7abd-02f2-440d-ba5c-fbed97691f2a.png)


## Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
