---
iip: 29
title: Safety Pool
status: Pending
author: Blickter (Blickter#8107)
discussions-to: https://discord.gg/illuvium
created: 2023-01-04
updated: 2023-01-26
---

## Simple Summary
Create a Safety Pool within the Illuvium Treasury. The Safety Pool is a separate grouping of funds up to a maximum of $15M USDT. The Safety Pool may be utilized to cover DAO costs. Alternatively, the funds in the Safety Pool may be transferred to the Vault for regular distribution.

## Overview
The Safety Pool will be held by the DAO as USDT, and tracked separately from other Treasury assets. This will enable on-chain transparency for Safety Pool funds. Additional proposals, such as ICCP-4, must specify what revenue will fund the Safety Pool. If not specified by IIP or ICCP, revenue will go to the Vault for distribution.

Revenue generated from purchases will be swapped for USDT on the open market and moved directly into this wallet. Any revenue in excess of $15M USDT will be treated as normal revenue, and will go to the Vault for distribution.

## Rationale
The implementation of the Safety Pool is in response to broader market conditions and uncertainty. It is critical that the DAO provides stability and engages in conservative risk-management strategies. This implementation provides additional flexibility as compared to diverting revenue directly into the Treasury. USDT was chosen to avoid reduce risk associated with market trends, and to provide a separate currency from USDC for tracking purposes. Additionally, as a standalone proposal, it is more straightforward to release funds from the Safety Pool, or to modify values within the Safety Pool in the future.

## Sizing the Safety Pool
The Council chose the size of the Safety Pool ($15M USDT) after consulting the internal team, who recommended that amount to cover approximately two years of development and costs based on current expenditure projections and existing stablecoin runway.

## Utilizing the Safety Pool
The Safety Pool can only be utilized by the DAO via an ICCP and the amount and reason must be specified. Any portion of the Safety Pool may be utilized in this way.

If other revenue sources are sufficient to fund the DAO, the Safety Pool may be transferred to the Vault for regular distributions via ICCP. 
