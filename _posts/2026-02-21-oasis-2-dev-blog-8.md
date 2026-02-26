---
title: "OASIS 2 Dev-Blog #8"
category: oasis
tags: [devblog, mechanics]
excerpt: a small change of plans
---

Hi! Obviously, no showcase video yet. I've made some minor changes in development direction recently and as such, it's been delayed a bit. I'm now aiming for late March, but I'm not extremely confident in it as of writing. However, I will be doing screenshots for this post, as the game *is also* now *technically actually really* playable! As always this should be considered a work in progress and any of it could change at any time.

## Delay

So, first, a quick explanation of what's changed. Originally I was going to create the video with no cyberware systems and no skill systems. However, I've realized that's kinda stupid, as cyberware is definitely a major aspect of 1, and will be in 2 as well. That's why its been delayed. I've already implemented the most basic framework of the cyberware system (which I will detail further below), and probably in the next week I'll work on skills (after Next Fest is over). 

In terms of other content, to prevent *another* delay (so I can start actually showing this to others) that's not being changed. Being implemented before the video is a single faction, 1 objective type (maybe 2), 3 or so guns, melee, and some different other items. This faction is the most basic faction in OASIS 1, the gangs. They've technically already been implemented (you'll see them below), but I plan on expanding their clothing collection.

I'm also considering between now and when its actually ready for a multiplayer recording posting some singleplayer gameplay. May or may not do this, unsure about it right now. While it is *technically* playable, it still isn't quite ready for an actual gameplay session.

## New Things

{% include figure popup=true image_path="/assets/images/posts/oasis2_blog8/general.png" %}

### Cyberware Implementation

I believe I've talked about this in a previous post, but cyberware in OASIS 2 will work differently than in 1. Instead of a "Core" determining the availability of cyberware, there will be various slots with a spot for only one cyberware in each slot. Cyberware will now however have subslots in which mods and additional effects can be equipped. 

For example, this is how the HUD cyberware will work: There'll be various cyberware pickable in the "Eye" slot, each will have certain subslots available in them, such as: Weapon HUD slot, Health HUD slot, or a Vision slot (this slot would contain items such as SmartVision and the Objective Tracker).

Humanity will also be more of a factor in limiting how much cyberware can be equipped. I'm expecting maybe 4 or 5 main slots (there are currently 8 planned, but that number may end up shrinking) and a handful of subslots can be used before reaching the limit. Low humanity may also have negative effects, but its too early to say now (right now there are no other effects, but I do have ideas, if I think they're too brutal for normal play, I may make them hardcore-only instead).

### Menu + New Hub Scene

{% include figure popup=true image_path="/assets/images/posts/oasis2_blog8/menu.png" %}

I've implemented what will probably be the main menu for the game (though it will be visually improved later, again work in progress) as well as the character creation UI. It now saves the last used save profile, so you can more quickly jump back in. I'll likely not add a "Extra Modes" type of thing to the menu this time. Anything extra like that I want to do will likely be implemented as a new region in the main game instead (on top of the 6 regions currently planned)

{% include figure popup=true image_path="/assets/images/posts/oasis2_blog8/hub.png" caption="Also seen here: You have a setting for 'Player Color'. This not only will change the color of your nameplate and pings in multiplayer but will also change various aspects of the game, such as the color of the stash and some miscellaneous HUD elements. This color is a global option, independent of the current profile." %}

Also new is the first version of the game's hub scene, the inside of the back of the truck you'll be traveling in. Here you'll be able to access your stash, change clothing with the wardrobe, accept missions, or talk to your driver/mechanic Maki, who has a little screen to talk to you to from the cab. She'll have a few starting quests for you. To re-iterate yet again, *very much a work in progress* - the interactable to accept missions from is literally just a cube right now.

### Beginning of the Game's Progression

{% include figure popup=true image_path="/assets/images/posts/oasis2_blog8/gang.png" caption="Fun fact: I died seconds after this screenshot because the AI are *very* accurate right now lol" %}

As I started earlier, I've started implementing parts of the game's progression. I've added the first *actual* faction, the generic Gang. They are very similar to their OASIS 1 counterpart and as such are very aggressive. 

I've also started on the first region, Fukuoka. This prefecture will be the starting region in the game, featuring a few traders and relatively simple objectives and enemy types (such as Gangs) to introduce you to the game. 

One of these traders is the "Smelmart Employee". Known only as that, he can provide supplies from his store's stock for you, under the table. For a fee, of course. By default, he doesn't sell any weapons, but may be willing to bring in a friend from Smelmart's Security division with some of their surplus weaponry after some investment from you.

### Skill System Implementation

The skill system is going to be very different compared to 1's. There won't be one single "player level" anymore. Instead, different stats will gain XP from doing certain related actions and will level up once reaching a certain threshold. 

When they level up, you'll get a skill point. You can then spend those skill points on skills in trees related to the various stats. Certain skills may have some additional requirements, such as a certain level in a stat before being able to pick up that skill. 

There will also be passive benefits related to levels in the various skills (for example, there'll be a "fitness" stat which will improve stamina usage and movespeed with each level).

As of writing, none of this has been implemented yet, but that is the current plan for skills. The names of things as well as final implementation may change.

## Future

As for Dyskairos, I cannot say for certain when weekly runs will come (if it will at all at this point). I may decide to take a small break to do it after creating the multiplayer showcase video. 

Otherwise, that's about it for now until next month. I'm planning to do a post in a week or two that'll be a all-around overview on OASIS 2 and new features being introduced (that article is going to be written with the assumption you have played OASIS: Tokyo), and then the next post after that will *hopefully* be a post alongside the showcase/multiplayer video (for real this time).