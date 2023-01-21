# Reader Writer Problem

Date: October 10, 2022 7:21 AM
Important: Solution ⇒ Mutex for Read Count Update / Common Mutex for Read and Write /  Read Count Semaphore
Status: In progress

# Reader Writer Problem

1. **Reader Thread** ⇒ Read Only 
2. **Writer Thread** ⇒ Write and Update 

### Problem

- If more than 1 Reader thread are present then their is no issue
- If more than 1 writer or 1 writer and other thread then their is Race Condition and Data Inconsistency

### Solution

- **Mutex or Binary Semaphore**
    - To ensure mutual exclusion, when **Read Count** (is updated)
- **Wrt**
    - Mutex / Binary Semaphore
    - Common for reader and writer
- **Read Count**
    - integer {0}
    - Tracks how many readers are reading in Critical Section

![Screenshot_2022-10-10-07-31-02_1366x768.png](Reader%20Writer%20Problem%2042ececdb6e4c40edb97354ee96257304/Screenshot_2022-10-10-07-31-02_1366x768.png)

![Untitled](Reader%20Writer%20Problem%2042ececdb6e4c40edb97354ee96257304/Untitled.png)