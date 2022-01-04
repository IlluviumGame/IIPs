---
iip: 15
title: $sILV claims on hold
status: Proposed
author: Kieran Warwick (kieran@illuvium.io)
discussions-to: https://discord.gg/illuvium
created: 2022-01-03
updated: N/A
---

## Simple Summary
We have found a vulnerability in our staking contracts, and as such, the eDAO has had to put a temporary pause on $sILV minting. The attack vector has been closed, and no funds have been compromised. This is purely a protection mechanism for the DAO. This IIP is designed to ratify the eDAO’s decision. 

The vulnerability has been fixed within the staking V2 contracts, and we expect to have them launched shortly. $ILV holders will have plenty of time before the Land Sale to claim their $sILV if they wish. 

## Abstract
sILV minting has been temporarily put on hold until the release of V2 contracts.  

## Overview 
The solidity team has found a potential attack vector that could lead to an attacker being able to mint an unlimited amount of $sILV. The problem doesn’t affect $ILV tokens as they are escrowed for 12 months, the eDAO can easily step in to fix the issue prior to the unlocking and v2 contracts will be live before $ILV yield starts to unlock with the vulnerability patched. It does have the ability to affect $sILV though which is unlocked and is currently being traded on the open market. For this reason, the eDAO needed to take immediate action to remove any potential attack vector. This IIP is designed to formalise and ratify the decision of the eDAO. 

## Rationale
The eDAO couldn’t allow an attacker to potentially hurt the project by minting $sILV and dumping it on the open market. For this reason, they immediately took action and as a result zero funds were lost and the contracts remain safe. 

## Test Cases
N/A.