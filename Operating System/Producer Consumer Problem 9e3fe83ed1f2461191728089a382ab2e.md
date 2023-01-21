# Producer Consumer Problem

Date: October 9, 2022 4:26 PM
Important: Solution  ⇒  Three Semaphores | Mutex | Empty | Filled
Status: Done

## Producer Consumer Problem

1. **Producer Thread** : Will produce data which will be used by consumer thread.
2. **Consumer Thread**: Will consume the data created by producer thread.
3. **Critical Section (Buffer)** : Here Producer Thread will save data and Consumer will take data.

### Problem :

- We need scyncronization between producer and consumer.
- Producer must not insert data when the buffer is full.
- Consumer must not pick / remove data when the buffer is empty.

### Solution:

> Use three semaphores
> 
1. Mutex / Binary → To get mutual exclusion between producer and consumer
2. Empty (Counting Semaphores) → A counting semaphores. initial value is `n` (no. of empty slots in buffer)
3. Fill (counting Semaphores) → No. of filled Slots. `initial value = 0`