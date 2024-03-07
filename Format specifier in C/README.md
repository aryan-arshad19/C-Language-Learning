Understanding Format Specifiers in C
---
Format specifiers in C are special characters used in functions like `printf()` and `scanf()` to specify the type of data being read or written. They tell the compiler how to interpret the data that needs to be formatted or read from the input.

Here are some common format specifiers and their usage:

1. **`%d`:** This specifier is used to represent integers. It is commonly used with `printf()` to display integer values.

   Example:
   ```c
   int num = 10;
   printf("The value of num is: %d\n", num);
   ```

2. **`%f`:** This specifier is used to represent floating-point numbers. It is commonly used with `printf()` to display floating-point values.

   Example:
   ```c
   float pi = 3.14159;
   printf("The value of pi is: %f\n", pi);
   ```

3. **`%c`:** This specifier is used to represent characters. It is commonly used with `printf()` to display characters.

   Example:
   ```c
   char ch = 'A';
   printf("The character is: %c\n", ch);
   ```

4. **`%s`:** This specifier is used to represent strings. It is commonly used with `printf()` to display strings.

   Example:
   ```c
   char str[] = "Hello, World!";
   printf("The string is: %s\n", str);
   ```

5. **`%p`:** This specifier is used to represent pointers. It is commonly used with `printf()` to display memory addresses.

   Example:
   ```c
   int *ptr;
   printf("The address of ptr is: %p\n", (void *)ptr);
   ```

6. **`%x` and `%X`:** These specifiers are used to represent hexadecimal numbers. `%x` displays lowercase hexadecimal digits while `%X` displays uppercase hexadecimal digits.

   Example:
   ```c
   int num = 255;
   printf("The hexadecimal representation of num is: %x\n", num);
   ```

