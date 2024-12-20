Source : https://terokarvinen.com/trust-to-blockchain/#homework
# Protocol Building Blocks
A protocol is a series of steps, involving two or more parties, designed to accomplish a task.
characteristics Of protocol:

* Everyone involved in the protocol must know the protocol and all of the steps to follow in advance.
* Everyone involved in the protocol must agree to follow it.
* The protocol must be unambiguous; each step must be well defined and there must be no chance of a misunderstanding.
* The protocol must be complete; there must be a specified action for every possible situation.

# Types of Protocol
  Arbitrated Protocols
  
In an Arbitrated Protocol, An arbitrator is a disinterested third party trusted to complete a protocol (see Figure 2.1a). Disinterested means that the arbitrator has no vested interest in the protocol and no particular allegiance to any of the parties involved. Trusted means that all people involved in the protocol accept what he says as true, what he does as correct, and that he will complete his part of the protocol. Arbitrators can help complete protocols between two mutually distrustful parties.

Adjudicated Protocols

Because of the high cost of hiring arbitrators, arbitrated protocols can be subdivided into two lower-level subprotocols. One is a nonarbitrated subprotocol, executed every time parties want to complete the protocol. The other is an arbitrated subprotocol, executed only in exceptional circumstances—when there is a dispute. This special type of arbitrator is called an adjudicator 
An adjudicator is also a disinterested and trusted third party. Unlike an arbitrator, he is not directly involved in every protocol. The adjudicator is called in only to determine whether a protocol was performed fairly.

Self-Enforcing Protocols

The protocol itself guarantees fairness there is a mutual trust between the parties. 

# Attacks against Protocols

There are two types of attacks agaisnt protocols Active vs passive attacks. 
Someone not involved in the protocol can eavesdrop on some or all of the protocol. This is called a passive attack, because the attacker does not affect the protocol.
Alternatively, an attacker could try to alter the protocol to his own advantage. He could pretend to be someone else, introduce new messages in the protocol, delete existing messages, substitute one message for another, replay old messages, interrupt a communications channel, or alter stored information in a computer. These are called active attacks, because they require active intervention. The form of these attacks depends on the network.

# COMMUNICATIONS USING PUBLIC-KEY CRYPTOGRAPHY
In public key cryptography system there are two keys one is public which can be shared with anyone who wants to encrypt the message and the other one is private which is only known to the person intented to decrupt the message encrypted with the public key . 
In most practical implementations public-key cryptography is used to secure and distribute session keys; those session keys are used with symmetric algorithms to secure message traffic. This is sometimes called a hybrid cryptosystem.
# Digital signature 
Key Concepts of Digital Signatures
* Authentication: Digital signatures verify that the sender of a message is genuine. Only the holder of the private key associated with the signature can create a valid signature, making it possible to authenticate the sender’s identity.

* Data Integrity: Digital signatures provide assurance that the content has not been altered since it was signed. If the data changes after signing, the signature verification will fail, alerting the recipient to potential tampering.

* Non-repudiation: Once a document or transaction is signed, the signer cannot deny their involvement. This is crucial for legal, financial, and official documents, as it provides evidence of the sender’s commitment to the contents.

# How Digital Signatures Work
Digital signatures rely on public-key cryptography, particularly a pair of keys: a private key for signing and a public key for verification. The process typically involves the following steps:

Hashing: The message or document is hashed using a secure hashing algorithm (e.g., SHA-256) to create a unique fixed-size hash value. This hash represents the document in a compact form.

Signing: The signer uses their private key to encrypt the hash, creating the digital signature. This signature is unique to both the signer and the specific document or transaction.

Verification: The recipient uses the signer’s public key to decrypt the digital signature, recovering the hash. They then hash the original document themselves and compare it to the decrypted hash. If the two match, the signature is valid, confirming both authenticity and integrity.

# RANDOM AND PSEUDO-RANDOM-SEQUENCE GENERATION
In essence, a computer, as a finite-state machine, has a limited number of possible states and operates deterministically—its output is entirely defined by its inputs and current state. This means that any random-number generator on a computer will eventually repeat itself (periodicity), which makes it predictable over time. Since predictability contradicts the idea of true randomness, a computer alone cannot generate genuinely random numbers. True randomness requires input from a truly random, external source (such as physical noise), which a computer cannot internally produce. Thus, without an external random input, computer-generated "random" numbers are inherently pseudo-random, not truly random.
Cryptographically Secure Pseudo-Random Sequences
For a sequence to be cryptographically secure pseudo-random, it must be be computationally infeasible to predict what the next random bit will be, given complete knowledge of the algorithm or hardware generating the sequence and all of the previous bits in the stream.

a) Pubkey today.
WhatsApp's end-to-end encryption (E2EE) protects messages, media, and group chats by using a cryptographic system to secure data in transit.
Asymmetric cryptography: Each user generates a public-private key pair. The public key encrypts messages, and the private key decrypts them
Source : https://www.businesstoday.in/latest/story/how-does-whatsapp-end-to-end-encryption-work-156881-2019-01-08
![image](https://github.com/user-attachments/assets/8e7c709a-8821-4325-8b3e-6f6679b63ecf) and CHAT GPT for answer rewrite

b) Messaging using PGP
Key generation ![image](https://github.com/user-attachments/assets/68e75f05-af6d-400d-b0aa-cd9edf3c272b)

<img width="649" alt="Screenshot 2024-11-06 at 5 17 40" src="https://github.com/user-attachments/assets/7db41ddd-0a2e-4788-979a-f2ddf7fe3c6d">
alice key
<img width="542" alt="Screenshot 2024-11-06 at 5 20 24" src="https://github.com/user-attachments/assets/256cee35-f8d4-4da0-98ac-00dfb36f878c">
key imported in alice folder
<img width="721" alt="Screenshot 2024-11-06 at 5 22 02" src="https://github.com/user-attachments/assets/521b3a1b-598d-42d1-ab18-0dc890484f46">
After signing the deepaks key
<img width="681" alt="Screenshot 2024-11-06 at 5 26 04" src="https://github.com/user-attachments/assets/955de3e6-e527-4332-8784-311c2ba3026f">
Finger print for deepak shows alice as unknwon we wil sign in the next step
<img width="568" alt="Screenshot 2024-11-06 at 5 51 42" src="https://github.com/user-attachments/assets/83844f21-8e99-4065-b348-bbc56762b121">
After signing full trust is established between both parties
<img width="578" alt="Screenshot 2024-11-06 at 5 52 44" src="https://github.com/user-attachments/assets/3aadd0c0-2462-414d-934c-21924051281a">

Message encrypted using private key of alice
<img width="708" alt="Screenshot 2024-11-06 at 5 58 39" src="https://github.com/user-attachments/assets/c60ac9ba-4b77-407c-bc3a-4878cfd3d1b3">
<img width="601" alt="Screenshot 2024-11-06 at 5 59 24" src="https://github.com/user-attachments/assets/998b108b-7b99-497b-9828-3cc96fb4a599">

Receiver decrypts the message
<img width="701" alt="Screenshot 2024-11-06 at 6 00 48" src="https://github.com/user-attachments/assets/5914426f-5857-41ea-a830-51e2af53d454">

source :https://terokarvinen.com/2023/pgp-encrypt-sign-verify/

C)
opmsg operates as a lightweight encryption and signing tool designed for simplicity, modern cryptography, and secure message exchange without the extensive key management features typical of tools like gpg. Here’s a breakdown of how opmsg works:

opmsg focuses on using temporary or session-based keys, rather than managing a long-term keyring.
Each message is typically encrypted and signed with ephemeral (temporary) keys, which can be derived from a passphrase or password. This reduces the risk associated with long-term key storage.
opmsg leverages elliptic-curve cryptography (ECC), specifically curve25519, which is known for its strong security and efficiency.
By using modern encryption standards, opmsg can achieve secure encryption and signing without the overhead of more complex and older protocols.
The sender uses opmsg to encrypt a message, potentially supplying a passphrase or password to derive the key.
opmsg then:
Encrypts the message content.
Signs the message with a derived ephemeral key.
Combines the encrypted content and signature into a single self-contained file.
The resulting encrypted message can then be sent to the recipient.
Decrypting and Verifying a Message:
The recipient receives the encrypted file and uses opmsg to decrypt and verify it.
By supplying the correct passphrase or password, the recipient can:
Decrypt the content to retrieve the original message.
Verify the signature to ensure the message's authenticity and integrity.

# encrypting a message
opmsg -e -r recipient_name -m "Your secret message here" -o encrypted_message.opmsg
-e tells opmsg to encrypt the message.
-r recipient_name specifies the intended recipient.
-m "Your secret message here" is the plaintext message to encrypt.
-o encrypted_message.opmsg specifies the output file.

# decrypting a message 
opmsg -d -i encrypted_message.opmsg -o decrypted_message.txt
-d indicates decryption.
-i encrypted_message.opmsg is the encrypted message file to decrypt.
-o decrypted_message.txt is the file to save the decrypted content.



d) # Explain PGP
PGP (Pretty Good Privacy) and GPG (GNU Privacy Guard) are encryption tools widely used to protect the privacy and integrity of data, particularly for email communication. They use a combination of cryptographic techniques to prevent eavesdropping (interception by unauthorized parties) and malicious modification (tampering).
# Encryption to Prevent Eavesdropping
PGP and GPG use asymmetric encryption, which means that each user has a pair of keys: a public key (shared with others) and a private key (kept secret).When someone wants to send an encrypted message, they encrypt it using the recipient's public key. Only the recipient's private key can decrypt this message. This ensures that if an attacker intercepts the message, they cannot read it because they don’t have the private key.PGP and GPG actually combine asymmetric and symmetric encryption. First, they create a random session key to encrypt the message with faster symmetric encryption (e.g., AES). Then, this session key is encrypted with the recipient's public key. This encrypted session key and encrypted message are both sent to the recipient. Upon receiving, the recipient uses their private key to decrypt the session key, and then uses it to decrypt the message itself.
This method prevents eavesdropping because even if an attacker intercepts the message, they lack the private key required to decrypt the session key, which is necessary to access the actual message.
# Digital Signatures to Prevent Malicious Modification
To ensure that a message has not been altered, PGP and GPG use digital signatures. The sender creates a hash of the message (a unique "fingerprint" generated by a hashing algorithm like SHA-256) and then encrypts this hash with their private key to create a digital signature.
The recipient can use the sender's public key to decrypt the digital signature and retrieve the original hash. Then, they hash the received message on their end and compare it to the hash retrieved from the digital signature. If they match, it means the message has not been modified.
Since only the sender’s public key can decrypt a signature created with their private key, this also verifies the sender’s identity. If an attacker attempted to tamper with the message and re-sign it, they would not be able to create a valid signature without the sender’s private key.


The  flags that make this happens are  --encrypt Encrypt the message --sign signs the message using sender private key --output encrypted.pgp  saves the encrypted content to the file, receiver decrypt the message usng gpg --decrypt encrypted.pgp  and sender public key do decrypt the hash of signature for sender verification. 

Sources :https://terokarvinen.com/2023/pgp-encrypt-sign-verify/  and CHAT GPT for answer rewrite

F) Password management
I use lastpass for my password management It allows for quick search and password generation easily and this is available in all devices mac windows mobile ios and android. 
Features includes 
<img width="642" alt="image" src="https://github.com/user-attachments/assets/e184624e-5761-4e14-a97a-ef1976a9c648">

<img width="377" alt="image" src="https://github.com/user-attachments/assets/83e39781-5f65-404d-8db8-99fc4232426b">

For individuals who don’t use password managers, several types of security vulnerabilities and attacks become more likely. Password managers help create, store, and manage strong and unique passwords, which makes accounts more resistant to various attacks. Without a password manager, users are more vulnerable to the following types of attacks:
*  Password Reuse Attacks
*  Phishing Attacks
*  Weak Passwords and Brute-Force Attacks
*  Dictionary Attacks
*  Social Engineering Attacks
*  Keystroke Logging (Keylogging)
*  Shoulder Surfing and Visual Hacking
*  Account Recovery Exploits
* Password Reset Link Exploits
* Data Breach Exposure
Sources: google.com and lastpass and CHAT GPT for answer rewrite


g)  Sources are added after each answer 






