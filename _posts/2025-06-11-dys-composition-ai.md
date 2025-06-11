---
title: "Dyskairos Dev-Blog: AI Composition in Godot"
category: dyskairos
tags: [devblog, game-ai]
excerpt: Talking about my technical design for the enemy AI in Dyskairos
header:
  overlay_image: assets/images/tower1.png
  show_overlay_excerpt: false
---

Hi! Something a little bit different this month, I wanted to talk about how I'm doing my enemies' AI in my current game [Dyskairos](https://store.steampowered.com/app/3463170). I feel like this approach has been very useful and easy to use for me and I haven't seen any examples of anyone else doing it like this, so I figured I'd talk about it a bit as it might be helpful to someone else as well. Apologies in advance for the screenshots of code.

## Background

First, I wanted to start about how I started doing AI in this project. I initially started with using [LimboAI](https://github.com/limbonaut/limboai) which the best solution I could find for me (and is a good solution in general, if you want something already tried and tested I'd definitely just use that), but since it's a GDExtension addon (or its own version of the editor) I relied on it updating with Godot. 

During 4.4's release cycle I wanted to update to it as soon as I could (like moments after its release), so I decided to create my own AI solution instead so I could update the project the moment it came out. At this point I had already made [Koi's Bots](/koi/koi-bots) so inspired by that, my previous systems, and some of what LimboAI did, I created my own system that allowed me to easily create routines unique to each enemy type in my game using reusable components.

## AI Through Composition

{% include figure popup=true image_path="/assets/images/posts/dys_comp/enemy_townsfolk.png" %}

This is part of the script for a new enemy I've made for the full game. The bulk of the AI happens in this `process` method. In terms of complexity, it's a fairly average ranged enemy. It's a bit more advanced than the drone in the demo since it actually needs to reload (the drone technically does too, but it reloads instantly so it isn't very noticable). 

`FindMultiTarget` is a component type I've created just for this enemy type as the original version of the component would look only for the player (small spoiler for the game: these enemies will be fighting each other so that will not suffice in this enemy type's case). This component looks for the player and/or all nodes in a target group nearby with various settings for line of sight and fov detection. When it finds a target, it returns true and so enters combat. Once it is in combat, the component instead simply checks if its target is still valid.

In combat, it will to strafe around to random positions near it, inching closer and closer to the target, occasionally firing in bursts at it and reloading when empty. When it doesn't find a target, it'll simply patrol randomly around where it spawned. These enemies also have a "handler"-like enemy that they go with, that will direct them to attack a specified target that it sees but they may not. To learn more about that though, you'll just have to play the game yourself when it releases. :)

You may notice that other aspects that are specific to the enemy itself, such as handling parts of its AnimationTree, are not handled through a component. These definitely could be done as a generic component, but since they'd likely be the only one using that component I felt like cases like that would be better suited to just doing that in the enemy's script instead.

### Components

{% include figure popup=true image_path="/assets/images/posts/dys_comp/weaponfiring.png" %}

As an example of the individual components, this is the component used for firing ranged weapons. It handles how much it should shoot at one time - a "burst", and then the delay between those bursts. When the component is used for the first time, it enters a cooldown of at least 0.2 seconds before being allowed to fire in order to prevent the situation of immediately shooting the moment a target turns a corner and it sees it for the first time.

This component is very similar to what I used in [OASIS](https://store.steampowered.com/app/2531340) for weapon firing, but contains a few less features as I decided they weren't necessary for Dyskairos (such as checking the angle to the target before being allowed to fire). OASIS 2 doesn't have any real AI implemented as of yet, but it will likely have this weapon firing code in some form when it does.

Below you can see a screenshot of the end result, the enemy in action:

{% include figure popup=true image_path="/assets/images/posts/dys_comp/townsfolkcombat.png" %}

## Conclusion

I hope this inspired or helped you in some way! Or was just interesting short read. Please wishlist [Dyskairos](https://store.steampowered.com/app/3463170) and thank you for reading! Next up will probably be an OASIS 2 Dev-Blog - I'm planning to alternate between OASIS and non-OASIS posts month by month for the time being.