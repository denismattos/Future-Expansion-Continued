# Forewords
## 4.1.4
I imagine some would argue against a change in documentation warranting a new release, especially considering most players browse Unciv mods through the game client, that doesn't display documentation in any way.  
But I'd argue this is an update – and, correspondingly a release – of the reupload side – as opposed to the mod side – of the repo.  
As I stated on the readme, my first and foremost aim with this reupload has always been preservation. This is, actually, the most important aspect of the repo to me. I'd want the mod to continue in any way or form, regardless of me having any hand on it.  
And, since I haven't found a list of mirrors anywhere else, I believe this update is very relevant, indeed.
***
Future Expansion – Continued is approaching the end of my original plans when reuploading the mod.  
I still need to correct the mod's yellow errors currently reported by Unciv, but that will recquire a greater understanding of how the game handles mods, that I don't currently have.  
I will now attempt to start tackling that, so I can achieve a mostly definitive release, go to maintenance mode – only following up on Unciv's updates and fixing reported issues – and focus on my as-yet-unreleased mod of Future Expansion.
## 4.1.3
I'm strongly concerned about information loss and would like to think it's a personal cause for preservation, but truth is me being prolix and a hoarder probably has a lot to do with it.  
Anyhow, I'm doing some cleanup, but taking measures to preserve what's being removed by moving to alternative locations, instead.

When [I had to update the mod due to a change in the game's checks' stringency](https://github.com/denismattos/Future-Expansion-Continued/blob/main/forewords.md##4.1.2) it got me thinking about Sullien's code comments.  
There's [a whole movement against commenting code](https://www.google.com/search?q=don%27t%20comment%20code), but I'm personally mostly favorable to comments – again: prolix.  
In this case, however, arguing is moot, as [.json is a format that doesn't support comments by design](https://www.stefanjudis.com/notes/why-doesnt-json-support-comments/). Who knows when Unciv's checks might start being stringent about that, too?  
That's why I'm removing all of Sullien's comments from the .json and preserving them on [a separate file](https://github.com/denismattos/Future-Expansion-Continued/blob/main/authors_comments.md).

I'm also moving all previous and any forthcoming updates' forewords to this separate file, here.
## 4.1.2
TL;DR: I had to pick a terrain for a natural wonder, because one of the game's checks became more strict.

RtFM:  
Starting with [4.8.15](https://github.com/yairm210/Unciv/releases/tag/4.8.15), Unciv's ruleset validator requires all Natural Wonders to contain `turnsInto`, an attribute that [determines which type will the base terrain be after the map generation places the wonder](https://yairm210.github.io/Unciv/Modders/Mod-file-structure/3-Map-related-JSON-files/#terrainsjson).  
As of 4.11.16, there's no way to escape this check, so a Natural Wonder must necessarily change the base terrain it's placed onto.  
This wasn't the case when Sullien developed Future Expansion and this presents me with one of the common issues with reuploading old mods: making decisions over work that isn't actually mine.

The obvious solutions, as was pointed out to me on the game's Discord, are simply picking a terrain type that makes sense or creating a new terrain type to use with the wonder. However, both solutions mean I will essentially be creatively altering the mod, something I specifically want to avoid on this reupload (I'm planning a fork with my own modifications, but it's still a WiP.).  
If the wonder in question's `occursOn` attribute had only one terrain type listed, this would be easy (I'd just pick the same type), but it lists 2: Desert and Plains – which makes sense, considering Sullien's inspiration was likely the monolith from [2001: A Space Odyssey](https://en.wikipedia.org/wiki/2001:_A_Space_Odyssey_(disambiguation)), which, at least in [the movie](https://en.wikipedia.org/wiki/2001:_A_Space_Odyssey), appears on an arid landscape.

The stopgap measure I implemented was picking Desert as the modified terrain type, considering [the landscape in the movie is exceedingly arid, with only rocks and dust](https://th.bing.com/th/id/OIP.B3yBG_AcusZNl0l_F3Q1iAHaEK?rs=1&pid=ImgDetMain), and the Plains terrain type is meant to represent more of a semi-arid climate, as indicated by [the base terrain having 1 Food and 1 Production yields, both in Civ 5 and Unciv](https://breeze.nohost.network/civilization/wiki/Plains_(Civ5)), as opposed to Desert, [which yields nothing](https://breeze.nohost.network/civilization/wiki/Desert_(Civ5)).  
(The best solution would probably be creating an Alien Monolith terrain type, but that would recquire a knowledge of the game – i. e., Kotlin – much greater than my currently meager understanding and, also, some artistic skills I lack and don't have the time to develop – at least, not now.)

However, I intend this to be temporary, as I feel the game should allow the base terrain beneath a wonder to remain the same.  
In fact, I'd argue the very allowance of `occursOn` for a list of strings implies demanding a definite type in `turnsInto` breaks coherence in terrain design.  
For whatever it's worth, [I've already suggested the devs implement a provision to not change the terrain](https://github.com/yairm210/Unciv/issues/11689).  
I could try pushing this myself if I knew more Kotlin, but, as I said, that's not the case.  
Maybe I'll be able to do it, in the future, if someone's not already done it, by then.  
2<sup>nd</sup>-best solution could maybe be the new, dedicated terrain type. But I'd rather pursue the former.