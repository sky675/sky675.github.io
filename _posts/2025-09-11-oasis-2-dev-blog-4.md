---
title: "OASIS 2 Dev-Blog #4"
category: oasis
tags: [devblog, mechanics]
excerpt: Main mechanics backend work mostly - Working on trying to setup a good sustainable and expandable foundation for the game
---

Hi! Here's a new bi-monthly dev-blog about the progress of OASIS 2. Most of the development time since the last post was spent on working more on the mission generator and the creation of the region, trader, and time systems as well as integrating the systems into each other. Some work was also done on characters and clothing, but it was mostly preliminary work with not much to show (yet). 

As always, everything in this post should be considered a work in progress and could change at any time. As of right now, I'm still primarily working on this only on weekends (with getting Dyskairos finished and out still being my main priority). And again, this post will be only text because of these things.

## Mission Generator/Region System

As I stated in [Blog 3](/oasis/oasis-2-dev-blog-3), in this game you'll be traveling to different regions around the country. Each region will have its own enemy factions and level distribution. Missions are generated depending on the current region. Regions also have a reputation level, like OASIS 1. As before, at max XP, you'll likely need to complete a unique mission in order to advance to the next level of that region. Read Blog 3 if you'd like more information on these systems, what I said there is generally still correct (though you can find actual implementation details below).

## Trader System

The main feature I've worked on in the last 2 months has been the trader system. Traders will work largely the same as shops did in OASIS 1, with individual categories that can be upgraded using money. Most traders will now also have side quests you can do which will reward you with money, items, new items you can buy from them, or other rewards. 

Traders are heavily related to regions. Some traders may need a certain level in a region before they're accessible and you'll need to be in one of the trader's related regions to access their shop. Their shops will be separate scenes that you'll have to travel to.

Also being introduced is a second currency, a "rare money". I don't have a name for it right now, but it's name will likely be crypto-inspired or somewhat arbitrary (think tarkov's gp coins, that was the start of the idea behind it). This new currency, as the name implies, will primarily be used for rarer/high-end items and will be harder to come by than typical yen.

## Time System

Another new system that is currently still actively being worked on is Time. Actions such as traveling to or from missions, shops, and other regions will take time. Generated missions will now also persist after doing a mission and gradually expire, being replaced the next day with a different mission. As of now (I'm undecided on this - I could have it keep track of other regions' missions while in a different region), traveling to different a region will also cause new missions to be generated.

The time that will get tracked specifically are days (will likely be formatted in a month-day format of some kind with a certain start date though) and the time of day within the day (think like Zenless Zone Zero or Persona with Morning, Noon, etc). Some traders may not be available at certain times of day and certain quests may expire after a number of days. Other time-based mechanics (to use examples from 1: neural chips, export auctions, and limited time buffs) will also use this system instead of real time or a mission-based countdown.

## Other Additions

Here's just a simple rundown of what else I've done with this these past 2 months, unrelated to the 2 systems above:
- Various animation improvements (initially the movement anims were just snapped to based on direction, they're now lerped based on the character's velocity)
- Disconnecting/reconnecting (you previously couldn't leave a server because there wasn't any need to and as of right now it is still hardcoded to use localhost lol)
- Initial implementation of status effects (currently isn't much, but without going into too much unneeded detail, it's a lot more improved compared to how I had to create effects for 1 - in that game, npcs typically had their own version of a certain effect. with this new design, it should be a lot simpler for me to create new effects and will be simpler to implement for npcs since in most cases I won't have to do anything special)
- Initial character appearance implementation (hair/eye/skin color now get set/saved, currently can't be actually picked though)
- Preparation for character/clothing customization (formatting textures into something more usable in order to make them colorable, also created a second set of clothes for clothing implementation - non-gear clothing will likely be its own menu (similar to Quick Mode's appearance dropdowns) instead of items this time)

## Future

I'm currently planning to release Dyskairos in November, as a result November's blog post will likely be about that, so the next update post may be October or December, I'm unsure right now (could be both! My current idea for October's post is an update for every project I've worked on since the last time I posted about that project, including koi and this). 

As a whole, the game's foundation is shaping out fairly well, at this pace I *might* have some sorta-presentable testing gameplay footage ready in a couple months. My next focus (after the Time system is fully implemented, it isn't fully complete yet) will likely be on the character/player side, implementing stuff such as:
- Equippable/changeable clothing and character customization
- General effect types (like bleeding and buffs for the to-be-implemented skill system)
- The reworked stamina system [(mentioned in the first dev-blog)](/oasis/oasis2-devblog-1/#miscellaneous)
- The ability to be revived in multiplayer (a feature from [GMod OASIS](/oasis/the-history-of-oasis/#garrys-mod))
- Improving my current implementation for leaning (it's a bit lacking tbh)
- And other things!

Lastly, please wishlist [Dyskairos](https://store.steampowered.com/app/3463170) and let me know what you think of the new demo version via Discord (in the footer)! Wishlisting that game (and buying it once it releases) will directly help in the development of this one. Thank you for your support!