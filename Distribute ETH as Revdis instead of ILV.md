Simple Summary
Distribute $ETH directly as Revenue Distribution to $ILV Stakers instead of converting them to $ILV before Distribution.

Abstract
Swapping $ETH to $ILV by TWAP via Sushiswap is very inefficient and does not primarily benefit $ILV Stakers. It only benefits large sellers looking to get exit liquidity.

Overview
By swapping all $ETH to $ILV you basically create exit liquidity to large investors that can snipe these TWAP buys. TWAP, stands for Time-weighted average price. It bascially means that every 5 minutes, hour, or any other arbitrary time interval there will be a transaction executed. That’s how the protocol would most likely buy ILV from the market with its ETH revenue. Here an example:

Illuvium Landsale Revenue: 4000 ETH
TWAP Buy ILV: Swap 10 ETH to ILV every hour. 
Result: After 400 hours the algorithm swapped all 4000 ETH to ILV without spiking the price in one big swap.

How does this system give exit liquidity to large ILV investors that want to sell?
As Ethereum is an open blockchain you can see all incoming transactions in the mempool. These are transactions that are waiting to be included in a block. As a large holder wanting to sell, I will watch transactions to the ETH/ILV Sushiswap pool (programmatically with a bot, now physically). 

Once an ETH-to-ILV transaction comes in I will spot it in the mempool and immediately broadcast my ILV-to-ETH transaction. More sophisticated investors will implement this via Eden Network or Private Broadcasting Offerings from Mining pools to execute the sell ILV transaction exactly in the same block as the ETH-to-ILV transaction without even appearing in the mempool.
So you basically only provide exit liquidity to big investors that want to exit ILV at favorable conditions.


One might think: But these guys would sell anyway and therefore tank the price, right? So why distribute ETH to stakers?

Absolutely, that might happen, but then the big seller actually loses out on those sells, as they do not have the exit liquidity and push prices lower, making less money selling their ILV than with the TWAP liquidity. If ETH instead of ILV gets distributed to stakers, then, at lower prices, the ETH distributed to stakers could buy a staker more ILV with his distributed ETH as the stakers profits from the liquidity shock caused by a large investor selling and pushing the price down.

Some might think that RevDis in ILV will actually "pump" the price of ILV. Nothing is further from the truth. Swapping ETH to ILV just creates inefficiencies and cost, especially on smaller stakers. In the best case scenario buying ILV with ETH just defers an ILV sell event to the date where ILV gets distributed to stakers.

Here another example with some pictures:


This is what an order book looks like for ILV right now:

https://imgur.com/a/aOA9AHE


This is what the orderbook looks like after the Protocol would set a buy order (This would be a limit order, whereas the protocol actually would send a market order via sushiswap, but as blocks take time to be mined and the transaction will be visible in the mempool, the onchain swap is equal to a limit order for large sellers:

https://imgur.com/a/0NwLvnb

In this case the buy order would have been for 10 ILV at a price of 279.5 USDT. A large seller would now snipe this limit order and sell exactly 10 ILV into it and then wait for the next 10 ILV bid and repeat this process until the protocol runs out of ETH or the seller runs out of ILV. This would not pump the price at all. The price would remain the same until the sellers run out of ILV.




Rationale

What's the advantage for distributing ETH directly to stakers instead of ILV?
1. ETH is the gold standard currency for NFTs and would make ILV as an asset even more desirable for investors.

2. You actually punish large sellers if they want to exit into low liquidity and reward stakers that want to buy ILV with their ETH received from RevDis.

3. You actually create a REAL buy pressure event as stakers who want to buy more ILV with ETH distributed from RevDis create REAL demand and inflows. Instead of a large sell event once ILV RevDis gets distributed you create a buy event once ETH gets distributed. 

4. There is a lot of inefficiency involved in swapping ETH to ILV and then back to ETH for stakers that just want to sell their RevDis.

5. Large sellers are forced to sell at a lower price and give long-term believers the chance to profit off of this sell pressure instead of giving the large seller good exit liquidity.

6. There is no real good reason to distribute ILV as RevDis. The only one I can think of is to trap small stakers for whom it is not worth it to claim ILV, so less sell pressure?

Test Cases
N/A

Copyright
Copyright and related rights waived via CC0.
