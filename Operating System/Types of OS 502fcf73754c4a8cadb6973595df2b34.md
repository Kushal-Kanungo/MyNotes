# Types of OS

Date: October 3, 2022 8:30 PM
Status: Done

# Types Of OS

## Single Process OS

> Example : MS Dos
> 
1. 1 process at a time
2. 2nd process waits until the first is finished
3. No Context Switching
4. Process Starvation
5. Priority cannot be set
6. CPU idle in I/O Operations

## Batch Process OS

> Example ATLAS
> 
1. Users prepares jobs using punch cards
2. Then submits to computer operators
3. **Operator** sort the jobs in batches
4. Operator submit the batches to processor one by one
5. CPU do jobs sequentially of a batch 
6. Priority cannot be set
7. May lead to starvation 
8. CPU idle in I/O operations

## Multi Programming OS

> The Dijkstra
> 
1. Single CPU
2. **Context Switching  for processes** 
    
    > Storing the state of a process and start other one and then restore the execution of that process
    > 
3. Switching happens only one goes to wait state
4. CPU idle time reduced

## Multi Tasking OS

> CTSS, MIT
> 
1. Single CPU
2. Able to run more than one task simultaneously
3. Context sharing and **time sharing** is used
    
    > Like process shares time in context sharing is done so no a single process take all time every job gets time to finish
    > 
4. CPU idle time is further reduced

## Multi Processing OS

> Windows NT
> 
1. More than 1 CPU so if 1 CPU fails other works
2. Less starvation because if 1 CPU is busy other can do other job.
3. Context Switching and all other available in Multi Tasking OS

## Distributed OS

> LOCUS
> 
1. Loosely coupled
2. Single OS and multiple hardware of CPU in a network
3. OS will give jobs to these different hardware
4. These systems can also of different configuration

## Real Time OS (RTOS)

> Example: ATCS
> 

> When we required error free computation in real time
> 
1. Air Traffic Control System
2. **Response Time** should be very low.