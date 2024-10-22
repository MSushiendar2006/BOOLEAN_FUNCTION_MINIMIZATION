## BOOLEAN_FUNCTION_MINIMIZATION

## AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.
F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 
F2=xy’z+x’y’z+w’xy+wx’y+wxy

## Equipment Required:

Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime*

## Theory:

## Procedure:

1.	Type the program in Quartus software.
2.	Compile and run the program.
3.	Generate the RTL schematic and save the logic diagram.
4.	Create nodes for inputs and outputs to generate the timing diagram.
5.	For different input combinations generate the timing diagram.

## Program:
```
F1:
module boolenminization(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=(~a)&(~b)&(~c)&(~d)|(a)&(~c)&(~d)|(~b)&(c)&(~d)|(~a)&(b)&(c)&(d)|(b)&(~c)&(d);
endmodule
```

```
F2:
module boolenminization2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=(x)&(~y)&(z)|(~x)&(~y)&(z)|(~w)&(x)&(y)|(w)&(~x)&(y)|(w)&(x)&(y);
endmodule
```



## Developed by:
```
Name: SUSHIENDAR M
Register Number: 212223040217
```

## Truth Table:
![image](https://github.com/user-attachments/assets/b50d871a-a694-4788-82b5-4cf55e1f47d9)

![image](https://github.com/user-attachments/assets/596a05f6-f99a-4fc9-8ee4-569fadfaa5de)


## RTL:
```
F1:
```
![image](https://github.com/user-attachments/assets/0c62e091-eea1-4a4f-ba9c-84f271e05c67)

```
F2:
```
![image](https://github.com/user-attachments/assets/2aefecf8-0bfe-46b2-b77b-6588ccfe16e2)

## Output:
```
F1
```
![h6nclv7b](https://github.com/user-attachments/assets/babd04c2-8f1c-4c3b-8df8-8874a6959fef)

```
F2
```
![image](https://github.com/user-attachments/assets/e89ffaa3-3d13-45ee-b299-df0a67f14703)




## Result:
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

