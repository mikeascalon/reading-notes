# Reading Notes

What is the basic principle behind the Caesar Cipher, and how was it used historically?

The Caesar Cipher is one of the simplest and oldest encryption techniques in cryptography, named after Julius Caesar, who is believed to have used it to protect sensitive information. The basic principle behind the Caesar Cipher is a substitution cipher, where each letter in the plaintext is shifted a fixed number of positions down or up the alphabet. This shift is known as the "key" or "shift value."

What are the key differences between symmetric and asymmetric encryption? How is asymmetric used in secure communication today?

* **Symmetric Encryption:** In symmetric encryption, the same key is used for both encryption and decryption. This means that both the sender and receiver must have access to the same secret key, making key distribution and management critical. Common symmetric encryption algorithms include AES (Advanced Encryption Standard) and DES (Data Encryption Standard).

* **Asymmetric Encryption:** Asymmetric encryption, also known as public-key encryption, uses a pair of keys: a public key and a private key. The public key is used for encryption, while the private key is used for decryption. This eliminates the need for both parties to share a secret key, making key distribution easier and more secure. Common asymmetric encryption algorithms include RSA and ECC (Elliptic Curve Cryptography).

How do computers generate random numbers, and what are the differences between true random number generation (TRNG) and pseudo-random number generation (PRNG)? Discuss their use cases in cryptography.

**Random Numbers in Computing:**

* Random numbers play a crucial role in various computer applications, including cryptography, gambling, video games, and more.
  
* Randomness is essential in cryptography to ensure the security of encryption algorithms, as cryptographic keys must be unpredictable to resist attacks.

**True Random Numbers (TRNG):**

* TRNGs generate truly random numbers by measuring unpredictable physical phenomena or environmental factors, such as radioactive decay, atmospheric noise, or user keyboard input timings.
  
* These sources of entropy are considered unpredictable, making TRNGs a valuable source of true randomness for cryptographic applications.
  
* The article mentions the /dev/random device on Linux, which is an example of a TRNG that "blocks" until it gathers enough entropy to provide a truly random number.

**Pseudo-Random Numbers (PRNG):**

* PRNGs generate numbers that appear random but are generated using deterministic algorithms and an initial seed value.
PRNGs are not truly random, and if an attacker knows the algorithm and seed value, they can predict the generated numbers.
While PRNGs are suitable for many applications, such as video games, they are not ideal for cryptographic purposes where true unpredictability is crucial.

What’s the difference between encryption and decryption? Explain with an analogy.

* *Encryption* is like putting a letter in a locked box before sending it through the mail. Imagine you have a sensitive letter that you want to send to a friend. 

* *Decryption* is the process your friend uses to read the letter. When your friend receives the locked box, they use their key to unlock it and read the letter inside. 


## Resources

[Encryption, decryption, and cracking](https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:online-data-security/xcae6f4a7ff015e7d:data-encryption-techniques/a/encryption-decryption-and-code-cracking)

[Caesar cipher](https://en.wikipedia.org/wiki/Caesar_cipher)

[How Computers Generate Random Numbers](https://www.howtogeek.com/183051/htg-explains-how-computers-generate-random-numbers/)

[ChatGPT](https://chat.openai.com/)