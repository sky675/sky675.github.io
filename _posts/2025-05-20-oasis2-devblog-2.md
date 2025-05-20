---
title: "OASIS 2 Dev-Blog #2"
category: oasis
tags: [devblog]
excerpt: This month was an ordeal and I want to write about it and show it
topgallery:
  - image_path: /assets/images/posts/oasis2_blog2/leaningig.png
    url: /assets/images/posts/oasis2_blog2/leaningig.png
    title: "Leaning :) Still needs to be adjusted. Necks are also fairly strechy, for which I'll probably either try retargeting again (the 'issues' picture is what happened when I tried it initially) or try with different animations."
gallery:
  - image_path: /assets/images/posts/oasis2_blog2/thecolorisfortesting.png
    url: /assets/images/posts/oasis2_blog2/thecolorisfortesting.png
    title: "Fem model. I'm unsure what's causing the weird bits around the neck and the feet being upside down, you'll notice these on the other images as well, though the neck isn't as bad on the male model."
  - image_path: /assets/images/posts/oasis2_blog2/whyitgoupwhenilookdown.png
    url: /assets/images/posts/oasis2_blog2/whyitgoupwhenilookdown.png
    title: "Peculiar issue, when you look down the weapon rig starts pointing up instead (looking up works correctly and in a testing scene it works fine, so I'm not sure what's wrong here either)"
---

Hi! This post was intended to be earlier in the month, but I had a couple of significant issues that was blocking it until now. First off, Dyskairos development is going [along](/assets/images/posts/oasis2_blog2/dys_vz58.png) [well](/assets/images/posts/oasis2_blog2/dys_mech.png). 

I was unable to meet the milestone I had set for the June Next Fest though (ended up reaching it a few days after the deadline lol), so the demo update will now be released to coincide with the October Next Fest - it will likely be in late August, probably with a new gameplay video. At the point of that Next Fest, the game should be finished so the full game will probably release shortly after it ends (in November probably).

As in the previous blog post, I'm prefacing the rest of this post by saying *literally everything* shown in this post is unfinished and/or temporary/placeholder. Anything could change at any moment (and probably will). This is still in *very* early development.

## Character

Most of the work since the last post was spent on getting a weapon and character model system setup similar to what I had in OASIS 1. To be honest, this was fairly difficult and I ran into [numerous](/assets/images/posts/oasis2_blog2/bug_usingfemweapon.png) [issues](/assets/images/posts/oasis2_blog2/bug_whatretargetingdoes.png). Most of these have been fixed, but some still need to be addressed. Regardless, I ended up with probably the closest thing to the old system that I can do on my own. 

The primary pain point I had with 1's design was that I had to do animating in play mode, which was time consuming and wasn't very easy to use. This time, I'm able to do animations externally instead (such as in Blender, which I find much easier to use) and now I can also potentially have someone else animate too without them having the entire project.

There are a couple things left in terms of character-specific stuff (such as possibly adding crouching animations and face/hair customization) and many other things that can be improved still. Regardless, it's all at a decent enough state now that I want to move onto the next core feature, which is level/mission generation.

Below you can find some screenshots of the current state of the project including current yet-to-be-fixed issues. I'm unsure if the remaining issues are related to the models/animations or Godot itself, I'm fairly certain at this point that it isn't my code.
{% include gallery id="topgallery" %}
{% include gallery caption="'Low-Poly HK USP' (https://skfb.ly/6voxW) by TastyTony is licensed under Creative Commons Attribution (http://creativecommons.org/licenses/by/4.0/)." layout="half" %}
I currently don't intend on actually using this model in the game, I just needed a weapon model that already had bones and I already had it downloaded. Figured I'd credit it regardless. If you happen to have any insight on these issues, please email me or something!

## Missions and Levels

To reiterate from the first blog post, in OASIS 2 you'll be mobile, travelling from prefecture to prefecture, with each region having its own "reputation level", similar to the first game. As such, missions will act very similar to how they were in OASIS 1, procedurally generated from various objective types, enemy types, locations, and potentially different modifiers. 

A set of missions will be generated based on the region and its current level. Enemies and locations will change depending on said region, and regions may have unique aspects that can occasionally affect missions. Mission events (such as reinforcements) will also be expanded upon from the first game, including unrelated teams coming in and looking for their own objective (such as the corp teams found in the Facility in 1, which I also mentioned in the first post).

Of course, these "locations" will also be procedurally generated like the first game. I don't really have more to say on that right now, though old areas will probably return in some form and there'll probably be some new ones too.

## The Rest

You also maybe noticed in the screenshots above that I also have hotkeys reimplemented. These work exactly as they did in OASIS 1, so I don't have anything to say on them. I've also implemented magazines and the ability to add alternate ammo types. As I mentioned previously, I'm planning to do "generic" ammo types, such as FMJ, AP, Slugs, etc, (instead of specific real-world types of ammo like M855 or SOST) so that capability is in now. 

You're also able to do magazine checks now. When a weapon is fired the magazines contents will turn unknown and in order to know again you must check the magazine - either via a keybind with the equipped weapon or an item function in the inventory. With weapon HUD cyberware, it will be similar to how it was in OASIS 1 and you won't need to check the magazine anymore, but how much it says depends on the quality of the cyberware (eg a basic HUD will only print broad amounts such as "less than half", and the HUD will probably only show a bar).

That's about all I have for this month, I spent like 2+ weeks trying to fix various issues and only now have something relatively stable and somewhat working correctly. Please wishlist Dyskairos if you haven't already and thank you for the support!