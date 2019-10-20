# BlockChain
San José State University

CS266: Topics in Information Security Autumn 2019

Prof. Guha Jayachandran
https://cs.stanford.edu/~guhaj/


The goal of this project is to build a basic blockchain with a proof-of-work mechanism and Merkle tree-based data storage.

*Deliverables*

1) Code that

A) implements a blockchain—in particular, a main loop that repeatedly obtains new data
and computes and outputs the hash ​H(d)​ of data structure ​d​ (see instructions below).

B) The data structure ​d​ must contain
- a hash of the previous block
- a Merkle Tree (see instruction D below) - a nonce

C) The first 16 (binary) digits of each block hash must be 0.
from DataSimulator import DataSimulator DSim = DataSimulator()
d = getNewData()
import ECC
isVerified = ECC.verify(publicKey, message, signature)


D) the Merkle Tree must be build from all valid elements received from the DataSimulator, i.e. all valid ​(publicKey, message, signature)​ tuples where the signature is valid


2) Provide a Merkle Tree-proof that a specific item is part of the Merkle Tree in an ancestor of the last block. In detail, given the created blockchain after 5 blocks, show proof that the headline
cabinet meets to balance budget priorities
was “put on the blockchain.”

