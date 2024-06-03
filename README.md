# Future Expansion Continued
A continuation of [@Sullien](https://github.com/Sullien)'s great – and, now, defunct – [Future Expansion](https://github.com/Sullien/Future-Expansion) for [Unciv](https://github.com/yairm210/Unciv).

This continued version merely fixes syntax to comply with Unciv's latest updates.

# WiP Warning
**This mod is still a WiP, limited by my currently restricted knowledge of Unciv, the original expansion mod and even JS in general.  
I can't guarantee its stability or usability in-game.  
I'll do my best to address any received feedback.  
Thanks in advance for your patience and tolerance.**

# Ownership Disclaimer
Inspired by the awesome [@emipa606](https://github.com/emipa606). \=\)

* This is an updated version of an existing mod.
* I claim no ownership of the mod.
* This version may be taken down by request from the original author.
* The original author is free to use this mod to update their own.
* Since I did not create the mod, I will not accept donations for it.
## Foreword to 4.1.2
TL;DR: I had to pick a terrain for a natural wonder, because one of the game's checks became more strict.

RtFM:  
Starting with [4.8.15](https://github.com/yairm210/Unciv/releases/tag/4.8.15), Unciv's ruleset validator requires all Natural Wonders to contain `turnsInto`, an attribute that [determines which type will the base terrain be after the map generation places the wonder](https://yairm210.github.io/Unciv/Modders/Mod-file-structure/3-Map-related-JSON-files/#terrainsjson).  
As of 4.11.16, there's no way to escape this check, so a Natural Wonder must necessarily change the base terrain it's placed onto.  
This wasn't the case when Sullien developed Future Expansion and this presents me with one of the common issues with reuploading old mods: making decisions over work that isn't actually mine.

The obvious solutions, as was pointed out to me on the game's Discord, are simply picking a terrain type that makes sense or creating a new terrain type to use with the wonder. However, both solutions mean I will essentially be creatively altering the mod, something I specifically want to avoid on this reupload (I'm planning a fork with my own modifications, but it's still a WiP.).  
If the wonder in question's `occursOn` attribute had only one terrain type listed, this would be easy (I'd just pick the same type), but it lists 2: Desert and Plains – which makes sense, considering Sullien's inspiration was likely the monolith from [2001: A Space Odyssey](https://en.wikipedia.org/wiki/2001:_A_Space_Odyssey_(disambiguation)), which, at least in [the movie](https://en.wikipedia.org/wiki/2001:_A_Space_Odyssey), appears on an arid landscape.

The stopgap measure I implemented was picking Desert as the modified terrain type, considering [the landscape in the movie is exceedingly arid, with only rocks and dust](https://th.bing.com/th/id/OIP.B3yBG_AcusZNl0l_F3Q1iAHaEK?rs=1&pid=ImgDetMain), and the Plains terrain type is meant to represent more of a semi-arid climate, as indicated by [the base terrain having 1 Food and 1 Production yields, both in Civ 5 and Unciv](https://breeze.nohost.network/civilization/wiki/Plains_(Civ5)), as opposed to Desert, [which yields nothing](https://breeze.nohost.network/civilization/wiki/Desert_(Civ5)).  
(The best solution would probably be creating an Alien Monolith terrain type, but that would recquire a knowledge of JS much greater than my currently meager understanding and, also, some artistic skills I lack and don't have the time to develop – at least, not now.)

However, I intend this to be temporary, as I feel the game should allow the base terrain beneath a wonder to remain the same.  
In fact, I'd argue the very allowance of `occursOn` for a list of strings implies demanding a definite type in `turnsInto` breaks coherence in terrain design.  
For whatever it's worth, [I've already suggested the devs implement a provision to not change the terrain](https://github.com/yairm210/Unciv/issues/11689).  
I could try pushing this myself if I knew more JS, but, as I said, that's not the case.  
Maybe I'll be able to do it, in the future, if someone's not already done it, by then.  
2<sup>nd</sup>-best solution could maybe be the new, dedicated terrain type. But I'd rather pursue the former.

# Changelog
## 4.1.2
Alien Monolith now converts base terrain to desert, to comply with Unciv's current syntax.

## 4.1.1
* Changed instant building abilities uniques values to comply with Unciv's current syntax.
* Corrected a few minor syntax errors.

# Original Mod Description
Mod that greatly expands the late-game eras, with a focus on Atomic, Information and Future eras.

The main objective is to prevent the late-game from feeling stale by introducing new units, improvements and mechanics. 

While this mod extends game length, the goal is to not extend it too long. If you have any feedback/suggestions feel free to contact me.

## Latest Version Changelog(4.1)-9/18/2022

-Lowered all Post-Industrial Tech costs by 10%

-Private Grids now provide -30% Science

-Lowered overall costs of Civilian units

-Unique Cavalry units no longer upgrade to Landships

-Unique Rifleman no longer upgrade to Great War Infantry

-Pillaging Improvements now yields gold

-Completing the Futurism Policy now enables you to purchase Great Spacefarers with faith

-Excavation sites now provide -4 Gold and -1 Culture

-Perks no longer provide negative culture after adopting Constitution

-Modern and later era units are no longer unlocked by Perks

-Reworked Perks so they are now all limited by Eras

-Social Network Company has -5% Happiness

-Slightly buffered Space Organization

-Medical Labs and Tactical Supplier no longer require a Perk

-Recycling Centers and Drones no longer require a Perk

-Late Atomic-Era and Information era Stat buildings no longer require a Perk

-Mechanized Infantry no longer consumes Iron

-Tanks and Modern Armor now consume 1 Oil

-Future-era wonders are now shown on the Tech tree

-Teleport Station now affects Future Soldiers

-Space Elevator now provides Great Person Generation bonuses to all cities, and doubles them on Capital

-Coal Plant now requires the Electricity Tech

-Power Plants now provide -2 power

-Scientific Theory now provides +1 Gold to Trading Post

-Recon now updates to Paratrooper

-Recon, Paratroopers and Future Soldier now gain the Skirmish Promotion

-Stadiums no longer require a Perk

-Ecology now provides +1 Food to Lumber Mills

-Radio now unlocks the Resort Improvement

-Aluminum is now revealed by Replaceable Parts	

--
Should be compatible with any mod that does not directly alter the G&K Tech Tree