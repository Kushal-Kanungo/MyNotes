# Dining Philosophers Problem

Date: October 9, 2022 8:20 PM
Important: Each Fork Semaphore | For Deadlock Free ⇒ 4 ph. atmost , Only pick when both fork available | Odd Even ⇒ Even Ph. Right fork first and vic versa
Status: Not started

# Dining Philosophers Problem

### Problem

- We have **5 Philosophers**
- Only Two States Possible
    - Thinking
    - Eating
- They sit on a circular table with noodles and 5 forks
- Thinking State ⇒ Philosopher doesn’t interact with others
- Eating State ⇒ When he gets hungry, he picks two adjacent forks right and left. And he can pick one fork at a time
- Can’t pick a fork which is already picked by other

### Solution

- Each fork a Binary Semaphore
- A ph. calls wait() operation to acquire a fork
- Release fork by calling signal()
- Semaphore fork[5]{1}
    
    This Solution ensure that no two adjacent philosophers are eating simultaneously. But it could create **DeadLock**
    
    - If all ph. pick their left fork it will be Deadlock condition where every ph. in infinite waiting state
        
        Solution
        
        - Allow at most 4 ph. at a time to sitting
        - Allow a ph. to pick fork only if both are available and to do this, he must pick them in critical section
        - Odd-even Rule  ⇒ an odd ph. Picks up first his left fork and then his right fork, whereas an even ph. Picks up his right fork then his left fork.