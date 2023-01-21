# Process Scheduling

Date: October 8, 2022 11:37 AM
Important: Scheduling Algos | FCFS | SJF | Priority Scheduling
Status: Done

## Process Scheduling

> Ready Queue to giving it to CPU is know as Process Scheduling it is done by **Dispatcher**
> 

## 2-Types Process Scheduling Algorithms

- **No-Preemption Algorithms**
    1. If process gets CPU it will not leave it until 
        1. It terminates
        2. Or it goes for I/O 
    2. Process-Starvation is High
    3. CPU Utilisation is low
- **Preemption Algorithms**
    1. There is time sharing so every process get chance when time quantum is finished of a process it again goes to ready queue.
    2. Overhead is more
    3. CPU utilisation is high
    4. Process Starvation is low

## Why Process Scheduling ?

1. Maximum CPU utilization.
2. Minimum Turn around time.
3. Minimum Wait time. *If a process in ready queue it should get CPU fast less wait*
4. Response Time. *Process Get CPU first time* 
5. Maximum Throughput. *No. of process completed in per unit time*

## Some Important Terms

- **Throughput**
    
    Number of process completed in per unit of time
    
- **Arrival Time (AT)**
    
    Time when process is arrived at ready queue
    
- **Burst Time (BT)**
    
    Time required by process for its execution
    
- **Turnaround Time (TAT)**
    
    Time taken from first process enters to ready queue till it terminates. `CT-AT`
    
- **Wait Time (WT)**
    
    Time process spends waiting for CPU. `TAT-BT`
    
- **Response Time (RT)**
    
    Time duration between process getting into ready queue and process getting CPU for the first time
    
- **Completion Time (CT)**
    
    Time taken till process gets terminated
    

# Process Scheduling Algorithms

### 1. **FCFS** First Come First Serve Algorithm

> First process come to ready queue scheduled first
> 
- Problem in this algo: **Convoy Effect**
    
    When a process with *high* **BT** burst time is scheduled before than *less* **BT** time processes more process has to wait for it to complete, it increase the **Average Burst Time**, hence lead to *poor resource management*. 
    

### 2. **SJF Shortest Job First**

> Process with least burst time will get CPU first
> 
1. **Non-Preemptive Version** 
    1. Process with least BT will dispatch to CPU first
    2. Must to estimation of BT for each process in Ready Queue “*Which is nearly impossible to guess perfectly*”
    3. Convoy Effect is still possible if very first process comes in Ready Queue is having large BT
    4. Process Starvation might Happen
    5. Criteria for SJF Algo is `AT+BT` 
2. **Preemptive Version →** *Better then non-preemptive*
    1. Criterial is `AT+BT` and preempt
    2. If first process is having a high `BT` but it scheduled, when new process arrived at Ready Queue and having low `BT` then the current process will be preempt by this new process
    3. No Convoy Effect
    4. In a nutshell when a new process arrives with lower `BT` then current running process and it will be switched

### 3. Priority Scheduling [Non-Preemptive]

1. Priority is assigned to process when it is created.
2. SJF is a special case of general priority scheduling with priority inversely proportional to BT
3. At a particular time highest priority process will be scheduled and it will not be preempt

### 4. Priority Scheduling [Preemptive]

1. Current process will be preempted if next job is high priority
2. May cause **indefinite waiting time (Starvation)** for lower priority jobs / **Convoy Effect**
    
    > Ageing is a solution → Gradually increasing the priority of jobs whose wait for long time. `Priority+=1`
    > 
3. Have many overheads 
4. It have Convoy Effect

### 5. Round Robin Scheduling

1. Most popular
2. Like FCFS but preemptive 
3. Designed for time sharing system. Does not depend on BT
4. Criteria: **AT+time quantum(TQ)**.
5. No process is going to wait forever
6. If TQ is small , more context switching , more over head.