# Day 1 - C++, DSA foundations and setting up for the project!

## C++:
C++ is a high level, object oriented programming language used for various purposes. Flow: 
Instructions in a text file -> Compiler turns thm to program -> Computer runs the programs.

```
Code in a .cpp file (hello.cpp)
        ↓
Compiler checks and translates it to machine readable form
        ↓
An executable program is created (hello)
        ↓
We run the program(./hello)
```

## Compiling and running a CPP program: 
To compile a .cpp program we must: 

```bash
g++ -std=c++20 -Wall -Wextra hello.cpp -o hello
```
What each element represents here: 

|       Part            |                   Meaning                 |
|-----------------------|-------------------------------------------|  
| ```g++```             | Represents the GNU C++ Compiler.          |
| ```-std=c++20```      | Instruct to use the modern C++ 20 rules.  |
| ```-Wall -Wextra```   | TO display all the warnings.              |
| ```hello.cpp```       | Name of the cpp file to be compiled.      |
| ```-o hello```        | Name the executable as hello.             |   

To run the executable file: 
```bash
./hello
```

