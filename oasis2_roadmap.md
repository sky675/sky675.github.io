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

This is the current (as of 10/26/26) planned roadmap for OASIS II. Anything here is subject to change at any point. The best way to support this project is by spreading the word, buying my previous games and spreading the word about those too! Every wishlist and every purchase helps me immensely.

Updates to this roadmap can be found in the git history [here](https://github.com/sky675/sky675.github.io/commits/main/oasis2_roadmap.md).

## 0.5 (Current, Planned Early Access Release) - April 2027
- Weather system/visuals (rain, etc)
	- How weather worked in Tokyo is that it would pick the weather state for each scene that could have it, and that would persist while the game was open. Now it'll work more like normal weather, as time progresses it'll get better/worse, and changing regions will randomize it (not planning to have like a forecast or anything like that, this is *mostly* visual)
	- Currently only planning for the basic weather states that were in Tokyo (clear, cloudy (what it always is as of rn), overcast, light rain, heavy rain), but in the future want to add other weather (primarily snow-related stuff).
- Stocks system
	- Simple stock trading sim, will be an additional, riskier, way of getting v-mon. Will also be manipulatable via the hacking system, corp area missions, and certain quests
- Exports system **(partially started, focusing on demo polish)**
	- Reimplementing exports from Tokyo, though a bit differently. Obtainable from hacking, semi-related to stocks (a stock may go up or down if you list an export about a corp for sale, etc). This time they'll be sold in in-game time instead of IRL time.
	- Exports are physical items in your inventory, which can then be given to Maki to either be sold at an auction or used for a one-try mission with special effects (corp area loot but without the corp's security, etc)
- Hacking expansion (new interface + set of programs)
- Office map type expansion (local office-type variants + new rooms)
- New weapons (aiming for at least 3 weapons per milestone, currently considering: type 89, p22x(?), saiga/sk-12)
- More advanced hitbox script (intended for the head, but may be added to other parts in the future) **(done)**
	- Splits up a hitbox into more specific locations based on where the bullet actually hits the hitbox, will be used for helmets, armored face masks, etc
- Bullet penetration system (maybe, this may get moved later)
- New gear (depends on what I can get my hands on, but aiming for at least a helmet, an unarmored vest, and a new backpack)
- Hair under helmets/hats
- New containers (ammo, weapons/atts/mags, general item containers)
- Voiceline system (planning to start with just some generic grunt noises)
	- If you want to volunteer to voice characters, please email me or message on discord! Primarily looking for male and female voices who can speak: English and Japanese (but I may want other languages in the future).
- HUD cyberware expansion
	- Overview AUX hud (shows the health of teammates)
	- SmartVision (will be part of a base cyberware and not a mod, probably will come with no mod slots or maybe only a health one, tbd)
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
	- This will primarily be only be used for high value armor (helmets with faceshields, high-tier armor), bots using them will also be affected, existing items will have no durability
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
- Visible holstered weapons (currently cut due to workload concerns, may implement in future with only certain weapons initially)
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
