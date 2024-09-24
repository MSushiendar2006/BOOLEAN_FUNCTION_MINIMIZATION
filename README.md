# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module boolean_minimization(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);

and g1(s,ydash,z);
and g2(t,x,y);
and g3(u,w,z);
or g4(f2,s,t,u);
endmodule
```

Developed by: RegisterNumber:*/
```
SUSHIENDAR M
212223040217
```


**RTL realization**
![image](https://github.com/user-attachments/assets/0db1359e-0350-44cf-83ca-1198df2f85d3)


**Truth Table:**
![image](https://github.com/user-attachments/assets/f9a04093-2abb-45bb-afa3-22b8ab9d30f0)



**Timing Diagram**
![image](https://github.com/user-attachments/assets/ba0cf797-64b8-47f9-976b-0604eb6d1942)


**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

