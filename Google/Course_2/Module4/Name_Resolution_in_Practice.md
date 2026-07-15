DNS in practice operates with a set of defined resource record types. ​These allow for different kinds of DNS resolutions to take place. ​There are dozens of different resource record types defined, but ​a lot of them only serve very specialized purposes

### A record
Used to point a certain domain name at a certain IPv4 IP address 

### Round robin
A concept that involves iterating over a list of items one by one in an orderly fashion 

### Quad A record 
very similar to an A record, except that it returns an IPv6 address instead of an IPv4 address 

### CNAME record
Used to redirect traffic from one domain name to another 
- By setting up a CNAME that points microsoft.com at www.microsoft.com, you'd only have to change the A record for www.microsoft.com

### Mail exchange (MX)
This resource record is used in order to deliver email to the correct server 

### Service record (SRV)
Used to define the location of various specific services 

### Text record (TXT)
Originally intended to be used only for associating some descriptive text with a domain name for human consumption 

# There are three parts of a domain name
1. www
2. google
3. .com

- The last part of a domain name is known as the TLD 

### Top level domain (TLD)
The last part of a domain name 

- Administration and definition of TLDs is handled by a nonprofit ​organization known as ICANN,

### ICANN
The Internet Corporation for Assigned Names and Numbers 

### Domains
Used to demarcate where control moves from TLD name server to an authoritative name server 

### Fully qualified domain name (FQDN)
When you combine all of these parts together you have what's known as this

- DNS can technically support up to 127 levels of domain in total for a  single fully qualified domain name 
- There are some other restrictions in place for how a domain name can be specified. ​Each individual section can only be 63 characters long, and ​a complete FQDN is limited to a total of 255 characters. 

### DNS zones
allow for easier control over multiple levels of a domain 

### Zone files
Simple configuration files that declare all resource records for a particular zone 
- ​A zone file has to contain an SOA or ​a start of authority, resource record declaration.

### Start of authority (SOA)
Declares the zone and the name of the name server that is authoritative for it

### NS records
Indicate other name servers that might also be responsible for this zone 

### Reverse lookup zone files 
These let DNS resolvers ask for an IP and get the FQDN associated with it returned 

### Pointer record (PTR)
Resolves an IP to a name