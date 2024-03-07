
# 🔍 Getting to Know Variables in C

Some folks think variables in C are just names where we put values. But there's more to it!

In C:

- Variables hold different types of data (like numbers or letters).
- We have to tell C what type of data each variable will hold.
- Variables are like memory addresses where we store data.
- They only exist in certain parts of our program and for a specific time.
- They help us use memory wisely and write code that's easy to understand.

Here is an example of a variable given below:

```c
#include <stdio.h>

int main() {
    // Declare a variable of type integer named 'age'
    int age;

    // Assign a value to the variable 'age'
    age = 30;

    // Print the value of the variable 'age'
    printf("My age is: %d\n", age);

    return 0;
}
