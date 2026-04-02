# Development Log

## Instructions
Document your development process as you work on the assignment. Add entries showing:
- What you worked on
- Problems you encountered
- How you solved them
- Time spent

**Requirements**: Minimum 5 entries showing progression over time.

---

## Example Entry Format:

### Entry 1 - [March 27, 2026, 11:40 PM]
**What I did**: Forked the repository and set up my student ID

**Details**: 
- Created GitHub account with university email
- Forked the starter repository
- Changed student ID on line 92 to my actual ID (441234567)
- Compiled and ran the program successfully

**Challenges**: Had to install JDK first because javac wasn't recognized

**Solution**: Downloaded JDK 17 from Oracle website and set PATH variable

**Time spent**: 30 minutes

---

## Your Development Log:

### Entry 1 - [March 27, 2026, 6:45 PM]
What I did:
Started Part 1 by setting up GitHub repository and preparing the project environment.

Details:
I created a GitHub account using my university email and forked the starter repository provided by the instructor. I cloned the repository to my computer and opened the project in my IDE. I updated my student ID in the required location in the code and ensured the project structure was correct.

Challenges: 
Initially, Git was not configured correctly on my computer, and I was unsure how to fork and clone the repository properly.

Solution:
I reviewed GitHub documentation and followed the steps to fork the repository, clone it locally, and connect it to my IDE.

Time spent: 2 hour

---

### Entry 2 - [March 28, 2026, 7:15 PM]
 
What I did:
Compiled and ran the original code to understand how the scheduler works.

Details:
I executed the provided Java program and observed how threads simulate processes in Round-Robin scheduling. I analyzed how each process gets CPU time based on the time quantum and how unfinished processes return to the ready queue. I committed my progress to GitHub after confirming the code runs successfully.

Challenges:
Understanding how the ready queue updates dynamically during execution was confusing at first.

Solution:
I carefully compared the console output with the code logic and reviewed lecture slides on Round-Robin scheduling.

Time spent: 3 hours
---

### Entry 3 - [March 29, 2026, 11:10 PM]

What I did:
Implemented Feature 1 in Part 2 and committed changes to GitHub.

Details:
I modified the output to display process priority when a process is added to the ready queue. I ensured that the change only affected output formatting without modifying the scheduling logic. After testing the output, I committed and pushed the changes to GitHub.

Challenges:
I needed to find the correct location to insert the print statement without affecting program functionality.

Solution:
I reviewed the code structure carefully and inserted the print statement in the correct method where the process enters the ready queue.

Time spent: 3 hours
---

### Entry 4 - [March 30, 2026, 7:30 PM]

What I did:
Implemented Feature 2 and Feature 3 and updated repository on GitHub.

Details:
I added Feature 2 to count the total number of context switches during program execution. Then I implemented Feature 3 to calculate waiting time for each process using System.currentTimeMillis(). I also added a process summary table showing process name, burst time, and waiting time. After verifying correctness, I committed and pushed the updated code.

Challenges:
Determining where to calculate waiting time without changing the original scheduling behavior was difficult.

Solution:
I inserted the waiting time calculation before the process re-enters the ready queue to ensure accurate measurement.

Time spent: 6 hours
---

### Entry 5 - [Aِِpril 2, 2026, 9:05 PM]

What I did:
Completed Part 3 by analyzing output and answering conceptual questions.

Details:
I used the program output to answer questions related to thread vs process, ready queue behavior, and thread states. I explained how Round-Robin scheduling ensures fairness and improves responsiveness in multitasking systems. I reviewed all answers to ensure they match the implemented features and output results.

Challenges:
Understanding thread lifecycle stages and connecting theoretical concepts to program output required careful analysis.

Solution:
I traced one process step by step from creation until termination and matched each stage with thread state definitions.

Time spent: 4 hours
---

### Entry 6 - [Optional - Date and Time]
**What I did**: 

**Details**: 

**Challenges**: 

**Solution**: 

**Time spent**: 

---

## Summary 
Total time spent on assignment: 18 hours

Most challenging part:
Calculating waiting time correctly without modifying the original scheduling logic was the most difficult part.

Most interesting learning:
I learned how multithreading allows multiple processes to share CPU time efficiently and how Round-Robin scheduling ensures fairness between processes.

What I would do differently next time:
I would plan the feature implementation earlier and create a diagram showing thread states before coding.

**Total time spent on assignment**: [18 hours]

