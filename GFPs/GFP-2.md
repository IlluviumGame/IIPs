---
GFP: 2
title: Enable Beyond Disk Fragments in Overworld
status: Pending
Sponsor: Alexa
Key contributors: Filow, Garf
discussions-to: https://discord.gg/illuvium
created: 15 September 2024
---

### Simple Summary
This proposal seeks to introduce Beyond D1sk fragments as collectible items within the Overworld (OW). Players will gather fragments during paid OW runs, which can be combined to forge a Standard or Mega D1sk. This feature aims to enhance interoperability between Beyond and Overworld while providing an additional incentive for players to engage with the Overworld.

### Abstract
This proposal allows players to collect D1sk fragments during OW runs, which can be combined to forge either a Standard or Mega D1sk. This provides a gameplay-driven alternative for accessing Beyond D1sks. By introducing this reward system, players are encouraged to engage more deeply with the OW, potentially increasing fuel purchases, while also promoting Beyond organically through gameplay, allowing players to discover it naturally without the need for direct advertising.

### Overview
The core idea is to introduce collectible Beyond D1sk fragments within OW, allowing players to discover them across various locations. Once a player gathers enough fragments, they can forge a Standard or Mega D1sk in Beyond. The required number of fragments and drop rates would be adjustable by the team to maintain balance with Beyond’s economy. To increase availability and player engagement, it may be preferable to require a higher number of fragments to forge a D1sk, making fragments more common and distributed across multiple runs. 

Here are some key points:
* The number of fragments required to forge a Mega D1sk would be six times that of a Standard D1sk, ensuring the price correlation between them is maintained.
* D1sk fragments would be found in fragment caches, with higher stage regions containing more fragments. Stage 0 regions would not contain any fragment caches.
* Fragment caches themselves would have three stages with differing content values based on their own stage. A stage one cache would contain few fragments, whereas a stage three cache would contain a large amount of fragments. 
* D1sk fragments would always match the active non-alpha set/wave. You can only use fragments of one wave for that particular wave.
* D1sk fragments would only be collectable while a set/wave is active.
* Forged D1sks from fragments would not count towards the individual stretch goals, so the value of purchasing d1sks is maintained.
* Scanning a region would show the location of the fragment caches, increasing the value of the scan feature.
* Opening a fragment cache would consume either no ergon energy or a minimal amount, such as 10-100 ergon energy, encouraging deeper exploration of the map.
* The number of fragment caches present in a region would use a similar mechanic as big ore deposits in a region. There will always be one present on the map, with a chance of having multiple fragment caches showing up.
* The fragment cache stages have a fixed probability to show up in all three run stages. Whether you go on a cheap run or an expensive run, you will always have the same odds of finding a Stage 1 or 2 or 3 fragment cache. 
* D1sk fragments extracted from a cache would be tradable.

The design of the fragments economy will be up to the team to design. Here is an example to illustrate the idea using the following metrics:

ETH price - 2350$ <br>
Standard D1sk - 0.003 ETH - 7$ <br>
Mega D1sk - 0.018 ETH - 42$ <br>
Stage 1 travel - 150 crypton - 0.556$ <br>
Stage 2 travel - 450 crypton - 1.667$ <br>
Stage 3 travel - 1350 crypton - 5$ <br>

Standard D1sk Fragments required - 350 <br>
Mega D1sk Fragments required - 2100 <br>
Fragment Caches per region - 1 to 3 <br>
Price per fragment - 0.02$ <br>

**Number of fragments inside each cache stage per region stage:**
|               | Stage 1 Run       | Stage 2 Run       | Stage 3 Run        |
|:---------------|:-------------------|:-------------------|:--------------------|
| Stage 1 Cache | 1 - 5 Fragments   | 3 - 10 Fragments  | 9 - 20 Fragments   |
| Stage 2 Cache | 5 - 10 Fragments  | 10 - 20 Fragments | 20 - 30 Fragments  |
| Stage 3 Cache | 15 - 30 Fragments | 30 - 60 Fragments | 45 - 100 Fragments |


**Chance of obtaining each Fragment Cache stage:**
|                      | Stage 1 | Stage 2 | Stage 3 |
|----------------------|---------|---------|---------|
| Chance to find Cache | 80%     | 15%     | 5%      |


**Number of average runs required to be able to mint each D1sk with Fragments:**
|               | Stage 1 | Stage 2 | Stage 3 |
|---------------|---------|---------|---------|
| Standard D1sk | 85      | 37      | 12      |
| Mega D1sk     | 512     | 221     | 74      |

Note: These values are based on an average of finding one cache per run, and further balancing may adjust fragment quantities and drop rates. The team may also explore the option of having variable probabilities for cache stages across different run levels to better fit the Overworld gameplay.

### Rationale
Integrating D1sk fragments into OW enhances the gameplay experience while establishing a seamless connection between Beyond and OW. Players will gain additional value from each OW run, potentially boosting both engagement and fuel consumption. From a marketing standpoint, this approach promotes Beyond organically through gameplay, allowing players to discover it naturally without the need for direct advertising. This should help increase the supply of Beyond Illuvitars in line with Illuvium’s growing player base, ensuring the rarity of previous waves is preserved. By keeping this feature exclusive to paid runs, it ensures alignment with the in-game economy and further incentivizes fuel purchases. Using a stage system for the fragment caches is in line with the project’s stage system and provides a minor luck-based aspect to the cache mechanic.
