# EX 27 C program that demonstrates the use of typedef to create a new alias name for a data type.
## DATE:03/09/2025
## AIM:
To write a C program that demonstrates the use of typedef to create a new alias name for a data type.

## Algorithm
1. Start the program.
2. Define a new alias name for a data type using typedef.
3. Declare variables using the alias.
4. Assign values to the variables. 
5. Display the values using printf.  

## Program:
#include <stdio.h>

// create a new alias name
typedef unsigned int uint;

int main() {
    uint a, b;  // using the typedef alias for unsigned int
    a = 25;
    b = 50;

    printf("Value of a: %u\n", a);
    printf("Value of b: %u\n", b);

    return 0;
}

## Output:

<img width="1311" height="576" alt="image" src="https://github.com/user-attachments/assets/a1a1af75-2c90-468d-b761-b19bb9d7e769" />


## Result:
Thus the program was executed and the output was verified successfully.
