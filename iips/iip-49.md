---
iip: 49
title: QuestDex and Player-Driven Quest System
status: Pending
Sponsor: Filow 
Key Contributors: Aaron, Nijafe, Scoriox, Dr.Spoon, Splendor, Jimberino, nASTY, yeehah
discussions-to: https://discord.com/channels/760344898200666112/1233056314142363779
---
# Simple Summary:
Introduce a player-driven quest system in the Illuvium Overworld that enables players to create and offer quests to others. This system aims to enhance player interaction and engagement with the Overworld, providing opportunities for investors/collectors to participate without direct gameplay and allowing players access to every Overworld stage and region without paying travel fees. The implementation of this system will require the creation of a marketplace for quests (QuestDex).

# Abstract:
The proposed player-driven quest system aims to enhance player autonomy, promote community collaboration, and provide opportunities for both gameplay and investment. The proposal outlines the mechanics of the quest system, including methods for quest creation, quest objectives, quest rewards, quest requirements, quest costs, types of quests, the Quest Journal, the QuestDex UI and Illuvium Zero integration.

# Overview:
The proposed player-driven quest system introduces a new dimension to the Overworld gameplay, enabling players to both create quests and participate in quests sponsored by others. Here are the main components of the quest system:

**Quest creation methods**

Quest creators may submit quests through various platforms such as the Illuvium website, mobile app, the Quest Hub in Sanctum Mesa, or directly within Illuvium Zero. Upon submission, the necessary fuel for travel, quest fee, and any required number of shards matching the quest details will be automatically transferred from the quest creator's wallet to an Illuvium escrow wallet.

**Quest objectives**

Quests encompass three primary activities: capturing Illuvials, mining rocks, and harvesting plants. Quest creators can choose one or multiple activities for their quests.

**Quest rewards**

Rewards for completing quests will comprise a percentage of the loot gathered during the quest, which will be selected randomly. This reward percentage is determined by the quest creator.

**Quest requirements**

Quest creators have the option to set minimum requirements for players to accept their quests. These requirements can include criteria such as the minimum player level, the minimum average level of the player’s Illuvials, the minimum number of completed quests, the minimum percentage of quests successfully finished, or even gear with a minimum bonus percentage for specific activities.

**Quest costs**

Quests would include an additional fee on top of the standard travel cost, serving as a contribution towards maintaining the QuestDex, with proceeds directed to the DAO. This fee would vary depending on the platform through which the quest creator submits their quest. Submitting quests via the website or mobile app would incur the highest fee, while using the Quest Hub in Sanctum Mesa would entail the standard fee. Accessing the QuestDex in Illuvium Zero would result in the lowest fee, providing an additional value proposition to land plots, even those that are F2P. Regardless of the platform, this fee would always be at least one unit of fuel. Upon quest completion, the fee would be automatically sold at the current market price, with all proceeds going entirely to the DAO.

**Quest types**

There are two types of quests: free-for-all quests and player-hiring quests. Free-for-all quests are accessible to any player who meets the quest’s minimum requirements, whereas player-hiring quests involve the quest creator specifically selecting who they want to complete their quest. Both quest types feature a completion timer, which can be customized by the quest creator, ranging from 1 to 7 days. The timer begins when a player accepts a free-for-all quest or when the quest creator selects the player for hire in hiring quests.

**Quest Journal**

A player’s Quest Journal would be accessible in-game, allowing players to review their quests and track their quest completion history. Quest creators could access another player’s Quest Journal through the QuestDex when submitting player-hiring quests. The Quest Journal would contain sections for completed quests, failed quests, hired quests, and active quests. It would display the player’s all-time quest completion rate and the most recent quests completed within the past 7 to 30 days. Players would be limited in the number of hired quests they could undertake and could only have one active quest at a time.

**QuestDex**

The QuestDex would be accessible through various platforms such as the Illuvium website, mobile app, the Quest Hub in Sanctum Mesa, or directly within Illuvium Zero. For players wishing to initiate a quest, they would access the QuestDex via the Quest Hub in Sanctum Mesa. The QuestDex UI should be highly intuitive and easy to navigate, offering various filtering and sorting options. Quest creators should find it effortless to publish quests in the QuestDex by selecting the quest type, region, stage, objective, minimum player requirements, and reward structure. Additionally, they should have access to the Overworld leaderboards per region and the player’s Quest Journal when submitting player-hiring quests. Players wishing to initiate a quest should be able to quickly sort through available quests by type, stage, reward percentage, requirements, objectives, etc. Furthermore, when a player starts a quest, it should be automatically removed from the QuestDex, ensuring that only one player can accept a specific quest at a time.

**QuestDex Illuvium Zero building**

Integrating the QuestDex with Illuvium Zero would offer an additional value proposition to land plots, even those that are F2P, as it would incur the lowest fee when submitting quests. Implementing the QuestDex within the current marketplace building seems to be the most logical choice, possibly by creating a third building level for Dex features. However, the decision ultimately rests with the team, whether they prefer to integrate this feature into the existing marketplace building, incorporate it into the Nexus building, or opt for the creation of an entirely new building dedicated to the QuestDex.

# Rationale:

The implementation of the player-driven quest system serves several key purposes within the game. Firstly, it promotes player interaction and collaboration, fostering a sense of community within the Illuvium universe. Secondly, the quest system offers a pathway for investors, collectors, mobile-only players, or those with lower computer specifications to participate in the Overworld economy without engaging in direct gameplay, thereby increasing the game's accessibility and appeal to a wider audience. Lastly, it provides players with a means to access every Overworld stage region without incurring travel fees, offering a pathway for F2P players to progress to higher stage regions.

# Community Concerns:

There were a few points of concern raised during discussions regarding this proposal: loot distribution, potential issues with bad player behavior in free-for-all quests, the similarity to buying from the Illuvidex, and the presence of missions already available in the Overworld.

**Loot distribution**

To address loot distribution challenges, a 'Quest Counter' system could be implemented. This system, assigns each tier/stage a numerical value as shown in the following tables:
![Screenshot 2024-05-01 at 9 25 46 AM](https://github.com/Nijafe/IIPs/assets/152656998/b1a23752-194f-41f4-b12c-00ae0c86d867)

The loot distribution would commence with the highest tiers, randomly assigning illuvials/materials between the quest creator and the player while their QuestCounter stays below the division threshold or until all loot is distributed. This approach ensures fair distribution, even when dealing with odd numbers, with any surplus illuvials/materials always being allocated to the quest creator. This distribution method would apply whether the quest objective is capturing illuvials, mining rocks, or harvesting plants. Additionally, any loot collected that doesn't match the active quest would be allocated entirely to the quest creator.

**Here are some examples:**

If a player captures seven illuvials (five T1S1, one T2S2, and one T1S3), the total counter would be 20 (5 x 1 + 1 x 6 + 1 x 9). With a 50% split, each player would receive 10 counters. Therefore, in the end, one player would have four T1S1 and one T2S2, and the other would have one T1S1 and one T1S3.
If a player captures six illuvials (one T4S3, one T3S3, and four T3S1), resulting in a total counter of 75 (1 x 36 + 1 x 27 + 4 x 3). With a 50% split equals 37.5 points, one player would get the T4S3 equaling 36 points, and the other would get the T3S3 and three T3S1 which equals 35 points. Since both player’s counters are under the 37.5 division threshold, the remaining illuvial would go to the quest creator.
If a player catches six Illuvials (three T3S2, one T4S2, one T5S2, and one T5S3) with a total counter of 90 (3 x 6 + 1 x 12 + 1 x 15 + 1 x 45), and with a 50% split, the division threshold would be equal to the T5S3 Illuvial counter. Consequently, the loot division would result in one player receiving the T5S3 Illuvial, while the other player would receive the rest of the Illuvials. If the player's quest reward share percentage was lower than 50%, they wouldn’t be eligible to receive the T5S3 Illuvial.

These examples also illustrate how it is in the player’s best interest to perform as well as possible to become eligible to roll for the rarer illuvials captured, thus helping to discourage undesirable player behavior.

**Bad player behavior in free-for-all quests**

To mitigate potential misconduct in free-for-all quests, specific measures can be implemented. Requirements such as minimum player levels and quest completion percentages act as natural deterrents. Additionally, quests offering higher percentage rewards are usually accessible only to players with higher completion rates. In cases of three consecutive failed quests, a strike policy would be enacted, resulting in a temporary ban from the questing system. Repeated temporary bans could lead to a permanent ban from questing. Moreover, quest creators can create blacklists of players from whom they do not want their quests accepted.

**Similar experience to buying off the Illuvidex**

One could argue that with this player-driven quest system, it might feel somewhat similar to using the Illuvidex. However, the quest creators would never know precisely what they would receive, as there would still be an element of RNG involved in the player runs. Additionally, the potential to acquire something extremely rare would still exist. Not only that, simply buying from the Illuvidex wouldn’t provide the benefit to players that cannot afford to pay to travel to higher stage regions as this questing system does.

**Overworld already has missions**

The presence of missions in the Overworld doesn't negate the potential for a player-driven quest system. Unlike missions, players wouldn’t have to pay, as their travels would be sponsored by another player.

# Quest Example:

Quest creators should have the freedom to craft their quests as they see fit within certain parameters, including selecting the objective, minimum completion requirements, region, stage, player requirements, provided items, and rewards. Here are some examples:

**New Player Quest**

Objective: Capture 1 illuvial, mine 1 rock and harvest 1 plant.
Region: Brightland Steppes, stage 1.
Requirements: 100% success rate on the most recently completed quests. Players with no completed quests are also eligible.

**Quest Items**: 7x T1 Shard, 2x T2 Shard, 1x T3 Shard.

Rewards: 10% of all acquired loot will be awarded.

**Illuvial Capture Quest** 

Objective: Capture at least 5 illuvials.
Region: Abyssal Basin, stage 1.
Requirements: 100% success rate on the most recently completed quests. Minimum ranger level 10. Minimum of 25% bonus capture rate gear.

**Quest Items**: 7x T1 Shard, 2x T2 Shard, 1x T3 Shard.

Rewards: 25% of captured illuvials.

**Lynx Capture Quest** 

Objective: Capture as many lynxes as possible. Not capturing any lynx will result in quest failure.
Region: Crimson waste, stage 2.
Requirements: 100% success rate on the most recently completed quests. Minimum ranger level 20. Minimum of 50% bonus capture rate gear. Minimum of 50 quests successfully completed.

**Quest Items**: 5x T2 Shard, 4x T3 Shard, 1x T4 Shard.

Rewards: 50% of captured lynxes.

**Shard Mining Quest**

Objective: Gather at least 3 shards.
Region: Taiga Boreal, stage 2.
Requirements: Minimum of 25% double gathering chance and 50% bonus gathering rate gear. Minimum ranger level 15.  Minimum of 30 quests successfully completed.
Rewards: 30% of all the ores and shards collected.

**High Tier Materials Gathering Quest** 

Objective: Gather as many materials as possible, either from rocks or plants. Not gathering any material will result in quest failure.
Region: Abyssal Basin, stage 3.
Requirements: Minimum of 50% double gathering chance and 100% bonus gathering rate gear. Minimum of 100 quests successfully completed.
Rewards: 40% of all the materials collected.

# Conclusion:
In conclusion, the player-driven quest system presents a compelling opportunity to enrich the cooperative player experience in Illuvium, offering new avenues for collaboration and reward. By empowering players to create and participate in quests tailored to their preferences, the system enhances the depth and longevity of the Overworld gameplay while reinforcing the game's value proposition and providing an additional source of revenue for the DAO. Through the implementation of this innovative quest system, Illuvium aims to establish itself as a leading player-driven gaming ecosystem in the blockchain space.
