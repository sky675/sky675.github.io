---
title: "OASIS: Tokyo v1.3 Changelog"
site-title: "OASIS: Tokyo v1.3 Changelog"
toc: true
toc_label: Changelog
full-width-toc: true
nopage: true
excerpt: comparatively less than 1.2, but still substantiantial in its own way
header:
  overlay_image: assets/images/apartments.png
  show_overlay_excerpt: false
gallery:
  - image_path: /assets/images/apartments_1.png
    url: /assets/images/apartments_1.png
  - image_path: /assets/images/apartments_2.png
    url: /assets/images/apartments_2.png
---

Hi! Here's the full changelog for 1.3. There's a bit less than before in terms of new things, but I did warn this update would be relatively small. That's not to say there isn't quite a bit in this update though! A new mode, a new area, a new objective type, and more can be found below!

# Gauntlet
{% include video id="tR55Euknp7s" provider="youtube" %}
New gamemode! Defend your generator against increasingly difficult waves of enemies, while scavenging and buying supplies during break periods. Occasionally venture out and complete a randomly assigned objective in the level in order to prevent guaranteed damage to the generator. Entertain the stream's audience by winning rounds and getting kills in quick succession and they may send a support reward to help you out.

Also customizable!
- All main enemy types can be picked as enemies (Gang, SectCom, Corp Security)
- 4 different match difficulties
- 3 match lengths (matches can last from 5 to around 30 minutes)
- 3 areas to pick from (Office Complex, Warehouses, Slums)

I had this idea a couple months ago and thought it'd be fun, I hope you find it fun too!
This mode can be found in "Extra Modes" in the main menu. There are no current plans to implement this into the main game.

<br>

# New Items
![newitems](/assets/images/new_items_13.png)

In this update there are 9 new items, as well as 12 new junk items, both of which you can find out about below.

## Pistol Extended Magazines
Added new extended mags for each pistol:
- 21 round mag for the K71/K72
- 11 round mag for the M1911
- 10 round mag for the Makarov
- 20 round mag for the P92

The existing larger extended mag for the K71 has been moved into a new upgrade level in the shop. These can also be found as loot.

## New Attachments
![okp7](/assets/images/okp_sight.png)
- Added a railed dust cover for AK platform rifles (the weapon needs to be unequipped in order to attach this)
- Added a lower height variant of the Bisai2 sight
- Added new AK mount sight OKP-7
- Added a new laser with buffs related to aiming when enabled

All of these can be found in the shop or as loot.

## New Stamina Item
Added a new water bottle: 4 uses, restores 75 stamina on use, and will completely restore max stamina outside of missions. Found in a new upgrade level in the shop or as loot.

## New Junk Items
A new assortment of items have been added to be found as junk, which can be sold or requested for. Some of these items might have a new use in the future :)

<br>

# Other Additions
I've also got in this update: a new objective type, a new area, and some new features and mechanics.

## New Objective Type
In this update is a new objective type, similar to Upload: Cluster. In this objective you'll defend mini servers that you activate one at a time. You'll need to stick near each mini server as they run in order for them to finish, as they only progress when you are nearby. Complete the objective by finishing all the mini servers and then returning to the central server. This new objective can be found starting at reputation level 2.

## New Area
{% include gallery %}
There's also a new area in this update, Apartments, found starting at reputation level 2. This new area is the location of the base of operations for a gang on the outskirts of the city, though any of the typical factions and objectives can be found on missions here.

## Pawn Shop
The pawn shop now sells things too! You'll find a new terminal on the counter, but you'll need to buy its first upgrade level before it sells anything. 
In this new shop you'll find a random assortment of all items that can be found as loot (for a higher price than normal), including corporate unique items. You can upgrade the shop further to get a higher chance of rarer items and a small discount. The shop's inventory will change each time you are in Arinobu. 
This has also been added as a separate unlock in debt mode, available after buying the pawn shop itself.

## AI Improvements
- Enemies will no longer continue to attack targets they should be ignoring if they were already targeting it before it was set to ignore (such as upload servers that just finished)
- Enemies will now hear you reloading and using items nearby if they arent in combat or already investigating something else
- Enemies with the capability of running away will now try to get out of range of grenades (this is security and targets+bosses primarily) 
	- this isn't perfect and can cause them to run back towards the grenade to get to cover on the other side of it sometimes - will try to fix this eventually (maybe, its kinda funny tbh)

## Misc Additions
- Added compensators and some other items that were missing to the request item pool
- Replaced the previously generic elimination reputation level 5 priority mission with a new one using the new Cluster objective.
- Replaced default equipment button in Quick Mode loadout with a "Random Equipment" button
	- does exactly what it says it does, also added this for quick endgame and the new gauntlet mode
- Added new variants to buildings in slums

<br>

# Quality of Life
This time I've only got a general list of new quality of life stuff I've added, instead of subcategories.

- Switched to 64 bit (i realized pretty much everyone has 64 bit now so theres not really any reason to be building 32 bit lol)
	- if you happen to be on 32 bit only still somehow, i've made a new beta branch that'll be 1.2 which will still be 32 bit. (you should know if you are)
- Normalized the size of quick mode's death stats text
- Made quick mode's EMP death text match the main game's EMP death text
- Added loadout difficulty to quick endgame's death text
- Added a sound when turning in request items
- Updated shop terminals in Arinobu to include the interaction key in their interaction text
- Cleaner gamemode will no longer show never used current stats on the briefing screen
- Added a little weapon sway when looking around (can be disabled in settings if you want to revert it to how it was previously, made it pretty minimal tho)
- Added a dovetail-ish mount to the AKs where the mount point is (they mostly fit lol) - this is purely visual
- Added a setting to change aiming to toggle instead of hold
- Only spawn points closer to the player is used now when spawning reinforcement waves (should reduce the chance of upload waves spawning across the entire level)
- Updated the ADS position for the R200 with sights equipped (changed it to be the same as irons, so its closer to the player)
- The Full Heal button in the cyberware UI now gets reset each time its opened (to allow healing multiple times in the same scene)

<br>

# Balance/Adjustments

## Item Balancing
- Added a 2.5% aim speed debuff to the AK mount (the new railed dust cover has a 2.5% aim movespeed debuff and a 1% movespeed debuff). AK mount sights (kobra and the new okp-7) remain unchanged.

## Shotgun Damage Range
Shotgun pellets will now have 30% reduced damage after travelling about 15m. In most cases this should still 1 shot headshot if a pellet hits, but against higher tier enemies with more health it may not. This change affects enemy shotguns as well.

## Health After Death Changes
- In Hardcore, you'll now have 75 health upon respawning instead of 15, but you'll lose 2.5% more of your current money on death
- Lifeline cards have had their health increased similarly, no price changes (most will have a full heal now)

## Misc Changes
- Reduced out of stamina slow multiplier from -50% to -20%
- Enemies that spawn after being triggered by a certain secret will now spawn with a specific difficulty set independent of the current selected difficulty
- Ogura's followers will now stick closer to her when patrolling (reduced their patrol distance so they wont go out as far)
- Akaji will now fire his shotgun multiple times in one burst, and his bursts are now generally a bit more frequent
- Fukuma is a lot more accurate now and fires a bit more frequently, also swapped his red dot out for a different sight
- Reduced the price of clothing in the loadout menu by around 25-35% (you can pick the ak and also start with a backpack on hard loadout difficulty now with this)

<br>

# Fixes
- Fixed baked character voices not using voice volume mixer
- Fixed baked character enemies that have completely despawned back into the pool and then respawned not dying properly causing them to stay active (this has possibly been a thing since launch, sorry it took me so long to find this if you happened to run into this lol)
- Baked characters helmet hitbox works now
- Resized the Telescopic Scope to be more in line with other sights
- Adjusted the size of the Makarov when dropped so it is no longer huge when compared to the other pistols
- Enemies should no longer get stuck on objective servers and actually path around them now
- The male gang high threat target now actually wears the level 3 vest like intended instead of the old vest
- Fixed left hand slight shaking with ak weapons (idk how long this has been like this i didnt notice it until now)
- Fixed Office Complex pillars having larger colliders than they should
- Cleaner mode infinite loading should now actually be completely fixed, i found the actual source of the issue this time lol

Please report any bugs or issues you find in the Discord so I can fix them.

<br>

# Future + Roadmap

ok first up, heres whats currently planned for 1.4:
- the previously mentioned new area in the last update's plan for 1.4 has evolved into something a bit more than that lol. 
	- itll be some new content to do once at max rep - will be optional tho, probably will have some unique/rare rewards and stuff
	- currently estimating about 2-3 hours worth of stuff to do at minimum with no deaths - actual content of the mode is still being planned so this could change, but this is what im going for
	- more extraction shooter-y than normal gameplay is - will have a sort of soft time limit per mission, also going to add a stamina usage reduction buff to the player while inside the mission as the area will probably be *at least* the size of fukushima
- was planning to do a pistol reanimation for this update, but the [first animation i made for this](https://youtu.be/g-Rp-fX-Lig) ended up being longer than every other reload animation in the game. so the 1.4 update *might* include a full reanimation of all the reloads in the game. 
	- im still kinda undecided on how i wanna go about this (or if i really wanna do this at all) atm
	- itll at least include a reanimation of just the particularly bad ones (pistols, skorpion, etc. these are like 2-3+ years old at this point and those are the ones im most unhappy with as i feel like i can do better now), and fixing up some of the other ones. 
- probably other things, havent completely decided yet 
	- shotgun and rifle container weapons for one to complete that set
	- maybe new achievements for some of the new stuff added since launch
	- ive got a few misc ideas still on the list i could possibly do (most of these updates are either ideas ive had post launch, or stuff i had to cut for some reason or another previously)

currently planning to release 1.4 sometime in winter this year (maybe around the anniversary of the game's release? we'll see)

<hr>
{% comment %}
the gauntlet was also originally going to have an english host announcer alongside the tts announcer, but couldnt make that happen for the time being so that might be added in later (but i also kinda like the vibe of the stream audio not being played for the contestant so might not lol)
{% endcomment %}

now, onto the status of my next project, still tentatively called The Tower: 
the demo/prototype/vertical slice/pre-alpha/whatever (im actually not sure atm lol) is likely going to be out sometime *after* the next fest thats coming up. its getting there but theres still a bit of a ways to go.

ill probably post a short preview in the coming weeks to youtube once its mostly there, like i did with gauntlet mode. if theres interest, ill post screenshots/videos of development and stuff in discord too. for now though, as a little preview i added a wip image of the tower itself to [its section on my projects page](/projects/#third-project-tower). one of the new items added this update is in a way also a little preview too.

thanks for reading. hope you enjoy this update and i hope you'll stay tuned for whats coming.