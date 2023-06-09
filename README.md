# mecurier's salt and pepper
For Baldur's Gate series games. This mini mod compilation includes severeal tweaks to reflect my personal flavor of gameplay.

Supported games: BG1EE, BG2EE and EET. Some components might work with BG1/BG2 classic but I didn't test any. 

## Installation

Installation is similar to any standard weidu mod. Recommend to install after most rule/class/kit/item-changing mods.

## Compatability

Technically this mod should be compatible with most mods. Nevertheless, some tweaks may be overided by mods installed afterwards.

This mod is designed such that features from the following mods are retained as much as possible. Install them before this mod:
- Tweak Anthology
- Item Revisions 
- Spell Revisions
 
## Contents
### Group 1000: Economy system tweaks
#### Component 101x: Standardize store buy and sell markups
Regular shops buy at 25% value, fences buy at 20% value, no depreciation

OR

All shops buy at 20%, no depreciation

The goal is to save players effort in heading to the best buyer to dump their loot and meanwhile slightly cut player's income as new contents from EE games and mods are already introducing lots of extra loot.

#### Component 102x: Tweak BG1 Officer Vai's bounty
Officer Vai buys only trophies, at 100% value

OR

Officer Vai buys only trophies, at 50% value

OR

Officer Vai buys only trophies, at whatever discont set previously

#### Component 103x: Standardize store selling markups
All shops sell at 150%

OR

All shops sell at *AT LEAST* 150%

#### Component 111x: Tweak random treasures

No random treasures from creatures

OR

No random treasures from areas (WIP, don't install)

OR

No random treasures from creatures and areas (WIP, don't install)

This component alleviates players' pain in looting random gems, golds, etc. and help "keep the floor clean".
Side effects include missed out scrolls and slightly cut income.

#### Component 1120: No wizard scrolls from random treasures

This component has three major impacts:
- You actually need to buy most scrolls in order to learn respective spells, and they are usually not cheap
- Much less "free" XP from forgetting and re-learning spells from extra copies of scrolls
- Access to high level spells are limited by plot progress

### Group 2000: Generic combat system tweaks
#### Component 201x: Alternative proficiency mastery system (install *BEFORE* SCS)
4 stars true grandmastery

OR

4 stars BG2EE style grandmastery

OR

4 stars BG2EE style grandmastery，5th star for true grandmastery exclusive to kensais and archers

Note: 4 star (true) grandmastery is design that the character gains full benefit of the respective grandmastery but with 4 stars at level 9. 

If the 3rd option is installed, kensais and archers will be eligiable to reach true grandmastery at level 12.

This is a mixture of Tweak Anthology's (True) Grandmastery and Scales of Balance's "Weapon Proficiency Overhaul" component. 

| Stars | THAC0  | Damage | Speed factor | APR (option 1) | APR (option 2 & 3) | Required level|
|:------|:-------|:-------|:-------------|:---------------|:-------------------|:--------------|
|1|0|0|0|0|0|1|
|2|1|2|0|0.5|0.5|1|
|3|2|4|-1|1|1|6|
|4|3|5|-3|1.5|1|9|
|5 (option 3 only)|3|5|-3|N/A|1.5|12|

#### Component 202x: 2e and 3.5e hybrid proficiency system (install *BEFORE* SCS)

Can be installed with or Without multiclass grandmastery.

This component makes the following changs:
- 0 star: proficient; 1 star: specialization; ... ; 4 star: grandmastery
- All classes are proficiency with whatever weapons they are allowed to use
- All classes can invest up to 2 stars in any fighting style 
- Fighters can reach BG2EE-style grandmastery (4 stars) at level 9
- Warriors can invest 1 star in two weapon categories or fighting styles at level 1
- Thieves, clerics, shamans, and monks can invest 1 star in one fighting style at level 1
- Mages and sourcerers gain no proficiency stars at all

Fighting styles are redesigned such that each star approximately corresponds to one 3.5e-style feat

*Single weapon style (emulating Improved Critical feat):*
- 1 star: -1 THAC0 bonus
- 2 stars: -1 THAC0 bonus and scoring critical hits when rolling 19 & 20

*Two-handed style (emulating Power Attack feat):*
- 1 star: +2 damage bonus, +1 THAC0 penalty 
- 2 stars: +4 damage bonus, +1 THAC0 penalty

*Sword-and-shield style (emulating Combat Expertise feat):*
- 1 star: -1 AC bonus, +1 THAC0 penalty 
- 2 stars: -2 AC bonus, +1 THAC0 penalty

This style is designed to work with *Items Revisions component: Revised Shield Bonuses*, netting a significant overall AC bonus from shield utilization.

*Two-weapons style (2e and 3.5e hybrid rule):*
- 0 star: +4 THAC0 penalty for main hand, +8 THAC0 penalty and -2 damage penalty for off hand
- 1 star: +2 THAC0 penalty for main hand, +4 THAC0 penalty and -2 damage penalty for off hand
- 2 stars: no THAC0 penalty for main hand, +2 THAC0 penalty and -2 damage penalty for off hand

Note: installing this component will make non-humanoid monsters more challenging in SCS as their effective proficiency level is scaled up by one level.

#### Component 2100: Alternative saving throw tables for smoothier progress and better class distinction

This component is designed to work with *Spell Revisions* to take advantage of its revised saving throw types.

| LEVEL |  1 |  2 |  3 |  4 |  5 |  6 |  7 |  8 |  9 | 10 | 11 | 12 | 13 | 14 | 15 | 16 | 17 | 18 | 19 | 20 |
|:------|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|
| Good  | 13 | 13 | 12 | 12 | 11 | 11 | 10 | 10 |  9 |  9 |  8 |  8 |  7 |  7 |  6 |  6 |  5 |  5 |  4 |  4 |
| Fair  | 15 | 15 | 14 | 14 | 13 | 13 | 12 | 12 | 11 | 11 | 10 | 10 |  9 |  9 |  8 |  8 |  7 |  7 |  6 |  6 |
| Bad   | 17 | 17 | 16 | 16 | 15 | 15 | 14 | 14 | 13 | 13 | 12 | 12 | 11 | 11 | 10 | 10 |  9 |  9 |  8 |  8 |

| Class        | Death | Polymorph | Breath | Spell/Wand |
|:-------------|:------|:----------|:-------|:-----------|
|Warrior       | Good  | Fair      | Fair   | Bad        |
|Cleric/Shaman | Fair  | Fair      | Bad    | Good       |
|Thief         | Fair  | Fair      | Good   | Bad        |
|Mage/Sorceror | Bad   | Fair      | Fair   | Good       |
|Monk          | Good  | Good      | Good   | Good       |

#### Component 2200: Alternative strength modification: bonus starts from 15 STR and smoothier progress

|STR|vanilla THAC0|vanilla damage|vanilla bash|vanilla weight allowance|modded THAC0|modded damage|modded bash|modded weight allowance|
|:--|:------------|:-------------|:-----------|:-----------------------|:-----------|:------------|:----------|:----------------------|
|11|||11|70|||11|80|
|12|||12|90|||13|95|
|13|||13|90|||16|115|
|14|||14|120|||20|140|
|15|||15|120||1|25|170|
|16||1|16|150|1|2|30|210|
|17|1|1|18|170|2|3|35|260|
|18|1|2|20|200|2|4|40|320|
|18/0-50|1|3|25|220|2|5|40|360|
|18/51-100|1|3|30~45|250~400|3|5|45|400|
|19|3|7|50|500|3|6|50|500|
|20|3|8|55|600|4|7|55|600|
|21|4|9|60|700|4|8|60|700|
|22|4|10|65|800|5|9|65|800|
|23|5|11|70|1000|6|10|70|1000|
|24|6|12|75|1200|6|12|75|1200|
|25|7|14|80|1600|7|14|80|1600|

#### Component 2210: Apply 1.5x strength damage bonus for two-handed melee weapons

Note: the exta 0.5x damage will show up in charecter info panel after about 1 second after equiping.

### Group 3000: Item tweaks
#### Component 3010: Option: Specific ranged weaponry tweak

This component tweaks the following items:
- Strong Arm: changed from +2 weapon to non-magical, as the proper damage bonus from strength enabled by component 3040 alone makes it a potent weapon. This also gives you a good reason to use +2/+3 arrows if component 3030 is installed.

#### Component 3020: Option: 3.5e style to-hit and damage for launchers and ammo

with dice size approximation: longbows deal 1d6+1 damage, light crossbows deal 1d8 damage, heavy crossbows deal 1d8+1 damage

OR

without dice size approximation (experimental): longbows and light crossbows deal 1d8 damage, heavy crossbows deal 1d10 damage (the damages are correct in combat but will not show properly in character stats panel)

#### Component 3030: Option: Best instead of stacking enchantment bonuss from launchers and ammo

Bows, corssbows, and slings will be treat as +x weapon when determine what monsters they can hit and have +x THAC0 and damage bonus, where x is the *hightest* enchantment level of the launcher and ammo.

#### Component 3040: Option: Proper damage bonus for bows per strength requirement

Composite bows will have damage bonus equal to that of their strength requirement.

#### Component 3099: Apply options set in components 30xx

Components 30xx will not be effective until this component is installed.

#### Component 3110: Tweak attacks per round for bows

Base 2 APR for all class with 2 THAC0 penalty

OR

Base 2 APR and 2 THAC0 penalty for warrior classes eligible for specialization, 1 APR for other classes

Note: emulating the Rapid Shot feat.

#### Component 3130: Base 1 APR for darts and throwing daggers

Per 3.5e rule.

#### Component 3140: Only damage bonus from strength for slings and throwable weapons

These weapons will use Strength for damage bonus and Dexterity for THAC0 bonus, per 3.5e rule.

#### Component 3150: Two-handed slings

Per 3.5e rule.

#### Component 3160: Make crossbows usable by all classes but single-class druids

Per 3.5e rule.

#### Component 3300: Helms don't grant critical hit protection

Per 3.5e rule.

#### Component 3500: More importable BG1/SOD items available in BG2-SoA (lazy implementation)

Add the following items to Adventure's Mart:
- Kiel's morning star
- Claw of Kazgoroth
- Koveras's ring of protection
- Armor of missle attraction

### Group 4000: Spell tweaks
#### Component 4001： Make Protection from Missiles caster only

Make the *Protection from (Normal) Missiles* spell affect the caster only. Also the duration is set to 5 turns (1 hour), same as other low level protection spells. This component is compatible with SCS despite installation order.

### Group 5000: Class and kit tweaks
#### Component 5010: Archers have equipment restrictions mirroring kensais'

Archers will not be able to use helms, bracers, gauntlets, shields, or any melee weapon except for daggers, effectively making them "ranged kensais".

### Group 6000: Tactical challenges tweaks
#### Component 6200: Make SCS kobolds' poisonous weaponry undroppable (install *AFTER* SCS)

### Group 7000: Misc tweaks
#### Component 7010: NPC Customization (for power gamers only!)

This component allows players to change stats, race, alignment, class, kit, racial enemy of joinable NPCs, so that the game can be played as if using a created party without loss of NPC interaction contents. A new game is required to see the effect.

Refer to `mcr_salt_and_pepper\2da\npc_customization.2da` for details. 

# Credits

This mod referred to design concepts and/or used weidu libraries from the following mods. The author is grateful for their great contributions to the game community!

* [The Tweak Anthology](https://www.gibberlings3.net/files/file/973-the-tweaks-anthology/) by Gibberlings3.net community
* [Sword Coast Stratagems](https://www.gibberlings3.net/files/file/914-sword-coast-stratagems/) by DavidW
* [Scales of Balance](https://github.com/UnearthedArcana/Scales_of_Balance) by subtledoctor
* [Item Revisions](https://www.gibberlings3.net/files/file/969-item-revisions/) by Demivrgvs, Mike1072 and Ardanis
* [Spell Revisions](https://www.gibberlings3.net/files/file/970-spell-revisions/) by Demivrgvs
* [Baldurs-gate-dnd-3.5](https://github.com/Holic75/Baldurs-gate-dnd-3.5) by Holic75
* [Enchant the Missile Launchers](https://forums.beamdog.com/discussion/58374/enchant-the-missile-launchers-ranged-weapon-tweak) by Dee
