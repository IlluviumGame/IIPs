---
iip: 37-R
title: Allow Purchasers and Land Holders To create Buy/Sell Orders For Fuel
status: Pending
author: Aaron | Illuvium
discussions-to: https://discord.gg/illuvium
created: 2023-08-08
updated: 2023-09-05
---

## Simple Summary:
The current plan is to build a multi-token pool using an AMM system that only allows landholders and players to sell or buy Fuel (respectively) at market price, with slippage, which requires significant liquidity. This simple proposal suggests instead building an order book system and clearly defines how buyers and sellers of Fuel can specify prices for their orders so that they are not required to accept the current market price.


## Abstract:
Currently, players can only purchase Fuel at the prevailing best price, while landholders are restricted to selling their Fuel at this same rate. The proposed system enhances this framework: players will still have the option to buy Fuel at the best available price, and landholders can continue to sell in the same manner. However, an added feature will now allow users to specify their desired price, completing the transaction once the market matches their set rate. Note: Any rails parameters would still need to be defined and approved via Council, but doing so is significantly easier than using the multi-token AMM approach.


## Motivation:
Allowing landholders and players to set a price that works for them is an added benefit that lets people play the market and engage more deeply with the ecosystem. Experienced players can effectively act as an arbitrageur. At the same time, novices will still have the option to hit a ‘buy now’ button and know they are getting the best price currently available. The system is simple and easy to understand. Additionally, it removes the need for liquidity. 


## Specification:
The proposed system includes the following specifications:
- Buy and Sell Orders: Players and landowners can place buy or sell orders, respectively, and set their price or sell at the best available price.


## Overview: 
Below is a complete overview of the system:



**Buy Order Placement**
Allows players to place buy orders for Fuel. Players can specify the amount of Fuel they wish to purchase and the price they are willing to pay per unit of Fuel. If they don’t specify a price, the system will automatically set the price to the best available price in the market. This feature is essential for enabling players to acquire Fuel for use in the game.



**Sell Order Placement**
Enables landowners to sell the Fuel they generate. Landowners can specify the amount of Fuel they wish to sell and set their price. If they don’t set a price, the system will automatically sell the Fuel at the best available price.



**Locking Orders To Storage**
As we don’t want to allow players to use orders as a “storage hack”, any order created would be required to sit in the storage of the landholder. This incentivises landholders to build more storage (increasing the game’s strategy elements) or set a reasonable price to enable quick fulfilment.



**No Second Order Sales**
In our commitment to maintaining a stable and user-centric economy within the game, we've instituted a "No Second Order Sales policy." This means that once a player purchases Fuel, it cannot be resold to the pool. This decision has been made to prevent speculative trading, reduce the potential for external market manipulation, and ensure that the primary transaction between the game's producers (landholders) and consumers (players) remains straightforward. We aim to create a more predictable and stable in-game economic environment for the Fuel Pool by eliminating secondary market dynamics and focusing on genuine utility and consumption rather than speculative trading.



## Rationale:
Custom pricing offers players and landowners greater flexibility in buying and selling Fuel while also ensuring the stability of the Fuel market by incentivising landholders to set sell orders at a price that players take up quickly. It keeps with our promise of building an interconnected universe where landholders and players have a tangible impact on each other while removing some of the inefficiencies of the previous multi-token AMM system.

## Sponsor:
Aaron | Illuvium
