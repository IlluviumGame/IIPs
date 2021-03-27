---
iip: 3
title: Changes to Illuvium Balancer Liquidity Bootstrapping Pool
status: WIP
author: Delphi Digital (team@delphidigital.io)
discussions-to: https://discord.gg/DrDfmwuBrU
created: 2021-03-27
updated: N/A
---
<!--You can leave these HTML comments in your merged IIP and delete the visible duplicate text guides, they will not appear and may be helpful to refer to if you edit it again. This is the suggested template for new IIPs. Note that an IIP number will be assigned by an editor. When opening a pull request to submit your IIP, please use an abbreviated title in the filename, `iip-draft_title_abbrev.md`. The title should be 44 characters or less.-->


## Overview
<!--A short (~200 word) description of the proposed change, the abstract should clearly describe the proposed change. This is what *will* be done if the IIP is implemented, not *why* it should be done or *how* it will be done. If the IIP proposes deploying a new contract, write, "we propose to deploy a new contract that will do x".-->

As investors in Illuvium, our team at Delphi Digital couldn’t be more optimistic about the future of the game and what the team has been working so hard on. On March 30th, Illuvium’s governance token ILV will finally launch via Balancer’s Liquidity Bootstrapping Protocol – this is an exciting event. We believe the current design of the LBP is well thought out, but there’s just one element that we’d like to propose to shift, the starting price. If you’ve spent any time in Illuvium’s discord, it’s inspiring to see how strong of a community has already formed despite Illuvium’s game not being launched yet.

We believe a starting price of $50 is much more appropriate. It’s the ideal way to allow the existing community to purchase at a favorable level, while still ending the sale at a price that reflects current demand. It’s important to note that regardless of the starting price, Balancer’s LBP allows the final price of the ILV token to settle at a level that reflects current demand.

As the initial proposal described, price action during an LBP is the result of a push and pull between the weight change (that drives price down) and the buyers (that drive price up). This means price decline is steady and predictable while price rise is sporadic. Looking at historical LBP data shows that price typically spikes early on as people rush in, declines as demand slows down (relative to the initial bid) and weights change, and then picks back up as we enter price discovery mode, typically ending above the starting level. We believe that starting lower helps create a healthy trajectory while also allowing the early community members to buy in a more favorable level. One thing we’ve learned is that strong communities are incredibly important, and there’s no better way to bolster that community than allowing them to invest at levels that align them in the long run with the project.
Regardless of what is decided here, we are still strong supporters of Illuvium and believe the community will rally around its vision. We just thought it would be worth sharing our thoughts here and letting the community/council decide how to best proceed given our feedback. 


## Specification
<!--The specification should describe the syntax and semantics of any new feature, there are five sections
1. Overview
2. Rationale
3. Technical Specification
4. Test Cases
5. Configurable Values
-->

* **New Starting Price:** $50 (in ETH)

### Test Cases
<!--Test cases for an implementation are mandatory for IIPs but can be included with the implementation..-->
N/A


## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).