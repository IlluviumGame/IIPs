---
iip: 16
title: $sILV reimbursement
status: Proposed
author: Kieran Warwick (kieran@illuvium.io)
discussions-to: https://discord.gg/illuvium
created: 2022-01-14
updated: N/A
---

## Simple Summary
The council will decide if the DAO reimburses those who traded in the unofficial Uniswap sILV pool after the eDAO rescued the LP providers.

## Abstract
Should the DAO reimburse people who traded in the sILV pool after the recovery transaction? (block 13940834)  

## Overview 
On January 3rd, 2022, analysts discovered a vulnerability in our staking contracts, allowing an attacker to mint an unlimited amount of $sILV. The executioner DAO (eDAO) temporarily paused sILV minting until the release of Staking V2, fixing the vulnerability. We believed no attackers took advantage of the exploit at the time. We made this announcement on [Discord](https://discord.com/channels/760344898200666112/768749374255398943/927732522782191616) and our [socials](https://twitter.com/illuviumio/status/1478191824556621825).

However, the attacker had been minting sILV using many addresses over a long period so they would remain undetected. Through this, they were able to mint approximately 8,000 sILV.  

After our announcements about the vulnerability and the pausing of sILV minting, the attacker realised we had discovered the exploit and started to sell their sILV tokens and began draining the Uniswap pool. Had this been allowed to happen, the LP providers would have lost all their liquidity. As such, the eDAO held an emergency meeting and decided to mint a large amount of sILV and sold this into the pool, effectively dropping the price of sILV to zero. The eDAO stored this value with the intention to distribute it back to those affected at a later date.

The council had already decided to reimburse all Liquidity Providers and trades before the announcement and rescue transaction (block 13940834). Still, it was yet to determine if it would allow for a grace period after the rescue transaction for those that bought sILV after it had dropped to zero. The purpose of this IIP is to decide whether the Council should give a grace period to those affected.


## Rationale
We received enough feedback from affected users who traded after the rescue transaction to warrant an IIP. However, trades that happened after the snapshot are incredibly complex. It is difficult to determine the impact objectively, especially considering the ability of bad actors to game the system once they knew that sILV would be worthless.
As such, the Council must make the final decision.

## Test Cases
N/A.
