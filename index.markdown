---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: splash
#classes: wide
#full-width: true
title: skaaie
masthead_title: Homepage
tagline: >- 
  I'm sky, currently a solo game developer. I am primarily a programmer and game designer, and specifically enjoy trying to create unique spins on the FPS genre. 
  <br><br>
  I have around 7 years of experience with Unity and C#, and began working in Godot (using GDScript) as my primary engine in 2024. I also have some experience with Lua from my Garry's Mod days.
  <br><br>
  Below you can find a portfolio of projects I've worked on!<br>In the navigation above you can also find my blog posts.
header:
  no-bottom: false
#  overlay_image: assets/images/library_hero.png
  actions:
   - url: mailto:skaaiedev@gmail.com
     label: "Contact Email"
---

## OASIS: Tokyo - Solo Developed
![oasis](/assets/images/vlcsnap-2023-05-30-19h02m20s512.png)

[OASIS](https://store.steampowered.com/app/2531340) is a semi-tactical FPS with roguelite elements set in a cyberpunk version of Japan with a focus on inventory management. In it, you need to increase your reputation in the underworld in order to find the fabled "Oasis", a hidden location shrouded in mystery. While doing this, you must contend with limited inventory space and need to balance sufficient ammo and meds with extra bag space for loot.

This is my first commerical project I've released and was made with Unity. About 95% of scripts the game uses was written by me from scratch over the span of about 3 years, including the menus, enemy AI, weapon functionality, and inventory systems.

I've also started work on a sequel using Godot that is in its early stages. My goal with the sequel is to evolve the ideas of the first game with added multiplayer co-op support.

## Dyskairos - Solo Developed
![dys](/assets/images/vlcsnap-2025-01-28-03h18m34s404.png)

[Dyskairos](https://store.steampowered.com/app/3463170) is a metroidvania-inspired FPS with roguelike features. You find yourself trapped in the vicinity of a mysterious tower and must find a valuable material stored at the top of the tower in order to escape. In order to climb it, you'll need to adapt to find a way to the next floor and then back out of the tower before the tower's cycle finishes - which will shuffle the items inside around.

This is my second commercial project. It's my first major project in Godot. Development started in late 2023 after experimenting with the engine (due to you probably know what), but was sidelined in order to create post-launch content for OASIS. I returned to this while working on OASIS: Tokyo v1.4 (around October 2024, with it becoming my main focus once that was released in November).

I started this project with the goal of creating as many assets as possible myself. The only models in the project that weren't made by me are environment props (save for one enemy and half of another enemy).

## Digidrone - Game Jam Game
![digidrone](/assets/images/digidrone_FXP1eLm6Zf.png)

[Digidrone](https://sky675.itch.io/digidrone) was made for the GMTK 2024 game jam with [a friend of mine](https://github.com/NateStanley). It's a short (<10 min) puzzle game where you play as two robots navigating a post-apocalyptic environment. 

I handled most of the coding (excluding the intro ui and the audio log playing ui) as well as created the map, designed the puzzles, and sourced sound effects. My friend created the 3d models and other textures. It was my first released project in Godot.

## Iterations - Game Jam Game
(no photo)

[Iterations](https://sky675.itch.io/iterations) was made for the GMTK 2025 game jam with [the same friend of mine](https://github.com/NateStanley). It's an arena shooter roguelite about an AI stuck in an infinite training loop where it is forced to fruitlessly defend its ship from an impending attack.

As with Digidrone, I handled most of the game design, coding (excluding the visuals of the UI), created the map, and sourced textures and sound effects (excluding the VO). It was my first time properly using a CI/CD build workflow in order to easily update the game on itch. Similar workflows are currently being used for my current projects.

## StalkerRP - Community Project
![ppl](/assets/images/hl2_JI82pfAuj2.png){: .align-center}

[This](https://github.com/sky675/srpv5) was a Garry's Mod server I developed with the help of [the same friend of mine](https://github.com/NateStanley) which was active from 2016 to 2021 (with some hiatuses). It's a "roleplay" gamemode based on the Stalker game series. 

During the server's life, I created many features that (to my knowledge at least) was unique to the server when compared to similar servers at the time, focused mainly on improving the experience of players. Those features also inspired other features that would later be added to OASIS, other projects and would also be seen in some form in later communities' servers.

## Koi - Side Project
![koi](/assets/images/koi_vXmYK5Pv67.png)

Koi is a side project I've been working on that was originally inspired by the Bot Warfare mods for the older Call of Duty games. In it, I'm creating a moddable offline game inspired by Call of Duty's multiplayer mode, primarily for my desire to watch bots fight (and fight with them) in various gamemodes that aren't in those older CoDs (and also desire for a moddable CoD MP-type game in general, since that doesn't seem to exist at the moment). 

I also have the intention of open sourcing it once it's further along (namely, once it has actual player models or at least support for them instead of just the capsules the game currently is using). 

Development has largely been on hiatus at the moment as I'm busy with both Dyskairos and the OASIS sequel, though said sequel currently has AI based on the [design of the bots](/koi/koi-bots) in this project.