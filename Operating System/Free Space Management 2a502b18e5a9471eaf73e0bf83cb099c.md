# Free Space Management

Date: October 16, 2022 7:05 PM
Important: Defragmntation | Compsction | First Fit | Next Fit | Best Fit | First Fit
Status: Not started

# De fragmentation / Compaction

- All the free partitions are made contiguous, and all the loaded partitions are brought together.
- The efficiency of the system is decreased in the case of compaction since all the free spaces will be transferred from several places to a single place.

### How Free Space is stored / represented in OS ?

- Free holes in the memory are represented by a free list (Linked-List data structure).

### How to satisfy a request of a of n size from a list of free holes ?

- **First Fit**
    1. First Hole that is big enough
    2. Simple easy to implement
    3. Fast / Less time complexity
- **Next Fit**
    1. Enhancement of first fit search start from last allocated hole
    2. Same advantage of first fit.
- **Best Fit**
    1.  Lesser **Internal fragmentation**.
    2. May create many small holes and cause major external fragmentation.
    3. Slow, as required to iterate whole free holes list.
- **Worst Fit**
    1. Allocate the largest hole that is big enough.
    2. Slow, as required to iterate whole free holes list.
    3. Leaves larger holes that may accommodate other processes.

### Internal Fragmentation

When a more space is allocated than need it creates an empty hole

![Untitled](Free%20Space%20Management%202a502b18e5a9471eaf73e0bf83cb099c/Untitled.png)

### External Fragmentation

![Untitled](Free%20Space%20Management%202a502b18e5a9471eaf73e0bf83cb099c/Untitled%201.png)