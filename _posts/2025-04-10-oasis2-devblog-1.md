---
title: "OASIS 2 Dev-Blog #1"
category: oasis
tags: [devblog]
excerpt: I've got multiplayer working but also I talk about plans for the game
---

Hi! I just want to preface this by saying *literally everything* in this article is very early and very much still a work in progress. Anything I mention here is currently the plan but that plan could change in the future. 

Also, actual development only started about a month ago as of writing and Dyskairos is currently still my priority. However, I have finished what I consider the "basics" and I would like to at least try to be a bit more open about development (even if it's only on this personal site that I don't post updates about publicly lol). So this article is mostly going to be about my plans for the game.

## Multiplayer

{% include figure popup=true image_path="/assets/images/posts/oasis2_blog1/15hourssofar.png" caption="The only picture in this article since this is all there is so far. Features 2 players, an ai, and several test items + weapons" %}

So, first thing I want to show is that I have multiplayer working! I could never really comprehend multiplayer in Unity (as I mentioned in the [History of OASIS](/oasis/the-history-of-oasis), I had tried to add MP to an earlier version of OASIS and ended up sorta bricking the project). For whatever reason though, Godot's multiplayer is a lot easier for me to understand. 

I'm currently planning for mainly co-op only, however bonus PvP modes aren't entirely off the table (more than likely won't have any kind of matchmaking or real "stakes" though). Of course, you'll still be able to play the game offline and singleplayer. I'll probably add bot support for those PvP modes as well.

## Setting and Design

So, when it comes to OASIS 2, my main philosophy is expanding the design ideas of OASIS 1. Pretty much "the same ideas but improved". In OASIS 2, you'll be based out of a mobile command center-type vehicle (think the Mobile Operations Center from GTA Online, also slightly inspired by the Elmo in Girl's Frontline 2) and will be travelling to different prefectures throughout the game.

Each region will be its own "reputation level", and some may have unique features (such as a special objective type found only in that region, or a special "corp areas" with unique loot, like OASIS 1). After "completing" the region, you'll be able to return to it for a harder difficulty and better loot (think expert+ in OASIS 1). Regions will also typically have a point of contact character based in that region, which will offer a shop and their own questlines. For co-op, saves will be stored on each player's end. You'll be able to play some solo then later join someone and keep that progress.

If you join someone who has access to a later region, you will be able to play missions in that region and buy from the region's shop but you will not be able to access the quests from that region (in other words, other people will not be able to influence your save's overall progression unless they are at the same point in the progression).

### Skill System Expansion

Another thing I'm planning is an expansion of the skill system. There will still be skill trees and skill points, but there won't be a "simple" XP-based level system anymore. 

Instead, there will be various stats which are progressed via various means. Increasing these stats will increase your level which will give skill points. However, most skills will have stat requirements, so you can only spend those points in the trees of stats you've leveled (some won't have requirements though). Master skills will still exist as well.

Most of the skill categories will return in some form, with also some new trees as well. I'm also considering being able to pick from stat/skill "presets" but also being able to start as a blank slate too.

### Cyberware System

OASIS 2 takes place around 10-20 years earlier than 1 does (it's actually a prequel). Because of this, the cyberware will be more rudimentary, but at the same time be more advanced in terms of mechanics. 

Instead of specific slots, there'll be a limit to the amount of cyberware that can be installed at once. You also won't be able to install 2 cyberware of the same type. However, cyberware will have mod slots that expand their capability. As an example, an eye cyberware will be able to accept mods that adds hud elements. So, instead of 3 bespoke eye cyberware each with their own hud element it would be one cyberware with 3 mods installed.

I'm also going to attempt to have every cyberware be freely uninstallable, so that there's no need for a reset cyberware function.

### Hacking System

Another system I'm looking at reworking is hacking. OASIS 1's hacking was admittedly *very* half-baked and at some point turned into mostly an afterthought, so I'd like to improve it in 2. This is a very very early idea still and will more than likely change, but my current idea is a bit inspired by how netrunning is done in Cyberpunk Red. 

Each mission location will have a procedural network generated for it. Various access points will be added around the generated map. Upon connecting to a network with your hacking device, you'll be able to progress "room by room" within the network, with each room having its own thing attached to it (whether its export data, location-specific security (such as turrets), passwords or various types of ice/defensive programs). You'll be able to collect, take over, and combat these various things via your own programs. 

While this is going on, enemy defender hackers (ill come up with or find a better name for this lol) may also be in the network and may be able to find where you are and send on-site security to your location. So you'll need to be quick, be able to jack out quickly, or have friends (real or otherwise) defending you.

### Miscellaneous

Here are a couple other random things currently planned:
- Leaning (I've pre-emptively setup the controller to allow it, I just need to implement it)
- Multigrid inventories (this is actually already implemented, currently the "pockets" are setup as the 4 1x1 squares typical for this style of game. I'm also considering 2 1x2s and 2 1x1s in a shape similar to OASIS 1's pockets though)
- Item rotation (this is also already implemented, but has some issues I need to fix still as of writing)
- Foldable empty bags/vests (Arena Breakout has issues imo, but this is one feature I actually like about that game)
- Multiple/special ammo types loaded individually into mags (not going to do specific rounds such as SOST or M855, I'll likely just do generic types such as "FMJ", "AP", or "HP")
	- The loading process will probably be the same as 1 (I still find it more engaging than dragging onto the mag and waiting)
- Planning on a small stamina rework: 
	- Removing max stamina removal due to low stamina at the end of a mission (instead, being at high stamina at the end of a mission may increase a related stat or something)
	- Drinking will be able to "overheal" stamina (with an upper limit)
	- However actions that expend stamina will increase the stamina drained the longer you've been doing that action
	- For example, the stamina lost when sprinting will be higher when you've been sprinting for 30 seconds compared to the initial loss rate. The rate increase will gradually reduce back down when you aren't doing that action.
- More "invading" groups in missions besides just the main faction of the mission arriving as reinforcements or a faction hunting the main faction (such as strike teams with their own separate objective in the location such as in the Saitama Facility)

## The Beginning

Like I mentioned before, this is all still extremely early. I've only spent 10-15 actual hours on this project so far, and again most of this article is essentially just plans. Finishing Dyskairos's content is still the main thing I'm working on right now. I'll probably do more blog posts like this for OASIS 2 (and potentially dev videos in the future?).

Finally, if you weren't aware, Dyskairos now has a demo on Steam. If you haven't yet, please try it out and let me know what you think in the Discord (linked in the footer)! 

I'm currently working on an update to the demo that will be released prior to one of the Next Fests. I'm not sure which one yet, it'll probably end up being based on the state of the game a few weeks out from the deadline, since I want to release it a month or 2 after the event. 

I'll make a post about it (both on this site and on the game's page) when I've decided it's time. At that point I will have decided on a release date as well, so please wishlist the game if you haven't already and stay tuned!