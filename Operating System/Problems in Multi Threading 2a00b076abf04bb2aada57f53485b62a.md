# Problems in Multi Threading

Date: October 9, 2022 11:58 AM
Important: Critical Section | Race Condition | Solution | Locks | Atomic
Status: Done

# Critical Section

Segment of code where process and threads access shared resources, such as common variables and files, and perform write operation on them.

# Race Condition

When two or more threads share same data and try to change it at same time. Because thread scheduling algorithm can swap threads any time we don't know the order. Therefore, the result of the change in data is dependent on  the thread scheduling algorithm. i.e. both threads are racing to access/change the data

For Example : 

c+=1 ⇒ 

1. `temp = c+1`
2. `c = temp`

If thread switching is done after step a then in consistent data will we generated

```python
from threading import *
count = 0

def task():
    global count
    for i in range(100000):
        count += 1

if __name__ == '__main__':
    t1 = Thread(target=task)
    t2 = Thread(target=task)

    t1.start()
    t2.start()
    t1.join()
    t2.join()
    print(count)
```

## Solution of Race Condition

- Create a updating operation **Atomic** like in one cycle
- **Mutual Exclusion**  using LOCKS → No two process can access critical section at the same time
    1. When  a thread starting we use `lock.aquire()`
    2. When when a thread is finished its work in critical section `lock.realease`
    
    ### Disadvantage of locks
    
    1. **Contention** : If a thread locked and terminated afterword then remaining process are gone for indefinite wait with `lock.release` never done 
    2. **Deadlock** : Thread1 locked R1 and Thread2 locked R2 and both required each other resource which are locked 
    3. **Starvation of high priority threads** if a lower priority acquired the critical action first
    4. **Busy Waiting** While a thread is locked the Critical Section other process are in CPU but not doing any work so wasting CPU cycles
    
    Example of Locks
    
    ```python
    from threading import *
    count = 0
    lock = Lock()
    
    def task():
    		lock.acuire()
        global count
        for i in range(100000):
            count += 1
    		lock.release()
    
    if __name__ == '__main__':
        t1 = Thread(target=task)
        t2 = Thread(target=task)
    
        t1.start()
        t2.start()
        t1.join()
        t2.join()
        print(count)
    ```
    
- **Peterson’s Solution** → Only for two threads
    1. Create a array where we keep a thread is ready to enter Critical Section
    2. Turn shows which thread turn is ?