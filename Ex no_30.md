# EX 30 C program to add two integer elements in an array using realloc() and that array already has three elements.
## DATE:03/09/2025
## AIM:
To write a C program to add two integer elements in an array using realloc() and that array already has three elements.

## Algorithm
1. Start the program.
2. Allocate memory for 3 integer elements and read their values
3. Use realloc() to increase the size of the array to hold 5 integers.
4. Read the two new elements and add them to the array. 
5. Display all the 5 elements.  

## Program:
#include <stdio.h>
#include <stdlib.h>

int main() {
    int *arr, i;
    arr = (int *)malloc(3 * sizeof(int));
    printf("Enter 3 integers: ");
    for(i = 0; i < 3; i++)
        scanf("%d", &arr[i]);

    arr = (int *)realloc(arr, 5 * sizeof(int));
    printf("Enter 2 more integers: ");
    for(i = 3; i < 5; i++)
        scanf("%d", &arr[i]);

    printf("Array elements are: ");
    for(i = 0; i < 5; i++)
        printf("%d ", arr[i]);

    free(arr);
    return 0;
}


## Output:

<img width="1622" height="741" alt="image" src="https://github.com/user-attachments/assets/d783e706-8871-4cbd-82a4-c030fef152e5" />


## Result:
Thus the program was executed and the output was verified successfully.
