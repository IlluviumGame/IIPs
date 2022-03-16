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
Make it easier for DAO members to learn about candidates, express their preferences, and ensure all stakeholders have representation on the Council. 
* Creating a more robust, standardized application process
* Creating a centralized location to store applicant content (e.g., interviews, the application)
* Expanding the Council to seven seats
* Creating roles for key stakeholders on the Council
* Staggering Council Member elections 
* Allow voting for multiple candidates

# Abstract
Improvements to the Illuvium Council and Countil election process.

# Motivation
The current election process leads to several challenges.
* It's difficult to compare candidates
* Information about candidates is spread over many places (discord, illuvium.io governance, youtube). Without an organizational structure, the information can be challenging to find.
* There's the danger of people with the most name recognition getting the most votes based on notoriety alone.
* There's no guarantee all stakeholders (e.g., the community, content creators, guilds, core team, investors) will all have a voice in council meetings.
* There's the potential for all council members to turn over at the same time, leading to a loss of institutional knowledge
* Only allowing one candidate leads to a council that doesn't necessarily represent the DAOs preference by hiding the preferences for non-first choice candidates. For example, if Person A were everyone's second choice, they would get no votes despite everyone in the DAO believing they deserved a seat on the Council (given they only picked one person for a five-seat Council). 

# Specification

## Council Members

The Illivium Council is expanded to seven voting seats and one advisory seat, broken down as follows:

Elected by DAO
* 5 members of the DAO
* 1 content creator (voting or advisory)
* 1 guild representative (voting or advisor)

Elected by Core team
* 1 member of the core team

Content creators and guild representatives will both apply for the same seat, and someone can only apply for one. The application will specify the role and specific entity (e.g., Guild/[guild name] or Content Creator/[YouTube Channel]). This question will be part of the standardized application Council. The person with the most votes will win a voting seat. The person with the most votes representing the other role wins an advisory seat. This means the voting and advisory seats will always turn over simultaneously. For example, 

Voting results
1. Person A (Guild) = 100 vILV (voting seat)
2. Person B (Guild) = 90 vILV
3. Person C (Content Creator) = 85 vILV (advisory seat)

Council Members serve for 3 epochs (exception for initial rollout as specified below) and can be reelected indefinitely.

### Justification
Content creators and guilds are key stakeholders in the Illuvium ecosystem. The long-term success of the DAO will be bolstered by a close relationship with the people that interact with and use the products the DAO builds. 

Meetings and decisions can get challenging when there are more than eight people [hrg.org article](https://hbr.org/2018/06/the-most-productive-meetings-have-fewer-than-8-people). You also need an odd number of voting seats to ensure votes don't end in a tie.

That leads to the optimum number of voting seats at most seven, with room for an additional person in the conversation. The content creator and guild representatives both represent users, so they were chosen to be compressed into one voting role, with the other role (i.e, content creator or guild representative) in the advisory role, so they still have a voice. 

## Staggered Elections
* Council elections will be staggered over 3-month epochs.
* Council members serve for 3 epochs
* Each epoch 2 of the Council members elected by the DAO will go up for election.
* Every fourth epoch (e.g., 1, 4, 7), a Core team member election is also held
* The epoch where the content creator or guild representative is up for election, the person with the most overall votes wins a voting seat, and the person with the most votes from the other role will win an advisory role.
* The DAO will vote using the multipreference quadratic voting described below. The core team can use the same method or opt for another method of their choosing.

### Justification
Staggering elections ensures the Council never loses too much institutional knowledge at one time. The stagger also allows Council Members to serve for 3 epochs, providing them more time to get integrated and have an impact.

## Multipreference Quadratic Voting
* DAO members have votes equal to the ILV holdings in wallets they control.
* DAO members can spread their vote over any number of candidates.
* The votes given to a candidate when a DAO member allocates ILV to them will be equal to the square root of the number of ILV allocated. 

### Example

A DAO member has 100 ILV. Candidates A, B, C, and D are running. The DAO member could case their votes as follows.

* Candidate A = 10 vILV (10^2 = 100)
* Candidate A = 5 vILV; Candidate B = 5 vILV; Candidate C = 5 vILV; Candidate D = 5 vILV (5^2 * 4 = 100)
* Candidate A = 8 vILV; Candidate B = 6 vILV (8^2 + 6^2 = 100)

### Justification
This allows DAO members to better express their preferences for who should represent the DAO on the Council. Candidates that have wide support at the DAO but few first choice votes (e.g., everyone's second choice) have a chance at winning a seat.

## Standardized Questions
The Council will have ownership, with the DAOs approval, of creating an application that includes a set of standardized questions.

### Justification
Ensures DAO members have information about candidates that will help them make informed decisions. As the representative body of the DAO, the Council is accountable for ensuring the right questions are being asked of candidates. The DAO is a check to ensure the information the DAO wants is on the application.

## Election Hub
Illuvium will provide an election hub where applications are available quickly, and candidates can attach additional material (e.g., links to interviews or past work). The specific implementation will be left up to the core team. The crux of this specification is the information is available easily to DAO members.

### Justification
Making the information available quickly provides DAO members the most time to make an informed decision. Allowing candidates to attach additional information allows them to make information easily accessible.

# Implementation

## Elections

Notes
* Epoch 0 = The current epoch
* The bullets are the seats up for election

Epoch +1
* 5 DAO members [DAO]
* 1 Content Creator or Guild Rep (plus 1 advisory seat) [DAO]
* 1 Core team member [Core Team]

Epoc +2
* The 2 DAO voted seats with the 5th and 6th place totals in the Epoch 1

Epoc +3
* The 2 DAO voted seats with the 3rd and 4th place total in Epoch 1

Epoch +4
* The 2 DAO voted seats with the 1st and 2nd place totals in Epoch 1
* 1 Core team member

Epoch +5 and onward
* The 2 DAO voted seats that have served three epochs. If one of those seats is the Content Creator/Guild Representative seat, the advisory seat will also change.
* A Core team member if the current member has served three epochs since last elected

## Election Hub
The core team will propose an IIP that meets the requirements in the Election Hub section by the end of the epoch following the one in which this IIP passes.

# Rationale

The rationale is contained inline with the specification as a Justification subsection.

# Test Cases

Not applicable