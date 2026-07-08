- On a local area network or LAN, ​nodes can communicate with each ​other through their physical Mac addresses. ​

- ​IP addresses are a 32-bit long numbers made up of ​four octets and each octet is ​normally described in decimal numbers. ​Eight bits of data or a single octet can ​represent all decimal numbers from 0-255. ​For example, 12.34.56.78 is a valid IP address, ​but 123.456.789.100 would not ​be because it has numbers ​larger than could be represented by eight bits. ​

- IP addresses belong to networks, not to the devices attached to those networks

- Your laptop will always have ​the same MAC address no matter where you use it, ​but it'll have a different IP address assigned to it ​at an Internet cafe than it would when you're at home. 

- remember that on many modern networks, ​you can connect a new device and ​an IP address will be assigned to it ​automatically through a technology known ​as Dynamic Host Configuration Protocol. ​An IP address assigned this ​way is known as a dynamic IP address. ​The opposite of this is known as a static IP address, ​which must be configured on a node manually

### IP datagram
A highly structured series of fields that are strictly defined 

- The most common version of IP is version 4 or IPv4

### Header Length field
Almost always 20 bytes in length when dealing with IPv4

### Service type field
These 8 bits can be used to specify details about quality of service or Qos, technologies 

### Total length field
Indicates the total length of the IP datagram it's attached to 

### Identification Field
A 16-bit number that's used to group messages together

- The maximum size of a single datagram is the largest number you can represent with 16 bits which is 65,535

- If the total amount of data that needs to be sent is larger than what can fit in a single datagram, the IP layer needs to split this data up into many individual packets 

### Flag field 
used to indicate if a datagram is allowed to be fragmented, or to indicate that the datagram has already been fragmented 

### Fragmentation
The process of taking a single IP datagram and splitting it up into several smaller datagrams 

### Time to live (TTL) field
An 8-bit field that indicates how many router hops a datagram can traverse before it's thrown away 

### Protocol field
Another 8-bit field that contains data about what transport layer protocol is being used 

### Header checksum field
A checksum of the contents of the entire IP datagram header 

### IP options field 
An optional field and is used to set special characteristics for datagrams primarily used for testing purposes 

### Padding field
A series of zeros used to ensure the header is the correct total size 

- You might wonder how this relates to what we've learned so far. ​You might remember that in our breakdown of an ethernet ​frame we mentioned a section we described as the data payload section. ​This is exactly what the IP datagram is and ​this process is known as encapsulation. ​The entire contents of an IP datagram are encapsulated as the payload of ​an ethernet frame. ​You might have picked up on the fact that our IP datagram also has a payload ​section. ​The contents of this payload are the entirety of a TCP or UDP packet. ​Hopefully this helps you better understand why we talk about ​networking in terms of layers, each layer is needed for the one above it

- IP addresses can be split into two sections: the **network ID** and the **host ID**

### Address class system
A way of defining how the global IP address space is split up

### Address resolution protocol (ARP)
A protocol used to discover the hardware address of a node with a certain IP address 

### ARP table
A list of IP addresses and the MAC addresses associated with them

- ARP table entries generally expire after a short amount of time to ensure changes in the network are accounted for 