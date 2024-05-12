
A crypto exchange is a platform that allows users to buy and sell their cryptocurrencies.

Centralized exchanges own your private key and usually hide the complexity as they are mostly very matured products. They are usually easier to use than decentralized exchanges. They can be also used for on-ramp/off-ramp fiat money.

Decentralized exchanges don't have access to your private key and you don't hold any money on them, so they are more secure. The UI/UX is more complex though and you have to learn very well how to use them.


### **AMM vs Order-book**

![[Pasted image 20240207200156.png]]

There are 2 main mechanisms for the swapping between coins:

1. Order-book matching 
2. AMM (automated market maker)

In the case of order-book matching implementation, all the parties have to agree on the swap exchange rate. The market makers can create bids at a certain price and allow others to fill those bids. Until the bid is taken the market maker can withdraw the offer or update the price. 

In some cases, this can be inefficient as both parties have to agree on the price to be executed which means you won’t be able to always find buyers/sellers.

An AMM is a smart contract that holds assets in the form of liquidity pools(LP) for both sides of the trading pair and automatically sets the price for trading based on a price curve. 

One of the main advantages compared to the order book mechanism is that you don’t need a counterpart to execute a trade, so you can execute your trade any time. 

Your funds are also in your custody until the transactions goes through which means there is no counterpart risk. 

There are other important benefits as well that we won’t discuss in this lesson.


### **Which one to use?**

![[Pasted image 20240207200410.png]]

Try to use decentralized exchanges whenever you can.

In general you should only keep as much money on centralized exchanges as you need for trading.

You will also use centralized exchanges for on-ramp/off-ramp money but once you are done with that that you should move your coins on-chain into self custody.

Some coins will be available or liquid enough only on certain centralized exchanges. In that case you can buy the coins there but then make sure you move the coins on-chain into self custody.

### **Decentralized exchanges (DEX's)**

![[Pasted image 20240207200508.png]]

Most heavily used decentralized spot exchanges use some kind of AMM implementation. Some of them are cross-chain some of them only work on one chain. If you wanna use decentralized perps exchanges then you have to check their implementations one by one as they are pretty complex.

Some of the spot exchanges focus on swapping stablecoins others focus on swapping other tokens.

Every chain has its main DEX's. Before buying any coins you will always have to check where those coins are available.

Largest ones are:

#### **Uniswap, Sushiswap, PancakeSwap**



### **Where to buy**

Large cap coins are usually available on several chains and both on centralized/decentralized exchanges.

Small cap tokens are usually only available on decentralized exchanges and only on their original chain. There are few exceptions as some tokens launch on exchange launchpads.

If a token is available on many exchanges then you will have to check where it is the best to for you to buy a particular token.

You wanna buy securely (verified platform) and as cheap as possible. To make sure you won't overpay, you have to find exchanges where the token is liquid enough (your buy size don't move the price too much). The bigger your size is the less options you have.

In some cases you have to bridge your money to a different chain. You can also withdraw money from centralized exchanges on certain networks. For instance you have some $USDC on-chain wallet on Ethereum and you wanna move it to BNB Smart Chain chain to buy other tokens. You can use a bridge to move your tokens over. You can also just send it to Binance through Ethereum network and then withdraw it on BNB Smart Chain network.

### **Buying coins on Uniswap**

![[Pasted image 20240207201027.png]]

Uniswap is the largest spot exchange on Ethereum. We will use this in the lesson but you will always have to double check where the coins are available. Buying coins on any of the decentralized spot exchanges should be a very similar process.

1. Connect your wallet (Metamask) that has some $ETH in it for gas fees and the tokens you wanna sell for the tokens you wanna buy.
2. Choose coins to sell and buy (look for token address if it's not in the dropdown).
3. Authorize the dApp to sell your tokens.
4. Choose the amount of tokens you wanna buy/sell.
5. Set the slippage tolerance (almost always it should be 0.5%)
6. Check if the price impact is not too high
7. Click on swap
8. Interact with Metamask and start the transaction
9. Wait for the transaction to confirm


### **Easiest way to find where to buy coins**

1. Search for, and identify the token you're trying to buy then use **Coingecko** or **CoinMarketCap**. 

The basic info like price, MC, liquidity, and FDV can be all found on these pages.

2. If the coin can’t be found on those sites (common for new/small coins), use **Dextools** or **Dexscreener**. 

3. To find more info about small cap coins (e.g. emission schedule, future events) the best thing is to check the docs of the project or talk to people in the project’s discord server.


### **Finding Token Address**

![[Pasted image 20240207201435.png]]

Once you figured which DEX you wanna buy the tokens on you might have to find the token address as well.

Coingecko and Dexscreener both should show you the token address. Once you find it you can copy that address to the token field on Uniswap (or other DEX) and the coin will pop up.

If you wanna be extra careful then check the token details on etherscan. Looking at the token holder and transfer numbers is a good start. If you wanna buy $USDC you would expect a lot of addresses holding that coin for instance.


### **How to buy alts**

1. Find the Coin (Dexscreener, CoinGecko), Confirm its the right token ![[Pasted image 20240208013343.png]]
2. What address![[Pasted image 20240208013355.png]]
3. What market
4. ![[Pasted image 20240208013438.png]]
5. What Chain![[Pasted image 20240208013655.png]]
7. Where can buy


### **Token approval**

## References
<!-- Links to pages not referenced in the content -->
-[[Decentralized]]