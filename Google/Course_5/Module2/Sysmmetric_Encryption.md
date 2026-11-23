### Cryptography 
hiding messages from potential enemies 

### Encryption
The act of taking a message, called plaintext, and applying an operation to it, called a cipher, so that you receive a garbled, unreadable message as the output, called ciphertext 

### Encryption algorithm
the underlying logic of process that's used to convert the plaintext into ciphertext 

### Cryptosystem 
A collection of algorithms for key generation and encryption and decryption operations that comprise a cryptographic service should remain secure - even if everything about the system is known, except the key

The system should remain secure even if your adversary knows exactly what kind of encryption systems you're employing, as long as your **keys remain secure**

### Cryptography
Overarching discipline that covers the practice of coding and hiding messages from third parties 

the study of this practice is referred to as cryptology 

the opposite of this, looking for hidden messages or trying to decipher coded messages is referred to as cryptanalysis 

### Frequency analysis
The practice of studying the frequency with which letters appear in a ciphertext 

### Steganography
The practice of hiding info from observers, but not encoding it 

These types of encryption algorithms are called symmetric because they use the same key to encrypt and decrypt messages 

### Substitution cipher
an encryption mechanism that replaces parts of your plaintext with ciphertext 

### Stream cipher
Takes a stream of input and encrypts the stream one character or one digit at a time outputting one encryption character or digit at a time

### Block Cipher
The cipher takes data in, places it into a bucket or block of data that's a fixed size, then encodes that entire block as one unit

### Data encryption standard (DES)
Designed in the 1970s by IBM, with some input from the US National Security Agency 

### FIPS
Federal Information Processing Standard 

DES is a symmetric block cipher that uses 64-bit key sizes and operates on blocks 64-bits in size 

though the key size is technically 64-bits in length, 8-bits are used only for parity checking, a simple form of error checking 

This means that real world key length for DES is only 56-bits

Key length is super important in cryptography since it essentially defines the maximum potential strength of the system

### Advances encryption standard (AES)
Also a symmetric block cipher, similar to DES in which it replaced 

AES uses 128-bit blocks, twice the size of DES blocks, and supports key lengths of 128-bit, 192-bit, or 256-bit

Because of the large key size, brute-force attacks on AES are only **theoretical** right now, because the computing power required (or time required using modern tech) exceeds anything feasible today

An important thing to keep in mind when considering various encryption algorithms is **speed** and **ease of implementation**

### RC4 (Rivest Cipher 4)
A symmetric stream cipher that gained widespread adoption because of its simplicity and speed 

# Symmetric vs. Asymmetric Encryption

## Symmetric Encryption

**Definition:** An encryption method that uses the same key to encrypt and decrypt data.

### How it works:
1. The sender encrypts a message using a secret key.
2. The receiver uses the same secret key to decrypt the message.
3. Both people must have access to the same key.

**Example:** Alice encrypts a message using a secret key and sends it to Bob. Bob uses that same key to decrypt and read the message.

### Pros
- Fast encryption and decryption.
- Works well with large amounts of data.
- Requires less computing power.
- Efficient for securing network communications.

### Cons
- Both parties must securely share the same key.
- If someone steals the key, they can decrypt the data.
- Managing and distributing keys becomes difficult when there are many users.

---

## Asymmetric Encryption

**Definition:** An encryption method that uses two different keys: a public key and a private key.

### How it works:
1. Each user has a public key and a private key.
2. The public key can be shared with others.
3. The private key must be kept secret.
4. Someone encrypts a message using the receiver's public key.
5. Only the receiver's private key can decrypt that message.

**Example:** Alice wants to send Bob a secure message. She encrypts it using Bob's public key. Bob then uses his private key to decrypt and read the message.

### Pros
- You don't need to share your private key.
- Makes secure communication easier between people who haven't shared a secret key before.
- Supports digital signatures and identity verification.
- Helps securely exchange symmetric encryption keys.

### Cons
- Slower than symmetric encryption.
- Requires more computing power.
- Not as efficient for encrypting large amounts of data.
- Requires proper management of public and private keys.

---

## Main Differences

| Feature | Symmetric Encryption | Asymmetric Encryption |
|---|---|---|
| Keys used | One shared key | Two keys (public and private) |
| Speed | Faster | Slower |
| Key sharing | Secret key must be shared securely | Public key can be shared openly |
| Security | Depends on keeping the shared key secret | Private key must remain secret |
| Best used for | Encrypting large amounts of data | Secure key exchange and digital signatures |

---

## Real-World Example: HTTPS

HTTPS uses both symmetric and asymmetric encryption.

- **Asymmetric encryption:** Helps establish secure communication and authenticate the server.
- **Symmetric encryption:** Used to encrypt the actual data being exchanged because it is faster and more efficient.

## Quick Things to Remember

- **Symmetric =** Same key to encrypt and decrypt.
- **Asymmetric =** Two different keys (public and private).
- **Symmetric =** Faster.
- **Asymmetric =** Easier to exchange keys securely.
- Both can work together to provide secure communication.

**Simple analogy:**
- Symmetric encryption is like sharing one house key. Both people use the same key.
- Asymmetric encryption is like having a public mailbox slot that anyone can put a message through, but only you have the private key to open it.