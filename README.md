# Distributed-Computing-System
Distributed computing refers to a system where **processing** and **data storage** is distributed across multiple devices or systems, rather than being handled by a single central device.

## Advantages of Distributed Systems
Some advantages of Distributed Systems are as follows :

> - Every node in the distributed system is connected to each other because they can share data with others easily.
> - The addition of more nodes in the distributed system is easy.
> - If one node gets failed, it does not lead to the failure of the entire distributed system. Other nodes run fine.
> - Resources like printers can be communicated with multiple nodes.
> - Distributed Systems are widely used in modern computing, big data processing, and content delivery networks.
## Disadvantages of Distributed Systems
Some disadvantages of Distributed Systems are as follows :

> - In distributed systems, it is challenging to provide adequate security because both the nodes and the connections must be protected.
> - In comparison to a single-user system, the database related to distributed systems is more complicated and difficult to manage.
> - While traveling from one node to another node, some data may be lost in the network.

## What is Scalable System in Distributed System?
Software scalability refers to the capacity to adapt to changing workloads by altering the scheduling mechanism and parallelism level.
Scalability is all about making sure your online store (or any system) can handle growth smoothly. It's like having a store that doesn't get overwhelmed when more people want to buy your products. Whether you need a bigger room (vertical scalability) or more distributed rooms (horizontal scalability), the goal is to keep your business running smoothly, no matter how big it gets.

![Physical-Model](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20210209202449/Scaling-Concept.png)"Physical-Model")

- **Need for Scalability Framework**: The scalability framework is required for the applications as it refers to a software system’s ability to scale up in some way when and where required because of the changing demands of the system like increasing users or workload, etc.
- the Spring Framework's scalability is attributed to its modular architecture, support for IoC, AOP, and DI, integration capabilities, and tools like Spring Boot that are tailored for building scalable microservices. These features promote flexibility, maintainability, and efficient resource utilization in large and complex applications.
- **How to Measure Scalability** : The system has the best scalability when the workload and computing resources are increased or lowered by a factor of K at the same time while the average response time of the system or application remains unchanged.

## Role of Middleware in Distributed System

Middleware is software that acts as a link between two or more objects
Middleware simplifies complex distributed applications,
**Block Representation of Middleware:**
![Physical-Model](https://media.geeksforgeeks.org/wp-content/uploads/20211126103158/UntitledDiagram8.jpg)"Physical-Model")

### Advantages of Middleware in Distributed Systems:
> - Middleware is an intermediate layer of software that sits between the application and the network. It is used in distributed systems to provide common services, > > such as authentication, authorization, compilation for best performance on particular architectures, input/output translation, and error handling.
> - Middleware offers a number of advantages to distributed systems. Middleware can be modularized from the application so it has better potential for reuse with other applications running on different platforms. 
> - Application developers can design Middleware so it’s sufficiently high-level that it becomes independent of specific hardware environments or operating system > > > platforms which simplifies porting applications developed on one type of platform onto another without rewriting code or without resorting to inefficient and > > > > > expensive binary compatibility toolsets such as cross-compilers.

## Types of Distributed Computing System Models

### Physical Model
It encompasses the hardware composition of a distributed system in terms of computers and other devices and their interconnections. It is primarily used to **design**, **manage**, **implement** and **determine** the performance of a **distributed system**. consists of the following components:
- **Nodes** : are the end devices that have the ability of processing data, executing tasks and communicating with the other nodes. Each node has an Operating System, execution environment and different middleware requirements that facilitate communication and other vital tasks.
- **Links** : are the communication channels between different nodes and intermediate devices.Generally, physical links are required for high performance and real> > time computing. Different connection types that can be implemented are as follows:
> - **Point-to-point links** – It establishes a connection and allows data transfer between only two nodes.
> - **Broadcast links** – It enables a single node to transmit data to multiple nodes simultaneously.
> - **Multi-Access links** – Multiple nodes share the same communication channel to transfer data. Requires protocols to avoid interference while transmission

- **Middleware** : These are the **softwares** installed and executed on the nodes. By running middleware on **each node**, the distributed computing system achieves a **decentralised control** and **decision-making**. It handles various tasks like **communication with other nodes**, **resource management**, **fault tolerance**, **synchronisation** of different nodes and security to prevent malicious and unauthorised access.
- **Network Topology** – This defines the arrangement of nodes and links in the distributed computing system. The most common network topologies that are implemented are bus, star, mesh, ring or hybrid. Choice of topology is done by determining the exact use cases and the requirements.
- Communication Protocols : are the set rules and procedures for transmitting data from in the links. Examples of these protocols include TCP, UDP, HTTPS, MQTT etc. These allow the nodes to communicate and interpret the data.

  ![Physical-Model](https://media.geeksforgeeks.org/wp-content/uploads/20230622002416/Physical-Model.jpg)"Physical-Model")
