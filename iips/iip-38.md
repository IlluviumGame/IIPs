---
iip: 38
title: Free Market Fuel with Autonomous Supply Balancing
status: Withdrawn
sponsor: Nijafe
discussions-to: https://discord.gg/illuvium
created: 2023-08-20
---

## Simple Summary
Fuel plays a pivotal role in the thriving Illuvium ecosystem, and this proposal aims to provide a detailed insight into its various aspects:
  
- Fuel Tokenomics: Attributes of ERC20 Fuel tokens (Crypton, Solon, Hyperion).
- Fuel Production: Exclusively through player engagement with NFT land.
- Utilization of Fuel: Diverse in-game actions.
- Fuel Market Transactions: Order book system for fair buying/selling (Market/Limit).
- Price Stabilization: Innovative approach adjusting production based on demand.

## Overview

### Fuel Economy
- In the Illuvium Zero ecosystem, three types of ERC20 Fuels (Crypton, Solon, and Hyperion) will operate independently, each serving different in-game actions, with some actions allowing any Fuel type to be used.
- NFT land owners will receive a 5% share of all in-game purchases (excluding transactions involving sILV2).
- When possible, in-game purchases will be priced in Fuel.
- For purchases not priced in Fuel, 5% of the total amount will still be distributed to land ownersthrough alternative means.
### Fuel Supply
- Fuel production solely occurs when players engage with Illuvium Zero using NFT land.
- The supply of Fuel is unlimited, allowing players to continually participate in the in-game economy.
- However, each time Fuel is used for in-game purchases, it is effectively burned, maintaining a balance between supply and demand.

### Buying and Selling Fuel
- An order book system facilitates the buying and selling of Fuel.
- Players can either sell Fuel at the prevailing "Market" value or set a specific price using a "Limit" order.
- Whenever any type of Fuel is sold, the DAO will mint 19x the Fuel amount, combining the Fuel from the land owner and DAO to be transferred to the purchaser.
With this enhanced framework, Illuvium Zero can thrive as a vibrant and sustainable gaming ecosystem. The independent functionality of each Fuel type, coupled with the fair distribution of revenue to NFT land owners, ensures a balanced and dynamic in-game economy. Additionally, the flexible approach to pricing in Fuel or alternative means allows for smooth and transparent transactions, contributing to an enjoyable gaming experience for all participants.

### Price Stabilization Mechanism for Fuel Production
To perpetuate price stability and prevent fluctuations of magnitude, we propose a predictable and decentralized approach for adjusting Fuel production based on demand, significantly reducing the need for rails:
- In-game purchases will be priced in units of Fuel
- Supply Adjustments: Production of each Fuel type is adjusted in direct correlation with the change in demand from the previous month. If the demand changed X% for that month, fuel production adjusts to (X/2)% for the following month.
- Community-Friendly Approach: Unlike centralized entities, which often face community pushback when abruptly changing supply, our decentralized and market-driven method ensures a more acceptable adjustment process.
- Predictable Nature: Land owners can proactively plan for monthly adjustments as they are front selling these changes, further contributing to price stability.
- Free Market Influence: While supply adjustments help in maintaining stability, the free market remains the ultimate determinant of Fuel prices.
By adopting this refined mechanism, we can foster a more stable Fuel market while allowing market forces to naturally govern price fluctuations. This approach is particularly beneficial for web3 gaming, where community satisfaction is paramount.

## Discussion

1. Fixed Supply, Free Market Price
2. Monthly Demand Adjusted Supply, Free Market Price (This Proposal)
3. Market Adjusted Supply, Fixed/pegged Price

(1) Fixed Supply, Free Market Price
Pros:
- Easier to Implement: Requires less resources to implement.
Cons:
- Extreme Price Volatility: Could negatively impact players of the OW.
- Rails: Due to the volatile nature of an open market, there is a need for a rails system to prevent prices from getting out of control.
- Centralization: With no mechanism to stabilize prices, developers/DAO may need to step in more often to make adjustments. There may be adjustments to fuel production masked as “content updates” (e.g. “A new structure will be introduced next week that will increase fuel production”).
- Unpredictability: Changes in game mechanics or pricing can come at any time with announcements that may negatively affect the value of your fuel.

(3) Market Adjusted Supply, Fixed/pegged Price
Pros:
- Buyers Certainty: Buyers always know what they need to pay for that in-game experience
Cons:
- Less Agency for Land Owners: Removes meta-game as land owners will have no reason to sell fuel aside from maxing out storage capacity. Will not affect buyers prices.
