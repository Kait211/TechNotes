- **Address class system:** A system that defines how the global IP address space is split up.

- **Address Resolution Protocol (ARP):** A protocol used to discover the hardware (MAC) address of a node with a certain IP address.

- **ARP table:** A list of IP addresses and the MAC addresses associated with them.

- **ASN (Autonomous System Number):** A number assigned to an individual autonomous system.

- **Demarcate:** To set the boundaries of something.

- **Demarcation point:** The location where one network or system ends and another begins.

- **Destination network:** The column in a routing table that contains a row for each network the router knows about.

- **DHCP (Dynamic Host Configuration Protocol):** A technology that automatically assigns an IP address to a new device. It is an Application Layer protocol that automates the network configuration process.

- **Dotted decimal notation:** A format that uses dots to separate numbers in a string, such as an IPv4 address (e.g., `192.168.1.1`).

- **Dynamic IP address:** An IP address assigned automatically to a device by DHCP.

- **Exterior gateway protocol:** Protocols used to exchange routing information between independent autonomous systems.

- **Flag field:** A field that indicates whether an IP datagram can be fragmented or whether it has already been fragmented.

- **Fragmentation:** The process of splitting a single IP datagram into several smaller datagrams.

- **Fragmentation offset field:** A field that helps the receiving device reassemble fragmented packets in the correct order.

- **Header checksum field:** A checksum used to verify the integrity of the IPv4 header.

- **Header length field:** A 4-bit field that specifies the length of the IP header. For IPv4, it is usually 20 bytes.

- **IANA (Internet Assigned Numbers Authority):** A non-profit organization that manages global IP address allocation and other Internet protocol resources.

- **Identification field:** A 16-bit field used to identify and group fragments that belong to the same original datagram.

- **Interface:** For a router, the port that connects the router to a network. Routers send and receive data through interfaces, which are also referenced in routing tables.

- **Interior gateway protocol:** Protocols used by routers to exchange routing information within a single autonomous system.

- **IP datagram:** A structured packet of data consisting of an IP header and payload.

- **IP options field:** An optional IPv4 header field used to specify special characteristics, primarily for testing and diagnostics.

- **Network Address Translation (NAT):** A technology that allows many private IP addresses to share a single public IP address.

- **Next hop:** The IP address of the next router that should receive a packet on its way to the destination. If the destination is directly connected, no additional hop is required.

- **Non-routable address space:** Ranges of private IP addresses reserved for use within local networks. These addresses cannot be routed over the public Internet.

- **Padding field:** A series of zeros added to ensure the IP header has the correct total size.

- **Protocol field:** An 8-bit field that identifies which Transport Layer protocol (such as TCP or UDP) is being used.

- **Routing protocols:** Special protocols routers use to exchange routing information and determine the best paths through a network.

- **Service type field:** An 8-bit field used to specify Quality of Service (QoS) information for packet handling.

- **Static IP address:** An IP address that is manually assigned to a device and does not change automatically.

- **Subnet mask:** A 32-bit value, usually written as four decimal octets, that identifies the network and host portions of an IPv4 address.

- **Subnetting:** The process of dividing a large network into smaller subnetworks (subnets).

- **Time-To-Live (TTL) field:** An 8-bit field that specifies the maximum number of router hops a packet can travel before being discarded.

- **Total hops:** The total number of routers or network devices a packet passes through from source to destination. Routers typically choose the path with the fewest hops.

- **Total length field:** A 16-bit field that specifies the total size of the IP datagram, including both the header and data.