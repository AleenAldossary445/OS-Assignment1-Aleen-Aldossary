# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**

[[A process is a program that is running on the system and has its own memory and resources. A thread is a smaller unit inside a process, and multiple threads can exist within the same process and share memory. The main difference is that processes are heavier and take more time and resources to create, while threads are lighter and faster. Threads share the same memory, so communication between them is easier compared to processes. We used threads in this assignment because they are more efficient and suitable for simulations where tasks need to run concurrently with less overhead.]]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**

[In Round-Robin scheduling, if a process does not finish within its time quantum, it is moved back to the end of the ready queue. This means it will wait for its turn again while other processes get CPU time. The process does not lose its progress, it just pauses and resumes later. For example, in my program output, when P1 used its time but didn’t finish, it was re-queued behind P2 and P3. Then it got CPU time again when its turn came back in the queue.]

Example from my output:
```
[P1 (Priority: 1) added to ready queue ]
```

**Explanation of example:**
[In this example, when process P1 was added to the ready queue, it got a chance to run for its assigned time quantum. Since it didn’t finish within that time, it was paused and moved to the end of the queue, allowing other processes like P2 and P3 to run. From the output, we can see that P1 was not removed; it simply waited for its next turn. When its turn came again, it continued execution from where it left off. This shows how Round-Robin scheduling ensures fairness by giving each process equal chances to use the CPU]

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

[Process P1 starts in the New state when it is created. Then it moves to the Runnable state where it waits in the ready queue for CPU time. When selected, it enters the Running state and begins execution.
If it doesn’t finish or needs to wait (like for I/O), it goes to the Waiting state. After that, it returns to the ready queue and continues execution. Finally, once it finishes completely, it enters the Terminated state.]
1. New: P1 is in the New state when it is first created but has not started execution yet.
 3. Runnable: P1 becomes Runnable after it is ready to run and is waiting in the ready queue for CPU time.
 4. Running: P1 enters the Running state when the CPU starts executing it during its time quantum.
 5. Waiting: P1 goes to Waiting if it needs to wait for something like I/O or if it is paused before finishing.
 6. Terminated: P1 reaches the Terminated state when it completes all its execution and no longer needs the CPU.




---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: [Name of application/scenario]

**Description**: 
[Describe the real-world scenario or application]

**Why Round-Robin works well here**: 
[Explain why Round-Robin scheduling is suitable. Consider fairness, responsiveness, predictability, etc.]

### Example 2: [Name of application/scenario]

**Description**: 
[Describe the real-world scenario or application]

**Why Round-Robin works well here**: 
[Explain why Round-Robin scheduling is suitable. Consider fairness, responsiveness, predictability, etc.]

---

## Summary

**Key concepts I understood through these questions:**
1. 
2. 
3. 

**Concepts I need to study more:**
1. 
2. 
