# Concurrency

> What is Concurrency?

*Concurrency is the ability of different parts or units of a program to be executed out-of-order or in partial order without affecting the final outcome.*

> What is Parallelism?

*Parallelism is the execution of multiple programs/different parts of a program at the same time.*

**Parallelism is *NOT* Concurrency!**

![[1.png]]
Consider two processes. Both have to wait for some I/O, but at different times.

On multiprocessor systems, they can be executed in **true parallel**. 
Each process will be executed by a seperate processor.

However on single processor systems, they will have to be run sequentially. But, if they are simply run one after the other, time will be lost during the waiting periods.
So, they are executed **concurrently**.

The processor begins with Process 1. As soon as it begins waiting, it switches to Process 2. 
When Process 2 has to wait, it switches back to Process 1.
After Process 1 is complete, it switches back and completes Process 2.

This ensures the CPU is never idle.

This technique is known as **context-switching**.

However Operating Systems that utilize *only* context-switching are flawed. Processes which never wait for I/O will never be switched, which can lead to process-starvation.

This is why context-switching is used alongside **time-sharing**, where processes are given time slices to run in. They are switched when they wait for I/O, *or* their time slice elapses.

