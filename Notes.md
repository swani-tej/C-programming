

---

## 1. Introduction to C Programming

* **What is C?**
  C is a general-purpose, procedural programming language developed by Dennis Ritchie in 1972 at Bell Labs.
* **Features of C:**

  * Simple and efficient
  * Portable
  * Structured programming language
  * Rich library functions
  * Low-level manipulation capability
* **Uses of C:** System programming, Embedded systems, OS development, Compilers, etc.

---

## 2. Basic Structure of a C Program

```c
#include <stdio.h>

int main() {
    // Your code here
    return 0;
}
```

* `#include <stdio.h>`: Preprocessor directive to include standard input-output library.
* `int main()`: Main function, starting point of execution.
* `return 0;`: Terminates program and returns 0 to OS.

---

## 3. Data Types and Variables

* **Basic Data Types:**

  * `int` — Integer (whole numbers)
  * `float` — Floating-point numbers (decimals)
  * `double` — Double precision floating-point numbers
  * `char` — Single character

* **Variable Declaration:**

```c
int a;
float b;
char c;
```

* **Initialization:**

```c
int a = 10;
float b = 3.14;
char c = 'A';
```

---

## 4. Operators in C

* **Arithmetic Operators:** `+`, `-`, `*`, `/`, `%`
* **Relational Operators:** `==`, `!=`, `>`, `<`, `>=`, `<=`
* **Logical Operators:** `&&`, `||`, `!`
* **Assignment Operators:** `=`, `+=`, `-=`, `*=`, `/=`
* **Increment/Decrement:** `++`, `--`

---

## 5. Input and Output

* `printf()` — to print output.
* `scanf()` — to take input.

Example:

```c
int num;
printf("Enter a number: ");
scanf("%d", &num);
printf("You entered %d", num);
```

---

## 6. Control Structures

### a) Conditional Statements

* `if` statement:

```c
if (condition) {
    // code
}
```

* `if-else`:

```c
if (condition) {
    // code
} else {
    // code
}
```

* `else if` ladder
* `switch-case` statement

### b) Loops

* `for` loop
* `while` loop
* `do-while` loop

Example:

```c
for (int i = 0; i < 5; i++) {
    printf("%d ", i);
}
```

---

## 7. Functions

* Functions help modularize code.
* Syntax:

```c
return_type function_name(parameter_list) {
    // function body
}
```

Example:

```c
int add(int a, int b) {
    return a + b;
}
```

* Function call: `int result = add(3, 4);`

---

## 8. Arrays

* Collection of elements of the same type.
* Declaration:

```c
int arr[5];  // array of 5 integers
```

* Initialization:

```c
int arr[5] = {1, 2, 3, 4, 5};
```

* Access elements using index: `arr[0]`, `arr[1]`, etc.

---

## 9. Strings

* A string is an array of characters terminated by a null character `\0`.
* Declaration:

```c
char str[20] = "Hello";
```

* Use `printf("%s", str)` to print strings.

---

## 10. Pointers

* A pointer stores the address of a variable.
* Declaration:

```c
int *p;
int a = 10;
p = &a;  // p points to a
```

* Dereferencing:

```c
printf("%d", *p);  // outputs 10
```

---

## 11. Structures

* Grouping different types of variables under one name.

```c
struct Student {
    int id;
    char name[50];
    float marks;
};
```

* Access members using `.` operator:

```c
struct Student s1;
s1.id = 1;
```

---

## 12. File Handling

* Working with files in C using:

  * `fopen()`, `fclose()`
  * `fprintf()`, `fscanf()`
  * `fread()`, `fwrite()`

Example:

```c
FILE *fp;
fp = fopen("file.txt", "w");
fprintf(fp, "Hello File");
fclose(fp);
```

---

## 13. Dynamic Memory Allocation

* Allocate memory during runtime using:

  * `malloc()`
  * `calloc()`
  * `realloc()`
  * `free()`

Example:

```c
int *ptr = (int *)malloc(sizeof(int) * 5);
free(ptr);
```

---

## 14. Advanced Concepts

### a) Recursion

* A function calling itself.

```c
int factorial(int n) {
    if (n == 0) return 1;
    else return n * factorial(n - 1);
}
```

### b) Command Line Arguments

```c
int main(int argc, char *argv[]) {
    // argc: number of arguments
    // argv: array of argument strings
}
```

### c) Bitwise Operators

* Operators that work at the bit level: `&`, `|`, `^`, `~`, `<<`, `>>`

---

## 15. Common Libraries and Functions

* `<stdio.h>` — Input/output functions
* `<stdlib.h>` — Memory allocation, process control
* `<string.h>` — String handling functions like `strcpy()`, `strlen()`, `strcmp()`
* `<math.h>` — Mathematical functions like `sqrt()`, `pow()`

---

## 16. Tips for Learning C

* Practice writing simple programs daily.
* Understand memory management concepts.
* Debug programs using print statements or a debugger.
* Work on projects or assignments.

---
