
### DYOR

Always do your own research.

In the lessons we give you the currently recommended tools (wallets, tokens, exchanges,  marketplaces, etc.) BUT you are responsible for your own decisions.

Some of these could rug or could be exploited.

Always use everything carefully and do proper risk management.


### **Metamask is a hot (software) wallet used to interact with the EVM compatible blockchains like Ethereum, Avalanche, or Fantom.**

It allows users to access their wallet through a browser extension or mobile app, which can then be used to interact with decentralized applications.

Don't use Metamask on mobile.

Use it only as browser extension with Chrome or Brave.


### **Non-custodial**

As discussed in previous lessons with Metamask you own your private key (in a form of seed phrase).

While a custodial wallet is usually considered less secure than a non-custodial wallet, many prefer them because they don’t require as much responsibility and are usually more convenient. 90% of the people are better off using only exchanges as they have no idea how things work.

But you are a professional. If you learn to use Metamask well then it's much safer than the exchanges and you have much more control over your money, transactions and interactions.

Also, to use dApps you will need to use non-custodial wallets.


### Seed Phrase

There are several ways to store your seed phrase. You have to make sure no one can get access to it besides you and you shouldn’t lose it either.

What I do personally is to save it in a text file then encode it (AES 256-Bit Encryption for instance) and keep it on a USB stick or cloud storage.

This is so that if someone compromises the file, it’s still encrypted and protected by a strong password.

Some people like to write it down on a piece of paper. I personally don't like that approach as it could get damaged or lost.


### **Using your seed phrase**

The ONLY time you have to use your seed phrase is when you login to Metamask through the MM interface.

Never ever type your seed phrase anywhere else. If you accidentally do that and expose your account will be exposed. This means all the addresses with that account will be exposed too.

If it happens then immediately move your funds to another account from all of your addresses of the exposed account if your money is not gone yet.



### Using Addresses

![[Pasted image 20240206204248.png]]

Within one account (one Metamask instance with one seed phrase) you can create many addresses. In the UI it's called account which is a bit confusing.

Create a few to spread risk. If you sign some malicious transactions then you will only lose your money that's under that address. The rest of your addresses within that account should be safe as long as you don't give out your seed phrase.

**For trying new dApps (DeFi protocol, NFT mints) always use a burner address. You should only add as much money as necessary and you are willing to lose.** 



### **Connecting to different RPC's**

![[Pasted image 20240206204236.png]]

A Remote Procedure Call (RPC) node is a computer server that allows users to read data on the blockchain and send transactions to different networks.

dApps need to communicate with blockchains to access info and make transactions. This connection is facilitated by what is known as RPC nodes.

Add/switch networks in the settings.

Why would you switch RPC's? Sometimes the nodes go down or get congested, so you have to switch to another one to execute your transactions. Some of the nodes also have privacy issues.


### **Connecting to different networks**

As discussed on the previous slide all the networks like Ethereum have several RPC nodes, so when you switch RPC you might stay on the same network.

But you can use Metamask with all the EVM compatible chains (Fantom, Avalanche) as well.

You can add the different networks as just new RPC nodes in the settings. The main difference will be the chain ID that identifies the given blockchain.

Once you added the new network, you can easily switch between.


### **Add money to the address to execute transactions**


![[Pasted image 20240206204701.png]]

To be able to execute transactions you will have to send chain native coins to pay gas. You have to send them from some other addresses or exchanges. You need $ETH in your wallet on Ethereum network to be able to execute transactions. On other chains it can be other tokens: $FTM -> Fantom network, $ETH -> Arbitrum network.

### **Add money to the address to execute transactions**

![[Pasted image 20240206205219.png]]

To be able to execute transactions you will have to send chain native coins to pay gas. You have to send them from some other addresses or exchanges.

You need $ETH in your wallet on Ethereum network to be able to execute transactions. On other chains it can be other tokens: $FTM -> Fantom network,
$ETH -> Arbitrum network.

## References
<!-- Links to pages not referenced in the content -->
-[[Decentralized]]
