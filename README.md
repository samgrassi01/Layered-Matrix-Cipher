# Layered-Matrix-Cipher

This is a symmetric encryption scheme that uses rectangular matrices and non-linear functions to build a homomorphic 
cipher, resistant to know-plaintext attacks.

A few months ago, I was introduced into the realm of cryptography when, thinking about some math concepts, I realized it
would be possible to encode a message or data into vector form, and then encrypt it with a randomely initialized nonsingular
matrix.  After programming this idea out, I discovered it worked.  Intrigued, I decided to spend some time learning about 
cryptography, which ultimately led to the development of my "Mathematics of Cryptography" tutorial repository.  

After playing with the cipher I cam up with more, and the more I learned about cryptography, the more excited about the cipher
I became.  For example I discovered the cipher is a homomorphic encryption cipher.  However, through reading a blog post on
[safe AI](https://iamtrask.github.io/2017/03/17/safe-ai/), I discovered the paper "[Efficient Integer Vector Homomorphic 
Encryption](https://courses.csail.mit.edu/6.857/2015/files/yu-lai-payor.pdf)" by Yu Et al.  After reading the paper and looking at the code, I discovered that the cipher I came up with was very 
similar to the base idea of the cipher posited in the paper (the paper implemented a few beautiful ideas such as key-switching
I did not come up with).  However after reading the paper following up on the Efficient Integer Vector Homomorphic Encryption 
scheme titled "[Cryptanalysis of a Homomorphic Encryption Scheme](https://eprint.iacr.org/2016/775.pdf)" by Bogos Et al, I began to understand the deeper flaws of this
cipher.  

The cipher I implement in this repository implements a couple improvements to the Efficient Integer Vector Homomorphic Encryption
scheme, specifically with respect to the original ciphers suseptability to known plaintext attacks.

Homomorphic encryption (HE) is an incredibly important, newer form of encryption that I hope will become ubiquitous in the world.
HE's applications range from health care to safe AI.  Expand on this point furthur.
