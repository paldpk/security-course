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

A. How i used public key

