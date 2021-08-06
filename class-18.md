# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Read 18: Cryptography

Cryptography, or the art and science of encrypting sensitive information, was once exclusive to the realms of government, academia, and the military. However, with recent technological advancements, cryptography has begun to permeate all facets of everyday life.

Everything from your smartphone to your banking relies heavily on cryptography to keep your information safe and your livelihood secure.

[Introduction to Cryptography](https://thebestvpn.com/cryptography/)

I must read the content in the above link

### Encryption, decryption, and craking

**Encryption**: scrambling the data according to a secret key.

**Decryption**: recovering the original data from scrambled data by using the secret key.

**Code cracking**: uncovering the original data without knowing the secret, by using a variety of clever techniques.

Encrypting data means that we scramble the original data to hide the meaning of the text, while still making it possible for the data to be unscrambled using a secret key.

Encryption enables two people (or computers!) to share private information over open networks.

The two most common types of encryption used in securing Internet communications are:-

    1. symmetric encryption and 
    2. public key encryption.

A symmetric encryption is any technique where the same key is used to both encrypt and decrypt the data. The Caesar Cipher is one of the simplest symmetric encryption techniques, and of course, one of the easiest to crack.

Since then, cryptologists have invented many more symmetric encryption techniques, including the ones used today to encrypt data like passwords.

Public key encryption is an asymmetric encryption technique which uses different keys for encryption and decryption, allowing computers over the Internet to securely communicate with each other.

High-level process of public key encryption steps are:-

    1. Key generation
        Each person (or their computer) must generate a pair of keys that identifies them: a private key and a public key.

    2. Key exchange
        The sending and receiving computers exchange public keys with each other via a reliable channel, like TCP/IP. The private keys are never exchanged.

    3. Encryption
        The sending computer encrypts the secret data using the receiving computer's public key and a mathematical operation.

    4. Sending encrypted data
        The sender can now safely transmit the encrypted data over the Internet without worry of onlookers.

    5. Decryption
        Now the receiver can decrypt the message, using their private key. That's the only key that can be used to decrypt the message (in the world!).


[Cryptography crash course](https://www.youtube.com/watch?v=jhXCTbFnK8o)














...............................................................................

__Attributions for the following Reference materials and their authors__

[Encryption, descyption, and cracking](https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:online-data-security/xcae6f4a7ff015e7d:data-encryption-techniques/a/encryption-decryption-and-code-cracking)

[Introduction to Cryptography](https://thebestvpn.com/cryptography/)

[>> NEXT (Read: Class 19)](https://wondwosentsige.github.io/code-401-reading-note/class-19)