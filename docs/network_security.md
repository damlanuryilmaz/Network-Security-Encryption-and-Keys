# Network Security Encryption and Keys

## Meaning of Network Security 

[1]Despite being a crucial component of network security policy, the art and science of cryptography and its function in ensuring secrecy, integrity, and authentication constitute a separate emphasis because network security is such a broad issue. The Internet Protocol (IP) is the network-layer protocol used by the great majority of network traffic today.

## Network intrusions 

[1]Millions of packets per second are sent and received between hosts via routers in network traffic. And it means big data and it needs a secure layers and protocols to protect the data or not cause any data.

There are some types of intrusion, they are briefly:

* The Land Attack: It is the simplest attack. The computer sending endless messages to itself, unable to stop so, it tricks a computer into overloading itself, making it unavailable to everyone.

* The Smurf Attack: It creates a fake traffic, and it overwhelms the victim computer with so much fake traffic that it can't handle real requests.

*	The Teardrop Attack: An attacker sends specially crafted packets that exploit vulnerabilities in the way a computer reassembles incoming data. This can cause the target computer to crash or become unresponsive.

Another type of attacks are DDoS attacks. DDoS meaning is distributed denial-of-service attack, and it overwhelms a targeted server, service, or network with internet traffic, like a malicious digital flood. The targeted system cannot be accessed by genuine users due to a flood of traffic. It causes a big chaos. Also, it is by issuing commands to “attack zombie” computer programs. It creates a target computer and hackers can leverage the target computer. And this makes identifying such attacks extremely difficult. 

## Key Terms for Network Security 

[2]Plaintext or Cleartext: Unencrypted data. It's vulnerable to eavesdropping and should be encrypted for sensitive information. It needs to be protected. Examples include login credentials and online purchases.

Ciphertext: Unreadable data created by encrypting plaintext. It requires a decryption key to be read. This protects sensitive information and ensures confidentiality. Examples include HTTPS websites and encrypted emails.

Key: A parameter of the encryption algorithm. They are like secret codes in network security, locking your online data and ensuring only authorized users access it.

Encipher (encrypt): It converts readable data to unreadable code, protecting it from unauthorized access. This is important for secure online activities like transactions and communication.

Decipher (decrypt): It unlocks encrypted data, restoring it to readable form for secure communication, data access, digital signatures, and malware detection. And transform ciphertext to plaintext.

Symmetric key algorithms: It uses a single, shared key for both encryption and decryption. This makes them fast and efficient, ideal for large data. It also known secret-key, single-key, or one-key algorithm.

Asymmetric key algorithms: It also known as public-key cryptography, use a pair of keys: a public key and a private key. This provides stronger security than symmetric key algorithms. These keys are related keys and using one key to decrypt and other key to encrypt. A user will make his encryption key, denoted as the public key, known, but the decryption key is not disclosed. The decryption key is often called the private or secret key.

Digital Signature: It is like an electronic seal of approval, ensuring a document is authentic and untampered with. It uses encryption and unique codes to verify the sender and prevent modifications. This technology is crucial for secure online activities like e-commerce, e-government, and email.

These are used for attacks and unwanted attempts to data to protect it. Because it is important to use a high-level key-pair and cryptography to protect our data. 

Simplified example of Public Key Cryptography: 

First, the original message passed through a cryptographic one-way hash function. It makes is encrypted and even though original message is long, now it is a small function with a private key of the sender. And the sender is responsible for this key. 

And this encrypted hash value acts like a digital signature. Digital signature added to the original message to form the message to be transmitted. Now, entire message to be transmitted is first encrypted with the public key of the receiver. Over an untrusted network, the message is delivered to the receiver. With receiver’s private key, the message is decrypted. A message that is encrypted with Alice's public key can only be decrypted by those who have her private key. This is what public-key cryptography is all about. Alice oversees keeping her private key secure.

The received message should be composed of the original message and the digital signature. The same cryptographic one-way hash algorithm used by the sender is applied to the original message portion of the received message. Now the digital signature is decrypted with sender’s public key. 

Receiver can check if the messages are same or not so they can understand it is sent from the original sender or not. Digital signature provides some assurance that the sender is who they claims to be, and that integrity of the message has been verified. And if the key is secure, parties can use this key to communicate in the future securely. This allows symmetric encryption. Now, the communication is completed. 

## Encryption Algorithms 

[2]There is a mathematical explanation of the encryption with function:

1.	Conventional Encryption:

E = F (D, K)

where,
D is data to be encoded
K is key variable
E is the resulting enciphered text
F is the function (F’ needs to be exist)

D = F’ (E, K)

It needs to be existed because it needs to be decrypted. 

2.	Public – Key Encryption:

E = F (D, K)

D = F’ (E, K’)

Difference is between conventional encryption and public-key encryption is K and K’. Because in public-key encryption we need to a pair of keys to encrypt this data.

## Firewalls 

[3]Firewalls enforce an access policy by operating as a gateway between to networks. Firewalls are defined as a collection of components placed between two networks that collectively have the following properties, but of course these are goals not the facts:[4]

*	All traffic from inside to outside and vice versa, must pass through the firewall.
*	Only authorized traffic, as defined by the local security policy, will be allowed to pass.
*	The firewall itself is immune to penetration.

There are two major classes:

[3]Packet Filter Firewalls: These are gatekeepers of network security. They are inspecting and controlling incoming and outgoing traffic based on pre-defined rules. They are simple, efficient, and cost-effective, but offer limited security compared to other solutions. They examine the packet and decide whether it can pass or not.

Proxy Firewalls: They go beyond simple packet filtering, inspecting traffic at the application level for enhanced security. They can block threats, control application access, enforce policies, and anonymize your network. But be aware of performance impact, configuration complexity, and potential single point of failure. They examine the data within the flow, then re-create the flow in the network at the other side of the firewall.

## Conclusion
Network security acts as our shield in the ever-evolving digital landscape. Firewalls, like gatekeepers, control and filter traffic, while keys unlock encrypted data, ensuring its confidentiality. Encryption safeguards our sensitive information, and digital signatures verify the authenticity of messages and documents. By investing in network security, we protect our digital infrastructure, fostering innovation, building trust, and securing a brighter future.


## References
[1]  G. A. Marin, "Network security basics," in IEEE Security & Privacy, vol. 3, no. 6, pp. 68-72, Nov.-Dec. 2005, doi: 10.1109/MSP.2005.153.

[2]  P. W. Dowd and J. T. McHenry, "Network security: it's time to take it seriously," in Computer, vol. 31, no. 9, pp. 24-28, Sept. 1998, doi: 10.1109/2.708446.

[3]  Popek, Gerald J., and Charles S. Kline. "Encryption and secure computer networks." ACM Computing Surveys (CSUR) 11.4 (1979): 331-356.

[4]  S. M. Bellovin and W. R. Cheswick, "Network firewalls," in IEEE Communications Magazine, vol. 32, no. 9, pp. 50-57, Sept. 1994, doi: 10.1109/35.312843.

