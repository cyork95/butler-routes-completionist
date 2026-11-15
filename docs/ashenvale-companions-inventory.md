# Ashenvale companions inventory (pack 0.33.0)

Every entry shipped in the two Ashenvale companion guides, one line each:
name, NPC/item id, source type, coordinates or vendor, and the data source
verified against. All coordinates are the client's own (live) map frame on map
1440 (Ashenvale). Game data is questie-forever npcs.json, items.json and
objects.json; quest linkage checked against the full quest table and the
55-quest core contract (`ashenvale.guide`). The data carries an explicit `rare`
role flag; 13 Ashenvale NPCs hold the flag. Band cutoff: the core band is
18-32; level 32 is the top and is IN, anything above is OUT (the
Westfall/Hillsbrad/Arathi precedent).

## ashenvale-rares.guide — 12 rares + fixed world containers

- Apothecary Falthis | npc3735 | level 22 rare (faction H — Horde-aligned, attackable by Alliance) | loop over 3 northern points (32.64, 21.98), (33.17, 21.91), (33.2, 21.1) | no loot recorded at all; no quest in the data references this NPC | source: npcs.json + quests.json
- Akkrilus | npc3773 | level 26 rare | single point (25.62, 63.54), southwest | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Terrowulf Packlord | npc3792 | level 32 rare (band top, IN) | single point (49.77, 39.61), east of center | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Lady Vespia | npc10559 | level 22 rare | loop over 2 northwest-shore points (9.87, 14.34), (13.63, 24.73) | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Rorgish Jowl | npc10639 | level 25 rare | single point (35.82, 36.61), north | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Oakpaw | npc10640 | level 27 rare | single point (56.01, 62.75), southeast of center | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Branch Snapper | npc10641 | level 25 rare | single point (46.51, 44.27), center | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Eck'alom | npc10642 | level 27 rare | single point (52.76, 70.05), southeast | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Mugglefin | npc10643 | level 23 rare | single point (19.38, 42.73), west | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Mist Howler | npc10644 | level 22 rare | loop over 2 northwest points (20.93, 36.92), (26.8, 18.35) | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Prince Raze | npc10647 | level 32 rare (band top, IN) | loop over 2 far-east points (78.08, 46.35), (81.56, 48.51) | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Ursol'lok | npc12037 | level 31 rare | single point (83.37, 48.51), far-east edge | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Fixed world containers | obj2849 (Battered Chest, 4 pts) + obj2850/obj2852 (Solid Chest, 12 + 7 pts) + obj3659/obj3695 (Barrel of Melon Juice + Food Crate, 24 shared pts) + obj3662/obj3705 (Food Crate + Barrel of Milk, 1 shared pt) + obj3689/obj3702 (Weapon Crate + Armor Crate, 4 shared pts) + obj19021 (Rusty Chest, 39 pts) + obj19022 (Worn Chest, 1 pt) + obj178144 (Troll Chest, 14 pts) + obj179487/obj179489 (Waterlogged Footlocker, 11 + 1 pts) + obj441128 (Vibrating Crate, 3 pts) | one loop step, 121 unique points, all ordinary low-level goods; no unique treasure confirmed | source: objects.json
- No contract quest has object-type objectives naming any shipped container (the only contract object objectives are q1022's obj19027 and q1140's obj19901/obj20352, none shipped here). No rare is a giver, ender, or objective of any contract quest (all 55 checked against the 13 rare ids, start/end/objectives).

Argued exclusions:
- Above the level-32 cutoff (out-of-band world content, Arathi precedent — and with zero loot there is nothing to come back for): Varo'then's Ghost (npc6118, lvl 48, 1 pt (97.9, 47.9) far east, dual 1440/1447).
- Quest-owned objectives (core covers them): q1022's Tome of Mel'Thandris (obj19027) and q1140's freed-soul objects (obj19901, obj20352).
- Out-of-zone quests reference some generic containers as objectives (q540 Hillsbrad on Barrel of Melon Juice 3659; q544 on Weapon/Food Crates 3689/3690; q2178/q5482/q6123/q6124 on Armor Crate 3702; q97204 on Food Crate 3690) — all accept outside Ashenvale, so none is Ashenvale-contract content and none blocks shipping the generics here.
- Tame lines: none shipped. All 13 rares have zero loot records in the data (no beast-evidence typing possible — npc records carry no classification flag), and the core guide carries no tame lines or references to any Ashenvale rare — logged in docs/companion-unverified.md instead of shipped as fact.

## ashenvale-recipes.guide — 9 vendor-sold + 10 exclusive single-dropper drops

Vendor-sold (profession from the item-name convention: Pattern = Leatherworking unless cloth-named, Plans = Blacksmithing, Formula = Enchanting, Recipe food/fish/drink = Cooking, Recipe potion/elixir = Alchemy — no profession flag exists in the data; all listed vendors spawn on map 1440):
- Recipe: Big Bear Steak | item3734 | buy from Ulthaan, npc3960, Butcher (50.01, 66.64) | Cooking | source: items.json vendors
- Recipe: Lean Venison | item5489 | buy from Ulthaan, npc3960 | Cooking | source: items.json vendors
- Pattern: Barbaric Leggings | item5973 | buy from Lardan, npc3958, Leatherworking Supplies (34.79, 49.84) | Leatherworking | source: items.json vendors
- Recipe: Shadow Protection Potion | item6054 | buy from Harklan Moongrove, npc3956, Alchemy Supplies (50.84, 67) | Alchemy | source: items.json vendors
- Recipe: Rockscale Cod | item6369 | buy from Wik'Tar, npc12962, Fish Merchant & Supplies (11.71, 34.1), west coast | Cooking | source: items.json vendors
- Pattern: Herbalist's Gloves | item7361 | buy from Harlown Darkweave, npc6731, Leatherworking Supplies (18.23, 60.04), southwest — the SOLE vendor anywhere (also spawns 1442; the 1440 point is used) | Leatherworking (gloves = leather, by the item-name convention) | source: items.json vendors
- Formula: Enchant Cloak - Minor Agility | item11039 | buy from Dalria, npc3954, Trade Goods (35.12, 52.12) — also a generic multi-zone world drop, but vendor-sold in-zone like the Arathi precedent | Enchanting | source: items.json vendors
- Formula: Enchant Bracer - Lesser Strength | item11101 | buy from Dalria, npc3954 | Enchanting | source: items.json vendors
- Recipe: Mithril Head Trout | item17062 | buy from Wik'Tar, npc12962 | Cooking | source: items.json vendors

Drops (sole dropper, genuinely Ashenvale content):
- Formula: Enchant Bracer - Minor Healing Power | item249475 | collect from the Dark Strand Cultist, npc3725 (level 18, 7 far-north points) — the SOLE dropper anywhere | Enchanting (name basis: Formula) | source: items.json drops
- Recipe: Bear Brisket | item250182 | collect from the Ashenvale Bear, npc3809 (level 21, 90 points across the zone) — the SOLE dropper anywhere | Cooking | source: items.json drops
- Recipe: Cleric's Elixir | item250368 | collect from the Xavian Hellcaller, npc3757 (level 29, 6 eastern points) — the SOLE dropper anywhere | Alchemy (content basis: elixir) | source: items.json drops
- Recipe: Elixir of Strength | item250385 | collect from the Shadethicket Oracle, npc3931 (level 30, 1 point (66.66, 82.17) southeast) — the SOLE dropper anywhere | Alchemy (content basis: elixir) | source: items.json drops
- Plans: Sterling Silver Gauntlet | item251337 | collect from the Wrathtail Myrmidon, npc3711 (level 20, 14 northwest-shore points) — the SOLE dropper anywhere | Blacksmithing | source: items.json drops
- Plans: Blessed Plate Pauldrons | item251438 | collect from the Highborne Lichling, npc6117 (level 46, 2 far-east-edge points (98.2, 47), (99.1, 46.2)) — the SOLE dropper anywhere; out-of-band, ships with an honest come-back-later note (Westfall Shafety Sheep precedent) | Blacksmithing | source: items.json drops
- Plans: Bronze Dory | item251455 | collect from the Dark Strand Enforcer, npc3727 (level 20, 1 point (31.62, 30.68) far north) — the SOLE dropper anywhere | Blacksmithing | source: items.json drops
- Plans: Iron Fists | item251456 | collect from the Bleakheart Hellcaller, npc3771 (level 26, 8 eastern points) — the SOLE dropper anywhere | Blacksmithing | source: items.json drops
- Pattern: Hillman's Leather Boots | item252804 | collect from the Shadowhorn Stag, npc3817 (level 22, 69 points across the zone) — the SOLE dropper anywhere | Leatherworking | source: items.json drops
- Pattern: Tooled Leather Belt | item252858 | collect from the Highborne Apparition, npc6116 (level 45, 2 far-east-edge points (98.6, 45.8), (99.1, 46.2)) — the SOLE dropper anywhere; out-of-band, ships with an honest come-back-later note | Leatherworking | source: items.json drops

Every other Ashenvale-dropping recipe drops in 3+ zones (generic world drops, Elwynn rule) — none shipped. Quest-reward recipes are unverifiable from quest records — none shipped. Professions with NO Ashenvale source: Tailoring, First Aid, Engineering, Fishing — stated in the guide, not padded (Dun Morogh Blacksmithing precedent).

Argued exclusions:
- Samophlange Manual Cover (item11147) and Samophlange Manual Page (item11148): matched the Manual regex but both carry `questItem:true` — they are quest items, not recipes. No quest in the data references them (start/objectives checked), so their chain is unverifiable — logged in docs/companion-unverified.md, not shipped.
- Formula: Enchant Gloves - Herbalism (item11151): 5 droppers across 3 zone maps (1440/1448 ancients + 1442 ancients) — multi-zone world drop, not Ashenvale content (Elwynn rule) — logged in docs/companion-unverified.md.
