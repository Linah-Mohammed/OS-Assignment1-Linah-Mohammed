# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer: A process is a program that is currently in execution and has its own independent memory space and system resources. Each process operates separately from other processes, which makes process creation more expensive in terms of memory and CPU overhead. A thread, on the other hand, is a lightweight unit of execution inside a process that shares the same memory and resources with other threads. Threads are faster to create and allow efficient communication because they share the same address space. In this assignment, threads were used because they efficiently simulate CPU scheduling without requiring multiple independent programs. Multithreading makes the simulation more realistic since operating systems use threads to handle concurrent tasks. Using threads also reduces overhead compared to creating separate processes for each simulated task.**

[Write your answer here. Consider: What is a process? What is a thread? How do they differ in terms of memory, resources, creation overhead? Why are threads more suitable for this simulation?]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer: In Round-Robin scheduling, if a process does not finish during its assigned time quantum, the scheduler pauses the process and places it at the end of the ready queue. This ensures fairness because all processes get equal access to the CPU. The scheduler continues cycling through the queue until each process finishes execution.**

[Write your answer here. Describe the specific behavior - where does the process go? When does it run again? Give an example from your actual program output showing a process that was re-queued.]

Example from my output: Example from my output:
```
▶ P1 executing quantum [4000ms]
Remaining time: 4382ms
↻ P1 yields CPU for context switch

➕ P1 added to ready queue (Priority: 3)

[Paste a relevant snippet from your program output here showing a process being re-queued]
```

**Explanation of example: According to the result, process P1 ran for one complete quantum (4000 ms), however it didn't end because 4382 ms remained. As a result, P1 was positioned at the end of the ready queue after the scheduler executed a context switch. Afterwards, P1 was given CPU time once more until its execution was complete. This behavior illustrates how Round-Robin scheduling ensures that no process monopolizes the CPU, maintaining fairness.**
[Explain what's happening in the output snippet you pasted]

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:
New:
P1 is in the New state when it is first created and added to the ready queue:
➕ P1 added to ready queue (Priority: 3)
Runnable:
P1 becomes Runnable when it is waiting in the ready queue for CPU scheduling. The ready queue shows that P1 is waiting for its turn:
Ready Queue:
[P3 → P4 → ... → P1]
Running:
P1 enters the Running state when the CPU scheduler assigns it execution time:
▶ P1 executing quantum [4000ms]
Waiting:
After using the full quantum without finishing, P1 is paused and waits again in the ready queue:
Remaining time: 4382ms
↻ P1 yields CPU for context switch
Terminated:
Finally, P1 completes execution when its remaining burst time becomes zero:
▶ P1 executing quantum [382ms]
Remaining time: 0ms
✓ P1 finished execution! **



## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**
### Example 1: [Web Server]
**Description**: 
Web servers handle multiple client requests at the same time. Each client request can be processed using a separate thread.
**Why Round-Robin works well here**: 
Round Robin ensures that each client request receives fair CPU time. No single request can monopolize system resources. This improves response time and maintains system responsiveness when many users access the server simultaneously.

### Example 2: [Operating System Task Scheduling]

**Description**: 

Operating systems manage multiple background tasks such as system updates, file indexing, and application processes.

**Why Round-Robin works well here**: 

Round Robin scheduling ensures that each task gets equal CPU time, preventing starvation. It allows the system to remain responsive even when many tasks are running. This improves fairness and ensures efficient CPU utilization.
---

## Summary

**Key concepts I understood through these questions:**
1. Difference between process and thread in terms of memory and performance
2. How Round Robin scheduling ensures fairness between processes
3. Thread lifecycle states and how threads transition during execution



**Concepts I need to study more:**
1. Thread synchronization mechanisms such as mutex and semaphores
2. Deadlock conditions and prevention techniques

