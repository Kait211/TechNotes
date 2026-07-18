A dial-up connection uses POTS for data transfer, and gets it's name because the connection is established by actually dialing a phone number 

- Transferring data across a dial-up connection ​is done through devices called modems.
- early modems had very low baud rates

### Baud rate
A measurement of how many bits can be passed across a phone line in a second 

- When dial up was used users had to choose between using the internet or the phone 

### Broadband 
any connectivity technology that isn't dial-up internet 

### T-carrier technologies
Originally invented by AT&T in order to transmit multiple phone calls over a single link 
- T-carrier technologies require dedicated lines, which makes them more expensive. ​For this reason, you usually only see them in use by businesses. ​But other broadband solutions also exist for both businesses and consumers. 
- ​T carrier technologies were ​first invented by AT& T in order to ​provision a system that allowed ​lots of phone calls to travel across a single cable. ​Every individual phone call ​was made over individual pairs ​of copper wire before Transmission System 1, ​the first T carrier specification called T1 for short. ​With the T1 specification, ​AT&T invented a way to carry ​up to 24 simultaneous phone calls ​across a single piece of twisted pair copper. ​
- Over the years, the phrase T1 has come to mean ​any twisted pair copper connection capable of ​speeds of 1.544 megabits per second, ​even if it doesn't strictly follow ​the original transmission system 1 specification
- A T3 line is 28 T1s all multiplexed, ​achieving a total throughput speed of ​44.736 megabits per second.

# Digital Subscriber Line (DSL) - Short Notes

- **DSL (Digital Subscriber Line)** uses existing **telephone lines** to provide Internet access.
- It is **much faster than dial-up**.
- **Internet and phone calls can be used at the same time** on the same line.
- DSL uses a **DSL modem (DSLAM)** to maintain the connection.
- Unlike dial-up, the connection is **always on** while the modem is powered.

## Types of DSL

### ADSL (Asymmetric DSL)
- **Faster downloads** than uploads.
- Best for **home users**.
- Lower cost because most people download more than they upload.

**Example:**
- Downloading videos = Fast
- Uploading files = Slower

### SDSL (Symmetric DSL)
- **Equal download and upload speeds.**
- Originally used by **businesses** hosting servers.
- Now also available for home users.
- Typical speed: **Up to 1.544 Mbps (same as a T1 line).**

### HDSL (High-bit-rate DSL)
- Faster version of SDSL.
- Speeds **greater than 1.544 Mbps**.

## Advantages of DSL
- Faster than dial-up.
- Always connected.
- Can use the phone and Internet at the same time.
- Uses existing phone line infrastructure.

## Easy to Remember

- **Dial-up** = Slow, one at a time (Internet *or* phone).
- **DSL** = Faster, always on, Internet **and** phone together.
- **ADSL** = Download > Upload.
- **SDSL** = Download = Upload.

- Cable Internet connections are usually ​managed by what's known as a cable modem.

### Cable Modem
The device that sits at the edge of a consumer's network and connects it to the cable modem termination system or CMTS
- ​The CMTS is what connects lots of ​different cable connections to an ISP's core network. 

- ​The core of the Internet has ​long used fiber for its connections, ​both due to higher speeds and because fiber allows for ​transmission to travel much ​further without degradation of the signal. ​Remember that fiber connections use light for ​data transmission instead of electrical currents. ​

# Fiber connections
​FTTX stands for Fiber To The X, ​where the X can be one of many things. ​We'll cover a few of these possibilities. ​The first term you might hear is FTTN, ​which means Fiber To The Neighborhood. ​This means that fiber technologies ​are used to deliver data ​to a single physical cabinet ​that serves a certain amount of the population. ​From this cabinet, twisted-pair copper or ​coax might be used for the last length of distance. ​The next version you might come across is FTTB. 
​This stands for Fiber To The Building, ​Fiber To The Business or even Fiber To The Basement, ​since this is generally where ​cables to buildings physically enter. ​FTTB is a setup where ​fiber technologies are used for ​data delivery to an individual building. ​After that, twisted-pair copper is ​typically used to actually ​connect those inside of the building. ​A third version you might hear is FTTH, ​which Stands for Fiber To The Home. ​This is used in instances where fiber is actually run to ​each individual residence in ​a neighborhood or apartment building. 

- ​FTTH and FTTB may both also be referred to as FTTP, ​Fiber To The Premises. ​Instead of a modem, the demarcation point for ​fiber technologies is known as ​Optical Network Terminator or ONT.

### Optical Network Terminator (ONT)
Converts data from protocols the fiber network can understand, to those that more traditional, twisted-pair copper networks can understand 
- Optical Network Terminator (ONT) is the demarcation point for fiber technologies

# Broadband Protocols

## PPP (Point-to-Point Protocol)
- Data Link Layer protocol.
- Sends data between **two directly connected devices**.
- Provides:
  - Authentication
  - Error checking
  - Compression

## PPP Authentication
- **PAP:** Password-based authentication.
- **CHAP:** More secure, repeatedly verifies identity.

## FCS (Frame Check Sequence)
- Checks if data was damaged during transmission.

## Encapsulation
- Each network layer adds headers/trailers to data.
- Receiver removes them (**de-encapsulation**).

## PPPoE (PPP over Ethernet)
- PPP inside an Ethernet frame.
- Used with some **DSL internet connections**.
- Adds PPP features to Ethernet.

## Key Difference
- **PPP = direct connection between two devices**
- **PPPoE = PPP sent over Ethernet**

- Unlike LAN or a local area network, WAN stands for wide area network.

### Wide Area Networks (WAN)
Acts like a single network, but spans across multiple physical locations 

# LAN vs WAN

## LAN (Local Area Network)
- Small area (home, school, office).
- Faster and cheaper.
- Connects nearby devices.

## WAN (Wide Area Network)
- Large area (cities, countries, Internet).
- Slower and more expensive.
- Connects distant networks.

## Why use each?
- LAN = devices close together.
- WAN = connect networks far apart.

Example:
Home Wi-Fi = LAN  
Internet = WAN

Your Device
   ↓
LAN (Wi-Fi/Ethernet)
   ↓
Router
   ↓
WAN (Internet)
   ↓
Google

- Your router is basically the bridge between your LAN and the WAN.

# WAN Basics

## WAN
- Connects LANs over large distances.
- Uses ISPs and WAN routers.
- VPNs secure WAN connections over the Internet.

## WAN Router
- Connects a LAN to a WAN.
- Routes traffic between networks.

## SD-WAN
- Software-based WAN.
- Easier and cheaper to manage.

## WAN Optimization
- **Compression:** Makes files smaller.
- **Caching:** Stores copies locally for faster access.
- **Traffic shaping:** Controls/prioritizes traffic.
 - bandwidth throttling: controlling network traffic volume during peak use times
 - rate limiting: capping maximum data rates/speeds
 - use of complex algorithms: classifying and prioritizing data to give preference to more important traffic (e.g., an organization might want to prioritize private LAN-to-LAN traffic within the organization’s WAN and give a lower priority to employees accessing the public Internet).

## Packet Switching
- Breaks data into packets.
- Packets travel and are rebuilt at the destination.

## MPLS
- Uses labels to route data faster.

# Main idea:
WAN connects distant LANs. Routers connect them. VPNs secure them.

### A point-to-point VPN, 
also called a site-to-site VPN, ​establishes a VPN tunnel between two sites. 
- This operates a lot like ​the way that a traditional VPN setup ​lets individual users act as ​if they're on the network they're connecting to. ​It's just that the VPN tunneling logic ​is handled by network devices ​at either side so that users ​don't all have to establish their own connections. 

![site_to_sit_vpn Diagram](../../images/site_to_sit_vpn.png)

- The Internet Service Provider (ISP) handles sending data from one site to another.