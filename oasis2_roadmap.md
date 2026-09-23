---
layout: single
title: OASIS II Roadmap
toc: true
toc_label: Roadmap
full-width-toc: true
nopage: true
noindex: true
header:
  overlay_image: assets/images/oasis2_bannerv3.png
---

This is the current (as of 9/21/26) planned roadmap for OASIS II. Anything here is subject to change at any point. The best way to support this project is by spreading the word, buying my previous games and spreading the word about those too!

## Latest Updates
You should use the table of contents to the right if this has gotten particularly long, I only remove entries after a milestone has been completed.
(9/22)
Playtest tomorrow :)
- Various adjustments to the roadmap (changing some wording, had an idea on how to do an alternate export use mechanic)
- Added a (mostly) blank 0.8 to start with (the version numbers are not a percentage complete or anything like that btw, it will go to 0.10+ if necessary)

(9/21)
- Made my twitter account public, please follow! I plan to start posting on it occasionally (not as often as I update this page but more than monthly hopefully) [https://x.com/skaaie](https://x.com/skaaie). I also opened message requests on it, but email or Discord is still the best way to contact me, I probably won't check DMs on that much.
- Added new containers to 0.5 milestone (may add them during the playtest, we'll see lol)
- Clarify that the SmartVision cyberware will likely have some kind of downside (trading it for no weapon/aux hud, maybe no other hud in general, etc. still unsure what I want to actually do for that)

(9/20)
Not certain yet, but aiming for playtest on the **23rd** (waiting for early access change to get approved first)
- Added voiceline system to 0.5 part of roadmap (will likely start with just like a little grunt when spotting and on death, don't want to use the pack voicelines I used for Tokyo this time)
- Added hacking system mods to 0.7 (I *may* swap this with peripheral floors depending on how many peripheral ideas I have when its time to start on that)
- Moved the previous milestones to the bottom of the page

(9/16)
This isn't really an update to the roadmap itself, just a general update:
- Enabled early access on the store page
- Added new store assets (the screenshots look good enough still, so they'll stay for now)
- Clarified "small office" in the 0.5 part of the roadmap to mean "local office-type" environments, fundamentally this will just mean a larger entrance room with a lot of exits and a more condensed map, similar to the local office maps in Tokyo
- Also added penetration to the 0.5 part of the roadmap. The PTRD in dys was *sorta* a test for this, and while I was on the fence initially still, I kinda want to do it now and reworking the bullets to allow this should be relatively simple (it'll be a relatively simple system overall, I'm not gonna do like ricochets or anything like that), it may get moved until later though based on how much time I have.

Preparation is going well, primarily waiting for people to become available to run a multiplayer session, and if that goes well the playtest might be started this week! (fair warning it probably wont, it'll probably be next week, need time to edit the monthly missions video)

(9/15)
Added some new stuff to future milestones and officially moved onto 0.5! Specifically:
- Plan for the early access release to have some new gear (if you happen to have any you've made that you're willing to donate to me (with credit) I'd be very grateful, the place I got the current gear from doubled their prices with no warning or sale...)
- 0.6 will have a new item type, permadeath profiles, and the fourth region (featuring Reiko, that region's main trader)
- 0.7 will have a new objective type (as previously mentioned I have 2 more ideas that I plan to implement over time, not sure which one this one will be yet)

The playtest is still planned for this month, I'll also post a blog post alongside it. I've also done a bunch of lighting updates again, so expect new screenshots lol (I've learned more about lighting in this engine in general, to the point that I'll probably change the capsule art and store gifs as well)

## 0.5 (Current, Planned Early Access Release) - April 2027
- Weather system/visuals (rain, etc)
	- How weather worked in Tokyo is that it would pick the weather state for each scene that could have it, and that would persist while the game was open. Now it'll work more like normal weather, as time progresses it'll get better/worse, and changing regions will randomize it (to an extent, it won't go from like clear to heavy rain)
	- Currently only planning for the basic weather states that were in Tokyo (clear, cloudy (what it always is as of rn), overcast, light rain, heavy rain), but in the future want to add other weather (primarily snow).
- Stocks system
	- Simple stock trading sim, will be an additional, riskier, way of getting v-mon. Will also be manipulatable via the hacking system, corp area missions, and certain quests
- Exports system
	- Reimplementing exports from Tokyo, but without the mission modifying part. Obtainable from hacking, semi-related to stocks (a stock may go up or down if you list an export about a corp for sale, etc). This time they'll be sold in in-game time instead of IRL time.
	- Exports may be able to be redeemed to create a one-attempt mission in the current region with a specific type of modifier (corp area item loot without having to deal with corp security, etc) (not 100% sure on this yet, this'll probably change lol)
- Hacking expansion (new interface + set of programs)
- Office map type expansion (local office-type variants + new rooms)
- New weapons (aiming for at least 3 weapons per milestone, currently considering: type 89, p22x(?), saiga/sk-12)
- More advanced hitbox script (intended for the head, but may be added to other parts in the future): Splits up a hitbox into more specific locations based on where the bullet actually hits the hitbox, will be used for helmets, armored face masks, etc
- Bullet penetration system (maybe, this may get moved later)
- New gear (depends on what I can get my hands on, but aiming for at least a helmet, an unarmored vest, and a backpack)
- New containers (ammo, weapons/atts/mags, general item containers)
- Voiceline system (planning to start with just some generic grunt noises)
	- If you want to volunteer to voice characters, please email me or message on discord! Primarily looking for male and female voices for: English and Japanese.
- HUD cyberware expansion
	- Overview AUX hud (shows the health of teammates)
	- SmartVision (will be part of a base cyberware and not a mod, probably will come with no mod slots or maybe only a health one)
	- Advanced weapon hud (shows mags/ammo left in inv)
	- ???
- ???

## 0.6 - ??? 2027
- Raid/Strike team event type 
	- Rival/enemy-unrelated AI squads may randomly spawn in a mission, with a desired goal, who will then retreat after completing that goal (or after taking too many casualities)
	- These squads' objectives occasionally might conflict with yours, and may cause a mission fail if their objective is completed before yours
	- Potential objectives will range from killing a certain amount of the mission's factions ai (where ones they kill won't count as a kill for you), to taking retrieval/objective items (they'll have an inventory to be able to get them back), or completely unrelated objectives such as reaching and investigating various parts of the level.
- Hacking expansion (Peripheral floors)
	- This will introduce new elements to levels (cameras, perhaps turrets, more) that can be controlled via hacking
	- If an enemy hacker/daemon is active in the network, it will control these peripherals (cameras will direct hostiles to you payday-style, turrets will, well, shoot you, etc), you can either destroy the peripherals physically (after which nobody can use them) or reach that point in the network to take it over and prevent the enemy from using it (typically they'll be in the global tower)
	- The floor will allow you to control the elements yourself (being able to see through the camera, turning on/off the turret + switching its iff, etc)
- Existing map expansions (tbd, probably some new rooms for each)
- New weapons (currently considering: famas/fmr 5.56, spas/s12, evo/vz3)
- Cyberware clothing item (clothing items that provide a cyberware effect, such as glasses that give a hud element without needing eye cyberware)
- Fourth region (at least 1 new trader)
- Permadeath profile mode (play with a permadeath mechanic)
	- In MP the save will only be deleted if the whole team wipes
	- Will probably end up not *actually* deleting the save, instead just making it not playable and kicking you to the menu, so the stats can be seen later (as a memorial type of thing)
	- Also will have a hardcore variant
- ???

## 0.7 - ??? 2027
- ???
- Hacking expansion (mods)
	- Hardware/software mods that affect how the hacking interface and your programs work (buff stats permanently, buff programs, etc)
	- Daemons will be able to apply temporary debuffs
- New map type (tbd)
- New weapons (currently considering: v45, t95 (5.45 ver))
- Grenades
- New objective type (tbd)
- ???

## 0.8 - ???
- ???
- New map type or existing map expansions (tbd)
- New weapons (tbd)
- ???

## Supporter Edition
When the game is available, either through early access or with full release (if I decide to not do early access), I'm planning to create a small "supporter" DLC (final name may be different).
This is currently what I'm planning to include in it (could change at any time):
- 4K screenshots/wallpapers of environments/characters
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

## Previous Milestones

### 0.2 - Done (June 2026)
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

### 0.3 - Done (July 2026)
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

### 0.4 - Done (September 2026)
- Hacking system **(done)** [(details in this post here)](/oasis/oasis-2-august-26)
- Free loadout system **(done)**
- New map type (slums) **(done)**
- Adjusted Makarov animations **(done, its about 25% faster now)**
- G17 pistol **(done)**
- M1911 pistol **(done)**
- RPM-45 smg (ump) **(done)**
- VZ smg (9x18) **(done)**
- Short mag-based delay when reloading **(done)**
- New AI behaviour/types: **(done)**
- New factions (corporate security (generic), PMC) **(done)** 
- Defuse objective type **(done)**
- Cluster objective type (this'll be a little different than Tokyo's, I'm removing the central server from this so it's just multiple mini-upload objectives now) **(done)**
- Brand new objective type (split into 3 different objectives: Transmit, DeadDrop, and Scatter) **(done)**
- Some way to manually skip time (host only) **(done)**
- Burst fire for weapons that should have it (I skipped implementing it initially) **(done)**
- The ability for character parts to add extra ragdoll collision shapes (ex: backpack not phasing into the ground) **(done)**
