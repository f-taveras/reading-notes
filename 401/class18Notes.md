<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>

## What is the basic principle behind the Caesar Cipher, and how was it used historically?
The Caesar Cipher is a simple substitution cipher where each letter in the plaintext is shifted a certain number of places down or up the alphabet.

__For example__, with a shift of 3, __'A'__ would be replaced by __'D'__, __'B'__ would become __'E'__, and so on.

It was named after Julius Caesar, who reportedly used it to communicate with his generals.
The Caesar Cipher provided a basic level of security by obscuring the contents of messages. Its simplicity, however, made it easy to crack, even in ancient times.

## What are the key differences between symmetric and asymmetric encryption? How is asymmetric used in secure communication today?

### Symmetric Encryption

* __Key:__ Uses the same key for encryption and decryption.
* __Speed:__ Generally faster than asymmetric encryption.
* __Use Case:__ Ideal for encrypting large volumes of data, like files or database information.
* __Example:__ AES (Advanced Encryption Standard).

### Asymmetric Encryption

* __Key:__ Uses a pair of keys – a public key for encryption and a private key for decryption.
* __Speed:__ Slower due to complex mathematical operations.
* __Use Case__: Commonly used for secure key exchange, digital signatures, and encrypting small pieces of data like passwords.
* __Example:__ RSA (Rivest–Shamir–Adleman).

### Usage in Secure Communication Today

Asymmetric encryption is widely used for secure communications over the internet, such as in HTTPS, email encryption, and secure file transfer protocols.
It's also crucial for establishing secure connections (like in SSL/TLS) where symmetric keys are exchanged securely using asymmetric methods.

## How do computers generate random numbers, and what are the differences between true random number generation (TRNG) and pseudo-random number generation (PRNG)? Discuss their use cases in cryptography.

True Random Number Generation (TRNG)

* __Principle:__ Uses physical phenomena (like electronic noise) to generate numbers.
* __Characteristics:__ Truly random and unpredictable.
* __Use Case__: Used in high-security cryptographic applications where unpredictability is critical, such as generating keys for encryption.

Pseudo-Random Number Generation (PRNG)

* __Principle:__ Uses algorithms to generate sequences of numbers that only appear random.
* __Characteristics:__ Deterministic and repeatable if the initial seed value is known.
* __Use Case__: Commonly used in applications where a high volume of random numbers is required quickly, like simulations, but not suitable for high-security encryption key generation.
## What’s the difference between encryption and decryption? Explain with an analogy.

### Encryption

Imagine locking a valuable item in a safe. The __'item'__ is your data, and the __'safe'__ is the encryption algorithm. The key to the safe is the encryption key, which secures the data so that only authorized individuals can access it.

### Decryption

Imagine unlocking the safe to retrieve the valuable item. Here, the correct key __(decryption key)__ is used to unlock __(decrypt)__ the data, returning it to its original, readable form.

<sub>Information modeled using ChatGPT</sub>