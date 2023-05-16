## Cryptography

#### Things I Want to Know More About


### Encryptions, Decryption and Hacking

1. What is the basic principle behind the Caesar Cipher, and how was it used historically?

shift by 6 letters, rewrite using the same letters. Allowed encrypted messages to be sent confidentially. 

Just think of the level of paranoia considering a hypothetical literacy rate of 15%. 

### Ceasar Cipher

YHWH 

Limited number of shifts

### Cryptography Crash Course

Defensive depth--like a castle 

First more complex crypto, created by IBM, but cracked in 2 days as computing power increased.

AES--uses much bigger bit keys, 128 bit key would take trillions of years to be broken by brute force. 

Use keys now by key exchange. One way functions. Cool paint analogy. 


### Intro to Cryptography

2. What are the key differences between symmetric and asymmetric encryption? How is asymmetric used in secure communication today?  

Diffie Hellman key enchange, keys sent by both sender and receiver are called symmetric keys becuase the key is the same on both sides. You create a key, mixed with the public key, send that to the other side, then they send their key mixed with the public key to you, and you can each mix the key again on your side to make the same key. 

Asymmetric, is two different keys, public keys and private keys, can send the lock box, and you are the only one with a key that can open it. `https://`

4 types of cryptographic functions:
1. authentication
2. nonrepudiation--irrefutable transactions
3. confidentiality
4. integrity--data is not viewed or altered during transmission

https everywhere extension

### How Computers Generate Random Numbers

3. How do computers generate random numbers, and what are the differences between true random number generation (TRNG) and pseudo-random number generation (PRNG)? Discuss their use cases in cryptography.

To generate a “true” random number, the computer measures some type of physical phenomenon that takes place outside of the computer. 

Pseudorandom numbers are an alternative to “true” random numbers. A computer could use a seed value and an algorithm to generate numbers that appear to be random, but that are in fact predictable. The computer doesn’t gather any random data from the environment.

If an attacker can guess your algorithm, they might be able to guess the pseduo-random number and hack your data

4. What’s the difference between encryption and decryption? Explain with an analogy.

You protect your plaintext message and then send it in ciphertext, to read the ciphertext message, you must de-code it using a key. For the Ceasar cypher, the person who gets the message would know about the 3 letter shift. 