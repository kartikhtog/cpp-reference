# C++ cheatsheet

## Shared Pointers
### Shared_ptr
- Reference counted
### week_prt
- Lets you "peek" at a shared_ptr without bumping the reference cout
### unique_ptr
- Noncopyable (use std::move)



## Create a makefile
``` gcc -c main.cpp ```
``` gcc main.o -lstdc++ #link cpp standard library ```
``` ./a.out ```
- or
``` g++ main.o #this will link the standard library automatically ```
- or
``` g++ -Wall -g -c <file>.cpp -o <file>.o ```
- or
``` g++ main.c # shortest way ```
