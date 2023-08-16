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


| **Table 1**      |        |             |   | **( 1 )**              | **(Fixed Supply, Free Market Price)** |                  |   | **( 2 )**              | **(Monthly Adjusted Supply, Free Market Price)** |                  |   | **( 3 )**              | **(Market Adjusted Supply, Fixed Price)** |                  |
|---------------|--------|-------------|---|--------------------|-------------------------------------|------------------|---|--------------------|------------------------------------------------|------------------|---|--------------------|-----------------------------------------|------------------|
| **Month**        | **Demand** | **Revenue**     |   | **FUEL units (fixed)** | **Unit Price (avg)**                    | **Average % Change** |   | **FUEL units (fixed)** | **Unit Price (avg)**                               | **Average % Change** |   | **FUEL units (fixed)** | **Unit Price (avg)**                        | **Average % Change** |
| Day 1         | 0%     | $100.00     |   | 100                | **$1.00**                               | 0.0%             |   | 100                | **$1.00**                                         | 0.0%             |   | 100                | **$1.00**                                   | 0.0%             |
| January       | 5%     | $105.00     |   | 100                | **$1.05**                               | 5.0%             |   | 103                | **$1.02**                                          | 2.4%             |   | 105                | **$1.00**                                   | 0.0%             |
| February      | 6%     | $111.30     |   | 100                | **$1.11**                               | 6.0%             |   | 106                | **$1.05**                                          | 2.9%             |   | 111                | **$1.00**                                   | 0.0%             |
| March         | 10%    | $122.43     |   | 100                | **$1.22**                               | 10.0%            |   | 111                | **$1.10**                                          | 4.8%             |   | 122                | **$1.00**                                   | 0.0%             |
| April         | 12%    | $137.12     |   | 100                | **$1.37**                              | 12.0%            |   | 118                | **$1.17**                                          | 5.7%             |   | 137                | **$1.00**                                   | 0.0%             |
| May           | -5%    | $130.27     |   | 100                | **$1.30**                               | -5.0%            |   | 115                | **$1.14**                                          | -2.6%            |   | 130                | **$1.00**                                   | 0.0%             |
| June          | -4%    | $125.05     |   | 100                | **$1.25**                               | -4.0%            |   | 112                | **$1.11**                                          | -2.0%            |   | 125                | **$1.00**                                   | 0.0%             |
| July          | 15%    | $143.81     |   | 100                | **$1.44**                               | 15.0%            |   | 121                | **$1.19**                                          | 7.0%             |   | 144                | **$1.00**                                   | 0.0%             |
| August        | 20%    | $172.58     |   | 100                | **$1.73**                               | 20.0%            |   | 133                | **$1.30**                                          | 9.1%             |   | 173                | **$1.00**                                   | 0.0%             |
| September     | -15%   | $146.69     |   | 100                | **$1.47**                               | -15.0%           |   | 123                | **$1.19**                                         | -8.1%            |   | 147                | **$1.00**                                   | 0.0%             |
| October       | -16%   | $123.22     |   | 100                | **$1.23**                               | -16.0%           |   | 113                | **$1.09**                                          | -8.7%            |   | 123                | **$1.00**                                   | 0.0%             |
| November      | -20%   | $98.58      |   | 100                | **$0.99**                               | -20.0%           |   | 102                | **$0.97**                                          | -11.1%           |   | 99                 | **$1.00**                                   | 0.0%             |
| December      | -22%   | $76.89      |   | 100                | **$0.77**                               | -22.0%           |   | 91                 | **$0.85**                                          | -12.4%           |   | 77                 | **$1.00**                                   | 0.0%             |
|  | **Total Travels**       | **$1,592.93** |   | **1300**               |                                |  **82%**                 |   | **1445**               |                                            |  **91%**                |   | **1593**               |                                    |  **100%**                |




**Table 1: Overview of the application of the three projected models: Free market, Monthly Adjusted Supply and Fixed Price.** 
The average pricings of fuel units with randomly chosen demand is set out over a period of one year. The first model reflects the demand in its pricing one-to-one. The second model takes the average demand change of each previous month and divides it over both the fuel production and pricing. The last model changes the amount of fuel produced based on the demand.

You’ll see that the model this IIP proposes (2.) is the best of both worlds. It reduces the volatility compared to (1.), but unlike (3.) allows for the market to price fuel. Reducing the volatility will make prices more stable for OW players to adjust to.

**Practicality:**

**Bullish Month:** In months June to July the revenue increases by 15%, in a fixed fuel model this might mean the price moves from $1.25 to $1.44 (15% change), but in an adjusted model, in the same situation might mean the price moves from $1.11 to $1.19 (7% change)

**Bearish Month:** In months August to September the revenue decreases by 15%, in a fixed fuel model this might mean the price moves from $1.73 to $1.47 (-15% change), but in an adjusted model, in the same situation might mean the price moves from $1.30 to $1.19 (-8.7% change)


|               |        |             |   | **( 1 )**              | **(Fixed Supply, Free Market Price)** |                  |   | **( 2 )**              | **(Monthly Adjusted Supply, Free Market Price)** |                  |   | **( 3 )**              | **(Market Adjusted Supply, Fixed Price)** |                  |
|---------------|--------|-------------|---|--------------------|-------------------------------------|------------------|---|--------------------|------------------------------------------------|------------------|---|--------------------|-----------------------------------------|------------------|
| **Month**         | **Demand** | **Revenue**    |   | **FUEL units (fixed)** | **Unit Price (avg)**                    | **Average % Change** |   | **FUEL units (fixed)** | **Unit Price (avg)**                               | **Average % Change** |   | **FUEL units (fixed)** | **Unit Price (avg)**                       | **Average % Change** |
| Day 1         | 0%     | $100.00     |   | 100                | **$1.00**                               | 0.0%             |   | 100.0              | **$1.00**                                          | 0.0%             |   | 100.0              | **$1.00**                                   | 0.0%             |
| January       | 20%    | $120.00     |   | 100                | **$1.20**                               | 20.0%            |   | 110.0              | **$1.09**                                          | 9.1%             |   | 120.0              | **$1.00**                                  | 0.0%             |
| February      | 20%    | $144.00     |   | 100                | **$1.44**                               | 20.0%            |   | 121.0              | **$1.19**                                          | 9.1%             |   | 144.0              | **$1.00**                                   | 0.0%             |
| March         | 20%    | $172.80     |   | 100                | **$1.73**                               | 20.0%            |   | 133.1              | **$1.30**                                          | 9.1%             |   | 172.8              | **$1.00**                                   | 0.0%             |
| April         | 20%    | $207.36     |   | 100                | **$2.07**                               | 20.0%            |   | 146.4              | **$1.42**                                          | 9.1%             |   | 207.4              | **$1.00**                                  | 0.0%             |
| May           | 20%    | $248.83     |   | 100                | **$2.49**                               | 20.0%            |   | 161.1              | **$1.55**                                          | 9.1%             |   | 248.8              | **$1.00**                                   | 0.0%             |
| June          | 20%    | $298.60     |   | 100                | **$2.99**                               | 20.0%            |   | 177.2              | **$1.69**                                          | 9.1%             |   | 298.6              | **$1.00**                                  | 0.0%             |
| July          | 20%    | $358.32     |   | 100                | **$3.58**                               | 20.0%            |   | 194.9              | **$1.84**                                          | 9.1%             |   | 358.3              | **$1.00**                                  | 0.0%             |
| August        | 20%    | $429.98     |   | 100                | **$4.30**                               | 20.0%            |   | 214.4              | **$2.01**                                          | 9.1%             |   | 430.0              | **$1.00**                                   | 0.0%             |
| September     | 20%    | $515.98     |   | 100                | **$5.16**                               | 20.0%            |   | 235.8              | **$2.19**                                          | 9.1%             |   | 516.0              | **$1.00**                                   | 0.0%             |
| October       | 20%    | $619.17     |   | 100                | **$6.19**                               | 20.0%            |   | 259.4              | **$2.39**                                          | 9.1%             |   | 619.2              | **$1.00**                                   | 0.0%             |
| November      | 20%    | $743.01     |   | 100                | **$7.43**                               | 20.0%            |   | 285.3              | **$2.60**                                          | 9.1%             |   | 743.0              | **$1.00**                                  | 0.0%             |
| December      | 20%    | $891.61     |   | 100                | **$8.92**                               | 20.0%            |   | 313.8              | **$2.84**                                          | 9.1%             |   | 891.6              | **$1.00**                                   | 0.0%             |
|  |  **Total Travels**      | **$4,849.66**|   | **1300**               |                                     | **27%**              |   | **2452.3**             |                                                | **51%**              |   | **4849.7**             |                                         | **100%**            |



**Extreme Bullish Year:** Month over month production will be increased to off-set the pricing of each fuel type acting as a lasso to pull the prices back down. After a year where demand increases 20% month over month, in model (1) the price will be up 892% whereas in model (2) the price will be up 284%.


|           |               |         |   | **( 1 )**             | **(Fixed Supply, Free Market Price)** |                  |   | **( 2 )**              | **(Monthly Adjusted Supply, Free Market Price)** |                  |   | **( 3 )**              | **(Market Adjusted Supply, Fixed Price)** |                  |
|-----------|---------------|---------|---|--------------------|-------------------------------------|------------------|---|--------------------|------------------------------------------------|------------------|---|--------------------|-----------------------------------------|------------------|
| **Month**     | **Demand**        | **Revenue** |   | **FUEL units (fixed)** | **Unit Price (avg)**                    | **Average % Change** |   | **FUEL units (fixed)** | **Unit Price (avg)**                               | **Average % Change** |   | **FUEL units (fixed)** | **Unit Price (avg)**                       | **Average % Change** |
| Day 1     | 0%            | $100.00 |   | 100                | **$1.00**                               | 0.0%             |   | 100.0              | **$1.00**                                         | 0.0%             |   | 100.0              | **$1.00**                                   | 0.0%             |
| January   | -20%          | $80.00  |   | 100                | **$0.80**                               | -20.0%           |   | 90.0               | **$0.89**                                          | -11.1%           |   | 80.0               | **$1.00**                                   | 0.0%             |
| February  | -20%          | $64.00  |   | 100                | **$0.64**                               | -20.0%           |   | 81.0               | **$0.79**                                          | -11.1%           |   | 64.0               | **$1.00**                                   | 0.0%             |
| March     | -20%          | $51.20  |   | 100                | **$0.51**                               | -20.0%           |   | 72.9               | **$0.70**                                          | -11.1%           |   | 51.2               | **$1.00**                                   | 0.0%             |
| April     | -20%          | $40.96  |   | 100                | **$0.41**                               | -20.0%           |   | 65.6               | **$0.62**                                          | -11.1%           |   | 41.0               | **$1.00**                                   | 0.0%             |
| May       | -20%          | $32.77  |   | 100                | **$0.33**                               | -20.0%           |   | 59.0               | **$0.55**                                          | -11.1%           |   | 32.8               | **$1.00**                                   | 0.0%             |
| June      | -20%          | $26.21  |   | 100                | **$0.26**                               | -20.0%           |   | 53.1               | **$0.49**                                          | -11.1%           |   | 26.2               | **$1.00**                                   | 0.0%             |
| July      | -20%          | $20.97  |   | 100                | **$0.21**                               | -20.0%           |   | 47.8               | **$0.44**                                          | -11.1%           |   | 21.0               | **$1.00**                                   | 0.0%             |
| August    | -20%          | $16.78  |   | 100                | **$0.17**                               | -20.0%           |   | 43.0               | **$0.39**                                          | -11.1%           |   | 16.8               | **$1.00**                                   | 0.0%             |
| September | -20%          | $13.42  |   | 100                | **$0.13**                               | -20.0%           |   | 38.7               | **$0.35**                                          | -11.1%           |   | 13.4               | **$1.00**                                   | 0.0%             |
| October   | -20%          | $10.74  |   | 100                | **$0.11**                               | -20.0%           |   | 34.9               | **$0.31**                                          | -11.1%           |   | 10.7               | **$1.00**                                   | 0.0%             |
| November  | -20%          | $8.59   |   | 100                | **$0.09**                               | -20.0%           |   | 31.4               | **$0.27**                                          | -11.1%           |   | 8.6                | **$1.00**                                   | 0.0%             |
| December  | -20%          | $6.87   |   | 100                | **$0.07**                               | -20.0%           |   | 28.2               | **$0.24**                                          | -11.1%           |   | 6.9                | **$1.00**                                   | 0.0%             |
|           | **Total Travels** | **$472.51** |   | **1300**               |                                     | **275%**             |   | **745.8**              |                                                | **158%**            |   | **472.5**             |                                         | **100%**             |



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

