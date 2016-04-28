# pintos-threads
## About Pintos
Pintos is a simple operating system framework for the 80x86 architecture. It supports kernel threads, loading and running user programs, and a file system, but it implements all of these in a very simple way.
## About the project
Pintos implements a minimally functional thread system that does not support a lot of features out of the box. This project aimed at making modifications and extending the thread system to support additional functionalities by overcoming various synchronization problems.
## Project Goals
#### Alarm Clock
Reimplement timer_sleep(), defined in devices/timer.c. Although a working implementation is provided, it "busy waits," that is, it spins in a loop checking the current time and calling thread_yield() until enough time has gone by. Reimplement it to avoid busy waiting.
#### Priority Scheduling
Implement priority scheduling in Pintos. Some of the functionalities which were to be added include priority donation, thread preemption, FIFO thread scheduling in case of all threads having same priority, chain priority donation, multiple priority donations, nested priority donations, thread wakeup ordering based on priority, etc.
#### Advanced Scheduler
Implement a multilevel feedback queue scheduler to reduce the average response time for running jobs on your system. Although this was a part of the project, the work on this has not been started/completed.
## Resources
1. [Stanford Pintos Threads](https://web.stanford.edu/class/cs140/projects/pintos/pintos_2.html)
