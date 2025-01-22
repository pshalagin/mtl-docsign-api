# MTL Document Signature API

A solution for better documents signing using Stellar blockchain and decentralized file systems.

## Idea

The following workflow proposed -- 
1. A user uses GUI in order to upload a document to a decentralized cloud
2. A service acts like a signature broker accepting incoming signature transactions (sending small amounts of crypto with a document hash as memo).
3. User can "sign", i.e. the service builds a transaction which user signs in any their Stellar wallet. After that the doc is considered signed.
4. A doc status, all its signers, transaction links can be requested via API and with GUI.
5. Optional feature is to draw back a signature with another transactions.   


## Implementation

### Proposed Techs

#### Steganography

* https://github.com/tbpaolini/imgconceal
* https://hackernoon.com/simple-image-steganography-in-python-18c7b534854f

#### Distributed File Storage

* https://www.tahoe-lafs.org/trac/tahoe-lafs

#### Cryptography

* Stellar key algo -- https://ed25519.cr.yp.to/software.html 
* https://stackoverflow.com/questions/37725969/several-pgp-signatures-for-one-file 
