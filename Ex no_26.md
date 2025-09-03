# EX 26 C program demonstrating a self-referential structure where an employee has a pointer to their manager.
## DATE:03/09/2025
## AIM:
To write a C program to demonstrate a self-referential structure where an employee has a pointer to their manager.

## Algorithm
1. Start the program.
2. Define a self-referential structure Employee with members: name, id, and a pointer to another Employee (manager).
3. Declare employee variables and assign manager pointers accordingly.
4. Initialize the employee details including linking employees to their managers.
5. Display the employee’s details along with their manager’s details.  

## Program:
#include <stdio.h>

struct Employee {
    char name[50];
    int id;
    struct Employee *manager;
};

int main() {
    struct Employee e1 = {"Arjun", 101, NULL};
    struct Employee e2 = {"Priya", 102, &e1};
    struct Employee e3 = {"Kumar", 103, &e1};

    printf("Employee: %s, ID: %d, Manager: %s\n", e1.name, e1.id, "None");
    printf("Employee: %s, ID: %d, Manager: %s\n", e2.name, e2.id, e2.manager->name);
    printf("Employee: %s, ID: %d, Manager: %s\n", e3.name, e3.id, e3.manager->name);

    return 0;
}


## Output:

<img width="1628" height="662" alt="image" src="https://github.com/user-attachments/assets/a3d937d9-3cfc-4316-b4e9-15f043ba6dba" />


## Result:
Thus the program was executed and the output was verified successfully.
