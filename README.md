# Python programming language
## Introduction to Python:
- Python was first developed by ___`Guido van Rossum`___, and released in ___`1991`___. Python was named after ___`Monty Python's Flying Circus`___ a comedy series created by the comedy group Monty Python.
- It is a general-purpose programming language that also works nicely as a scripting language.
- It is a high level ___`Interpreted`___ programming language, which means the source code of python does not need compilation like other languages. Source code of python directly gets converted to binary format at the time of writing code.
- It is ___`Dynamically typed`___ language, which means the type for a variable is decided at the run time only, we do not have to specify the type of a variable.
- ___`Interpreter`___ is a layer of software logic between your code and the computer hardware on your machine.

> Advantages/Features of Python programming language:
- It is easy to code, high level programming language, uses clear and readable syntax
- It is free & open source programming language, with huge global community
- It is portable programming language (works on different platforms and operating systems)
- It has extensive support libraries which provide modules suited for different tasks like automation, web scrapping, text processing, image processing, machine learning, data analytics etc.
- It supports GUI (Graphical user interface) applications and has framework for web

> Disadvanategs of Python programming language: 
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
- In Python, memory allocation is typically divided into Stack memory and Heap memory
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

### PyObject concept:
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

### Comments in Python:
- Comments are lines in the code that are ignored by the compiler or interpreter during program execution.
- They are used to provide explanations or context within the code for better understanding.
- Professionally, comments are used to add the name of the project, the name of the developer, the starting date of the project, the purpose of the block of code, and any additional requirements.
- There are two main types of comments:
  > ___`Single-line comments`___
  
  > ___`Multi-line comments`___

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
