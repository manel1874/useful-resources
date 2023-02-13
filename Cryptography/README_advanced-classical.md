# Advanced classical cryptography

## Table of Contents


* [Elliptic Curves](#elliptic-curves)
	* [Textbooks](#textbooks)
* [Zero knowledge proofs](#zero-knowledge-proofs)
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
* [Differential Privacy](#differential-privacy)

* [Network Security](#network-security)

--------

## Elliptic Curves

### Textbooks

- Algebraic Aspects of Cryptography, Koblitz, 1997
A book about Elliptic and Hyperelliptic Cryptosystems. Includes ECDSA


## Zero knowledge proofs

- [ZK Jobs](https://github.com/ZeroKnowledgefm/ZKJobs)
- [Ingopedia zk](https://github.com/ingonyama-zk/ingopedia)
- [LinkTree zk](https://linktr.ee/zeroknowledge)

### Introductory papers

- [Why and How zk-SNARK Works: Definitive Explanation](https://arxiv.org/pdf/1906.07221.pdf)

### Original papers

- [The knowledge complexity of interactive proof system, original, GMR85](https://dl.acm.org/doi/pdf/10.1145/22145.22178)

- [The knowledge complexity of interactive proof systems, extension, GMR89](https://people.csail.mit.edu/silvio/Selected%20Scientific%20Papers/Proof%20Systems/The_Knowledge_Complexity_Of_Interactive_Proof_Systems.pdf):
>- Introduce the notion of interactive proof systems.
>- Ans: How much knowledge is transmitted to the verifier in an interactive proof system for L?
>- Def: An interactive proof system for L is zero-knowledge if for each x \in L, the prover tells the verifier essentially nothing, other than that x \in L.
>- Meaning of zk: one can compute in poly-time, from x \in L, without a prover, the same (or almost the same) probability distribution that the verifier would see with the prover.
>- Examples. Perfect zero-knowledge proof systems: all languages in BPP have; QR and QNR languages (not in BPP); graph isomorphism [GMW]. Statistically zero-knowledge proof systems: graph nonisomorphism [GMW]. Computationally zero-knowledge proofs (if secure encryption exists): all languages in NP. Zero-knowledge proofs: all languages in IP [BGGHKMR]

- [Non-interactive zero-knowledge and its applications](https://dl.acm.org/doi/10.1145/62212.62222)

### zkSNARKs

- [Marlin: Preprocessing zkSNARKs with Universal and Updatable SRS](https://eprint.iacr.org/2019/1047.pdf)
- [Marlin \& me](https://github.com/ingonyama-zk/papers/blob/main/Marlin_and_me.pdf)

### CP-ZKP
Commit-and-Prove Zero-Knowledge Proof Systems

- [Proposal: Commit-and-Prove Zero-Knowledge Proof Systems and Extensions](https://docs.zkproof.org/pages/standards/accepted-workshop4/proposal-commit.pdf)

### Programming resources

- [A Concise, Opinionated ZK Link Tree by Thor314](https://github.com/thor314/zk-links)

#### Tutorials:

- [A beginner's intro to coding zero-knowledge proofs](https://dev.to/spalladino/a-beginners-intro-to-coding-zero-knowledge-proofs-c56?utm_source=tldrnewsletter). [Github repo](https://github.com/spalladino/zkp-tests)

### Hardware optimization

- [PipeMSM: Hardware Acceleration for Multi-Scalar Multiplication](https://eprint.iacr.org/2022/999.pdf)

### Applications

- [Blind Certificate Authorities](https://eprint.iacr.org/2018/1022.pdf)


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
  
#### ECDSA 

Attaks: 

- [On the security of ECDSA with additive key derivation and presignatures](https://www.shoup.net/papers/2021-1330.pdf)
- [rwc2022 : Threshold ECDSA with additive key derivation and presignatures : an attack, and a solution](https://medium.com/coinmonks/rwc2022-threshold-ecdsa-with-additive-key-derivation-and-presignatures-an-attack-and-a-958b95801b95)

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


## Differential Privacy

## Network Security

### CA

#### Blind CA

- [Blind Certificate Authorities](https://eprint.iacr.org/2018/1022.pdf)


