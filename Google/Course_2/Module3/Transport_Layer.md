### Transport layer
Allows traffic to be directed to specific network applications

### Application layer
Allows these applications to communicate in a way they understand 

# Transport Layer Notes
- The **Transport Layer** is responsible for reliable communication between devices.
- Its main jobs include:
  - **Multiplexing** network traffic
  - **Demultiplexing** network traffic
  - Establishing long-lasting connections
  - Checking for errors and verifying data integrity

## Learning Objectives
By the end of this lesson, you should be able to:

- Explain **multiplexing** and **demultiplexing**
- Identify the differences between **TCP** and **UDP**
- Understand the **TCP three-way handshake**
- Explain how **TCP flags** are used
- Describe how **firewalls** help protect networks

## Multiplexing
- Allows a device to send network traffic to **multiple services** at the same time.
- The **Transport Layer** directs data to the correct destination service.

## Demultiplexing
- Occurs on the receiving device.
- Takes incoming traffic and delivers it to the **correct application or service**.

![Multi_Demultiplexer Diagram](../../images/Multi_Demultiplexer.png)

## Ports
A 16-bit number that's used to direct traffic to specific services running on a networked computer 

- FTP is an older method used for transferring files from one ​computer to another, but you still see it in use today. ​FTP traditionally listens on port 21, so if you wanted to establish a connection to ​an FTP server running on the same IP that our example web server was running on, ​you direct traffic to 10.1.1.100 port 21.

- Just like how an Ethernet frame ​encapsulates an IP datagram, ​an IP datagram encapsulates a TCP segment

- Remember that an Ethernet frame has a payload section, ​which is really just the entire contents ​of an IP datagram. ​Remember also that an IP datagram has a payload section, ​and this is made up of what's known as a TCP segment.

### TCP segment
Made up of a TCP header and a data section 

- This data section, as you might guess, ​is just another payload area for ​where the application layer places its data.

- A TCP header itself is split ​into lots of fields containing lots of information

![TCP Header Diagram](../../images/TCP_header.png)

### Destination port 
The port of the service the traffic is intended for 

### Source port
A high-numbered port chosen from a special section of ports known as ephemeral ports 

### Sequence number
A 32-bit number that's used to keep track of where in a sequence of TCP segments this one is expected to be 

### Acknowledgement number
The number of the next expected segment 

### Data offset field 
A 4-bit number that communicates how long the TCP header for this segment is 

### TCP checksum
Specifies the range of sequence numbers that might be sent before an acknowledgement is requited 

- the checksum is calculated across ​the entire segment and is compared with ​the checksum in the header to make sure that there ​was no data lost or corrupted along the way. 

### Urgent pointer field
Used in conjunction with one of the TCP control flags to point out particular segments that might be more important than others 

### Options field 
It is sometimes used for more complicated flow control protocols 

# TCP Control flags
- **URG (urgent)**
A value of one here indicates that the segment is considered urgent and that the urgent pointer field has more data about this 
- **ACK (acknowledged)**
A value of one in this field means that the acknowledgement number field should be examined 
- **PSH (push)**
The transmitting device wants the receiving device to push currently-buffered data to the application on the receiving end as soon as possible 
- **RST (reset)**
One of the sides in a TCP connection hasn't been able to properly recover from a series of mission or malformed segments 
- **SYN (synchronized)**
It's used when first establishing a TCP connection and makes sure the receiving end knows to examine the sequence number field 
- **FIN (finish)**
When this flag is set to one, it means the transmitting computer doesn't have any more data to send and the connection can be closed 

![Three way handshake Diagram](../../images/Three_way_handshake.png)

### Handshake 
a Way for two devices to ensure that they're speaking the same protocol and will be able to understand each other 

![client/server Diagram](../../images/client_server.png)

- Once one of the devices involved with the TCP connection is ready to ​close the connection, something known as a four-way handshake happens.

![Four_way_handshake Diagram](../../images/Four_way_handshake.png)