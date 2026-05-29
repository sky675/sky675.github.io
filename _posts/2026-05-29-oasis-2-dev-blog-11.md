---
title: "OASIS 2 Dev-Blog #11"
category: oasis
tags: [devblog]
excerpt: so close, yet still so far away
header:
  overlay_image: assets/images/oasis2_bannerv1.png
---

Hi! Plan's changed (again). Obviously, I decided not to upload a video of the first multiplayer playtest. A lot of it wasn't really usable anyway - we ran into a lot more issues than I originally thought we would, though they've been fixed and another playtest is planned soon. I'm still planning to upload a video of it, however I will be waiting until:
1. I have the Steam page for the game approved and ready to launch.
2. The previously-mentioned OASIS 1 update is also ready to go.

While building for this playtest, I hit the free github actions storage limit for this month, so it will still be a few weeks. In the meantime, I am also working on expanding the game's current content so the video will have a larger variety of content to showcase.

## Screenshot Utility

{% include figure popup=true image_path="/assets/images/posts/oasis2_blog11/4k_screenshot.png" caption="I've always wanted to include a logo on a screenshot lol" %}

In this blog, I also want to talk about what I made that I'll use for store assets and non-gameplay screenshots. For context, for both 1 and Dys, almost all images and videos were captured in-game during actual gameplay (though sometimes using noclip). This time, I've developed a solution that allows me to make more "curated" screenshots, rather than having to play until what I'm trying to screenshot happens naturally. This comes in two parts: a "DummySpawner" and a screenshot camera.

![node structure](/assets/images/posts/oasis2_blog11/node_setup.png){: .align-left}

The DummySpawner is a node I've made that spawns a specific subfaction of a faction, but then hijacks its intended AI with one that can be controlled using properties on the node and child nodes, allowing me to make it move and look around freely from the editor.

The screenshot camera is fairly simple, it's a camera that can moved around using typical controls, however it is inside a SubViewport that is set to a 4k resolution, allowing me to take screenshots at that resolution without the actual game window being 4k (I don't have a 4k monitor anyway lol) by saving the image of the subviewport's texture to disk. The screenshot above is one of those screenshots! This will primarily be used as cropped screenshots for posts and store assets, so they likely won't ever be used at the actual full 4k resolution (the screenshot above being an exception, of course).

I also tried using Godot's AnimationPlayer with it, and while it worked, I don't find the AnimationPlayer particularly easy to use, so I plan to expand this solution further with scripting that allows me to make repeatable scripted sequences, potentially even cutscenes down the line, using tweens (in a similar way to how [Dyskairos's ai is setup](/dyskairos/dys-composition-ai)).

## New Stuff
{% include figure popup=true image_path="/assets/images/posts/oasis2_blog11/maki.png" caption="Say hello to Maki! She will be the first character you meet in the game and is the driver/mechanic of the truck." %}

Here's a broad list of other things I've added this month:
- added the pump action shotgun (currently has 2 ammo types, buckshot and slug)
- added the M4 rifle plus its semi-auto counterpart (it can be seen in the screenshot further up! all the attachments from 1 are implemented, though i may add more in the future. non-zero chance of them being backported to 1 but not likely, depends on the situation when i make them)
- implemented the gadget attachment type (currently features 3 of the 4 attachments 1 had, other one will be implemented later)
- added "actual" vest and backpack (seen in screenshot above)
- added body masks to character parts to reduce clipping, currently implemented on tops only
- added more clothing meshes (facemasks, etc)
- added an actual "design" for Maki (seen above, could be improved in the future but i'm happy with it right now)
- added lots of things to improve static characters (now supports face customization, looking around, misc animations)
- added sorta temporary representation of the smelmart trader (mostly just need to replace his top)
- improved main truck scene and smelmart scene (i'll likely put them in the video now, originally it would've been just a single mission but these scenes look good now so it'll be a bit longer)
- created some simple actual quests (including the first actual preset missions)
- decided on the "rare money" name, its now called "V-Mon" or "V文" (this is how its referred in the UI)
- added some new reflex sights
- lots of minor/internal things that would be even more pointless to mention than some of the stuff above

I've also setup a workflow for creating automatically generated changelog posts for new test versions. These posts are not indexed and will not be linked directly on this site - though they can be found in the repo for this site on my GitHub linked here - as they're intended for private use in testing (I hit discord's character limit with a build and made this as a result), but they're there if you're interested!

## Future

That's about it for this month! June should be considered tenative for now - as the planned video *is* technically 5+ months late and growing right now. While I'm more confident in the game's presentation now, I'm still not 100% confident so there is a non-zero chance it could be July instead. The primary reason for these delays is that I want this first video introduction to look as good as possible. I want to give this the best chance at getting off the ground I can.

As for the next post, I'm currently not considering writing a post to accompany the video, so it will probably be a post about the upcoming Next Fest. I play a ton of demos in these events and have kept a spreadsheet for each one - primarily for statistic and research purposes - where I track each demo I download. I plan to go over my favorite demos from this upcoming next fest, just so maybe the few people reading this may find something they might like if they like my stuff (though I'm more obscure than most of what I'll likely be showing lol)!