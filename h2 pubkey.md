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

