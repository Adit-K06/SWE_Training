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

## Variables and basic data types
A variable stores a value with a name. 
There are 5 basic data types in cpp, they are: 

```cpp
// 1) int : Stores whole numbers (eg: -45, 72, 0)
int age = 15;

// 2) float : Stores decimal numbers (eg: 0.25, 3.15, 15.26589)
float interest = 8.25;

// 3) char : Stores only one character (eg: a, F, *)
char grade = 'B';

// 4) bool : Stores True or False (eg: True, False)
bool isFake = true;

// 5) String : Stores text (eg: "Adit")
// To use string we need to add the header file: #include >string>
std::string name = "Adit";
```

## Input and Output operations (I/O Ops)
To output something we can just use: 

```cpp
std::cout << "Hello!";
```

Now to take input, we simply use: 

```cpp
std::string name;
std::cin >> name;
std::cout << "Hello!" + name;
```
If we input ```Adit```, we get the ouput as ```Hello! Adit```.

## Conditions and loops
Conditions: Used when we have to chooses between 2 or more actions: 

```cpp
if(num % 2 == 0){
    std::cout << "Even" << endl;
}else {
    std::cout << "Odd" << endl;
}
```
You must have observed, I have written the ```endl`` here. It basically instructs the compiler to go to the next line and whatever is asked to print after this is printed in the next line.

Loops : Used when we want to loop something again and again.
There are 3 basic loops in c++: 

```cpp
// 1) for loop: Used when the number of times to be looped is known: 
for(int i=0; i<10, i++){
    std::cout << i;
}

// Output :  1 2 3 4 5 6 7 8 9

// 2) while loop: Used when the condition for looping is known: 
while(isTrue == false){
    // some logic
}

// 3) do-while loop: Same as the while loop but the logic will be performed atleast once. 
do {
    // some logic
} while(isTrue == false)
```

