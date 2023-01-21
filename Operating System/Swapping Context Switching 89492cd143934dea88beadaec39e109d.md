# Swapping / Context Switching

Date: October 7, 2022 8:02 AM
Important: Swapping | Context Switching | Orphan | Zombie
Status: Done

# Swapping

1. Time-sharing System may have medium term scheduler (MTS).
2. Remove processes from memory to reduce degree of multi-programming
3. These removed processes can be reintroduced into memory, and its execution can be continued where it left off. This is called **Swapping**.
4. Swap-out and swap-in is done by MTS.
5. Swapping is necessary to improve process mix or because a change in memory requirements has over committed available memory, requiring memory to freed up.
6. Swapping is a mechanism which a process can be swapped temporarily out of main memory. To secondary storage and make that memory available to processes. At some later time, the system swaps back the process from the secondary storage to main memory. 

# Context-Switching

1. Switching the CPU to another process requires performing a state save of the current process and state restore of a different process.
2. When this occurs, kernel saves the context of the old process in its PCB and loads the saved context of the new process scheduled to run.
3. It is pure overhead, because the system does no useful work while switching
4. Speed varies from machine to machine, depending on the memory, depending on the memory speed, the number of registers that must be copied etc.

# Orphan Process

1. The process whose parent process has been terminated and it still running.
2. Orphan processes are adopted by init process.
3. Init is the first process of OS.

# Zombie Process / Defunct Process

1. A zombie process is a process whose execution is completed but it still has an entry in the process table.
2. Zombie process occurs for child processes, as the parent process still needs to read its child’s exit status. Once this is done using the wait system call, the zombie process is eliminated from the process table. This is knowing as reaping the Zombie Process
3. It is because parent process may call wait() on child process for a longer time duration and child process got terminated much earlier.
4. As entry in the process can only be removed after the parent process reads the exit status of child process. Hence, child process remains a zombie till it is removed from the process table.