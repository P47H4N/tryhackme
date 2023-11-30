# Encryption - Crypto 101
An introduction to encryption, as part of a series on crypto

## Task 1: What will this room cover?
**I'm ready to learn about encryption**

> No answer needed

## Task 2: Key terms
**I agree not to complain too much about how theory heavy this room is.**

> No answer needed

**Are SSH keys protected with a passphrase or a password?**

> passphrase

## Task 3: Why is Encryption important?
**What does SSH stand for?**

> Secure Shell

**How do webservers prove their identity?**

> certificates

**What is the main set of standards you need to comply with if you store or process payment card details?**

> PCI-DSS

## Task 4: Crucial Crypto Maths
**What's 30 % 5?**

> 0

**What's 25 % 7**

> 4

**What's 118613842 % 9091**

Use this python code we can solve this:
```print(118613842 % 9091)```

> 3565

## Task 5: Types of Encryption
**Should you trust DES? Yea/Nay**

DES is no longer considered secure for short key lengths (56 bits). AES is now used.

> Nay

**What was the result of the attempt to make DES more secure so that it could be used for longer?**

> Triple DES

**Is it ok to share your public key? Yea/Nay**

Public keys can be shared but private keys cannot be shared.

> Yea

## Task 6: RSA - Rivest Shamir Adleman
**p = 4391, q = 6659. What is n?**

```n = p * q```

> 29239669

**I understand enough about RSA to move on, and I know where to look to learn more if I want to.**

> No answer needed

## Task 7: Establishing Keys Using Asymmetric Cryptography
**I understand how keys can be established using Public Key (asymmetric) cryptography.**

> No answer needed

## Task 8: Digital signatures and Certificates
**Who is TryHackMe's HTTPS certificate issued by?**

Click on the lock icon to the left of the browser icon. Click on *Connection is secure*.

![TryHackMe](https://github.com/P47H4N/tryhackme/assets/107831066/c0cd258e-097e-488e-833b-643c7a1edde4)

Click on *Certificate is valid*.

![TryHackMe](https://github.com/P47H4N/tryhackme/assets/107831066/fc07d881-51a1-4e58-ae94-a72a16428827)

Read the certificate.

![TryHackMe Certificate](https://github.com/P47H4N/tryhackme/assets/107831066/af4d4719-08cc-481c-a199-befd44afb15d)

> E1

## Task 9: SSH Authentication
**I recommend giving this a go yourself. Deploy a VM, like Linux Fundamentals 2 and try to add an SSH key and log in with the private key.**

> No answer needed

**Download the SSH Private Key attached to this room.**

> No answer needed

**What algorithm does the key use?**

Open the SSH Private Key attached to this room.

![SSH](https://github.com/P47H4N/tryhackme/assets/107831066/72648f4d-993c-4df7-a305-844f32158bbb)

> RSA

**Crack the password with John The Ripper and rockyou, what's the passphrase for the key?**

We will need to use ssh2john first to convert SSH Private Key to John format. 

```wget https://raw.githubusercontent.com/magnumripper/JohnTheRipper/bleeding-jumbo/run/ssh2john.py```

Now convert the key by using following command:

```python ssh2john.py idrsa.id_rsa > johnkey```

Now crack the password by using following command:

```john --wordlist=/usr/share/wordlists/rockyou.txt johnkey```

We got the answer.

> delicious

## Task 10: Explaining Diffie Hellman Key Exchange
**I understand how Diffie Hellman Key Exchange works at a basic level**

> No answer needed

## Task 11: PGP, GPG and AES
**Time to try some GPG. Download the archive attached and extract it somewhere sensible.**

> No answer needed

**You have the private key, and a file encrypted with the public key. Decrypt the file. What's the secret word?**

Download the file attached to the room. Unzip the compress file ussing ```unzip gpg.zip``` command.

Now import the key by using following command:

```gpg --import tryhackme.key```

Now decrypt the message by using following command:

```gpg --output message.txt --decrypt message.gpg```

> Pineapple

## Task 12: The Future - Quantum Computers and Encryption
**I understand that quantum computers affect the future of encryption. I know where to look if I want to learn more.**

> No answer needed

***Written by: Shariat Ullah Pathan***
