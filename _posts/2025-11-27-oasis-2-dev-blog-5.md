---
title: "OASIS 2 Dev-Blog #5"
category: oasis
tags: [devblog]
excerpt: in this one i'm focusing on weapons and bots
gallery:
  - image_path: /assets/images/posts/oasis2_blog5/makarov1.png
    url: /assets/images/posts/oasis2_blog5/makarov1.png
  - image_path: /assets/images/posts/oasis2_blog5/makarov2.png
    url: /assets/images/posts/oasis2_blog5/makarov2.png
---

Hi! Welcome to another bi-monthly (for now) post on my progress on OASIS 2. If you're not aware of this project, this is the prequel to my previous game, [OASIS: Tokyo](https://store.steampowered.com/app/2531340). It is a single-player/co-op cyberpunk FPS set 20 years before the first game. You can read more about it in the previous dev-blogs, such as [this one here](/oasis/oasis-2-dev-blog-3) which details the expanded gameplay loop and multiplayer co-op.

Work from the Project Roundup post up until [Dyskairos's](https://store.steampowered.com/app/3463170) release was pretty stagnant, as I was focusing on fixing and polishing it up as well as preparing for its release in general. Now that it's out though, I've started fully working towards a showcase of some sorts for this project (no date on that though right now).

As a side-note, like I mentioned before, Dyskairos is largely a finished game. I feel like I accomplished what I set out to do on that and I'm happy with it (even if some people may not like it). However, I am planning on *at least* one additional update featuring that Weekly/Daily run idea originally stated in the [Project Roundup](/misc/project-roundup-1#dyskairos). That will likely be coming in Jan/Feb, after the upcoming Winter Sale.

## Weapons

Anyway, onto OASIS. As always, this is should be considered a massive work-in-progress, but in the last few weeks I have made substantial strides in the way of weapons. I'd like you to meet a potentially familiar face:

{% include gallery caption="Note: These screenshots are very small because the game is currently only being ran in a relatively small window to make seeing both perspectives easier. Sorry!" %}

The Makarov PM, also used in the original OASIS, is the first *actual* weapon being implemented. It is also serving as a test bed for new improvements over the original game:
- Multiple ammo types
- Check magazine
- Attachments changing the size of weapons
- Dynamic item icons and drop models
- Near-wall animation and other new animations
- And more!

The plan is to eventually reimplement most (if not all) weapons from OASIS: Tokyo, and add new ones as well! To start with, I will probably only do 4 or 5 weapons though - one of each major "archetype" (eg the Makarov is pistol, maybe a M4 as a rifle, some shotgun, maybe a smg, maybe a melee weapon, and a medical item or 2 which will technically be weapons (and were in 1 as well)).

## AI

I also want to go a bit in-depth on how I'm planning to implement the AI, since I'll likely start on that in the coming weeks. I'm still planning to structure it similarly as the AI are in [koi](/koi/koi-bots), my bot warfare-inspired side project. As it is, there will be two levels to each bot: A "low-level" AI, which will handle combat and the actual moving around, and a "top-level" AI, which will decide on what it should be doing when not directly in combat. These two levels will have their own personalities/roles that determine how they act.

The low-level AI will work similarly to how the AI in OASIS: Tokyo worked, but in a more broad sense, instead of solely being based on faction. Here are the "personalities" currently being planned:
- Normal (this is default balanced behaviour, strafing around until their target hasn't been visible for a certain amount of time where they'll push their last known position)
- Aggressive (these will push their target quickly, and more quickly strafe closer to their target)
- Defensive (these will not typically push the target and camp angles, similar to how some SectCom worked in Tokyo)
- More personalities with unique behaviour will likely be added in the future

The top-level AI will have a "role", which determines where the AI should go out of combat and how to respond to nearby friendlies getting into combat (and such).
Here are the roles currently planned:
- Guard (default behaviour, similar to how typical enemies worked out of combat in Tokyo, they'll patrol around their area and investigate sounds)
- Hunter Leader (will actively seek out nearby enemies and sounds)
- Defense Leader (like guard, but with a higher sound detection range. if they hear a sound, they'll direct a nearby guard to investigate it if there is one instead of them)
- Objective Leader (will spawn with an intended objective in the map of some kind, likely reaching a certain location. they'll try to make their way to that location and then leave. similar to corp squads in the facility in tokyo)
- Follower (will follow a specified bot or pick one nearby to follow if spawned without a leader)
- Again, potential for unique roles in the future

If it isn't obvious, I'm largely planning to add mostly the same AI types found in Tokyo and expand from there (though Defense Leader is entirely new, delegation isn't something the old AI did). Flanking is a potential option I might try to look at eventually, as an example.

## Future

That's about all I have to say for now. As I've stated previously, I'm planning to more publicly reveal the game with a "showcase" video of some kind, likely with a co-op mission demonstration. I was aiming for sometime in December for this, but it will likely end up being in January or February. 

Following this, I'm going to expand it into a vertical slice/demo of some kind. It will likely only feature a single region (maybe 2), as well as the time system,  plus some quests, etc. This may or may not be publicly available. Currently, my plan to try to get a publisher on board, and that is meant for that. *(if you are one and are interested in picking this project up please email me!! my email can be found on this site's main page)*

I'm going to continue these monthly blog posts, though I'm currently unsure what December's will be about. If I make significant progress over the next 2 or so weeks (since I typically post these towards the beginning of the month instead of the end like this one), it may end up being another OASIS Dev-Blog, but if not it may be another Project Roundup or such again. Thank you for your support! See you then!