### Protocol
A defined set of standards that computers must follow in order to communicate properly 

### Computer Networking
The name we've given to the full scope of how computers communicate with each other 

# Five Layer Network Module
5. Application: The top layer of the TCP/IP model that provides network services directly to user applications, allowing programs like web browsers and email clients to communicate over a network.
4. Transport: Sorts out which client and server programs are supposed to get the data 
3. Network: Allows different networks to communicate with each other through devices known as routers
2. Data Link: Responsible for defining a common way of interpreting these signals so network devices can communicate
1. Physical: Represents the physical devices that interconnect computers 

| # | Layer Name  | Protocol          | Protocol Data Unit | Addressing |
|---|-------------|-------------------|--------------------|------------|
| 5 | Application | HTTP, SMTP, etc.  | Messages           | n/a        |
| 4 | Transport   | TCP/UDP           | Segment            | Port #'s   |
| 3 | Network     | IP                | Packet / Datagram  | IP Address |
| 2 | Data Link   | Ethernet, Wi-Fi   | Frames             | MAC Address|
| 1 | Physical    | n/a               | Bits               | n/a        |

- The **Ethernet standards also define a protocol responsible for getting data to nodes on the same network or link

### Internetwork
A collection of networks connected together through routers, the most famous of these being the internet 

**IP (Internet Protocol)** is responsible for **addressing and routing data packets** between devices across networks. **TCP (Transmission Control Protocol)** is a transport protocol that ensures data is delivered **reliably, in the correct order, and without errors**. **UDP (User Datagram Protocol)** is also a transport protocol, but it sends data **quickly without guaranteeing delivery or order**. The main difference is that **IP routes data**, **TCP prioritizes reliability**, and **UDP prioritizes speed**.