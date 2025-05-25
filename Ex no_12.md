# EX 12 C program to check whether the given number is prime or not using function without return type and with arguments.
## DATE:
## AIM:
To write a C program to check whether the given number is prime or not using function without return type and with arguments.

## Algorithm
1. Start
2. Define function checkPrime(num)
If num <= 1, print "not a prime" and exit function
3. Initialize isPrime = 1
4. Loop from i = 2 to num / 2
5. If num % i == 0, set isPrime = 0 and break
6. If isPrime == 1, print "prime"
Else, print "not prime"
7. In main(), read number n
8. Call checkPrime(n)
9. End
## Program:
```
#include <stdio.h>
void checkPrime(int num) {
    int i, isPrime = 1;
    if (num <= 1) {
        printf("%d is not a prime number.\n", num);
        return;
    }
    for (i = 2; i <= num / 2; i++) {
        if (num % i == 0) {
            isPrime = 0;
            break;
        }
    }
    if (isPrime)
        printf("%d is a prime number.\n", num);
    else
        printf("%d is not a prime number.\n", num);
}
int main() {
    int n;
    printf("Enter a number: ");
    scanf("%d", &n);
    checkPrime(n);
    return 0;
}
```

## Output:

![image](https://github.com/user-attachments/assets/76e3ce58-a543-4099-b915-204e6a0c1330)


## Result:
Thus the program was executed and the output was verified successfully.
