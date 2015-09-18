# Sons of Isra

The idea is to generate an expansive mod that's based around the Sons of Isra cult and their spread across the Overworld.

This mod is not about adding features, so much as it's about adding a system of lore and events that are triggered primarily by chunk loading to provide a more structured, interactive experience that differs from the usual fare of random mobs and formless progression.

One of the main aims is getting the AI to a state where the entities are actually performing actions, building structures and actively taking part in the world rather than semi-passively wandering around waiting for player triggers.

Broad Features:
 - Active entity AI
 - Solid hierarchy of cult structures, with limited spawn numbers and world anchors
 - Multi-branching tech progression tree
 - Deep lore with suitable basic drop rates and tech-gated revelations
 - Option for players to side with the cult and gain reputation
 - Reputation persistence across multiple servers
 - Full custom skinning on all items and entities
 - Complete encapsulation (no reliance upon other mods for functionality)

# Active AI
Instead of having the cult structures simply spawn, there will be mechanics to allow for partial spawns, with the cult entites then setting about mining and processing materials to finish the structures.

The AI will also account for the entity idle time, and have them constantly doing something specific rather than just milling around aimlessly - even if it's just something simple like going on patrol or hunting hostile mobs.

The AI will also make decisions based upon perceived player intent, rather than specific actions. Approach them with an apple, and they'll walk up to you. Approach them with a sword in hand, and they'll start firing. Get them to start chasing you, and they'll constantly do checks of your health and the distance from their spawn point to decide whether it's still worth trying to run you down.

# Hierarchy of Structures
This is relatively simple: There will be unlimited cultist camps, effigies, etc. all spawning in a fairly standard way - but everything else will be world-limited. Say 50 shrines, 20 cultist towers, 5 sacrificial pits and 1 colossal central structure. I'm also considering having things start out with just a single shrine and camps, and having the camps periodically step up until the caps are reached - giving a sense of the cult gaining power over time.

The central cult structure will be an end-game level structure with effectively mini-boss subsections which slowly repair if you fail to take out some central objective.

# Branching Tech Tree Progression
The idea is that rather than just having a single path to a few end-game items, there would be specific, powerful items with a small level of customization, and these would then combine with other short-tree, relatively isolated items in order to move down what is effectively a spec branch.

You build your basics and construct a machine. You can put that machine into one of three states by crafting or adding plugins or whatever, and then it's fixed in that state. It lets you build a higher level machine which makes building items of that state much easier, but if you want to build things along another state you need to go back and construct that first basic machine and redo an entirely different chain.

This should help to develop a sense of having chosen an actual path in the game, rather than just massing resources and being able to instantly leap-frog around logistics problems (I'm looking at you, Applied Energistics).

# Deep Lore and Gated Revelations
In each of the structures (and possibly carried by standard and 'heroic' entities) there will be some level of lore. At lower levels, this will basically just be some basic propaganda about Isra. As you murder your way through higher level cultists, you will receive strategic and/or tactical information about the cult, as well as darker lore regarding Isra.

So you start out just hearing about the cult and that they worship some god called Isra. As you move up, you find out about the sinister militaristic motives of the cult, and probably two or three different perspectives on the cult in general. Some followers are cynical mercenaries hoping for land-grabs and riches, some are pious in their belief in the light of the great Isra, and some are working on the Grand Plan and follow the Truth of Isra.

There will also be an element of tech and crafting involved in this, with players able to build machines and structures which - as well as affording them tangible benefits - will also enable them to gain knowledge as to the true nature and scemes of the cult and their god.

# Cult Reputation System
Basically, you do things for the cult to help them out, and they'll become less hostile towards you. So you don't necessarily need to rampage through shrines to get loot and lore - you can contribute to cult projects and get rewards that way.

This will become a secondary path to the end-game events in the central structure, with different outcomes.

# Reputation Persistence
Exactly as it sounds, though a lot more logistically challenging, on account of needing to keep servers running to track it all.

The core idea is to have individual servers make calls out to one of the reputation servers simply reporting a player name, a reputation status and probably some kind of crypto function to check for valid submits. Though it's probably more secure to have servers make calls for reputation increases and the central servers approving them - as that would allow server-side checks to make sure submits weren't being made too fast and/or across multiple servers simultaneously for a single account.

# Full Custom Skinning
On mod items only, not full for the entire texture set.

Stylistically, it would all follow vanilla themes and pallets. Nothing overly fancy. Something that fits.

# Complete Encapsulation
As it sounds. The mod should not rely on any other mod to function (Forge not withstanding) if at all possible.

Where necessary, functionality will be duplicated rather than copied or flatly imported from other mods.
