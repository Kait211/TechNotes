### Dynamic host configuration protocol (DHCP)
An application layer protocol that automates the configuration process of hosts on a network 

- ​Using DHCP, you can configure a range of ​IP addresses that's set aside for these client devices. ​This ensures that any of these devices ​can obtain an IP address when they need one, ​but solves the problem of having to maintain a list ​of every node on the network and its corresponding IP.

### Dynamic allocation
A range of IP addresses is set aside for client devices and one of these IPs is issued to these devices when they request one 

### Automatic allocation
A range of IP addresses is set aside for assignment purposes 

### Fixed allocation 
requires a manually specified list of MAC address and their corresponding IPs

- When a computer requests an IP, ​the DHCP server looks for its MAC address in ​a table and assigns ​the IP that corresponds to that MAC address. ​If the MAC address isn't found, ​the DHCP server might fall ​back to automatic or dynamic allocation, ​or it might refuse to assign an IP altogether.

### Network time protocol (NTP)
Used to keep all computers on a network synchronized in time

- the entire point of ​DHCP is to help configure the network layer itself.

### DHCP discovery
The Process by which a client configured to use DHCP attempts to get network configuration information 

# DHCP Discovery Process (DORA)

## 1. Discover
- Client **doesn't have an IP address** yet.
- Sends a **DHCP Discover** broadcast to find a DHCP server.
- **Source IP:** `0.0.0.0`
- **Destination IP:** `255.255.255.255` (broadcast)
- **Source Port:** UDP **68**
- **Destination Port:** UDP **67**

## 2. Offer
- DHCP server offers an available IP address.
- Sends a **DHCP Offer** broadcast.
- **Source Port:** UDP **67**
- **Destination Port:** UDP **68**
- Includes the **client's MAC address** so the correct client knows the offer is for it.

## 3. Request
- Client accepts the offered IP.
- Sends a **DHCP Request** broadcast saying:
  > "I want to use this IP address."
- **Source IP:** `0.0.0.0`
- **Destination IP:** `255.255.255.255`

## 4. Acknowledge (ACK)
- DHCP server confirms the assignment with a **DHCP ACK**.
- Client receives:
  - IP address
  - Subnet mask
  - Default gateway
  - DNS server(s)
  - Lease time
- Client can now communicate on the network.

# DHCP Lease
- An assigned IP address is called a **DHCP lease**.
- Every lease has an **expiration time**.
- When the lease expires, the client repeats the **DORA** process to obtain a new lease.
- If the client disconnects, it can **release** the lease so the IP returns to the pool of available addresses.