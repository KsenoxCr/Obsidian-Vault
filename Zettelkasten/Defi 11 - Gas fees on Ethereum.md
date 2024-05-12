### Gas

![[Pasted image 20240302190735.png]]

Gas refers to the unit that measures the amount of computational effort required to execute operations on the blockhain.

Since every Ethereum transaction requires computation to execute, every transaction also requires a fee. Gas refers to the fee required to execute a transaction. It doesn't matter if the transaction succeeds or fails.


### Why gas fee exists

Gas fees help keep the Ethereum network secure.

Bad actors are prevented from spamming the network by requiring gas for every computation executed on the network.

In order to avoid accidental/malicious infinite loops or other computational waste in the code, every transaction is required to set a limit on how many computational steps of code execution it can use.


### Denominations of Ether

![[Pasted image 20240302190858.png]]

Gas fees on Ethereum are paid in ether ($ETH).

Gas prices are denoted in gwei. Gwei itself is a denomination of $ETH, each gwei is equal to 0.000000001 ETH (10^-9 ETH). This also means that 1 $ETH equals 1,000,000,000 gwei.

Rather than saying that gas costs 0.000000001 $ETH, you can say your gas costs 1 gwei.


### Gas limit

Gas limit is the max amount of gas you are willing to spend on a transaction. More complex transactions with smart contracts that require more computational work also require a higher gas limit. A standard ETH transfer requires a gas limit of 21,000 units of gas.

If you put a gas limit of 30,000 for a simple ETH transfer, then 21,000 would be consumed and you would get back the rest (9,000).

If you specify too little gas limit like 18,000 for a simple ETH transfer, then the EVM (Ethereum Virtual Machine) will consume your 18,000 gas units but the transaction will fail. The EVM then reverts the changes, but that gas is consumed and you lose the transaction fee.

MetaMask automatically sets your gas limit depending on the transaction. In almost all cases, this will be enough to complete your transaction. If you want to check it or edit it, you can turn on advanced gas controls.



### London fork

The transaction fee calculation was changed with the London Upgrade in August 2021.

Let's say you have to pay 1 $ETH with the gas limit of 21,000 units.

Calculation before London Upgrade with 100 gwei gas price:

Gas units (limit) \ Gas price per unit i.e 21,000 \ 100 = 2,100,000 gwei (0.0021 $ETH)

Calculation after London Upgrade with 50 gwei base fee and 10 gwei priority fee:

Gas units \ (base fee + priority fee). 21,000 \ (50 + 10) = 1,260,000 gwei (0.00126 $ETH).

From now on we will focus only on the new system (after London upgrade).


### Block

![[Pasted image 20240302191215.png]]

To maintain a synced state and agree on the precise history of transactions among all participants, transactions are batched into blocks. This means many transactions are committed, agreed on, and synced all at once.

To maintain the transaction history, blocks are ordered and transactions within blocks are ordered as well.


### Block size

Before the London Upgrade, Ethereum had fixed-sized blocks. In case of high network demand, these blocks operated at full capacity. Due to this users often had to wait for demand to reduce to get included in a block.

The London Upgrade added variable-sized blocks. All blocks have a target size of 15 million gas, but the size of blocks can change based on network demand up to 30 million gas (2x the target block size).

 If the block size is greater than the target block size, the base fee for the following block will be increased. If the block size is less than the target block size then the base fee will be decreased. The amount by which the base fee is adjusted is proportional to how far the current block size is from the target.



### Base fee

Every block has a base fee which acts as a reserve price.

To be eligible to be included in a block the offered price per gas must reach the base fee. The base fee is calculated based on the prev blocks which makes transaction fees more predictable. When the block is added the base fee is "burned".

The base fee is calculated by comparing the size of the previous block with the target size. The base fee will increase by max 12.5% a block if the target block size is exceeded.



### Base fee calculation

![[Pasted image 20240302191507.png]]

Check the table below. To add a transaction on block  a wallet will let the user know that the max base fee to be included on the next block is 202.7 gwei (current base fee) \* 1.125 (112.5%) = 228.1 gwei.

This is why gas fees can spike insanely high for a few minutes/hours in case of high demand. But this exponential growth (112.5%) makes it economically non-viable for block size to stay high for a long time since users will not make transactions if it's not worth it.

 For instance no one wants to pay 1 $ETH in gas to trade 0.5 $ETH for $USDC.



### Priority fee (tip)

![[Pasted image 20240302191628.png]]

Before the London Upgrade, miners would receive the total gas fee from any transaction included in a block.

After London Upgrade with the base fee getting burned a priority fee (tip) was introduced to incentivize miners to include a transaction in the block. 

With no tips, miners would mine empty blocks as they would receive the same block reward. 

A small tip provides miners an incentive to include a transaction. If you wanna have your transaction prioritized you need a higher tip to outbid other competing transactions.

### Max fee

Users can specify a max limit they are willing to pay for their transaction to be executed. This optional parameter is known as the maxFeePerGas. 

For a transaction to be executed, the max fee must be greater or equal than the sum of the base fee + the priority fee (tip). 

The transaction sender is refunded the difference between the max fee and the sum of the base fee and tip.

max fee >= base fee + priority fee

refund = max fee - (base fee + priority fee)

If you use the advanced Metamask gas UI then currently you are able to set the max for base fee. In this case your max fee won't exceed max base fee + tip.



### MetaMask

Currently if you use MetaMask most of the things are calculated by Metamask for you. 

You can choose from Low/Market/Agressive speed and see the estimated execution time and fees.

I almost always choose Agressive since the difference is negligible and I don't want my transaction reverted in case of some people frontrun me.


### MetaMask Advanced

Advanced gas fee is recommended when you really wanna execute your transactions quickly. 

For instance in case of a huge market dump or a long awaited NFT mint.

You have to increase both the Max base fee and the Priority fee if you wanna make sure your transaction succeeds.

## References
<!-- Links to pages not referenced in the content -->
-[[Decentralized]]