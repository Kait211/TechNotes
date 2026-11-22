### New Terms and Their Definitions: Course 5, Module 2

**Advanced Encryption Standard (AES):** The first and only public cipher that's approved for use with top secret information by the United States National Security Agency.

**Asymmetric encryption:** Systems where different keys are used to encrypt and decrypt.

**Authentication:** A crucial application for cryptographic hash functions.

**Block ciphers:** The cipher takes data in, places that into a bucket or block of data that's a fixed size, then encodes that entire block as one unit.

**CA (Certificate Authority):** The entity that's responsible for storing, issuing, and signing certificates. It's a crucial component of the PKI system.

**Caesar cipher:** A substitution alphabet, where you replace characters in the alphabet with others, usually by shifting or rotating the alphabet.

**CBC-MAC (Cipher Block Chaining Message Authentication Codes):** A mechanism for building MACs using block ciphers.

**Central repository:** Needed to securely store and index keys. A certificate management system makes managing access to storage, certificates, and certificate issuance easier.

**Certificate fingerprints:** Hash digests of the whole certificate. They aren't actually fields in the certificate itself but are computed by clients when validating or inspecting certificates.

**Certificate Revocation List (CRL):** A means to distribute a list of certificates that are no longer valid.

**Certificate Signature Algorithm:** This field indicates what public key algorithm is used for the public key and what hashing algorithm is used to sign the certificate.

**Certificate-based authentication:** The most secure option, but it requires more support and management overhead since every client must have a certificate.

**Certificate Signature Value:** The digital signature data itself.

**CMACs (Cipher-based Message Authentication Codes):** Similar to HMAC, but instead of using a hashing function to produce a digest, a symmetric cipher with a shared key is used to encrypt the message, and the resulting output is used as the MAC.

**Code signing certificates:** Used for signing executable programs and allow users to verify signatures and ensure that applications haven't been tampered with.

**Cryptanalysis:** Looking for hidden messages or trying to decipher coded messages.

**Cryptography:** The overarching discipline that covers the practice of coding and hiding messages from third parties.

**Cryptology:** The study of cryptography.

**Cryptosystem:** A collection of algorithms for key generation and encryption and decryption operations that comprise a cryptographic service.

**Cryptographic hashing:** Different from encryption because cryptographic hash functions should be one-directional.

**Data binding and sealing:** Involves using the secret key to derive a unique key that's then used for encryption of data.

**Decryption:** The reverse process of encryption; taking the garbled output and transforming it back into readable plaintext.

**DES (Data Encryption Standard):** One of the earliest encryption standards.

**Deterministic:** Means that the same input value should always return the same hash value.

**DH (Diffie-Hellman):** A popular key exchange algorithm, named for its co-inventors.

**DSA (Digital Signature Algorithm):** An example of an asymmetric encryption system, used for signing and verifying data.

**ECDH & ECDSA:** Elliptic curve variants of Diffie-Hellman and DSA, respectively.

**Elliptic Curve Cryptography (ECC):** A public key encryption system that uses the algebraic structure of elliptic curves over finite fields to generate secure keys.

**Encapsulating Security Payload:** Part of the IPsec suite of protocols, which encapsulates IP packets, providing confidentiality, integrity, and authentication of the packets.

**Encryption:** The act of taking a message (plaintext) and applying an operation to it (cipher) so that you receive a garbled, unreadable message as the output (ciphertext).

**Encryption algorithm:** The underlying logic or process used to convert plaintext into ciphertext.

**End-entity (leaf certificate):** A certificate that has no authority as a CA.

**Entropy pool:** A source of random data to help seed random number generators.

**FIPS (Federal Information Processing Standard):** The DES that was adopted as a federal standard for encrypting and securing government data.

**Forward secrecy:** A property of a cryptographic system where, even if the private key is compromised, the session keys are still safe.

**Frequency analysis:** The practice of studying the frequency with which letters appear in ciphertext.

**Full Disk Encryption (FDE):** The practice of encrypting the entire drive in the system.

**Hash collisions:** Two different inputs mapping to the same output.

**Hashing (Hash function):** A type of function or operation that takes in an arbitrary data input and maps it to an output of a fixed size, called a hash or a digest.

**HMAC (Keyed-Hash Message Authentication Codes):** Uses a cryptographic hash function along with a secret key to generate a MAC.

**HTTPS:** Hypertext Transfer Protocol Secure is a secure version of HTTP that ensures communication between your web browser and a website is secured through encryption.

**Intermediary (subordinate) CA:** Means that the entity that this certificate was issued to can now sign other certificates.

**IPsec (Internet Protocol Security):** A VPN protocol that was designed in conjunction with IPv6.

**Issuer Name:** This field contains information about the authority that signed the certificate.

**Kerckhoff's principle:** A principle that states that a cryptosystem should remain secure even if everything about the system is known except for the key.

**Key:** A crucial component of a cipher that introduces something unique into your cipher.

**Key length:** Defines the maximum potential strength of the system.

**Key signing parties:** Organized by people interested in establishing a web of trust. Participants perform the same verification and signing.

**Key size:** The total number of bits or data that comprises the encryption key.

**L2TP (Layer 2 Tunneling Protocol):** Typically used to support VPNs.

**MACs (Message Authentication Codes):** A bit of information that allows authentication of a received message, ensuring that the message came from the alleged sender and not a third party masquerading as them.

**MD5:** A popular and widely used hash function designed in the early 1990s as a cryptographic hashing function.

**MIC (Message Integrity Check):** Essentially a hash digest of the message in question.

**NIST:** National Institute of Standards and Technology.

**Password salt:** Additional randomized data that's added into the hashing function to generate a hash that's unique to the password and salt combination.

**PGP (Pretty Good Privacy) encryption:** An encryption application that allows authentication of data along with privacy from third parties, relying upon asymmetric encryption to achieve this.

**PKI system:** A system that defines the creation, storage, and distribution of digital certificates.

**Pseudo-random:** Something that isn't truly random.

**Public key authentication:** A key pair is generated by the user who wants to authenticate.

**Public key signatures:** A digital signature generated by composing the message and combining it with the private key.

**RA (Registration Authority):** Responsible for verifying the identities of entities requesting certificates to be signed and stored with the CA.

**Rainbow table attacks:** Trade computational power for disk space by pre-computing hashes and storing them in a table.

**Rainbow tables:** A pre-computed table of possible password values and their corresponding hashes.

**Random numbers:** Important in encryption because they help avoid patterns that an adversary could discover through close observation and analysis of encrypted messages over time.

**RC4 (Rivest Cipher 4):** A stream cipher that gained widespread adoption because of its simplicity and speed.

**Remote attestation:** The idea of a system authenticating its software and hardware configuration to a remote system.

**Root Certificate Authority:** Self-signed because they are the start of the chain of trust, so there's no higher authority that can sign on their behalf.

**RSA:** One of the first practical asymmetric cryptography systems to be developed, named for the initials of its three co-inventors: Ron Rivest, Adi Shamir, and Leonard Adleman.

**Secure channel:** Provided by IPsec, which provides confidentiality, integrity, and authentication of data being passed.

**Secure element:** A tamper-resistant chip often embedded in the microprocessor or integrated into the mainboard of a mobile device.

**Secure Shell (SSH):** A secure network protocol that uses encryption to allow access to a network service over unsecured networks.

**Security through obscurity:** The principle that if no one knows what algorithm is being used or the general security practices, then one is safe from attackers.

**Self-signed certificate:** A certificate that has been signed by the same entity that issued the certificate.

**Serial number:** A unique identifier for a certificate assigned by the CA, which allows the CA to manage and identify individual certificates.

**Session key:** The shared symmetric encryption key used during TLS sessions to encrypt data being sent back and forth.

**SHA1:** Part of the Secure Hash Algorithm suite of functions, designed by the NSA and published in 1995.

**Shannon's maxim:** States that the system should remain secure even if your adversary knows exactly what kind of encryption systems you're employing, as long as your keys remain secure.

**SSL 3.0:** The latest revision of SSL, which was deprecated in 2015.

**SSL/TLS Client Certificate:** Certificates bound to clients and used to authenticate the client to the server, allowing access control to an SSL/TLS service.

**SSL/TLS Server Certificate:** A certificate that a web server presents to a client as part of the initial secure setup of an SSL/TLS connection.

**Steganography:** The practice of hiding information from observers, but not encoding it.

**Stream ciphers:** Take a stream of input and encrypt it one character or digit at a time, outputting one encrypted character or digit at a time.

**Subject:** This field contains identifying information about the entity the certificate was issued to.

**Subject Public Key Info:** These two subfields define the algorithm of the public key along with the public key itself.

**Substitution cipher:** An encryption mechanism that replaces parts of your plaintext with ciphertext.

**Symmetric key algorithm:** Encryption algorithms that use the same key to encrypt and decrypt messages.

**TLS 1.2:** The recommended revision of TLS.

**TLS 1.2 with AES GCM:** A specific mode of operation for the AES block cipher that essentially turns it into a stream cipher.

**TLS Handshake:** A mechanism to initially establish a channel for an application to communicate with a service.

**TPM (Trusted Platform Module):** A hardware device typically integrated into a computer that acts as a dedicated cryptographic processor.

**Transport mode:** One of the two modes of operation supported by IPsec. Only the payload of the IP packet is encrypted, leaving the IP headers untouched.

**Trusted Execution Environment (TEE):** Provides a full-blown isolated execution environment that runs alongside the main OS.

**Tunnel:** Provided by L2TP, which permits the passing of unmodified packets from one network to another.

**Tunnel mode:** One of the two modes of operation supported by IPsec. The entire IP packet, including the header and payload, is encrypted and encapsulated inside a new IP packet with new headers.

**Username and password authentication:** Can be used in conjunction with certificate authentication, providing additional layers of security.

**Validity:** This field contains two subfields, Not Before and Not After, which define the dates when the certificate is valid.

**Version:** What version of the X.509 standard the certificate adheres to.

**VPN (Virtual Private Network):** A secure method of connecting a device to a private network over the internet.

**Web of trust:** A system where individuals, instead of certificate authorities, sign other individuals' public keys.

**X.509 standard:** Defines the format of digital certificates, as well as a certificate revocation list (CRL).