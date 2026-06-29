---
title: "OASIS II Dev-Blog #12"
category: oasis
tags: [devblog, mechanics]
excerpt: the "i finally published the page and posted the video" one
header:
  overlay_image: assets/images/oasis2_bannerv1.png
---

Hi! I've [technically already done](/misc/nextfest-june-26) my monthly post for this month, but I wanted to have a post to go along with the gameplay video *finally* being uploaded (if you haven't been reading the previous posts, that was initially planned like 4 months ago). This post will be about describing the main changes and additions for II compared to Tokyo as quickly as I can. You can read the main description of the game on the [store page](https://store.steampowered.com/app/4883680/OASIS_II/) and a more in-depth version of this in a [previous blog post](/oasis/oasis-2-dev-blog-9). I've also got a [general development roadmap](/oasis2_roadmap.md) elsewhere on this site.

- Regions: There are multiple regions you can operate out of, each with their own reputation levels. Each region has their own pool of enemy factions, objective types, and map areas.
- Traders: Each region has different traders each with their own shop inventories and questlines. Quests are technically optional, but provide a variety of rewards for completing them. Traders can only be visited while you are in their region.
- Time: Traveling to missions, traders, and to other regions takes time. Traders have limited inventories that get restocked over time, they may also have quests that need to be completed in a certain amount of time after accepting them. Future features will make further use of this system.
- Improved mission generation: Levels are generated differently and creation of new elements of missions (factions, objectives, etc) is easier. "Preset" missions are now possible, these are used in quests and will have the same layout and settings each time. Loot lists are now dynamically generated from assigned tags of items. Theoretically (there is no mod support *at the moment*), mods that add custom items are possible and their items will be automatically added to existing loot lists (provided they're tagged correctly).
- Improved player controller/weapons: Leaning, animations for checking the current mag, alternate ammo types (ap/jhp/etc), reworked stamina and bleeding, new inventory systems, upgradeable stash, and more.
- New Cyberware system: No more cores, one cyberware per slot type, cyberware can have mods installed to it that modify the installed cyberware or add additional functions. Modular HUD returns as mods to eye cyberware.
- New Skills system: No longer has one main player level, there are various stats each with their own XP source, level and associated skill tree. Gaining a level in a stat gives you a skill point that can be spent in any tree, though many skills have stat requirements. Stats also have a level cap, meaning there are a finite amount of skill points (unlike in Tokyo, where there was technically no limit)
- AI: Enemy AI are structured in a much more iterable way, allowing for more variety in behavior (though right now they all use the same types). AI can use a second weapon and have their own "mini inventory", from which they can use items from. They are still not lootable - though it is also possible now and future enemies *may* be lootable *in certain conditions*.
- Story: This is a prequel. If you know, you know. I will not reveal more than what is on the store page at this time.

## New Stuff
Since I've been doing this each time, here's a list of main things I've added/done since the last blog post (in the past month):
- New map area: Warehouses
- Second region: Chugoku
- Traders for second region: Cyberclinic and Hara
- First skill trees
- New attachments (technically reimplemented, but there is a new angled foregrip i found! besides the dbal attachment (which is mentioned on the roadmap), all attachments have been reimplemented except for a few sights)
- Steam networking implementation (though its technically untested as of writing, waiting on keys currently)
- Lots of balances and fixes, plus setup for future stuff

That's about it for now! I have been doing these monthly, typically at the end of the month, for the last 8 months. Thank you for your support.