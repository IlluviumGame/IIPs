---
iccp: 13
title: Fuel Economy and Land Sale Integration
status: Pending
author: Animositas
discussions-to: https://discord.gg/illuvium
created: 2023-08-05
---

## Simple Summary
This proposal defines how Illuvium will leverage small, predictable sales of Illuvium Zero land plots to scale fuel production to support onboarding of more players to Illuvium Overworld. 
This ICCP is an addendum to IIP-37 “Allow Purchasers/Sellers to set price for Fuel” proposed by Aaron Warwick. 

**Major improvements:**
- Automatic Price Stabilization Mechanic
- Transparent and Low Volatility Additional Future Land Sale Process 

**Minor improvement:**
- Scalability of Illuvium Zero paid player base through Fractionalization of Land Plots

**[Link to Q & A](https://github.com/Rickytan77/IIPs/blob/master/assets/ICCP-13%20%20-%20Q%20%26%20A%20-%20Fuel%20Economy%20and%20Land%20Sale%20Integration/Q%26A%20ICCP-13%20-%20Fuel%20and%20Land%20Economy%20Integration.pdf)**

## Objective
The objective of the Fuel and Land Economy Integration proposal is to avoid creating a new mechanic to increase the fuel supply per plot and instead leverage the ready-made mechanic that is already in our economy of additional land plots.  The simplest approach to do this in a controlled way for both Overworld and Illuvium Zero players is to very gradually mint new land plots as paying players enter the ecosystem.  This allows controlled fuel supply growth for many months that should result in fairly stable fuel prices for Overworld players and minimal manual or automatic adjustments needed to fuel production in Illuvium Zero.  

Additionally, an optional mechanic to fractionalize future land plots at a point determined by the DAO can be used to increase the number of paying players in Illuvium Zero without any additional diluting effects to revdis structures or existing land holders.

## Implementation
**Automatic Price Stabilization Mechanic via Land Plot Sales**

This proposal gradually introduces additional land plots into circulation via Dutch Auction sales once a ‘Land Sale Threshold’ has been reached. This threshold sets a minimum number of unique wallets purchasing fuel in one month before additional land sales would be triggered.
 
Once the threshold is reached, a Dutch Auction would be held on the 15th of each month to sell land plots based on a ‘Land Release Ratio’.  This ratio determines how many new land plots will be released based on the number of net wallets purchasing fuel during the month (i.e. X players purchasing fuel = 1 new land plot sold).  See Q&A for an example.
 
The specific values for the Cost of Fuel for Travel, Fuel Supply per land plot, Maximum Fuel Price (Guardrail), Land Sale Threshold, and Land Release Ratio would be recommended by the team and confirmed by the councils in a future ICCP. 

**(Optional Mechanic) Fractionalization of Land Plots**

Future land sales can optionally be sold in a fractionalized manner.  To achieve this in a non-dilutive way, fractionalized land plots should have proportionally reduced revenue.  For instance, a Tier 1 land plot could be split into two different T0.5 plots, four different T0.25 plots, or ten different T0.1 plots that are each eligible to sell fractionalized amounts of fuel. 
 
For maintaining in-game balance, all production values and resource requirements in Illuvium Zero would mirror the land plots of the respective T1, T2, T3, and T4.  When selling fuel on the market, the total amount eligible to be sold would be reduced by the fractionalized amount.  T5 land plots would be explicitly excluded from fractionalization due to the difficulty of coordinating a tournament with many different owners of the land plot.

The evaluation and technical considerations for fractionalized land should be left for future balancing decisions but this is introduced in this ICCP as an optional mechanic as it allows much more granular sales of future land. 


## Rationale
Increases in the quantity of fuel produced by Illuvium Zero plots will be necessary as the Overworld player base grows.  This can be administered through either increasing the amount each plot produces or by increasing the number of plots.  This proposal solves the question of how to address this in the mid-term (>1M active Overworld players monthly) while also providing clarity on future land distributions.
