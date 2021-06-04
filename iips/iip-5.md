---
iip: 5
title: 
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

This IIP proposes the creation of the IlluviumRewarder contract and minting 50k sILV. The contract will be receiving the sILV to distribute over 90 days to sushi yield farmers, which can be used for purchasing NFTs in a unique collection that will be later available for converting to in-game collectibles.

## Overview

### NFTs

NFTs used in this proposal will be able to be burned for in-game items, but won't affect the game balance. We will be deploying a new page at nfts.illuvium.io to allow users to swap their sILV for those NFTs.

### Sushi Yield

Double farmings will be available at https://app.sushi.com/yield, so current ILV/ETH liquidity providers in Sushi will be able to stake their LP tokens in the "Double Yield Farms" section to start earning SUSHI + sILV yield.
