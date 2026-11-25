### Network hardening 
The process of securing a network by reducing it's potential vulnerabilities through configuration changes and taking specific steps 

### Implicit deny
A network security concept where anything not explicitly permitted or allowed should be denied 

### Analyzing logs
The practice of collecting logs from different network and sometimes client devices on your network, then performing an automated analysis on them

**Logs analysis systems** are configured using user-defined rules to match interesting or atypical log entries 

**Normalizing log data** is an important step, since logs from different devices and systems may not be formatted in a common way 

### Correlation analysis
The process of taking log data from different systems and matching events across the systems 

This is usually called a post fail analysis, since its investigating how a compromise happened after the breach is detected 

### Flood guards
Provide protection against DoS or Denial of Service attacks 

If an attacker can manage to deploy a rogue DHCP server on your network, they could hand out DHCP leases with whatever information they want 
 
DHCP snooping also makes you designate either a trusted DHCP server IP, if it's operating as a DHCP helper, and forwarding DHCP requests to the server, or you can enable DHCP snooping trust on the uplinked port, where legitimate DHCP responses would now come from 

​Now, any DHCP responses coming ​from either an untrusted IP address or ​from a downlink switch port would be ​detected as untrusted and discarded by the switch

ARP (Address Resolution Protocol): A protocol used to find the MAC address associated with an IP address on a local network.

dynamic ARP inspection. ​ARP allows for a Layer 2 man-in-the-middle attack ​because of the unauthenticated nature of ARP. ​It allows an attacker to ​forge an ARP response advertising ​its MAC address as ​the physical address matching a victim's IP address. 

This type of ARP response is called gratuitous ARP response, since it's effectively answering a query that no one made 

### EAP-TLS
An authentication type supported by EAP that uses TLS to provide mutual authentication both the client and the authenticating server 

VPNs are commonly used to provide **secure remote access**, and **link two networks** securely. 