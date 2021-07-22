---
iip: 7
title: Flash Pools V2
status: Proposed
author: Kieran Warwick (kieran@illuvium.io)
discussions-to: https://discord.gg/illuvium
created: 2021-07-22
updated: N/A
---

## Simple Summary
The Illuvium dev team has found a limitation in the Flash Pools contract, and as
such, we have designed a new contract to give us the flexibility to deploy all current
ERC-20 tokens.

## Abstract 
We implement Flash Pools using the existing V1 contract while Quantstamp audits
Flash Pools V2. Once complete, token XYZ will be the first Flash Pool v2 deployed.

## Overview
Illuvium core devs have found a limitation in the existing Flash Pools contract due to
an issue with precision, and tokens with extremely large supply cant be launched.
For this reason, I am suggesting we launch the AXS Flash Pool utilizing the audited
v1 contract. Once audited, the XYZ token would become the first Flash Pool v2.
Preceding this would be a fortnightly council vote that includes multiple tokens of
interest that have been discussed in the Illuvium Governance channel within Discord.
 
## Rationale
Flash Pools are a great marketing tool, and the above solution allows us to safely
continue launching v1 pools while waiting for the v2 contract to be audited. Delaying
Flash Pools further may negatively impact the community and doesn’t seem
necessary given the workaround above.

### Test Cases
N/A

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
