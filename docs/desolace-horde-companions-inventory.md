# Desolace (Horde) companions inventory (game data, accept-zone key 1443)

Source: local Forever game data (questie-forever NPC/object/item dumps), same build as `docs/desolace-horde-census.md`. Band 31-45, Horde core contract 25 (`desolace-horde` in `docs/quest-contracts.json`). Faction key: 8589934770 = Horde, 4294967373 = Alliance, AH = neutral vendor flag, null = neutral.

## RARES - 6 flagged, all 6 shipped (5 same-as-Alliance + the Cursed Centaur band delta)

| NPC | Lvl | Point(s) | Sole-drop signature | Guide step |
|-----|-----|----------|---------------------|------------|
| 14229 Accursed Slitherblade | 35 | 1 pt (42.17,19.01) | 284713 Accursed Legguards | single + collect |
| 14228 Giggler | 34 | 1 pt (61.29,28.91) | 284712 Hyena Hide Helm | single + collect |
| 14225 Prince Kellen | 33 | 1 pt (78.93,21.25) | 284717 Royal Satyr Slicer | single + collect |
| 14227 Hissperak | 37 | 1 pt (52.86,50.08) | none (generics only) | single + kill note |
| 14226 Kaskk | 40 | 1 pt (51.15,86.13) | 284708 Demonstrike Emblem | single + collect |
| 11688 Cursed Centaur | 43 | 1 pt (30.36,60.18) | none (505 loot items, every one shared) | single + kill note |

Notes:
- All six are faction null (neutral spawns, engageable by Horde). No rare is friendly to Horde or unkillable - no Falthis exclusion applies.
- No core-contract overlap (checked exactly over the 25-contract quest records: no shipped rare is a giver, ender, objective, or kill target, and no shipped rare drops a core quest item). The 12031 hit against Kaskk/11688 drop lists is an ID collision: item 12031 (Lodestone Necklace) is a generic world-drop green with 400+ droppers, not NPC 12031 (MaiLahii) - no overlap.
- 11688 ships as a kill-note rare (Fingat pattern): level 43 sits IN the Horde 31-45 band, generic loot only, no quest link of any kind. DELTA vs the Alliance inventory, which excluded it as above-band with no sole - the band half of that exclusion does not transfer; flagged in `docs/companion-unverified.md`, not silently harmonized.
- Hissperak ships as a kill-note rare (same pattern as the Alliance round).
- Tameability: no tame lines ship. The core guide carries zero `only Hunter` lines, so the corroboration half is unmet for everything. Logged in `docs/companion-unverified.md`.
- Respawn timers: unconfirmed anywhere in the data; none stated.

## ITEM-START HUNT - 1480 only

- The Horde core item-start scan found exactly one Horde item-start: 1480 (Flayed Demon Skins 20310 + 6766, dual variants) off the Burning Blade family in the north-center camp (52-57, 21-33): Augur 4663 (5%/2%, 20 pts), Reaver 4664 (12 pts), Adept 4665 (14 pts), Felsworn 4666 (14 pts), Shadowmage 4667 (2 pts), Seer 13019 (1 pt) - all 1443-only; Summoner 4668 / Invoker 4705 also spawn 1412 (said so, not used). The rares guide carries the hunt: kill + optional collect of either skin + a note pointing at the core guides 1480 line - NO accept/turnin lines (companions never carry quest lines).
- The cores other special shapes are core content, not hunts: the 93045 Maraudon expedition and the 1367/1368 clan chains route in `desolace-horde.guide` - the inventory says so rather than duplicating them.

## TREASURES

- Generic "Solid Chest": object 2855 (10 fixed pts: 52.42,28.53 / 54.35,28.12 / 54.82,26.09 / 55.14,30.00 / 73.47,41.59 / 74.57,47.14 / 74.62,49.11 / 74.82,19.33 / 77.19,17.89 / 78.88,23.34) and 2857 (15 fixed pts: 29.30,60.58 / 29.57,58.02 / 30.53,54.82 / 32.63,61.12 / 32.74,55.11 / 32.75,59.55 / 34.23,52.90 / 35.16,61.44 / 35.75,92.10 / 39.82,94.24 / 40.58,94.62 / 65.94,80.75 / 71.45,71.67 / 71.94,78.63 / 73.89,73.72). Points verified identical to the Alliance inventory. ONE loop step over all 25 fixed points, said plainly as generic chests. No contract quest takes either.
- Generic "Battered Chest": object 106318 (6 fixed pts: 81.00,48.40 / 82.40,53.80 / 84.50,72.10 / 84.80,73.00 / 86.30,78.20 / 86.60,78.30). Points verified identical. ONE loop step, said plainly.
- Footlockers (DELTA - absent from the Alliance inventory; present in this build with fixed points and generic loot, shipped): Waterlogged Footlocker 179491 (7 pts: 31.65,22.52 / 34.05,20.70 / 35.44,20.78 / 36.56,22.11 / 37.18,21.96 / 37.47,21.30 / 37.63,22.90) + Mossy Footlocker 179493 (3 pts: 34.36,16.95 / 34.71,12.61 / 35.54,13.95). Contents are generic greens/food/potions (Jade, Moonberry Juice, healing potions), no quest refs. ONE loop step over all 10 points.
- Unique objects (DELTA - absent from the Alliance inventory; each the SOLE source of its item, Horde-openable, shipped with own steps/notes): Blooming Satyrweed 404402 (3 pts: 74.40,19.00 / 75.90,16.60 / 75.90,21.10 - yields 213120 Rune of the Dreamer); Libram of Deliverance 423695 (1 pt: 66.50,7.40 - yields 213513); Utheks Staff 587338 (1 pt: 42.20,82.10 - yields 256058). All faction null.
- Excluded with reason: Karnitols Chest 35251 + Malem Chest 50961 (furniture for Alliance-only quests 1454/1455 + 1437/1465, set aside for the record and unroutable for Horde); Lost Shipping Crate 656789 (furniture for the Alliance crate twin 94841); Tear of Theradras 22246 (writ-94308 object for an out-of-contract writ - quest-adjacent, no generic loot); Sack of Meat 22245 (set dressing); Shellfish Traps 176582/176592/176635 (functional fishing furniture, not the container class - 9 of 10 yields are incidental multi-source greens; the Big Iron Fishing Pole sole-trap-source reads as a data artifact, logged in companion-unverified.md); Brightly Colored Eggs (seasonal Noblegarden); Giant Softshell Clam 177784 + Demon Portals + the 658115 crate (core-contracted content for 6142 / 5581 / 94895 - the core guides own them); Rackmores Chest 177786 + Log 177787 (furniture for 6161, main-contracted shared - core content per the Dun Morogh precedent); Resonite Cask 178145 (no loot); mines and herb nodes (gathering, not treasure); forges, anvils, braziers, campfires, bells, mailboxes, portals (set dressing / no quest / no loot).

## RECIPES - 38 shipped (32 vendor + 6 drop)

Profession inference is by item-name class (Recipe by content, Schematic = Engineering, Pattern = Tailoring/Leatherworking by content, Formula = Enchanting, Plans = Blacksmithing) - the data carries no profession field; each inference is stated below. Every buy is npc-pinned to the exact in-zone vendor.

Vendor-sold:
- Cooking, Super-Seller 680 (AH neutral, 40.48,79.27): 3734 Recipe: Big Bear Steak, 4609 Recipe: Barbecued Buzzard Wing, 12227 Recipe: Lean Wolf Steak (SOLE vendor), 12229 Recipe: Hot Wolf Ribs, 12239 Recipe: Dragonbreath Chili, 12233 Recipe: Mystery Stew (Horde pin - the Alliance-only Janet Hommers also sells it, Horde buys from 680).
- Cooking, Vendor-Tron 1000 (AH neutral, 60.33,38.12): 3735 Recipe: Hot Lion Chops, 5489 Recipe: Lean Venison, 12228 Recipe: Roast Raptor, 12231 Recipe: Jungle Stew.
- Cooking + Tailoring, Kireena (Horde, Trade Goods, 50.98,53.55): 12232 Recipe: Carrion Surprise, 12240 Recipe: Heavy Kodo Stew, 7114 Pattern: Azure Silk Gloves (Tailoring by silk; the only other vendor is out-of-zone).
- Fishing, Wulan (Horde, Cooking Supplies, 26.17,69.65): 6369 Recipe: Rockscale Cod, 17062 Recipe: Mithril Head Trout, 21099 Recipe: Smoked Sagefish, 21219 Recipe: Sagefish Delight.
- Blacksmithing, Muuran (Horde, Superior Macecrafter, 55.59,56.50): 10858 Plans: Solid Iron Maul.
- Enchanting, Gorhak (Magram quartermaster, neutral, 66.25,79.42): 249486 Formula: Enchant Bracer - Lesser Agility (SOLE vendor); 249489 Formula: Enchant Bracer - Lesser Healing Power (also Molkar, Gelkis quartermaster, neutral, 35.68,92.23).
- Alchemy, Gorhak: 250979 Recipe: Greater Spellblasting Potion, 250985 Recipe: Greater Frenzy Potion (both SOLE vendor) - DELTA, see below.
- Blacksmithing, Gorhak: 251390 Plans: Hard Gold Gauntlet, 251458 Plans: Iron Morningstar (both SOLE vendor) - DELTA.
- Leatherworking, Gorhak: 252833 Pattern: Mystic Thick Armor Kit (armor kit), 274491 Pattern: Centaur Hoofwarmers (hoofwarmers) (both SOLE vendor) - 252833 DELTA.
- Tailoring, Gorhak: 253974 Pattern: Silk Reagent Bag (silk bag), 254682 Pattern: Stormcloth Gloves (cloth) (both SOLE vendor) - DELTA.
- Engineering, Gorhak: 269901 Schematic: Centaur Banner Deployment Device, 269903 Schematic: Hoof-Shaped Foot Pedal (both SOLE vendor) - 269901 DELTA.

Mob drops, every dropper spawning only in Desolace (Elwynn rule satisfied by construction; all droppers in-band):
- 211247 Pattern: Phoenix Bindings <- 4663 Burning Blade Augur (20 pts, north-center camp; Tailoring gate per the cloth-wrist open inference, flagged below).
- 249488 Formula: Enchant Bracer - Agility <- 4681 Mage Hunter (38, 8 pts, Mannoroc side).
- 250363 Recipe: Potion of Predatory Senses (Alchemy) <- 4684 Nether Sorceress (39, 5 pts, west).
- 250370 Recipe: Elixir of Fortitude (Alchemy) <- 4632 Kolkar Centaur (30, 7 pts, Kolkar camp) - DELTA.
- 251387 Plans: Hard Gold Bracers (Blacksmithing) <- 4711 Slitherblade Naga (32, 16 pts, coast; a 6143 core-target family - farmed on the cores coast leg anyway) - DELTA.
- 254016 Pattern: Earthen Silk Hood (Tailoring, silk) <- 4719 Slitherblade Sea Witch (35, 14 pts, coast) - DELTA.

Excluded with reason: 249512 Formula: Dreambough Wand (1-dropper/3-zones Badlands-family mob, incidental Desolace point - same exclusion as Alliance); all other Desolace-dropping recipes are generic multi-zone world drops (verified by the narrow scan above - only these 6 have in-zone-exclusive sources); quest-reward recipes (quest records carry no reward data - none shipped); trainer-taught staples (Polestars own profession guides).
Professions with NO in-zone Horde source (stated plainly in the guide, not padded): First Aid only. Genuine faction differences (stated, not harmonized): Fishing and Blacksmithing HAVE Horde sources here (Wulans four; Muurans one plus Gorhaks two) while the Alliance inventory lists neither - all Horde-only vendors; the six Horde-vendor recipes they excluded (6369/17062/21099/21219/7114/10858) are this guides vendors.
Open inferences (Butlers calls): 211247s Tailoring gate (cloth-wrist reading of "Bindings" - the data carries no profession field; if Leatherworking, the steps gate is wrong but the collect, dropper, and points are unaffected); profession-by-name-class for the 8 new Gorhak + 3 new drop recipes (each stated above).

## TAMEABLES - none ship

No data flag for tameability anywhere; the core guide carries zero `only Hunter` lines so corroboration is unmet for everything (same as the Alliance round). Logged in `docs/companion-unverified.md`.

## Alliance-inventory deltas (flagged, not silently harmonized)

1. 11688 Cursed Centaur ships here (in-band at 43) vs excluded there (above-band) - genuine band difference.
2. Footlockers (10 fixed pts) + 3 unique sole-source objects shipped - absent from their inventory (build drift or scan miss; present in this build, verified above).
3. 8 extra Gorhak recipes + 3 extra narrow drops shipped - same note.
4. 12233s in-zone neutral pin is Super-Seller 680 in this build (their inventory cited Tron; the vendor list reads [4897, 8150, 12246] now) - Horde buys from 680.
5. Shellfish-trap pole quirk + tame absence logged in companion-unverified.md (their round logged tame the same way).

