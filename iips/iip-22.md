---
iip: 22
title: Revenue Distribution
status: Proposed
author: Aaron Warwick
discussions-to: https://discord.gg/illuvium
created: 2022-05-31
updated: N/A
---

## Simple Summary

The token buyback function is a simple mechanism to smooth revenue distribution. We favour simplicity over complexity for several reasons, but primarily because we can achieve all the goals with a more straightforward system that is easy to understand.

## Abstract

Following months of discussion with the community, we propose a simple mechanism for handling revenue distributions. Our solution achieves all the following goals:

- Smoothly distribute smaller or larger amounts depending on revenue fluctuations.

- Limit the maximum distribution amount so we do not distribute considerable quantities in a single day.

- It should be theoretically possible to distribute everything.

- It should limit the number of transactions to minimise gas.

- It should mitigate front running and sandwich attacks.

## Overview

Interested parties should read the White Paper to understand the distinction between the Vault, the Treasury, and where we generate revenue.

The proposed mechanism distributes a daily target amount, defined as a fixed percentage of the entire Vault. However, if the target is higher or lower than a fixed minimum or maximum, we use those values instead. The Daily Distribution then gets broken into several smaller, randomised values to smooth the price impact. Randomising the values makes it impossible to know how many transactions remain in the day, protecting against frontrunning.

![Formula](../assets/iip-22/formula.png)

**Example - Converting Daily Distribution into individual transactions**

Daily Distribution = 2,000 ETH.

Transaction 1: 123

Transaction 2: 654

Transaction 3: 87

Transaction 4: 31

Transaction 5: 1105

Total: 2000 ETH

This process works by choosing smaller random amounts until we reach the total.

**Definitions**

**MinMax():** A function that takes three inputs (min, max, and target) and outputs the target, unless it is lower or higher than the minimum and maximum.

**Daily Distribution:** The total distributed for that day, in ETH.

ETH is swapped for ILV before distribution, but we always measure the amount in ETH.

**V(snapshot):** Daily Vault Snapshot (i.e. the total value of ETH in the Vault at the start of the day)

**R(min):** The minimum daily revenue distribution.

If V < R(min), V is substituted for R(min), which means that if we don’t have enough in the Vault to distribute the minimum, we distribute the entire contents of the Vault.

**R(max):** The maximum daily revenue distribution.

**T:** The target percentage of the Vault to distribute per day.

**Proposed Configuration Variables**

Updates to the variables occur via ICCP

R(min): **500 ETH**

R(max): **5000 ETH**

T: **15%**

Additionally, we set a slippage limit such that the transaction fails if the slippage is higher than the slippage limit. The proposed slippage limit is **3%**.

**Worked Examples - Total Daily Distribution**
**Each example uses the originally proposed configuration variables. The new proposed variable for T is 15%.**

**Example - Using the Target Range Distribution**
Day 1: The Vault contains 10,000 ETH. The daily target is therefore 10,000 \* 20% = 2,000 ETH. Since this value is within the correct range, we distribute exactly 2,000 ETH. At the end of the first day, the Vault will have 8,000 ETH.

Day 2: The Vault contains 8,000 ETH. The daily target is therefore 8,000 \* 20% = 1,600 ETH. Since this value is within the correct range, we distribute exactly 1,600 ETH. At the end of the second day, the Vault will have 6,400 ETH.

**Example - Using Minimum Value Distribution**
Day 1: The Vault contains 1,000 ETH. The daily target is therefore 1000 \* 20% = 200 ETH. Since this value is lower than the minimum daily distribution of 500 ETH, we distribute 500 ETH instead. At the end of the first day, the Vault will have 500 ETH.

Day 2: The Vault contains 500 ETH. The daily target is therefore 500 \* 20% = 100 ETH. Since this value is lower than the minimum daily distribution of 500 ETH, we distribute 500 ETH instead. At the end of the second day, the Vault will now have 0 ETH.

The best way to think about this scenario is that, when low, the Vault will keep distributing until it is empty, ensuring distributions are reasonably quick.

Lowering the minimum daily distribution increases the time taken for the Vault to empty.

Raising the minimum daily distribution decreases the time the Vault takes to empty.

**Example - Using Maximum Value Distribution**

Day 1: The Vault contains 50,000 ETH. The daily target is therefore 50,000 \* 20% = 10,000 ETH. Since this value is higher than the maximum daily distribution of 5,000 ETH, we distribute 5,000 ETH instead. At the end of the first day, the Vault will have 45,000 ETH.

Day 2: The Vault contains 45,000 ETH. The daily target is therefore 45,000 \* 20% = 9,000 ETH. Since this value is higher than the maximum daily distribution of 5,000 ETH, we distribute 5,000 ETH instead. At the end of the second day, the Vault will have 40,000 ETH.

The best way to think about this scenario is that, when high, the Vault will keep distributing the maximum amount allowable per day.

Lowering the maximum daily distribution increases the time taken for the Vault to decrease into the normal range.

Raising the maximum daily distribution decreases the time taken for the Vault to decrease into the normal range.

## Discussions

**Rewarding Long-Term Stakers**
Revenue distribution only considers those currently staked and only at their current weight. Since upgrading to Staking v2, everyone must have a staking period of at least one month, receiving the smallest weighting. Doing this rewards those with longer lock durations and eliminates the risk of someone staking for a single day to receive rewards. However, there are many more optimisations available.

Unlike yield, revenue distribution does not distinguish between pools. It only cares that you are staked in one of the pools, so pool weights are not considered.

**Revenue Distribution Lag:** Currently, potential stakers can judge the outcome of more significant events and then decide if they wish to stake. By introducing a lag (1 or 2 weeks), we could incentivise those parties to stake before the sale.

**Reduce Minimum Weight or Increase the Minimum Lock Period:** The simplest method to reward long-term stakers further would be to reduce the minimum weight (i.e. Change the weight for 1-month stakers from 1 → 1/12 or some other fraction) or increase the lock period.

**Increase the weight for ultra long-term stakers:** Add new weights for lock durations greater than one year.

**Require relocking tokens at the end of their locking period:** The percentage of the total supply that is locked is an important metric. The project appears less stable if we do not require relocking.

**Changing to ETH-Based Distribution**

Even though the above system is relatively simple, some complexities and trust are still required from those outside the eDAO. For example, even though we randomise and hide the purchases, members of the private mempool can see the purchases and profit from them. While a minor risk, since these malicious actors are removed near instantly from the group, it is still a consideration. A more substantial consideration is the sell actions of the DAO to fund development. An ICCP must accompany these, and making them public allows malicious actors to benefit. Again, there are many ways to mitigate these issues, but the most straightforward approach to increasing reliability and security is eliminating moving parts.

The benefits of distribution in ETH (technically wETH) are numerous:

- Complete removal of any risks associated with sandwich attacks.

- Provides an entirely trustless system of distribution.

- Reduces fees.

- Eliminates the need for randomness and smaller distributions.

The downside of distribution in ETH is:

- There is no price action on the token, except for those that choose to swap ETH for more ILV directly. Illuvium Labs could build this type of “reinvestment option” to make it easy for stakers.

Regardless of the appetite for this change, we should be prudent and start by using the current revenue distribution system. Any change requires reengineering the contracts, and it makes sense to move away from the current system only if experience shows it is suboptimal.

**We encourage the community to discuss these changes. They are not required to proceed, but interested parties must understand the options. An appropriate time to include any significant changes (i.e. An IIP rather than ICCP) would be during the development of Staking v3, which targets a Layer 2 launch.**

## Rationale

Revenue distribution must be simple and understandable. The proposed mechanism is robust and gives the Council the power to adjust the parameters quickly. It limits frontrunning and slippage as much as possible and rewards stakers based on the duration of their lock.

Additionally, it ensures that the Vault has a mechanism to empty and smooth out distributions when it encounters spikes in revenue

## Test Cases

N/A
