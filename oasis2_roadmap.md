---
layout: single
title: OASIS II Roadmap
toc: true
toc_label: Roadmap
full-width-toc: true
nopage: true
noindex: true
header:
  overlay_image: assets/images/oasis2_bannerv2.png
---

This is the current (as of 8/29/26) planned roadmap for OASIS II. Anything here is subject to change at any point. The best way to support this project is by spreading the word, buying my previous games and spreading the word about those too!

## Latest Updates
You should use the table of contents to the right if this has gotten particularly long, I only remove entries after a milestone has been completed.
(8/29)
- Added m1911 + ump (rpm-45), as well as .45 ammo types to go with them
- Added vz82 (9x18 smg)
- Added a 0.7 milestone, with the remaining weapons in it and grenades (if I cant think of a solution for ai throwing them without blowing up by then, I'm just not gonna worry about that at the end of the day its not a huge deal)

There are 2 remaining major things on the list blocking a public playtest: 1. new map area (will decide what to do for that over the next day), 2. some misc setup in regards to accepting feedback and such.

(8/24)
- Updated the future milestones with 0.6 features and some additional stuff in 0.5. Posting the dev-blog for this month with this.
- Adjusted expected completion dates for milestones, some wording, plus added a section about supporter DLC plans

(8/21)
- Adjusted some future milestones. Ran into issues recording hacking (again), but should be finally good enough, the blog post/video is otherwise ready/recorded, expect it sometime during the weekend (i'll try not to get *that* distracted by stalker 2 dlc and mw4 beta lol)

(8/18)
Finished Transmit and its alternate types! I've removed the explanation from yesterday since its slightly different from the actual implementation:
- Transmit: Items are placed in a container at the beginning of the level, need to find where to deliver it to inside the level
- DeadDrop: Items are placed throughout the level, need to find them and deliver it to something at the beginning of the level
- Scatter: Items are placed throughout the level, as well as the entity or entities that they need to be delivered to
Also added some more items that have been in the milestone for 0.4, but wasn't here publicly.
(later in the day)
- Implemented most of what I added earlier. In terms of features, the milestone is done! But there's still content that needs to be produced before I think about whether its ready for a public playtest or not. Regardless, going to work on this month's blog post/video for now, and get back to them after that.
- Also added a few new quests (there are currently 23 quests)

(8/17)
- I ran into a few issues trying to record footage this weekend. As such, video is delayed since I had to fix those issues (still aiming for this week though). I decided to work on the objective types planned for this milestone after that. I did the defuse entity type yesterday, so I'll try to include defuse gameplay in the video.
- Cluster is also now implemented, and as such all main objectives from Tokyo have been implemented! Cluster is slightly different than it was in Tokyo: The central server has been removed from the objective, its just the multiple mini-Upload objectives now.

(8/15)
- Wasn't planning to add an update today, but I implemented a quick new idea I had: there is now a delay before inserting a new mag! This delay is dependent on the mag and is also affected by the inventory the inv is in (vests will be faster than pockets), generally its around 0.2-0.4 seconds of delay, with 50+ round mags having 0.5+ seconds (the standard makarov mag is instant, so unchanged). Bots are also affected by this, though without the inventory part.

(8/14)
- Added a second pistol, decided to just call it the G17 this time instead of K71 (seems fine lol), as well as the G18 to go with it. They currently only have the standard and aftermarket mags, I've decided to skip the bigger extended mag for now - I'll add it in the future if I can get changing item size via equipped magazine working in a way I'm happy with.
- Finished one last thing I forgot for hacking: a stat for hacking. Most interfaces will require a certain stat level to equip (though there is a beginner one that doesn't).
Will likely do a new build sometime over the next day, planning for video/post on Monday atm

(8/11)
- Finishing up hacking took a lot longer than expected lol. Very happy with how it turned out! Still expect a blog post/video in a week or so (from today tho). The post is mostly written, but I want a few more new things before I do a new build to collect footage from. (probably grenades next)
- Added exports to 0.5 (may end up moving it to 0.4, but idk)
(later in the day)
- After investigating grenades, I've decided to shelve them for now. My primary reason for this is I'm not the biggest fan of only players being able to use them, but I cannot currently think of a way for bots to throw them (without them killing themselves with them 90% of the time due to how they can move). I think my time could be better spent on other aspects of the game first, and then coming back to grenades later once the game is closer to release and most of Tokyo's arsenal has been reimplemented. So instead, I've added the VZ82 to the weapon list for this milestone (so 9x18 has an SMG). As such, my focus is now: K71 (or whatever its name will be now), then implementing Defuse (I've already imported the EMP model, I just need to script it) and *maybe* the new objective type idea.
- Also, decided on which idea to use for this one, and added some details about the idea.

(8/7)
- Hacking mechanics mostly done, two primary things left: enemy hackers and dynamic tower generation, then next will be some starting content for it. Expect a blog post in a week or so going over the new mechanics, probably a new preview video too

(8/3)
- Implemented a free loadout container, actual implementation is slightly different than originally described, and has been changed accordingly: the only way to get a loadout from it is by dying, it does not reset over time

(8/2)
- First thing for 0.4, sped up the makarov reload animations by around 25%, haven't done any real missions with it yet, but it does feel moderately better just shooting and reloading
- Did a bunch of AI behaviour stuff last night, made a few new micro and macro types and distributed them where appropriate in the factions (each faction should be more distinct, even moreso than in tokyo)
- New factions - corporate security (including Kage security for the Kage map type), PMCs (new for 2, these are foreign pmcs, hired by whoever, gameplay wise they're a bit of a mix between gang and sectcom, they're generally more aggressive than sectcom, but not too aggressive)

## 0.2 - Done
- Steam multiplayer/lobby implementation **(done)**
- Warehouses map type **(done)**
- Pump-action shotgun **(done)**
- AR-based platform (M4A1 + semi-auto variant) **(done)**
- "Actual" equipment for characters **(done)**
- Retrieval objective type **(done)**
- Bounty objective type **(done)**
- Gadget weapon attachment type **(done)**
- Initial skill trees for stats system **(done)**
- Profile/save creation options (hardcore, sandbox, etc) **(done)**
- Second region (+ related traders) **(done)**

## 0.3 (Current) - Done
- Alert system **(done)**
- Setup for potential localization **(done)**
- Double barrel shotgun **(done)**
- AK platform (all the ak-based weapons in tokyo, plus a new one) **(done)**
- PM-9 smg (features sight and suppressor att slots that weren't in tokyo) **(done)**
- Destruction objective type **(done)**
- Upload/Defense objective type **(done)**
- Third region (+ related traders) **(done)**
- Upgradeable stash rows (via a trader) **(done)**
- Passive V-Mon gain (mining, also at a trader, will also be able to convert between the 2 currencies at a loss, will be upgradeable) **(done)**
- Multi-mode gadget attachment type (dbal reimplementation) **(done)**
- New ammo types (incendiary, match, ???) **(done)**
	- 5 ammo types currently exist for non-shotgun weapons: FMJ (default/normal), AP, JHP, Incendiary (new), Match (new)
	- 4 ammo types currently exist for shotgun weapons: Buckshot, Slug, Flechette (new), Dragon's Breath (new)

## 0.4 - October 2026
- Hacking system **(done)**
	- Is completely different than Tokyo's hacking mechanics, had a new idea for it. More focused on manipulating stuff in the levels themselves rather than the enemies. Mechnically inspired by Cyberpunk Red's netrunning (sorta). Further details about it can be read [in this post here](/oasis/oasis-2-august-26)
- Some form of "welfare" system (free loadout) **(done)**
	- I run out of gear and money fairly often currently when playtesting solo, so something like this is definitely necessary, a free knife is not enough for this game lol
	- Available after every death. Given by various traders, loadout varies depending on the trader (later traders will give better gear).
- New map type (tbd)
- Adjusted Makarov animations (need to make it faster, its fairly hard to use right now because the reload is so slow compared to other weapons) **(done, its about 25% faster now)**
- G17 pistol **(done)**
- M1911 pistol **(done)**
- RPM-45 smg (ump) **(done)**
- VZ smg (9x18) **(done)**
- Short mag-based delay when reloading **(done)**
- New AI behaviour/types: **(done)**
	- Camper (they'll just hold in cover, instead of pushing after a few seconds)
	- "Simple" (doesn't use cover to reload/heal)
	- Flank (when set, ai can (try) to flank the target when they're out of strafing range)
	- Follower (patrols around group leader)
	- Defense (when the ai hears something, it will instruct another member of the group to investigate it instead, it can also investigate it with them)
	- AI now have the option of shooting while chasing if they aren't sprinting (previously they couldn't)
- New factions (corporate security (generic), PMC) **(done)** 
- Defuse objective type **(done)**
- Cluster objective type (this'll be a little different than Tokyo's, I'm removing the central server from this so it's just multiple mini-upload objectives now) **(done)**
- Brand new objective type (split into 3 different objectives: Transmit, DeadDrop, and Scatter) **(done)**
	- The basic flow of this is you take an item (or items) and deliver it to an entity in the mission, but where the items are and where the entity (or entities) are vary depending on the type
- Finishing a certain trader's scene (adding gambling-type minigames to it because I thought it'd be fun)
- Some way to manually skip time (host only) **(done)**
- Burst fire for weapons that should have it (I skipped implementing it initially) **(done)**
- The ability for character parts to add extra ragdoll collision shapes (ex: backpack not phasing into the ground) **(done)**
- Potentionally a public playtest of some form (after the milestone is complete)

## 0.5 - Winter 2026/Spring 2027
- Weather system/visuals (rain, etc)
	- How weather worked in Tokyo is that it would pick the weather state for each scene that could have it, and that would persist while the game was open. Now it'll work more like normal weather, as time progresses it'll get better/worse, and changing regions will randomize it to an extent
	- Currently only planning for the basic weather states that were in Tokyo (clear, cloudy (what it always is as of rn), overcast, light rain, heavy rain), but in the future want to add other weather like snow.
- Stocks system 
	- Simple stock trading sim, will be an additional, riskier, way of getting v-mon. Will also be manipulatable via the hacking system, corp area missions, and certain quests
- Exports system
	- Reimplementing exports from Tokyo, but without the mission modifying part. Obtainable from hacking, semi-related to stocks (a stock may go up or down if you list an export about a corp for sale, etc). This time they'll be sold in in-game time instead of IRL time.
- Hacking expansion (new interface + set of programs)
- New map type/existing expansion (tbd)
- New weapons (aiming for at least 3 weapons per milestone, currently considering: type 89, p22x(?), saiga/sk-12)
- More advanced hitbox script (intended for the head, but may be added to other parts in the future): Splits up a hitbox into more specific locations based on where the bullet actually hits the hitbox, will be used for helmets, armored face masks, etc
- HUD cyberware expansion
	- Overview AUX hud (shows the health of teammates)
	- SmartVision (potentially, will be part of a base cyberware and not a mod)
	- Advanced weapon hud (shows mags/ammo left)
	- ???
- ???

## 0.6 - ??? 2027
- Raid/Strike team event type 
	- Rival/enemy-unrelated AI squads may randomly spawn in a mission, with a desired goal, who will then retreat after completing that goal (or after taking too many casualities)
	- These squads' objectives occasionally might conflict with yours, and may cause a mission fail if their objective is completed before yours
	- Potential objectives will range from killing a certain amount of the mission's factions ai (where ones they kill won't count as a kill for you), to taking retrieval/objective items (they'll have an inventory to be able to get them back), or completely unrelated objectives such as reaching and investigating various parts of the level.
- Hacking expansion (Peripheral floors)
	- This will introduce new elements to levels (cameras, perhaps turrets, more) that can be controlled via hacking
	- If an enemy hacker/daemon is active in the network, it will control these peripherals (cameras will direct hostiles to you, turrets will, well, shoot you, etc), you can either destroy the peripherals physically (after which nobody can use them) or reach that point in the network to take it over and prevent the enemy from using it (typically they'll be in the global tower)
	- The floor will allow you to control the elements yourself (being able to see through the camera, turning on/off the turret + switching its iff, etc)
- New map type/existing expansion (tbd)
- New weapons (currently considering: famas/fmr 5.56, spas/s12, evo/vz3)
- ???

## 0.7 - ??? 2027
- ???
- New map type/existing expansion (tbd)
- New weapons (currently considering: v45, t95 (5.45))
- Grenade reimplementation
- ???

## Supporter Edition
When the game is available, either through early access or with full release (if I decide to not do early access), I'm planning to create a small "supporter" DLC (final name may be different).
This is currently what I'm planning to include in it (could change at any time):
- 4K screenshots/wallpapers
- High quality versions of any music I've made for it
- Some special in-game nameplates
- A "weapon viewer" mode, which will consist of a scene where you can pick any weapon in the game, customize it how you'd like, then screenshot it, with or without a background
- Probably will do something similar with character models too

## Expectation for full release - ??? 2028+
- Six total regions
- Main storyline with three endings
- By this point, everything relevant from Tokyo should be reimplemented (weapons, objectives, etc)
- Container weapons could potentially also be added (as in the weapons they were based on, not the container weapons themselves)
- ???
