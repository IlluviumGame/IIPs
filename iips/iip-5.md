---
iip: 5
title: Introduce sILV double farming rewards in Sushi
status: WIP
author: Pedro Bergamini
discussions-to: https://discord.gg/illuvium
created: 2021-06-03
updated: N/A
---

## Simple Summary

The Sushi team recently listed the ILV token in their MasterChef V1 contract, making it possible for ILV-ETH SUSHI LP holders to stake their tokens and earn Sushi tokens APY. Sushi is now launching their MasterChefV2 contract, which makes many improvements in their Yield system and allows us to develop a Rewarder contract linked to our ILV-ETH MCV2 staking pool and distribute double farming rewards, similar to what [Alchemix](https://alchemixfi.medium.com/farming-with-added-benefits-5a2a10b49719) launched last week.

It's important to note that this will have no impact on the treasuries ILV allocation. The left-over ILV from the BLP sale will be dealt with in a separate IIP to be discussed with the council later.

## Abstract 

This IIP proposes the creation of the IlluviumRewarder contract and minting 50k sILV. The contract will be receiving the sILV to distribute over 90 days to sushi yield farmers. sILV is used as an in-game currency that will be able to be sent to ImmutableX layer 2 and spent for Illuvium NFTs. All in-game purchases are indexed to USD so a price conversion from sILV to USD (based on ILV) is used.
## Overview

### sILV

The Rewarder contract will be using sILV, which means the eDAO will mint 50k sILV for the double farming incentives, and later when we launch the IlluviDEX those will be able to be used for buying NFTs in the marketplace.

### Sushi Yield

Double farmings will be available at https://app.sushi.com/yield, so current ILV/ETH liquidity providers in Sushi will be able to stake their LP tokens in the "Double Yield Farms" section to start earning SUSHI + sILV yield.
