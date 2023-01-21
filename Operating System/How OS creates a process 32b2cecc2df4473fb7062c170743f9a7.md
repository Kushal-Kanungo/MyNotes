# How OS creates a process

Date: October 6, 2022 2:01 PM
Status: Done

## What is a Program ?

> **Program is a compiled code which is ready to execute in system.**
> 

## What is Process ?

> **A process is a program under execution.**
> 

## Conversion of Program to Process by OS (5 Steps)

1. Load the program and static data in memory
2. Allocate the runtime stack. *This stack will be used for local functions, local variables*
3. Heap Memory Allocation. *This Heap memory will be used for dynamic allocations (eg. mallock , new)*
4. IO Tasks
    1. Input Handle
    2. Output Handle 
    3. Error Handle
5. OS handoffs control to main()

## Architecture of  Process

![Untitled](How%20OS%20creates%20a%20process%2032b2cecc2df4473fb7062c170743f9a7/Untitled.png)

### For Stack Overflown

> **Errors Set the Base Case in Recursive calls**
> 

### For Out of Memory Errors

> **Deallocate unnecessary objects**
> 

## Attributes of Process

### Process Table

OS have a table where it stores all the process this table is known as Process Table

A single entry in this table is know as **PCB** *Process Control Block*

### Process Control Block -

 *A single entry in Process Table*

> It stores attributes of a process
> 

It have seven attributes

- Process ID
    
    It is **unique identifier** for a process
    
- Program Counter
    
    The Process is a set of instructions for CPU to execute starting from index 0
    
    Program Counter shows which instruction to execute 
    
- [Process State](Process%20States%20283268e54d9f49029219778c8e5a4ab2.md)
    
    In which is the state is like new,wait,run
    
- Priority
    
    Stores priority of a process
    
- Register
    
    Save the state of registers
    
    Stack Pointer, Base Pointer, CR States in these register is stored in here
    
- Open File System
    
    Some files are opened by process
    
- Open Device System
    
    Some devices are used by process
    

![Untitled](How%20OS%20creates%20a%20process%2032b2cecc2df4473fb7062c170743f9a7/Untitled%201.png)