### Subnetting
The process of taking a large network and splitting it up into many individual and smaller subnetworks or subnets 

- Incorrect subnetting setups are a common problem you might run into as an IT support specialist, so it's important to have a strong understanding of how it works 

- This is where subnetting comes in. ​With subnets, you can split your large network up into many smaller ones. ​These individual subnets will all have their own gateway routers, ​serving as the ingress and egress point for each subnet. 

### Subnet masks 
32-bit numbers that are normally written out as four octets in decimal 

-  ​The number 9 in binary is just 1001. ​But since each octet needs eight bits, ​we need to pad it with some zeros in front. ​As far as an IP address is concerned, ​having a number 9 as the first octet is ​actually represented as 00001001.

- A single 8-bit number can represent 256 different numbers, or more specifically, the numbers 0-255

- The subnet mask 255.255.255.224 ​would translate to 27 ones followed by five zeros. ​This means that we have five bits of ​host ID space or a total of 32 addresses. 

- If you have an eight-bit number, ​you can just perform the math 2^8. ​This gives you 256, ​which lets you know that an eight-bit number can ​represent 256 decimal numbers, ​or put another way, the numbers zero through 255. ​A four-bit number would be 2^4 or 16 total numbers. ​A 16-bit number would be 2^16 or 65,536 numbers.

- we can refer to binary ​as base 2 and decimal as base 10. ​

- Two of the most important operators are **OR** and **AND**

- In computer logic, a 1 represents **true** and a **0** represents **false**

### X OR Y = Z
"if either x or y is true, then Z is true; otherwise, it's false."

- A subnet mask is a way for a computer to use AND operations to determine if an IP address exists on the same network

### Demarcation point 
To describe where one network or system ends and another one begins 

- With CIDR, the network ID ​and subnet ID are combined into one

- ​CIDR basically just abandons ​the concept of address classes entirely, ​allowing an address to be ​defined by only two individual IDs.

- In this case, the last two octets represent the host ID. The first two octets in the subnet mask are all ones in binary (11111111,11111111). This tells the router that the first two octets of the IP address are the subnet ID.

- You always lose two host IDs per network. For example, the subnet mask of 255.255.255.0 has the last octet available for host IDs (256 potential hosts). But remember, zero is generally not used, and 255 is normally reserved as a broadcast address.This means that, really, only the numbers 1-254 are available for assignment to a host.