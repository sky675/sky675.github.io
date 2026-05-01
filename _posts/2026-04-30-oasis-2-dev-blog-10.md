---
title: "OASIS 2 Dev-Blog #10"
category: oasis
tags: [devblog, mechanics]
excerpt: i should probably stop trying to announce dates lol
header:
  overlay_image: assets/images/oasis2_bannerv1.png
gallery:
  - image_path: /assets/images/posts/oasis2_blog10/vlcsnap-2026-04-14-14h19m56s370.png
    url: /assets/images/posts/oasis2_blog10/vlcsnap-2026-04-14-14h19m56s370.png
  - image_path: /assets/images/posts/oasis2_blog10/vlcsnap-2026-04-14-14h23m30s696.png
    url: /assets/images/posts/oasis2_blog10/vlcsnap-2026-04-14-14h23m30s696.png
  - image_path: /assets/images/posts/oasis2_blog10/vlcsnap-2026-04-30-20h30m17s409.png
    url: /assets/images/posts/oasis2_blog10/vlcsnap-2026-04-30-20h30m17s409.png
---

Hi! So, obviously I didn't upload anything this month. However, there was still a milestone this month! I had the first multiplayer playtest a few days ago. Due to various issues, none of the missions we played were really suitable for a video. Most of those issues have been fixed though, so another one should happen over the next week, and I *should* have decent footage from it this time! If it hasn't been uploaded already, you can expect a video of a multiplayer mission on my channel in the next few days. In the meantime, I do have some screenshots to share, both from solo playtests as well as the first playtest!

{% include gallery %}

In regards to the rest of the roadmap, mentioned in [Dev-Blog #9](/oasis/oasis-2-dev-blog-9), that will largely remain the same. I firmly believe the Steam page will be up by July (will likely be in June, but no promises lol, definitely will have bought another app credit to make the page by that point at least). Once the page is up (or at least ready and in the review queue), I'll work on the mentioned Tokyo update. I'm planning to push that update with the page's launch and the trailer/2nd video.

In regards to actual development, here's a list of the major work I've done in the past month:
- implemented audio for equiping/moving items, as well as various item functions (clientside)
- further improved mission generation by changing its pools to use a rarity dictionary similar to loot lists (this way i can easily make certain objectives/areas/factions rarer than others)
- new rooms for office, new entrances, new material variants
- added some background buildings for use, some recreated from 1's probuilder models, some brand new
- added an actual scene for currently only shop (smelmart), currently its missing props inside and the actual trader (or the representation of him at least)
- added a soundscape/reverb system
- unfinished/abandoned mission state has now been actually implemented (leaving while mid mission, oasis 1 had this)
- first set of stats: weapon specialization (now just named after their types because specialization was too long), fitness, strength, and negotiation (representations of the main trees from 1), currently no skill trees to go with them yet
- stamina regen item (water bottle), can overheal stamina in run (you dont lose max stamina anymore as a reminder, with some other changes that can be found in the previously linked Dev-Blog 9)
- implemented various task and reward types for quests, as well as 4 quests (to start with)
- add first set of cyberware (low tier eye-cyberware, mods for the existing hud elements, armor, as well as some misc ideas i could make with the stuff already implemented, though those largely have temp names rn)
- added the ability to customize parts of your face (new eye iris/highlights, eyebrows, etc), also implemented on bots
- added a second objective type, Retrieval

This is a relatively short one this month. To be honest, this is largely just to get my monthly post in. As such, I don't have too much to say as a conclusion, so thank you for your support!