---
iip: 70
title: Blueprint and Skin Production Streamlining Proposal 
sponsor: Perry | Illuvium
key contributors (authors): Perry, Christoph, Jay
discussions-to: https://discord.com/channels/760344898200666112/1301095755787927572
---

## Abstract
This proposal outlines changes to the current blueprint and skin production process across Illuvium Overworld (OW) and Illuvium Zero (IZ). The proposed modifications aim to simplify gameplay loops, reduce on-chain transaction and system load, and make Blueprints consumable when minting skins, creating more stable demand.

## Summary
- Streamlined Morphopod and Dye Production: Remove unnecessary back-and-forth interaction between OW and IZ for producing Dyes/ Skins.
- Consumable Blueprints: Adjust Blueprints to be consumable upon minting.

## Overview
### Current Gameplay Loop & Blueprint Production Challenges
Our current system for skin creation relies on an interaction between Morphopods, Dyes, and Blueprints, with resources moving back and forth between Overworld (OW) and Illuvium Zero (IZ). Through this setup, players catch Morphopods in OW, transfer them to IZ to mutate plants and produce Dye NFTs, which are then used with Blueprint NFTs to mint Skins. This cross-game interaction has revealed several potential issues that we aim to address:
1. Producing Dye NFTs through the existing process generates a significant number of on-chain transactions, which can strain our backend infrastructure.
2. The transfer of Morphopods and Dyes between OW and IZ introduces a layer of friction to the gameplay. While it adds some interoperability between the two games, it doesn’t meaningfully enhance player engagement or add depth to the experience.
3. Since Blueprints are currently reusable indefinitely, Blueprint NFT owners may lose exclusivity over cosmetics production, potentially allowing players (including non-landowners) to enter the Blueprint market.
4. Even with Dyes and Blueprints in hand, players are still required to return to Overworld to gather additional resources to mint Skins. This added step further complicates the process.

### Proposed Adjustments
In response to these challenges, we propose the following adjustments:
1. The Podarium’s role will be redefined, removing Dyes from the production process entirely to simplify the system. This change eliminates the need for mutated plants and Podariums to create skins. However, we plan to reintroduce the Podarium at a later stage with a meaningful purpose.
2. Once a Blueprint is found, users can mint it with a mint cost and a Morphopod cost. Furthermore, users will be able to “purchase” morphopods in IZ for resources to not mandate people to play OW. These Blueprint NFTs can be sold or used in the Forge in the Overworld to create skins.
3. When a player uses a Blueprint NFT to mint a skin, it will be consumed or ‘burned’. Players can still remint these Blueprints and sell them on the market if they want.


## Rationale
By removing Dyes and simplifying Morphopod integration, we’re reducing unnecessary complexity and minimizing backend strain from frequent on-chain transactions. The shift toward consumable Blueprints introduces a strategic layer, preserving market exclusivity for landowners and the NFTs. Overall, these adjustments align our resource and asset flows with a more engaging, efficient, and economically sustainable system.
