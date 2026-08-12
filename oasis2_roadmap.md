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

This is the current (as of 8/11/26) planned roadmap for OASIS II. Anything here is subject to change at any point. The best way to support this project is by spreading the word, buying my previous games and spreading the word about those too!

## Latest Updates
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

(7/30)
- Finished the Kansai traders (for now) and as such, 0.3 is finished!
- Removed misc details from 0.3 elements

(7/29) 
- Moved potential public playtest to 0.4 (I still have some playtest keys intended for private tests though, if you ask nicely I'll give you one if you want it! I just don't think its completely ready for absolutely anyone to play this yet.)
- Adjusted details about the 0.4 "welfare system" (later traders will give better free gear)
- Added Makarov animation adjustments to 0.4
- Added a basically blank 0.6 entry
- Changed new map type to include potential map expansion instead
- New banner :)

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

## 0.4 - End of Winter 2026
- Hacking system **(done)**
	- Will be completely different than Tokyo's hacking mechanics, have a new idea for it. It'll be more focused on manipulating stuff in the levels themselves rather than the enemies. Mechnically inspired by Cyberpunk Red's netrunning (sorta). Further details will be announced in a future dev blog
- Some form of "welfare" system (free loadout) **(done)**
	- I run out of gear and money fairly often currently when playtesting solo, so something like this is definitely necessary, a free knife is not enough for this game lol
	- Available after every death. Given by various traders, loadout varies depending on the trader (later traders will give better gear).
- New map type (tbd)
- Adjusted Makarov animations (need to make it faster, its fairly hard to use right now because the reload is so slow compared to other weapons) **(done, its about 25% faster now)**
- New weapons (tbd, probably the k71 (may use a new name for it lol), m1911 and ump, vz (9x18))
- New AI behaviour/types: **(done)**
	- Camper (they'll just hold in cover, instead of pushing after a few seconds)
	- "Simple" (doesn't use cover to reload/heal)
	- Flank (when set, ai can (try) to flank the target when they're out of strafing range)
	- Follower (patrols around group leader)
	- Defense (when the ai hears something, it will instruct another member of the group to investigate it instead, it can also investigate it with them)
	- AI now have the option of shooting while chasing if they aren't sprinting (previously they couldn't)
- New factions (corporate security (generic), PMC) **(done)** 
- Defuse objective type
- Cluster objective type
- Brand new objective type (for now, calling it "Transmit", but it may have multiple names)
	- The basic flow of this is you take an item (or items) and deliver it to an entity in the mission
	- You may need to either find the items in the level, or have the items available at the start of the mission and need to find the entity, or maybe both, depending on the configuration of the objective.
- ???
- Potentionally a public playtest of some form (unsure when)

## 0.5 - ??? 2027
- Weather system/visuals (rain, etc)
	- How weather worked in Tokyo is that it would pick the weather state for each scene that could have it, and that would persist while the game was open. Now it'll work more like normal weather, as time progresses it'll get better/worse, and changing regions will randomize it completely
	- Currently only planning for the basic weather states that were in Tokyo (clear, cloudy (what it always is as of rn), overcast, light rain, heavy rain), but in the future want to add other weather like snow.
- Stocks system 
	- Simple stock trading sim, will be an additional, riskier, way of getting v-mon. Will also be manipulatable via the hacking system, corp area missions, and quests
- Exports system
	- Reimplementing exports from Tokyo, but without the mission modifying part. Obtainable from hacking, semi-related to stocks. This time they'll be sold in in-game time instead of IRL time.
- New map type/existing expansion (tbd)
- New weapons (aiming for at least 3 weapons per milestone, currently considering: type-89, p22x(?), saiga/sk-12)
- ???

## 0.6 - ??? 2027
- ???
- New map type/existing expansion (tbd)
- New weapons (tbd)
- ???

## Expectation for full release - ??? 2028+
- Six total regions
- Main storyline with three endings
- By this point, everything relevant from Tokyo should be reimplemented (weapons, objectives, etc)
- ???
