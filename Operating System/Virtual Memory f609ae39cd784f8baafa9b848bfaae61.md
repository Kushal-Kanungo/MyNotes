# Virtual Memory

Date: October 29, 2022 1:58 PM
Important: Demand Paging | Pure Demand Paging | Paging Fault | Pager Guesses | 
Status: Done

## Virtual Memory

It is a technique that allows the execution of processes that are not completely in memory. It provides illusion of having a very big main memory. This is done by treating a part of secondary memory as main memory. (Swap Space.)

### Advantages

- Program can be larger than physical memory
- Because each user program could take less physical memory, more program could be run at the same time.
- Increase CPU utilization and throughput.
- Running a program that is not entirely in memory would benefit both the system and the user.

### **Demand Paging** is popular method of virtual memory management.

> In demand paging the pages that are less used stored in secondary memory when its demand is made a **page fault** occurs. Then there are various **page replacement algorithms** which are used to determine the page which will be replaced.
> 

- Rather than swapping the entire process into memory, we use Lazy Swapper. A lazy swapper never swaps a page in memory unless that page will be needed.
- We are viewing a process as sequence of pages rather than a large contiguous address space. Instead of **Swapper** we use **Pager**.

### How Demand Paging Works ?

- When a process is to be swapped the **pager guesses** which page will be used.
- Instead of swapping in  a whole process, the pager brings only those pages into memory.
- OS decreases the swap time and the amount of physical memory required.
- A **valid-invalid bit** scheme in the page table that show which pages are in memory and are on the disk
    - Valid-invalid bit **1 means page is valid** and in memory.
    - Valid-invalid bit **0 means page is not valid** or present at disk.
- If a page is not present in main memory than a Page Fault occurs.
    
    
    **Procedure to handle page fault**
    
    - **Check an internal table (PCB)** to determine whether the reference was valid or an invalid memory address access.
    - If **ref. is invalid process throws exception** else pager will swap-in page.
    - We find a free frame from **frame-free list**.
    - Schedule a disk operation to read the desired page into the **newly allocated frame**.
    - When disk read is complete. we modify the page table that the page is now in memory.
    - Restart the instruction that was interrupted by the trap. The process can now access the page as through it had always in memory.

### Pure Demanding Paging

- In extreme cases we can start executing **process with no pages** in memory. When OS sets the instruction pointer to the first instruction of the process, which is not in the memory. The process immediately faults for the page and page is brought in  the memory
- Never bring a **page in memory until required**.

## Disadvantage of virtual memory

- The system can become **slower** as swapping takes time.
- **Thrashing** may occur.