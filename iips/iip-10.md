---
iip: 10
title: Illuvium Zero
status: WIP
author: Aaron Warwick (aaron@illuvium.io)
discussions-to: https://discord.gg/illuvium
created: 2021-08-17
updated: N/A
---

## Simple Summary
You are a Valain reconnaissance drone, ejected off your ship before impact with a ruined alien planet.Your mission: build a secure base of operations on the planet, gathering as much intel as possible. You collect, mine, and process local resources to build generators, storage silos, research facilities, and other key structures and tools.

Energy scans and observations of strange phenomena hint that this is no ordinary planet. Exotic particles visibly spill from rifts in the very fabric of reality—and these may or may not be related to the deity-like beasts that seem to dilate in and out of existence, like apparitions that materialize into corporeal forms.

With only the equipment of a reconnaissance drone, it seems unlikely you will be able to capture these beasts.

But by studying them, and researching their fuel, you may be able to make use of them—and their considerable powers.



## Abstract 
Illuvium Zero launch will consist in a few development phases:

### Proof of Concept
* No blockchain elements
* Most buildings
* Basic resource types
* One fuel type

### Alpha
* All artwork for existing game entities
* Working UI
* All fuel types

### Private Beta
* Add a simulation of trading
* Converter Buildings

### Public Beta
* Land as NFT via sales event
* Available on App Store and Google Play Store
* Mint Skins from a Blueprint

### Version 1 Release
* Each Structure on the Land  wiped in preparation for release. To ensure fairness for all players.
* All elements set up as NFTs and built on IMX
* Finalised UI elements
* Finalised Art

Backend server to allow networked trading between real players

Modify Illuvium game to use fuels generated from Illuvium Zero.

## Overview

### Gameplay Overview
* Resources
A Resource is a major component of Illuvium Zero, and they are the drivers of the games internal economy. Many actions, including building a Structure require (and consume) at least one Resource type. Other actions can generate a Resource.

Three (3) types of Resource are proposed, although the general thinking holds if there are 2, 3, 4 or more.

In order that players don’t get ‘stuck’ the suggestion is that they should be ‘air dropped’ a minimum set of resources each day. This could be conditional (only send if resources are lower than X or it could just be a consistent amount each day). it could also be an Action on the home building ('Request Support' ‘Radio in Airdrop’ etc).

Basically this would be a small amount but enough for them to build a Mine type building after a day or two.

#### Fuel
Generating Fuel is one of the main goals of Illuvium: Zero. It is used as a cost in many high level buildings, and potentially can be used as a way of sharing revenue in the Illuvium game by enabling forging of Armour, Weapon, Shards, and so on.

> **_Note:_** To avoid confusion with Resources we generally avoid using the term ‘resource’ in relation to Fuel.

The conversion of a Resource into Exotic Particle requires a Fuel Converter or access to the Marketplace.

#### Source
The term Site refers to the location of natural (or unnatural) deposits from which a Resource or Exotic Particle can be extracted. The quantity of each Site type is finite and immutable: it is defined directly on the Land NFT.

When combined with an Extractor, a Site can be used to generate a Resource or Exotic Particle. There is a one-to-one relationship between a Site type and the Resources and Exotic Particles it can generate.

#### Resource and Fuel Generating Buildings
The general process to get from the natural resources of a Site to a Exotic Particle ready for use in the main game is as follows:

* A Extractor is built at the Resource Site or a Converter is built on clear land.
* The Structure has actions or passive generators which extract the Resource.
* These resources are used to build a Fuel Converter or Fuel Extractor.

In the game engine we have two options for generating something:

* **Actions** These require a player to click a building and press a button to start an action which will take time to complete. The action typically has a known and fixed result and timeframe.

The progress of the action is shown above the building with a progress indicator. When the action is complete the progress bar will turn in to a button which the player can click to complete the action. The action button indicator above the building will ‘nag’ the player via animation or visual effects to let them know the action has completed.

Actions may have a Resource or Exotic Particle cost. Actions can be quite varied in their effect, but one effect is to generate a Resource type or Exotic Particle type.

* **Passive Generators**  A passive generator is a component of a Building that generates a Resource  type or Exotic Particle type over time without requiring player action. It must still be collected by the player (by clicking a building and clicking the gather button) in order to move from the Structure to the player's Matter Silo.

Passive generators typically have a limit to the amount that can be generated analogous to storage space that gets filled. When this limit is reached an action button appears above the building and ‘nags’ the player in a similar manner to a completed action.

Players may retrieve gathered Resources or Fuel at any time, they do not need to wait for the storage to be filled. 

#### Resource and Fuel Building Types
Taking the above notes in to consideration the following table provides for some building ideas which allow players to make meaningful decisions about what they build on their land:

| Building Category | Action  | Passive Generator   | Requires Site?  | Details/Notes   |
|---|---|---|---|---|
| Resource Extractor | Generate Resource | Generate Resource | Y | The simplest building type. Place it on a Site to generate a Resource both actively and passively. |
| Resource Converter | Generate Resource  from Resource | None | N | Takes a certain amount of one Resource and converts it in to another. |
| Fuel Extractor | Generate Exotic Particle | Generate Exotic Particle | Y | This building generates Exotic Particle from a Site. |
| Fuel Converter | Generate Exotic Particle | None | N   | Takes a certain amount of one Exotic Particle and converts it in to another. |

Details of these buildings of course need to be balanced, but the idea is that the player can choose between ultimate flexibility (e.g. Mine + Converter) vs ultimate efficiency (Refinery). They can also make decisions based on their play style, would they prefer to have more passive generation, maybe they only log in a few times a week vs a much more active action driven play style (logging in multiple times per day).

Note that a Building Category is not a Building Type. There could also be many types of buildings within a given category, for example:

    Mine →  Large Mine → Enhanced Mine →  etc

Generally these would have a linear progression, such that bigger is better, but this doesn’t have to be strictly followed and we can introduce other factors, for example an ‘Enhanced Mine’ might generate many more Resources at optimal usage, but may also require the player to log in frequently and launch many Actions per day to reach this optimal output. 

#### Illuvial Scanning and Blueprints

Another exciting aspect of the Illuvium: Zero game is the ability to create new skins via a Blueprint for the main Illuvium game. The creation of new skins requires the scanning of Illuvials, which is in itself an interesting part of the game, as the player gets to build a collection of scanned Illuvials. As well as appealing to players who enjoy collecting the scanned Illuvials may give additional insight in to the creatures characteristics in the main game.

The general process to be able to Scan Illuvials is as follows:

* Player builds each required building of the Singularity Scanner

* Player builds the Singularity Scanner

* Player starts the scanning activity

* Player completes the scan of an Illuvial and now has an Illuvial scan.

* Player builds the Quantum Fabricant

* Player launches a research/design action based on the scanned Illuvial Type

* Player completes activity and is awarded a Blueprint to build a new skin

* Player uses the plan to mint an NFT

> **_Note:_** This process is largely similar for building a Weapon or Armour Blueprint except the Materials Lab is used instead of the Singularity Scanner.

> **_Note:_**  In the first iteration of the game, the plans for skins can be researched but the plan cannot be used to mint a new NFT for the skin.

#### Affinity
In order to build connection to the themes of the main game, Affinity will play a role in the scanning of Illuvials. This is achieved by offering players Land from each Region. These each attract different Illuvials based on their Affinity. The Singularity Scanner can also be upgraded to attract higher tier Illuvials.

#### Scanning Building Types
Taking the above notes in to consideration the following table provides for some building ideas which allow players to make meaningful decisions about what they build on their land:

| Building Category  | Action | Passive Generator | Passive Effect  | Details/Notes  |
|---|---|---|---|---|
| Singularity Scanner  | Scan Illuvial  | None  | None  | Basic building for scanning Illuvials. |
| Data Bank | Download  | None  | Increases Illuvial Scan Storage  | A scanner alone will store only 1 scan (could be 2 or 3, but it is a small amount). The data bank would allow for increased storage. This could include an action to ‘download’ the data from the scanner to the Data Bank, or it could simply be a passive action. |
| Lure  | None  | None  | Decrease Scan Time  | This building is used to generate energy that attracts Illuvials and can therefore decrease scan time. |
| Quantum Fabricant | Create Blueprint | None | None | This is the activity that creates a Blueprint (to build skins/suits/emotes/etc) from Illuvial scans. Clicking the action opens an interface for selecting the design that will be researched. |


## Rationale
<!-- TODO -->
