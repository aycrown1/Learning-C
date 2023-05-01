#Learn C language 

## Why Learn C ?
C is a high-level, general-purpose programming language that was originally developed by Dennis Ritchie at Bell Labs in the 1970s. It is a procedural programming language, which means that it follows a step-by-step approach to solve problems.

C has been widely used for developing operating systems, device drivers, software applications, and embedded systems. It is also popular among computer science students because of its simplicity, powerful features, and fast execution speed.

C programming is awesome for several reasons, including:
* It has a simple syntax that is easy to learn and use
* It is a powerful language that allows for low-level programming and efficient use of system resources
* It has a vast library of functions that can be used to perform a wide range of tasks
* It is portable, meaning that programs written in C can run on many different platforms and operating systems
* It has influenced many other programming languages, making it a valuable language to learn for software development.

## Entry point.
an entry point is the location within a program where execution begins. In C programs, the entry point is typically the "main" function.

"Main" is a function in the C programming language that serves as the entry point for the program. It is where program execution begins and typically contains the code that performs the program's main task. The "main" function must be present in all C programs.

## Compilation.

To compile a C program using gcc, you can use the following command:

```shell

gcc <source_file.c> -o <output_file>

```

When you type "gcc main.c" into a command prompt, the GCC (GNU Compiler Collection) toolchain is invoked to compile the "main.c" file into an executable program. The resulting program can then be run on the system.

By default, when compiling a C program with gcc, the output program name will be "a.out". However, you can specify a different output file name using the "-o" flag, as shown in the example above.

### Compilation flags.

```shell

gcc Wall, -Werror, -Wextra, -pedantic, and -std=gnu89 *c -o

```
* `-Wall`: Enables all warning messages that gcc can generate. This can help catch potential errors and improve code quality.
* `-Werror`: Treats all warnings as errors, causing the compilation to fail if any warnings are generated. This can help enforce a high level of code quality.
* `-Wextra`: Enables additional warning messages beyond those enabled by -Wall. This can catch additional potential issues in the code.
* `-pedantic`: Enables warnings for code that may not strictly conform to the C language standard. This can help ensure portability and compatibility across different platforms and compilers.
* `-std=gnu89`: Specifies the C language standard to use for compilation. In this case, it is using the GNU C89 standard, which is a version of the C language specification that includes some additional features beyond the original C89 standard.
* `-o`: Specifies the output file name for the compiled binary. In this case, it is using -o followed by no file name, which means the output file name will be the default name (a.out).

Using compilation flags such as -Wall, -Werror, -Wextra, -pedantic, and -std can help improve the quality, readability, and maintainability of C code. Here are some of the reasons why:

-Wall, -Werror, and -Wextra enable warning messages that can catch potential issues in the code, such as uninitialized variables, unused variables, or implicit type conversions. By catching these issues early, before the code is even executed, developers can avoid introducing bugs and improve the overall quality of the code.

-pedantic warns about non-portable constructs and non-standard extensions to the C language. By ensuring that code adheres to the C standard, developers can avoid writing code that may not work properly on different platforms or with different compilers.

-std specifies the C language standard to use for compilation. By using a specific standard, developers can ensure that their code adheres to a well-defined set of rules and conventions, which can improve portability and compatibility with other code.


## Coding Style.

C language specification does not mandate any particular coding style or formatting. However, there are several popular coding styles that are commonly used by C programmers to improve code readability and maintainability.

One widely-used C coding style is the "K&R style," named after Brian Kernighan and Dennis Ritchie, who wrote the seminal book "The C Programming Language" and used this style throughout the book. The K&R style emphasizes brevity and uses a minimalistic approach to formatting, with a focus on clarity and simplicity.

Another popular C coding style is the "GNU style," used by many open source projects and supported by the GNU coding standards. The GNU style places a greater emphasis on consistency and readability, using a more structured and verbose approach to formatting.

### Betty style checker.

The most wide used by C student and learners is "Betty style checker,".

Betty is a style checker tool for C programming that enforces a specific coding style guide. Betty was originally created for use in Holberton School, a coding bootcamp in the United States, to help students improve their coding style and consistency.

The Betty coding style guide emphasizes readability, simplicity, and consistency in C code. It includes guidelines for code formatting, naming conventions, function declarations, and other aspects of C programming. Some of the key guidelines in the Betty style guide include:

* Use snake_case naming convention for variables and functions.
* Indent code using tabs, not spaces, with a tab width of 4 characters.
* Limit lines to a maximum of 80 characters in length.
* Use a space after commas and around operators.
* Place opening curly braces on the same line as the function or control statement, and closing braces on a new line.

To use [Betty](https://github.com/holbertonschool/Betty), you can download and install the tool from its Github repository, and then run it on your C code files to check for compliance with the style guide. Betty will provide feedback and suggestions for how to improve the code's style and formatting. Using a tool like Betty can help improve the readability and maintainability of C code, making it easier to understand and work with for both the original developer and other programmers who may need to modify or maintain the code in the future.

## C syntax.

C syntax refers to the set of rules and conventions that dictate how C code is structured and written. These rules define how to write statements, expressions, declarations, functions, control structures, and other language constructs in C.
In C, the basic syntax includes elements such as:

* Keywords: These are reserved words in the C language that have a specific meaning and cannot be used as identifiers. Examples include int, char, if, and while.

* Identifiers: These are names used to identify variables, functions, and other program elements. Identifiers must adhere to certain rules, such as starting with a letter or underscore and consisting of letters, digits, and underscores.

* Operators: These are symbols used to perform operations on values or variables. Examples include + for addition, - for subtraction, * for multiplication, / for division, and = for assignment.

* Statements: These are individual lines of code that perform a specific action or set of actions. Examples of C statements include variable declarations, function calls, conditional statements (if and else), and loops (for and while).

C code is made up of functions, which are blocks of code that perfo>
C code uses variables to store data. Variables are declared with a >
C code uses control structures, such as if-else statements, loops, >

* Braces and semicolons: In C, braces ({}) are used to enclose blocks of code, while semicolons (;) are used to terminate individual statements.

* Comments: These are used to add notes to the code that are ignored by the compiler. Comments in C can be single-line (//) or multi-line (/* ... */).

* C code is written in plain text files, with the file extension .c.

* C code can use preprocessor directives, which are commands that are processed by the preprocessor before the code is compiled. Preprocessor directives are indicated with a # symbol and include commands to include header files, define constants, and perform other tasks.

## Data Type.

In C, data types are used to specify the type of data that a variable can hold before it been called or used. The syntax for declaring a variable with a specific data type in C is:

```c
data_type variable_name;
```

C provides several built-in data types that can be used to declare variables, including:

* `int type`: used for integer values. including `int`, `short`, `long`, and `long long`. Each integer type has a different range of values it can represent.
* `char type`: used for character values. C provides two character types: char and signed char.
* `float type`: used for floating-point values
* `double type`: used for double-precision floating-point values
* `void type`: used for indicating that a function does not return a value
* `Boolean type`: This is a built-in data type in C99 and later versions. The _Bool type can have the values 0 or 1 to represent false or true, respectively.

In addition to these built-in data types, C also allows for the creation of user-defined data types using the struct keyword. A struct is a collection of related variables that can be treated as a single entity.

For example, to declare a struct that represents a person with a name and age, you could use the following syntax:

```c
struct person {
    char name[50];
    int age;
};

```
This declares a new data type called `person`, which has two fields: `name`, which is an array of characters with a maximum length of 50, and `age`, which is an integer.

Using the proper syntax for data types in C is important for ensuring that variables are properly initialized and used, and can help prevent errors and bugs in code.

## Declearation, Defination and Function call

A variable declaration tells the compiler the name and type of a variable, without providing its value or memory location. Similarly, a function declaration tells the compiler the name, return type, and parameter types of a function, without providing its implementation.

```c
int my_declearation;

```
```c
int add(int a, int b);
```

A definition is a statement that both declares and implements an identifier. A definition provides the full details of an identifier, including its implementation and any necessary storage allocation.

For example, a variable definition declares a variable and provides its initial value and storage location. Similarly, a function definition provides the full implementation of a function, including its body and any necessary local variables.

```c
int my_variable = 42;
```
```c
int mul(int a, int b) {
  int product = a * b;
  return (product);
}
```
It is important to note that in C, a declaration can be separated from its definition, but a definition must be a declaration.

A  function call is a statement that invokes a function and passes it the required arguments. Here is an example of a function call to the `mul` funtion.

```c
int result = mul(2, 3);
```
The function call executes the code within the function definition and returns a value to the caller.
## Return value.

`return` is a keyword in many programming languages, including C, that is used to exit a function and return a value to the caller. In C, the `return` statement can be used in a function to return a value of a specified type.

The syntax of the return statement in C is as follows:

```c
return (expression);

```
Here, `expression` is the value that the function will return. The type of the expression must match the return type of the function. For example, if the function has a return type of `int`, the expression must evaluate to an `int`.

If the return statement is called without an expression, it is used to exit the function and return control to the caller. In this case, the function return type must be `void`.

Here is an example of a function that uses the `return` statement to return a value:

```c
int add(int a, int b) {
  int sum = a + b;
  return sum;
}
```

### Value for Return.

The value for a return statement in C is an expression that is evaluated and returned to the caller of the function. The specific value that is returned depends on the function's implementation and the type of value that is expected by the caller.

Conventionally, a return value of `0` is often used to indicate that a function executed successfully, and a nonzero value (such as `1`) is used to indicate that an error occurred. However, the specific meaning of a non-negative return value  can be implementation-dependent and can vary from function to function.=

A return value of `-1` is often used to indicate an error in functions that return an integer, such as the `open()` system call in Unix-like operating systems. However, the specific meaning of a `-1` return value can also depend on the function's implementation and the context in which it is used.

