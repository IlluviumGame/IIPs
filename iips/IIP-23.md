---
iip: 23
title: Illuvium Forge
status: Proposed
author: Aaron Warwick & Pedro Bergamini (0xpedro.eth)
discussions-to: https://discord.gg/illuvium
created: 2022-06-22
updated: N/A
---

## Simple Summary

Illuvium Forge gives prospective customers access to specific locked ILV positions at a discount. It allows the seed and team investors to offer their tokens at fixed discounts decided by the Council. When a customer purchases those tokens, the sellers receive their share of the proceeds and the buyers receive a newly minted Shard NFT that stores all the details of their position. The purpose of this is to give access to early liquidity without directly affecting the token price.
Every time someone acquires a position, it locks the tokens for the selected period (from 1 to 3 years), further reducing unlocked ILV supply.

## Abstract

As with any project, the token supply must eventually enter the market. However, not all projects handle this in the same way. Previously, the Council voted on a one-time delay of said tokens while we pushed to bring to market revenue-generating events. With the first land sale’s conclusion, we are ready to begin revenue distributions, and we look to other ways to handle new tokens entering the market.

Forge allows those token holders the opportunity to gain liquidity by selling those tokens at a discount for a large lock-up. It is available for everyone, not just VCs, and the general community can purchase ILV at a discount for the first time.

## Overview

Prospective buyers purchase positions via an NFT that holds the details of the tokens they stake to receive RevDis and Yield Rewards.

### Vesting Contract

The Vesting contract stores a vesting position for each original locked ILV holder (seed and team members) with all necessary data for its related vesting schedules, such as the number of tokens and the start and end timestamps. Notice that even though it’s an ERC721 contract, transfer functionality is disabled.

It provides the following functionality:

**View Balance** - Show the holders of locked tokens an up-to-date balance of their positions.

**Claim Tokens** - Allows the holders of locked tokens the ability to claim tokens as per their linear vesting schedule (usually one year, except for the founders who we configure to unlock over three years)

**Claim Revenue Distributions** - These specific locked positions do not claim through the existing Staking App and instead use the Rewards contract. This means owners of a staked Shard and existing ILV would need to claim once through the Staking App and once through the Forge app. In a future update, we should merge this as a QOL improvement. However, this is a complex task and to begin, it is much better for security to keep them decoupled.

### Registry Contract

The Registry contract creates the interactions between the two interested parties (the buyer and the seller).

It provides the following functionality:

**Communicates with Vesting Contract** - The Registry Contract has special permissions to update Vesting Positions.

**Offers tokens to the market** - Holders of Vesting positions use the registry to offer their tokens at the specified discount. When those tokens are purchased, the original holder receives their share of the liquidity.

**Allows purchasers to buy locked ILV** - A purchaser decides the length of their lock-up, which determines their discount, and the number of tokens they wish to purchase, limited by the number of tokens on offer.

**Allows Shard NFT holders to stake** - Before the newly created Shard NFTs can receive Revenue Distributions and Yield Rewards, they must stake in the Rewards contract. An auto-stake option exists to make this seamless.

**Withdraws tokens from the market** - Holders of Vesting positions that have previously offered their tokens can withdraw them from the market, allowing holders the control to only offer when they wish.

**Redeems NFTs for ILV** - Once the locking period expires on an NFT, the holder redeems it for ILV.

**Views total ILV offered** - Self-explanatory.

We should clarify that at no point does a purchaser interact with a single holder of a Vesting position. Instead, the prospective buyer only interacts with the aggregate of all Vesting positions that have offered their tokens. Vesting position holders don’t determine the price or the lock-up. Set discounts exist for each lock-up period, fully defined and controlled by the Council, and Vesting Position holders choose to make their tokens available, or not.

### Rewards Contract

Staked Shard NFTs representing locked tokens are eligible for Revenue Distributions and Yield Rewards. The Rewards contract works the same way as the current staking pools. The eDao sets the weight of this new pool with values that make it function as an extension of the ILV pool. Between the ILV pool and the Rewards pool, the total weight should be equivalent to 20% of the total rewards. Periodic updates are required to keep these values aligned, and the Council can adjust the target values via ICCP.

The Council can always vote on adjustments to the pool weights. Those weights are not the concern of this IIP.

It provides the following functionality:

**Stakes NFTs** - Stakes an NFT so that it can receive rewards.

**Unstakes NFTs** - Unstakes an NFT so that it can be redeemed for ILV.

**Claims Rewards and Yield** - This allows a holder of a staked NFT to claim their percentage of the total claimable rewards and yield.

**Views Rewards and Yield** - Shows a holder of a stake NFT their claimable Rewards and Yield.

### Proposed Lock Configuration

- **1-year lock:** 8% discount

- **2-year lock:** 18% discount

- **3-year lock:** 28% discount

As with all ILV contracts, these values are configurable by ICCP.

## Rationale

Illuvium Forge is a suite of solidity contracts that further improve the Illuvium protocol. It provides a clever way for holders of Vesting positions to gain access to liquidity without those tokens hitting the market. Many future improvements could further extend the functionality, but for now, it is essential to stay focused and implement the core features in a timely manner.

## Test Cases

N/A.
