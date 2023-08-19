---
iip: 38
title: Free Market Fuel with Autonomous Supply Balancing
status: Pending
author: Nick (Nijafe_Plays)
discussions-to: https://discord.gg/illuvium
created: 7-26-2023
---

## Simple Summary:
Fuel plays a pivotal role in the thriving Illuvium ecosystem, and this proposal aims to provide a detailed insight into its various aspects:
- Fuel Tokenomics: Attributes of ERC20 Fuel tokens (Crypton, Solon, Hyperion).
- Fuel Production: Exclusively through player engagement with NFT land.
- Utilization of Fuel: Diverse in-game actions.
- Fuel Market Transactions: Order book system for fair buying/selling (Market/Limit).
- Price Stabilization: Innovative approach adjusting production based on demand.

## **[Full Proposal linked here](https://github.com/Rickytan77/IIPs/blob/master/assets/IIP-38%20-%20Free%20Market%20Fuel%20with%20Autonomous%20Supply%20Balancing/Fuel_IIP38_Nijafe.pdf)**
  

## Overview of Fuel Economy:
- In the Illuvium Zero ecosystem, three types of ERC20 Fuels (Crypton, Solon, and Hyperion) will operate independently, each serving different in-game actions, with some actions allowing any Fuel type to be used.
- NFT land owners will receive a 5% share of all in-game purchases (excluding transactions involving sILV2).
- When possible, in-game purchases will be priced in Fuel.
- For purchases not priced in Fuel, 5% of the total amount will still be distributed to land ownersthrough alternative means.


**Fuel Supply:**
- Fuel production solely occurs when players engage with Illuvium Zero using NFT land.
- The supply of Fuel is unlimited, allowing players to continually participate in the in-game economy.
- However, each time Fuel is used for in-game purchases, it is effectively burned, maintaining a balance between supply and demand.


**Buying and Selling Fuel:**
- An order book system facilitates the buying and selling of Fuel.
- Players can either sell Fuel at the prevailing "Market" value or set a specific price using a "Limit" order.
- Whenever any type of Fuel is sold, the DAO will mint 19x the Fuel amount, combining the Fuel from the land owner and DAO to be transferred to the purchaser.


With this enhanced framework, Illuvium Zero can thrive as a vibrant and sustainable gaming ecosystem. The independent functionality of each Fuel type, coupled with the fair distribution of revenue to NFT land owners, ensures a balanced and dynamic in-game economy. Additionally, the flexible approach to pricing in Fuel or alternative means allows for smooth and transparent transactions, contributing to an enjoyable gaming experience for all participants.


## Price Stabilization Mechanism for Fuel Production:

To perpetuate price stability and prevent fluctuations of magnitude, we propose a predictable and decentralized approach for adjusting Fuel production based on demand, significantly reducing the need for rails:

- In-game purchases will be priced in units of Fuel
- Supply Adjustments: Production of each Fuel type is adjusted in direct correlation with the change in demand from the previous month. If the demand changed X% for that month, fuel production adjusts to (X/2)% for the following month.
- Community-Friendly Approach: Unlike centralized entities, which often face community pushback when abruptly changing supply, our decentralized and market-driven method ensures a more acceptable adjustment process.
- Predictable Nature: Land owners can proactively plan for monthly adjustments as they are front selling these changes, further contributing to price stability.
- Free Market Influence: While supply adjustments help in maintaining stability, the free market remains the ultimate determinant of Fuel prices.
  
By adopting this refined mechanism, we can foster a more stable Fuel market while allowing market forces to naturally govern price fluctuations. This approach is particularly beneficial for web3 gaming, where community satisfaction is paramount.


## Discussion: 

This chart compares 3 of the most reasonable models
1. Fixed Supply, Free Market Price
2. Monthly Demand Adjusted Supply, Free Market Price (This Proposal)
3. Market Adjusted Supply, Fixed/pegged Price


**(1) Fixed Supply, Free Market Price**

**Pros:**

- **Easier to Implement:** Requires less resources to implement.

**Cons:**

- **Extreme Price Volatility:** Could negatively impact players of the OW.

- **Rails:** Due to the volatile nature of an open market, there is a need for a rails system to prevent prices from getting out of control.

- **Centralization:** With no mechanism to stabilize prices, developers/DAO may need to step in more often to make adjustments. There may be adjustments to fuel production masked as “content updates” (e.g. “A new structure will be introduced next week that will increase fuel production”).

- **Unpredictability:** Changes in game mechanics or pricing can come at any time with announcements that may negatively affect the value of your fuel.


**(3) Market Adjusted Supply, Fixed/pegged Price**

**Pros:**

- **Buyers Certainty:** Buyers always know what they need to pay for that in-game experience

**Cons:**

- **Less Agency for Land Owners:** Removes meta-game as land owners will have no reason to sell fuel aside from maxing out storage capacity. Will not affect buyers prices.


## **Please refer to:**  **[Table 1](https://github.com/Rickytan77/IIPs/blob/master/assets/IIP-38%20-%20Free%20Market%20Fuel%20with%20Autonomous%20Supply%20Balancing/IIP-38%20-%20TABLE%201.pdf)**


**Table 1: Overview of the application of the three projected models: Free market, Monthly Adjusted Supply and Fixed Price.** 
The average pricings of fuel units with randomly chosen demand is set out over a period of one year. The first model reflects the demand in its pricing one-to-one. The second model takes the average demand change of each previous month and divides it over both the fuel production and pricing. The last model changes the amount of fuel produced based on the demand.

You’ll see that the model this IIP proposes (2.) is the best of both worlds. It reduces the volatility compared to (1.), but unlike (3.) allows for the market to price fuel. Reducing the volatility will make prices more stable for OW players to adjust to.

**Practicality:**

**Bullish Month:** In months June to July the revenue increases by 15%, in a fixed fuel model this might mean the price moves from $1.25 to $1.44 (15% change), but in an adjusted model, in the same situation might mean the price moves from $1.11 to $1.19 (7% change)

**Bearish Month:** In months August to September the revenue decreases by 15%, in a fixed fuel model this might mean the price moves from $1.73 to $1.47 (-15% change), but in an adjusted model, in the same situation might mean the price moves from $1.30 to $1.19 (-8.7% change)


## **Please refer to Table:**  **[Extreme Bullish Year](https://github.com/Rickytan77/IIPs/blob/master/assets/IIP-38%20-%20Free%20Market%20Fuel%20with%20Autonomous%20Supply%20Balancing/IIP-38%20-%20TABLE-%20EXTREME%20BULLISH%20YEAR.pdf)**

**Extreme Bullish Year:** Month over month production will be increased to off-set the pricing of each fuel type acting as a lasso to pull the prices back down. After a year where demand increases 20% month over month, in model (1) the price will be up 892% whereas in model (2) the price will be up 284%.


## **Please refer to Table:**  **[Extreme Bearish Year](https://github.com/Rickytan77/IIPs/blob/master/assets/IIP-38%20-%20Free%20Market%20Fuel%20with%20Autonomous%20Supply%20Balancing/IIP-38%20-%20TABLE-%20EXTREME%20BEARISH%20YEAR.pdf)**

**Extreme Bearish Year:** Month over month production will be decreased to off-set the pricing of each fuel type acting as a lasso to pull the prices back up. After a year where demand decreases 20% month over month, in model (1) the price will be down 93% whereas in model (2) the price will be down 76%.


Both of these first two models allow agency over their fuel and the impact it has on the price, but one is less volatile than the other.


## Conclusion:
The Illuvium fuel economy provides land owners with a multi factor meta-game to extract their share of the 5% of in-game purchases, requiring strategic choices and encourages a harmonious correlation between fuel types. These elements contribute to the richness of the Illuvium experience, making it more dynamic, engaging, and impactful for players and the
ecosystem alike.

It’s clear that if and when fuel prices need to be adjusted they will. The debate comes down to whether the community wants this to occur in a centralized or decentralized manner. This proposal model will make predictable automated adjustments to fuel supply, significantly reducing the likelihood of rails to be hit, the DAO needs to step in and make changes, or the need for developers to make production changes masked as “content updates.”


## Additional Features of the Illuvium Fuel Economy:
- Environmental Impact (Lore): The ecosystem acknowledges the environmental consequences of fuel usage. As more fuel is utilized, its concentration increases in the air through emissions. However, there's a silver lining—increased fuel concentration in the air benefits land owners, allowing for more efficient extraction from the atmosphere.
- Strategic Storage Options: When storage reaches maximum capacity, land owners have two choices: either sell the excess fuel to the market or send it to an overworld account as an ERC20 token.
- Fuel Type Correlation: Certain in-game purchases are open to being made with any fuel type, fostering a correlation between the prices of different fuels. For example, D1SKs can be priced in units of any fuel. If one fuel type, say Solon, becomes the lowest-priced, players will naturally lean towards using Solon for their D1SK purchases, putting pressure on it to align with other fuel types’ prices. This interdependence ensures a balanced and interconnected fuel market.
- Fuel should be transferable out of IZ storage into an OW account on the same or different wallet address.


## Test Cases
Real world Crude Oil. When demand goes up, production goes up, when demand softens, production is slowed.


## Sponsor:
Nick (Nijafe_Plays)

