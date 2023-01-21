# Complex Scheduling Algos

Date: October 8, 2022 6:17 PM
Important: MLQ | MLFQ Scheduling
Status: Done

## Multi-Level Queue Scheduling (MLQ)

1. Ready Queue is divided into multiple queue depending on priority
2. A process is ***permanently assigned*** to one of the queues depending on memory size, priority, process type etc.
3. Each Queue has its own scheduling algorithm
4. Generally Queue Divided in three Queues
    1. **System Process** → Created by OS(Highest Priority) | **Robin Round Scheduling** 
    2. **Interactive Process** (Foreground Process) → Needs user Input (I/O) | **Robin Round Scheduling**
    3. **Batch Process (Background Process)** → Runs Silently no user input required (least priority preempted by **IP**)  | **FCFS Scheduling** 
5. Convoy Effect is still present for lower priority most visible in Batch Process Que

## Multi Level Feedback Queue Scheduling (MLFQ)

1. Multiple Sub-queues are present
2. Allow the process to move between queues
3. Queues are separated by BT
    1. Higher BT lower queue
    2. I/O Required Process have higher priority so upper queues
    3. Ageing method to counter Convoy Effect
4. Less Starvation
5. More Flexible 
6. Configurable  by user to meet system design requirement