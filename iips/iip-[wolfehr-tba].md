---
iip: tbd
title: Illuvium Council Election Improvements
status: WIP
author: Heath Wolfeld (@wolfehr)
discussions-to: tbd
created: tbd
updated: 2022/03/10
---

# Simple Summary
Make it easier for DAO members to learn about candidates, express their preferences, and ensure all stakeholders have representation on the council. 
* Creating a more robust, standardized application process
* Creating a centralized location to store applicant content (e.g., interviews, the application)
* Expanding the council to seven seats
* Creating roles for key stakeholders on the Council
* Staggering Council Member elections 
* Allow voting for multiple candidates

# Abstract
Improvements to the Illuvium Council and Countil election process.

# Motivation
The current election process leads to a number of challenges.
* It's difficult to compare candidates
* Information about candidates is spread over a number of different places (discord, illuvium.io governance, youtube). Without an organizational structure the information can be difficult to find.
* There's the danger of people with the most name recognition getting the most votes based on notoriety alone.
* There's no gurantee all stakeholders (e.g., the community, content creators, guilds, core team, investors) will all a voice in council meetings.
* There's the potential for all council members to turn over at the same time, leading to a loss of institutional knowledge
* Only allowing one candidate leads to a council that doesn't necessarily represent the DAOs preference by hiding the preferences for non-first choice candidates. For example, if Person A was everyone's second choice, they would get no votes despite everyone in the DAO believing they deserved a seat on the council (given they only picked one person for a five seat council). 

# Specification

## Council Changes

The Illivium Council is expanded to seven voting setas and one advisory seat, broken down as follows

Elected by DAO
* 5 members of the DAO
* 1 content creator (voting or advisory)
* 1 guild representative (voting or advisor)

Elected by Core team
* 1 member of the core team



### Justification
Content creators and guilds are key stakeholdes in the Illuvium ecosystem. The long term success of the DAO will bolstered by a close relationship with the people that interact with and use the products the DAO builds. 

Meetings and decisions can get challening when there are more than 8 people [hrg.org article](https://hbr.org/2018/06/the-most-productive-meetings-have-fewer-than-8-people). You also need an odd number of voting seats to ensure votes don't end in a tie. That leads to the optimium number of voting seats to be at most seven, with room for an additional person in the coversation. The content creator and guild representatives both represent users so they were chosen to be compresed into one voting role, with the other role (i.e, content creator or guild representative) in the advisory role so they still have a voice. 

### Staggered Elections
* Council elecitons will be staggered over 3 month epochs.
* Council members serve for 3 epochs
* Each epoch 2 of the Council members elected by the DAO will go up for election.
* Every fouth epoch (e.g., 1, 4, 7) a Core team member election is also held
* The epoch where the content creator or guild representative is up for election, the person with the most overall votes wins a voting seat and the person with the most votes from the other role will win an advisory role.
* The DAO will vote using the multipreference quadratic voting described below. The core team can use the same method, or opt for another method of their chosing.

### Multipreference Quadratic Voting
* DAO members have votes equal to the ILV holdings in wallets they control.
* DAO members can spread their vote over any number of candidates.
* The votes given to a candidate when a DAO member allocates ILV to them will be equal to the square root of the number of ILV allocated. 

### Example

A DAO member has 100 ILV. Candidates A, B, C, and D are running. The DAO member could case their votes as follows.

|Candidate A|Candidate B|Candidate C|Candidate D|Vote Math|
|---|---|---|---|
|10|0|0|0|









