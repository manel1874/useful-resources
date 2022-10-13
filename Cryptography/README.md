# Cryptography

--------
## Table of Contents

* [Core Textbooks](#core-textbooks)
* [Text Tutorials](#text-tutorials)
	* [Privacy Enhancing Technologies](#privacy-enhancing-technologies)
	* [Crypto tools](#crypto-tools)
	* [Simulation proof](#simulation-proof)
* [Post-quantum](#post-quantum)
	* [Textbooks](#textbooks)
	* [Review Articles](#review-articles)
* [Advanced topics](#advanced-topics)
	* [Elliptic Curves](#elliptic-curves)
		* [Textbooks](#textbooks)
	* [Physically unclonable functions](#physically-unclonable-functions)
	* [Oblivious Transfer](#oblivious-transfer)
	* [Secure multiparty computation](#secure-multiparty-computation)
	* [Homomorphic encryption](#homomorphic-encryption)
## Core Textbooks

- Cryptography: Theory and practice, Douglas R. Stinson. 
Covers all basic crypto concepts. Block ciphers (AES), Hash functions, RSA, attacjs to RSA, PKC and DLog, DLog attacks, Signature Schemes, (P)RNG, Key Distribution, Key Agreement Schemes, PKI, Secret Sharing and Access Structures

- Applied Cryptography, Alfred J. Menezes, Paul C. van Oorschot, Scott A. Vanstone.
Interesting chapters: Number-Theoretic Reference Problems, Hash functions and data integrity, Digital Signatures, Efficient Algorithms of basic multi-precision operations.

- Foundations of Cryptography I, Oded Goldreich. 
Computational complexity approach: One-way functions, Hard-Core Predicates, Zero-knowledge Proof Systems

- Foundations of Cryptography II, Oded Goldreich. 
Digital Signatures and MAC, Two party protocols, NIZKs


## Text Tutorials

### Privacy Enhancing Technologies

- Garbled Circuits as Randomized Encodings of Functions: a Primer, Applebaum
- Homomorphic Encryption, Halevi
- The Complexity of Differential Privacy

### Crypto tools

- The Complexity of Public-Key Cryptography, Barak
- Pseudorandom Functions: Three Decades Later, Bogdanov and Rose

### Simulation proof

- How to Simulate It - A Tutorial on the Simulation Proof Technique, Lindell
- Universal Composability Framework, Canetti


## Post-quantum

### Textbooks

- Post-Quantum Cryptography, Bernstein, Buchmann, Dahmen, Springer (2008)
Comparison to quantum cryptography, Hash-based Digital Signature Schemes, Code-based cryptography, Lattice-based Cryptography, Multivariate PKCs

### Review Articles

- Post-quantum cryptography ? dealing with the fallout of physics success, Bernstein, Lange, 2017

## Advanced topics

### Elliptic Curves

#### Textbooks

- Algebraic Aspects of Cryptography, Koblitz, 1997
A book about Elliptic and Hyperelliptic Cryptosystems. Includes ECDSA

### Physically unclonable functions

- Physically Unclonable Functions: Constructions, Properties and Applications, Roel Maes, 2013, Springer

### Oblivious Transfer

- Non-interactive oblivious transfer, Bellare, Micali, 1989
- Efficient Oblivious Transfer Protocols, Naor, Pinkas
- The Simplest Protocol for Oblivious Transfer, Chou, Orlandi
- Extending Oblivious Transfer Efficiently, Ishai, Kilian, Nissim, Petrank


### Secure multiparty computation

#### Textbooks

- A Pragmatic Introduction to Secure Multi-Party Computation, Evans, Kolesnikov, Rosulek, 2018

#### Tutorials

- [Youtube] [Introduction to Computing on Encrypted Data](https://www.youtube.com/watch?v=_nO2S2cexAk&list=PLiHaXFHjrqYfGA2ltpQH7_pVGTp9cACMn&index=2), Nigel Smart, KU Leuven, 2021
- [Slides] [2PC course](https://web.engr.oregonstate.edu/~rosulekm/), Mike Rosulek, 2018, Bonn Summer School

#### Implementations

- [Awesome MPC frameworks](https://github.com/rdragos/awesome-mpc/blob/master/readme.md)

#### Post-quantum security

- [Post-Quantum Multi-Party Computations](https://arxiv.org/pdf/2005.12904.pdf), Agarwal, et al. 

Techniques used in this paper: 

Quantum Multi-Key Fully-Homomorphic Encryption; Quantum-Secure Multi-Committer Extractable Commitment; Quantum-Secure Multi-Verifier Zero-Knowledge; Quantum-Secure Non-Malleable Commitments

Interesting element: An explicit quantum attack against a classically-secure ZK protocol


#### Secure quantum multiparty computation

- [Quantum Garbled Circuits](https://arxiv.org/pdf/2006.01085.pdf), Brakerski, Yuen, 2020



### Homomorphic Encryption

#### Tutorials

- [Medium] [Homomorphic Encryption for beginners: a practical guide I](https://medium.com/privacy-preserving-natural-language-processing/homomorphic-encryption-for-beginners-a-practical-guide-part-1-b8f26d03a98a)
- [Medium] [Homomorphic Encryption for beginners: a practical guide II](https://medium.com/privacy-preserving-natural-language-processing/homomorphic-encryption-for-beginners-a-practical-guide-part-2-the-fourier-transform-77bcaf9a1756)

#### Overview papers

- [Fully homomorphic encryption for mathematicians](https://eprint.iacr.org/2013/250.pdf), Silverberg. About [Craig Gentry](https://crypto.stanford.edu/craig/craig-thesis.pdf) approach. Inefficient in practice but with a conceptual breakthrough.
- https://eprint.iacr.org/2015/1192.pdf

#### Lecture notes

- [Shafi Goldwasser notes](https://www.cs.bu.edu/~reyzin/teaching/s11cs937/notes-shafi-1.pdf) on chapter 3.
- https://crypto.stanford.edu/craig/craig-thesis.pdf Introduction (1.1)

### Application
- https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5930176/ (Secure Logistic Regression Based on Homomorphic Encryption




