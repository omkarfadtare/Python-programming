# Python programming language
## Introduction:
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

## Memory allocation in Python:
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

## Garbage collection in Python:
- It is defined as the process of reclaiming or releasing allocated memory when it is no longer needed by the program.
- The ___`Python garbage collector`___ handles memory allocation and deallocation automatically.
- The garbage collector (GC) operates in the background and is triggered when the reference count reaches zero.
- The reference count rises when the following occurs:
  > An object is given a new name.
  > An object is placed in a container, such as a tuple or a dictionary.
- The reference count lowers when the following occurs:
  > An object’s reference is reassigned.
  > An object’s reference moves out of scope.
  > An object is removed.






