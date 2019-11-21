---
layout: post
title: Modern Rules Problems – Oko, Thief of Crowns
---

All things weirds with Oko, Thief of Crowns in Modern

Sean Tomlinson - L1 Judge

{:class="table table-bordered"}
    | Tex Space    	| Blue Space     	| Lambda           	|
    |--------------	|----------------	|------------------	|
    | sXYZ         	| sBlue          	| sXYZ abcde fghy 	|
    | Jaobe XTZ    	| Blue Game 5.2 	| 5.2              	|


Oko, Thief of Crowns is a very interesting card with a lot of complexity hidden within its rules text. This article will explore the strange and interesting interactions relating to Oko which may not be obvious at first glance. The overall aim of the article is not to have you memorise all interactions, but to give a general awareness of the domains in which Oko applies in strange ways, so that when you get called to a live situation involving Oko, you don’t stray into a trap. 

For ease of skimming and general reading, I’ll pose each vignette in the format of interaction, answer and explanation. Some of these explanations are long and complicated, and I want to avoid the answer being lost or difficult to find.

## +2 Create a Food token.

We’ll start out easy and with a full stomach, nothing tricky here (famous last words). 

<p float="left">
  <img src="https://img.scryfall.com/cards/large/front/4/6/46582e55-c6f4-46e4-a78e-2c586ca4cf4d.jpg?1572489226" width="25%" height="25%">                                                                                                           <img src="https://img.scryfall.com/cards/large/front/3/4/3462a3d0-5552-49fa-9eb7-100960c55891.jpg?1574073631" width="25%" height="25%" />
</p>

## +1: Target artifact or creature loses all abilities and becomes a green Elk creature with base power and toughness 3/3.

There’s a lot to this ability and it makes for some interesting interactions that aren’t immediately obvious. But first, let’s look at the clarifications from the release notes to Throne of Eldraine.

* The effects of Oko’s second and third abilities last indefinitely. They don’t expire during the cleanup step or if you or Oko leave the game. Oko’s third ability doesn’t expire if the creature you take has its power raised above 3 later.

* If the affected creature gains an ability after Oko’s second ability resolves, it will keep that ability.

* Oko’s second ability overwrites all previous effects that set the creature’s base power and toughness to specific values. Any power- or toughness-setting effects that start to apply after Oko’s second ability resolves will overwrite this effect.

* Effects that modify a creature’s power and/or toughness, such as the effect of Festive Funeral, will apply to the creature no matter when they started to take effect. The same is true for any counters that change its power and/or toughness.

* Oko’s second ability overwrites all colors and creature types the affected creature has. It’s just a green Elk. The creature keeps any supertypes (such as legendary) it has, but loses any other card types it has (such as artifact).

* Oko’s second ability may target a permanent that is only temporarily an artifact or a creature, such as Oko, the Trickster. If this happens, the effect causes that permanent to remain a green Elk creature even after the temporary effect expires.

* Because damage remains marked on a creature until the damage is removed as the turn ends, nonlethal damage dealt to a creature may become lethal if Oko’s second ability changes its toughness during that turn.

We’re going to start off with a doozy of a layer system question.

### Does turning Magus of the Moon into an Elk stop it from affecting nonbasic lands?

<p float="left">
  <img src="https://img.scryfall.com/cards/large/front/c/0/c06a4443-6851-4873-8fb8-2ef76c9d6d2c.jpg?1562933679" width="25%" height="25%">                                                                                                            <img src="https://img.scryfall.com/cards/large/front/3/4/3462a3d0-5552-49fa-9eb7-100960c55891.jpg?1574073631" width="25%" height="25%" />
</p>

Answer: No

Explanation: So, what’s going on here? Oko’s +1 ability sets up a continuous effect, Magus of the Moon also has a continuous effect. Therefore, the interactions of these effects are handled by the ‘Interaction of Continuous Effects’ section of the Comprehensive Rules. This is colloquially called the ‘layer system’.

See comprehensive rule 613.1 for a full digest, but in short, continuous effects are applied in a series of layers in the following order: 

Layer 1: Copy effects.
Layer 2: Control-changing effects. 
Layer 3: Text-changing effects.
Layer 4: Type-changing effects.
Layer 5: Color-changing effects. 
Layer 6: Ability-adding effects, ability-removing effects.
Layer 7: Power- and/or toughness-changing effects. 
Sub-layer A: Effects from Power/Toughness affecting CDAs.
Sub-layer B: Any Power/Toughness setting effects.
Sub-layer C: Any Power/Toughness changing effect that doesn’t set.
Sub-layer D: P/T changes from Counters.
Sub-layer E: Effects that switch P/T.

The ability printed on Magus of the Moon is dealt with in Layer 4. It changes the type of non-basic lands to Mountain. The +1 ability of Oko is dealt with in multiple layers. The ability makes the target an Elk in Layer 4 (the same time Magus is applying), green in Layer 5, ability-less in Layer 6 and finally a 3/3 in Layer 7. So, when Magus is applying its effect, it’s an Elk but hasn’t had its ability removed yet.

| Reminder | Layer | Effect |
| -------- | ----- | ------ |
| Copy | 1 |  |
| Control | 2 |  |
| Text | 3 |  |
| Type | 4 | Non-basics become Mountains <br> Magus becomes and Elk |
| Color | 5 | Magus becomes green |
| Ability | 6 | Magus loses abilities |
| PT | 7a |  |
|   | 7b | Magus becomes a 3/3 |
|   | 7c |  |
|   | 7d |  |
|   | 7e |  |
 
### What happens to Tarmogoyf if I use Oko’s +1 on it?

<p float="left">
  <img src="https://img.scryfall.com/cards/large/front/b/6/b6876d9e-0908-43ac-8542-09c7aa02b5ba.jpg?1562931701" width="25%" height="25%">                                                                                                           
  <img src="https://img.scryfall.com/cards/large/front/3/4/3462a3d0-5552-49fa-9eb7-100960c55891.jpg?1574073631" width="25%" height="25%" />
</p>

Answer: It will be a green 3/3 Creature - Elk named “Tarmogoyf” with no abilities.

Explanation: Tarmogoyf has a characteristic defining ability (CDA) which conveys information about its power and toughness. This power and toughness are applied in Layer 7a after Oko would have removed the ability in Layer 6. So, despite Oko’s +1 setting power and toughness in Layer 7b and Tarmogoyf’s CDA applying in Layer 7a before it, Oko’s +1 has removed the CDA in Layer 6.

| Reminder | Layer | Effect |
| -------- | ----- | ------ |
| Copy | 1 |  |
| Control | 2 |  |
| Text | 3 |  |
| Type | 4 | Tarmogoyf becomes an Elk |
| Color | 5 | Tarmogoyf becomes green |
| Ability | 6 | Tarmogoyf loses abilities |
| PT | 7a | Tarmogoyf’s CDA __*would*__ apply but has been removed |
|   | 7b | Tarmogoyf becomes a 3/3 |
|   | 7c |  |
|   | 7d |  |
|   | 7e |  |
 
### What happens to the permanent exiled with Deputy of Detention if I use Oko’s +1 on it before it’s removed from the battlefield?

<p float="left">
  <img src="https://img.scryfall.com/cards/large/front/7/e/7e362055-78a1-48fa-a4ef-6cf7e0b21b14.jpg?1572893724" width="25%" height="25%">                                                                                                       
  <img src="https://img.scryfall.com/cards/large/front/3/4/3462a3d0-5552-49fa-9eb7-100960c55891.jpg?1574073631" width="25%" height="25%" />
</p>

Answer: The permanent will return to the battlefield.

Explanation: This has to do more with Deputy of Detention, but it has come up a few times for me, so it’s worth covering here. When Deputy enters the battlefield, as part of its resolution it exiles a permanent and creates a continuous effect with a defined endpoint, i.e. this permanent is exiled until this object (Deputy) leaves the battlefield. The effect to return the permanent is set up on Deputy’s ETB resolving and exists independently of Deputy having its ability when it leaves the battlefield.
 
### What happens if I +1 on a Spell Queller with an opponent's spell exiled with its ETB ability?

<p float="left">
  <img src="https://img.scryfall.com/cards/large/front/9/b/9b76bcd4-580a-4435-afe9-290940b1837f.jpg?1562744041" width="25%" height="25%">                                                                                                     
  <img src="https://img.scryfall.com/cards/large/front/3/4/3462a3d0-5552-49fa-9eb7-100960c55891.jpg?1574073631" width="25%" height="25%" />
</p>

Answer: The spell is exiled permanently

Explanation: Unlike the previous answer, returning the spell taken with Spell Queller is a Triggered ability, meaning Oko’s +1 ability removes the mechanism by which the spell would be returned to the stack under the control of its owner. 
 
### Does Mox Amber tap for mana if I +1 Oko on their only Legendary permanent??

<p float="left">
  <img src="https://img.scryfall.com/cards/large/front/6/6/66024e69-ad60-4c9a-a0ca-da138d33ad80.jpg?1562736914" width="22%" height="22" />
  <img src="https://img.scryfall.com/cards/large/front/c/2/c2462fdf-a594-47d0-8e10-b55901e350d9.jpg?1572300417" width="22%" height="22%" /> 
  <img src="https://img.scryfall.com/cards/large/front/f/4/f480df6d-e227-4ccb-ad6d-a4ad48a360ad.jpg?1562201599" width="22%" height="22%" />                                                                                                               <img src="https://img.scryfall.com/cards/large/front/3/4/3462a3d0-5552-49fa-9eb7-100960c55891.jpg?1574073631" width="22%" height="22%" />
</p>

Answer: Yes

Oko’s +1 ability simply never changes supertypes of permanents. Therefore, although a 3/3 Elk with no abilities, the permanent is still a green Legendary and therefore Mox Amber adds green mana. This also applies to Snow (Arcum’s Astrolabe) and things that count it like Dead of Winter. It’s also worth adding that because the Legend supertype is retained, and so too is the name of the permanent. If you play another card with the same name as another Legendary permanent, which is an Elk due to Oko, you still need to sacrifice one due to the Legend rule.

### What happens if I +1 Oko on a Mycosynth Lattice?

<p float="left">
  <img src="https://img.scryfall.com/cards/large/front/e/7/e7e7f15a-074a-4137-88ca-e5d376d146fd.jpg?1562640258" width="25%" height="25%">                                                                                                   
  <img src="https://img.scryfall.com/cards/large/front/3/4/3462a3d0-5552-49fa-9eb7-100960c55891.jpg?1574073631" width="25%" height="25%" />
</p>

Answer: Mycosynth Lattice still makes everything an artifact, and all permanent and cards not on the battlefield colorless. 

Explanation: This is a Layers question again. The key thing to remember throughout this is that Lattice has an earlier timestamp than Oko, meaning that if Lattice and Oko’s +1 are impacting things in the same Layer, Lattice will apply first. So, in Layer 4 Lattice makes all permanents into artifacts, then Oko’s +1 makes Lattice into a creature. Then in Layer 5 Lattice makes all permanents and cards not on the battlefield colorless before Oko’s +1 makes Lattice green. In Layer 6 Oko’s +1 removes Lattice’s abilities (abilities already applied aren’t removed/undone). In Layer 7b Oko’s +1 makes the Lattice creature a 3/3. When all is said and done, you’re left with all permanents and cards not on the battlefield being colorless, except the Lattice which is a green 3/3 Elk with no abilities.

| Reminder | Layer | Effect |
| -------- | ----- | ------ |
| Copy | 1 |  |
| Control | 2 |  |
| Text | 3 |  |
| Type | 4 | Permanents become artifacts <br> Lattice becomes an Elk |
| Color | 5 | Permanents and cards become colorless <br> Lattice becomes green |
| Ability | 6 | Lattice loses abilities |
| PT | 7a |  |
|   | 7b | Lattice becomes a 3/3 |
|   | 7c |  |
|   | 7d |  |
|   | 7e |  |
 
## -5: Exchange control of target artifact or creature you control and target creature an opponent controls with power 3 or less.

There’s not a lot of gotcha scenarios that I could find for this ability. If they exist, they’re likely to be absurd corner-case situations, requiring all manner of silly effects you’re unlikely to see in a real game of Modern. However, the release notes give a good reminder of what to consider when exchanging permanents.

* If either of the target permanents is an illegal target when Oko’s last ability resolves, the exchange won’t happen.

* Gaining control of a permanent doesn’t cause you to gain control of any Auras or Equipment attached to it. Gaining control of an Equipment doesn’t cause it to become unattached, although its new controller may activate its equip abilities during their main phase.

That’s all folks! I hope this helped and was entertaining! Magic: the Gathering is complicated and this list should not be taken as exhaustive, definitive or authoritative. Listen to your head Judge as things can and often change.

Happy playing,

Sean Tomlinson
L1 Elk


# Acknowledgements

Many thanks to Charlie Anne Page (L2), John Barkestedt (L2), Chris Ambery (L2), Sam Milner (L1) and Luis Alverez Zucchino for proofreading and providing comments on early drafts of this article.
