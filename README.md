# file-encypt-decrypt-using-openssl #

How To Encrypt And Decrypt Files Using OpenSSL On Ubuntu Linux
https://www.youtube.com/watch?v=YU1AI62khIY

**Lists all supported ciphers:**
openssl list-cipher-algorithms

**To Encrypt a file:**
openssl aes-256-cbc -a -salt -in sample.txt -out sample.enc
It will then ask to enter the encryption password, using which it will encrypt the file.

**To Decrypt the file:**
openssl aes-256-cbc -a -salt -d -in sample.enc -out sample.decrypt   [output extension can be anything]
It will ask for password. Please enter the sample password used for encrypting this file.

**Alternate way to encrypt and decrypt using public private key:**
https://linuxconfig.org/easy-way-to-encrypt-and-decrypt-large-files-using-openssl-and-linux
