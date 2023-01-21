# Concurrency & Multi threading

Date: October 9, 2022 11:18 AM
Important: Concurrency | Threads | Thread Scheduling | Benefits
Status: Done

# Concurrency

- Ability of OS to perform multiple instruction at same time
- To achieve concurrency process is divided into Threads.

# Threads

> Multi Threading is only possible in more than 1 CPU
> 
- A sub process or light weight process
- Threads are independent of each other means they have independent path of execution
- Used to achieve parallelism
- Threads of a process share same memory space assigned to process  by OS

Example. **MS Word have three process** 

1. Text Editor
2. Spell Checker
3. Text Format

## Thread Scheduling

- Threads are scheduled for execution based on priority
- **Thread Context Switching** → OS saves current state and switch
- Fast Switching as compared to process switching. *Cache is same for a processor*
- Each thread has a **Program Counter**
- Depending on Thread Scheduling Algorithms threads are scheduled
- **TCB → Thread Control Block**

# Benefits of Multi Threading

- Responsiveness
    
    Interactive programs are more responsive
    
- Resource Sharing
    
    If instead of threads we divided into process then resource sharing will be complex
    
    We had to IPC Inter Process Communication
    
- Economy
    
    More economical to allocate resources and other things then process
    
- Better utilises Multi Cores
    
    

In cpp multi threading is achieved by `#include<threads>`

```cpp
#include<iostream>
#include<threads>
using namespace std;
void taskA(){
	for(int i=0; i<10; i++ )
		cout << "Task A";
}
void taskB(){
	for(int i=0; i<10; i++ )
		cout << "Task B";
}

int main(){
// taskA assigned to thread 1
thread t1(taskA);
// taskB assigned to thread 2
thread t2(taskB);

// to wait until task are finished
t1.join();
t2.join();
}
```