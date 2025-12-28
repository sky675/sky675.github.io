---
title: "OASIS 2 Dev-Blog #6"
category: oasis
tags: [devblog, game-ai]
excerpt: in which i've created some ai (the cool kind). the game is also now technically playable (kinda)
---

Hi! I've made fairly significant progress and it is nearing the end of the month (as I mentioned previously, I didn't really have any posts for this month planned). So I figured this could be a bit of a "preview" for the planned showcase early next year. As always, this is currently in active development, should be considered very much a work-in-progress and could change at any moment for any reason.

## AI

First off, the "standard" AI has been implemented. They have 1:1 feature parity with OASIS 1's enemies (and in some cases might be better?). They can strafe, chase lost targets, investigate sounds, run to cover to heal or reload - everything the first game's AI could do, and more! Since the AI use the same weapon manager the players use, the AI also naturally support being equipped with multiple weapons and can use actual items. 

To explain, in OASIS: Tokyo AI healing was largely "fake": it would hide their weapon, show a bandages healing anim, and a standalone healing effect would be applied while the animation plays. They could do this as many times as they want as long as their HP was below the threshold for switching to that state. 

In OASIS 2 they have actual references to the items they are using - they're actually the same items players can use - making it fairly easy for the AI in the future to do things such as: Using non-healing med items (such as a damage reduction item) when getting near a place they're investigating, throwing a grenade, or simply just drinking water randomly. Since they are, again, the same items players use, they'll also run out of those items as well.

![aifight](/assets/images/posts/oasis2_blog6/aifight.png)

This is a screenshot of a small AI vs AI fight in a quickly made test arena I've made to demonstrate the current state of the AI (and the game as a whole). AI also now can have dynamically generated weapons. They'll have a chance to have various attachments on their weapons or even use different ammo types and magazines.

## Level Generation

![levelgen](/assets/images/posts/oasis2_blog6/levelgen.png)

Recent work has also been done in the level/mission department as well, and I've added in enviroment pieces that are the first pieces of the Offices map type. Levels can be generated with them right now (though they are a bit limited as there are only two empty rooms for it to choose from and no lighting). Also with that, initial patrol AI spawning have been implemented. 

As such, the game is now *sorta technically* playable! You can accept a mission, go to it, and find enemies to fight on a randomly generated map. However, objectives still need to be implemented - currently you automatically win after being in the map for 5 seconds.

## Future

Obviously, I'm not quite ready for a more public reveal/showcase yet. But it is getting there! I'm currently aiming for potentially February for that showcase now. Next I'll likely be working on expanding the Offices map type and will also be implementing the first and most basic objective type: Elimination. With that, I'll also begin implementing other mission-related features previously mentioned in earlier dev blogs such as events (reinforcements, etc).

If you'd like to support me in this game's development, please buy [OASIS 1](https://store.steampowered.com/app/2531340) or [Dyskairos](https://store.steampowered.com/app/3463170) if you haven't already! They are currently on sale for this year's Winter Sale. As always, thank you for your support.