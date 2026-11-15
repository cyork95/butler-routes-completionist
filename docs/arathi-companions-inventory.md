# Arathi companions inventory (pack 0.32.0)

Every entry shipped in the two Arathi Highlands companion guides, one line
each: name, NPC/item id, source type, coordinates or vendor, and the data source
verified against. All coordinates are the client's own (live) map frame on map
1417 (Arathi Highlands). Game data is questie-forever npcs.json, items.json
and objects.json; quest linkage checked against the full quest table and the
47-quest core contract (`arathi.guide`). The data carries explicit `rare`
role flags; 11 Arathi NPCs hold the flag. Band cutoff: the core band is 30-40,
drawn at the top (the Hillsbrad precedent — 33+ excluded there).

## arathi-rares.guide — 9 rares + fixed world containers

- Darbel Montrose | npc2598 | level 39 rare Shadow Council warlock (rank 2 record, but role-flagged rare), flagged rare in the data | loop over 14 Stromgarde points (bbox 25.2-29.8, 60.5-65.9) | no loot recorded at all | source: npcs.json
- Singer | npc2600 | level 34 rare, flagged rare in the data | single point (32.31, 30.99) north of the circle | no loot recorded at all | source: npcs.json
- Ruul Onestone | npc2602 | level 39 rare, flagged rare in the data | single point (17.96, 68.56), far west | no loot recorded at all | source: npcs.json
- Kovork | npc2603 | level 36 rare, flagged rare in the data | loop over 3 central points (30.37, 43.77), (31.76, 46.21), (33, 44.04) | no loot recorded at all | source: npcs.json
- Molok the Crusher | npc2604 | level 39 rare, flagged rare in the data | loop over 3 southern points (53.23, 80.18), (54.62, 79.71), (54.88, 81.51) | no loot recorded at all | source: npcs.json
- Zalas Witherbark | npc2605 | level 40 rare Warband Leader, flagged rare in the data | loop over 10 southeastern points (bbox 61.1-70.2, 72.4-81.8) | no loot recorded at all | source: npcs.json
- Nimar the Slayer | npc2606 | level 37 rare Warband Leader, flagged rare in the data | loop over 15 east-central points (bbox 60.2-73.5, 61.3-74.7) | no loot recorded at all | source: npcs.json
- Geomancer Flintdagger | npc2609 | level 40 rare, flagged rare in the data | single point (82.8, 32.23), far east | no loot recorded at all | source: npcs.json
- Tamra Stormpike | npc14275 | level 28 rare (also a Hillsbrad rare; dual-zone spawn), flagged rare in the data | loop over 3 far-west points (9.1, 47.2), (10.6, 51), (11.4, 49.9) | no loot recorded in this data build at all | source: npcs.json
- Fixed Chests — world containers | obj2855 (Solid Chest, 9 pts) + obj2857 (Solid Chest, 18 pts) + obj153451 (Solid Chest, 1 pt, far NE) + obj3659 (Barrel of Melon Juice, 2 pts) + obj3695 (Food Crate, 2 pts, same placements) + obj3706 (Barrel of Sweet Nectar, 32 pts) + obj3707 (Food Crate, 32 pts, same placements) + obj4096/obj105579/obj105581 (Alliance Chest, 3+4+4 pts) + obj105578 (Horde Chest, 3 pts, contested-zone supply chest, anyone can open) | one loop step, 76 unique points, all ordinary low-level goods | source: objects.json
- Illari's Loot Cache | obj418855 | single point (94.15, 69.28), far east | no quest in the data references this object — unique cache, own step; contents unconfirmed in the data | source: objects.json + quests.json
- No contract quest has object-type objectives (checked all 47), so none of the shipped containers is quest-owned. No rare is a giver, ender, or objective of any contract quest (all 47 start/end records checked against the 11 rare ids).

Argued exclusions:
- Above the level-40 cutoff (out-of-band world content, Hillsbrad precedent): Foulbelly (npc2601, lvl 42, 4 pts in the west) and Prince Nazjak (npc2779, lvl 41, 24 pts in the southwest).
- Quest-owned containers (core covers them, Dun Morogh precedent): Trelane's Chest/Footlocker/Lockbox (obj2716/2717/2718 — source the contracted 696's three items), the Sealed Barrel (obj422911 — contracted 79677's Spice), the Messenger Bag and Hastily Rolled-Up Satchel (obj406918/424006 — the contracted Eagle's Fist chain), the Syndicate Footlocker (obj656157 — contracted 96784's start).
- Quest-significant singletons: Cache of Explosives (obj2704) — its only significance is Wetlands-contract quest 633 (precise start/objective reference check); the Wetlands guide owns it.
- Tame lines: none shipped. All 11 rares have zero loot records in the data (no beast-evidence typing possible), and the core guide carries no tame lines or references to any Arathi rare — logged in docs/companion-unverified.md instead of shipped as fact.

## arathi-recipes.guide — 15 vendor-sold + 8 exclusive/near-exclusive drops

Vendor-sold (profession from the item-name convention: Pattern-cloth = Tailoring, Pattern-leather/mail = Leatherworking, Plans = Blacksmithing, Schematic = Engineering, Formula = Enchanting, Recipe food/drink = Cooking, Recipe potion = Alchemy, Manual bandage = First Aid — no profession flag exists in the data; all listed vendors spawn on map 1417):
- Recipe: Curiously Tasty Omelet | item3682 | buy from Keena, npc2821, Trade Goods (74.09, 32.73) | Cooking | source: items.json vendors
- Recipe: Roast Raptor | item12228 | buy from Keena, npc2821 (also sold by Hammon Karwn, npc2810) | Cooking | source: items.json vendors
- Pattern: Barbaric Leggings | item5973 | buy from Keena, npc2821 (also sold by Hammon Karwn, npc2810) | Leatherworking | source: items.json vendors
- Formula: Enchant Bracer - Lesser Deflection | item11163 | buy from Keena, npc2821 | Enchanting | source: items.json vendors
- Recipe: Barbecued Buzzard Wing | item4609 | buy from Narj Deepslice, npc2814, Butcher (45.54, 47.61), Refuge Pointe | Cooking | source: items.json vendors
- Pattern: Barbaric Leggings | item5973 | buy from Hammon Karwn, npc2810, Superior Tradesman (46.49, 47.41), Refuge Pointe | Leatherworking | source: items.json vendors
- Recipe: Roast Raptor | item12228 | buy from Hammon Karwn, npc2810 | Cooking | source: items.json vendors
- Recipe: Frost Protection Potion | item6056 | buy from Drovnar Strongbrew, npc2812, Alchemy Supplies (46.32, 47.04), Refuge Pointe | Alchemy | source: items.json vendors
- Pattern: Azure Silk Cloak | item7089 | buy from Jun'ha, npc6574, Tailoring Supplies (72.69, 36.45) | Tailoring | source: items.json vendors
- Pattern: Linen Reagent Bag | item253665 + Pattern: Woolen Reagent Bag | item253668 | buy from Jun'ha, npc6574 (34 vendors each worldwide, but vendor-sold in-zone like the Hillsbrad precedent) | Tailoring | source: items.json vendors
- Pattern: Green Leather Armor | item7613 | buy from George Candarte, npc2698, Leatherworking Supplies (28.1, 11.8), north (also spawns 1424/1425; the 1417 point is used) | Leatherworking | source: items.json vendors
- Plans: Solid Iron Maul | item10858 | buy from Jannos Ironwill, npc1471, Superior Macecrafter (45.98, 47.72), Refuge Pointe | Blacksmithing | source: items.json vendors
- Pattern: Raptor Hide Harness | item13287 | buy from Tunkk, npc2819, Leatherworking Supplies (74.84, 34.59) — the SOLE vendor anywhere | Leatherworking | source: items.json vendors
- Pattern: Raptor Hide Belt | item13288 | buy from Androd Fadran, npc2816, Leatherworking Supplies (45.08, 46.83), Refuge Pointe — the SOLE vendor anywhere | Leatherworking | source: items.json vendors
- Manual: Heavy Silk Bandage | item16112 + Manual: Mageweave Bandage | item16113 | buy from Deneb Walker, npc2805, Scrolls & Potions (26.97, 58.83) | First Aid | source: items.json vendors

Drops (sole dropper, or 2 droppers both in-zone — genuinely Arathi content):
- Pattern: Murloc Scale Bracers | item5789 | collect from the Blackwater Deckhand, npc2636 (level 38, 3 Faldir's points) — one of only 2 droppers anywhere, both accounted in-zone | Leatherworking | source: items.json drops
- Formula: Twisted Nether Wand | item249487 | collect from the Boulderfist Magus, npc2567 (level 36, 9 southern points) — the SOLE dropper anywhere | Enchanting (name basis: Formula) | source: items.json drops
- Plans: Sterling Silver Boots | item251335 | collect from the Syndicate Watchman, npc2261 (level 20, 1 point (19, 20) northwest) — the SOLE dropper anywhere | Blacksmithing | source: items.json drops
- Plans: Hard Gold Boots | item251386 | collect from the Syndicate Highwayman, npc2586 (level 30, 23 Northfold points) and the Syndicate Smuggler, npc267065 (level 35, 28 western points) — the ONLY 2 droppers anywhere, both in-zone | Blacksmithing | source: items.json drops
- Plans: Shining Mithril Pauldrons | item251393 | collect from the Daggerspine Sorceress, npc2596 (level 39, 8 shore points) — the SOLE dropper anywhere | Blacksmithing | source: items.json drops
- Pattern: Earthen Silk Slippers | item254014 | collect from the Witherbark Troll, npc2552 (level 30, 5 points) — the SOLE dropper anywhere | Tailoring (slippers = cloth) | source: items.json drops
- Manual: Greater Healing Potion | item255723 | collect from the Syndicate Mercenary, npc2589 (level 31, 14 Northfold points) — the SOLE dropper anywhere | Alchemy (content basis: potion; the Manual prefix is shared with First Aid bandages, so the basis is logged here) | source: items.json drops
- Schematic: EZ-Thro Bronze Mortar | item264212 | collect from the Boulderfist Shaman, npc2570 (level 38, 12 western points) — the SOLE dropper anywhere | Engineering | source: items.json drops

Every other Arathi-dropping recipe drops in 3+ zones, most in dozens (generic world drops, Elwynn rule) — none shipped. Quest-reward recipes are unverifiable from quest records — none shipped. Professions with NO Arathi source: Fishing — stated in the guide, not padded (Dun Morogh Blacksmithing precedent).

Profession gates use `when skill <Profession> 1` (supported by the format); stock class (limited vs unlimited) is not in the local data, so no recipe is marked limited.
