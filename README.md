# Producer-Consumer-Problem
The producer generates items and puts items onto the table. The consumer will pick up items. The table can only hold two items at the same time. When the table is complete, the producer will wait. When there are no items, the consumer will wait. We use semaphores to synchronize producer and consumer.  Mutual exclusion should be considered. We use threads in the producer program and consumer program. Shared memory is used for the “table”.
# My Implementation 
I implemented this using one file. Read the comments in producerConsumer.c for more information on my thought process.
# What is happening 
Creates one producer and one consumer. Producer produces 100 random numbers and consumer consumes 100 numbers. The producer and consumer are synchronized working as fast as possible. Producer will most likely produce 2 items to start then consumer will start consuming. Producer will produce after item is consumed.The first item produced is last consumed.
# How to compile
Compile :
$ producerConsumer.c -pthread -o producerConsumer
$ ./producerConsumer
# More information
More producers can be created by altering THREADSIZE   
