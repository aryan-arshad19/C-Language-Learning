***Scanf Function in C***


The `scanf()` function in C is used to read formatted input from the standard input stream, typically the keyboard, and store the values into variables. It belongs to the standard input/output library `<stdio.h>`. Here's a breakdown of how it works:

**Basic Syntax:**
```c
#include <stdio.h>

int main() {
    int integerVariable;
    float floatVariable;
    char characterVariable;

    // Reading integer input
    printf("Enter an integer: ");
    scanf("%d", &integerVariable);

    // Reading float input
    printf("Enter a float: ");
    scanf("%f", &floatVariable);

    // Reading character input
    printf("Enter a character: ");
    scanf(" %c", &characterVariable); 
    // Note the space before %c to consume any whitespace or newline characters

    // Displaying the inputs
    printf("You entered: %d, %f, %c\n", integerVariable,floatVariable, characterVariable);

    return 0;
}
```

- `%d` is the format specifier for integers.
- `%f` is the format specifier for floating-point numbers.
- `%c` is the format specifier for characters.
- `&` is the address-of operator used to pass the address of the variables where `scanf()` should store the input values.

**Important Points:**
- `scanf()` stops reading input as soon as it encounters whitespace (spaces, tabs, newlines).
- It's crucial to handle newline characters (`\n`) that might be left in the input buffer by preceding input operations.
- Always check the return value of `scanf()` to ensure that the input was successfully read.

**Error Handling Example:**
```c
#include <stdio.h>

int main() {
    int num;
    printf("Enter an integer: ");
    if (scanf("%d", &num) == 1) {
        printf("You entered: %d\n", num);
    } else {
        printf("Invalid input\n");
    }
    return 0;
}
```
This code checks if `scanf()` successfully reads an integer value. If it does, it proceeds to print the input; otherwise, it notifies the user about the invalid input.

In summary, `scanf()` is a fundamental function in C for reading formatted input, and understanding its usage is essential for interactive console applications.