---
title: "OASIS 2 Dev-Blog #7"
category: oasis
tags: [devblog]
excerpt: so close but not quite close enough yet. (some rambling included)
---

Hi! Here's another progress update. Not too much to talk about for the intro here, like I said last time it is *technically* playable, but I need to flesh the content and visuals out a little bit before the showcase video can be made. As always, this should all be considered very much a work in progress. 

Originally I was going to add some screenshots to this post, but I'll save it for a pre-showcase post or such as the ui is still being worked on, and I'd rather show it when it is done (and also it's nearly the end of the month plus I don't think anyone is actually reading these lol).

## New Features
As a start, heres some highlights on some new things I've added in the past few weeks.

### Control Modifier
Like in 1, crouching will also not be a feature in this game (for the same reasons as 1 too lol). Instead, Left Control (default key) is now a "modifier" key. It's used to do alternative actions depending on the context. Currently, these are the actions that can be done:
- Holding it in general slows your movement speed, it also reduces the auto detection range of AI vs you (movement speed changes in general will also change it as well)
- Holding it + Interact on a dead player will revive them, provided you have a `Revive Kit` in your inventory (this is a mechanic from [GMod OASIS](/oasis/the-history-of-oasis)). Currently there is only one type of revive kit, but in the future I'll probably add different variants, much like the Lifeline cards in OASIS 1. Additionally, if the player was killed via headshot they cannot be revived. As a reminder, player corpses are lootable so in this case their gear can still be saved, you'll just need to carry the gear yourself out of the map.
- Holding it + Interact on an equipable item will have it skip trying to equip the item, putting it straight into your inventory (if theres room) instead. (as of writing this has a bit of an issue, as there *is* rotation, but it currently doesn't try to rotate the item to fit it in the inventory, so you cannot pick up a 2x1 item into the pockets since it is 2 1x1 slots and 2 1x2 slots. this'll be fixed later.)

### Bleeding
Bleeding has received a minor rework compared to 1. Internally, instead of there being one bleeding effect that is applied multiple times, it is now one effect which has stacks added to it when a bleed happens. Aas such, bleed damage will now come all at once instead of at varying intervals. Certain ammo types will also have the capability of applying multiple stacks at once (random chance). AI are now also affected by bleed (they weren't in 1). Currently they don't really react to the bleed specifically but they can remove stacks by using healing items that remove stacks just the same as the player can.

### Time of Day
As also mentioned previously (first in blog post 3 i think?), the general gameplay has also changed compared to 1. You can read more about it there (the idea hasn't changed too much since I wrote that), but the gist of it is there is now a time system. Generated missions now persist after completing a mission and expire after a number of days. Traveling to different areas and missions change the time based on the distance or how long you took in the mission with 5 different time of days it cycles through per day. This has now been fully implemented with a sky that changes based on the current time.

### HUD
I've begun working on the hud. As in 1, it will be modifyable via cyberware to a varying degree, but there are some new base features. I've added nameplates and a pinging system for multiplayer. Nameplates work pretty typically, they'll show their name above their body as well as their chosen color (there'll be a color selector in the settings where you can specify a specific color to use, which is independent from the selected save file). When not visible, they'll still be trackable in the world via a little indicator with their color. Pings are also fairly basic, it places a UI element at where you're looking temporarily that others can see. 

As I have stated, I *do not* plan on adding any form of matchmaking - multiplayer will only be via lobby codes/invites. So while I'm currently not planning on adding any kind of voice chat (as I'd expect people to already be in Discord or such), there is a text chat. *(There is a small voice in my head saying it'd be funny to try to add proximity chat anyway though.. Maybe with a radio cyberware and/or item too.. We'll see.)*

## More Map Generation

The main thing I've been working on is further work on map generation, more specifically with the offices map type. There are now lights (which are fake since I was getting light bleed when lighting for them was enabled, but it looks pretty good anyway imo), as well as doors (which work pretty much the same as 1, though there are some minor AI changes related to them).

Specifically, I've been working on creating more rooms and setting up loot/containers. I ended up writing my own plugin to make it easier to find props/entities of certain types such as containers, as none of the "Asset Placer" plugins I could find had what I was looking for. *(I just wanted to be able to specify certain folders to search and just only show stuff in those folders without having to manually add new assets, so thats what I did.)*

I've also began to work on the UI in general, improving it in general and having actually something there in some places, instead of just the default theme.

## Future

Aiming for video likely in late Feb/early March at the moment, its shaping up quite well but there's a number of things that still need to be done.

With the video there may also be a small OASIS 1 update, I'm planning to:
1. Have it where the last 3 enemies in Elimination head towards the player (this is how the objective works in 2 now)
2. Rework the secret puzzle to not require the radio in the intro (I also reverted the rng values for that radio to near-launch values, those are grabbed from this site so thats live currently)
3. Fix a bug in the Runaway AI action that I noticed while porting that code to GDScript (it makes them run to the wrong side of an object occasionally)
4. Some misc article changes, related to content I'm planning for OASIS 2, maybe some new articles (some lore retcons/previews if you will)
5. Probably add a banner in the menu for this game or something idk *(I'm uncomfortable directly promoting it in the update post since the news posts types specifically say that promotion for another game should only be in the cross promotion post type, but I see promotion for other games all the time that are not that type so idk what to think lol)*

If this doesn't end up happening alongside the video, I'll probably end up doing it with the Steam page launch instead (so there's something for the banner to link to)

On Dyskairos, I'm currently not sure when Dyskairos' weekly runs will be done. I have it planned out, just need to set aside time from this to actually work on it *(its not exactly appealing with how its been selling tbh, to be frank I'd rather work on this which I know at least some people are/were waiting on and I think is already turning out much better than that game did, even so early like this).*

Anyway, that's about it for now. Hopefully next month's post will be accompanied by a youtube video showcasing the game, but we'll see.