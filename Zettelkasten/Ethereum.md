
## **What is Ethereum?**

"Ethereum is a deterministic but practically unbounded state machine, consisting of a globally accessible singleton state and a virtual machine that applies changes to that state." - Gavin Wood 

**That sounds a bit complex doesn't it? Let's try a more simple way.** 

Ethereum is a blockchain with a computer embedded in it. It is the foundation for building apps and organizations in a decentralized, permissionless, censorship-resistant way. 

**To make it even simpler:** 

Ethereum is basically a "world computer" that executes applications on the top of a blockchain.



### **Ethereum compared to Bitcoin**

Ethereum’s purpose is not mainly to be a currency payment network like Bitcoin. While ether ($ETH) is a necessary for the operation of Ethereum, $ETH is intended as a utility currency to pay for the usage of the "world computer". 

Ethereum is a general purpose, programmable blockchain that executes code. Ethereum can function as a computer and applications can be implemented on it. 

This is why you can have decentralized applications on it.



### **Ether Currency Units**

Ether can be divided into smaller units down to the smallest unit possible called wei. 
It's like the penny (one-cent-coin) for to US Dollar. 

**Wei = 1
wei** **Gwei = 10^9 wei** 
**Ether (ETH) = 10^18 wei** 

We is the smallest unit of ETH, but most often you will use gwei (connected to gas fees) and ether ($ETH).



### **Externally Owned Accounts (EOAs) and Contracts**

The type of account that you can create through your wallet is called an externally owned account (EOA). These accounts have a private key. Having access to the private key means you have access to funds or contracts. 

Only EOAs can initiate transactions, but contracts can react to transactions by calling other contracts. 

Simply put, with the help of your wallet you can access your account (EOA) and you can trigger executing applications. When you wanna swap $BTC for $ETH you actually do this.


## **Smart Contracts**

That other type of account is called a contract account. A contract account is a smart contract deployed to the network, controlled by smart contract code. A contract account does not have a private key. It is owned/controlled by the logic of the code in the smart contract. Contract account also have addresses just like EOA.

Users don't write code. Application developers upload programs and users make requests to execute these code snippets with varying parameters. We call the programs uploaded to and executed by the network smart contracts.

You need smart contracts to write application code. Uniswap, Opensea, and other applications all have product specific smart contracts.

### **Transactions**

![[Pasted image 20240206190506.png]]

To update the data on the blockchain, Ethereum uses messages, in the form of transactions, representing the change. They are signed messages originated by an address, broadcasted by the Ethereum network.

They are the only things that can trigger a change of state (data update) or cause a contract to execute. Ethereum doesn’t run autonomously. Everything starts with a transaction.

This means if you wanna buy a coin, mint an NFT, or do anything that updates the data on the blockchain, it must be done through transactions.

Transactions need gas. Gas is the fee required to successfully conduct a transaction or execute a contract. The concept of gas was created to pay miners (PoW) for their work done on maintaining and securing the blockchain. After Ethereum switched to proof-of-stake (PoS), gas fees became the reward for staking $ETH and taking part in the validation.

### **Gas fees**

![[Pasted image 20240206190830.png]]

Ethereum transaction requires computational resources to execute. Those resources have to be paid for to ensure Ethereum is not spammed with random transactions and cannot get stuck in infinite computational loops.

Payment for computation is made in the form of a gas fee.

Gas is the unit that measures the amount of computation needed to execute programs on the Ethereum network.


### Wallets

Ethereum wallets are applications that give you control over your account, so a wallet is your gateway to the Ethereum blockchain. It holds your public/private keys and can create and send transactions on your behalf.

When you interact with the Ethereum network through your wallet you identify yourself with your keys.

### **Keys and Addresses**

The private keys are at the center of all user interaction with Ethereum. Account addresses are created directly from private keys.

Access and control of funds is done with digital signatures, which are also created using the private key.

A private key comes with a public key. Think of the public key as similar to a box account number, and the private key as similar to the key of that box. The private key provides control over the account, and the public key identifies it to others.

### Tokens on Ethereum

Tokens are not like $ETH because the Ethereum network does not know anything about them.

Sending/owning $ETH is built into the Ethereum network, but sending/owning tokens like $DOGE is not.

The $ETH balance of the accounts is handled by the protocol level, but the token balance of the accounts is handled at the smart contract level.

If you wanna create a new token you have to use smart contracts that has rules for ownership, transfers, etc.

## References
<!-- Links to pages not referenced in the content -->
-[[Decentralized]]
