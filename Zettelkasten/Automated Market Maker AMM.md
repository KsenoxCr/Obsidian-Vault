
An AMM is a decentralized application that provides a way to swap/trade tokens in a non-custodial way is called a DEX (decentralized exchange). 

The swap only executes if the conditions are met by all parties. If any of the conditions is not met the transaction is reverted and all parties retain their funds.

AMM's are one of the largest inventions DeFi products have ever come up with. They totally changed the game.
‎

### AMM vs Order book

‎Order-book matching and AMM (automated market maker) are 2 main mechanisms for the swaps.
‎
For the order-book matching implementation all the parties have to agree on the swap exchange rate. The market makers can create bids at a certain price and allow others to fill those bids. Until the bid is taken the market maker can withdraw the offer or update the price. This can be inefficient as both parties have to agree on the price to be executed, so you won’t be able to always find buyers/sellers.
‎
An AMM is a smart contract that holds assets in the form of liquidity pool (LP) for both sides of the trading pair and automatically sets the price based on a price curve. One of the main pros compared to the order book mechanism is that you don’t need a counterpart to execute a trade, so you can execute your trade any time. Your funds are also in your custody until the transactions goes through so there is no counterpart risk. 

### AMM implementations

‎In this section we will focus only on pool2 (constant product formula) and stable swap formula.
‎
Pool2 is the original AMM mechanism by Uniswap v2. Most of the other main DEX’s (Sushi, PancakeSwap, SpiritSwap, TraderJoe, etc.) Use this mechanism as well. 

There is also a newer Uniswap version (v3) which is more advanced and won’t be discussed here.
‎
The other main implementation is the stable swap formula which was created by Curve finance to trade highly correlated assets.

### Constant product formula

![[Pasted image 20240218154015.png]]

The Uniswap v2 (pool2) trading price ratio is defined with the x \* y = k trading curve ratio where x is the balance of token A, y is the balance of token B, and k is a constant invariant that never changes. 

To maintain this k invariant if you want to sell A, B must be bought by the contract and vice versa.

### **Constant product calculation**

![[Pasted image 20240218154033.png]]

‎We will use ETH- USDC pool for the example and will neglect gas fees and transaction fees. 

The pool has 100 ETH that currently trades at $100 and 10,000 USDC that of course $1 each.
‎
100 \* 10,000 = 1,000,000. This means an initial value of 1,000,000 for constant k.
‎
Let’s say we wanna buy 20ETH. 1,000,000 = (100 - 20) \* x. If you solve this you get x = 12,500. This means we have to pay 12,500 - 10,000 = 2,500 USDC to get 20 ETH.

Let’s try to buy 20 ETH again. Currently the pool looks like this: 1,000,000 = 80 \* 12,500
‎
After the 20 ETH buy it's gonna be:
‎
1,000,000 = (80 - 20) \* x. If you solve this then x = 16,667. We have to pay 16,667 - 12,500 = 4,167 USDC to get 20 ETH.

The price before our transaction was $125 / ETH but we only got 20 ETH for swapping 4,167 USDC which translates to $208 / ETH.
‎
As you can see the more one-sided the pool gets the bigger the price impact will be for the swaps.

### Constant product main considerations

You need to get some math knowledge to understand this concept but you have to understand the basics to avoid costly mistakes.

The next slide covers the main takeaways.

### Constant product main considerations | 2

- If you buy major alts then most likely you won't have any issues as your size will be small compared to the liquidity in the pool, so you barely move the price (low price impact) on the curve.

- If the pool is very imbalanced then you might get worse price (large price impact) than buying it somewhere else. Again this likely won't happen to major coins.

- If the pool has low liquidity then you might get bad price (large price impact) even if the pool is balanced. This can happen in the case of low cap altcoins.

- **Always check what your price impact would be before buying**. If you don't like the terms then buy the coin somewhere else. **If you can't buy it anywhere else then think twice if it's worth buying**.

- **Super imbalanced pools are a warning sign**. Always figure out why the pool got into that state in the first place. Think of the stETH-ETH pool back in 2022 June when big entities were forced to sell regardless the price impact.

- Most of the new altcoins are not available on CEX's and you have to buy them on-chain on Uniswap or similar. In that case you have no choice but buy the coin on AMM's.

### **Stableswap formula**

![[Pasted image 20240218154118.png]]

The constant product invariant doesn’t make any assumptions about the pricing of underlying assets and spreads liquidity across all prices evenly.

The stable swap invariant enables to focus most of the liquidity around 1.0 (or any other price) which is great for creating liquidity for stablecoin pairs.

This is great if you wanna switch a large amount of stables like $USDC for another stable like $USDT. The price doesn't move that much as long as the pool is not too imbalanced thanks to the mostly linear connection between the prices.
‎
Check Curve Finance and compare it to Uniswap v2 when it comes to buying stables with other stables. You will see it's much better to do it on Curve if you wanna buy large amounts.


### **Stable Swap considerations**

- Most likely you won't even have to use these types of pools. You won't use Curve as it is for whales who wanna swap millions of dollars worth of stables. - There are some newer cutting-edge DeFi products that use stable swap too with low liquidity. Those are super advanced products like Solidly ve(3,3). If you want to use these then you have to really understand what you are doing. If you don't then you should avoid them.

# Slippage vs Price Impact

Slippage and Price Impact are two common terms used to describe the outcome of a change in price when swapping cryptocurrency.

It is important to note that these terms do not mean the same thing.‎

Price impact is the change in token price caused by your trade.

Slippage is the change in token price caused by the total movement of the market while your trade is going through. 

### Slippage | 1

![[Pasted image 20240218225931.png]]

‎Slippage is basically when a trade settles for a different price than expected or requested.

 To put it another way it is the price difference that occurs between the token’s quoted price and the paid price. 

Slippage is reflected as the difference between the price you expect to receive after swapping vs what you actually receive after the swap is complete.
‎
High slippage is present in markets with high volatility and/or low liquidity.

### **Slippage | 2**

Let’s reuse the the initial pool from the example above. If you were to put in an order for a 20 ETH buy but someone else at the same time puts in another 20 ETH buy order both of you would expect to pay $125 / ETH for that order. 

But if the other transaction gets executed before yours that person pays the expected $125 / ETH and you will pay $208 / ETH. That’s a huge difference.
‎
Slippage could be both negative and positive but most likely it is gonna be negative thanks to how transactions work.
‎
AMM’s let you set slippage tolerance so you can protect yourself from much higher prices than you would expect.
‎
If the slippage tolerance is too low, your order may take longer to execute or not execute at all. 

If it is too high, another trader or a trading bot may see your pending transactions and front-run you.

### **Front running**

If another trader/bot sees your high slippage, by setting a higher gas fee than yours, will make his transaction execute first. 

After your transaction goes through as well, the front runner inputs another trade to sell it at a higher price that was made possible by you.
‎
Make sure you don’t set the slippage too high 0.5-1% should work well.

If you would like to see more details on sandwich attacks and MEV then check the Experienced Misc track and look for the MEV 101 thread.

### Price impact

![[Pasted image 20240218230925.png]]

‎We talked about price impact in the the previous lesson as well but it's important to understand that the price impact only considers the current state of the pool and how the size of your trade moves to price for the tokens. 

Price Impact is reflected as the difference between the current market price and how your trade impacts the total liquidity in a pool.

You can always see the estimated price impact when you decide how much you wanna buy/sell.

If you wanna buy big amounts that of course will move the price more even in a balanced pool. 

![[Pasted image 20240218231213.png]]

![[Pasted image 20240218231233.png]]

![[Pasted image 20240218231243.png]]
![[Pasted image 20240218231251.png]]

![[Pasted image 20240218231300.png]]

### Sandwich attack

![[Pasted image 20240218231447.png]]

# **Providing Liquidity (LP)**

"Anyone can become a liquidity provider (LP) for a pool by depositing an equivalent value of each underlying token in return for pool tokens. These tokens track pro-rata LP shares of the total reserves, and can be redeemed for the underlying assets at any time." - Uniswap

AMM’s can only work effectively if the liquidity pool is deep enough, so the swaps between two tokens will be executed with an acceptably low slippage. AMM's incentivize users to LP to make the pools deep enough, so other users can trade the assets.

### **LP calculations**

![[Pasted image 20240218232005.png]]

In lesson  (AMM) the pool had 100 ETH and 10,000 USDC initial liquidity.
‎
Liquidity can be provided by adding the same value of both tokens based on the current state of the liquidity pool which means 1 ETH for every 100 USDC with the current state of the pool.
‎
Let’s add another 100 ETH (10,000 USDC value) and 10,000 USDC to the pool.
‎
The new constant invariant can now be calculated as:
‎
(100 + 100) \* (10,000 + 10,000) = 4,000,000
‎
With this liquidity provided we have a deeper pool. Let’s try the 20 ETH buy swap again.
‎
4,000,000 = (200 - 20) \* x
x = 22,222
‎
It costs 22,222 - 20,000 = 2,222 $USDC. This translates to $111 / ETH price. As expected thanks to the deeper pool the price difference is smaller.
‎
By default liquidity providers get a small fee after each trade. On top of that with liquidity mining programs those LP tokens can get additional yield but there is risks involved as well.

### **Impermanent Loss (IL)**

There are some risks involved with LP’s. Besides the usual smart contract risk there is also impermanent loss.
‎
Impermanent loss occurs when you provide liquidity to a pool, and the price of your assets are different compared to when you deposited them. The bigger the change is, the more you are exposed to impermanent loss.

### **Impermanent loss calculations**

We will use the previous numbers for the calculation. You added 100 $ETH and 10.000 $USDC to the pool. That represents 50% of the pool.
‎
In this example we assume while $ETH goes up to $400, the liquidity remains constant in the pool (k = 4,000,000). While this is happening, arbitrageurs will add $ETH to the pool and take $USD (selling $ETH to the pool) from it until the ratio reflects the current price. As we learned earlier the price of the assets in the pool is determined by their ratio.
‎
Let's calculate the number of $ETH and $USDC coins in the pool.
‎
4,000,000 = x \* 400x, where x is the number of $ETH's.
10,000 = x^2
x = 100 (number of $ETH coins in the pool)
‎
Now we have 100 $ETH and 40,000 $USDC in the pool.
‎
If you take your money out (50% of the pool) you will get 50 $ETH and 20,000 $USDC. That’s worth 40,000 $USDC at $400/ETH price. If you had decided just to hold onto those asset instead, you would have 100 $ETH and 10,000 $USDC which is 50,000 $USDC.
‎
As you see you just lost 20% of your money thanks to IL.

### **Considerations**

‎Providing liquidity on safer pairs like $ETH-$USDC should be fine as the price of $ETH doesn't change that fast. Also consider if the pool belongs to a well established or to a new product.

If you decide to to LP-ing for small cap coins then you have to actively manage your positions as the token prices can change quickly and you could lose a lot of money thanks to impermanent loss.

With small size LP-ing is usually not a good idea as gas can be expensive compared to the yields. Always calculate your expected returns upfront.

In case of liquidity mining programs (extra incentive to bring in users), the yield can be high for a shorter period of time and it might be a good idea to do LP-ing. If you decide to do this you have to actively manage your positions and know that your are also exposed to smart contract risks.
### **Pair examples**

**‎$USDC - $USDT**

This is super safe as they are two large cap stables. You won't suffer IL as long as they keep the peg. Since it's super safe you should expect much lower returns. Unless there is some insane liquidity mining program this is usually a game for whales.

**$ETH - $USDC**

One token is a well established stable and the other is the second largest cap. Both of them are safe but $ETH price is expected to change over time. If your timeline is weeks then this should be fine. Larger returns than the previous one but still super small. If your size is little then it's likely not worth doing it.

**$FXS - $USDC**

A promising top100 coin and a stable. $FXS price can be volatile but it's still a large cap, so most likely you won't suffer IL if you pay attention. Yields can be large enough to consider doing it even with smaller size. If you decide to do this then you will have to keep an eye on your position.

**$FXS - $ETH**

Almost the same like the previous. Since $ETH is not too volatile it doesn't make a big difference compared to $USDC if you actively manage your position. Also if $ETH goes down a lot then $FXS will as well.

**$XYZ - $ETH/$USDC**

I don't recommend you doing smaller cap coins. It's much riskier and you have to super actively manage your position, plus you have to have a perfect understanding of what's going on. Only for experienced DeFi degenz.



## References
<!-- Links to pages not referenced in the content -->
-[[Decentralized]]