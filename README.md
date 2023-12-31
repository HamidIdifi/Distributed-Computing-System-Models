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
Middleware simplifies complex distributed applications.

**Block Representation of Middleware:**

![Physical-Model](https://media.geeksforgeeks.org/wp-content/uploads/20211126103158/UntitledDiagram8.jpg)

### Advantages of Middleware in Distributed Systems:
> - Middleware is an intermediate layer of software that sits between the application and the network. It is used in distributed systems to provide common services, > > such as authentication, authorization, compilation for best performance on particular architectures, input/output translation, and error handling.
> - Middleware offers a number of advantages to distributed systems. Middleware can be modularized from the application so it has better potential for reuse with other applications running on different platforms. 
> - Application developers can design Middleware so it’s sufficiently high-level that it becomes independent of specific hardware environments or operating system
> platforms which simplifies porting applications developed on one type of platform onto another without rewriting code or without resorting to inefficient and  > expensive binary compatibility toolsets such as cross-compilers.

### some examples of middleware

- **Message-Oriented Middleware (MOM)**:

> Examples: Apache Kafka, RabbitMQ, ActiveMQ .
> 
> Purpose: Facilitates asynchronous communication between distributed components by enabling message queuing and pub/sub patterns.

- **Remote Procedure Call (RPC) Middleware**:

> Examples: gRPC, Apache Thrift, Java RMI (Remote Method Invocation).
> 
> Purpose: Enables communication between distributed components by allowing one program to execute code on another program residing on a different machine.

- **Object Request Broker (ORB)**:

> Examples: CORBA (Common Object Request Broker Architecture), ICE (Internet Communications Engine)
> 
> Purpose: Facilitates communication and interaction between objects in a distributed system, allowing objects written in different languages to work together.

- **Web Services Middleware**:

> Examples: SOAP (Simple Object Access Protocol), REST (Representational State Transfer)
> 
> Purpose: Facilitates communication and interoperability between distributed systems over the web. SOAP is a protocol, while REST is an architectural style.

- **Enterprise Service Bus (ESB)**:

> Examples: Apache Camel, Mule ESB, Apache ServiceMix
> 
> Purpose: Facilitates communication, integration, and coordination between various services and applications within an enterprise.

- **Database Middleware**:

> Examples: Java Database Connectivity (JDBC), Object-Relational Mapping (ORM) frameworks like Hibernate
> 
> Purpose: Provides a standardized interface for communication between applications and databases, abstracting the underlying database details.

- **Middleware for Publish/Subscribe**:

> Examples: MQTT (Message Queuing Telemetry Transport), CoAP (Constrained Application Protocol)
> 
> Purpose: Facilitates communication between distributed components using a publish/subscribe model, where one component (publisher) sends messages, and others > > *> > (subscribers) receive them.

- **Distributed Cache Middleware**:

> Examples: Redis, Memcached
> 
> Purpose: Provides a distributed, in-memory cache that enhances performance and scalability by reducing the load on databases.

- **Transaction Middleware**:

> Examples: Java Transaction API (JTA), Microsoft Distributed Transaction Coordinator (MSDTC)
> 
> Purpose: Ensures atomicity, consistency, isolation, and durability (ACID properties) for transactions that span multiple distributed components.

## Types of Distributed Computing System Models

### Physical Model

It encompasses the hardware composition of a distributed system in terms of computers and other devices and their interconnections. It is primarily used to **design**, **manage**, **implement** and **determine** the performance of a **distributed system**.

consists of the following components:
- **Nodes** : are the end devices that have the ability of processing data, executing tasks and communicating with the other nodes. Each node has an Operating System, execution environment and different middleware requirements that facilitate communication and other vital tasks.
- 
- **Links** : are the communication channels between different nodes and intermediate devices.Generally, physical links are required for high performance and real> > time computing. Different connection types that can be implemented are as follows:
> - **Point-to-point links** – It establishes a connection and allows data transfer between only two nodes.
> - **Broadcast links** – It enables a single node to transmit data to multiple nodes simultaneously.
> - **Multi-Access links** – Multiple nodes share the same communication channel to transfer data. Requires protocols to avoid interference while transmission

- **Middleware** : These are the **softwares** installed and executed on the nodes. By running middleware on **each node**, the distributed computing system achieves a **decentralised control** and **decision-making**. It handles various tasks like **communication with other nodes**, **resource management**, **fault tolerance**, **synchronisation** of different nodes and security to prevent malicious and unauthorised access.
- **Network Topology** – This defines the arrangement of nodes and links in the distributed computing system. The most common network topologies that are implemented are bus, star, mesh, ring or hybrid. Choice of topology is done by determining the exact use cases and the requirements.
- 
- **Communication Protocols** : are the set rules and procedures for transmitting data from in the links. Examples of these protocols include TCP, UDP, HTTPS, MQTT etc. These allow the nodes to communicate and interpret the data.

  ![Physical-Model](https://media.geeksforgeeks.org/wp-content/uploads/20230622002416/Physical-Model.jpg)"Physical-Model")

  ### Architectural model

  Architectural model in distributed computing system is the overall design and structure of the system, and how its different components are organised to interact with each other and provide the desired functionalities.
  
  - **Client-Server model** It is a centralised approach in which the clients initiate requests for services and severs respond by providing those services. It mainly works on the request-response model where the client sends a request to the server and the server processes it, and responds to the client accordingly. It can be achieved by using TCP/IP, HTTP protocols on the transport layer. This is mainly used in web services, cloud computing, database management systems etc.
 
   ![](https://media.geeksforgeeks.org/wp-content/uploads/20191016114416/801.png)
 
  - **Peer-to-peer model** – It is a decentralised approach in which all the distributed computing nodes, known as peers, are all the same in terms of computing capabilities and can both request as well as provide services to other peers. It is a highly scalable model because the peers can join and leave the system dynamically
 
   ![](https://media.geeksforgeeks.org/wp-content/uploads/20220826190244/GFGP2PArchitecture.png)
 
  - **Layered model** involves organising the system into multiple layers, where each layer will provision a specific service. Each layer communicated with the adjacent layers using certain well-defined protocols without affecting the integrity of the system. A hierarchical structure is obtained where each layer abstracts the underlying complexity of lower layers.
 
  - **Micro-services model** – In this system, a complex application or task, is decomposed into multiple independent tasks and these services running on different servers. Each service performs only a single function and is focussed on a specific business-capability.

![](https://media.geeksforgeeks.org/wp-content/uploads/20230622020049/Screenshot-2023-06-22-at-15955-AM.jpg)


### Fundamental Model
 It represents the essential components that are required to understand a distributed system’s behaviour. Three fundamental models are as follows:
 #### Interaction Model  
 – Distributed computing systems are full of many processes interacting with each other in highly complex ways. Interaction model provides a framework to understand > the mechanisms and patterns that are used for communication and coordination among various processes. Different components that are important in this model are:
> - **Message Passing** – It deals with passing messages that may contain, data, instructions, a service request, or process synchronisation between different computing nodes. It may be synchronous or asynchronous depending on the types of tasks and processes.

> - **Publish/Subscribe Systems** – Also known as pub/sub system. In this the publishing process can publish a message over a topic and the processes that are

> subscribed to that topic can take it up and execute the process for themselves. It is more important in an event-driven architecture.

> - **Remote Procedure Call (RPC)** – RPC is about calling functions or procedures on another computer as if they were local, making remote actions feel local.
> > It's like asking a friend in another room to do something for you, and you communicate by sending messages (calls and responses).
> > ![Physical-Model](https://media.geeksforgeeks.org/wp-content/uploads/operating-system-remote-call-procedure-working.png)
### Failure Model 
– This model addresses the faults and failures that occur in the distributed computing system. It provides a framework to identify and rectify the faults that occur or may occur in the system.
Fault tolerance mechanisms are implemented so as to handle failures by replication and error detection and recovery methods. Different failures that may occur are:
- **Crash failures** – A process or node unexpectedly stops functioning.
- **Omission failures** – It involves a loss of message, resulting in absence of required communication.
- **Timing failures** – The process deviates from its expected time quantum and may lead to delays or unsynchronised response times.
- **Byzantine failures** – The process may send malicious or unexpected messages that conflict with the set protocols.

### Security Model 
– Distributed computing systems may suffer malicious attacks, unauthorised access and data breaches. Security model provides a framework for understanding the security requirements, threats, vulnerabilities, and mechanisms to safeguard the system and its resources.
Various aspects that are vital in the security model are – 
- **Authentication** – It verifies the identity of the users accessing the system. It ensures that only the authorised and trusted entities get access. It involves –
> - **Password-based authentication** – Users provide a unique password to prove their identity.
> - **Public-key cryptography** – Entities possess a private key and a corresponding public key, allowing verification of their authenticity.
> - **Multi-factor authentication** – Multiple factors, such as passwords, biometrics, or security tokens, are used to validate identity.
- **Encryption** – It is the process of transforming data into a format that is unreadable without a decryption key. It protects sensitive information from unauthorized access or disclosure.

 ![](https://media.geeksforgeeks.org/wp-content/uploads/20220107194600/Screenshot44.png)

- **Data Integrity** – Data integrity mechanisms protect against unauthorised modifications or tampering of data. They ensure that data remains unchanged during storage, transmission, or processing. Data integrity mechanisms include:
> - **Hash functions** – Generating a hash value or checksum from data to verify its integrity.
> - **Digital signatures** – Using cryptographic techniques to sign data and verify its authenticity and integrity.
