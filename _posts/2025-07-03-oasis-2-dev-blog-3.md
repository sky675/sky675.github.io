---
title: "OASIS 2 Dev-Blog #3"
category: oasis
tags: [devblog, mechanics]
excerpt: Things went a lot better this time
---

Hi! Welcome to a new (bi-monthly for now) dev blog post for OASIS 2. Most of this month was spent on creating the level/mission systems. I'm also going to go into more detail on what my plan is for how missions and the overall gameplay loop will work. As always, everything in this post should be considered a work in progress and can change at any time (this is still like pre-pre-alpha). This post also won't have any pictures as there isn't really much to show visually with this as of right now.

## Level and Mission Generation

Missions work pretty much the same as in OASIS 1, but this time I'm architecting it a bit differently. Previously, whether an opposing/invading faction would spawn in a mission would be based on a template for that objective of the mission (but aside from a slightly increased payout range they're identical to the regular version of the objective template). Because of this, there would need to be a version of that template for each faction. Now, the faction and any mid-mission events (such as the opposing factions or reinforcements) are generated with the mission independent of the objective so I can more easily make more unique preset missions for priority missions. 

Because each faction's objectives in OASIS 1 were their own unique objective templates it lead to issues of having to update multiple different templates when I wanted to change how the objective was balanced. There would typically be at least 3 or 4 templates per faction per objective. Instead, now I can reuse the objectives anywhere a mission is created, whether it was generated or is a preset mission as the faction to use is decided/generated at the mission level now (there won't be any "templates" this time, just an assortment of different elements from various sources that get combined together). When making preset missions, I can also now specify it to have a specific seed, which will lead to the same level layout each time.

Level generation is still fairly early and I don't have a real group of rooms to use yet (just some test ones using csg), but one major improvement over 1 already is that seeds are now actually consistent. In OASIS 1, seeds were actually pretty much useless as the part of it that decided which rooms to use did not use the seed that was specified (I didn't realize this until a few months ago lol). Now every part of the level generation process will use the same seed (including loot but I'll probably end up changing that later). This is what enables the ability to specify seeds at the mission level, instead of it being decided when generating the level.

## Gameplay Loop

Disclaimer: None of what is mentioned in this section has been actually implemented yet, so the playable game may end up being a little different than what's described here.

As I've mentioned previously, the loop will be fairly similar to OASIS 1's. Randomly generated missions will be available to you based on the current state of your progression and at a certain threshold of XP a special mission will become available that needs to be completed in order to progress. However, like I've also already mentioned previously, your base is a vehicle that can travel to different regions of the country, and so those missions will more be based on the current region you're in and your reputation within that region instead. Each region will have its own distribution of factions and level types to pick from (though some regions will likely share factions and levels).

There will be different contacts in each region which will provide an additional means of progression: Questlines. Like Iwakura's questline that I added in 1, these will largely not be random and additionally also have the ability to come with preset missions with specified seeds (so that the mission's layout is the same each time). Questlines will largely still be optional but some may provide meta buffs or upgrades (again like Iwakura's questline) and some may complete on their own just through the main progression. I also plan for questlines to factor into the endings though, so for alternate endings they won't be optional. These contacts may also have shops or other services available for use.

Traveling from region to region isn't free though. Time in game is now dynamic, and will progress after doing missions, traveling to new regions or contact's locations, or by simply waiting. Limited effects (such as long term buffs or chip effects in 1) will be based on this time (as opposed to a number of missions or real life time). There may also be quests that may expire after a certain amount of time (haven't designed any yet to be honest but it's a possibility lol). Available missions will also persist now, and will be swapped out at random intervals every few days (you may also be able to pay to immediately get new missions, haven't decided for sure yet). 

Contacts' shops will be a combination of the normal shops and the OASIS Hunt shops. They'll be upgradeable with money (and questlines) but will have a limited stock that gets replinished over time. You'll also need to spend time to travel to the shop, but there'll also be an "online" version of shops that can be unlocked with which you can buy things directly from your vehicle. Certain contacts/shops may also not be available at certain times of day.

Also returning (in a way) is the Alert System from the OASIS Hunt mode. Alert level will accumulate after completing a mission (based on speed + enemy kills, again like in 1), and will reduce over time. Like in 1, a higher alert level will cause higher tier enemies to spawn. It will now also increase the base difficulty of missions (difficulty will no longer be choosable, it'll mostly be based on this now, but I'll probably add a way to manipulate the alert level or some baseline difficulty to pick from). In your current region (the active story one), the system will exist but will be capped to a certain limit (depending on the region). When returning to a completed region, the alert level will be uncapped and loot will have an increased chance to spawn rare items (yet again like in 1). Time will also be a factor in difficulty as well: the later the date is the higher the base alert values will be.

In terms of co-op, the perceived current time for alert values will probably be the average of all players' individual times. Other factors in mission generation and difficulty will be based on the host. For regions that are not unlocked by a player but are for the host, they can interact with shops and services and participate in missions there, but will not be able to receive quests from any contacts in the region. Play modes will also be returning in some form. I haven't fully planned out the details yet but there will be a hardcore mode and saves with that mode will only be able to play with other hardcore saves.

## Other Additions

I've also added a few other more minor features this month. 

First is a loot list system, dynamically created via tags applied to items (also allows potential future mod support for items). I've implemented this in a way that will make it much easier to handle and balance the spawn rate of new items.

Next (and a new one for OASIS) is the ability to loot corpses (as well as the implementation of ragdolls in general). This is primarily for looting other players when they die (since they'll lose it otherwise), but could potentially be expanded to include being able to loot bosses/special bots (to get mission items from them or a boss's unique weapon). I still don't want *every* enemy to be lootable or drop usable weapons though.

I've also implemented a stash system (stored locally per player). I've accounted for the possiblity for it to be upgradeable in the future.

## Future

In early August, [Dyskairos](https://store.steampowered.com/app/3463170)'s demo will be getting an update, which will add the third floor of the tower, 2 new weapons, and a few other things. The next post will be a description of everything in the update along with its release. In terms of the full game's progress, its content is currently about 75% done (the demo will have about 15-25% of the game's total intended content) and is going along well (a week or so after October's Next Fest is the release date I'm aiming for right now). For OASIS, the next major feature I'm currently considering to start next is an effect system and the start of skills/cyberware. Please wishlist Dyskairos if you haven't already and thank you for your support as always.