# C++ cheatsheet


## Shared Pointers
### Shared_ptr
- Reference counted
### week_prt
- Lets you "peek" at a shared_ptr without bumping the reference cout
### unique_ptr
- Noncopyable (use std::move)

## Const
- To say it wont change
    - When declaring a local variable
    ``` int const zero = 0; ```
    - An a function parameter
    ```
    int taxes(int const total) // can't change input value now 
    int something(Percon const& p) // can't change anything about p 
    ```
        - Note here something can only call const functions of p like the following GetName
    - Modifier on a memeber function
    ``` 
    int GetName() const; // getName can't change an variable of the class this belongs to 
    ```
- const: Before or After?
    - these are the same
    ```
    int const ci = 3; // after
    const int ci = 3; // before
    // complier doesn't care 
    ```
    - *but* humans care
        - const on the right is easier to understand specially when you bring in other concepts
        - *just put it after*



## Create a makefile
```
gcc -c main.cpp
gcc main.o -lstdc++ #link cpp standard library 
./a.out 
```
- or
``` 
g++ main.o #this will link the standard library automatically 
```
- or
``` 
g++ -Wall -g -c <file>.cpp -o <file>.o 
```
- or
``` 
g++ main.c # shortest way
```


## c++ versions
### c++ 11
- Move Semantics and rvalues
- auto
- Range-based for
- Lambdas
- Scoped enums (enum classes)
- Variadic templates
- Defaulted and deleted functions
- Tuple
- Smart pointers
### C++ 14
- Generic lambdas
- Capture expression in lambdas
- Standard user defined literals
### c++ 17
- Structured bindings
- if initializers
- Class template argument deductions
- string_view
- optional
- Parallel algorithmns