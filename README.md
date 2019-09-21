# mecurier's salt and pepper
for Baldur's Gate series games

Supported games: BG2 and all EE games (not tested on BG1)

This mini mod compilation includes severeal tweaks to reflect my personal flavor of gameplay.

## Installation

Installation is similar to any standard weidu mod. Recommend to install after most item-changing and rule-changing mods 
(e.g. Item revisions, SCS, etc.)

## Compatability

Technically this mod should be compatible with most mods. Nevertheless, some tweaks may be overided by mods installed afterwards.

## Contents

### 10 Standardize store buy and sell markups

This component standardize sell and buy markups in all stores: sell at 150% and buy at 25%. Specially, fences buy at 15%. 
The goal is to save players effort in heading to the best buyer to dump their loot and meanwhile slightly cut player's
income as new contents from EE games and mods are already introducing lots of extra loot.

### 20 Remove random treasure

This component alleviate players' pain in looting random gems, golds, etc. from monsters to help them "keep the floor clean".
Side effects include missed out scrolls and slightly cut income.

### 30 Standardize to hit and damage bonus from enchantment on launchers and ammo

This component aim to help players who believe the games is inconsistent about to hit and damage bonus in launchers and ammo.
It will remove to hit and damage bonus from all ammo, and grant to hit and damage bonus to all launchers per their 
enchantment level. In addition, heavy crossbows get extra +2 damage bonus, long bows get extra +1 to hit bonus, composite bows 
get due damage bonuses matching their minimum strength requirement. Magical items with unique names keep their special bonuses 
per Item Revisions Revised (https://github.com/BartyMae/IR_Revised), with a few adjustments:

* Drowcraft Light Crossbow of Speed +1 is changed to +3 enchantment to keep it in line with other drow weaponry.
* Strong Arm +2 (composite long bow) is changed to +0 enchantment (non-magical) to balance its exceptional damage bonus.

This component does not update item descriptions to reflect stats change due to the complexity of the problem 
(mutiple languages, different descriptions in vannila and modded games, etc.). If someone knows an elegant solution please 
kindly let me know. Thanks!

### 40 Alternative weapon profiency and mastery system

A mixture of Tweak Anthology's True Grand Mastery and loosened version of Scales of Balance's "Weapon Proficiency Overhaul" component. 

Weapon mastery are streamlined to 4 levels with smoothed bonus:

| Mastery | THAC0  | Damage | Speed factor | APR |
|:--------|:-------|:-------|:-------------|:----|
|*|0|0|0|0|
|**|1|2|0|0.5|
|***|2|4|-1|1|
|****|3|5|-3|1.5|

* Single and multiclass fighters can invest up to 2 pips per weapon at level 1, 3 pips at level 6, and 4 pips at level 9; In addition, they start with 7 pips to distribute at level 1 
* Classes and kits can invest 4 pips in certain weapons can now invest 3 pips (Dwarven Defender etc.)

# Mods recommended to be used together

* SCS
* Tweak Anthology
* Scales of Balance
* Item Revisions Revised
* Spell Revisions Revised
* 3.5e Weapon Style Rebalance http://www.shsforums.net/files/file/1205-35-edition-weapon-style-rebalance/
* Enchant the Missile Launchers: A Small Ranged Weapon Tweak https://forums.beamdog.com/discussion/58374/enchant-the-missile-launchers-ranged-weapon-tweak
companion

# Credits

This mod uses concepts and code snippets from the following mods. The author is grateful for their great contributions to the game community!

* Tweak Anthology by Gibberlings3.net community
* Scales of Balance by subtledoctor
* Item Revisions Revised by Demivrgvs et al., revised by Bartimaeus
* Spell Revisions Revised by Demivrgvs et al., revised by Bartimaeus
