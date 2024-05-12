
## Questions

- How to know when false breakout to the opposite side matters or not. I.e there is a clean box but there is one candle that dumps out of the box and reverses back right away

## Terms



## Optimal Rules:

#### Setup:

- Strong Breakout, 50 over 100 EMA, both sloping upwards (if 100 EMA exists)
- Box needs to be H1-H8
- 12/21 Bands flip red, green, red. green (atleast 2 candles to confirm flip)
- Support tested 3 times and resistance tested 2 times (separate)  (wick is enough), Use fibonacci tools 25/75 premium and discount zones.
  (Order of is sup or res tested first doesnt matter)
  

- **Entry**: When price breaks out, falls back to traps inside, breaks out again 
- **Take Profit**: When 12/21 Bands flip red on the same time frame, first candle after flip (if under 1R, don't take profit)
- **Stop Loss**: Little under 50 EMA


#### Extra rules:

- Timeframe needs to be the one with the most stable ema/most tightly box, even if there is a setup on slighly less stable
- Dont count flush wicks as support area bottoms
- ~~Box bottom needs to be above 50 fib level  meaning that price cant pull back more than 50%~~
- ~~on the time frame of the box, the impulse is confirmed by Ema sloping upwards~~
  
  Example
### Test:

1. Wick inside box counts as entry (Must be better than close)
- Only two test of R/S
- Can box still be traded if there was an entry that failed due to being a false breakout
Example:
![[Pasted image 20240505025354.png]]

- wick above or below counts as reset of test meaning that price doesnt need to close across ema to count the next test of 75/25 S/R area 
- 3 or 4 tests of resistance
- How big of a difference is there for trading with time period (i.e 10 am - 10 pm) vs no time period (247)
- Volume to confluence the pump before box
- take profit on the same time frame of box
- take profit only if bands are red and they point down
- If bands flip red, look if next HTF trend is still intact
- Exit on first or second candle of bands flip
- wait for 50 ema to be above 100 or count when they are just about to cross (the so count the first impulse leg of a trend) Example:
![[Pasted image 20240505022450.png]]
- Box bottom needs to be above 50 fib level  meaning that price cant pull back more than 50%
Example:

![[Pasted image 20240505023212.png]]

- Dont count flush wicks as support area bottoms
Example:

![[Pasted image 20240505023254.png]]

Example of false flip red, 90R to 170R!

![[Pasted image 20240430222236.png]]


### Problems: 

This one here is the first box before bull run of 2021, find a way to be part of this (maybe 3 support tests and only 2 resistance tests)

![[Pasted image 20240430024727.png]]

IT would get 170R if dont count 12/21 red flip of two candles (bands werent moving down but sideways)

![[Pasted image 20240430025126.png]]

## Weird Excemptions

- Price tested resistance twice but rules say only ones as price didnt fall below EMA after second test so not valid

![[Pasted image 20240505194201.png]]
this exception missed a huge pump:

![[Pasted image 20240505194504.png]]
Example 2 of same exception:

![[Pasted image 20240505201959.png]]






### Come up with a rule that makes it possible to ignore these long wicks 

![[Pasted image 20240507215121.png]]


#### Can this count as test of support

![[Pasted image 20240507215350.png]]




### What to do it this scenario:

- Where on 2H TF the ema is "too volatile" (dont have a rule or metric yet) but there is a valid setup but on better TFs there is no setup

### 2H:

![[Pasted image 20240507215855.png]]

### 3H: (only 2 test of support)

![[Pasted image 20240507215958.png]]


- Maybe go always go the the one where price is the most packed around the price? (measure on 3 spots to find which one on average is closest)


### For the test of levels: 

- Maybe price should close above/below 50 EMA and stay there for atleast ex. 3 candles before moving to 25/75 can count as another test of S/R

Example: where price does not stay above it :

![[Pasted image 20240507220816.png]]

## Upgraded rules

- 50 over 100 EMA:  
     - (if they exists, might not on new tokens)
     - both sloping upwards
- Strong breakout: 
     - BOS/MSB with above MA volume on breakout (on 1+ bullish candles after breakout level)
     - momentum candle after the breakout level = 3 smaller bullish candler or single large candle (compared to other candles around it)) 
     - Why momentum candle? => because price needs to be impulsive and not just grind up 
- Box formation:
     - Valid box can only form on H1-H8
     - Timeframe is chosen before entry setup happens, on timeframe that has the best ratio of least volatile/most packed 50 EMA
     - 50 EMA needs to be in the middle of the price action for atleast one cross = price is packed around EMA
     - Box low is counted from the lowest wick below 50 EMA
     - Box low can't be below breakout level
- Price needs to test S/R 25/75 zones 2 & 3 separate times:
     - 2 for Resistance & 3 for support
     - Support needs to be tested first before resistance can be tested
     - (wick is enough) 
     - (separate = price need to close back above/below ema before it can test again)
- 12/21 Bands flip red, green, red. green 
     - (atleast 2 candles to confirm flip) 

Extra rules:

- Only one trade can be open at a time (for all tokens as market usually moves as a whole)

- **Entry**: When price breaks out, falls back to traps inside (wick or close), breaks out again (bullish candle close above box high) 
- **Stop Loss**: under 50 EMA
- **Take Profit**: When 12/21 Bands flip red on Daily timeframe


## Questions/Thoughts

- Should breakout level be counted from the candle close or the wick 

- It seems that the impulse move might need more volume than just slightly above MA on a single candle to high prob continuation move

- Maybe tests cant happen back to back so it avoids patterns like this:

![[Pasted image 20240511224222.png]]

- Is this a valid box when before hand there was another box? There was a slight impulsive breakout after the first box but price retraced fully after it

![[Pasted image 20240511214218.png]]

- Make a rule that "before the first valid test, EMA needs to already be stable"
  -> this way we avoid setups like this where box is premature:

![[Pasted image 20240511225021.png]]

![[Pasted image 20240511225159.png]]



## References
<!-- Links to pages not referenced in the content -->
-[[Trading]]
