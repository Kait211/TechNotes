### WPA
designed as a short-term replacement that would be compatible with older WEB-enabled hardware with a simple firmware update 

​To address the shortcomings of WEP security, ​a new security protocol was introduced called ​TKIP or the Temporal Key Integrity Protocol.

# TKIP introduced three new features
1. A more secure key derivation method was used to more securely incorporate the IV into the per packer encryption key.

2. A sequence counter was implemented to prevent replay attacks by rejecting out of order packets 

3. A 64-bit MIC or Message Integrity Check was introduced to prevent forging, tampering, or corruption of packets.

Under WPA, the **pre-shared key** is the wifi password you share with people when they come over and want to use your wireless network

### CCMP
Counter Mode CBC-MAC Protocol

### WPA2 Security

- **WPA2:** Uses AES encryption instead of the older, insecure RC4 cipher.
- **CCMP:** Provides encryption and authentication to protect Wi-Fi data.
- **Four-way handshake:** Allows a client and access point to authenticate and establish encryption keys.
- **PMK (Pairwise Master Key):** The main key used to generate other encryption keys.
- **PTK (Pairwise Transient Key):** A temporary key used to encrypt communication between a client and access point.
- The PTK is actually made up of five individual keys, each with their own purpose 
- Two keys are used for encryption and confirmation of EAPol packets, and encapsulating protocol carries these messages 
- Two keys are used for sending and receiving message integrity codes.
- And finally, there's a temporal jey, which actually used to encrypt data
- **GTK (Group Temporal Key):** A shared key used to encrypt broadcast and multicast traffic.
- Since this type of traffic must be readable by all clients connected to an AP, this GTK is shared between all clients 
- It's updated and retransmitted periodically, and when a client dissociates the AP
- **WPA2-Personal (PSK):** Uses a shared Wi-Fi password for authentication.
- **WPA2-Enterprise:** Uses 802.1X authentication, typically with a RADIUS server.
- **WPS (Wi-Fi Protected Setup):** A convenience feature that makes connecting devices to Wi-Fi easier.
- **Offline Brute-Force Attack:** An attacker captures the four-way handshake and attempts to guess the Wi-Fi password offline.
- **Rainbow Tables:** Precomputed values used to speed up password-cracking attempts.

If 802.1x is too complicated for a company, the next best alternative would be WPA2 with AES/CCMP mode.

a long and complex passphrase that wouldn't be found in a dictionary would increase the amount of time and resources an attacker would need to break the passphrase 

If your company values security over convenience, you should make sure that WPS isn't enabled on your APs