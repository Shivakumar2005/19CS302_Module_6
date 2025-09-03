# EX 28 C program that demonstrates the use of enum (enumeration) type to define and use named integer constants.
## DATE:03/09/2025
## AIM:
To write a C program that demonstrates the use of enum (enumeration) type to define and use named integer constants.

## Algorithm
1. Start the program.
2. Define an enumeration type with named integer constants.
3. Declare a variable of that enumeration type.
4. Assign a value from the enumeration to the variable. 
5. Display the value using printf.  

## Program:
#include <stdio.h>

enum Weekday {Sunday, Monday, Tuesday, Wednesday, Thursday, Friday, Saturday};

int main() {
    enum Weekday today;
    today = Wednesday;
    printf("Day number: %d\n", today);
    return 0;
}


## Output:

<img width="1422" height="561" alt="image" src="https://github.com/user-attachments/assets/8c6bcc8d-b4e1-421e-a2ca-f3a8377b1cc7" />


## Result:
Thus the program was executed and the output was verified successfully.
