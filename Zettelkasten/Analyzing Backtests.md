
### Backtesting Review

In this section you're going to go back and critically evaluate your backtesting performance.

Common mistakes/ biases that affect traders are:

- Hindsight bias *
- Allowing winners to run beyond your TP
- Ignoring losers
- Changing your rules during testing *
- Data snooping (relevant later)
- Look ahead bias *
- Missing trades *

**Problem of mine = *

#### Can't Ignore losers

- Then you're just **wasting time**
- the **data is not accurate**

### Backtesting Weaknesses

Backtesting is fantastic when used as the tool it is supposed to be.

But it is just that, a tool.

Here are the main weaknesses in Backtesting that you must be aware of

- Doesn't account for Market impact (slippage)
- Doesn't account for Transaction costs (fees)

![[Pasted image 20240212020131.png]]

#### Never waste time live testing a system with negative expectancy in backtesting



## Win Rate

Now we begin the process of crunching your numbers from Backtesting.

To do this we will look at some statistics & probabilities. I cannot stress enough how important these next 3 lessons are for you as a trader. 

If you "don't like" mathematics, learn to like it. Or be a loser, whichever you prefer 😄 

I'm deadly serious, a solid understanding of basic probabilistic maths is essential. 

We start with Win Rate. Nice and simple.

Watch now!

#### Win rate = % of Winning Trades out of Total # of Trades

(Number of Winning Trades/ Total Number of Trades) x 100

this is NOT enough!

Win rate is a vanity metric

Many profitable Traders have <50% Win Rates


## Risk Reward

Having a high Win Rate is great, but it's nothing without also knowing how much you stand to win each time you're right.

#### Risk Reward = How much profit (reward) you make in return for 1 unit of potential losses (risk)

Units not $ amount

Essential for calculating the profitability of your systems

Also a great mental model for life

#### Example

I risk $100 to make $300

I risk $1000 to make $3000

**Both are +3R (1 risk = reward)**

## Expected Value

Now you understand Win Rate and Risk Reward, we move on to the single most important piece of statistical analysis you can do as a trader.

Expected Value.

Expected Value (or EV) is a formula that tells you in simple terms whether something is worth doing. 

If you get a positive number, it's called positive expectancy. That means if you take the same trade setup a large number of times, you should expect to make money on average. This is HUGE.

If you get a negative number, it's called negative expectancy. That means if you take the same trade setup a large number of times, you should expect to make lose on average. This is also very important, as it shows us systems and trades we wish to avoid.

### EV = Risk, Reward & Probability

**EV = P(W) x Reward - P(L) x Risk **

P() = Probability of 

#### Coin Toss Example: 

60% Heads

40% Tails

Double your money if right

**Heads**

EV = (0.6 x 1) - (0.4 x 1) = 0.2

AKA Positive Expentancy

**Tails**

EV = (0.4 x 1) - (0.6 x 1) = -0.2

AKA Negative Expentancy

### You must collect data 

Take 100 trades, journal them and track your Risk, Reward & Probability

## References
<!-- Links to pages not referenced in the content -->
-[[Trading]] 
