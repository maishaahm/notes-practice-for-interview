# Asymptotic Notation

### [Harvard CS50 - Asymptotic Notation (video)](https://www.youtube.com/watch?v=iOq5kSKqeR4)

Analyzes how fast a program's runtime grows asymptotically. In other words, as the size of your inputs increase towards infinity, how does the runtime of your program grow?

Some common running times are:
  - O(n^2)
  - O(n log n)
  - O(n)
  - O(log n)
  - O(1)
O(n^2) are asymptotically slower than O(n), but O(n^2) has the possbility of running faster (e.g. small input sizes).
![image](https://github.com/user-attachments/assets/6c379a5c-1da1-4c41-b146-51daa2e3e547)

**Omega Notation**, Ω, is about the lowerbound, or the best-case scenario.

Binary search can take only 1 step in the best-case scenario, when the item you are looking for is in the middle of the array. This is noted as Ω(1). 
But in the worst-case, it has to perform (log n) split checks of the array to find the right element - O(log n). 

Worst-case upperbounds are reffered to with the **Big-O** that we are already familiar with.

**Theta (Θ) Notation** is when an algorithm's best- and worst-cases are the same.

### Cracking the Coding Interview, Big O Chapter

In industry, people have merged Θ and O together. Big O is closer to what academics means by Θ - offerring the tightest description of the runtime.

1. Drop the constants e.g. O(2N) -> O(N)
2. Drop the non-dominant terms e.g. O(N + log N) -> O(N)

**When do you add/multiply an algorithm with multiple steps?**
1. Add runtimes if the form is "do this, then when you're done, do that."
2. Multiply tuntimes if the form is "do thsi dor each time you do that."

**Amortized Times**

Review D:

**Log N Runtimes**

When you see a problem where the number of elements in the problem space gets halved each time, that will likely be a O(log N) runtime. 
The base of the log does not matter for the purposes of Big O since logs of different bases are only different by a constant factor.

**Recursive Runtimes**

The time complexity of recursion depends on the number of times the function calls itself. If a function calls itself two times, the its time complexcity is O(2^N). 
When you have a recursive function that makes multiple calls, the runtime will often look like O(branches ^N), where the branches are the number of times each recursive calls branches. 

Unlike log, the base of an exponent does matter.

NEXT STEPS: STEP-BY-STEP ANALYSIS OF ALGORITHMS (loops, if-else, nested loops). MORE PRACTICE!

