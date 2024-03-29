---
iip: 20
title: Parameters for Illuvium: Zero Land Sale
status: Proposed
author: Aaron Warwick (kieran@illuvium.io)
discussions-to: https://discord.gg/illuvium
created: 2021-11-19
updated: 2022-03-05
---

## Simple Summary

Illuvium: Zero will soon be ready. Leading up to this, we must get approval
on the details of the Land Sale. Following this IIP will be the release of two additional guide documents. One describes Illuvium: Zero and the other explains how to purchase land. While not explicitly required for this IIP, they will give much-needed context in an easily digestible way.

## Abstract

A 3D isometric city building game is being developed using Unity and is getting closer to its Alpha release. Illuvium: Zero requires a land sale, which will mint the land players will use to play Illuvium: Zero. Illuvium will host the Land Sale in the IlluviDEX and mint the NFTs on IMX. It represents our largest web app to date.

## Overview

**Land Sale Timings**

|                            |            |
| -------------------------- | ---------- |
| **Total Duration Of Sale** | Three days |
| **Plot Sold Per Batch**    | 278 plots  |
| **Batch Release Date**     | 1 per hour |
| **Duration of Each Batch** | 2          |

Practically, approximately 278 new plots will go on sale every hour. At this point, they will start reducing in price until someone purchases them.
There is nothing needed to do for purchase besides selecting the plot and paying the price on display. If you wish to buy for a lower price, wait for
it to drop, but remember that another person can purchase the same plot as you.
Since tranches are released every hour, there may be some overlap. One tranche will be 1 hour old (approximately 30% of the starting price),
and the other will be brand new. Each batch will have roughly the same ratio of Tiers as the overall land numbers.

**Land NFT Numbers**
| | |
| -------------------------- | ---------- |
| **Total Land NFT plots** | 100000 |
| **Total plots available in the first sale** | 20000\* |
| **Tier 5 Land plots to be sold in the first sale** | 2 |
| **Tier 4 Land plots to be sold in the first sale** | 869 |
| **Tier 3 Land plots to be sold in the first sale** | 2088 |
| **Tier 2 Land plots to be sold in the first sale** | 5012 |
| **Tier 1 Land plots to be sold in the first sale** | 12029 |

Illuvium will reserve 25 (Tier 1) plots for giveaways during the landsale event and 4 plots (1 of each Tier, excluding Tier 5) for
live testing purposes and quality assurance.
**Land NFT Details**
Each plot of land will have limited details available before purchase as outlined below:

|              |                                                                                                            |
| ------------ | ---------------------------------------------------------------------------------------------------------- |
| **Region**   | There are 7 regions in total. Region affects the probability of Illuvial affinity scanned.                 |
| **Tier**     | There are 5 Tiers in total. Tier affects the number of element and fuel sites and the landmarks available. |
| **Location** | Location is only relevant for future expansions where adjacent land may be able to be merged.              |

Once purchased, the IMX will mint an NFT containing details of the land plot. We use a random seed to deterministically generate the site and landmark details that comprise the land plot.

The deterministic function that generates these details will be stored in the immutable blockchain contract and can be used to verify that applications like the Illuvium: Zero game client or the IlluviDEX web application honour the land generation function defined in the contract.

This function generates the following details:
| | |
|------------------- |------------------------------------------------------------------------------------------- |
| **Element Sites** | An array of Element Sites containing details of each site's type and location. |
| **Fuel Sites** | An array of Fuel Sites containing details of each site's type and location. |
| **Landmark** | The type of any generated Landmark. Empty for those Tiers which do not include Landmarks. |

**Number of Sites and Landmarks per Tier**

There are a fixed number of Sites and Landmarks per tier, but the type of these Sites and Landmarks can vary. For example, one Tier 1 site may have one of each Element Site or 3 Lakes.

Higher level Tiers have sites that are more resource rich. Accordingly each Tier above Tier 1 has a production boost which increases the amount of Fuel and Elements generated by the Sites on the Plot. The higher the Tier level the higher the production boost.

The following table defines the number of Element Sites, the number of Fuel Sites, the class of Landmark, and the Production Boost for each tier:

| **Land Tier** | **# of Element Sites** | **# of Fuel Sites** | **Number and type of Landmark** | **Production Boost** |
| ------------- | ---------------------- | ------------------- | ------------------------------- | -------------------- |
| Tier 1        | 3                      | 1                   | None. No landmark.              | 0%                   |
| Tier 2        | 6                      | 3                   | None. No landmark.              | 33.33%               |
| Tier 3        | 9                      | 6                   | 1 Element landmark.             | 100%                 |
| Tier 4        | 12                     | 9                   | 1 Fuel landmark.                | 300%                 |
| Tier 5        | 15                     | 12                  | 1 Arena.                        | 900%                 |

Quantities of sites are defined, meaning that all land of a particular tier will have the potential to produce just as much as any other land plot.

There will be minor differences due to:

- Variety and spread of sites
- Location of sites on the plot
- The synergy between sites and Landmark

We feel the slight randomness adds an element of excitement to the sale.

**Land NFT Pricing**
The land sale uses a declining price model, configured with a starting value that declines at 2.5% per minute\* for two hours.
| **Tier** | **Starting price in ETH** |
|:-------------------------------------------------: |:-------------------------: |
| Starting Price for Tier 5 Land Plot in First Sale | Live English Auction |
| Starting Price for Tier 4 Land Plot in First Sale | 80 |
| Starting Price for Tier 3 Land Plot in First Sale | 20 |
| Starting Price for Tier 2 Land Plot in First Sale | 6 |
| Starting Price for Tier 1 Land Plot in First Sale | 2 |

![Percentage](../assets/iip-20/land-percentage-time.png)

**Tier 5 Land Auction**

Illuvium will host a live event streamed on Twitch to auction the tier 5 land parcels. This auction will be different, with bidders pushing the price
with their bid. There is a fixed end time for the auction, but each offer extends the auction by 5 minutes.

**Payments**

ETH and sILV2 are valid payment options, but not in one transaction. While sILV2 will not attract external revenue, it will incentivise current token
holders to claim their yield tokens as sILV2. This phenomenon will massively reduce the total supply of ILV long term.

**Revenue Distribution**
Landowners will have the opportunity to earn revenue from players in the main game through the novel use of a Balancer multi-token Weighted Pool. They will do so by swapping fuels they generate in-game for ETH. On the other side, players in Illuvium will exchange ETH\* for fuel and use it to complete all transactions in the game except for trading between players.

The target will be for landowners to earn approximately 5% of the total revenue generated from in-game purchases in Illuvium.

**Change To Illuvium Pricing**

The goal for Illuvium: Zero is to make it exciting for landowners to have some agency, which includes influencing the price of the fuel they swap and having an impact on the main game. However, Illuvium games require some level of stability to function well. We have come up with a solution to these requirements:

Illuvium will not fix fuel (required for all in-game interactions) to USD. Instead, pricing in-game will be a fixed amount of fuel. Since this could cause fuel prices to fluctuate significantly depending on the actions of the landholders, the DAO will automatically supply or withdraw fuel from the balancer pool if the price differs by more than 25%.

Practically, suppose the demand for fuel is higher or lower than the production. In that case, the price of actions in Illuvium can increase or decrease by up to 25%. Landholders can choose to sell when the price is high, and players can buy fuel when low.

The council can adjust the parameters of either the base price for fuel or the percentage variance allowed. They can also change the approximate percentage of revenue received by landholders.

\*sILV2 will not be used to swap for fuel. Instead, sILV2 acts as an alternative to fuel pegged to the price of ILV.

## Rationale

Illuvium provided all the details of the Land Sale early. However, after community feedback, the prices were too low. We have since seen a downturn in the crypto market, and the price now seems reasonable. All the details above have been thought through carefully, and we feel they
are mature enough for the council to consider.

## Test Cases

N/A.
