# BOOLEAN_FUNCTION_MINIMIZATION
```
Developed by: MADHESH I
RegisterNumber:212224220055
```

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

![Screenshot 2024-12-05 132633](https://github.com/user-attachments/assets/d1be5cca-6e87-4144-9a1a-342a042ee182)

![Screenshot 2024-12-10 143326](https://github.com/user-attachments/assets/f29977cb-6ea0-48b0-ab53-12bc3551a29a)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

module funct2(w,x,y,z,f2);
 input w,x,y,z;
 output f2;
 assign f2=((~y & z)|( w & y )|(x & y));
 endmodule
```
![Screenshot 2024-12-10 143546](https://github.com/user-attachments/assets/77370a30-9f80-4508-8218-bf2e034b3ef7)


![Screenshot 2024-12-10 143554](https://github.com/user-attachments/assets/9014b1a8-cb45-4a34-94d6-6bb139a23e05)

**RTL realization**

![Screenshot 2024-12-10 143736](https://github.com/user-attachments/assets/7b660fe9-b1c3-42a4-9179-bd2456925065)


![Screenshot 2024-12-10 143739](https://github.com/user-attachments/assets/44729912-7de1-4b73-9369-348271800c49)


**Output:**

**RTL**

![Screenshot 2024-12-10 143736](https://github.com/user-attachments/assets/7b660fe9-b1c3-42a4-9179-bd2456925065)

![Screenshot 2024-12-10 143739](https://github.com/user-attachments/assets/44729912-7de1-4b73-9369-348271800c49)

**Timing Diagram**

![Screenshot 2024-12-10 143827](https://github.com/user-attachments/assets/d146538d-60d6-4d9d-acf5-64ae5e330faa)

![Screenshot 2024-12-10 143833](https://github.com/user-attachments/assets/8af8e7c3-efd0-4cb8-861e-42733abd2fe9)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

