---
title: "OASIS: Tokyo v1.2 Changelog"
site-title: "OASIS: Tokyo v1.2 Changelog"
toc: true
toc_label: Changelog
full-width-toc: true
nopage: true
excerpt: probably the most i've done in a 2 month time frame in a long time
header:
  overlay_image: assets/images/skyscraper.png
  show_overlay_excerpt: false
gallery:
  - image_path: /assets/images/skyscraper_back_elevator1.png
    url: /assets/images/skyscraper_back_elevator1.png
  - image_path: /assets/images/skyscraper_back_elevator2.png
    url: /assets/images/skyscraper_back_elevator2.png
---

Hi! This is the full changelog for update v1.2. This WILL contain some spoilers, particularly for endgame and some "secret" rare items in the game, so fair warning about that. You can use the table of contents to the right here to move to specific parts of the changelog. Every major addition or change has its own section.

# New Items
First off, new items. There are a little over 30 new items in this update.

## New Grenades
{% include figure image_path="/assets/images/grenade_lot.png" alt="new grenades" %}
- T41 Grenade - seen middle left above
	- impact grenade
- T42 Grenade - seen middle right above
	- short fuze grenade
- Both can be found within the new Jigane Industrial Warehouses area 

- Stun Grenade - seen on left side
	- slows movement and rotation while under its effects, slow-reducing buffs such as the pain editor cyberware reduces the grenade's debuff
- Flash Grenade - seen on right side
	- acts like a typical flashbang, makes your screen white and temporarily blinds enemies
	- there's a setting to make the screen black instead of white if desired
- Both of these can be found in the shop or as normal loot

## Lifeline Cards Minor Rework
- There are 5 of them now, and they were moved their own category in the shop. Each of them are on their own upgrade levels
- Each of them have an increasing number of features, basically as you go up you'll lose less and less for dying while its active
- Most of them are multiple use now, but if you end up dying while it is active it will still get removed regardless of how many uses are left

## New Gear
- Added a new container - 4x3 Plastic Bin that will only hold junk items (6x4 inventory size)
	- Found in shop

### New Backpack 
- Duffle Bag (4x3)
	- Found in shop or as loot

### New Vests
![vests](/assets/images/new_vests.png){: width="480"}
- C2 Chest Rig - 2x3 vest - seen left
- AR Armored Rig - 3x2 level II (pistol caliber only) armored vest - seen right
- Level III (rifle caliber) armor
- All of these items can be found in the shop or as loot

## New Clothing
- Added some black/grey variants of some tops that can be bought in the clothing shop. One can be seen in the picture of the new vest above
- Also moved clothing into their own categories based on gender, the main category now only has backpacks and vests

## New Meds
- 'Lucky' 
	- Applies a random effect on use (in most cases for only 90 seconds, these effects will also save, unlike normal med effects)
	- Found only as loot

- CoagL
	- Heals 10 bleed stacks and reduces bleed chance for 90 seconds while increasing stamina usage
- RegenR
	- Provides a healing over time buff for 90 seconds, also with increased stamina usage
	- Both this and CoagL can be found in shop or as loot

- Kage RegenE
	- Heals 8 bleed stacks and reduces bleed chance (more than CoagL) for 120 seconds while also increasing stamina usage
	- Can be found in the Kage corp area

## New Attachment Type
![comp](/assets/images/comp_combined.png){: .align-center width="480"}
Compensators
{: .text-center}

- Goes on barrel/supp slots
- Greatly decreases spread and recoil, especially while ADS
- Main downside is since this is on the same slot as suppressors, you cant get the reduced sound detection range from those with these equipped
- As with suppressors, these are per caliber - 9x19 compensator is for 9x19 guns, etc
- All can be found in shop or as loot

## New Cyberware Cores
- Alternate Basic Core with an adjusted slot distribution - moved 1 eye slot into neural
- New "Universal" Core
	- Has 5 core addon slots (still can only have 3 actual core addons)
	- Can use any core addon from any of the more specialized cores
	- Still restricted to a single extra slot core addon
	- Other slots are severely reduced:
		- 0 neural, 2 eyes, 0 body, 1 internal, 1 hands

## New Locked Briefcase
- Existing container key can be used to open this new one, as well as any future ones
- Contains a new SMG
- Spawns the same ways as the existing one does
- The existing one still spawns

## Misc Items Added
- There were tech core-related projectile cyberware I had forgotten to include in the shop, they're added now

<br>

# Other Additions
This is everything else added in this update: including a new area, new sections in existing areas, and new features

## New Area
{% include gallery %}
This new area, Skyscraper, begins appearing at reputation level 4. It has 3 exits, featuring some new exit mechanics:
- A main elevator at spawn
- An elevator in the back that needs to be temporarily activated to use (seen in one of the screenshots)
- A stairwell in the middle of the floor

## Night-Time Local Office Expansion
There's been a small expansion to the night-time Local Office variant
- Visible skybox through the ground has been fixed
- The surrounding area around the office has been opened up a bit, with new areas enemies can spawn from
- Also added a second exit, through an alley across the road on the front side of the building

## Slums
- Added interior soundscapes
- Added a new exit type: a tunnel with an openable shutter can spawn, with the exit behind the shutter. There is a button on the left side of the shutter to open it
- Removed glass material from windows that you could shoot through in slums

## Warehouses
- Forgot to actually add the new warehouses sections I had made previously, these are actually in now
- Added a new exit type: underground there is now a transition that can spawn to go even further underground, into the sewer. Inside the sewer there may be an alternate exit that can be taken after lowering the water.

## Arinobu
- Added some new background buildings to Arinobu's skyline

### Firing Range
![firing](/assets/images/firing_range.jpg)
- New feature in Arinobu's underground mall: a firing range
- Found in the new opened up shop across from military shop
- Weapons get unlimited ammo when entering the range while equipped
	- This can be toggled by the button outside of the range
- Targets can be cycled through some different enemy types and distances
	- Targets also have a headshot hitbox
	- Targets will pop back up after 3 seconds or after being switched to a different enemy type

These are not 1:1 to the enemies themselves, as these have only two hitboxes. In cases where the enemy has armor, it will use the enemy's chest armor level for the main hitbox. Targets do not have a helmet hitbox.
{: .notice--warning}

### Buying Exports
- Added the ability to buy exports to the auction house laptop in the hack shop
- This is an alternate way to get the locked briefcase key without hacking, as exports that have the mutator that spawns the key can appear here
- These exports do not persist and will be different each time you are in Arinobu

## Debt Mode Rework
Instead of simply setting the money to be negative, parts of the hub area now need to be bought in order to access them
- Old saves that had debt mode enabled will not have this, only new saves
- The tutorial will automatically be skipped with this enabled (since you dont have access to the mall immediately)
- Certain things need to be bought before other things can be bought. the apartment-side mall entrance is the first purchase, which will lead to more areas that can be unlocked

## Misc Additions
- Optimized lightmaps a bit, reducing the size of the game by a couple hundred megabytes
- Some minor improvements to the intro scene:
	- There is a railing in the stairwell now
	- Some new appropriate props have been added to the spawn room
- Added railings to local office variants that didn't have any
- Improved the stairs in office complex (you don't need to jump to get up them anymore)
- Some long hallways in office complex and some other areas now can have cover in them that can break up sightlines

<br>

# Quality of Life
I've also got more quality of life features. Some of these were requested, some I just thought they'd be nice things to have and would improve the game.

## New Settings
- Added a toggle to game settings that disables the damage effect visual (the thing that would make your screen flash red when taking damage)
- As previously mentioned above back in its section, the new flash grenade has a toggle in game settings to make the effect flash black instead of white

## Endgame Shops Ammo
Endgame/oasis hunt shops that have ammo in them (supply and survival) will now have guaranteed 2 mags and 1 ammo box for each weapon equipped, provided any applicable mags are accessible to the shop
- This is also on top of the shop's normal inventory, so it could potentially have more
- Rerolling will also restock the mags and ammo boxes as well
- Endgame shops are based on the upgrade levels for the shops in Arinobu so if you don't have mags unlocked for a weapon in the shop there, they won't spawn here
	- In quick endgame, upgrade levels are randomized so it will still be somewhat random for some guns whether or not mags appear

## Quick Mode Endgame Shop
An endgame shop and pawn ui has been added to the mission briefing menu in quick mode. The shop is based on the supply shop type, so this will get the same guaranteed ammo spawns as in endgame

## Other Quality of Life Additions
- Bleed Chance Multipler has been changed to "Bleed Chance Reduction Multiplier", and now shows the shows the raw value that modifies the bleed chance value instead
- Added a short delay to tooltips of items/skills/cyberware
- New pop up inventories (via open inventory or double click) will now be created slightly offset to the last opened inventory if one already exists
- Pop up inventories now adjust their size to the size of their inventory
- Pawn ui now requires an additional click to confirm selling
- Bandages, military gauze, and multi-use drink items can now be combined together to transfer their uses to the other
	- Larger items, such as medkits, cannot be combined still
- Shop ui will now properly update when buying a skill - or resetting while having a skill - that has a shop price modifier
- Updated the dropped visual for boss weapons when they die to more match the weapons they were using when they were alive
- Darkened the borders around items in the inventory to try and make them more visible in contrast to empty slots
- "Food Amount" has been changed to "Stamina Amount" in drink descriptions
	- Also specified the amount restored outside of missions is max stamina
- Renamed the IMA R200 Device Mount to IMA Tube Device Mount, and added a slot on the S12 for it
- The free knife will now always spawn on the kitchen counter in the apartment, so that you never *have* to do a mission starting with no weapon
- Added the name of the weapon in a locked briefcase to both the item name and the mutator that spawns it

<br>

# Balance/Adjustments

## Deferred Rendering
Switched to deferred rendering and increased the range of (or in some cases simply disabled) triggers that disable lights when not nearby because of this
- Performance *might* be worse in some situations, but should be largely the same
	- Performance is noticibly worse in some cases on warehouses, especially on higher difficulties. I'm still looking into this but for now have mitigated it as best as I can
- Lights disappearing in view should happen less often now except for in certain cases in some levels
	- URP's 8 light limit per object is still a thing in deferred and I combine the meshes in the level to improve performance, so if its still somewhat obvious in some places there's probably a reason for it - I did what I could

## Delayed Exits
You now need to be in an exit's trigger for typically 2.5 seconds to leave. This facilitates things such as the elevators in the new skyscraper area, the new exit types added to warehouses and slums, and future planned exits.

Exiting will now also automatically start if you're in the exit trigger when it activates. There is a 6 second delay when the scene loads before the exits are acitvated. Previously, because of the instant leaving, you had to reenter the exit trigger to actually leave if you entered it while it wasn't active

## Item Balancing
### Grenades
- Improved grenade damage a little, if a target is very near the grenade they will take damage from it regardless of line of sight
- M67 explosion radius increased, but the damage falloff curve was adjusted (should effectively be about the same, just can get slight damage from further away now)
- M67 fuze time increased to 4 seconds

### Other Items
- Significantly reduced the healing amount strong painkillers gives (~200 hp in total to 60)
	- This was moved into the new RegenR med seen above
	- Also reduced its price by 1000
- Made the level IIIA vest a bit cheaper
- Reduced suppressor sound detection range by around 33% for every weapon in the game (this is a buff)
- Locked briefcase weapons have an even lower detection range
- Can no longer add new items to opened locked briefcase invs
- Renamed Skotina-12 to SK-12
- Made the Basic Core a bit more cheaper

### Loot
- Made unique items in corp areas slightly more common, more-so on difficulties lower than expert (they were previously extremely rare below expert, now theyre less rare)
- Weapon crates now generally have more items in them at higher difficulties, additionally higher rarity items in them should now be *slightly* less rare in expert+

## Enemy Balancing
![ogura](/assets/images/ogura_new_armor.png){: .align-center width="60%"}
- Somewhat reduced the range at which enemies can be heard, they'll start getting quieter at a closer distance now
- Junko (the keys boss in stage 2 of endgame) now wears the new level II armored vest instead of the original IIIA armor. She'll now also rotate slightly faster and have slightly more health
- Ogura (the tier 4 target boss) and her direct followers that spawn around her will now wear the new level III armor instead of the original IIIA armor
	- Also should make her and her followers stand out more when nearby generic gang enemies happen to spawn with the same top
- High threat gang targets will now wear the level III armor instead of the original IIIA armor (they'll still wear a helmet as well)


## Misc Changes
- Switched all cyberware hacking projectile throwers (the ones the tech/savant core can buy) to use railgun attacks instead of homing projectiles
- Added defuse objs to quick mode 
- Reduced the size of the exit trigger in the tutorial shoothouse, so triggering it before shooting the last target should be harder to accidentally do
	- Also increased the speed of the exit door opening so times should be about the same if not faster (time stops when on the other side of the exit door)
- The first row of village missions in stage 3 of endgame/oasis hunt now have a chance of being replaced with a slums shop with a reduced safe period
- Reduced the objective scale for warehouses by a little bit - this will cause less enemies to spawn here, reducing lag generally, but also reduce rewards as well
	- It'll still be more than typical rewards generated at offices
- Reduced the enemy amount multiplier for expert+ by a little bit, also increased their spread and burst time stats a little bit to try and compensate tho
	- This is primarily for performance reasons

<br>

# Fixes
- Can no longer drag items with RMB or MMB
- Fixed ai spawning in shelves in offices
- Fixed an edge case that caused the main menu to become unresponsive
- Fixed being able to open pop up inventory while the item is equipped via double click function
- Adjusted aoe damage line of sight checking to check towards a more appropriate position on players and npcs, allowing for more consistent damage
- Fixed the ability to throw 2 grenades with 1 throw in certain circumstances
- Added more safeguards to try and prevent the infinite generation loop issue that can happen with the cleaner mode (this will also maybe help with similar less severe issues in endgame too)
- Fixed an issue where the skip initial message setting would get overriden by the invert y setting
- Doors should no longer close on npcs that are nearby right before theyre going to walk through them, causing them to phase through the door and not open it back up
- Shop price modifiers would previously not have been removed at all when the skill its from was removed, fixed this
- Fixed various locations in the game where the interact key placeholder wasn't being used, causing it to incorrectly show the interact key was f when it was rebound to a different key
- Submusclar Hardeners were previously incorrectly increasing bleed chance instead of decreasing
- Fixed multiple out of bounds opportunities
- Fixed the action ui being kinda wonky if its tween was rapidly restarted
- Baked AI characters were way too loud, they're now identical to normal non-baked AI
- Added some safeguards to inventory saving in case an item is bugged out somehow and can't be saved, so that the inventory doesn't entirely break
- Reimported some assets that broke and weren't appearing anymore
- Grenades will now no longer create a projectile when dying while cooking the grenade
- Fixed corp area destruction objs spawning the wrong enemy type as response waves, they should be the correct color uniforms now
- Fixed armor values being set wrong on sectcom female targets, and male targets having lower armor levels than intended
- Patched holes in the dropped model for the level IIIA armor
- Finally fixed multiple issues with stats from weapon parts not being correctly applied
- Tutorial text bubbles now work again (they might've been fine in the last main branch build? i'm not sure. regardless, if they werent, they work now)

<br>

# Known Issues
All of these will be fixed in either 1.3 or a patch if a big enough issue arises

- New clothing items arent in the extra mode appearance changer
- In some spots rain can fall through the ground in arinobu
- In some situations, the transition to the new exit in warehouses will slightly clip through the floor above it
- Warehouses in general can be a bit laggy now in some situations, im still not 100% sure why specifically this happens but thisll be worked on in the future. It's not unplayable

<br>

# Future + Roadmap

so, first and foremost, currently i am planning to do two more updates. 
- the first one is planned to be relatively small in size, and will mostly just feature a new extra mode idea i had that i think would be a fun addition. it will likely release sometime in june. 
- the second will likely include a new area, maybe two, and i'm not entirely sure what else right now.

focus has begun to shift more towards a new project - its also a fps, though its a bit different than oasis - i am currently planning to release a demo of sorts for this new game, and then by that point 1.3 will be out and ill switch focus back a bit to work on 1.4. *(i am currently planning to release both the aformentioned demo and 1.3 at or around the same time)*

if you're interested in this new project, please join the discord linked in the main menu or sub to my youtube linked below. i'll likely post something about it on both when its more ready to be shown off. i talk more about this new game on the [projects page on this site here](/projects/#third-project-tower).

thank you for reading, or just skipping all the way to the end. i hope you have fun with this update.