
### **Risks that hardware wallets mitigate | 1**


The main goal of a cold wallet is to provide a secure way to interact with the blockchain while mitigating the risk of someone gaining access to your private key. 

A hardware wallet stores the private keys offline that is designed to keep these secrets secure. This is the main purpose of the device. Every other functionality is only secondary to this main purpose. Even if your computer is hacked, the private keys needed to transfer your assets are never exposed. The keys only live on the device, they're never seen by your computer.

Your laptop is insecure in comparison. Storing the keys in a wallet on your laptop is a bad idea as the attack surface is way higher. Your keys are exposed to different malware and phishing attacks. ‎ ‎


### **Risks that hardware wallets mitigate | 2**

![[Pasted image 20240206210025.png]]

The other risk it mitigates is that you can have a better visibility of what transaction you sign. Your hot wallet on your laptop could be compromised and you sign a malicious transaction that looks legit.

The malware would show the correct function when you sign the transaction but would apply it to a separate transaction. 

If you use a cold wallet it will always display the actual transaction on your screen as you sign it. This is the main application of the Lattice1 that can show you the human readable format of what you sign instead of the hex version.



### **Risks that hardware wallets DON'T mitigate**

- Your hardware wallet does not implicitly secure your seed phrase. If your backup is compromised then a bad actor will have access to your funds regardless of your hardware wallet.
‎
- If you **lose your seed phrase** then you can’t recover your account.
‎
- NFT/token drains. If you **approve a malicious transaction** on your hardware wallet then consider your NFT’s/tokens gone. Always double check what you sign.
‎
- **Smart contract risk**.  If you stake or LP your tokens and there is a vulnerability in the smart contract then you could lose your tokens. You authorized the contract to have control over your funds. Or If you authorize the protocol like Uniswap to swap your tokens (you have to if you wanna sell tokens) and the smart contract gets hacked then your tokens could be stolen.


### Which hardware wallet to use?


Besides Ledger there are other good brands like Trezor and Lattice Grid. There are also different Ledger products like Ledger Nano X and Ledger Nano S Plus.

All of them store the private keys offline and you also have to sign transactions regardless which one you use.

The main difference is the usability. Let's see a few comparisons:

#### **Nano X vs Nano S Plus** 

Nano S Plus has no battery, no bluetooth but it's much cheaper. Those features are not important, so I would just buy Nano S Plus.

#### **Lattice Grid vs Ledger Stax**

They both make transactions easy to read which is super convenient. You always gotta check the transaction that you sign otherwise the cold wallet won't protect you. I would choose Ledger Stax as Lattice Grid is huge and it's not really portable.

#### **Ledger Stax vs Nano S Plus**

Stax makes it easy to read the transactions but it's much more expensive than the Nano S Plus. I will personally switch to Stax but if you can't afford the price then stick with Nano S Plus and deal with the worse UI/UX.

Regardless which one you use you have to read the transactions that you sign.


### Using your cold wallet seed phrase

Same like with software wallets you have to make sure you don't expose your seed phrase.

It's also super important not to accidentally type your cold wallet seed phrase into a hot wallet accidentally. If you take the seed phrase from a hardware wallet and accidentally import it to your computer, you've basically rendered your hardware wallet useless because there are now multiple places where your private keys are stored. Your cold wallet has now become a hot wallet.

If that happens then move your money to a different account (different seed phrase) as soon as possible.


### **Using Ledger with Metamask**

![[Pasted image 20240206211812.png]]

If the Ethereum App is installed on your Ledger then you can connect it to Metamask by clicking on Connect hardware wallet in your Metamask account.

The reason you don't have to install other EVM compatible chain apps on your Ledger is that you can easily switch between networks with the help of Metamask.

If you wanna use a non-EVM compatible chain like Solana then you will have to install other apps as well.

Once you connected your Ledger to Metamask you can do all the interaction through Metamask. Everything will be the same like when you use Metamask only except once you trigger a transaction you will have to sign it with your Ledger.



### **Using Ledger as a vault**

**If you use** one of your **Ledgers as a** **vault**, then **don't connect it to any dApps.**

In this case vault means your high value, long term holdings including coins and NFT's.

What does it count as high value? That's up to you. If you have 10 $ETH on a Ledger but you have 10,000 $ETH then you don't really care about those 10 $ETH's. On the other hand if you have 15 $ETH then those 10 $ETH's count as high value compared to your full portfolio size.

You can connect your Ledger to Metamask BUT **don't connect it to Uniswap, Opensea, or any other applications.** This gives you an extra level of safety.
## References
<!-- Links to pages not referenced in the content -->
-[[Decentralized]]