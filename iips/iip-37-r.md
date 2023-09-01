---
iip: 37-r
title: Fuel and Land Integration
status: Pending
sponsor: Aaron | Illuvium
discussions-to: https://discord.gg/illuvium
created: 2023-08-08
updated: 2023-08-30
---
## IIP-37-R Fuel and Land Integration - Allow Purchasers and Land Holders To create Buy/Sell Orders For Fuel

## Simple Summary:
The original plan is to build a multi-token pool using an AMM system that only allows landholders and players to sell or buy Fuel (respectively) at market price, with slippage, which requires significant liquidity. This simple proposal suggests instead building an order book system and clearly defines how buyers and sellers of Fuel can specify prices for their orders so that they are not required to accept the current market price.

## Abstract:
Currently, players can only purchase Fuel at the prevailing best price, while landholders are restricted to selling their Fuel at this same rate. The proposed system enhances this framework: players will still have the option to buy Fuel at the best available price, and landholders can continue to sell in the same manner. However, an added feature will now allow users to specify their desired price, completing the transaction once the market matches their set rate. 
 
The parameters for the Cost of Fuel for Travel, Fuel Supply per land plot, Maximum Fuel Price (Top Guardrail), and Land Sale details must be defined and approved in future ICCP(s).

## Motivation:
Allowing landholders and players to set a price that works for them is an added benefit that lets people play the market and engage more deeply with the ecosystem. Experienced players can effectively act as an arbitrageur. At the same time, novices will still have the option to hit a ‘buy now’ button and know they are getting the best price currently available. The system is simple and easy to understand. Additionally, it removes the need for liquidity.

Mechanics to manage the supply of fuel will take an all-encompassing approach with various systems including manual and automatic balancing, as well as future land sales.

## Specification:
The proposed system includes the following specifications:
* Buy and Sell Orders: Players and landowners can place buy or sell orders, respectively, and set their price or sell at the best available price via an orderbook system.
* Manual and Automatic Fuel Supply Balancing: Manual adjustments can be made to the fuel supply after open beta launch, while evaluating and preparing for a move to an automated approach.
* Guardrail Introductions: A guardrail or ‘base price’ at which unlimited fuel will be available will be set via future ICCP.
* Future Land Sales: Future, smaller-volume land sales will take place after open beta based on increasing demand for fuel.

## Overview:
Below is a complete overview of the system:

#### Buy Order Placement
Allows players to place buy orders for Fuel. Players can specify the amount of Fuel they wish to purchase and the price they are willing to pay per unit of Fuel. If they don’t specify a price, the system will automatically set the price to the best available price in the market. This feature is essential for enabling players to acquire Fuel for use in the game.

#### Sell Order Placement
Enables landowners to sell the Fuel they generate. Landowners can specify the amount of Fuel they wish to sell and set their price. If they don’t set a price, the system will automatically sell the Fuel at the best available price.

#### Fuel Guardrail
Enables players to set unlimited buy orders for Fuel at a fixed price (top guardrail). Players can specify the amount of fuel they wish to purchase at a price pre-defined by the council and team. To maintain the revenue sharing model with landowners, 5% of this fuel sales revenue will be distributed to landowners proportionally based on their weekly fuel sales defined from midnight UTC on Sunday. The distributions will occur at least monthly.

#### Guardrail Positioning
The price of unlimited fuel supplied by the DAO will serve as an appropriate upper bound for fuel accessibility and a mitigation against major price volatility. The market price via orderbook mechanic will serve as a discount for players from the set price of fuel provided by landowners.

#### Fuel Balancing
The parameters for the economic framework of the ecosystem including fuel production per land plot, fuel price at the guardrail, and in-game fuel value (such as energy per travel) will be proposed as a holistic system by the team and approved by the council prior to open beta launch.  During at least the first 3 months after open beta launch, balance changes to these parameters will be made by the team, in consultation with the council.

In preparation, an automated balancing system will be piloted beginning at open beta launch.  After evaluating and improving the model, when sufficient robustness and stress testing of the model has been completed, at the discretion of the team and council, it will be moved into usage in a future ICCP.

#### Land Plot Sales
As player demand for fuel increases, small, predictable sales of Illuvium Zero land plots will be leveraged to scale fuel production.  These micro-sales will not begin until a minimum of four months after open beta, pending fuel demand increasing. 

#### Locking Orders To Storage
As we don’t want to allow players to use orders as a “storage hack”, any order created would be required to sit in the storage of the landholder. This incentivises landholders to build more storage (increasing the game’s strategy elements) or set a reasonable price to enable quick fulfillment.


#### No Second Order Sales
In our commitment to maintaining a stable and user-centric economy within the game, we've instituted a "No Second Order Sales policy." This means that once a player purchases Fuel, it cannot be resold to the pool. This decision has been made to prevent speculative trading, reduce the potential for external market manipulation, and ensure that the primary transaction between the game's producers (landholders) and consumers (players) remains straightforward. We aim to create a more predictable and stable in-game economic environment for the Fuel Pool by eliminating secondary market dynamics and focusing on genuine utility and consumption rather than speculative trading.


Note: While it is not possible for us to ban actors from creating secondary pools, said pools would have to exist outside IMX, with low liquidity, high slippage, and many such layers of friction that we do not believe to be a large-scale problem. This is a starkly different situation than what has occurred with sILV/2.

#### Launch Timing
Illuvium Zero will be launched in open beta between 2-6 weeks (targeted 4 weeks pending technical feasibility) prior to Illuvium Overworld, to be defined in a future ICCP. This allows land plot development to occur, allowing a steady fuel supply from landowners within weeks after Overworld launches.

## Rationale:
Custom pricing offers players and landowners greater flexibility in buying and selling Fuel while also ensuring the stability of the Fuel market by incentivising landholders to set sell orders at a price that players take up quickly. It keeps with our promise of building an interconnected universe where landholders and players have a tangible impact on each other while removing some of the inefficiencies of the previous multi-token AMM system.

A top guardrail will be used to position the actual price of fuel produced by the DAO. The orderbook pricing system allows a fluctuating reduction in fuel costs positioning the landowners and other players in a symbiotic relationship.

An automated system for future land sales and fuel supply balancing is preferable to manual adjustments as it provides more predictability to players. However, an automated system has a higher risk of working effectively compared to adjustments by the development team until the economic system is in equilibrium and the automated fuel balancing model has time to mature.

The timing needed to develop Zero land virtually ensures that for the first weeks or months after Overworld launch, the price of fuel will stay at or just under the top guardrail. Launching Illuvium Zero weeks in advance reduces the time to reach a stable, free-market equilibrium. The top guardrail should be rarely used the longer the system runs.

#### Sponsor:
Aaron | Illuvium
#### Key Contributors:
Nijafe, Vetemor, Animositas, Seatin
