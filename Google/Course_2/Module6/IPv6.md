While IPv4 represents addresses with a 32-bit number, IPv6 represents addresses with 128 bits. This 128-bit update allows for a practically unlimited number of IPv6 addresses, 340 trillion trillion trillion addresses to be exact!

IPv5 was an experimental protocol that introduced the concept of connections 

### Multicast
A way of addressing groups of hosts all at once

### Link-local unicast addresses 
Allow for local network segment communications and are configured based upon a host's MAC address 

# IP header
### Version field 
A 4-bit field that defines what version of IP is in use 

### Traffic class field
An 8-bit field that defines the type of traffic contained within the IP datagram, and allows for different classes of traffic to receive different priorities 

### Flow label field
A 20-bit field that's used in conjunction with the traffic class field for routers to make decisions about the quality of service level for a specific datagram 

### Payload length field
a 16-bit field that defines how long the data payload section of the datagram is

### Next header field
A unique concept to IPv6, and needs a little extra explanation 

### Hop limit field 
An 8-bit field that's identical in purpose to the TTL field in an IPv4 header




### IPv6 tunnels
Servers take incoming IPv6 traffic and encapsulate it within traditional IPv4 datagram 

### IPv6 tunnel broker
Companies that provide IPv6 tunneling endpoints for you, so you don't have to introduce additional equipment to your network

Tunneling protocols allow users to carry IPv6 traffic across an IPv4 network. Tunnels are created using IPv6 servers on either end of a network connection

# Key Takeaways

- As IPv6 becomes more widely adopted, IPv6 traffic needs a way to travel over IPv4 networks.
- **Tunneling protocols** let IPv6 traffic travel across an IPv4 network.
- Multiple IPv6 tunneling protocols exist because the technology is still evolving.
- Each tunneling protocol has its own advantages and disadvantages, depending on the IPv6 endpoints being connected.