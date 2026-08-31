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

This is the current (as of 8/31/26) planned roadmap for OASIS II. Anything here is subject to change at any point. The best way to support this project is by spreading the word, buying my previous games and spreading the word about those too!

## Latest Updates
You should use the table of contents to the right if this has gotten particularly long, I only remove entries after a milestone has been completed.
(8/31)
- Reworked this roadmap a bit
- My current plan is: 
	- Playtest launch in 2-4 weeks from today
	- Playtest will be live for probably around 2 months (end of november, will provide an exact date on launch)
	- May update the playtest to include new content/features
	- After the playtest is disabled, I will replace it with a demo version with the intention of entering the feburary next fest with it (will probably remove the third region in the demo version but will otherwise mostly be the same as the playtest)
	- That demo will be removed a week or two after the next fest
	- Early access launch in April? (to give time to implement feedback, plus when 0.5 is fully finished)
- 0.4 is essentially done, so wiped previous updates
- Third map type is decided to be Slums, currently working on implementing it (will be a bit different than tokyo's version)

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

## 0.3 - Done
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

## 0.4 (Current) - September 2026
- Hacking system **(done)** [(details in this post here)](/oasis/oasis-2-august-26)
- Free loadout system **(done)**
- New map type (slums)
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
	- The basic flow of this is you take an item (or items) and deliver it to an entity in the mission, but where the items are and where the entity (or entities) are vary depending on the type
- Some way to manually skip time (host only) **(done)**
- Burst fire for weapons that should have it (I skipped implementing it initially) **(done)**
- The ability for character parts to add extra ragdoll collision shapes (ex: backpack not phasing into the ground) **(done)**

## 0.5 (Early Access Release) - April 2027
- Weather system/visuals (rain, etc)
	- How weather worked in Tokyo is that it would pick the weather state for each scene that could have it, and that would persist while the game was open. Now it'll work more like normal weather, as time progresses it'll get better/worse, and changing regions will randomize it to an extent
	- Currently only planning for the basic weather states that were in Tokyo (clear, cloudy (what it always is as of rn), overcast, light rain, heavy rain), but in the future want to add other weather like snow.
- Stocks system 
	- Simple stock trading sim, will be an additional, riskier, way of getting v-mon. Will also be manipulatable via the hacking system, corp area missions, and certain quests
- Exports system
	- Reimplementing exports from Tokyo, but without the mission modifying part. Obtainable from hacking, semi-related to stocks (a stock may go up or down if you list an export about a corp for sale, etc). This time they'll be sold in in-game time instead of IRL time.
- Hacking expansion (new interface + set of programs)
- Office map type expansion (small office variants + new rooms)
- New weapons (aiming for at least 3 weapons per milestone, currently considering: type 89, p22x(?), saiga/sk-12)
- More advanced hitbox script (intended for the head, but may be added to other parts in the future): Splits up a hitbox into more specific locations based on where the bullet actually hits the hitbox, will be used for helmets, armored face masks, etc
- HUD cyberware expansion
	- Overview AUX hud (shows the health of teammates)
	- SmartVision (will be part of a base cyberware and not a mod)
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
