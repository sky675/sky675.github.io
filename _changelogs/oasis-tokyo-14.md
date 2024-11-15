---
title: "OASIS: Tokyo v1.4 Changelog"
site-title: "OASIS: Tokyo v1.4 Changelog"
toc: true
toc_label: Changelog
full-width-toc: true
nopage: true
header:
  overlay_image: assets/images/quarantine.png
  show_overlay_excerpt: false
excerpt: iwakura welcomes you!
---

Hi! It's officially been a year (and about 2 weeks, had to delay a bit) since OASIS: Tokyo released on Steam. This fourth major update includes new main mode gameplay in the Questing System, detailed below, as well as a reload animation remake for every weapon, 4 new weapons, and more.

# Questing System

{% include video id="VcIiT0xx8Vc" provider="youtube" %}

The primary new feature in this update is the new questline, available at max rep. It's my attempt at a bit of a more traditional quest/task system. This includes a somewhat short questline featuring a new character, Iwakura, available once reaching the max reputation level.

She can be found behind a "new" door (the door existed before, but wasn't interactable) in the side alley of Arinobu. This door is locked unless you're at max rep. Iwakura has a set of tasks she needs your help with, and in return you'll get rare/special rewards for those tasks, including a little reward for completing them all (listen for distant gunfights in the village maps during the Oasis Hunt).

In order to complete those tasks, you'll need to visit a new area, accessible from her hideout: The Saitama Group Facility.

## The Facility

Missions in this area are intended to be a bit longer than typical missions (the entire map is around 2-3 times larger than a typical warehouses level), so stamina usage is reduced in the level to accommodate this. As you progress in her tasks, you'll gain access to more of the map. Along the way you'll also encounter corporate espionage teams with their own objectives on top of the typical security found inside, as well as 2 new bosses.

{% include figure popup=true image_path="/assets/images/nara.png" caption="One of the new bosses, Nara, and his second-in-command Maeda." alt="probably couldve tried to get a shot of both of them together but i didnt" %}

This is entirely optional in order to get an ending on the save. You can just never interact with it and immediately do the Oasis Hunt, this is just a bit more content you can do in the endgame.

# Reload Animation Overhaul

![reloads](/assets/images/reloadswoo.png)

I've went and remade the reload animations for every gun, hope they're at least marginally better than before lol.

Animations are now at least twice as long as a result (~1-2 secs to 3-4 secs in most cases, empty rifle reloads are now around 7 seconds and are the longest)

# New Items

Not too many new items this time, mainly just some new weapons.

## New Weapons

- [PM-9](/assets/images/pm9.png) - 9x19 SMG, 25 round mags
	- been wanting to add this for a while, finally found a model i liked and adjusted it a bit to fit the game's art style
- T95 - 5.45 bullpup AR, 30 round mags
	- wanted to add a second bullpup, but didnt want to add another 556 rifle. also didnt want to add 5.8 as an ammo type so this is in 5.45 lol
- 2 new locked container weapons: 1 shotgun ("To-Jyuushi", mag-fed) and 1 rifle ("Kaibutsu", 7.62 AR), rounding it out at 1 container for each weapon type.

## New Cyberware

![obj](/assets/images/objtracker.png)

- New Sonar-type level 3 eye cyberware "Objective Tracker" that shows where **inanimate** objectives (servers, objective items, etc) are on use 
	- Has a much slower cooldown and recharge rate compared to the Sonar, but will still benefit from the Sonar tech skill
	- Primarily intended to help players that may end up having a hard time finding objective items in the new questing system area, but will work in normal missions as well
	- This will however *not* show where the exits are in Oasis Hunt missions, so it's a bit useless there

# Quality of Life

- Added missing mag release button to VZ 3 model
- Mogaki and other IT corp areas now have a higher chance to have rarer tech spawn as loot (**flash drives**, phones, etc)
- SectCom SWAT can now use the helmet without a mask (purely visual)
- Added a little sound when activating the keycard reader in the finale scene (same sound can be found in the new scene as well)

# Balance Changes

- Boss followers will now also give their own target to their boss if the boss doesnt have one (which will then propagate the target to the other followers)
	- This will make Ogura and her followers a bit more aggressive
- Added a 25% increased recoil multiplier to the Control (yellow hand) hack when applied to the player
- Initial spawned AI distribution in the ending has been adjusted, KAMI's units should be more common now
- Added an extra hardware mod slot and a software mod slot to the IdeSys M2031 (will need to rebuy it, it will not retroactively add the new slots, sorry)
- Reduced the duration of the Blind (vision interference) hack when applied to the player from 10 seconds to 7

# Fixes/Misc Changes

- Disabled Unity analytics
	- I disabled collection from their dashboard on October 2nd, this is removing the analytics stuff from the code and the menu
- Fixed boss followers not actually getting the target of the boss as intended
- Minor adjustments to a certain secret area, primarily just changed a few minor details
- Fixed 5.45 AKs (74, AN-12) not accepting the aftermarket 5.45 TMag (never added it to its list it looks like woops)
- Fixed the homing range and radius software mods having the wrong path, breaking the stash in the save when they're obtained
- Added further safeguards so any other items i forget to update the path of shouldnt break the save
- Fixed the Custom AK hanguard turning into a IMA AK handguard while attached, resulting in a broken reload since the IMA handguard isn't supposed to have a grip slot (AKs that were broken from this will still be broken though)

# Known Issues

If you encounter SWAT-type (SectCom or Security) enemies that are kinda just everywhere ([like this](/assets/images/abomination.png)), unfortunately I have absolutely no idea whats actually doing this or how to fix it. I haven't ran into it with Bake Characters off, so maybe make sure thats off (not 100% sure if this will fix it tbh, it will also not change characters that have already been spawned anyway). This issue produces 0 errors and doesn't happen in the editor so I'm really at a loss here. Their hitboxes do still work when their clothes are like that though, so they *should* be killable and otherwise act like any other enemy. Otherwise, restarting the game will also fix it.

# Future

Like I mentioned previously, this is intended to be the last major update to this game so I can fully move on to new projects - unless I get an idea for something I really wanna add. *(tho tbh a sequel(/prequel?) of some kind with godot in a few years would be more likely than me making another major update, unity has become a pain for me to work in. the issue in known issues above being a fairly decent example. godot has its own issues, but i prefer its workflow much more atm, my new projects are using it)*

There is however a new project I've been working on you may or may not be aware of and might find interesting if you like OASIS!

My newest project - previously known in earlier changelogs and elsewhere on this site as "The Tower" - Dyskairos, now has [a demo I released recently on itch](https://sky675.itch.io/dyskairos). It's an FPS with roguelike and metroidvania elements, in which you ascend a mysterious tower in order to find a rare crystal that you need in order to leave. The demo includes the first two floors, please let me know what you think! (steam page coming probably in a few months at least, full release planned to be probably late 2025)

Whether or not you check out the Dyskairos demo, again I hope you enjoy 1.4! Please report any bugs or issues you find in either in the discord.