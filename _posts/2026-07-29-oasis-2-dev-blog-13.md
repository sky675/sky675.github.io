---
title: "OASIS II Dev-Blog July '26 (#13)"
category: oasis
tags: [devblog, mechanics]
excerpt: last numbered devblog, will switch to month year fully after this one
header:
  overlay_image: assets/images/oasis2_bannerv2.png
---

Hi! First post since launching the Steam page last month! Currently the plan remains the same, monthly posts detailing what I've implemented in the last month. I plan to upload new preview videos as I finish the major version milestones detailed in the [roadmap](/oasis2_roadmap). I made one for 0.3 (since that's essentially complete), but I didn't think it had enough new interesting stuff in it that was easily showable, so I'm leaving it unlisted. You can watch it here if you want:

{% include video id="2kYmBQwuyW8" provider="youtube" %}

## Alert System
{% include figure popup=true image_path="/assets/images/posts/oasis2_blog13/alert_level.png" %}
The main major feature I implemented this month was the "reworked" alert level system, as described in the roadmap. 

As a recap: in OASIS: Tokyo, during the end-game/oasis hunt mode available after reaching max rep, there was a feature named the "Alert Level". The intended goal of the end-game missions were to find the exit in the level as fast as possible in order to progress, and as such the alert level would increase if you took too long or killed any of the enemies in the level. The alert level determined what enemies spawned, ranging from SectCom to the JSDF to Saitama Group's own rapid response teams, all trying to stop you from reaching Fukushima.

This version is a little similar to Tokyo's alert level, but very different in a few key ways. Similar to Tokyo, the Alert System's level is increased by not completing missions quick enough as well as killing enemies related to the alert system, which may be different depending on the region. In this system however, the enemies won't spawn until either the mission has been completed or a certain amount of time has passed.

The primary intention of this system is to add a "soft time limit". I'm against adding a hard cut-off time limit (such as Tarkov's MIA status), but I do think there is a benefit in the gameplay loop of restricting the amount of time you spend in a single mission, so this is my solution for that. The first region will initially not have an alert level in order to make the early game a bit simpler. Instead, it will gain one once you unlock the second region.

{% include figure popup=true image_path="/assets/images/posts/oasis2_blog13/blackfac.png" %}
I'd like you to meet the current stand-in for the alert level enemies, the "black faction"! *(no actual name right now, their faction name in-game is literally "???")*

In their proper implementation, they're a bit like the suit enemies from Tokyo. They are ruthless operators who often target SectCom and corporate offices and are not typically the target of normal missions. The character on the capsule art is also technically a member of this faction! 

*(fun fact: the clothing I put together for her ended up partially inspiring this faction and as such she became a member retroactively lol)*

## Lighting Updates
As you hopefully may have noticed if you've watched both of the videos so far, one of the things I did this month was work on shader lighting! I've switched the lighting function being used by the shaders to be the one based on MToon's light function.

*(specifically, I took the godot-vrm addon's port of MToon and extracted just the parts for the light function, since I wanted to keep the shading I already had, though the body shader might receive some further parts of it in the future)* 

This has moderately improved the game's lighting, though since levels are procedurally generated at runtime I have to use VoxelGI for this and VoxelGI is not perfect, especially with the types of models I use for the environment. There is some occasional light bleed that I haven't been able to triage yet on certain maps.

## New Stuff
{% include figure popup=true image_path="/assets/images/posts/oasis2_blog13/julyblogpostmix.png" caption="PM-9 + New Ammo \ Kasumi (Kansai trader) \ AK + OKP-7" %}

As usual, here's a major list of what else is new/changed this month:
- Added special bones for vest/backpack straps, to try and improve the look of them (it sorta worked? still needs work)
- Ported signs from Tokyo, recreated some of the custom ones I made myself previously using them as well, though with some new references in some places (see if you can figure them out when u see them!)
- Added a dynamic light post that turns its light on/off depending on the current in-game time (used in static shop scenes)
- Other misc changes to scenes
- Added a new weapon hud element, it shows a percentage fill of the current magazine, which does not update automatically - it will automatically update after around ~8 seconds of not firing, but you can also force it to update immediately by checking mag. This is now the most basic weapon hud element, tier-wise
- Implemented the mission status hud element
- Double barrel shotgun
- AK system weapons (also includes a new one, AKS-74U)
- PM-9 smg
- Game can now potentially be localized in the future
- Added "Entity" objective base type, a generic objective type that uses an in-world entity (or multiple) to determine when the mission has been completed/failed
- New (reimplemented) objective types: Destruction, Upload (using the above type, currently only uses the server racks found in these objectives in Tokyo, but I do want to expand this to other potential objects later)
- Stash row upgrades is now an actual feature (shops can be setup with an upgrade level that will upgrade the amount of stash rows when theyre bought, or they can be given as quest rewards)
- First corp area, Kage, as well as related items (2 unique items this time!), currently the black faction is being used as a stand-in here as well
- Subfactions can now have effects randomly applied to its bots (ex: to simulate them having cyberware, higher tier black faction members use this to get limb armor)
- Traders can now buy certain types of items at different prices compared to other traders (one will buy weapons at a higher price than another will, etc)
- Combo gadget type (DualG)
- New ammo types:
	- For shotguns: Flechette (high pen, reduced damage), Dragon's Breath (very low direct damage, deals a damage over time effect when hits target)
	- For the rest: Incendiary (reduced damage, slightly higher pen, deals a damage over time effect when pens sufficiently), Match (slightly reduced damage, faster travel speed, reduced spread + recoil)
- Added a way to convert between the two currencies at certain traders (not a 1:1 conversion, you lose money in the transaction)
- Began work on Kansai (3rd region) region + traders (one of them is seen in the picture above)
- Added a passive way to gain VMon (will be unlocked during a quest line for the Kansai trader in the picture above, its also upgradeable via her)
- Shop upgrade levels can now potentially be locked/hidden behind certain quests (this currently only used in relation to the mechanic above, but will probably be used some later as more content is added)

That's all I have for now! I update the [roadmap](/oasis2_roadmap.md) fairly frequently, so if you're interested in the pace of development, that would be the best place to see daily updates right now.