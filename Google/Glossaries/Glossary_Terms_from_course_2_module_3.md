- **ACK flag**: One of the TCP control flags. ACK is short for acknowledge. A value of one in this field means that the acknowledgment number field should be examined.

- **Acknowledgement number**: The number of the next expected segment in a TCP sequence.

- **Application layer**: The layer that allows network applications to communicate in a way they understand.

- **Application layer payload**: The entire contents of whatever data applications want to send to each other.

- **CLOSE**: A connection state that indicates that the connection has been fully terminated, and that no further communication is possible.

- **CLOSE_WAIT**: A connection state that indicates that the connection has been closed at the TCP layer, but that the application that opened the socket hasn't released its hold on the socket yet.

- **Connection-oriented protocol**: A data-transmission protocol that establishes a connection at the transport layer and uses this to ensure that all data has been properly transmitted.

- **Connectionless protocol**: A data-transmission protocol that allows data to be exchanged without an established connection at the transport layer. The most common of these is known as UDP (User Datagram Protocol).

- **Data offset field**: The number of the next expected segment in a TCP packet/datagram.

- **Demultiplexing**: Taking traffic that's all aimed at the same node and delivering it to the proper receiving service.

- **Destination port**: The port of the service the TCP packet is intended for.

- **ESTABLISHED**: A TCP connection state indicating that the connection is in working order and both sides are free to send each other data.

- **FIN**: One of the TCP control flags. FIN is short for finish. When this flag is set to one, it means the transmitting computer doesn't have any more data to send and the connection can be closed.

- **FIN_WAIT**: A TCP socket state indicating that a FIN has been sent, but the corresponding ACK from the other end hasn't been received yet.

- **Firewall**: A device that blocks or allows network traffic based on established rules.

- **FTP**: An older method used for transferring files from one computer to another that is still in use today.

- **Handshake**: A way for two devices to ensure that they're speaking the same protocol and will be able to understand each other.

- **Instantiation**: The actual implementation of something defined elsewhere.

- **Listen**: A TCP socket state indicating that a socket is ready and listening for incoming connections.

- **Multiplexing**: The ability of network nodes to direct traffic toward many different receiving services.

- **Options field**: A field sometimes used for more complicated flow control protocols.

- **Port**: A 16-bit number used to direct traffic to specific services running on a networked computer.

- **Presentation layer**: The layer responsible for making sure that unencapsulated application layer data can be understood by the application.

- **PSH flag**: One of the TCP control flags. PSH is short for push. This flag tells the receiving device to deliver currently buffered data to the application as soon as possible.

- **RST flag**: One of the TCP control flags. RST is short for reset. This flag indicates that one side of a TCP connection hasn't been able to recover from a series of missing or malformed segments.

- **Sequence number**: A 32-bit number used to keep track of where a TCP segment belongs in a sequence.

- **Server (or Service)**: A program running on a computer that waits for requests from other computers.

- **Session layer**: The network layer responsible for facilitating communication between applications and the transport layer.

- **Socket**: The instantiation of an endpoint in a potential TCP connection.

- **Source port**: A high-numbered port chosen from the range of ephemeral ports.

- **SYN flag**: One of the TCP control flags. SYN stands for synchronize. This flag is used when establishing a TCP connection and tells the receiving end to examine the sequence number field.

- **SYN_RECEIVED**: A TCP socket state indicating that a listening socket has received a SYN request and has sent a SYN-ACK response.

- **SYN_SENT**: A TCP socket state indicating that a synchronization request has been sent, but the connection has not yet been established.

- **TCP checksum**: A mechanism that helps ensure no data is lost or corrupted during transmission.

- **TCP segment**: The payload portion of an IP datagram consisting of a TCP header and a data section.

- **TCP window**: The range of sequence numbers that may be sent before an acknowledgment is required.

- **URG flag**: One of the TCP control flags. URG is short for urgent. A value of one indicates that the segment is urgent and that the urgent pointer field contains additional information.

- **Urgent pointer field**: A field used with the URG flag to identify data that should be treated as more urgent than other segments.