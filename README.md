# [MOD] Van Helsing Enhanced: An Overhaul And Bugfix
__Current Version: v9-2__

__Authors: [ILL-](https://steamcommunity.com/profiles/76561197970451100), [WareBare](https://steamcommunity.com/id/warebare), And [A Cat](https://steamcommunity.com/id/felis_noctu)__

---
## DISCLAIMERS

___THIS MOD IS NO LONGER IN ACTIVE DEVELOPMENT BY THE ORIGINAL AUTHORS!___ This repo currently represents our work as of the last time ILL- released an update, and as the base game has updated since then: 
* **The authors keep no responsibility for any loss of data or errors that occur while using this mod. This mod changes several game files which may cause errors I am not aware of. Do not contact Neocore or use the in-game bug reporting feature to report any bugs you have while running this mod. Neocore does not provide support to people who run mods.**

It is **NOT** recommended to run this mod on existing characters, nor is it to remove the mod on a character created within this environment. Doing so is nearly guaranteed to cause data loss. Fresh characters only!

Fix-Only versions have been discontinued, as 1.04 fixes most of the issues with end game gear.

**About Multiplayer:**

Changing the core files of the game changes your version checksum, and two clients with different checksums cannot play together. Basically, you cannot play with anyone who does not have this mod installed. Uninstalling this mod will fix the problem, but there will be problems with gear missing their enchantments, gear missing entirely, other things like that. It will essentially break any gear you've obtained while running the mod.

---
## DESCRIPTION

The Van Helsing series has stolen a place in my heart as one of the most atmospheric and interesting ARPGs I've played. Unfortunately the recent installment is not living up to my expectations, and I wanted to do something about it.

What this mod aims to do is provide a more enjoyable experience with tons of additional content, much needed balance tweaks, overhauls to skills, bugfixes, and clarifying of game mechanics.

What this game does not do is make you overpowered without challenge or give you too much reward for too little risk. This is not a cheat mod, and the balance of this mod is completely different than that of the original game, for the better.

---
## MAJOR FEATURES

### __Monster Scaling:__
The vanilla balance in VHFC is rough around certain levels. The problems stem from being unable to keep up with decent resistances with new, good gear, and the vanilla scaling has some sudden, immense increases in difficulty. The new scaling I created using an exponential algorithm, smoothing out what was once a jagged, sometimes intense curve in monster power to a more subtle and steady increase with some emphasis on monsters gaining power when you do. For example from obtaining and leveling new skills at 20 and 40. Then when you start leveling slower and have enough time between levels to find some good gear to replace the old ones, the scaling rate starts increasing again. No more sudden, massive boosts of power in enemies that you can't keep up with.

Additionally, the less-known modifiers like monster resistance (which actually gives them their resistance/immunity statistics at level 100) now scales slowly, slowly incorporating monster resistances to certain damage types, until monsters start getting their immunities around level 80. Before it was a sudden increase at level 50 and other high levels they would gain huge bonuses, making the change between levels jarring. The other hidden stat which reduces the constructor's minion damage, suddenly starts increasing at level 30. I leveled a constructor to 78 and can say there was a massive increase in difficulty at some places, and this stat is why. Now this stat increases logarithmically to the same point as vanilla at level 100. No more sudden huge decreases in minion damage at levels 30,50, and 70. It's a nice smooth ride.

With this scaling you'll notice a drastic increase to your survivability at lower levels, and less sudden power spikes in monsters. You might find that the casual difficulty is actually casual. At level 100, this mods scaling and vanilla scaling meet, leaving you at the a similar monster difficulty. The monsters are roughly 5% stronger at level 100 with this scaling than in vanilla.

### __Mechanical Clarity:__
Van Helsing has some really confusing damage calculations and mechanics, and some of them don't even do what they say they do. I've cleared up these tooltips, as well as changing the tooltips of things to tell you exactly what they do. For example, bonus % damage values only apply to the weapon damage of a skill, not to any added damage bonuses. This is hardcoded and I cannot change it, but I can make it clear as to exactly what they do, so you know what to expect.

### __Total Rebalance:__
The intent of this rebalance is to change the damage differences between sources: weapon and added damage. Previously they were completely unbalanced after you got greater essences, and from level 50 onward most of your damage would come from added damage and not your weapon. However skills only scaled per level from weapon damage, and there was a hidden enchantment multiplier that handled added damage for different skills. This caused a huge imbalance in skills, and didn't incentivise leveling dps skills unless you wanted their masteries. Additionally stats and other % bonuses only affect weapon damage (this is hardcoded), so stats would have neglible effects on overall skill damage, as would any % damage bonuses on gear.
Additionally this should move the metagame away from being forced to abuse certain mechanics and skills to get to inhuman difficulties. This mod will allow for more diverse builds to succeed, and old builds that abused certain skills will no longer be nearly as effective.

### __Monster Rebalance:__
* Champions and Elites no longer share a loot table, and therefore champion packs no longer drop 3x the loot a single Elite does. Additionally Elites have been overhauled to be slightly harder and provide more loot, and their minions have actually been turned into minions instead of huge HP walls that stand near the Elite.
* All mana drain abilities have been reduced in scaling slightly. Chimera mana drain was significantly reduced. There are now some enemies with ranged, slow projectile mana drain attacks to bring some difficulty to ranged casters, they will only cast at a range so melee heroes will likely not be targeted when in close proximity. Mana draining skills used to only be a problem for melee classes due to the huge mana drain rates and melee classes having a smaller mana pool and lower regen, now mana drain is a threat to all classes, and the instant mana drain on melee classes has been removed.
* Caster-type enemies have had their spellpower reduced, which was their scaling strength on their spells. Some of their spells in combination with their spellpower could do 60x the damage a normal ranged mob could do. Additonally some missile speeds have been lowered to give you the chance to dodge them if you're fast. Enemies that casted only very slow-moving projectiles have not been touched. You can dodge those, I believe in you.
* Ranged monsters with instant-hit abilities (dreadknekts, rokhs) have had their damage reduced. Enemies who have projectiles that you can actually dodge have not been changed.
* Some giant enemies with smash-attacks that deal high aoe damage have had their windup time slightly increased, giving vigilant players time to escape before getting hit.
* Melee normal monsters have had their defense increased by about 40%, making them more than just more cannon fodder.
* Various elites have been tuned to provide more specific challenges associated with their skillset and resistances. For example some caster elites now fire slower-moving projectiles, but faster and spread out in an area.
* A large number of enemies had improper CC resistances, specifically elites. This allowed them to be stunned/instant killed at the rate of a normal mob. This has been fixed. Note that this does not make them invulnerable to CC, just very highly resistant. Bosses are still immune to all CC. CC does not include Slow or Vulnerability.
* Some enemies have been given improved CC resistance, notably some melee mobs and giants.

### __Skills:__
* The skill balance has been completely reworked. All skills now have a base damage multiplier, which applies damage from both weapon and added damage from enchantments. Previously skills had a hidden modifier to their added damage gains, and since most of your damage came from added damage on items and essences after level 50, some skills were left in the dust, and it was difficult to understand which skills had high enchantment bonuses, and which didnt. Skills also now level by increasing their total damage by 15% per level, bringing back incentives to max a skill for damage.
* Some skills have been touched up with modified damage multipliers that are different from their old weapon damage due to the new skill damage calculations. Other skills have been reworked slightly to provide a more obvious niche or role. Many skills have also been given different masteries and rage powerups. Note that a large number of old skill abuses: umbralist instant crit kill, elementalist and protectors' permanent invulnerability, and some overpowered skills being brought into line with the rest will probably require you to rethink your build.
* Katarina's skills have been rebalanced as well. Previously the player bonuses you could get from her were paltry at best, and completely overshadowed by her sheer combat power. Those bonuses are now stronger, and if you don't want to have a companion in battle you can keep her in spirit form and not lose out on her combat power. Her combat skills have been spiced up as well, and specializing her to your needs should be more rewarding.

Overall, all dps skills should be viable for the role they were intended for.

With the skill changes, item added damage enchantments have been significantly reduced to be more in line with their weapon damage counterpart, as such most of your damage will probably now come from your weapon unless you specifically gear for added damage.

### __Items and Loot: Fall in love with loot again__
* The enchantment system has been totally overhauled. There are now 5x the amount of item enchantments in the pool that can roll on items. With these changes come two kinds of enchantments: normal and rare. Rare enchantments come in two varieties: rare enchantments taken from unique items but are far less powerful, and rare versions of normal enchantments that can roll much higher. Rare enchantments appear at a 10% rate of normal enchantments. You can tell if an item has a rare enchantment by its significantly increased value.
* Critical hit chance and damage have also been toned down so it takes some more investment to hit the cap, or go past it. Whereas before they were pretty much the go-to stat for damage increases, now they're toppings on a larger, more diverse, non-vegan, damage increasing stat cake.
* The restrictions on what enchantments can show up on items has also been reduced, so there are more enchantments that can show up on pieces of gear they couldn't before. There are still restrictions: You wont see attack speed on caster weapons since they do nothing. The stats that would be useless for a class or innapropriate on gear still won't appear on those pieces of gear.
* Essences have been changed as well. Greater essences were clearly balanced in the original game to be used at level 100, but the fact that you got them at level 50 caused a huge power spike. Greater essences have now been balanced for use at levels 50-75. Now there are two new tiers of Essences: Major and Ancient. They are not just upgraded versions of the other essences as I wanted to bring more variety to the potential bonuses you could get from essences. There are currently only a few Major and Ancient essences in the game, including Epic ones, and more will be added soon.
* Katarina's set items have been overhauled as well, with each set focused on a specific role. They also have more set bonuses and more set items. Because of the loot changes and a much larger variety of mods available on Katarina's gear (crit, damage%, etc) she can scale very well into the end game instead of fizzling out around level 75.
* I've also gone through and fixed all the discrepancies in set item bonuses where a decimal point was misplaced in the original files, giving things like the manticore set 10-20x the bonuses on some stats.
* Godlike items have also been changed. Godlike items now roll 6 random enchantments instead of their original fixed starting bonuses that weren't always useful, and their upgrades have been changed a bit to be more appropriate for the item type they're on. In addition, they have very high base stats, higher than any other items in that slot, making them the best gear you can wear in that slot. There are currently more Godlike items than in the vanilla game, which only had 6, and only a few could even drop. I will be adding more in future versions. The names of Godlike items have also been changed.
* A bunch of new Epic items are added into the game, mostly at higher levels, some of which are truly unique.

### __Adventure Mode:__
* The bosses in Bounty and Boss Hunt Adventures have been overhauled, becoming much more difficult akin to a boss in story mode, with Bounty bosses being weaker than Boss Hunt bosses. Boss Hunt and Bounty modes should be considered tough challenges on higher difficulties, made to test your strength. The bosses have additional skills and varying specializations that can be deadly. Bounty bosses drop a lot of Gold and Essences, and Boss Hunt Bosses drop a lot more of everything, and have a great chance of dropping the highest tier of items. This feature will be expanded upon soon as well.
* Arena has been completely overhauled to a totally new experience, it is much more difficult and has much higher rewards. View the v9 changelogs to see the full changes.
* Treasure Hunt mode is now just that: a hunt for treasure. The chests drop significantly more loot than a regular chest. Beware, some of them have extra enemies guarding them!

The overall feel and endgame play has shifted: with the changes to loot and skills, the endgame should now be much more rewarding in the way of building strength through gaining items and honing your playstyle, and working your way through the inhuman difficulties. Gear can potentially be very, very powerful with lucky rolls, so you should now be able to slowly gear yourself up to playing on the hardest difficulty without abusing the old skill mechanics.

When you install this mod you may find your damage has gone up or down significantly. Before immediately coming to the forums, try playing for a while, maybe even on a higher or lower difficulty. The game's balance has been changed to the model of working through difficulties and gaining new gear, and your old builds and items will take a minute to catch up.

### __Known Issues:__
There is a known issue where an Epic or Set item that always spawns with an enchantment can get a second enchantment of the same type. For example, if an Epic weapon always rolls a % weapon damage mod, it can roll a second % weapon damage mod on its random enchantments. This can also happen with Set item bonuses and Godlike upgrade bonuses.

There's also an issue with converting old Godlike items to the new ones, any Godlike items that you obtained before this mod can possibly break, either nothing will happen or they will have extra bonuses they shouldn't.

---
## MINOR FEATURES

* Key Chests properly drop what they say they should: An Epic, Set, or Godlike item, depending on the chest. Please note that Godlike and Set items only drop at level 100, even from key chests. Previously Silver and Gold chests only had a small chance to drop their intended item, often requiring 4 or more keys to get a Godlike. With the difficulty of getting fate points in the latest versions, you should be rewarded for opening those chests. Additionally they drop more items, and have a chance to drop more than one of their intended item, if you're really lucky.
* Godlike and Set items now drop properly from champions, bosses, and anything else that can drop an Epic item. Previously they couldn't drop from anything but the Key Chests. Arena chests have an additional chance to drop Set and Godlike gear at higher arena wins. The current droprates for Set items are 1 to every 5 Epics, and Godlike drops are at 1 to every 50 Epics. The Epic droprate is unchanged.
* Katarina's Epic and Set items are now able to drop. Previously they could not, even though she has some cool Epics and Set items.
* Gold and item drops have been increased from in-map chests as well as adventure rewards. I wanted to bring back the "Oh sweet a loot chest" treasure-hunting aspect of the game.
* Added in v2: New monster scaling. A more gentle leveling experience when it matters, and a more difficult experience when you can keep up.

---
## BUGFIXES

* Only working Set items drop. The 30+ Set items without Set Bonuses no longer drop, and until Neocore gives them bonuses or I do you will only get the functional Set items, and there are still plenty to choose from. Each class has at least one class-specific Set, and there are several cross-class Sets.
* The 46 instances of set items having over 100x their intended stats have all been fixed. I'm serious.
* Fixed a ton of inconsistencies in individual item base stats, across all rarities.
* Katarina's Epic and Set items can actually drop, whereas they previously could not. She has a lot of them, too.
* Tons of summoned AI fixes, as well as some changes to Katarina's behavior. They should now be more consistent, and you'll find a lot of them are just better in combat because of it.
* Fixed monsters and monster skills that did far too much damage, didn't do any damage, monsters that didn't attack at all, champions and elites that didn't drop loot, etc.
* And a ton more not mentioned here. Most of them relate to content and balance issues, as I cannot fix technical problems in most cases.

---
## PLANNED FEATURES

v9 has covered pretty much all of what I intend to do with this mod and now mostly requires polish. I will be enhancing the current features and fixing bugs and balancing the game as time goes on. I will also be adding in new items and enchantments, and continuing to polish up the balance and skills in the game.

---
## DOWNLOAD AND INSTALLATION

You can download any version of this mod from my Google Dropbox here: [Download Here](https://github.com/FelesNoctis/VHFC-Enhanced/blob/main/Van%20Helsing%20Enhanced%20v9-2.zip)

__v9-2:__ This version is the full mod experience, with all features discussed above included. You cannot pick which parts of the mod you want as of v4 and later, due to the number of changes that change the same files.

To install, extract the zip file to `\steamapps\common\The Incredible Adventures of Van Helsing Final Cut`

To uninstall, delete your _cfg_ and _strings_ folders in your installation directory, and steam should automatically redownload the original files for you. If steam does not, check the integrity of your game cache in the steam window. You can also backup your cfg folder to later replace the mod files with the original (this is the safest option).

___Whenever Neocore applies a patch through steam, it will overwrite the mod files and you will have to re-download the mod! If you run the unmodded game after running v4 or later you will lose most of your items permanently. Make sure if steam downloads something, it's not an update to VHFC, and if it is, redownload and install the mod again to prevent things from disappearing.___

If there are any issues related to the changes the mod makes, or any discussion related to the mod feel free to post in this thread.

___Huge thanks to WareBare for reworking the skill damage calculations and balancing half of the classes.___

___The changelog is now in the first post in the Steam thread.___

---
## LIST OF SPECIFIC MECHANICS

There are some added mechanics that use Keywords to describe what they do. More will be added in the future.

__On Hit Effect:__

On Hit Effects are special effects that can be triggered by dealing damage to enemies. As of v7 any skill that deals damage can trigger On Hit Effects, except minion and summoning skills. Katarina can also use On Hit Effects with her basic attack.

_List of On Hit Effects:_
- Sunder- Deals physical damage equal to 35% of your weapon damage and 17.5% of your added damage, and each subsequent hit of sunder has a higher crit chance and crit damage. Chance to activate
- Shred Resistance- Permanently reduces enemy resistances by 10%. Chance to activate.
- First Strike- Deals 100% base damage on the first hit against every monster. This is an additional damage source and will show up as an additional damage number.
- Spot Weakness- Applies a 50% vulnerability to the enemy for 3 seconds. Chance to activate
- Spirit Arc- When Procced, deals damage similar to Katarina's spirit arc skill. This damage scales to 100% of your (blue) stat.
- Chance to stun/freeze/slow- Does exactly what you think.
- Enchanted Strike- Deals bonus arcane damage equal to 250% of your added elemental damage bonuses. Chance to proc.
- Ignite- Sets your target aflame, dealing 50% of your weapon damage and 150% of your added elemental damage over 4 seconds. Chance to proc.
- Envenom- Poisons your target, dealing 60% of your weapon damage and 175% of your added elemental damage over 6 seconds. Chance to proc.
- Arcane Explosion- Deals arcane damage in a 4m radius equal to 150% of your added elemental damage. Chance to proc.

Enhanced versions of On Hit effects have 3x the strength of their normal variants, and Super versions have 5x the strength.

On Hit effects can only proc once per second on the same target if it's an AoE effect, and 2 times per second for single target effects.
