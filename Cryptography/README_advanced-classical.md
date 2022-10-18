# Advanced classical cryptography

## Table of Contents


* [Elliptic Curves](#elliptic-curves)
	* [Textbooks](#textbooks)
* [Secure multiparty computation](#secure-multiparty-computation)
	* [Textbooks](#textbooks)
	* [Tutorials](#tutorials)
	* [Implementations](#implementations)
	* [2PC protocols](#2pc-protocols)
	* [Post-quantum security](#post-quantum-security)
	* [Secure quantum multiparty computation](#secure-quantum-multiparty-computation)
	* [Applications](#applications)
	* [Blockchain hybrid model](#blockchain-hybrid-model)
* [Homomorphic encryption](#homomorphic-encryption)
* [Physically unclonable functions](#physically-unclonable-functions)
* [Oblivious Transfer](#oblivious-transfer)
	* [Main protocols](#main-protocols)
	* [Bounded classical storage model](#bounded-classical-storage-model)
	* [Combiners](#combiners)
	* [Extractors](#extractors)
* [Leakage Resistant Secret Sharing](#leakage-resistant-secret-sharing)

--------

## Elliptic Curves

### Textbooks

- Algebraic Aspects of Cryptography, Koblitz, 1997
A book about Elliptic and Hyperelliptic Cryptosystems. Includes ECDSA


## Secure multiparty computation

### Textbooks

- A Pragmatic Introduction to Secure Multi-Party Computation, Evans, Kolesnikov, Rosulek, 2018

### Tutorials

- [Youtube] [Introduction to Computing on Encrypted Data](https://www.youtube.com/watch?v=_nO2S2cexAk&list=PLiHaXFHjrqYfGA2ltpQH7_pVGTp9cACMn&index=2), Nigel Smart, KU Leuven, 2021
- [Slides] [2PC course](https://web.engr.oregonstate.edu/~rosulekm/), Mike Rosulek, 2018, Bonn Summer School

### Implementations

- [Awesome MPC frameworks](https://github.com/rdragos/awesome-mpc/blob/master/readme.md)

### 2PC protocols

- [Authenticated Garbling and Efficient Maliciously Secure Two-Party Computation](https://eprint.iacr.org/2017/030.pdf)

Evaluates AES circuit with malicious security in 37 ms with an online time of just 1 ms


### Post-quantum security

- [Post-Quantum Multi-Party Computations](https://arxiv.org/pdf/2005.12904.pdf), Agarwal, et al. 

Techniques used in this paper: 

Quantum Multi-Key Fully-Homomorphic Encryption; Quantum-Secure Multi-Committer Extractable Commitment; Quantum-Secure Multi-Verifier Zero-Knowledge; Quantum-Secure Non-Malleable Commitments

Interesting element: An explicit quantum attack against a classically-secure ZK protocol


### Secure quantum multiparty computation

- [Quantum Garbled Circuits](https://arxiv.org/pdf/2006.01085.pdf), Brakerski, Yuen, 2020

### Applications

- Millionaires Problem

- Secure auctions. Use bid privacy and bid non-malleability

- Secure voting 

- Biometric data:
  - Efficient Privacy-Preserving Biometric Identification
  - Privacy-Preserving Fingercode Authentication

- Private Set Intersection:
  - Efficient Private Matching and Set Intersection
  - Faster Private Set Intersection based on OT Extension
  - Private Set Intersection: Are Garbled Circuits Better than Custom Protocols?

- ID3 Algorithm
  - Privacy Preserving Data Mining by Lindell&Pinkas ID3 Decision Tree Algo
  - Privacy-Preserving Collaborative Prediction using Random Forests
  - Privacy-Preserving Decision Trees over Vertically Partitioned Data

- k-Nearest
  - Efficient Privacy-Preserving k-Nearest Neighbor Search
  - Privacy Preserving K-nearest Neighbor Classification
  - Private Nearest Neighbors Classification in Federated Databases

- Neural Networks:
  - Garbled Neural Networks are Practical
  - QUOTIENT: Two-Party Secure Neural Network Training and Prediction

- Regression:
  - Privacy-Preserving Ridge Regression on Hundreds of Millions of Records
  - Privacy preserving linear regression modelling of distributed databases
  - Scalability of Privacy-Preserving Linear Regression in Epidemiological Studies
  - Privacy-Preserving Distributed Linear Regression on High-Dimensional Data

- Association Rules:
  - Application of Distributed Oblivious Transfer Protocol in Association Rule Mining
  - Privacy-preserving distributed mining of association rules using Elliptic-curve cryptosystem and Shamir?s secret sharing scheme

- Collision of moving objects
  -  Privacy-preserving collision detection of moving objects

### Blockchain hybrid model

Main researcher: [Vipul Goyal](https://dblp.org/pid/38/303.html)

- [Blockchains Enable Non-Interactive MPC](https://eprint.iacr.org/2021/1233.pdf)
- [Founding Secure Computation on Blockchains](https://link.springer.com/chapter/10.1007/978-3-030-17656-3_13)

Implementations: [Nillion](https://apply.workable.com/nillion/)

## Homomorphic Encryption

### Tutorials

- [Medium] [Homomorphic Encryption for beginners: a practical guide I](https://medium.com/privacy-preserving-natural-language-processing/homomorphic-encryption-for-beginners-a-practical-guide-part-1-b8f26d03a98a)
- [Medium] [Homomorphic Encryption for beginners: a practical guide II](https://medium.com/privacy-preserving-natural-language-processing/homomorphic-encryption-for-beginners-a-practical-guide-part-2-the-fourier-transform-77bcaf9a1756)

### Overview papers

- [Fully homomorphic encryption for mathematicians](https://eprint.iacr.org/2013/250.pdf), Silverberg. About [Craig Gentry](https://crypto.stanford.edu/craig/craig-thesis.pdf) approach. Inefficient in practice but with a conceptual breakthrough.
- [A Guide to Fully Homomorphic Encryption](https://eprint.iacr.org/2015/1192.pdf). Important table (1) describing all possible approaches along with assumption models: DLWE, PLWE, RLWE, SVP, among others.

### Lecture notes

- [Shafi Goldwasser notes](https://www.cs.bu.edu/~reyzin/teaching/s11cs937/notes-shafi-1.pdf) on chapter 3.
- https://crypto.stanford.edu/craig/craig-thesis.pdf Introduction (1.1)

### Applications
- [Secure Logistic Regression Based on Homomorphic Encryption](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5930176/)


## Physically unclonable functions

- Physically Unclonable Functions: Constructions, Properties and Applications, Roel Maes, 2013, Springer

## Oblivious Transfer

## Main protocols

- Non-interactive oblivious transfer, Bellare, Micali, 1989
- Efficient Oblivious Transfer Protocols, Naor, Pinkas
- The Simplest Protocol for Oblivious Transfer, Chou, Orlandi
- Extending Oblivious Transfer Efficiently, Ishai, Kilian, Nissim, Petrank

### Bounded classical storage model

- [Oblivious transfer with a memory-bounded receiver](https://ieeexplore.ieee.org/document/743500)
- [Constant-Round Oblivious Transfer in the Bounded Storage Model](https://link.springer.com/article/10.1007/s00145-006-0438-1)

>- Tools: Set encodings; Interactive Hashing

### Combiners:
- [Error-Tolerant Combiners for Oblivious Primitives](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/38321.pdf)
- [Efficiently from Semi-honest to Malicious OT via OLFE](https://eprint.iacr.org/2009/428.pdf)

### Extractors:
- [Extracting Correlations](https://web.cs.ucla.edu/~rafail/PUBLIC/103.pdf)
- [Secure Computation from Leaky Correlated Randomness](https://www.cs.purdue.edu/homes/hmaji/papers/GuptaIsMaSa14.pdf)
- [Secure Computation based on Leaky Correlations: High Resilience Setting](https://www.cs.purdue.edu/homes/hmaji/papers/C:BloMajNgu17.pdf) 
- [Secure Computation using Leaky Correlations (Asymptotically Optimal Constructions)](https://eprint.iacr.org/2018/372.pdf) 

## Leakage Resistant Secret Sharing
- [Leakage-resilience of the Shamir Secret-sharing Scheme against Physical-bit Leakages](https://eprint.iacr.org/2021/186.pdf)
- [Leakage Resilient Secret Sharing and Applications](https://eprint.iacr.org/2018/1154.pdf)
- [On the Local Leakage Resilience of Linear Secret Sharing Schemes](https://eprint.iacr.org/2019/653.pdf) 
- [Bounded Collusion Protocols, Cylinder-Intersection Extractors and Leakage-Resilient Secret Sharing](https://eprint.iacr.org/2020/473.pdf)
- [Leakage-Resilient Secret Sharing in Non-Compartmentalized Models](https://drops.dagstuhl.de/opus/volltexte/2020/12112/pdf/LIPIcs-ITC-2020-7.pdf)
- [Continuously Non-Malleable Secret Sharing for General Access Structures](https://eprint.iacr.org/2019/602.pdf)
- [The Mother of All Leakages: How to Simulate Noisy Leakages via Bounded Leakage (Almost) for Free](https://eprint.iacr.org/2020/1246.pdf) 




