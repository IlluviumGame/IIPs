---
iip: 10
title: Mini Game
status: Implemented
author: Aaron Warwick (aaron@illuvium.io)
discussions-to: https://discord.gg/illuvium
created: 2021-08-11
updated: N/A
---

## Simple Summary
The Illuvium Game Development team proposes to build a new game. This mini-game will have a smaller scope, and exist in the City Building
genre. The eventual goal is to have the mini-game interface with the main Illuvium game, for the purposes of revenue distribution and NFT
creation

## Abstract
A 3D isometric city building game will be developed using Unity3d. At least two additional core contributors will be hired. Regular updates will be
provided to the community, including proof of concept and a non blockchain linked version for the App Store and Google Play Store. Integration
with Illuvium via solidity contracts will be implemented before final release.

## Overview
### Development
An early draft of game design document for Illuvium: Zero has been distributed to the community. The GDD covers much of the content of the game, as a high level overview of the game dynamics. However, since the original document was shared, additional functionality has been added to further describe integration between the two games. One such function was the need for the creation of a shared pool to act as the bridge between the two games.

Additional research needs to be done to identify the best execution of the solidity contracts required, and how to set up a backend that best minimises gas fees and transaction times. The intention is to build the game in stages as follows with approximate timelines that assume no
major hurdles:

* POC (Start + 2 weeks) - An internal demo of core gameplay features with reasonable quality art. We will share videos of this POC with the public, but we will not share the build.
* v1.0 (Start + 10 weeks) - Land sales and mobile release. The land will be connected to the game. There will also be an option to play a 'virtual' version of the game not connected to land.
* v1.1 (Start + 14 weeks) - Blueprint NFT Minting, blueprints created in the game will be mintable on the blockchain.
* v2.0 (start + 18 weeks -> Aligned with the Release of Illuvium) - Full release. All game data (except for minted NFTs and land ownership) will be wiped. Pools will be established for Fuel. Fuel generated in Illuvium Zero will be usable in the main game.

This progression is suggested to speed up development by eliminating the need to build the back end systems immediately, which would no longer be a requirement for early builds.

### Land Sale
The land sale would consist of 100k plots of land sold over a large timeline, in much the same way that yield farmed tokens are distributed. Thus giving those that are early supporters of the project the opportunity to take part in an Illuvium universe gaming experience—before the masses who are only awaiting the main game. Land would be split into Tiers based on its production rate and rarity, with an algorithm used to generate and categorise each parcel of land into narrow bands that are unique but roughly equal.

A Dutch auction will be used to sell land in tranches to maximise hype, minimise gas wars, and ultimately lead to a fairer system for all participants. The highest tier land will be incredibly rare and offer the owner a connection to the Illuvium ecosystem in novel and exciting ways.
More information will be released soon.

#### Payment
Both ETH and sILV will be used as payment methods for land. While sILV will not attract external revenue, it will incentivize current token holders to claim their yield tokens as sILV. This phenomenon will massively reduce the total supply of ILV long term.

> **_Note:_** It is unclear yet if hybrid purchases can be made (sILV + ETH in one transaction)

## Rationale
Few NFT gaming projects have thus far created truly compelling use cases for land. While Illuvium: Zero still has room to grow with new features expected to be added over time, the underlying concept of a fun building game that ties directly to revenue distribution—and gives players agency in a dynamic that transcends beyond a single gaming experience—is an exciting prospect.

Illuvium: Zero also acts as an interesting proof of concept to integrate multiple games from the same shared universe. The project will effectively gamify staking in a novel and exciting way, that can lead to significant interest in the protocol, as well as the possibility of a large boost to revenue
distribution for staked token holders.

## Test Cases
N/A
