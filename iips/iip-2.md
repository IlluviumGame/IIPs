---
iip: 2
title: Illuvium Balancer Liquidity Bootstrapping Pool
status: Approved
author: Kieran Warwick (kieran@illuvium.io)
discussions-to: https://discord.gg/DrDfmwuBrU
created: 2021-03-22
updated: N/A
---
<!--You can leave these HTML comments in your merged IIP and delete the visible duplicate text guides, they will not appear and may be helpful to refer to if you edit it again. This is the suggested template for new IIPs. Note that an IIP number will be assigned by an editor. When opening a pull request to submit your IIP, please use an abbreviated title in the filename, `iip-draft_title_abbrev.md`. The title should be 44 characters or less.-->


## Simple Summary
<!--"If you can't explain it simply, you don't understand it well enough." Simply describe the outcome the proposed changes intends to achieve. This should be non-technical and accessible to a casual community member.-->
Creates Illuvium's Balancer Liquidity Bootstrapping Pool to be launched on March 30.

## Abstract
<!--A short (~200 word) description of the proposed change, the abstract should clearly describe the proposed change. This is what *will* be done if the IIP is implemented, not *why* it should be done or *how* it will be done. If the IIP proposes deploying a new contract, write, "we propose to deploy a new contract that will do x".-->

A Balancer Liquidity Bootstrapping Pool is designed to allow DeFi protocols to acquire capital from a smaller amount of liquidity than would usually be required when seeding a pool such as Uniswap or Sushiswap. The IIP proposes to create Illuvium's pool and launch the IDO on March 30.


## Specification
<!--The specification should describe the syntax and semantics of any new feature, there are five sections
1. Overview
2. Rationale
3. Technical Specification
4. Test Cases
5. Configurable Values
-->
* **Starting weights:** 96:4
* **End weights:** 50:50
* **Pair:** ETH/ILV
* **Starting Price:** $100 (in ETH)
* **Duration:** 72 hours
* **Token Supply:** 1 million


* **Token Contract Address:** 0x767fe9edc9e0df98e07454847909b5e959d7ca0e
* **Token Symbol:** ILV
* **Decimals of Precision:** 18


### Overview
<!--This is a high level overview of *how* the IIP will solve the problem. The overview should clearly describe how the new feature will be implemented.-->
Utilizing Balancer for our Launchpad we are able to fairly distribute 1,000,000 tokens subject to no lockup that will enable a healthy and stable price discovery process. In a BLBP the weights change over time to create downward pressure, so when the pool goes live, the price will begin to decline, which is why the initial price of the token is set to a high value.

There are two competing forces for the price of the token in a BLBP. The changing of the weights of the tokens will naturally push the price of the token down, since the weights start out with the token being worth the majority of the pool’s value, and end up at a much lower level. The other force is trading of the token. As people purchase the token, the number of tokens in the pool decreases, but the value of those tokens must still match the weights, so the price of the token increases to compensate.

What you will see is a gradual drop in token price, matched by periodic ‘bumps’ where the token goes back up. In theory, the price should eventually find some value that the overall market finds to be an accurate value for the token.


At the end of the IDO, the US dollar value of all purchases converts to points at a rate of one point per USD. These points can be used to redeem promo NFTs that will only be available for a short period of time following the sale. This applies only to those who hold all of their ILV purchases after the sale concludes until the NFTs redeem window is closed.


### Rationale
<!--This is where you explain the reasoning behind how you propose to solve the problem. Why did you propose to implement the change in this way, what were the considerations and trade-offs. The rationale fleshes out what motivated the design and why particular design decisions were made. It should describe alternate designs that were considered and related work. The rationale may also provide evidence of consensus within the community, and should discuss important objections or concerns raised during discussion.-->
This will be the public’s first chance to acquire ILV outside of the two Discord Airdrops. Balancer was chosen because it is the fairest way to distribute the tokens, which has been proven with many projects. Other options would be to use 50/50 AMMs like Uniswap and Sushiswap, which would require more liquidity to be added, and are not as suited for decentralized initial offerings as Balancer Smart Pools.



### Test Cases
<!--Test cases for an implementation are mandatory for IIPs but can be included with the implementation..-->
N/A


## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).