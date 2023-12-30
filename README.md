# Distributed-Computing-System-Models
Distributed computing refers to a system where **processing** and **data storage** is distributed across multiple devices or systems, rather than being handled by a single central device.

## Types of Distributed Computing System Models

### Physical Model
It encompasses the hardware composition of a distributed system in terms of computers and other devices and their interconnections. It is primarily used to **design**, **manage**, **implement** and **determine** the performance of a **distributed system**. consists of the following components:
- **Nodes** : are the end devices that have the ability of processing data, executing tasks and communicating with the other nodes. Each node has an Operating System, execution environment and different middleware requirements that facilitate communication and other vital tasks.
> - **Links** : are the communication channels between different nodes and intermediate devices.Generally, physical links are required for high performance and real> > > time computing. Different connection types that can be implemented are as follows:
> **Point-to-point links** – It establishes a connection and allows data transfer between only two nodes.
> **Broadcast links** – It enables a single node to transmit data to multiple nodes simultaneously.
> **Multi-Access links** – Multiple nodes share the same communication channel to transfer data. Requires protocols to avoid interference while transmission

- **Middleware** : These are the **softwares** installed and executed on the nodes. By running middleware on **each node**, the distributed computing system achieves a **decentralised control** and **decision-making**. It handles various tasks like **communication with other nodes**, **resource management**, fault tolerance, **synchronisation** of different nodes and security to prevent malicious and unauthorised access.
- **Network Topology** – This defines the arrangement of nodes and links in the distributed computing system. The most common network topologies that are implemented are bus, star, mesh, ring or hybrid. Choice of topology is done by determining the exact use cases and the requirements.
- Communication Protocols : are the set rules and procedures for transmitting data from in the links. Examples of these protocols include TCP, UDP, HTTPS, MQTT etc. These allow the nodes to communicate and interpret the data.

  ![Physical-Model](https://media.geeksforgeeks.org/wp-content/uploads/20230622002416/Physical-Model.jpg)"Physical-Model")
