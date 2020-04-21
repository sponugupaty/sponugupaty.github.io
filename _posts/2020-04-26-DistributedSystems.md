# Distributed Systems

Here's the table of contents:

1. TOC
{:toc}

## Fundamentals - Mixu ( 4 Hours )
[This](http://book.mixu.net/distsys/ebook.html) is an assessible introduction to distributed systems . This is also a quick read of about 70 pages . 

Key notes -
- The core of distributed programming is dealing with distance and having more than one thing
- Distributed computing is art of solving the same problem that you can solve on a single machine using multiple machines
- This is usuallly because the problem doesnt fit on a single machine 
- Nothing really demands that you use distributed computing
- At a small scale , hardware update is a viable strategy. However at large scale - impossible or cost prohibitive
- High end software is only helpful when it is able to replace slow network accesses with internal memory access
- The advantage of high end software is only when there is large amount of communication among nodes
- Ideally adding a machine should scale a system linearly - but overhead of data to be copied & co-ordination of tasks
- Everything starts with a need to deal with size 
- *Scalability* is the ability of a system , process or network to handle growing amount of work
- Or its ability to be enlarged to accomodate that growth
- 3 Types of scalability 
- Size Scalability - adding nodes makes system linearly faster ; growing dataset doesnt increase latency
- Geographic Scalability - Possible to use multiple datacenters to reduce time to respond to queries . 
- Handle the cross data center latency in a sensible manner 
- administrative scalability - adding nodes doesnt increase the administrative costs of system 
- A scalable system meets the peformance and avalability needs of its users 
- *Performance* is amount of work accomplished compared to time and resources used 
- Depending on context , may involve one of the following 
- 1.short response time/ low latency
- 2.High Throughput / Rate of processing work 
- 3.Low Utilisation of computing resources 
- *Latency* is the difference in time between something happening and becoming visible 
- Or latency is the time gap between something having already happened and becoming visible 
- Information can travel as fast as light and the hardward components also add their own latency 
- *Availability* - The portion of time a system is in a functioning condition 
- Distributed systems take a bunch of non-reliable components and builds a reliable system on top 
- Systems built with redundancy can be tolerant of partial failures and thus will be more available 
- Availability from a technical perspective is mostly about being fault tolerant 
- Availability Metrics -
  1. 90%(1 month ) 
  2. 99%( < 4 days )
  3. 99.9%( < 9 Hrs ) 
  4.99.99%( < 1 hr ) 
  5.99.999%( 5 mins ) 
  6.99.9999%( 31 sec )
- *Fault Tolerance* - Ability of a system to behave in a well-defined manner once fault occurs
- Increasing nodes - increases probability of failure ( reducing availability and increased administrative costs)
- Increasing nodes - increases need for communication among nodes ( reducing performance as scale increases )
- Increase in geographic distance - reducing performance for certain operations 
- an error is incorrect behavior, while an anomaly is unexpected behavior.
- Abstractions help us in making things more manageable by removing the real life constraints not relevant to solving a problem
- 3 Types of models -
  1. System Model ( Synchronous / Asynchronous )
  2. Failure Model ( Crash Fail , Partition , Byzantine )
  3. Consistency Model ( Strong , Eventual )
- Replication and Partition are two fine design techniques
- Partitioning  -
    1. Improves performance by reducing the amount of data that needs examining
    2. Improves availability by allowing partitions to fail independently 
- Replication -
    1. Improves peformance by making additional computing power available to a new copy of data 
    2. Improves availability by creating additional copies of data 
- Replication provides scalability , performance and fault tolerance 
- But issue is keeping independent copies of data on multiple machines in synch
- A good consistency model is crucial and for replication only strong consistency works
   1. Strong consistency - Assume the data is not replicated at all 
-  


## Fundamentals - Particular Class ( 4 Hours )
## Fundamentals - Papers ( 10 Hours )
