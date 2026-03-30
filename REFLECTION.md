# Reflection Questions

## Instructions
Answer the following questions about your learning experience. Each answer should be **at least 5-7 sentences** and show your understanding.

---

## Question 1: What did you learn about multithreading?

**Your Answer:**

[From this assignment, I learned how multithreading allows multiple tasks to run concurrently instead of executing one process at a time. Working with the Round-Robin scheduler helped me understand how threads share CPU time fairly using a fixed time quantum. I also understood how the Runnable interface works and how each process becomes a thread when Thread.start() is called. Before this assignment, threading was mostly theoretical for me, but implementing it in Java showed how thread execution actually happens step by step. I learned how threads move between different states such as running and waiting depending on scheduling decisions. Another important concept I learned was how synchronization between threads is managed using methods like join() and sleep(). Overall, this assignment helped me connect operating system concepts with real Java programming practice]

---

## Question 2: What was the most challenging part of this assignment?

**Your Answer:**

[The most challenging part for me was tracking waiting time and understanding when exactly a process should update its waiting duration. It was difficult at first because processes continuously leave and re-enter the ready queue in Round-Robin scheduling. I needed to think carefully about when a process starts waiting and when it resumes execution. Another challenge was making sure that the new features did not break the original scheduler logic. Debugging multithreaded behavior was also harder than normal programs because execution order changes every run. Sometimes the output looked correct but the calculations were slightly wrong. This forced me to test the program multiple times and carefully analyze the console output.]

---

## Question 3: How did you overcome the challenges you faced?

**Your Answer:**

[I overcame these challenges by testing each feature separately instead of implementing everything at once. After adding each modification, I ran the simulation several times to verify that the behavior remained correct. I also added temporary print statements to track execution flow and understand how threads were scheduled. Reading the starter code carefully helped me understand where to insert my changes without affecting existing functionality. When I faced confusion about thread behavior, I reviewed lecture materials and searched for examples of Java thread lifecycle usage. Breaking the problem into smaller steps made the implementation easier to manage. Gradually, the logic became clearer as I observed how processes moved through the ready queue.]

---

## Question 4: How can you apply multithreading concepts in real-world applications?

**Your Answer:**

[Multithreading is widely used in real-world systems where multiple tasks must run at the same time. For example, web servers use threads to handle many user requests simultaneously without blocking other users. Another example is modern applications like media players or mobile apps where background tasks run while the user interface remains responsive. The Round-Robin scheduling concept ensures fairness so no task monopolizes the CPU for too long. Game engines also rely on multithreading to manage graphics rendering, physics calculations, and user input concurrently. This assignment showed me how operating systems distribute CPU time efficiently between tasks. Understanding these concepts helps developers build faster and more responsive software systems.]

---

## Additional Reflections (Optional)

### What would you like to learn more about?

[Any topics related to threading, concurrency, or operating systems that you're curious about?]

---

### How confident do you feel about multithreading concepts now?

[Rate yourself and explain: Beginner / Intermediate / Confident]

[Explain your rating - what do you understand well? What needs more practice?]

---

### Feedback on the assignment

[Any comments about the assignment? Was it helpful? Too easy/hard? Suggestions for improvement?]
