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