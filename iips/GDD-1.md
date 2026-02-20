GDD: 1
title: Illuvium: DEATHMATCH
status: Pending
Sponsor: Nill
Key Contributors: Illuvium Team
discussions-to: https://discord.com/channels/760344898200666112/1470904125649584340
---
## Game Overview:

**1.1 Title**
Illuvium: Deathmatch 

**1.2 Concept**
A high-stakes battle royale where players choose an Illuvial to fight against other players’ Illuvials within a limited perimeter. Strategy, skill, and survival are pushed to the limits, with permanent consequences or glorious rewards for every challenger. Top survivors and killers earn valuable real money and in-game rewards, making each match a thrilling fight for glory and real stakes.

**1.3 Genres**
Risk to Earn
Battle Royale
Strategy
Gambling

**1.4 Platforms**
Initially: Browser (PC & Mobile).

**1.5 Unique Selling Points**
Risk to Earn mechanic combined with Illuvium’s IP (Illuvials, Regions and Web3 Ownership).

**1.6 Expansion Potential**
While this MVP delivers a gambling-first experience, it lays the foundation for future game modes that will enhance the traditional gaming side of the experience. The user experience has been designed to be simple, making the game accessible to a broad spectrum of players. If the MVP proves successful, we plan to introduce a game mode that expands in-fight possibilities, allowing players to command and boost their Illuvials during combat.

## Gameplay & Mechanics:

**2.1 Core Elements / Glossary**

a) **Challenger:** The Illuvial you pick for a specific match.

b) **Jackpot:** An accumulative prize that accrues throughout the matches.
	→ Each game mode has its own specific Jackpot.

c) **Prize Pool:** Specific rewards based on fees collected in that particular match.

d) **Winner:** The Challenger that is left standing. 
→Is not exposed to Permadeath. 
→Only the Winner gets a chance at winning the Jackpot.

e) **Top Survivors:** Top Challengers to last more in combat.
	→ Get access to Prize Pool rewards.See section 3.3.

f) **Top Executioners:** Top 3 Challengers per Combat Dome to slay the most enemies.
	*Note that in case of draw, tiebreaker would be most damage dealt.
	→ Are not exposed to Permadeath.
	→ Get rewarded the top 3 TPI challengers that would have suffered permadeath.

g) **Permadeath:** Challengers that die in Deathmatch are burnt, permanently erased.

h) **Loadout:** Set of equipment and actions performed before the fighting phase begins.

i) **Combat Booster Wheels:** Casino-style wheels whose outcome boosts the combat performance of your Challenger.
	→ Spinning costs credits, each spin is more expensive than the previous.

j) **Combat Dome:** Refers to a fighting instance, composed of 10-100 players.

k) **Dome Boundary:** Refers to the Combat Dome perimeter, which shrinks over time.
	→ Challengers will prioritize stepping inside the Boundary rather than attacking.
	→ Challengers outside the Boundary receive Ergon Damage.

l) **Ergon Damage:** Disruptive matter that damages challengers outside the Boundary.


**2.2 Game Modes**


<img width="655" height="276" alt="Screenshot 2026-02-20 at 11 08 15 AM" src="https://github.com/user-attachments/assets/da001692-3041-434c-9a61-2d438a18c2d5" />

These game modes run at fixed intervals, guaranteeing that players always have a match ready to join. 

If too few players register, the lobby carries over to the next scheduled start, improving concurrency and session reliability.

**2.3 Gameplay Loop**
a) Choose a Mode.
b) Choose a Schedule.
c) Choose a Challenger.
d) Loadout Phase → Spin the Wheels for Combat Boosters.
e) Fighting Phase:
-Reveal Phase: Opponent challengers and deployment area is revealed.
-Spectate: Watch your Challenger fight to death (optional).
f) Results Phase:
-Assess your Illuvial performance.
  1) Position.
  2) Time survived.
  3) Slain enemies.
  4) Damage dealt.
-Collect the Rewards.
  1) Top 10 Survivors earn monetary rewards.
  2) Top 3 Executioners earn Illuvial rewards.
  3) Potential Jackpot.

**Remarks:**
→ Once the loadout phase ends, everything is set. You can let the game run autonomously, sign off and see the results in any future instance.

→ MVP scope: Player agency ends at loadout phase. No player action can be done during the fighting phase.

→ Post MVP potential scope / game modes → Players get in-fight agency:
  1) Selecting when to cast omega with spacebar.
  2) High-Level movement commands.
  3) Targeting command.
  4) In-fight Combat boosters through an active economy system.

→ Opponent Disclosure: For the sake of fairplay, a player won’t see who else is registered for a session until the reveal phase (once the loadout phase has concluded).

**2.4 Matchmaking**

Combat Domes host a minimum of 10 players and a maximum of 100 players.

When a session has over 100 players, the match automatically has 2 phases.

Here’s how every game modality breaks down combat domes:


Skirmish: 10 - 100 players → **1 Combat Dome.**
Carnage / Conquest: 10 - 1.000 players → **From 1 to 10 Combat Domes.**
Leviathan: 10 - 10.000 players → **From 1 to 100 Combat Domes.**
What happens when player number is not ideal? 
Different behaviours based on the number of players: 

**10 - 100 players** → 1 Phase
→ 1x Combat Dome. Fight until 1 remains.

**100 - 200 players** → 2 Phases
→ Phase 1: 2x Combat Domes evenly distributed. [ Ie. 124 challengers = 62 each. ]
  -Challengers fight in each dome until 25 survive in each.
→ Phase 2: 1x Combat Dome with 50 challengers. Fight until 1 remains.

**200 - 300 players** → 2 Phases
→ Phase 1: 3x Combat Domes evenly distributed.
  -Challengers fight in each dome until 25 survive in each.
→ Phase 2: 1x Combat Dome with 75 challengers. Fight until 1 remains.

**300 - 400 players** → 2 Phases
→ Phase 1: 4x Combat Domes evenly distributed.
  -Challengers fight in each dome until 25 survive in each.
→ Phase 2: 1x Combat Dome with 100 challengers. Fight until 1 remains.

**400 - 10.000 players** → 2 Phases
→ Phase 1: Divide Player # by 100 and round the result up. 
  -The result above indicates the Combat Dome # needed for phase 1.
  -Equally distribute Player # across all Combat Domes.
  -Divide 100 by Combat Dome # to obtain how many challengers make it to Phase 2 per Combat Dome.
→ Phase 2: 1x Combat Dome with 100 challengers. Fight until 1 remains.

**2.5 Lobby and Reveal Rules**
a) **Set & Forget** Style. Actions to be done by a Player to participate in a match:
  i) Selects Mode.
  ii) Select Timeslot.
  iii) Select Challenger.
  iv) Select Loadout.
    1) Deployment Bidding.
    2) Spin the Wheels.
    
b) Now everything is programmed for the player. This allows the players to forget about the rest, and come back to spectate the fight or just come back to check the results.

c) Until the Reveal Phase, only the number of players and countdown timer will be visible.

d) The Reveal Phase discloses:
  i) All Player Names.
  ii) Challengers.
    1) Type.
    2) Tier & Stage.
    3) Level & TPl.
    4) Stats.
  iii) Loadouts.

**2.6 Four-Reel Slot Machine - Combat Boosters**
In the loadout phase, players get to play with a Slot Machine to acquire Combat Boosters for their Challengers.

**Slot Machine Rules : **
  1) Has 4 reels.
  2) First Reel: Attack Bonuses.
  3) Second Reel: Defense Bonuses.
  4) Third Reel: Penalties.
  5) Fourth Reel: Combo Wheel.
  6) You can roll the Reels as much as you want.
  7) The first roll is free.
  8) Each subsequent roll costs 10% of the entry fee.

**First Reel Boosters:** Effects and Odds.

<img width="664" height="209" alt="Screenshot 2026-02-20 at 11 18 11 AM" src="https://github.com/user-attachments/assets/13c5b15f-c2b9-4c1f-8115-77b2fa01a0ca" />



**Second Reel Boosters:** Effects and Odds.

<img width="654" height="212" alt="Screenshot 2026-02-20 at 11 18 43 AM" src="https://github.com/user-attachments/assets/ee3b3ce7-bdc5-4267-a25c-0a8a192e498d" />




**Third Reel Penalties:** Effects and Odds.

<img width="661" height="206" alt="Screenshot 2026-02-20 at 11 19 50 AM" src="https://github.com/user-attachments/assets/7a273bd5-663b-4a53-9c9f-0c739c60c80e" />




**Fourth Reel Bonuses:** Effects and Odds.

<img width="651" height="207" alt="Screenshot 2026-02-20 at 11 20 19 AM" src="https://github.com/user-attachments/assets/6eb1bc1e-033d-40d8-9d57-17d3b294a82b" />




**2.7 Ownership Bonus Stats & Holo / Dark Holo Illuvials**
**Level and TPI bonus stats** from ownership **apply in certain Deathmatch games.** While we want some modes to reward collectors for using their top Illuvials, we also want modes where Level and TPI bonuses do not apply. This ensures a more level playing field, encouraging both collectors and newcomers to use lower-tier or less-developed Illuvials while still having a fair chance to win.
In games where Ownership bonus is activated, picking a Holo or Dark Holo Challenger comes with additional advantages, as you are exposing a higher rarity Illuvial to Permadeath. For that, Holo and Dark Holo finishes increase the Challenger Stats for better Combat Performance:

<img width="615" height="111" alt="Screenshot 2026-02-20 at 11 21 34 AM" src="https://github.com/user-attachments/assets/8c364bd1-f988-4a13-8317-d7585ff3df9e" />



**2.8 Top 3 Executioners**
In every Combat Dome, the system will monitor which were the 3 challengers that killed the most opponents. This means that every single Combat Dome, be it in round 1 or round 2, will have 3 Top Executioners. Top Executioners Perks:

  -Do not experience permadeath.
  -Assigned by podium, each Top Executioner obtains one of the 3 Highest TPI Challengers that would have experienced Permadeath in that Combat Dome.

**2.9 Killing Blow Mechanic**
When a challenger delivers the killing blow to an enemy, they will instantly heal 10% of their maximum HP as a reward. This encourages an aggressive playstyle, rather than focusing solely on survival or defensive strategies.


## Monetization & Rewards:



## Combat Technical Specification:




## Social & Marketing Approach:


