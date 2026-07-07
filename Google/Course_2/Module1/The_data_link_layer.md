### Ethernet
The protocol most widely used to send data across individual links 
-  ​If two computers were to send data across the wire at the same time, ​this would result in literal collisions of the electrical current representing our ​ones and zeros, leaving the end result unintelligible. ​Ethernet as a protocol solved this problem by using a technique known as carrier ​sense.

### CSMA/CD
Used to determine when the communications channels are clear, and when a device is free to transmit data 
- ​The way CSMA CD works is actually pretty simple. ​If there's no data currently being transmitted on the network segment, ​a node will feel free to send data. ​If it turns out that two or more computers end up trying to send data at the same ​time, the computers detect this collision and stop sending data. ​Each device involved with the collision then waits a random interval of time ​before trying to send data again.

### MAC address
A globally unique identifier attached to an individual network interface 
- It's a 48-bit number normally represented by six grouping of two hexadecimal numbers 

### Hexadecimal 
A way to represent numbers using 16 digits 

| Hexadecimal | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | A | B | C | D | E | F |
|-------------|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Decimal     | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 | 13 | 14 | 15 |

### Octet
In computer networking, any number that can be represented by 8 bits 

### Organizationally Unique Identifier (OUI)
The first three octets of a MAC address 
- Ethernet uses MAC addresses to ensure that the data it sends has both an address for the machine that sent the transmission, as well as the one the transmission was intended for 
- A **unicast** transmission is always meant for just one receiving address 
- If the lest significant bit in the first octet is destination address is set to **zero**, it means that ethernet frame is intended for **only the destination address**
- If the least significant bit in the first octet of a destination address is set to one, it means you're dealing with a multicast frame

### Data packet
An all-encompassing term that represents any single set of binary data being sent across a network link 

### Ethernet frame
A highly structured collection of information presented in a specific order 

### Preamble 
8 bytes or 64 bits long, and can itself be split into two sections 

### Start frame delimiter (SFD)
Signals to a receiving device that the preamble is over and that the actual frame contents will now follow 

### Destination MAC address 
The hardware address of the intended recipient 

### Ether-type field
16 bits long and used to describe the protocol of the contents of the frame 

### VLAN header 
Indicates that the frame itself is what's called a VLAN frame 
- if a **VLAN** header is present, the EtherType field follows it 

### Virtual LAN (VLAN)
A technique that lets you have multiple logic LANs operating on the same physical equipment 

### Payload 
In networking terms, is the actual data being transported, which is everything that isn't a header 

### Frame check sequence 
A 4 byte or 32 but number that represents a checksum value for the entire frame 

- This **checksum value** is calculated by performing what's known as a cyclical redundancy check against the frame 

### Cyclical redundancy check (CRC)
An important concept for data integrity, and is used all over computing, not just network transmissions 
-  ​If the checksum computed by the receiving end doesn't match the checksum in ​the frame check sequence field, then the data is thrown out.