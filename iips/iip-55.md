---
iip: 55
title: Training Grounds, Illuvial Staking and TrainingDex
status: Proposed
sponsor: Dr.Spoon
key-contributors: Filow, Scoriox, MegaRatty, HappyBallz
discussions-to: https://discord.com/channels/760344898200666112/1233071586555330560
---

## Simple Summary:
1) Create the Training Grounds structure in Illuvium Zero. This structure offers a way to passively train Illuvials, allowing them to earn experience. Landowners can utilize Training Grounds to train their own Illuvials or rent any unused spaces out to other rangers.

2) Introduce the concept of Illuvial staking in Illuvium Zero by allowing landowners to stake Illuvials into the Training Grounds. Staked Illuvials act as teachers, providing an experience bonus to matching Illuvials undergoing training in the same Training Grounds.

3) Implement a player-driven marketplace for training Illuvials (TrainingDex) where landowners can advertise their Training Grounds, and rangers can easily browse through the available options.

## Abstract:
The proposal aims to create a dynamic player-driven ecosystem for Illuvial training, offering landowners the flexibility to either train their own Illuvials or rent out available slots. This proposal will outline the details of several key components, including the Training Grounds structure with general guidelines, an example of the structure details, training costs, and the renting feature. Additionally, it will cover aspects of Illuvial staking such as individual values, bonus efficiency, overall staking bonuses, and TrainingDex features such as usage fees, building infrastructure, and its UI.

## Overview:
The creation of the Training Grounds structure, the introduction of illuvial staking mechanism and the implementation of the TrainingDex must all be executed together, as they are all crucial for creating a vibrant and dynamic ecosystem for Illuvial training.

Here's a breakdown of each one:

### Training Grounds
The Training Grounds offer landowners a way to either train their Illuvials, passively accumulating experience, or to rent out free spaces to other rangers. All the names, guidelines, structure details, terminology, and training costs are only suggestions, and it will be up to the team to decide on them.

**Guidelines**

- Each structure level will increase the number of available training spots, the experience gained per hour, and the number of staked Illuvials available.
- The maximum training level for an Illuvial will be determined by the average level of the staked Illuvials present for instruction. If no Illuvials are staked, training will be limited to a certain level. E.g. half the required level for fusion.
- Landowners must replenish the equipment for each training spot using elements before they’re available to be used to train Illuvials.
- Training spots function as mini-element storages and can be prepared for periods ranging from one to seven days. Element consumption aligns with the illuvial training duration for that specific spot.
- Training spots can be replenished with elements instantly, facilitating preparation for subsequent Illuvial placement.
- Training spots rentals are available for up to seven days, with increments of one day.
- The cost of training an Illuvial depends on both the Illuvial tier and the land plot tier. Training Illuvials up to the land plot tier incurs a reduced fuel cost, while training Illuvials of a tier higher than the land plot tier will require the normal fuel price.
- Illuvials gain bonus experience based on the tier of the land plot. Each higher tier provides an increase to the bonus experience according to their production bonus.
- The building efficiency decreases the length of the training session.
- No Illuvials can be undergoing training when changing the staked Illuvials teaching in the Training Grounds.
- F2P plots seeking access to the Training Grounds must construct them using real fuel. These Training Grounds on F2P plots may have limitations compared to those on P2E land plots, such as a level cap for example.

**Structure details**

- Size: 2x3.
- Area of effect: 6.
- Maximum level: 6. 7 for Mega Cities.
- Required structures: Nexus, Quantum fabricant.
- Maximum amount of structures: unlimited.
- Land Tier influence: Training cost and experience boost.
- Number of staking spots: 1 for every building level.
- Maximum number of training spots: Land tier + 1 for every building level. E.g. F2P plots get 1 training spot per level and T4 plots get 5 training spots per level.

**Efficiency**

- Start efficiency 100%.
- Minimum efficiency: 25%.
- Maximum efficiency: 150%.
- Efficiency increases with power stations.
- Efficiency decreases the training duration, with 100% corresponding to 1 day.

**Land Tier Bonus**

Here’s an example of the innate experience bonus for each land plot tier:

![image](https://github.com/Jaganite/IIPs/assets/171840128/a2505430-6562-4087-9a24-411b75b3923c)

**Training Costs**

Here’s an example of the Training Grounds costs, X represents the fuel cost:

![image](https://github.com/Jaganite/IIPs/assets/171840128/3ac05b0f-3c3f-437c-adf4-ae92b3e01ef8)

**Renting Costs**

If the training cost for a specific Training Grounds spot is X, then the landowner would set the rental price at X + Y, where Y represents their share for renting out the Training Grounds. The ranger utilizing the Training Grounds would pay X + Y + Z, with Z being the DAO fee.


### Illuvial Staking
Illuvial staking enables landowners to stake Illuvials within the Training Grounds, where they act as teachers, raising the level cap to which Illuvials can be trained and providing an experience bonus to matching Illuvials undergoing training. The training level cap is determined by the average level of the staked Illuvials teaching at the Training Grounds, and the bonus efficiency is determined by the sum of the staked Illuvial’s individual stats.

![image](https://github.com/Jaganite/IIPs/assets/171840128/229eafc5-5f82-4f57-b8d2-f95fa1b2d15b)

As shown in the table above, an Illuvial with perfect individual values, totaling a score of 30, would provide an efficiency bonus of 150%. While an Illuvial with a total individual values score of 10 would only grant 50% of the bonus. The standard 100% bonus will be given by an illuvial with a total individual values score of 20.

To illustrate how the staking bonuses would function, let's assume that the base bonus for each staked Illuvial is 5% to the corresponding illuvial line and that each affinity/class synergy stage is also 5%. Synergies would function similarly to those in the arena, requiring 3/5/7 Illuvials of the same base affinity/class to provide a bonus (2/4/6 for rogues), and 2/3/4 Illuvials of the same composite affinity/class. It's important to note that bonuses from repeated Illuvials wouldn’t stack.

For example, a Training Grounds structure with six available staking spots, where the following Illuvials are staked: Rypter, Rypterus, Ryplance, Carablu, Caradulo, and Cardulox.

These Illuvials would compose a total bonus of:

![image](https://github.com/Jaganite/IIPs/assets/171840128/a1f6c75d-413b-4118-87cf-c0f6929fd531)

If all six Illuvials have the standard 100% bonus efficiency, bonuses would be as follows:

![image](https://github.com/Jaganite/IIPs/assets/171840128/82789cbb-626f-4e31-89c8-6819cfd30d58)

If all six illuvials have the maximum 150% bonus efficiency, bonuses would be as follows:

![image](https://github.com/Jaganite/IIPs/assets/171840128/724a9be3-681e-463c-89f9-d82cbaeeb033)

In this last example, a Ryplance training in this Training Grounds structure would receive a bonus experience percentage of 67.5% (22.5% + 15% + 7.5% + 22.5%). A Geyser training here would only receive a 15% bonus experience from the water synergy and a Rhamphyre would gain no bonus experience at all.

### Training Marketplace (TrainingDex)
TrainingDex serves as a marketplace for advertising a landowner’s Training Grounds. Landowners can choose to publicize their Training Grounds on the TrainingDex, allowing rangers to browse and select suitable training facilities. This marketplace promotes player-driven interactions, enriching the player experience and providing another revenue stream for the DAO. The fee is paid by the ranger utilizing the Training Grounds and varies according to the interface they use. The website or mobile app will have the highest fee, while accessing the TrainingDex through Sanctum Mesa incurs the normal fee, and accessing it through the Illuvium Zero results in a discounted fee. The fee would be automatically sold at the current market price, with all proceeds going entirely to the DAO, similar to the fees on the Illuvidex, for revenue distribution.

Introducing the TrainingDex within the current marketplace building seems to be the most logical choice. However, the decision ultimately rests with the team, whether they prefer to integrate this feature into the existing marketplace building, incorporate it into the Training Grounds building, or opt for the creation of an entirely new building dedicated to the TrainingDex.

The TrainingDex UI should be highly intuitive and easy to navigate, offering a range of filtering and sorting options. Landowners should find it effortless to advertise their Training Grounds, needing only to turn it public and set the training cost per tier. Rangers should be able to quickly sort through the available Training Grounds by their building level, illuvial level cap, experience bonuses, training cost, etc…

## Rationale:
The introduction of Training Grounds, Illuvial Staking, and TrainingDex represents a significant step forward in enhancing the player experience and the Illuvium Zero ecosystem. By providing players with avenues to passively train Illuvials, rent out training spaces, and stake Illuvials for bonuses, we are not only bringing our core game assets, Illuvials, to the heart of Illuvium Zero, but also fostering a dynamic and interactive environment where players can engage with one another and their assets in new and exciting ways. Furthermore, the implementation of TrainingDex as a marketplace adds another layer of depth to the game by allowing landowners to monetize their Training Grounds, providing even a way for F2P plots to generate real fuel. All this while also offering an additional source of revenue for the DAO.
