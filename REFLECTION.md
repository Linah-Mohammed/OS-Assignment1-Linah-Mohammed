# Reflection Questions

## Instructions
Answer the following questions about your learning experience. Each answer should be **at least 5-7 sentences** and show your understanding.

---

## Question 1: What did you learn about multithreading?

**Your Answer: This assignment taught me how multithreading enables the simultaneous execution of several tasks within a single process. I realized that threads are faster to create than processes because they are lightweight units of execution that share memory. I gained knowledge about the various states that threads can go through, including New, Runnable, Running, Waiting, and Terminated. I was able to comprehend how CPU time is distributed equitably across several threads utilizing a time quantum thanks to the Round Robin scheduling simulation. I also discovered how the CPU may effectively move between threads thanks to context switching. One key idea I discovered is that multithreading enhances system performance and responsiveness. I was able to make the connection between theoretical ideas from the textbook and real-world Java implementation thanks to this assignment.**

[Write your answer here. Discuss specific concepts like thread creation, thread states, how threads execute concurrently, what surprised you, etc.]

---

## Question 2: What was the most challenging part of this assignment?

**Your Answer: Understanding where to incorporate the additional features without changing the original scheduling logic was the most difficult aspect of this assignment. Maintaining the Round Robin method precisely as it was given in the beginning code was crucial. It was challenging to implement the waiting time calculation since I had to know when a process was executing on the CPU and when it was waiting in the ready queue. Finding the right place to increase the context switch counter was another difficulty. Additionally, I had to ensure that the sequence of execution was unaffected by the addition of priority. It was necessary to carefully analyze the code in order to comprehend how several threads interacted. I gained a better understanding of CPU scheduling's internal workings thanks to this assignment.**

[Describe the specific challenge. Was it understanding the code? Implementing a feature? Using Git? Explain what made it difficult and how it relates to the course concepts.]

---

## Question 3: How did you overcome the challenges you faced?

**Your Answer: By closely examining the code's structure step by step, I was able to overcome the obstacles. To have a better understanding of thread lifetime and scheduling ideas, I went over the course slides and the textbook chapters. After adding each feature, I regularly evaluated the program to make sure the original behavior was unaffected. I was able to confirm that the context switch counter and waiting time were operating properly thanks to debugging. I implemented one feature at a time, breaking the difficulty down into smaller chores. In order to verify accuracy, I also examined the program's output before and after changes. I was able to successfully finish the task thanks to this methodical technique.**

[Describe your problem-solving approach. Did you read documentation? Ask for help? Debug systematically? What resources did you use? What strategies worked?]

---

## Question 4: How can you apply multithreading concepts in real-world applications?

**Your Answer: Many real-world apps employ multithreading to increase responsiveness and speed. For instance, web browsers use several threads to load scripts, pictures, and web pages all at once. Multithreading is used in games to manage user input, physics computations, and graphics rendering simultaneously. Background threads are used by mobile applications to carry out operations like data downloads without causing the user interface to freeze. Threads are used by operating systems to effectively handle several tasks. Multithreading enhances user experience by enabling systems to manage several tasks at once. Developers can create scalable and effective software systems by having a solid understanding of multithreading.**

[Give specific examples from real applications you use (web browsers, games, mobile apps, etc.). Explain why threads are useful in those scenarios. Connect to what you learned in this assignment.]

---

## Additional Reflections (Optional)

### What would you like to learn more about?
I'd like to know more about synchronization methods like semaphores and mutex locks. Additionally, I'm curious about deadlocks and how operating systems identify and avoid them. It would be beneficial to learn about parallel programming and how to maximize performance with several CPU cores. Additionally, I'd like to investigate how multithreading functions with cloud computing and distributed systems. When creating high-performance software systems, several subjects are crucial.

[Any topics related to threading, concurrency, or operating systems that you're curious about?]

---

### How confident do you feel about multithreading concepts now?
in the middle. I have no trouble grasping the fundamentals of context switching, scheduling algorithms, and threads. I am reasonably confident in my ability to read and edit multithreaded code. I am aware of how threads enhance an application's responsiveness and performance. I still need to practice complex concepts like deadlocks, race situations, and synchronization, though. I think I can get to a higher level of comprehension with additional effort.
[Rate yourself and explain: Beginner / Intermediate / Confident]

[Explain your rating - what do you understand well? What needs more practice?]

---

### Feedback on the assignment
Understanding how CPU scheduling functions in actual systems was greatly aided by the assignment. It gave me hands-on experience putting thread behavior-related features into practice. I was able to make the connection between programming implementation and theoretical principles thanks to the project. The degree of difficulty was suitable and promoted problem-solving. I believe the homework really enhanced my comprehension of multithreading principles. Future assignments should incorporate additional real-world scheduling scenario examples.

[Any comments about the assignment? Was it helpful? Too easy/hard? Suggestions for improvement?]
