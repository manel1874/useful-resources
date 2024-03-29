# Cryptographic building blocks

## Table of Contents


* [Physically unclonable functions](#physically-unclonable-functions)
* [Commitment](#commitment)
* [Oblivious Transfer](#oblivious-transfer)
  	* [Flavours](#flavours)
	* [OT protocols](#ot-protocols)
	* [Bounded classical storage model](#bounded-classical-storage-model)
	* [Combiners](#combiners)
	* [Extractors](#extractors)
* [Oblivious Linear Evaluation](#oblivious-linear-evaluation)
  	* [Flavours](#flavours)
* [Fuzzy extractors](#fuzzy-extractors)
* [Leakage Resistant Secret Sharing](#leakage-resistant-secret-sharing)
* [Accumulators](#accumulators)
* [Threshold Cryptography](#threshold-cryptography)
* [Information Theory](#information-theory)


## Physically unclonable functions

- Physically Unclonable Functions: Constructions, Properties and Applications, Roel Maes, 2013, Springer
- [Physically Unclonable Functions in the Universal Composition Framework](https://eprint.iacr.org/2011/681.pdf), chp 5 OT in the PUF-hybrid model and using fuzzy extractors
- [Universally Composable Secure Computation with (Malicious) Physically Uncloneable Functions](https://web.cs.ucla.edu/~rafail/PUBLIC/151.pdf)

## Commitment

### Hash-based (ROM)

- [Topic 14: Random Oracle Model, Hashing Applications](https://www.cs.purdue.edu/homes/jblocki/courses/555_Spring17/slides/Lecture14.pdf): In practice, do not use hash functions based on Merkle-Damg�rd trees. 
- [Lec 3: Commitments and Random Oracle](https://crypto.stanford.edu/cs355/20sp/lec3.pdf) <- very good
- [Security proof](https://people.eecs.berkeley.edu/~daw/teaching/cs276-s06/mtsol.ps)

#### Video

- [Lecture 10.2: Cryptographic Commitments](https://www.youtube.com/watch?v=IkNZWJFcfcU): hash-based and pedersen.


## Oblivious Transfer

### Flavours

- OT
- Random OT
- Batch OT
- OT Extension
- Silent OT Extension

### OT protocols

- Non-interactive oblivious transfer, Bellare, Micali, 1989
- Efficient Oblivious Transfer Protocols, Naor, Pinkas
- The Simplest Protocol for Oblivious Transfer, Chou, Orlandi
- Extending Oblivious Transfer Efficiently, Ishai, Kilian, Nissim, Petrank

#### Post-quantum
- [Two-Round Oblivious Linear Evaluation from Learning with Errors](https://eprint.iacr.org/2020/635.pdf)

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

## Oblivious Linear Evaluation

### Flavours
- OLE
- Random OLE
- Batch OLE
- Vector OLE
- Silent OLE 

### Silent OLE

Silent: after a one-time cheap interaction, two parties can store small seeds, from which they can later locally generate a large number of OLEs while remaining offline.

- [Silver: Silent VOLE and Oblivious Transfer from Hardness of Decoding Structured LDPC Codes](https://eprint.iacr.org/2021/1150.pdf)


## Fuzzy extractors

- [Fuzzy Extractors: How to Generate Strong Keys from Biometrics and Other Noisy Data](https://www.cs.bu.edu/~reyzin/fuzzy.html)
Implementation: [here](https://www.cs.bu.edu/~reyzin/code/fuzzy.html)

## Leakage Resistant Secret Sharing
- [Leakage-resilience of the Shamir Secret-sharing Scheme against Physical-bit Leakages](https://eprint.iacr.org/2021/186.pdf)
- [Leakage Resilient Secret Sharing and Applications](https://eprint.iacr.org/2018/1154.pdf)
- [On the Local Leakage Resilience of Linear Secret Sharing Schemes](https://eprint.iacr.org/2019/653.pdf) 
- [Bounded Collusion Protocols, Cylinder-Intersection Extractors and Leakage-Resilient Secret Sharing](https://eprint.iacr.org/2020/473.pdf)
- [Leakage-Resilient Secret Sharing in Non-Compartmentalized Models](https://drops.dagstuhl.de/opus/volltexte/2020/12112/pdf/LIPIcs-ITC-2020-7.pdf)
- [Continuously Non-Malleable Secret Sharing for General Access Structures](https://eprint.iacr.org/2019/602.pdf)
- [The Mother of All Leakages: How to Simulate Noisy Leakages via Bounded Leakage (Almost) for Free](https://eprint.iacr.org/2020/1246.pdf) 

## Accumulators

- [An Overview of Cryptographic Accumulators](https://arxiv.org/pdf/2103.04330.pdf)

## Threshold Cryptography
- [YouTube] [Cyber Week 2019 - Academic Perspectives on Cybersecurity Challenges - Threshold Cryptography](https://www.youtube.com/watch?v=StDSvc4Mm50)

## Information Theory

### Important inequalities

#### Pinsker's inequality

- [Wiki](https://en.wikipedia.org/wiki/Pinsker%27s_inequality)

#### Fano inequality


### Divergence

- [Kullback-Leiber wiki](https://en.wikipedia.org/wiki/Kullback%E2%80%93Leibler_divergence)

### Entropy

-[R�nyi wiki](https://en.wikipedia.org/wiki/R%C3%A9nyi_entropy)
- Relation between entropy and divergence: [Renyi Divergence and Kullback-Leibler Divergence](https://arxiv.org/pdf/1206.2459.pdf); [What Is Randomness? The Interplay between Alpha Entropies, Total Variation and Guessing](https://www.mdpi.com/2673-9984/5/1/30)


