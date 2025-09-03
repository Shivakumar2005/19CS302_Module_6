# EX 29 C program to create two float variables using calloc() and find minimum among them.
## DATE:03/09/2025
## AIM:
To write a C program to create two float variables using calloc() and find minimum among them.

## Algorithm
1. Start the program.
2. Allocate memory for two float variables using calloc().
3. Read two float numbers from the user.
4. Compare the two numbers and find the minimum. 
5. Display the minimum number.  

## Program:
#include <stdio.h>
#include <stdlib.h>

int main() {
    float *a;
    a = (float *)calloc(2, sizeof(float));
    printf("Enter two float numbers: ");
    scanf("%f %f", &a[0], &a[1]);
    if (a[0] < a[1])
        printf("Minimum = %.2f\n", a[0]);
    else
        printf("Minimum = %.2f\n", a[1]);
    free(a);
    return 0;
}


## Output:

<img width="1364" height="568" alt="image" src="https://github.com/user-attachments/assets/70d2bf2c-260d-4143-a7f2-d48f9ff64b30" />


## Result:
Thus the program was executed and the output was verified successfully.
