---
iip: 4
title: Removal of Locked Tokens from Yield Farming
status: Implemented
author: Kieran Warwick (kieran@illuvium.io)
discussions-to: https://discord.gg/illuvium
created: 2021-04-14
updated: N/A
---

## Simple Summary

The community has highlighted an issue with the current ILV Yield Rewards. The main configuration in question relates to the fact that locked tokens are currently able to stake in the ILV pool or provide liquidity via the ILV / ETH pool and receive Yield Rewards. Allowing locked tokens to be staked in any Yield generating pool reduces the distribution of the ILV token to unlocked token holders, potentially harming the decentralisation of the project. Removing the ability for locked tokens to farm Yield Rewards will substantially increase the APY of both pools, which will incentivize new users to purchase and stake ILV.

## Abstract 

Automatically place all locked tokens into a newly created ILV pool with a weight configuration of 0 and remove the ability for locked tokens to be staked into the ILV pool or provide liquidity via the ILV/ETH pool that both generate yield rewards. Reconfigure the codebase to recognise this zero weight pool only for the purpose of distribution of Vault Distributions.


## Overview

### Yield Farming - 3m ILV distributed over 3 years 
* **Pool 1:** Unlocked Tokens ILV pool Weight [0.2] - 20% of the total Yield Rewards during periods of no flash pools.
* **Pool 2:** Unlocked Tokens ILV/ETH pool Weight [0.8] - 80% of the total Yield Rewards during periods of no flash pools.
* **Pool 3:** Locked Tokens ILV pool Weight [0.0] - 0% of the total.
 
### Revenue Distributions - 100%
Unchanged. All pools (except flash pools) receive the same weighting for the purpose of Vault Distributions.
 
### Voting Rights 
Included in governance:
 
* **Pool 1** 
* **Pool 3** 
 
Excluded from governance
 
* **Pool 2** 
 
NOTE: A further IIP is currently being developed to suggest a reconfiguration of the codebase to allow Pool 2 to take part in governance. Due to the complexity of this change, it requires a separate IIP that would be deliberated by the council on its own merits.


## Rationale

IIP 4 gives the prospective investors more confidence in the overall distribution of ILV, and the APY in the Illuvium protocol. The reduction in total tokens for locked token holders is expected to be far smaller than the increase in value of the token, and as such it makes strong financial sense to implement this IIP for all parties.
