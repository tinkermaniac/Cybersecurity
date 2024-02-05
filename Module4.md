# Module 4: Cryptography

<a id="module41"></a>
### 4.1 Cryptographic Fundamentals

#### Encryption and Decryption

Cryptography is the cornerstone of secure communication. Encryption ensures that information remains confidential during transmission and storage.

*Symmetric Encryption:*
- Utilizes a single key for both encryption and decryption.
- Example: Using the `openssl` command for symmetric encryption with AES:

```bash
openssl enc -aes-256-cbc -in plaintext.txt -out ciphertext.enc
```

*Asymmetric Encryption:*
- Involves a pair of public and private keys for encryption and decryption.
- Example: Generating an RSA key pair with `openssl` :
```bash
openssl genpkey -algorithm RSA -out private_key.pem
openssl rsa -pubout -in private_key.pem -out public_key.pem
```
### #Hash Functions and Digital Signatures

Hash functions create fixed-size outputs (hashes) from variable-size inputs. Digital signatures use asymmetric cryptography to verify the authenticity and integrity of messages.

*Hash Functions:*
- Example: Computing an SHA-256 hash with `openssl` :

```bash
openssl dgst -sha256 file.txt
```

*Digital Signatures:*
- Example: Generating a digital signature with `openssl` :

```bash
openssl dgst -sha256 -sign private_key.pem -out signature.sig file.txt
```

<a id="module42"></a>
### 4.2 Public Key Infrastructure (PKI)
Certificate Authorities (CAs)

Public Key Infrastructure (PKI) relies on Certificate Authorities (CAs) to issue and manage digital certificates.

*Issuing Certificates:*

1. Certificate Signing Request (CSR): Generate a CSR with `openssl` :
   ```bash
   openssl req -newkey rsa:2048 -keyout private_key.pem -out csr.pem
   ```

2. CA Signing: A CA signs the CSR, producing a digital certificate.

#### SSL/TLS Protocols

Secure Sockets Layer (SSL) and its successor, Transport Layer Security (TLS), provide secure communication over the internet.

Configuring SSL/TLS:
- Example: Configuring an Nginx server with SSL:

```nginx

server {
    listen 443 ssl;
    server_name example.com;

    ssl_certificate /path/to/certificate.crt;
    ssl_certificate_key /path/to/private_key.key;

    # Additional SSL configurations...
}
```
### [Go to Index](index.md) | [Previous Module: Operating System Security](Module3.md) | [Next Module: Web Application Security](Module5.md)

*Secure the Future. Learn Cybersecurity.*

### -Ritwik Dadarwal ;)
