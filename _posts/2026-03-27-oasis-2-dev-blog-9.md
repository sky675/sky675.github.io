---
title: "OASIS 2 Dev-Blog #9"
category: oasis
tags: [devblog, mechanics]
excerpt: the overview one
toc: true
---

Hi! As I mentioned in the previous post, this will largely be explaining OASIS 2 (as well as its differences and improvements from the original). This post is written mostly with the intended viewpoint of someone who has played through OASIS: Tokyo, so if you haven't, you may not fully understand some things (I get a bit technical as well so you may not fully understand it anyway lol). 

Around 95% of what's mentioned below has already been implemented in at least a basic form, but as always please consider everything below a work in progress and any of it could change at any time.

## Overview
{% include figure popup=true image_path="/assets/images/posts/oasis2_blog9/env.png" %}

OASIS 2 (working title) is a single-player/co-op "semi-tactical" FPS featuring elements inspired by extraction shooters and rogue-likes in a sci-fi cyberpunk setting. In it, you play as part of an outfit of mercenaries, taking various "under the table" jobs from corporations, criminal organizations, and anyone else who's willing to pay. 

You'll travel across a near-future alternate-history Japan in your Mobile Operating Base, meeting various traders with a variety of quests on top of procedurally generated missions, all of which will provide reputation in its related region. Improving your reputation in one region may provide a foothold into another one. You'll also be able to improve yourself, using a new cyberware system and a revamped skill system.

Story-wise, it's a prequel to OASIS: Tokyo. You may or may not be able to see where it fits in. There will be multiple possible endings.

## Changes/Improvements from OASIS: Tokyo

Next, I'm going to go into detail about what's different about this game compared to the original Tokyo. I've made major improvements in the maintainability of the project compared to Tokyo and believe I can produce more content for this game more easily than I could previously. There's even potential support for mods in the future.

### Missions/Gameplay Loop

On a broad level, the game is fairly different. Instead of a single reputation level, there are now multiple, one for each region of the game (6 currently planned). Regions will be unlocked sequentially, but not always by reaching the max level of the previous one. Mission difficulty can no longer be chosen, but at higher reputation levels the difficulty will still automatically increase. Each region will have some kind of unique feature or aspect, setting them apart from each other.

Shops are somewhat the same, but also very different. You'll have categories in each shop and be able to upgrade each category with money, but you won't always be so close to those shops. Shops now have a "trader" linked to them, and you'll need to actually travel to them to buy from them, as well as accept and turn in any quests they may have. Each region will have different traders available, so you may need to travel some distance in order to buy certain things. You'll eventually also be able to have items delivered to you though (how that's done is tbd). 

Also being introduced is a new currency. Currently called "Coins" (name will probably change, wanting suggestions so please let me know if you have any lol), this is a special, more rare currency that some traders may desire for certain goods or shop upgrades instead of typical Yen.

There is also now a Time System. Doing missions, traveling to other regions, and visiting traders will progress the day. Generated missions persist after completing one now and missions will expire/regenerate after a few days. Certain quests traders have may also be time sensitive. This is about all time is used for right now, but there are ideas which may be implemented in the future.

Higher reputation levels will also introduce a mechanic similar to the alert level mechanic found in the endgame of Tokyo, where you may find various parties invading the mission based on the current alert of the region. There will be ways to bring the alert level down, such as lying low or traveling to a different region (both of which spends time).

#### Mission Generation

In Tokyo, objective types had to have an objective type for each faction, which compounded as more factions and objective types were added. Objectives with hidden extra "hunter" factions were also technically their own objective type, independent of normal objectives. Now, objectives and factions are independent of each other, but the faction can still influence the rewards and description of the mission. 

Missions are generated based on the pool of objectives, factions, map scenes, and modifiers/events the current reputation level of the current region has. This allows missions to have more potential possiblities than before while also being able to create new additions to those pools without having to worry about other aspects of mission generation.

Missions can now also be more hand-crafted, such as inserting specific rooms into the generation or dynamically modifying the difficulty based on the region level's difficulty. These provide the ability to create unique missions for quests or special scenes (such as traders' shops, which as I mentioned earlier you'll need to actually visit to interact with them).

#### Level Generation
{% include figure popup=true image_path="/assets/images/posts/oasis2_blog9/level_gen.png" %}

In Tokyo, the "seed" in the pause menu in missions was actually largely useless. The seed for deciding the layout and the seed for deciding the actual parts of the level were actually 2 different things (and tbh I didn't realize that until last year). Since this is multiplayer, seeds actually need to be consistent, so they are! Missions can also be made with non-random seeds specifically set for them.

#### Loot

In Tokyo, loot lists consisted of various sub-lists of manually defined items and rarities. When I added a new item to loot, I'd have to find the loot lists it should be in and add them manually. This time, items have a list of tags they belong to, and lists are generated by finding items with certain tags, and changing their rarities/removing them entirely based on other tags those items may have. With this they are now entirely separate and down the line this could even be used to easily add modded items straight into loot lists without the original lists needing to be modified.

### Player
{% include figure popup=true image_path="/assets/images/posts/oasis2_blog9/lean.png" %}

The player controller has also been updated with some new features:
- Leaning is now a thing
- Still no ability to crouch, however Left Control has been made a "modifier" key, pressing it while doing certain actions will do an alternate action:
	- Holding it in general will slow you down, which will also reduce the range at which AI automatically detect you
	- Interacting with an item that can be equipped will instead have it be sent straight to your inventory, instead of trying to equip it first
	- Dead bodies of other players can be looted, interacting with a body while holding the modifier key with a special item in your inventory will instead allow you to revive them, provided they weren't killed via a headshot.
	- Other abilities with it will likely come in the future
- Stamina has been reworked: You no longer lose max stamina after completing a mission, instead you'll lose more stamina the more you repeatedly do an action (for example, the stamina usage for sprinting will increase the longer you sprint). Not doing an action will reduce the stamina usage for that action. Water and other drinks still exist and stamina can still be restored mid-mission. The items can also be drank outside of a mission which will add stamina above the maximum amount (up to 2x).
- The player now has actual hitboxes - previously the main collider was used for hit detection for the player, and "headshots" were randomized. AI can also aim towards specific hitboxes.
- Bleeding has also received a rework. Instead of multiple bleed effects applied at different times, there is now one bleed effect that has stacks applied to it when bleeds occur.

#### Inventory
{% include figure popup=true image_path="/assets/images/posts/oasis2_blog9/newinv.png" caption="Vest is placeholder, not planning on actually using that model" %}

Inventories now can have multiple smaller inventories in them. The base 3x2 pockets have been changed to 2 1x1 inventories stacked vertically, and 2 1x2 inventories beside them. Items now generate their own icons, allowing items such as weapons to have dynamic icons based on the attachments they have (dropped versions of weapons now also reflect the attachments they have). Items can now be rotated. 

The stash can now be upgraded with more rows (tbd how that'll actually be done, likely will be linked to a trader). Items that can contain inventories (namely backpacks and vests) can now be folded if no items are stored in them, reducing the space they take up but they cannot store items or be equipped until they are unfolded again. Picking up a foldable item that cannot fit in your inventory unfolded will automatically try add it folded.

#### Cyberware

Cyberware has also been reworked. Cores have been removed in favor of 8 slots each with their own cyberware that can fit in each of them. Different mods can also be fitted to cyberware in those slots to change or add additional effects. Humanity will also be more of a factor. My expectation is that you'll be able to equip cyberware to 4 or 5 of those slots as well as a handful of mods for those cyberware. 

HUD elements return as mods for cyberware in the Eyes slot. Cyberware in that slot will come with specific mod slots that accept certain types of HUD elements.

#### Skills

The Skill system has also been reworked. Instead of a single player level, you now have levels in multiple stats, which gain progress as you do things related to that stat. The stat's level will also affect actions related to that stat. When you gain a level in a stat, you'll earn a skill point. These can be spent in various skill trees, typically also linked to a stat. Most skills will require a certain level in a stat before you can take it. Master skills will also return, like before they are powerful skills at the end of skill trees that increase in skill point cost as you take related master skills in other trees. Stats currently have a level cap (meaning there is a finite amount of skill points, unlike in Tokyo), though that may change.

### Weapons

Weapons have also improved in various ways, primarily visually:
- There is now a near-wall animation played when up against geometry.
- There are now alternate types of ammo that can be loaded into weapons. As of writing there are: FMJ (normal ammo), AP (does more damage vs armor, less bleed chance), and JHP (high damage vs unarmored, high bleed chance, but does very little damage vs armor). More types are planned in the future. As of writing there are no shotguns implemented - there are multiple types planned for them too though.
- You can now check the status of your current magazine. By default it will provide a general description of how much ammo is in the mag, as well as the top bullet in the mag. With a weapon HUD cyberware mod, only information not shown by the mod's HUD element is shown (such as only the top bullet).
- Weapons now contain a "aim helper" that was in Dyskairos: weapon bullets are shot from the gun towards the center of the screen, though bullet drop is still a thing (should help with shooting at range in general though).

### AI

The enemy AI also have some new features as well. Enemies can now use multiple weapons as well as any usable item. They'll have their own limited amount of items they spawn with, and cannot use more once they run out. AI can now have randomized attachments on their weapons, including different ammo types. AI cannot be looted still, though they have the capability for it now - may use it for the ability to loot a boss's unique weapon or something like that, we'll see.

Enemies can now spawn in together in squads (technically they could before, but now it's built in to the system). These squads can also spawn with a leader enemy, which may change how the squad reacts to targets. AI now have a "personality and role" system, similar to the archetypes described in [my post on the AI of my side-project koi](/koi/koi-bots). The personality is the "micro" of the enemy, which determines how it handles combat. It may be hyper aggressive, it may sit and wait, it could even simply just run away. The role is the "macro" of the enemy, which determines how it moves outside of combat and how it communicates to other members of its squad. It can direct other members of the squad to a new target it sees or tell a nearby member to investigate a sound they hear instead of doing it themselves, among other things.

Tokyo's AI originates from an old Unity tutorial from many years ago which I believe was called something like "pluggable ai" or something like that (haven't tried to find it again tbh, it was for their tanks tutorial game, may not be on their site anymore). They were basically very modular state machines. You may guess this, but - like a lot of other things - when I wanted to add a unique AI type to the game, it was fairly cumbersome. I had to remake a lot of the same states, just with the slight changes I wanted it to have, which was pretty time consuming. 

This new system consists of 3 scripts, a main "handler", a micro resource, and a macro resource (both of which are extendable). These resources are very customizable with elements being able to be simply enabled/disabled, making it a lot easier to make new types of AI. It's a bit of Tokyo's AI system, the aformentioned koi's system, and [the system I designed for Dyskairos](/dyskairos/dys-composition-ai) all combined into one system that works pretty well and I'm happy with.

## Roadmap/Conclusion

I am once again changing the plan for announcements. Re-evaulating my pace, I've got a new plan, here's what you can expect:
- Early April - Short video showcasing gameplay of a single mission, may or may not be multiplayer, no Steam page
	- Will likely *not* post this to the Discord
	- Also may try development videos alongside blog posts if there's a decent response
- May/June/July - Larger video showcasing more of the game (the hub, shop scenes, other mechanics), will try to get a Steam page up by this point 
	- Will definitely post this to the Discord, intended to be a formal "announcement" video
	- May try to edit it into a shorter more trailer-like video and see if trailer channels can post it depending on response (eg ign gametrailers and such)
- After this point, I'll start actively trying to shop around for a publisher, especially if I post the trailer video (if you're involved with something like that and are interested in publishing the game please email me, lets talk!!).
- Not going to decide on a potential release date right now (though it definitely won't be this year, may not even be next)
	- May consider a playtest or something later in the year, again largely depending on the state of development and general response to the previous videos.

There's a few other things I also want to do between April and July (may or may not happen):
- One final update to OASIS: Tokyo, fixing the remaining minor issues that's been on my list and adjusting some of the lore articles to include some stuff planned for 2 as well as probably adding some new articles too. Specifically, planned for this update:
	- Fixing a bug I found with the AI's runaway state while porting it to 2's AI
	- In Elimination, once there are 3 enemies left, direct them towards the player and prevent more from spawning (this is what 2's version of this objective does)
	- Rework the secret puzzle to not require the radio in the intro scene (the solution won't change though, just don't want to force people to listen to my stupid 60 second meme song and static for 5-15 mins for it anymore lol)
- Publicly releasing koi and making its repo public.
- If a *single* person messages or emails me or posts in the Discord that they are interested in the weekly runs update that was planned for Dyskairos, I'll do it that weekend. Sales wise, it's completely dead (Tokyo is selling more than it still lmao), so I don't see much reason in updating it otherwise.

That's about it right now. Please let me know what you think! Hopefully you'll see a new video on my channel in the coming week or so, provided I don't run into any major issues with the remaining work needed for a real playtest.