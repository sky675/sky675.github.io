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

This is the current (as of 10/15/26) planned roadmap for OASIS II. Anything here is subject to change at any point. The best way to support this project is by spreading the word, buying my previous games and spreading the word about those too! Every wishlist and every purchase helps me immensely.

## Latest Updates
You should use the table of contents to the right if this has gotten particularly long, I only remove entries after a milestone has been completed.
(10/15)
Adjusting the supporter pack contents again, removing weapon viewer mode in favor of a "firing range/dev room" scene. Couldn't figure out a way to do the previous idea well, and I think this is probably a better idea anyway. Nameplates for it are done and working though!

The previous idea came from a scene that I made that generated a random weapon using a bot loadout. Unfortunately, I couldn't figure out a nice way to convert that into something that was customizable.

(10/13)
Cleared out some of the older updates since it's been a while. Trailer is done (generally at least, need to get some ppl to test watch it). Demo build is finished and uploaded. Tomorrow I plan to submit it for review (may or may not lol, plan to do a test playthrough of the demo first). Release of it is still planned for early December. It's in its own branch now, so I can begin working on the 0.5 features and content again. If I make significant progress over the next 2 weeks, I'll probably end up making a post, but right now I still plan not to, and plan to only make the previously mentioned Next Fest post instead.

As a reminder, here is what is changed for the demo from the playtest:
- Removed Kansai (just for demo pacing/content concerns, still in full release)
- Kasumi has a temporary shop in Chugoku that is unlocked at the same level Kansai would be unlocked
- Kasumi's Mining Pick mission has been moved to Chugoku, so it is finishable. (both it and its prerequisite will not reward region xp in the demo though)
	- The other Kansai quests still technically exist, so if you load a profile that had them they'll be visible, but they won't be completable (technically No Sniping should be completable)
- Added new quest for Hara to make up for some of the later game quests being inaccessible in the demo (this is not a temporary quest for the demo though)
- Protection mechanic added in the last playtest update has been buffed (reduced damage threshold, reduced max damage dealt to player at once)
	- Haven't tested it as of writing but I believe this should make it a bit easier - my goal balancing-wise is a 65-75% personal mission completion rate, it is currently 30-50% (though it is a bit skewed from testing missions).
- Some minor fixes for issues I found while recording footage for the trailer (fun fact 2 of the issues can be seen in the trailer, but I left them in because don't think it'd be that noticible, look out for them lol)

I do have a system planned for unlocking new (to the profile) regions for profiles that pass the level that would cause a new region to be unlocked while that region doesn't technically exist, so profiles that play long enough to unlock Kasumi in the demo will be able to access Kansai in the full game - though it will be via a quest Maki will have, not automatic.

(10/7)
Updating this to document a few ideas I had, most currently planned for 0.6 and/or the future, for which I added a "Potential Ideas" section for. Right now however, I'm currently working on a trailer, which will be released with the demo version (probably in early December). Next week, I will split off a new branch for the demo version, make the changes I've previously described (remove kansai, move kasumi into chugoku so the miner is accessible), and start setting up stuff for the demo app. 

Because of the playtest update posts this month and the playtest version currently being the same as the version of the main game, I probably won't do a dev-blog post for this month. Instead, I'll write a post about the games from Next Fest this month that I liked, since I enjoyed doing that in June.

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
- More advanced hitbox script (intended for the head, but may be added to other parts in the future) **(done)**
	- Splits up a hitbox into more specific locations based on where the bullet actually hits the hitbox, will be used for helmets, armored face masks, etc
- Bullet penetration system (maybe, this may get moved later)
- New gear (depends on what I can get my hands on, but aiming for at least a helmet, an unarmored vest, and a backpack)
- Hair under helmets/hats
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
- Durability on armor 
	- Certain clothing items may have a durability, and after its depleted it the affected hitboxes no longer have armor
	- This will primarily be only be used for high value armor (helmets with faceshields, high-tier armor), bots using them will also be affected, items like what are currently in-game will still have no durability
	- Can be repaired at shops
- Revive rework
	- Can be revived without item (but will be at 1 hp)
	- Certain items (first aid kit, kage kit) can use a charge to revive at higher hp (automatic, move it out of vests/pockets before reviving to not use it)
	- Revive kits will become multi-use, will revive with highest amount of hp
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
When the game is available, I'm planning to create a small "supporter" DLC (final name may be different).
This is currently what I'm planning to include in it (could change at any time):
- 4K screenshots/wallpapers of environments/characters
- High quality versions of any music I've made for it
- Some special in-game nameplates
- Firing range/dev room scene, where every item is available and custom missions can be created and played, but saving is disabled (multiplayer unsure atm)

## Expectation for full release - ??? 2028+
- Six total regions
- Main storyline with three endings
- By this point, everything relevant from Tokyo should be reimplemented (weapons, objectives, etc)
- Container weapons could potentially also be added (as in the weapons they were based on, not the container weapons themselves)
- ???

## Potential Ideas
These are broad ideas I have, these may or may not be implemented at any time during Early Access or after and are just here for posterity's sake
- Visible holstered weapons (I want to try to do this for 0.5, but unsure how feasible it is right now, may or may not happen, which is why its here instead of in there)
- Seasonal/Leaderboard profiles (special profile type that wipes weekly/monthly/quarterly/?, may or may not change the game in some way, scored based on stats in some way, may have an in-game/meta reward for high ranks like a special nameplate, discord role, or something)

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
