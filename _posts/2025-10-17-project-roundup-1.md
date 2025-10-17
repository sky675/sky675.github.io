---
title: "Project Roundup #1"
category: misc
tags: [devblog]
excerpt: I don't have a specific topic I wanna do this month, so here's the status of every one of my current projects
toc: true
---

## Dyskairos

[This is my current main project](https://store.steampowered.com/app/3463170) (if that wasnt already obvious). The demo is currently in Steam's Next Fest, so now would be a good time to check it out if you haven't already! As for the full game though, it's pretty much complete. The things it's still missing as of writing are:
- Music tracks for 1 floor
- 1 more weapon (a heavy weapon - not entirely sure what I wanna do for it yet, potentially will be something explosive) 
	- There are 5 more weapons currently in the game compared to what's in the demo (2 new light weapons, 2 new mediums, and 1 new heavy. My end goal is to have 5 of each slot. Weapons that exist in the demo may also get new mods.)

And in case you haven't played since the initial launch of the 0.6 demo, I've implemented a large amount of quality of life improvements and changes [since](/dyskairos/dys-demo-v3/#update---september-19th):
- There is now a "Current Objective" text in the inventory, so you'll always know what you should be trying to do
	- Do note though that in the full game, the "final" ending explicitly doesnt use this system, you'll have to find it on your own :) The townsfolk will help though
- Keycards will now only spawn at their first defined spawn point
	- This is replaced with a new per-save system in the full game, detailed below
- There are now notifications when you pick up a keycard, so you'll know if you didn't notice you went over the pickup
- The interact prompt will now tell you when you have full ammo for a slot and if you already have a certain unique upgrade (this is primarily for the static-spawn ones, as other uniques won't spawn if you already have them)
- Reduced PTRD Short/Sawn Barrel spread debuff (the sawn barrel's hip spread is no longer the entire screen)
- Updated to Godot 4.5 (primarily for the new shader cache stuff)
- Settings/Pause menu has a new visual theme
- Map entities that can be interacted with now have a periodic shing-type effect (even if they cant currently be interacted with)
- There is now an indicator in the pause menu when the game will save on exit (and when the game was last saved if not)
- Added a notification to introduce the Inventory button at the start of the game
- Servants now attack more smoothly (less time between attacks to better match the animation length)
- Storage Locker contents are now kept on death always, no matter the penalty setting 
	- Previously dying would entirely remove the contents when above none, making it kinda pointless in hindsight lol
- Gun Servants now only shoot when not moving (makes them more accurate)
- The mini-boss Gun Servants in Floor 1 no longer respawn after being killed once
- Various other changes and fixes to issues I didn't find initially

Here's a quick list of what to expect in the full game (mostly just features I've added, or changes I've made that I haven't backported to the demo):
- 5+ new floors (there may or may not be at least 1 secret one too)
- 3 endings (they can be done sequentially on the same save slot)
- 6 new weapons (which will even the weapon roster out at 5 per slot)
- 7 new unique upgrades (13 in total, up to 4 can be found at once, not including the 3 uniques with static spawn points)
- 5 new generic upgrades (15 in total)
- Various achievements (17 in total)
- Per-save seed-based key item spawning 
	- Keycards will spawn in different places per save, but in each save theyll always be at the same place for that save. You will also have an option for the original completely random spawns
	- As such, when you load a save from the demo in the full game, the save's seed will get generated and the keycard locations will change from the demo
- PTRD bullet can now penetrate
- Bosses (the single enemies with health bars specifically, such as the floor 2 heavy spider drone) can no longer be one-shot 
	- Damage is capped to 65% of their HP in one instance of damage 
	- I didn't want to nerf the PTRD's damage specifically, but I felt like it made the bosses a bit too easy, so I've done this and made a penetration system for it to compensate for this new damage cap
- Can now upgrade the rarity of a held weapon (as well as reroll its mods) in the shop
	- Upgrades it by giving it a random valid mod
	- Fairly expensive, but most weapons can be upgraded past Legendary to a new "Special" rarity only available from this (which is when it has 5 mods)
- Added small animation after falling down at the start of the game (primarily just for worldbuilding)
- Recoil curve mechanics for sustained fire with weapons
	- Feels a lot better when shooting automatic weapons now
	- Ported from OASIS 1 so guns will feel a bit more like that game's guns
	- Unfortunately cannot backport this to the demo
- Various other features and balance changes I dont remember (I'll have a full demo-to-release changelog on release, not doing too much investigating for this list, this is just what I remember)

I also have potential post launch ideas, including:
- Weekly/Daily Run (randomly generated save with an objective of reaching a certain point/interactable, with a leaderboard based on the time took to reach it)
- Nuzlocke-type save option (when dying, a random one (/all?) of the non-static unique abilities that get lost cannot be found anymore for the rest of the save (you won't know which))
*Please note that these are not guaranteed to be actually implemented.*

## OASIS 2

{% include figure popup=true image_path="/assets/images/posts/projects1/oasis_wip.png" caption="A big work in progress, not final. Hair color is also currently randomized." %}

With all the core major systems now at least partially implemented, I'm beginning to try and make the game's current assets look more presentable so I can start sharing screenshots and such. These characters' materials will likely be adjusted a bit more, but I think it's coming along pretty well! My current goals are to be able to record decent looking footage of a multiplayer mission by the end of the year and have a fully playable small vertical slice potentially available some time in the first half of 2026 (may or may not be public, I'd like to try and get a publisher of some kind on board because I don't think I'll be able to take this to its full potential alone).

Once Dyskairos is out I'll be able to start working on this more often. The two games will likely (somewhat) swap positions in my schedule (I'm currently primarily only working on OASIS on the weekends). 

Compared to OASIS 1 - where the post launch content was largely stuff I had to cut/sideline during initial development otherwise I'd be developing the game forever - I've been able to implement most of my ideas for Dyskairos, there isn't much that's been cut or sidelined for time. As such, there currently isn't too much planned to be added to the game after launch, allowing me to switch my focus towards this (which I feel like people may like more anyway?).

## Koi

I've started gradually working on an AI Season Mode (when I'm inspired to), where you can specify a series of matches and it puts different teams (there are currently 10 predefined teams) in a round robin format using the series of matches thats been defined (no pictures for now, maybe in the future). 

It also saves different stats of each team: each teams win/loss in general, against different teams, and in different modes. Also stores stats (namely kills/deaths) for each player against each team and in each mode). 

There are currently 6 gamemodes: TDM, Domination, Hardpoint/King of the Hill (will come up with my own name for this mode eventually), Elimination (tarkov arena teamfight/gunfight), Elimination Tournament (tarkov arena's now cut shootout mode), and (of course) Search and Destroy (will change this ones name as well lol). The recent BO7 beta has also pushed me to work on a configurable CTF gamemode as the next gamemode.

*I love Overload as a concept but the 3 games I got to play of it had awful teammates who were never near the flag, real open matchmaking there. As a side note, it also ended up convincing me to just uninstall CoD altogether. I love bo7's aesthetic (obviously, I love "cyberpunk/sci-fi but Japan"), but that beta was just not very fun lol, bought BF6 instead.*

I'm also planning the ability for Season Mode to have tournament mechanics, with the option to either: Use that alone instead of the typical season matches, or use it once the season's matches run out to determine the season's "winner". 

These tournaments will likely be single elimination, seeded by the current standings of the season (or randomly if used alone). There is also a high chance that the initial implementation will restrict the teams playing in it to 4, 8 or 16 teams, just for implementation simplicity (for seasons, it'll obviously be the highest ranking 4/8/16 teams).

I still enjoy watching these bots run around and shoot each other, and I'm still considering publishing videos (potentially 24/7 streams if I can?) of the game running in Season Mode (it can go from match to match entirely autonomously now with no user input). Please let me know if you'd be interested in watching that! (it's good second monitor content tbh)

## Iterations

This is the game a friend and I made for the GMTK 2025 Jam back in August. I was working on an update with some fixes but it is postponed for now due to lack of interest. May come back to it, may not idk.

## Conclusion

I hope you can see I've been a bit busy! Please subscribe to my Youtube channel if you havent already as I'll likely post OASIS 2 videos there once it is more ready in a few months if you're interested in that (they will likely be posted alongside blog posts too though).

[Dyskairos](https://store.steampowered.com/app/3463170) is still currently on track to release in early November, so please, again, check out the demo and wishlist if you haven't already! I'd also love to know what you think in the Discord (link in the footer). 

Next month will likely have two posts: A full changelog of everything changed/added in the full game compared to the demo, and an OASIS 2 devblog with pictures (probably - I've decided I would like to keep the bi-monthly focused blog posts for now)!