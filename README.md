# Python programming language
## Introduction to Python:
- Python was first developed by ___`Guido van Rossum`___, and released in ___`1991`___. Python was named after ___`Monty Python's Flying Circus`___ a comedy series created by the comedy group Monty Python.
- It is a general-purpose programming language that also works nicely as a scripting language.
- It is a high level ___`Interpreted`___ programming language, which means the source code of python does not need compilation like other languages. Source code of python directly gets converted to binary format at the time of writing code.
- It is ___`Dynamically typed`___ language, which means the type for a variable is decided at the run time only, we do not have to specify the type of a variable.
- ___`Interpreter`___ is a layer of software logic between your code and the computer hardware on your machine.

### Advantages/Features of Python programming language:
- It is easy to code, high level programming language, uses clear and readable syntax
- It is free & open source programming language, with huge global community
- It is portable programming language (works on different platforms and operating systems)
- It has extensive support libraries which provide modules suited for different tasks like automation, web scrapping, text processing, image processing, machine learning, data analytics etc.
- It supports GUI (Graphical user interface) applications and has framework for web

### Disadvanategs of Python programming language: 
- It has poor memory efficiency (Python needs a lot of memory space, this can be a disadvantage when we want to develop a memory optimised applications)
- It has a slow Speed (as Python code executes line by line and due to poor memory efficiency, the execution speed becomes slow)
- It is weak in mobile computing (due to its high memory usage and slow speed, it is generally not used for frontend programming or mobile app development. It is used for backdend programming)
- As it is a dynamically typed language, the data types of variables in Python can change suddenly. A variable holding a string may contain an integer later, and this can lead to runtime errors.

### Memory allocation in Python:
- In C or other languages, memory management is the responsibility of the programmer. The programmer has to manually allocate memory before it can be used by the program and release it when the program no longer needs it.
- In Python, memory management, or the allocation and deallocation of memory, is an automatic process.
- In the C language, the ___`malloc`___ method is used to request a block of memory from the operating system at run-time, whereas the ___`free`___ method is used to release memory allocated to the program back to the operating system when the program no longer needs it.
- The implementation of the Python language in C is called ___`CPython`___. CPython is the default and most widely used implementation of the Python language.
- When a Python program needs memory, CPython internally calls the 'malloc' method to allocate it and the 'free' method to release it when the program no longer needs the memory.
- Everything in Python, such as classes, functions, and even simple data types like integers, floats, and strings, are objects.
- When we define an integer in Python, CPython internally creates an object of type integer. These objects are stored in Heap memory.
- Variables in Python are just references to the actual object in memory. They are like names or labels that point to the actual object in memory; they do not store any value.
- In Python, memory allocation is typically divided into two types:
  > ___`Stack memory`___ Stack memory is used for managing function calls and their local variables. It's like a temporary scratchpad that is automatically cleared when a function finishes its job. You can think of it as a small, fast-access storage area for short-lived data.
  
  > ___`Heap memory`___ Heap memory is where Python stores more long-lasting and dynamically allocated data, like objects such as lists, dictionaries, and custom classes. It's a larger and more flexible storage space where data can persist beyond the scope of a single function.

### Garbage collection in Python:
- It is defined as the process of reclaiming or releasing allocated memory when it is no longer needed by the program.
- The ___`Python garbage collector`___ handles memory allocation and deallocation automatically.
- The garbage collector (GC) operates in the background and is triggered when the reference count reaches zero.
- The reference count rises when the following occurs:
  - An object is given a new name.
  - An object is placed in a container, such as a tuple or a dictionary.
- The reference count lowers when the following occurs:
  - An object’s reference is reassigned.
  - An object’s reference moves out of scope.
  - An object is removed.

### PyObject concept in Python:
- It is actually a C structure representing a generic Python object used in the CPython implementation.
- In Python, var = 10 and temp = 10 will typically have the same id because integers between -5 and 256 are cached, whereas var = 10 and var = 20 will have different ids as they refer to different objects.
- In Java, var = 10 and temp = 10 will indeed have different ids because they are primitive values, whereas var = 10 and var = 20 will have the same id if they are autoboxed to Integer objects with the same value.

### Threading & Multiprocessing:
- Both multiprocessing and threading in Python are ways to do multiple things at the same time, but they do it in different ways.
  > ___`Threading`___ is a process of running multiple threads (smaller units of a program) concurrently, sharing the same memory space. Means they can easily communicate and share data with each other and are good for tasks that involve a lot of waiting or I/O operations.
  
  > ___`Multiprocessing`___ In multiprocessing, each task is done by a completely separate process. These processes don't share memory space, which means they can run completely independent and in their own memory space. Multiprocessing is great for tasks that can be split into independent parts and processed in parallel. Think of it like having multiple workers working on different tasks simultaneously: Imagine you have a big task that needs to be done, and you have a team of people. Instead of making one person do the whole task, you divide it into smaller parts and have each person work on their part at the same time.
- If you have tasks that can be divided into independent parts and can benefit from parallel processing, use multiprocessing.
- If you have tasks that involve I/O operations and can run concurrently, use threading. Correct these statments grammatically.

### Shortkeys in Python's Jupyter notebook:
| Shortkeys   | Use                         |
|-------------|-----------------------------|
| ctrl+a      | select all                  |
| ctrl+c      | copy                        |
| ctrl+x      | cut                         |
| ctrl+v      | paste                       |
| esc+z       | undo                        |
| esc+a       | redo                        |
| ctrl+enter  | run cell                    |
| shift+enter | run cell and enter below    |
| esc+a       | insert cell above           |
| esc+b       | insert cell below           |
| esc+y       | change the cell to code     |
| esc+m       | change the cell to markdown |
| tab         | auto-complete code          |
| shift+tab   | preview documentation       |

### Indentation in Python:
- Indentation is like the blank space at the start of a line in your code. It's used to organize your code visually and tell the computer which parts of the code belong together, like grouping lines in a function or loop.

### Indexing in Python:
- Indexing in Python refers to the process of accessing individual elements within a data structure, such as a string, list, tuple, or other sequence types, using their position or index.

### Comments in Python:
- Comments are lines in the code that are ignored by the compiler or interpreter during program execution.
- They are used to provide explanations or context within the code for better understanding.
- Professionally, comments are used to add the name of the project, the name of the developer, the starting date of the project, the purpose of the block of code, and any additional requirements.
- There are two main types of comments:
  > ___`Single-line comments`___
  
  > ___`Multi-line comments`___

### Printing methods of string in Python:
- In Python, "printing methods" typically refer to the various functions and techniques used to display output to the console or other output streams.
- There are basically two ways of printing strings in Python:
  > ___`f'string method`___ writes the string directly to the standard output stream.
  
  > ___`Format string method`___ allows for more complex string formatting with placeholders.
- In Python, by default, the ___`print()`___ function ends with a newline character, causing the cursor to move to the next line after printing.
- To override this behavior and keep the cursor at the end of the printed output, you can use the ___`end=' '`___ parameter in the print() function.
  
### Raw string and Escape characters in Python:
- In Python, a raw string is a string literal prefixed with an ___`r`___. This notation tells Python to interpret the string exactly as it is, without any special processing for escape sequences.
- Escape characters in Python are special characters preceded by a backslash in a string literal.
- They are used to represent characters that are difficult or impossible to type directly into a string.
- Below are some common escape characters in Python:

| Escape character | Use                                                                                  |
|------------------|--------------------------------------------------------------------------------------|
| \n               | Represents a newline character, causing the text following it to start on a new line |
| \t               | Represents a tab character, causing the text following it to be indented             |
| \\               | Represents a single backslash character                                              |
| \'               | Represents a single quote character                                                  |
| \"               | Represents a double quote character                                                  |

### Variables in Python:
- Variables in Python are entities that store data. When naming variables, it's important to follow these guidelines:
  - Choose meaningful names that reflect the data they store.
  - Avoid using predefined keywords as variable names.
  - Do not start variable names with numbers.
  - Variable names should begin with a lowercase character.
  - Avoid special characters and spaces in variable names.
  - It's acceptable to use a combination of uppercase characters, lowercase characters, underscores, and numbers within the variable name.
- Types of variables in Python:
  > ___`Global variables`___ are defined outside of any function and can be accessed throughout the main program and any user-defined functions as well.

  > ___`Local variables`___ These variables are defined inside a function and can only be accessed within that specific function. Although it's possible to make a local variable act as a global variable using the 'global' keyword, it is generally not recommended due to potential confusion and scope-related issues.

### Predefined keywords in Python:
- Predefined keywords in Python refer to words that are reserved for specific purposes within the Python language.
- These keywords have predefined meanings and are used to define the syntax and structure of Python code.
- These keywords cannot be used as identifiers such as variable names, function names, or class names within Python code.

### Data types in Python:
- There are mainly 6 datatypes in python
  - ___`String (str)`___ ex. 'Python'
  - ___`Integer (int)`___ ex. 10,2,3,4
  - ___`FLoat (float)`___ ex. 10.2, 23.5
  - ___`Complex number (complex)`___ ex. 2+3j, 10+4j [real +imaginary] can be poitive or negative
  - ___`Boolean (bool)`___ ex. True, False
  - ___`Sequential (list[], tuple(), set{}, dictionary{key:value})`___
- The letter 'j' instead of 'i' is conventionally used in the complex datatype to represent the imaginary part of a complex number. This convention is adopted for several reasons:
  - In electrical engineering, the letter 'i' commonly denotes current.
  - In computing, 'i' frequently serves as the indexing variable in loops.
  - There's potential for confusion between 'i' and visually similar characters like 'l' (lowercase L) or '1' (the number one) in source code.
- Using 'j' helps avoid ambiguity and aligns with established practices in mathematics and programming, facilitating clearer and less error-prone code.

### Duck typing in Python:
- Duck typing in Python is a programming concept where the type or class of an object is determined by its behavior rather than its explicit type declaration.

### Typecasting in Python:
- Typecasting in Python refers to the process of converting one data type into another.
- When typecasting, it's important to remember the following:
  - When converting strings to integer or float data types, conversion occurs only if the string represents a valid integer or float value.
  - If the string contains alphabetic characters or other non-numeric characters, it cannot be converted to an integer or float.
  - Decimal integers represented as strings will be converted to float type directly. To convert them to integer type, they first need to be converted to float type and then to integer type.
  - It's not possible to directly convert complex numbers to integer or float data types. Complex numbers are a separate data type in Python and require their own operations for manipulation and conversion.

### Operators in Python:
- Operators in Python are special symbols or keywords used to perform various operations such as arithmetic, comparison, logical, assignment, and more.
- These operators manipulate the operands, which are the values or variables that the operator acts upon. (2+3=5; here 2 and 3 are oprands and + is an operator)
- There are mainly seven types of operators:
  - ___Arithmatic operators___
    - Addition (+)
    - `Substraction (-)
    - Multiplication (*)
    - Division (/)
    - Exponentiation (**)
    - Floor division (//)
    - Modulus (%)
  - ___`Assignment operators`___
    - Assign (=)
    - Add and assign (+=)
    - Substract and assign (-=)
    - Multiply and assign (*=)
    - Divide and assign (/=)
    - Modulus and assign (%=)
    - Exponentiation and assign (**=)
    - Floor divide and assign (//=)
  - ___`Comparison operators`___
    - Greater than (>)
    - Less than (<)
    - Equal to (==)
    - Not equal to (!=)
    - Greater than or equal to (>=)
    - Less than or equal to (<=)
  - ___`Logical operators`___
    - and (both conditions must be True/False)
    - or (any of the conditions must be True/False)
    - not (used as if not)
  - ___`Membership operators`___
    - in (returns true if value is present)
    - not in (returns true if value is not present)
  - ___`Identity operators`___
    - is (returns True if the first value is the same as the second)
    - is not (returns True if the first value is not the same as the second)
  - ___`Bitwise operators`___
    - AND
    - OR
    - XOR
    - right shift (>>)
    - left shift (<<)

> ___`AND bitwise operator:`___

| X | Y | XY |
|---|---|----|
| 0 | 0 | 0  |
| 0 | 1 | 0  |
| 1 | 0 | 0  |
| 1 | 1 | 1  |

> ___`OR bitwise operator:`___

| X | Y | XY |
|---|---|----|
| 0 | 0 | 1  |
| 0 | 1 | 1  |
| 1 | 0 | 1  |
| 1 | 1 | 0  |


> ___`XOR bitwise operator:`___

| X | Y | XY |
|---|---|----|
| 0 | 0 | 0  |
| 0 | 1 | 1  |
| 1 | 0 | 1  |
| 1 | 1 | 0  |

### Associativity of operators rule:
- The associativity of operators refers to the order in which operators of the same precedence level are evaluated in an expression.
- PEMDAS [Parentheses, Exponents, Multiplication, Division, Addition, Substraction]

### Conditional statement in Python:
- Conditional statements in Python are used to execute different blocks of code based on specified conditions.
  > ___`if statement`___ executes a block of code if a specified condition is true.
  
  > ___`if.. else statement`___ executes one block of code if the condition is true and another block if the condition is false.

  > ___`if.. elif.. else statement`___ allows for multiple conditions to be checked in sequence, executing the first block of code that evaluates to true. If none of the conditions are true, the else block is executed.


