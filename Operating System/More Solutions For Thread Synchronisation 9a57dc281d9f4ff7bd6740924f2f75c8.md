# More Solutions For Thread Synchronisation

Date: October 9, 2022 1:01 PM
Important: Conditional Variable ⇒ Save Busy Waiting signals when CS free | Semaphores ⇒ Int variable to for finite threads to access CS
Status: Done

# Conditional Variables

- This variables that lets the thread wait until a certain condition occurs.
- For this wait period CPU is freed from thread. So no busy waiting here unlike locks
- Internally it also uses locks
- Thread can enter a wait state only when it has acquired a lock. When a
thread enters the wait state, it will release the lock and wait until another
thread notifies that the event has occurred. Once the waiting thread enters
the running state, it again acquires the lock immediately and starts executing.

```python
from threading import *
import time

cond = Condition()
done = 1

def task(name):
    global done
    with cond:
        if done == 1:
            done = 2
            print("Waiting on condition variable cond: ", name)
            cond.wait()
            print("Condition met: ", name)
        else:
            for i in range(5):
                print('-')
                time.sleep(1)
            print("Signaling condition variable cond: ", name)
            cond.notify_all()
            print("Notification done ", name)

if __name__ == '__main__':
    t1 = Thread(target=task, args=('Task 1', ))
    t2 = Thread(target=task, args=('Task 2', ))

    t1.start()
    t2.start()
    t1.join()
    t2.join()
```

 

# Semaphores

- In semaphores we can define how many threads can access CS at a time.
- Syncronization Process
- It is an **integer** equal to number of resource
- Multiple thread can go and execute **C.S. concurrently**
- It allows **finite number of threads** to access resource whereas mutex/locks can only one
- **Binary Semaphore** : value can be 0 or 1
    - Same as mutex locks
- **Counting Semaphore**
    - Can range over unrestricted domain
    - Control access to finite number of instances
    - To overcome the need for busy waiting, we can modify the definition of
    the wait () and signal () semaphore operations. When a process executes the
    wait () operation and finds that the semaphore value is not positive, it must
    wait. However, rather than engaging in busy waiting, the process car block
    itself. The block- operation places a process into a waiting queue associated
    with the semaphore, and the state of the process is switched to the Waiting
    state. Then control is transferred to the CPU scheduler, which selects another
    process to execute.
    - A process that is blocked, waiting on a semaphore S, should be restarted
    when some other process executes a signal () operation. The process is
    restarted by a wakeup () operation, which changes the process from the
    waiting state to the ready state. The process is then placed in the ready
    queue.

```python
from threading import *
import time

# means 3 resources are available
sem = Semaphore(3)

def task(name):
    sem.acquire()
    for i in range(5):
        print(" {} working".format(name))
        time.sleep(1)
    sem.release()

if __name__ == '__main__':
    t1 = Thread(target=task, args=('Task1',))
    t2 = Thread(target=task, args=('Task2',))
    t3 = Thread(target=task, args=('Task3',))
    t4 = Thread(target=task, args=('Task4',))
    t5 = Thread(target=task, args=('Task5',))

    t1.start()
    t2.start()
    t3.start()
    t4.start()
    t5.start()
    t1.join()
    t2.join()
    t3.join()
    t4.join()
    t5.join()
```