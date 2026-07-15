### Domain name system (DNS)
A global and highly distributed network service that resolves strings of letters into IP addresses for you
- we need this because it's much easier to type ​www.weather.com into a web browser, ​then it is to remember that one of the IP addresses for ​this site is 184.29.131.121. ​

### Domain name
The term we use for something that can be resolved by DNS

- if you're a global web company, ​you'd want people from all over the world to have ​a great experience accessing your website. ​Instead of keeping all of your web servers in one place, ​you could distribute them across ​data centers across the globe. ​This way, someone in New York visiting ​a website might get served by ​a web server close to New York, ​while someone in New Delhi might ​get served by a web server close to New Delhi. ​Again, DNS helps provide this functionality. 

- ​Because of its global structure, ​DNS lets organizations decide if you're in the region, ​resolve the domain name to this IP. ​If you're in this other region, ​resolve this domain to this other IP. ​

### Name resolution
Process of using DNS to turn a domain name into an IP address is known as name resolution 

- Remember that MAC addresses are ​hard-coded and tied to specific pieces of hardware. But the IP address, subnet mask, ​and gateway for a host must be specifically configured. ​A DNS server is ​the fourth and final part of ​the standard modern network configuration. ​These are almost always the four things that must be ​configured for a host to ​operate on a network in an expected way.

# recap on what needs to be configured 
- IP address
- Subnet mask 
- Gateway for a host 
- DNS server 

# There are five primary types of DNS servers 
1. caching name servers
2. recursive name servers
3. root name servers
4. TLD name servers 
5. authoritative name servers 
- it's important to note that ​any given DNS server can ​fulfill many of these roles at once

### Caching and recursive name servers
Purpose is to store known domain name lookups for a certain amount of time 

### Recursive name servers
Performs full DNS resolution requests 

# Example of how this works
​You and your friend are both ​connected to the same network, ​and you both want to check out facebook.com. ​Your friend enters www.facebook.com into a web browser, ​which means that their computer ​now needs to know the IP of ​www.facebook.com in order to establish a connection. ​Both of your computers are on the same network, ​which usually means that they've both ​been configured with the same name server. ​So your friend's computer asks the name server for ​the IP of www.facebook.com, which it doesn't know. ​This name server now performs ​a fully recursive resolution to ​discover the correct IP for www.facebook.com. ​This IP is then both delivered to ​your friend's computer and stored locally in a cache. ​A few minutes later, you enter ​www.facebook.com into a web browser. ​Again, your computer needs ​to know the IP for this domain, ​so your computer asks ​the local name server it's been configured with, ​which is the same one your ​friend's computer was just talking to. ​Since the domain name www.facebook.com ​had just been looked up, ​the local name server still has ​the IP that it resolved to store ​and is able to deliver that back to ​your computer without having to perform a full lookup. ​This is how the same servers act as a caching server. ​

### Time to live (TTL)
A value, in seconds, that can be configured by the owner of a domain name for how long a name server is allowed to cache an entry before it should discard it and perform a full resolution again 

### Anycast
A technique that's used to route traffic to different destinations depending on factors like location. congestion, or link health 
- Using anycast, a computer can send ​a datagram to a specific IP but could ​see it routed to one of ​many different actual destinations ​depending on a few factors.
- There aren't really ​only 13 physical root name servers anymore. ​It's better to think of them as 13 authorities ​that provide root name lookups as a service.
- The root servers will respond to ​a DNS lookup with ​the TLD name server that should be queried.

### Top-level domain (TLD)
Represents the top of the hierarchical DNS name resolution system 
- Using www.facebook.com as an example again, ​the dot com portion should be thought of as the TLD.
- Authoritative name servers are responsible ​for the last two parts of any domain name, ​which is the resolution at which ​a single organization may be responsible for DNS lookups. 
- Using www.weather.com as an example, ​the TLD name server would point ​a lookup at the authoritative server for weather.com, ​which would likely be controlled by the weather channel, ​the organization itself that runs the site. ​Finally, the DNS lookup could be ​redirected at the authoritative server for weather.com, ​which would finally provide ​the actual IP of the server in question. 