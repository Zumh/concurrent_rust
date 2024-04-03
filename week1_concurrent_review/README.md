## Week1 Concurrent Programming Intro
* Concurrency is a fundamental concept for parallel computing, which is becoming increasingly important as the era of AI and IoT unfolds.
* Concurrency is difficult to reason about due to non-determinism, which arises from interleaving (the order of execution of instructions) and compiler optimizations.
* There are two main approaches to concurrency: lock-based concurrency (easy) and difficult concurrency.
* Lock-based concurrency removes most non-determinism by ensuring that only one agent can access a shared resource at a time. This makes it easy to reason about, but it can also reduce scalability.
* Difficult concurrency allows for more parallelism by carefully managing non-determinism. This requires a deep understanding of the theory and can be challenging to debug, but it can also lead to better performance.
* The key to writing correct and scalable concurrent code is to tame the right amount of non-determinism.

In addition to the above:
* Always start with easy concurrency (lock-based) and only move to difficult concurrency if it is a bottleneck.
* Don't prematurely optimize your code.
* Understand the theory of difficult concurrency, as this will make it easier to apply in practice.
* Concurrent code is usually small but can be difficult to debug. Use sanitizers, stress testers, assertions, and line-by-line debugging to help you find bugs.
* Mathematical and PL(Programming Language) thinking can help you debug concurrent programs by forcing you to think carefully about the safety and correctness of your code.

## In Short
* Focus on two main aspects:
    * Learning about safe APIs of existing concurrency libraries like locks and condition variables.
    * Implementation of concurrent libraries like concurrent stacks, queues, and garbage collectors.
* There are two types of concurrency: lock-based concurrency and lock-free concurrency.
    * Lock-based concurrency is easier to reason about but may not be very scalable.
    * Lock-free concurrency is more difficult to reason about but can be more scalable.
* The instructor advises students to start with lock-based concurrency for its simplicity and only move to lock-free concurrency when necessary.
* Debugging concurrent programs is more difficult than debugging sequential programs and the course will cover tools and techniques for debugging concurrent programs.
- http://googleusercontent.com/youtube_content/1

