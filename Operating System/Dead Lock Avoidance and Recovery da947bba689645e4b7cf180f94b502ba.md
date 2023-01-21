# Dead Lock Avoidance and Recovery

Date: October 12, 2022 12:22 AM
Status: Not started

## Deadlock Avoidance

1. We should  know what is Current State ?
    1. No of processes
    2. Need of Resource of each process
    3. Currently allocated amount of R. to each process
    4. Max. amount of each Resource
2. We have to schedule accordingly so our system remain in **Safe State or DL never occur.**
3. The system is in Safe State only if their exist a safe sequence.
4. If OS cannot prevent process of requesting resources in such a way that any deadlock occurs.
5. Scheduling Algorithm using which DL can be avoided by finding safe state. (Banker Algorithm).

## Banker Algorithm

When a process requests a set of resources, the system must determine whether allocating these resources will leave the system in a safe state. If yes, then resources may be allocated to the process. If not, the process must wait until other processes release enough resources.

## Deadlock Detection

- We use an algorithm to check if the system is in an Deadlock if it is we will use recovery.
- Otherwise after some time we re run deadlock detection algorithm

### Single instance of each resource

> Wait for Graph Algorithm ⇒ If a cycle exist in Wait for Graph then deadlock exist
> 

![Untitled](Dead%20Lock%20Avoidance%20and%20Recovery%20da947bba689645e4b7cf180f94b502ba/Untitled.png)

### Multiple Instances

- Banker Algorithm
    - If Safe Sequence available → No DL
    - If Safe Sequence not available → DL Detected

## Deadlock Recovery

1. **Process Termination**
    1. Abort All DL Processes
    2. Abort One process at a time until DL cycle is eliminated
2. **Resource Preemption**
    1. To eliminate DL, we successively preempt some resources from processes and give these resources to other processes until DL cycle is broken.