+++
title = "Massive Virtual World Simulations"
author = ["Brian Jones"]
date = 2016-08-17
tags = ["game", "dev"]
categories = ["posts"]
url = "/2016/08/17/massive-virtual-world-simulations"
draft = false
+++

Well, it seems some German folk, specifically [vektorweg](https://twitter.com/vektorweg) and [focx](https://twitter.com/focx), have convinced me to write a blog post about some random topic I puked out over Twitter earlier this evening. The following is some convoluted and potentially incoherent rehashing of an idea I've been stewing on for over a decade.

## Background

Before I dive into what the actual premise of this post is I'd like to provide a little background about my mindset.

My first actual gaming experience was on the Atari 2600 when I was a wee lad of no less than 4 years old. Eventually it was the fantasy game genre which ended up being a large part of my gaming career, dating all the way back to original Legend of Zelda on the NES I owned in the mid '80s. A decade later I was logging into EverQuest exclaiming to my little brother playing beside me, "I can finally visualize the fantasy world in 3d! I am in it!" Several years after that Blizzard released their polished version of an MMO, World of Warcraft, which I ended up playing on and off for years. Bethesda released their Elder Scrolls line and I briefly enjoyed the expansive single play worlds of Morrowind, and eventually Skyrim. Fill in the gaps with Neverwinter Nights, Diablo 2, Diablo 3, and a handful of other titles I can't remember, and that rounds out most of my graphical game experience.

I had tinkered with a MUD or two in high school, but it wasn't until sometime after the year 2000 that I actually discovered some of the roots to these games I had played in the form of roguelikes such as Nethack, Dungeon Crawl Stone Soup, and eventually even more bizarre offshoots of the genre like Dwarf Fortress, the latter of which I will focus on in a little more detail.

At the end of the day it's MMOs that kind of piss me off the most. In a way they are what I want, this expansive world with NPCs that I can interact with as I adventure through the world and get stronger. Yet at the same time they are exactly what I don't want, typically heavy handed non-organic story lines where you are thrust into a treadmill-like theme park where everyone standing around you is the world's hero executing the same story as yourself with nothing unique setting yourselves apart outside of whether you spent a billion hours raiding to get that super unique one in a trillion item drop off a boss 99% of the population will never see. Not to mention the NPCs are pretty much locked into an incredibly dull single faceted role of presenting you with a specific bit of story information, or in the rare case stabbing you because your faction state was below their threshold. How boring.

I knew that I wanted more, but it wasn't until I started playing the roguelikes, and eventually Dwarf Fortress, that this realization became concrete.

## Dwarf Fortress - A Small Virtual World Simulation

There are some decently written articles out there about Bay 12 games and the brothers behind Dwarf Fortress which eclipse my ability to explain the game in detail, so if you've never heard of it please throw it into Google and poke around. From my point of view they are nothing short of absolute geniuses who apply their trade for the sake of the trade itself. True artists if you will.

I have my own anecdotal experience which I can share about how perfectly this game shows that given a sufficiently complex system full of simple parts, complex behavior arises.

> For reasons the rest of the dwarfs in the fortress didn't understand, Bobby locked himself in the workshop he eventually designated to himself. The quiet type, usually kept to himself, helped his neighbor, liked his ale, yet there was always something odd about him. Once a guard himself, his companions in the fortress guard slowly became anxious as the days passed, Bobby continuing to stay locked up with no food nor ale. Eventually he lost his mind, stepped out into the hallway in an incredibly mad state, and his guard friends turned on him tearing every limb from his body in a bloody mess. The guards eventually became inflicted with PTSD for killing their old comrade, and the fortress eventually became overran by goblins as the the guard sat in the mess hall moping about over glasses of ale, completely neglecting their jobs.

I don't remember if the accuracy of the above story is perfect, but it does go to show that incredibly in depth stories can occur with the game player only giving marginal god-hand level commands to the actors in the game. Without a doubt this is what I find appealing about games where the developer effort can be completely focused on world and interaction building as opposed to visual bling and fluff.

What bothered me about Dwarf Fortress though was the scale. Sure, I have this group of dwarfs operating within a small section of the world, but I want to interact with the entire thing! I want the AI interactions to be so complex and over my head that it takes a monumental human effort to become even remotely recognized in the world's society no matter how far I travel, no matter how long I live, and no matter who I meet. I want things to be going on around me that I can only hope to glimpse insight towards, and if I am so lucky somehow be able to manipulate to my favor.

The limitation of course is how much of the world a single player's PC can simulate at once. Even though we have multi-core CPUs and gigabytes of RAM at our disposal for next to nothing in cost, it's still not enough to drive a sufficiently complex world. This is why I propose the obscene idea that a company spins up a game server cluster of such obscene and wasteful scale that it can encompass a full world of interactive AI where players are almost nearly the lowest common and unimportant denominator. Not because the human element isn't important! But because you need such a vast world to appeal to a human player in such an organic manner.

## Massive Virtual World Simulations

I [made](https://twitter.com/mojobojo/status/765845734918717440) [some](https://twitter.com/mojobojo/status/765846322381332480) random end of the day [tweets](https://twitter.com/mojobojo/status/765847904615436288) today about this crazy little idea that has been in the back of my mind for over a decade, which sparked writing this whole blog post after being prompted by some random peers out there.

Basically if you were to sum it up:

1. I think MMOs suck because they are just theme parks with predetermined stories, outcomes, and worlds full of nothing but _exactly everyone, who happens to all be a hero, playing the same exact story over and over, dressed in the same end game gear._
2. I think an interesting game world would be one where players are actually _deemphasized_, and the continuous interactions of the AI are actually what shape the world in general.
3. Although it follows (and this is what I gave up trying to explain on Twitter), that players can _eventually_ help shape the world, be it through fiat, power, fame, heroism, fatalism, politics, religion, economics, or what have you. Ultimately they are observers of the world, but players willing to go above and beyond can also _shape_ the world. I think that last point is the most important.

These aren't new thoughts, [CrappyGraphiX](https://twitter.com/CrappyGraphiX) and I have been discussing this for well over a decade now. As we gain more experience in game development, general development, and observe how the game industry has meandered on forward, we've continued to shape and reshape this idea over and over. Unfortunately it's been so far off the charts (even more so than our precious [https://armoredbits.com](https://armoredbits.com)) that we've never bothered to run forward with it. The time and money required to build such a complex world is well beyond us.

When contrasted with Dwarf Fortress, what I propose requires a massive amount of server computing power. It's like taking every world square of Dwarf Fortress and executing what happens between every AI actor in the game in parallel even if an actual human player isn't present to see the results. Given how modern day companies are ran this would be an obscene waste of resources, however, one could argue that given a sufficiently complex system an incredibly rich and interactive virtual world could arise far beyond what we've designed today, _especially_ if it was populated with actual human players who helped interact with it enough to give it shape.

@vektorweg pointed out that what I am proposing isn't a game because by deemphasizing the players I've remove the whole point of participating in the world. Maybe a better term would be "highly sophisticated interactive AI, low level player impact, massively multiplayer world simulation executing in parallel." Either way, what I envision is a system where the player can actually become prominent and powerful, however, their exploits must truly be world impacting achievements as oppose to "I collected 10 bear furs, I'm famous now right?", or following some easily published guide which leads them from level 1-10, 10-20, and so on, so forth. What I envision is an interactive world so complex even the players don't understand how deep their choices affect the system, where each day brings such sophisticated AI interactions that observing said interactions could be a profession in itself.

One example that has clearly stuck in my head over the years is the following:

> As I traveled down the road with my party of friends we came upon a hill from which battle noises came forth. Glancing over the ridge, we became spectators to the most massive battle ever seen in the entire land. There must have been thousands of NPC combatants from either side. When querying a tinkerer NPC pushing his cart past us, he explained that the Lord of the North and the Countess of the West had some dispute they could not resolve which resulted in this near perpetual war. We decided to jump in to see if we could turn the tide of the battle, and gain honor with the side we joined.

Now mind you I'm not sure if those kind of mechanics are possible (specifically the AI tinkerer communication), but I don't think it's too far fetched to consider a system that could be designed where "AI which made their way into high society" could battle each other on some plane in the middle of nowhere over some obscure yet globally understood AI derived political factoid, of which a player could jump in on and establish some kind of fame with the faction they aligned with.

Here is another example I like to describe when explaining how a world can be perpetually engaging:

> After the players wiped out the cavern full of mad dwarfs, eventually the dwarf spirits returned to their bones and the animated undead forms of their bodies remained. Another party of players eventually found the cave and cleared the undead. Yet still the amount of hidden wealth the players never found hit critical mass, attracting the attention of a nearby dragon who took residence there, which became a public nuisance by pestering the surrounding local villages, who eventually spawned a quest to destroy the dragon.

As you can see, in a roundabout way if the world rules are written correctly, while rotating through numerous interesting and interactive scenarios without requiring a full time staff of writers and theme park developers to describe what comes next, the world can perpetually carry on. If done correctly these events can even be less random and tried to an explicit overarching AI story mechanic which makes sense within the context of the given region. One could argue that if a complex enough system was designed the possibilities are nearly endless.

While I have numerous more topics to rant about in regards to building large multiplayer game worlds (the next of which is how standard numerical leveling is incredibly pointless), the final example I will propose is one which addresses singly large worlds vs sharding:

> I signed up on the Brulan server, while my buddy went to the Salagalic server to be with friends in his timezone. I nearly lost it when my buddy said he was going to the city of Xakolako, and I actually ran into him there! The devs lied to us! Brulan and Salagalic aren't actually server shards, they are completely unique locations in one large world!

I suppose you could say that the moral of the story here is that with theme park game worlds you have a limited amount of space. Eventually MMO companies addressed this limitation with a concept known as phasing (or instancing), where players could be in the same space but be seeing completely different visuals based on their quest progress. However, I would prefer to see exactly the same world as everyone else around me. I'm fine with lying to the player base about separate servers, only to have them find out it's actually one massive connected world. Even better, just give the entire player base such a huge selection of places to start and flock to that they naturally spread out anyways. Give them a solid reason to try and forge out on their own, to become heroes, to build towns, to observe the complex interactions of the world and document what happens for others.

## Conclusion

And there you have it, a half baked rant about building overly complex game worlds where the players themselves are actually second rate citizens taking backseat to AI.
