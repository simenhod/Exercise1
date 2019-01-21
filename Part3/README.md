# Reasons for concurrency and parallelism


To complete this exercise you will have to use git. Create one or several commits that adds answers to the following questions and push it to your groups repository to complete the task.

When answering the questions, remember to use all the resources at your disposal. Asking the internet isn't a form of "cheating", it's a way of learning.

 ### What is concurrency? What is parallelism? What's the difference?
 > Concurrency is when two or more tasks can start, run, and complete in overlapping time periods. It doesn't necessarily mean they'll ever both be running at the same instant. For example, multitasking on a single-core machine.

 > Parallelism is when tasks literally run at the same time, e.g., on a multicore processor.
 
 ### Why have machines become increasingly multicore in the past decade?
 > Because it have become difficult to increase the number of transistors in a CPU. Multicore helps increasing the performance and efficiency of the CPU, by doing several prosesses at the sametime by using threads. 
 
 ### What kinds of problems motivates the need for concurrent execution?
 (Or phrased differently: What problems do concurrency help in solving?)
 > The coordination of the simultaneous execution of transactions in a multiuser database system is known as concurrency control. The objective of concurrency control is to ensure the serializability of transactions in a multiuser database environment. Concurrency control is important because the simultaneous execution of transactions over a shared database can create several data integrity and consistency problems. The three main problems are lost updates, uncommitted data, and inconsistent retrievals.
 
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > it depends on the task. Concurrent programs may require more work when writing the code, but gives a reliable output
 
 ### What are the differences between processes, threads, green threads, and coroutines?
 > Fibers, lightweight threads, and green threads are other names for coroutines or coroutine-like things. They may sometimes look (typically on purpose) more like operating system threads in the programming language, but they do not run in parallel like real threads and work instead like coroutines.

 > With threads, the operating system switches running threads preemptively according to its scheduler, which is an algorithm in the operating system kernel. With coroutines, the programmer and programming language determine when to switch coroutines; in other words, tasks are cooperatively multitasked by pausing and resuming functions at set points, typically (but not necessarily) within a single thread.


 ### Which one of these do `pthread_create()` (C/POSIX), `threading.Thread()` (Python), `go` (Go) create?
 > *Your answer here*
 
 ### How does pythons Global Interpreter Lock (GIL) influence the way a python Thread behaves?
 > *Your answer here*
 
 ### With this in mind: What is the workaround for the GIL (Hint: it's another module)?
 > *Your answer here*
 
 ### What does `func GOMAXPROCS(n int) int` change? 
 > *Your answer here*
