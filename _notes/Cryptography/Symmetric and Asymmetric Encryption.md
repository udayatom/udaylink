**Symmetric Key Encryption:** [Encryption](https://www.geeksforgeeks.org/encryption-its-algorithms-and-its-future/) is a process to change the form of any message in order to protect it from reading by anyone. In Symmetric-key encryption the message is encrypted by using a key and the same key is used to decrypt the message which makes it easy to use but less secure. It also requires a safe method to transfer the key from one party to another.

**Asymmetric Key Encryption:** Asymmetric Key Encryption is based on public and private key encryption techniques. It uses two different key to encrypt and decrypt the message. It is more secure than the symmetric key encryption technique but is much slower.

**Symmetric Key Encryption**| **Asymmetric Key Encryption**
-------------------------------------------|----------------------------------------------
It only requires a single key for both encryption and decryption.|It requires two keys, a public key and a private key, one to encrypt and the other one to decrypt.
The size of cipher text is the same or smaller than the original plain text.|The size of cipher text is the same or larger than the original plain text.
The encryption process is very fast.|The encryption process is slow.
It is used when a large amount of data is required to transfer.|It is used to transfer small amounts of data.
It only provides confidentiality.|It provides confidentiality, authenticity, and non-repudiation.
The length of key used is 128 or 256 bits|The  length of key used is 2048 or higher
In symmetric key encryption, resource utilization is low as compared to asymmetric key encryption.|In asymmetric key encryption, resource utilization is high.
It is efficient as it is used for handling large amount of data.|It is comparatively less efficient as it can handle a small amount of data.
Security is less as only one key is used for both encryption and decryption purpose.|It is more secure as two keys are used here- one for encryption and the other for decryption. 
Examples: 3DES, AES, DES and RC4|Examples: Diffie-Hellman, ECC, El Gamal, DSA and RSA.

**Symmetric Encryption** 
```
The Mathematical Representation is as follows-  
P = D (K, E(P))

where K –> encryption and decryption key  
P –> plain text  
D –> Decryption   
E(P) –> Encryption of plain text
```

**Asymmetric Encryption** 
```
The Mathematical Representation is as follows-  
P = D(Kd, E (Ke,P))  
where Ke –> encryption key

Kd –> decryption key  
D –> Decryption  
E(Ke, P) –> Encryption of plain text using encryption key Ke . P –> plain text
```

 