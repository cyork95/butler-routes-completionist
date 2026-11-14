# Westfall companions inventory (pack 0.10.0)

Every entry shipped in the two Westfall companion guides, one line each: name,
NPC/item id, source type, coordinates or vendor, and the data source verified
against. All coordinates are the client's own (live) map frame on map 1436
(Westfall). Game data is questie-forever npcs.json, items.json and objects.json;
quest linkage checked against the full quest table and the core guide text. The
data carries explicit `rare` role flags on nine Westfall NPCs, which settle the
true-rare calls below.

## westfall-rares.guide — 14 rares + fixed world containers

- Master Digger | npc1424 | level 15 rare kobold, flagged rare in the data | single point (46.42, 19.06), the Jangolode Mine | signature drops item6205 Burrowing Shovel, item6206 Rock Chipper (each dropped by nothing else) | source: npcs.json + items.json
- Benny Blaanco | npc502 | level 15 rare | single point (49.47, 18.99) | no unique loot; greens only | source: npcs.json + items.json
- Slark | npc519 | level 15 rare murloc (drops a Murloc Eye; not tameable), flagged rare in the data | single point (47.01, 10.94), the northern shore | signature drops item3188 Coral Claymore, item6180 Slarkskin (each dropped by nothing else); also carries item1357 Captain Sander's Treasure Map, which starts contracted core quest 136 — noted as core-covered | source: npcs.json + items.json
- Silverspur | npc210533 | level 14 rare | loop over 6 points, the northwest (bbox 33.6-36.0, 37.2-40.8) | no loot recorded at all | source: npcs.json
- Brack | npc520 | level 19 rare, flagged rare in the data | single point (27.27, 44.54), the western shore | signature drops item2235 Brackclaw, item6179 Privateer's Cape (each dropped by nothing else); also carries item1357 Captain Sander's Treasure Map, which starts contracted core quest 136 — noted as core-covered | source: npcs.json + items.json
- Sergeant Brashclaw | npc506 | level 18 rare, flagged rare in the data | single point (36.88, 31.85) | signature drops item2203 Brashclaw's Chopper, item2204 Brashclaw's Skewer (each dropped by nothing else) | source: npcs.json + items.json
- Foe Reaper 4000 | npc573 | level 20 rare harvest machine (not tameable), flagged rare in the data | loop over 24 points across the farm fields (bbox 33.2-65.0, 19.3-69.4) | signature drops item933 Large Rucksack, item4434 Scarecrow Trousers (each dropped by nothing else) | source: npcs.json + items.json
- Dust Devil | npc832 | level 18 rare elemental (drops an Elemental Core; not tameable) | loop over 12 scattered points (bbox 33.3-68.6, 22.1-73.5) | signature drops item4290 Dust Bowl, item5669 Dust Devil Debris, item209058 Elemental Core (each dropped by nothing else) | source: npcs.json + items.json
- Undying Laborer | npc210537 | level 14 rare undead (not tameable) | loop over 24 points from the coast to the eastern mines (bbox 27.4-65.0, 8.6-64.4) | signature drop item208849 Libram of Blessings (dropped by nothing else; the data records nothing else on him) | source: npcs.json + items.json
- Leprithus | npc572 | level 19 rare ghoul (drops Ghoul Fingers; undead, not tameable), flagged rare in the data | loop over 2 points, one northern (41.93, 29.24) and one far eastern (64.71, 66.7) | signature drops item1314 Ghoul Fingers, item1387 Ghoulfang (each dropped by nothing else) | source: npcs.json + items.json
- Marisa du'Paige | npc599 | level 18 rare, flagged rare in the data | loop over 3 points, the southeast (bbox 42.2-44.2, 76.8-79.9) | signature drops item3019 Noble's Robe, item4660 Walking Boots (each dropped by nothing else) | source: npcs.json + items.json
- Brainwashed Noble | npc596 | level 18 rare, flagged rare in the data | single point (43.98, 78.33) | signature drops item3902 Staff of Nobles, item5967 Girdle of Nobility (each dropped by nothing else) | source: npcs.json + items.json
- Foreman Thistlenettle | npc626 | level 20 rare, the Jangolode foreman (not rare-flagged, but a named foreman with four exclusive drops and no quest link — genuine rare by the loot rule) | single point (42.22, 82.61) | signature drops item1875 Thistlenettle's Badge, item2166 Foreman's Leggings, item2167 Foreman's Gloves, item2168 Foreman's Boots (each dropped by nothing else) | source: npcs.json + items.json
- Horror of the Deep | npc210487 | level 20 rare (not rare-flagged, but a distinct named record with no quest link and no ambient twin — same shape as the Elwynn no-loot shippers) | loop over 4 points off the southwest coast (bbox 26.0-26.8, 66.0-69.8) | no loot recorded at all | source: npcs.json
- Fixed world containers | obj106319 (24 Battered Chest pts) + obj2849 (9 Battered Chest pts) + obj123214 + obj124072 (two Duskwood Chests at the same eastern point 70.4, 73.9) + obj1166 (Alexston's Chest, 1 pt) + obj177790 (Strange Lockbox, 1 pt) + obj19017 (Giant Clam, 6 coastal pts) + obj19019 (Box of Assorted Parts, 2 pts) + obj581777 (Suspicious Crate, 10 Moonbrook pts) + obj459259 (Mech Arm, 12 pts at the northeastern mine) + obj290 (Furlbrow's Wardrobe, 1 pt) | one loop step, 67 points, all ordinary low-level goods, no unique treasure | source: objects.json

Band cutoff argued: the zone's contract quests run to level 22 (quest 166), so the
cutoff is drawn at level 20 — everything above it is out-of-band world content
(Vultros and Klaven Mortwake at 26, the captains at 30-33, and higher). Nothing
at 19-20 is excluded on level alone; every shipped step states the rare's actual
level.

Argued exclusions:
- Core quest targets/item sources, covered by the core route: Old Murk-Eye (not rare-flagged; his only exclusive is item3636, the Scale that contracted quest 104 needs — a quest-target mob, not a genuine rare), the Defias Messenger (not rare-flagged; his only exclusive is item1381, the Mysterious Message that contracted quest 142 needs).
- Core quest NPCs: The Defias Traitor (155 escort), Captain Danuvin (102), Captain Grayson (103/104/152), Thor (6281 flight), Alba Fairmoon (92742-92819 chain), Ozwin Ironsprocket (92909-92911), Daphne Stilwell (Tome of Valor chain, uncontracted), Agent Kearnen (Klaven's Tower, uncontracted).
- Vendors (service NPCs, not rares): Defias Profiteer (also a recipe vendor — see the recipes guide), Gina MacGregor, William MacGregor, Mike Miller.
- Above the level-20 cutoff: Vultros (26, rare-flagged but out of band), Klaven Mortwake (26), Christopher Hewen (30), Kriggon Talsone (25, a recipe vendor — see the recipes guide), Protector of the People (40), Venture Co. Miner/Geologist (34), and all higher records.
- Ambient generics (mob types, not rare individuals): Defias Raider, Riverpaw Shaman, Lumberjack, Ghoul, Coyote Packleader (pack-alpha pattern, no unique loot, no rare flag), Young Fleshripper, Young Goretusk (Elwynn precedent).
- Cross-zone rares owned by the Elwynn companion: Longsnout (2 Westfall pts vs a 9-pt Elwynn loop) and Ada Gelhardt (3 vs 10) — excluded here to avoid duplicating them across companions.
- Quest-owned treasure objects: Captain's Footlocker, Broken Barrel, Old Jug, Locked Chest (contracted Sander chain 136-140, routed in the core guide); Old Footlocker (Stalvan chain 67/68, uncontracted); Connery's Trunk (96337); Forgotten Shrine (Call of Water chain); Gnomish Tome, Spellbook, Burned-Out Remains (collection quests). Leyline objects are ambient magic, not containers.

## westfall-recipes.guide — 10 recipes: 9 vendor-sold, 1 exclusive drop

- Recipe: Clam Chowder | item5528 | buy from Kriggon Talsone, npc4305, southwestern shore (36.23, 90.18) | Cooking | source: items.json vendors
- Recipe: Slitherskin Mackerel | item6326 | buy from Kriggon Talsone, npc4305 | Cooking | source: items.json vendors
- Recipe: Rainbow Fin Albacore | item6368 | buy from Kriggon Talsone, npc4305 | Cooking | source: items.json vendors
- Recipe: Spiced Chili Crab | item16111 | buy from Kriggon Talsone, npc4305 | Cooking | source: items.json vendors
- Recipe: Rage Potion | item5640 | buy from Defias Profiteer, npc1669, Moonbrook (43.47, 66.76) | Alchemy | source: items.json vendors
- Pattern: Murloc Scale Belt | item5786 | buy from Gina MacGregor, npc843, Sentinel Hill (57.64, 54.05) | Leatherworking | source: items.json vendors
- Pattern: Murloc Scale Breastplate | item5787 | buy from Gina MacGregor, npc843 | Leatherworking | source: items.json vendors
- Pattern: Red Linen Bag | item5771 | buy from Gina MacGregor, npc843 | Tailoring (linen) — also drops from Defias Looter + 2 other zones, but the vendor source ships it | source: items.json vendors
- Pattern: Blue Overalls | item6274 | buy from Gina MacGregor, npc843 | Tailoring | source: items.json vendors
- Schematic: Shafety Sheep | item264210 | collect from the Venture Co. Miner, npc1094, southeastern shore (75.2, 88.3) — the SOLE dropper anywhere, so genuinely Westfall content — but the miner is level 34, far above the band, so the step says to come back at high level | Engineering | source: items.json drops

Profession gates use `when skill <Profession> 1` (supported by the format); stock class (limited vs unlimited) is not in the local data, so no recipe is marked limited.

Borderline drop argued: Pattern: Red Woolen Bag (item5772) drops from the Westfall Defias Renegade Mage (npc450) plus one mob elsewhere — a two-zone world drop, not Westfall content per the Elwynn rule, so NOT shipped. Every other Westfall-dropping recipe also drops across dozens of zones (generic world drops).
