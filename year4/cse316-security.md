# CSE316 Computer Systems Security

**Note: I found the course material for 19/20 is copied from [an online course](www.coursera.org/learn/cryptography) so if you are interested and want to learn better, you should check it**

## Lecture 1

Some import definitions: 

* Security
* Protection
* Vulnerabilities
* Exploits
* Trust

Security Goals:

* Confidentiality < ---related to--- > Interception Threat
* Intergrity  < ---related to--- >  Modification Threat, Fabriction Threat
* Avilability < ---related to--- > Interruption Threat

Threats:

* Theft
* Privacy
* Destruction
* Interruption or interference with computer-controlled services


Design principles for secure systems:

* Economy
* Complete mediation
* Open design
    * Kerckhoff principle: A cryptographic system should be secure even if everything about the system, except the key, is public knowledge.
* Separation of privileges
* Least privilege
* Least common mechanism
* Acceptability
* Fail-safe defaults

Tools for security:

* Access control
* Encryption
* Authentication
* Intrusion detection
* Common sense


## Lecture 2 Classical and Modern Cryptography

1. Classical Cryptography:

* Private-key encryption
    * secure communication
    * secure storage
* The shift cipher
* Modular arithmetic
* The Vigenere cipher

Sufficient key space principle:
* The key space should be large enough to prevent "brute-force" exhausticve-search attacks


2. Modern Cryptography:

* Crypto definitions:
    * Threat Model
    * Security guarantee/goal
* Assumptions
* Proofs of security

3. Perfect secrecy:

The goal for security encryption is "impossible for the attacker to learn the key" -> "Regardless of any prior information the attacker has about the plaintext, the ciphertext should leak no additional information about the plaintext"


* Ciphertext-only attack
* Known-plaintext attack
* Chosen-plaintext attack
* Chosen-ciphertext attack

* Attacker’s information about the plaintext = attacker known distribution of the plaintext
* Perfect secrecy means that observing the ciphertext should not change the attacker’s knowledge about the distribution of the plaintext.

4. One-time pad

5. Computational secrecy
