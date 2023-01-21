# What and Why is OS

Date: October 3, 2022 2:27 PM
Status: Done

# Operating System

> An operating system is a program that controls the execution of application programs and acts as an interface between the user of a computer and the computer hardware
> 

> An operating system is a piece of software that manages all the resources of a computer
system, both hardware and software, and provides an environment in which the user can
execute his/her programs in a convenient and efficient manner by hiding underlying
complexity of the hardware and acting as a resource manager.
> 

## Why OS ?

1. If there is no OS?
    1. Bulky and Complex app. (because resource and hardware management will be in every app’s code base)
    2. Resource exploitation by 1 app
    3. No memory protection because any app can overwrite the memory used by another app
2. What is OS made up of ?
    1. Collection of System Software

# Functions of OS

1. Access to computer hardware
2. Interface b/w user and computer hardware
3. Resource Management
4. Hides the underlying complexity of hardware
5. Isolation and protection of different programs running from each other

# In Depth Learning

## Functionalities

- **Resource Management**
    
     During parallel accessing happens, the OS works as resource manager.
    
- **Process Management**
    
     It includes tasks like scheduling, termination of process. *CPU Scheduling is done by algorithms*. **Some Techniques**
    
    - **Shortest Job First** : The process which needs shortest CPU time scheduled first
    - **Round Robin Scheduling** : Each process is assigned a fixed CPU execution time in a cyclic way.
    - **Priority Based Scheduling** : The highest priority task is scheduled first.
- **Storage Management**
    
     The File System mechanism used in management of storage. All the data is stored in tracks of Hard Disk which is all managed by storage manager.
    
- **Memory Management**
    
     Refers to management of primary memory The OS has to keep track of how much memory is used and by whom. The OS also allocate and deallocate the memory space.
    
- **Security Management**
    
     Privacy is also provided by OS by means of passwords so that unauthorized applications can’t access data.
    
- **I/0 Management**
    
     This module keep track of I/O devices.
    
- **Context Switching**
    
     In most multitasking OSs, multiple running process on the system may need to change the state of execution. OS saves the execution state of previous process before switching to the current one.
    
- **Buffering**
    
    In this technique, input and output data are temporarily stored in input and output buffer.
    
- **Spool**  *Simultaneous Peripheral Operation On Line*
    
     This is a device management technique used for processing different tasks on the same input/output device. When there are various users on a network sharing the same resource then it can be a possibility that more than one user might give it a command at the same point in time. So, the operating system temporarily stores the data of every user on the hard disk of the computer to which the resource is attached. The individual user need to wait for the execution process to be completed. Instead, the operating system sends the data from the hard disk to the resource one by one.