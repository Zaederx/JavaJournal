# Concurrency

Note: When working with Threads, we are at the mercy of the Java Virtual Machine (JVM) and the Operating System when it comes to when threads are scheduled to run.
-Complete Java Master Class, LP academy
- This means that we cannot control order when it comes to concurrent processes.

Purposes of Concurrency

Often there will be times when long running task if ran sequentially, will block the main thread for performing other task. By using threading, the main thread is made free for the os to decide the timing of thread and when best to run some of all of a thread, in order to allow all threads to execute within good time and for apps not to appear to freeze as a thread ties up the main thread.

KeyWords:
- Process - a unit of execution that has its own memory space. When we start an application we start a process.
- Heap - each java application has its own memory space known as the heap. Java applications cannot access each others heaps (the heap is not shared between applications).
- Thread - unit of execution within a process.[For UI - JavaFX Application Thread ]
- Thread Stacks - memory that only that particular Thread can access. [will find out differences between what is stored in the heap and what is stored in the stack later]

Note:
- Creating a thread does not require as many resources as creating a thread.
- Every Java Application runs as a single process.
- Each Process can have multiple threads.
- Every process has a heap, and every thread and a thread stack.
Top Tip:
When working with threads , it is useful to have terminal out put coloured differently in-order to distinguish which thread is running / printing to console


## Multiple threads
- Local variables are stored in the thread stack (which means that each thread has a copy of the local variable in its own stack)
- Instance variables are stored in the process heap (application memory that all threads share).


A thread can be suspended between anyone of the steps of a for loop.
