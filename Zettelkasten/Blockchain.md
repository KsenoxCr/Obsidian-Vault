
![[Pasted image 20240204182428.png]]

**What is a blockchain?**

A blockchain is a simple and elegant data structure. It’s basically a linked list and each block has a cryptographic hash of the previous block. This creates an unalterable chain of blocks and their ID's, going back to the original block. Linked list: An ordered set of data elements, each containing a link to prev or next link. Unlike the blocks of the blockchain, the elements in the linked list can be altered. "Blockchains are public, permanent records. It's the most auditable ledger." - CZ

## Hash Functions 

Each block on the blockchain has an **hash** which is always the **same length** 

![[Pasted image 20240205210214.png]]

![[Pasted image 20240205210221.png]]

![[Pasted image 20240205210340.png]]

![[Pasted image 20240205210348.png]]

## Purpose of Hash Function is Identification without revealing the content

![[Pasted image 20240205210538.png]]

Hash is only valid when the chosen criteria happens. This criteria was chosen when the particular blockchain was created (ex. 0000 at the beginning) 

nonce = number used once

![[Pasted image 20240205211118.png]]

![[Pasted image 20240205211302.png]]

![[Pasted image 20240205211319.png]]

## Single Blockchain

blocks in the blockchain are connected by links

link = reference to the previous block

#### It is hard to spoof or cheat the block chain cause when one block is tampered, all blocks after it need to be re-mined. 

Thats due to them being linked to each other

![[Pasted image 20240205212721.png]]

### **How a blockchain becomes decentralized**

You need several nodes to reach decentralization. If all of them in the system replicates this linked list (and verifies its legitimacy by repeating the cryptographic hash functions), it will implement a slow distributed database that’s resistant to tampering. With this you can create completely decentralized systems that require no trust among participants. Of course to build functional protocols on blockchains, you need a lot more than this but this is the very basics.

## **Distributed blockchains

More nodes with the same blockchain are needed to validate if the data in a block is real/valid

If there was only a single blockchain, nobody can know whether one block's data was hacker or not

but with multiple identical ones the nodes can see if one is different than the rest = tampered. 


When there are thousands of nodes around the world, the majority can decide which data is valid


## **Public/private key pairs video**

![[Pasted image 20240205213944.png]]

Private --> accessed with seed phrase consisting of 12 to 24 words

Public key = wallet addresses that can be generated with the private key

#### Public keys: 

![[Pasted image 20240205214132.png]]

## It goes one way

With private key --> can generate public key

With public key --> can not get the private key



Signature on message is created based on message + public key

so the sender can be identified by the signature 




# **Transactions with public/private key pairs**

![[Pasted image 20240206172810.png]]

![[Pasted image 20240206172827.png]]

You should be the one who sends the transaction 


## NEVER lose or give away private key

If someone has your private key, they can sign transactions 



### **Applications**

Blockchains can be used for many things. Some of the most notable ones: 

**- Global Financial Infrastructure**
**- Voting**
**- Insurance policies**
**- Custodial records**
**- Crypto**

The list goes on but the point is that all these systems can be implemented transparently with no corruption.

# Private vs Public Blockchains

![[Pasted image 20240206174004.png]]

## Public Blockchain

### Advantages:

- truly decentralized
- democratized
- authority-free operation

### Disadvantages: 

- Big and slow

![[Pasted image 20240206174555.png]]

![[Pasted image 20240206174710.png]]'

![[Pasted image 20240206174920.png]]

![[Pasted image 20240206175009.png]]


![[Pasted image 20240206175156.png]]
## References
<!-- Links to pages not referenced in the content -->
-[[Decentralized]]