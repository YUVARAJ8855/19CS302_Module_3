# EX 11 C Program to convert a given decimal value to binary using function without arguments with return type.
## DATE:
## AIM:
To write a C Program to convert a given decimal value to binary using function without arguments with return type.

## Algorithm
1. Start. 
2. Declare a integer variable 
3. Define a function named dectobin. 
4. Return the integer. 
5. Read the value using scanf. 
6. Convert decimal to binary value. 
7. Print the dectobin 
8. End.  

## Program:
```
#include<stdio.h> 
Int dectobin(int d){ 
int bin =0,base=1,rem; 
while(d>0) 
{ 
rem=d%2; 
bin=bin+rem*base; 
d=d/2; 
base=base*10; 
} 
printf(" = %d in binary",bin); 
return 0; 
} 
int main() 
{ 
int dec; 
scanf("%d",&dec); 
printf("%d in decimal",dec); 
dectobin(dec); 
return 0; 
} 
```

## Output:

![image](https://github.com/user-attachments/assets/8eb65410-5976-47a3-ad83-2ac8ef34868b)


## Result:
Thus the program was executed and the output was verified successfully.
