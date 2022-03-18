---
iip: 18
title: Illuvium Staking v2
status: Proposed
author: Kieran Warwick (kieran@illuvium.io)
discussions-to: https://discord.gg/illuvium
created: 2022-03-18
updated: N/A
---

## Simple Summary

After collecting months of user feedback since the launch of the Illuvium Staking Contracts v1, the Illuvium team has designed a new set of smart contracts that implement additional features, gas optimisations, and security fixes. The goal is to deploy a better version of staking with a smoother UX and prepare the Illuvium protocol with a more flexible set of contracts for future features.

## Abstract

After a long delay, followed by a complete rework of the smart contracts to mitigate issues found in the v1 code, we are ready to deploy a new set of smart contracts. We concluded an external review from White Hat Samczsun, two external audits, and an internal audit. We are fully confident in the deployment and security of this product. All that remains is some minor quality assurance checks post-IIP approval.

Upgrading to Staking v2 will be mandatory as the upgrade requires the existing contracts to be deprecated.

The launch will be accompanied by an article and explainer video for new users, helping them to understand what Staking v2 is, as well as a detailed upgrade document and a video tutorial that guides token holders and makes the entire upgrade process as painless as possible. It includes user scenarios for different situations, such as flexible deposits.

## Overview

The exact date to begin rewards will be specified before deployment but should take no longer than one week. We require users to upgrade to v2 and receive many benefits and improvements in exchange.

Please see Definitions before reading to become familiar with the exact terminology.

### Upgrade Process

Staking v1 users must upgrade to v2 before receiving yield; however, they can still upgrade after the window closes.

A Merkle Tree of each user’s accumulated yield weight in v1 will be published and stored in IPFS for full transparency. Anyone will be able to verify the authenticity of the data.

**A detailed process for each type of stake:**

- Flexible Deposit in ILV Pool - Doesn’t count to yield in v2 unless unstaked and locked for a minimum period of 1 month in v2.

- Flexible Deposit in LP Pool - Doesn’t count to yield in v2 unless unstaked and locked for a minimum of 1 month in v2.

- Locked Deposit in ILV Pool - Counts to yield rewards after upgrading to v2 at the current weight.

- Unlocked Deposit in ILV Pool - Counts to yield rewards after upgrading to v2 at the current weight.

- Locked Deposit in LP Pool - Counts to yield rewards after upgrading to v2 at the current weight.

- Unlocked Deposit in LP Pool - Counts to yield rewards after upgrading to v2 at the current weight.

- Locked ILV Yield - Counts to yield rewards after upgrading to v2 at the current weight.

- Unlocked ILV Yield - N/A (Has not been 12 months since launch but will continue to count to yield rewards even after unlocked).

- Seed and Team - Automatically migrated to v2 and not counted towards yield.

### Main Changes

**Rewards Claiming**

Users will no longer be required to claim every stake or unstake function. This selection will only be required when claiming rewards, which users can now do for all pools in a single transaction. Users will also be able to unstake all unlocked tokens in a single transaction.

**Fixes and Gas Optimisations**

The new architecture comes with multiple gas optimisations by reducing the number of storage slots used by the deposit data structure, using new yield processing flows, and optimising the number of reads. These optimisations will make transactions cheaper.

**Transfer Positions**

Frequently asked by the community, user can transfer their v2 deposits to new addresses, which can be helpful in situations such as when a personal private key is leaked or anything that could motivate a user to move into a new Ethereum address.

v1 locked positions are still unable to be moved to new addresses.

**Upgradeability**

Staking v2 (Factory, Core Pools, and Flash Pools) implements the Universal Upgradeable Proxy Standard, allowing Council members to vote on upgrades proposed to the contracts, opening many possibilities for future Illuvium staking features and even for new products. It brings new powers to ILV token holders and reinforces our Govern-To-Earn mantra. With upgradeability, there is a lot of flexibility for new IIPs and the evolution of Illuvium DAO as a whole.

**Flexible Staking Removed**

We removed flexible staking in v2 to encourage users to commit to the project. Locking further reduces circulation, which puts upward pressure on the token. Weight calculations still follow the same 1 → 2 multiplier used in v1, which keeps the system fair and balanced for the long term.

The maximum locked period is still one year (2.0 weight).

**NFT Distributions**

A separate IIP is in progress with more details on the NFT distribution integration, but Staking v2 will include all the features required to make this integration seamless.

**Changes From Initial Proposal**

**Migration**

Our engineers removed migration from the contracts due to the added complexity in the v2 rework. Functionally, migration allowed users to pay a fee to transfer unlocked deposits to v2 while keeping their weight. Instead, the new contracts enable users to maintain that weight without doing anything. For smaller stakers, this is a win. For larger stakers, this will probably result in slightly higher gas fees.

We still plan to add migration through a helper contract, but we do not have a fixed timeline. The current advice for larger stakers is to unstake from v1 and restake in v2. Staking v2 is still far cheaper than v1, however for gas optimisation, all deposits should be in v2.

**Transfer Wallets**

The transfer wallet feature is restricted to wallets with no v1 staking history for security reasons. We recommend that users create a new wallet to begin staking in v2 if they would like to use this feature.

Exception - If you only deposited into the LP pool in v1, then v2 deposits can be transferred. We will investigate possible future upgrades that could return this feature for other users.

## Rationale

Staking v2 will be a big step for Illuvium DAO and bring many enhancements and fixes to the protocol collected since the v1 launch. With a lower gas cost, Illuvium DAO should have access to more users with a lower barrier to entry and a more straightforward user experience due to the flow changes and fixes. Contract upgradeability ensures that any future changes are swift and will empower the community with even more effective governance.

## Definitions

- **Locked Deposit** - This is when a user has staked tokens with a lock, and the lock has not yet expired.

- **Unlocked Deposit** - This is when a user has staked tokens with a lock, and the lock has expired.

- **Flexible Deposit** - This is when a user has staked tokens with no lock.

- **Locked ILV Yield** - Yield claimed and locked for 12 months.

- **Unlocked ILV Yield** - Yield claimed more than 12 months ago and hence unlocked.

- **Upgrade to v2** - Allowing v2 contract to read the v1 state and calculating yield in the v2 contract.

- **Migrate** - The process of taking an Unlocked Deposit in v1 and unstaking it, then restaking it v2 with the original weight.

- **Withdraw** - Unstaking a Flexible or Unlocked Deposit (but not migrating it to v2).

- **Pending Rewards** - The rewards that remained at the staking v1 end block when we paused rewards.

- **Accumulated Rewards** - The yield rewards earned from the pause until the resumption of yield. We calculate these manually.

## Test Cases

N/A.
