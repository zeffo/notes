# Types of Operating Systems

1. Batch
	- Automatically execute jobs in batches.
2. Multiprogramming
	- Can load multiple programs into **main memory** from **secondary storage**.
	- Programs are executed concurrently by **context-switching** on a single processor.
	- The running process is switched when it waits for some I/O.
	- Processes which never wait for I/O can cause other processes to never be executed (**process starvation**)
	- Increases CPU Usage and Decreases CPU Idle Time
3. Multitasking
	- An extension of **Multiprogramming** Operating Systems.
	- Programs are executed concurrently by context-switching and **time-sharing** on a single processor.
	- The running process is switched when it waits for some I/O *or* when it's assigned time slice has elapsed.
	- This addresses the flaw of process starvation in multiprogramming systems.
	- Increases CPU Usage *and* **responsiveness**, Decreases CPU Idle Time.
4. Multiprocessing
	- An extension of **Multitasking** Operating Systems.
	- Programs are executed in **parallel** on multiple processors working simultaneously.
	- Increases speed and responsiveness.
5. Real-time
	- Used for applications that process data and events that have critically defined time constraints.
	- Event-driven and preemptive.
6. Distributed
	- Manages a collection of independent and physically seperate, but networked and communicated computers ("Nodes")
	- Jobs are distributed across the nodes.
	- Gives the illusion that there is only a single computational entity.
7. Clustered
	- Similar to **Distributed** Operating Systems.
	- **Clusters** are made up of computers (nodes) sharing the same filesystem.
	- A single faulty node does not make the entire cluster unavailable
	- Used for improving performance and availability 
8. Embedded
	- Designed for **Embedded Systems**, *computer systems dedicated for a single purpose*, such as washing machines and microwaves.
	- Designed to increase functionality and reliability of a specific task.
	- A type of **Real-time** Operating Systems.
	- Highly Compact, Fast and Resource Efficient (due to limited hardware)