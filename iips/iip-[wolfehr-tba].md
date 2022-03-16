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

# Abstract
Improve the Illuvium Council and Countil election process by
* Expanding the Council to seven seats
* Designate one seat to the Core team
* Stagger elections
* Introduce multiprefernce quadratic voting
* Implement an application with standardized questions

# Motivation
The current election process leads to several challenges.
* Only allowing one candidate leads to a council that doesn't necessarily represent the DAOs preference by hiding the preferences for non-first choice candidates. For example, if Person A were everyone's second choice, they would get no votes despite everyone in the DAO believing they deserved a seat on the Council (given they only picked one person for a five-seat Council). 
* There's no guarantee all stakeholders (e.g., the community, content creators, guilds, core team, investors) will all have a voice in council meetings.
* There's the potential for all council members to turn over at the same time, leading to a loss of institutional knowledge
* There's the danger of people with the most name recognition getting the most votes based on notoriety alone.
* It's difficult to compare candidates


# Specification

## Council Members

The Illivium Council is expanded to seven voting seats and one advisory seat, broken down as follows:

Elected by DAO
* 6 members of the DAO

Elected by Core team
* 1 member of the core team

Council Members serve for 3 epochs (exception for initial rollout as specified below) and can be reelected indefinitely.

### Rationale

There are a lot of voices and opinions in the Illuvium community. Expanding the number of seats allows for more of those voices and opinions to be represented. 

Meetings and decisions can get challenging when there are more than eight people [hrg.org article](https://hbr.org/2018/06/the-most-productive-meetings-have-fewer-than-8-people). You also need an odd number of voting seats to ensure votes don't end in a tie. That leads to the optimum number of voting seats at most seven, with room for an additional person in the conversation.

Content creators and guilds are key stakeholders in the Illuvium ecosystem. The long-term success of the DAO will be bolstered by a close relationship with the people that interact with and use the products the DAO builds. So far it seems those roles are adequately represented on the Council and a specific provision to ensure their representation isn't necessary at this time.

## Staggered Elections
* Council elections will be staggered over 3-month epochs.
* Council members serve for 3 epochs
* Each epoch 2 of the Council members elected by the DAO will go up for election.
* Every fourth epoch (e.g., 1, 4, 7), a Core team member election is also held

### Rationale
Staggering elections ensures the Council never loses too much institutional knowledge at one time. The stagger also allows Council Members to serve for 3 epochs, providing them more time to get integrated and have an impact.

## Multipreference Quadratic Voting (DAO elected seats only)
* DAO members have votes equal to the ILV holdings in wallets they control.
* DAO members can spread their vote over any number of candidates.
* The votes given to a candidate when a DAO member allocates ILV to them will be equal to the square root of the number of ILV allocated. 
* The core team is accountable for determing how to elect their representative. They do not need approval from the DAO on their method of electing a representative.

### Example

A DAO member has 100 ILV. Candidates A, B, C, and D are running. The DAO member could case their votes as follows.

* Candidate A = 10 vILV (10^2 = 100)
* Candidate A = 5 vILV; Candidate B = 5 vILV; Candidate C = 5 vILV; Candidate D = 5 vILV (5^2 * 4 = 100)
* Candidate A = 8 vILV; Candidate B = 6 vILV (8^2 + 6^2 = 100)

### Rationale
This allows DAO members to better express their preferences for who should represent the DAO on the Council. Candidates that have wide support at the DAO but few first choice votes (e.g., everyone's second choice) have a chance at winning a seat.

The Core team should have the freedome to determine how to elect their representative. They only hold one seat, so the DAO should be a sufficient check on their power.

## Standardized Questions

Create an application that includes a set of standardized questions.The following questions will be used as the starting point, but can be modified. The Council will have ownership of maintaining the application, with the DAOs approval via a snapshot vote. 

* How long have you been apart of the Illuvium community?
* Why did you nominate yourself and how do you see yourself representing the community?
* Provide your perspective on an recent IIP. How would you have voted and why?
* Provide your perspective about an discussion in the DAO. What's the issue and how would you approach it as a Council member?
* What is something you'd personally champion in Illuvium during your tensure?
* What's your long-term vision for Illuvium?
* Is there anything else you'd like the DAO to know about you?

### Rationale
Ensures DAO members have information about candidates that will help them make informed decisions. As the representative body of the DAO, the Council is accountable for ensuring the right questions are being asked of candidates. The DAO is a check to ensure the information the DAO wants is on the application.

# Implementation

## Staggered Elections, Expanded Council, and Core Team Member

* Epoch 0 = The current epoch
* The bullets are the seats up for election

Epoch +1
* 6 DAO members [DAO]
* 1 Core team member [Core Team]

Epoc +2
* The 2 DAO voted seats with the 5th and 6th place totals in the Epoch 1

Epoc +3
* The 2 DAO voted seats with the 3rd and 4th place total in Epoch 1

Epoch +4
* The 2 DAO voted seats with the 1st and 2nd place totals in Epoch 1
* 1 Core team member

Epoch +5 and onward
* The 2 DAO voted seats that have served three epochs.
* A Core team member if the current member has served three epochs since last elected

### Multipreference quadratic voting
The council will be accountable for implementing a voting method that meets the requirments in the multipreference quadratic voting section for the election for epoch +1. 

### Standardized questions
The Council will update the application to use the questions specified in the Standardized Questions section. Updates can be proposed by the Council and approved via a snapshot vote that uses quadratic voting.

# Rationale

The rationale is contained inline with the specification as a Justification subsection.

# Test Cases

Not applicable