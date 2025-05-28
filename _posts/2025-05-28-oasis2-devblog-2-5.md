---
title: "OASIS 2 Dev-Blog #2.5"
category: oasis
tags: [devblog, modeling]
excerpt: In which I probably should've just waited a week to post the last post.
---

Hi! Rare double blog post for the month here, shortly after posting the [last post](/oasis/oasis2-devblog-2) I decided to look at other options to fix the issues mentioned in that post I hadn't originally considered. This will be an extremely short post, as I just want to give an update on the issues from that post.

{% include figure popup=true image_path="/assets/images/posts/oasis2_blog2p5/vlcsnap-2025-05-28-15h35m23s200.png" %}

I decided to first to try and use the anims I had used in OASIS 1. This worked (and they are absolutely better than the Mixamo animations, and actually had *improved* since the version of them I used previously), but because of this the previous solution for holding weapons no longer worked. 

It was at this point I remembered that SkeletonIK3D was actually still usable - I previously discounted it since it was deprecated, but after some research discovered that the alternative to it [probably isn't coming any time soon](https://github.com/godotengine/godot-proposals/discussions/9885#discussioncomment-9665995). So, I've decided to just implement IK similar to OASIS 1 using it now with the plan of replacing it with whatever the alternative is when it gets added to Godot.

{% include figure popup=true image_path="/assets/images/posts/oasis2_blog2p5/vlcsnap-2025-05-28-16h06m50s922.png" %}

While it works well, it isn't entirely bug free still. The first person hands still have issues, but I've got multiple potential solutions for that planned this time (including just using more SkeletonIK3Ds as a last resort lmao). Regardless, the big issues from Dev-Blog #2 have now been fixed, and I just wanted to write a quick post saying so. Of course, there's still stuff that can be improved and much more to work on, but that'll be at a later date.

Next month's post will be on how I've been making Dyskairos's AI, since I've realized I'm doing that (to my knowledge) somewhat uniquely, it's fairly simple and works really well for me. Please look out for that in probably a week or two!