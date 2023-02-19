# Chapter 1: Introduction to Distributed Systems

## Introduction to Distributed Systems
### What is a Distributed System?
>A distributed system is a software system in which components located on networked computers communicate and coordinate their actions by passing messages


### Parallel vs Distributed System
A **parallel system** uses shared memory
![](../images/1%20-%20parallel%20system.png)

A **distributed system** does not use shared components
![](../images/1%20-%20distributed%20system.png)


### Reasons for Distributed Systems
- Scalability
  - Massive performance
- Distribution of tasks and collaboration
- Reduced latency
- Improved fault tolerance


### Characteristics of Distributed Systems
- Each entity has its own memory
  - Synchronize distributed states
- Entities communicate by passing messages
- Each entity maintains only a part of the complete picture
- A distributed system needs to tolerate (partial) failure


### Building Distributed Systems is Hard
- Often failure
  - Difficult to spot
  - Split-brain scenarios: a state of a server cluster where nodes diverge from each other and have conflicts when handling incoming I/O operations
- Maintaining order and consistency is hard
- Coordination is hard
- Partial operation must be possible
- Testing is hard
- Profiling is hard
  - Slowness


### Fallacies of distributed Systems
- Network is reliable
- Latency is zero
- Bandwidth is infinite
- Network is secure
- Topology doesn't change
- Transport cost is zero
- Network is homogeneous



## Four Main Problems
- Partial failures
  - Some parts of the systems may fail while other parts may still work fine
- Unreliable networks
  - Distributed systems communicate over unreliable networks
- Unreliable time
  - Time can not be used to determine order
- No single source of the truth
  - Distributed systems need to coordinate and agree upon the truth


### Problem 1: Partial Failures


### Problem 2: Unreliable Networks


### Timeouts in Computer Networks


### Problem 3: Time in Computer Systems


### The Trouble with Computer Clocks


### Logical Time


### Problem 4: What is True in a Distributed System?


### Consensus


### Two Generals Problem


### Practical Variant of This Problem



## Distributed Databases
### What is a Distributed Database?


### Replication vs Partitioning


### Replication


### Approaches to Replication


### Synchronous vs Asynchronous Replication


### Problems with Replication Lag: Read-after-write consistency


### Achieving R-A-W consistency


### Problems with Replication Lag: Monotonic Reads


### Achieving Monotonic Reads


### Partitioning


### Replication and Partitioning


### Partitioning Key-Value Data


### Request Routing


### The CAP-Theorem


