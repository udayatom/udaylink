- #SymmentricEncryption
 
```
openssl enc -aes-256-cbc -base64 -in msg
```

1) *msg* -  is the file contains the plain text, after executing the above commands returns the output as follows after entering the encrypting password

```
cdp@MacBook-Pro Passhome % openssl enc -aes-256-cbc -base64 -in msg

enter aes-256-cbc encryption password:

Verifying - enter aes-256-cbc encryption password:

U2FsdGVkX1+1E4ecANkYKo+jZ9u0kaaUDd27+2JtgAo=

cdp@MacBook-Pro Passhome %
```

2) To write the encrytpted text to the specific file with following command

```
openssl enc -aes-256-cbc -base64 -in msg -out encytpedfile
```

3) To decrypt the encytped file with following command
```
openssl enc -aes-256-cbc -d -base64 -in enc
```
*-d* is used for the decryption, while decrytpting it requires the encrypting password

4) To store the decrypted text in the specific file using the -out attribute

```
openssl enc -aes-256-cbc -d -base64 -in enc -out dec
```  


- #AsymmentricEncryption

1) For generating the keypair using rsa as follows 
```
openssl genrsa -out keypair.pem 2048
```

2) To view only the private key in the base64 format 
```
openssl rsa -in keypair.pem
```

3)  To view the all the values along with the private key
```
openssl rsa -in keypair.pem -text
```

4) To get the detail about the private key except base64
```
openssl rsa -in keypair.pem -text -noout
```   





https://www.youtube.com/channel/UCQ9KcmhK_-wHLuXOdsaaMUw

#Cryptography
#openssl
 #aes

<iframe border=0 frameborder=0 height=400 width=600 src="https://www.youtube.com/embed/-nEh7X4dtuw"></iframe>
