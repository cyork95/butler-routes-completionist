# Alterac (Horde) companions inventory (game data, key 1416 only)

Source: local Forever game data (questie-forever NPC/object/item dumps), same build as `docs/alterac-horde-census.md`. Band 20-45, Horde core contract 50 (`alterac-horde` in `docs/quest-contracts.json`). Faction key: 8589934770 = Horde, 4294967373 = Alliance, AH = neutral vendor flag, null = neutral. Scope: spawns on the Alterac Mountains key (1416) only - Alterac Valley is the separate key 1459, which holds ZERO rare-flagged spawns in this data; battleground content is out of the packs scope regardless, so there is nothing to enumerate.

## RARES - 8 flagged, all 8 shipped

| NPC | Lvl | Point(s) | Sole-drop signature | Guide step |
|-----|-----|----------|---------------------|------------|
| 2258 Stone Fury | 37 | 1 pt (64.68,44.77) | 283254 Heart of Alterac | single + collect |
| 2447 Narillasanz | 44 | 1 pt (73.71,65.35) | 282778 Mark of the Red Flight | single + collect |
| 2452 Skhowl | 36 | 1 pt (31.43,51.51) | 3011 Feathered Headdress (75%) + 6331 Howling Blade (25%) | single + 2 collects |
| 2453 LoGrosh | 39 | 2 pts (47.52,32.31), (52.09,46.94) | 1678 Black Ogre Kickers + 4810 Boulder Pads + 6327 The Pacifier | loop + 3 collects |
| 14221 Gravis Slipknot | 36 | 1 pt (58.20,41.91) | 283255 Syndicate Executioners Slicer | single + collect |
| 14222 Araga | 35 | 1 pt (30.20,72.11); also spawns 1424 (not used) | 283253 Denmothers Hide | single + collect |
| 14223 Cranky Benj | 32 | 1 pt (37.29,19.83) | none (277 shared droppers, every one shared) | single + kill note |
| 14281 Jimmy the Bleeder | 23 | 1 pt (58.58,69.30); also spawns 1424, covered by hillsbrad-horde-rares at its 1424 point | 282713 Bloodstained Pants | single + collect |

Notes:
- All eight are faction null (neutral spawns, engageable by Horde). No rare is friendly to Horde or unkillable - no Falthis exclusion applies.
- No core-contract overlap: no shipped rare is a giver, ender, objective, or kill target of any of the 50-contract quest records (checked exactly - zero mentions). Loot overlap: Benj (14223) drops Turtle Meat 3712, the core 7321s objective - his step carries an honest note that the meat feeds the cores bisque loop (same kills the core already routes); he is not a quest subject (Snapjaws share the drop), so the Dun Morogh exclusion does not fire. Araga drops Tin Ore 2771 and Benj drops an Insignia Cloak 4722 - both ID collisions with NPC ids (2771 Drum Fel, 4722 Rau Cliffrunner); both items are generic multi-source world loot, not quest items. 6331s quest hits (95983/96103) are substring noise from NPC 263316 - verified, no real reference. No other sole item is referenced by any quest record.
- Tameability: no tame lines ship. No shipped rare carries drop evidence of a tameable beast family (meat/fang-type drops name no pet family and Benjs turtle meat has no core corroboration), npc records carry no tame flag, and the core guide carries zero `only Hunter` lines and no references to any shipped rare. Drop evidence alone is not the bar (Stonetalon/Teldrassil precedent needs core-guide corroboration too). Logged in `docs/companion-unverified.md`.
- Respawn timers: unconfirmed anywhere in the data; none stated.

## ITEM-START HUNTS - none

- The Horde cores explicit start-item scan found ZERO item-started Horde records (verified again here: no `start.item` on any of the 50 contract quests, and none on any Horde-mask 1416 record pool-wide). There are therefore no item-start hunts in this round - stated plainly with the scan behind it, rather than padding the rares guide. 7321 (Soothing Turtle Bisque) is an NPC-accept quest, not an item-start; no recipe item for it exists in the data.

## TREASURES

- Generic Solid Chest: object 2855 (8 fixed pts: 38.54,46.96 / 39.89,52.96 / 41.45,40.06 / 42.51,47.95 / 61.06,44.07 / 61.23,43.01 / 63.38,44.17 / 63.54,45.30) and 2857 (9 fixed pts: 35.29,53.40 / 35.82,55.85 / 36.12,55.03 / 37.50,15.09 / 38.86,14.80 / 39.64,15.25 / 40.29,20.60 / 53.67,20.99 / 56.40,26.93). Out-of-zone quests reference some generics (Horde 96102 on 2855, shared 95753 on 2857) - none is Alterac-contract content, same ruling as the Alliance round.
- Hidden Strongbox 2039 (16 fixed pts: 10.67,77.53 / 11.48,75.13 / 12.80,76.49 / 15.42,76.40 / 18.39,76.95 / 18.56,74.51 / 18.75,54.87 / 19.51,75.52 / 20.70,60.26 / 20.94,63.32 / 20.97,56.52 / 21.17,53.74 / 21.33,64.35 / 21.60,57.65 / 21.79,60.75 / 22.63,60.49).
- Battered Chest 2849 (1 pt: 4.90,59.50). Camp Crate 181302 (2 pts: 52.30,96.90 / 52.30,97.30; no recorded loot either way - same treatment as the Alliance round).
- Barrels and crates, generic food/drink/loot, openable by anyone: Barrel of Melon Juice 3659 + Food Crate 3695 (15 shared pts: 11.53,79.08 / 14.22,78.19 / 18.00,82.78 / 18.66,82.44 / 18.95,74.70 / 19.30,85.72 / 20.21,70.87 / 20.38,85.96 / 20.70,53.35 / 21.25,63.69 / 22.67,60.26 / 40.04,79.75 / 47.75,82.83 / 58.17,68.33 / 62.42,58.39); Barrel of Sweet Nectar 3706 + Food Crate 3707 (16 shared pts: 36.99,15.37 / 38.20,49.52 / 38.64,58.24 / 38.96,39.09 / 39.06,15.75 / 39.22,44.03 / 41.28,45.61 / 46.69,46.30 / 47.91,16.97 / 48.55,34.54 / 48.66,44.35 / 49.04,56.57 / 49.66,56.59 / 57.35,45.65 / 62.69,41.43 / 63.26,42.88). Out-of-zone and Durotar-contract quests reference some generics as objectives - none is Alterac-contract content, same ruling as above.
- Alterac Granite 2714 (6 fixed pts: 39.10,96.50 / 39.20,90.90 / 39.60,93.40 / 40.00,94.80 / 41.50,87.70 / 41.50,91.30; also spawns 1424 - the 1416 points are used). Yields are generic multi-source greens and gems; quest refs (2933 uncontracted Hinterlands, 87491 Alliance Wetlands) are adjacency, not ownership - same generic-container ruling as the barrels.
- Unique objects (each the SOLE source of its item, Horde-openable, shipped with own steps/notes): Spring Well 107045 (1 pt: 60.90,82.70 - yields 7771 Filled Red Waterskin); Frozen Remains 423841 (1 pt: 39.70,60.80 - yields 213452 Dormant Holy Rune; which class can use the rune is not in the data).
- Excluded with reason: Alliance Chest 3715 + Alliance Strongbox 105570 + Alliance Chest 105579 (Alliance-only objects); Weathered Bookcase 1760 (furniture for 540, Alliance-only Hillsbrad-contracted); Worn Wooden Chest 1765 (its ONLY yield is the Ensorcelled Parchment, quest item for 551 Alliance-uncontracted + Durotar-contracted 5648/5649/5654/5660 - quest-owned singleton); Dusty Rug 1728 (furniture for 524, Horde-core-contracted - the core owns it); Syndicate Documents 1738/1739/1740/556628 (furniture for 510/511, main-contracted - the main guide owns them); WANTED board 1763 (furniture for 549/566, Horde-core-contracted); Dangerous! board 2008 (furniture for 567, Horde-core-contracted); Bathrahs Cauldron 89931 (furniture for 1714, uncontracted shared - quest-owned, promote if a round contracts it); Manual 423896 (furniture for 79948, city-contracted); Fragrant Cauldron 181073 (furniture for 9029, uncontracted shared); Brightly Colored Eggs + Holiday Snow + Apple Bob (seasonal); fishing schools + Floating Wreckage (fishing nodes, not fixed containers); herbs and veins (gathering, not treasure); fires, campfires, bells, braziers, signposts, spell-effect props (set dressing / no quest / no loot).

## RECIPES - 20 vendor + 4 drops

Profession inference is by item-name class (Recipe by content, Schematic = Engineering, Pattern = Tailoring/Leatherworking by content, Formula = Enchanting, Plans = Blacksmithing, Manual poultice = First Aid) - the data carries no profession field; each inference is stated below. Every buy is npc-pinned to the exact in-zone vendor. No-source professions: Fishing only (same finding as the Alliance round, by a different route - see below).

Vendor-sold (faction checked vendor by vendor; every listed vendor is Horde-buyable):
- Tailoring + Enchanting + Leatherworking + Engineering + Alchemy, Zixil, Merchant Supreme (AH neutral, 53.60,98.70): 5772 Pattern: Red Woolen Bag (Tailoring), 6377 Formula: Enchant Boots - Minor Agility (Enchanting), 7362 Pattern: Earthen Leather Shoulders (Leatherworking, leather basis; SOLE vendor anywhere), 7561 Schematic: Goblin Jumper Cables (Engineering), 210709 Recipe: Elixir of Coalesced Regret (Alchemy, elixir-content basis).
- Tailoring + Alchemy, Christoph Jeffcoat (Horde, 61.10,80.70): 5788 Pattern: Thick Murloc Armor (Tailoring), 6054 Recipe: Shadow Protection Potion (Alchemy, potion basis).
- Tailoring, Mallen Swain (Horde, 60.60,82.90): 6274 Pattern: Blue Overalls, 6401 Pattern: Dark Silk Shirt, 253665 Pattern: Linen Reagent Bag + 253668 Pattern: Woolen Reagent Bag (reagent-bag basis; the Alliance-only Dominique Stefano also stocks both - Horde buys from Mallen).
- Cooking, Derak Nightfall (Horde, 62.00,81.10): 6330 Recipe: Bristle Whisker Catfish, 21099 Recipe: Smoked Sagefish + 21219 Recipe: Sagefish Delight (the Alliance-only Derek Odds also sells both, Paige neutrally too - Horde buys from Derak).
- Tailoring, Norvin Alderman (neutral, Cloaks, 16.02,65.54): 7087 Pattern: Crimson Silk Cloak + 7089 Pattern: Azure Silk Cloak.
- Engineering, Rizz Loosebolt (AH neutral, Engineering Supplies, 47.30,35.16): 13308 Schematic: Ice Deflector.
- Alchemy, Brokin (AH neutral, Alchemy Supplies, 38.24,38.87): 14634 Recipe: Frost Oil (SOLE vendor anywhere).
- Engineering, Zan Shivsproket (AH neutral, Specialty Engineer, 85.95,79.96): 7742 Schematic: Gnomish Cloaking Device (SOLE vendor anywhere).
- Cooking, Smudge Thunderwood (AH neutral, Poison Vendor, 86.12,79.58): 18160 Recipe: Thistle Tea (drink basis; SOLE vendor anywhere).

Mob drops, single in-zone family (+ adjacent-zone members, the established genuinely-Alterac bar; all droppers in-band):
- 251391 Plans: Hard Gold Pauldrons (Blacksmithing) <- 2252 Crushridge Ogre (34, 24 pts central; also spawns 1424 - the 1416 points are used).
- 255727 Manual: Superior Poultice (First Aid, poultice = bandage-adjacent basis, logged here) <- 2243 Syndicate Sentry (36, 24 pts north; also spawns 1422 Hillsbrad - the 1416 points are used).
- 284870 Schematic: Unsanctified Grenade (Engineering, grenade basis) <- 2287 Crushridge Warmonger (39, 20 pts west; also spawns 1424).
- 9296 Recipe: Gift of Arthas (Alchemy, elixir-content basis) <- 1783 Skeletal Flayer (50, 1 pt 85.80,29.50 east; + off-zone Ghoul) - out-of-band, ships with an honest come-back-later note (Safety Sheep precedent).

Excluded with reason: the 8 Archmage Alvareaux recipes (276984/276985 Blacksmithing + 276986-276991 Tailoring) - in-zone vendor is Alliance-only (fac A), unbuyable for Horde (genuine faction difference, stated not harmonized); 249512-style check N/A - every other Alterac-dropping recipe drops in 3+ map zones (verified by the two-zone scan above: only these 4 are within the bar; all else is generic multi-zone world drops, Elwynn rule); quest-reward recipes (quest records carry no reward data - none shipped); trainer-taught staples (Polestars own profession guides cover those).

## TAMEABLES - none ship

No data flag for tameability anywhere; the core guide carries zero `only Hunter` lines and no references to any shipped rare (Benjs turtle-meat drop is ingredient evidence, not pet-family evidence, and lacks core corroboration). Logged in `docs/companion-unverified.md`.

## Alliance-inventory deltas (flagged, not silently harmonized)

1. Loot drift: 7 of 8 rares now carry sole drops in this build (the Alliance inventory recorded none) - shipped as signature collects; Cranky Benj stays a kill note (no sole). Ogre point drift: 2252 shows 24 placed 1416 points here vs 47 central points there.
2. Narillasanz ships here (44, in-band) vs excluded there (above-band) - genuine band difference.
3. Worn Wooden Chest excluded here (quest-owned singleton: parchment for 551 + Durotar contracts) vs shipped there (generic) - genuine data-rule difference.
4. Jimmy same treatment both sides (1416 point here, 1424 point in hillsbrad-horde-rares, sole-drop pants in both).
5. Benj overlap noted here (Turtle Meat feeds 7321) - the Alliance round predates the current drop table.

