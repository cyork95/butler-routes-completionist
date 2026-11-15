# Duskwood companions inventory (pack 0.40.0)

Every entry shipped in the two Duskwood companion guides, one line each:
name, NPC/item id, source type, coordinates or vendor, and the data source
verified against. All coordinates are the client's own (live) map frame on
map 1431 (Duskwood). Game data is questie-forever npcs.json, objects.json
and items.json; quest linkage checked against the full quest table and the
93-quest core contract (`duskwood.guide`). The data carries an explicit
`rare` role flag; 6 Duskwood NPCs hold it. Band cutoff: the core band is
17–28.

## dustwallow-rares replacement — duskwood-rares.guide — 6 rares + fixed world containers

- Naraxis | npc574 | level 27 rare | single point (86.36, 47.57), far east | signatures: Husk of Naraxis (item4448) + Naraxis' Fang (item4449), both sole drops; no quest takes either | also drops Vial of Spider Venom (item1130, Q101 objective, 6 droppers) and Gooey Spider Leg (item2251, Q93 objective, 19 droppers) — the hunts live in the core guide, noted, never accepted here | source: npcs.json + items.json + quests.json
- Lupos | npc521 | level 23 rare | loop over 16 points (19.99, 26.39) … (70.63, 26.64), the western road and Raven Hill woods | signatures: Hide of Lupos (item3018) + Nightbane Staff (item3227), both sole drops; no quest takes either | also drops Lean Wolf Flank (item1015, Q90 objective, 14 droppers) — noted, never accepted here | source: npcs.json + items.json + quests.json
- Lord Malathrom | npc503 | level 31 rare, ABOVE BAND — shipped with an honest come-back-later note | loop over 7 points (20.31, 28.83) … (25.92, 30.9), north-west | signatures: Spiked Collar (item1187) + Cloak of Rot (item4462), both sole drops; no quest takes either | source: npcs.json + items.json + quests.json
- Fenros | npc507 | level 32 rare, ABOVE BAND — shipped with an honest come-back-later note | loop over 8 points (60.68, 40.7) … (63.88, 51.77), east | signatures: Ravenwood Bow (item4474) + Tribal Worg Helm (item6204), both sole drops; no quest takes either | source: npcs.json + items.json + quests.json
- Commander Felstrom | npc771 | level 32 rare, ABOVE BAND — shipped with an honest come-back-later note | loop over 10 points (13.18, 36.19) … (18.55, 35.73), west | signatures: Trouncing Boots (item4464) + Bonefist Gauntlets (item4465), both sole drops; no quest takes either | source: npcs.json + items.json + quests.json
- Nefaru | npc534 | level 34 rare, ABOVE BAND — shipped with an honest come-back-later note | loop over 3 points (61.85, 81.38), (63.48, 83.67), (74.33, 77.9), far south | signatures: Beastwalker Robe (item4476) + Nefarious Buckler (item4477), both sole drops; no quest takes either | source: npcs.json + items.json + quests.json
- Fixed world containers | obj2850 (Solid Chest, 20 pts) + obj2852 (Solid Chest, 32 pts) + obj3659/obj3695 (Barrel of Melon Juice + Food Crate, 34 shared pts) | one loop step, 86 unique points, ordinary low-level goods | source: objects.json
- Unique containers | obj21052 Defias Strongbox (23.92, 72.07), west | obj119/obj167 Abercrombie's Crate (33.42, 76.35), south-west | obj441114 Mysterious Box (65.7, 67.4), south | obj411348 Dusty Coffer (26.0, 31.0), north-west | obj410779 Offering Box (81.2, 71.8), far south-east | obj321/obj706187 Tear of Tilloa (78.35, 35.95), east | each its own step | source: objects.json
- Markers (flavor, no loot confirmed — one noted step) | obj37 Eliza's Tombstone (28.9, 30.5) | obj410034 Carved Stone (49.4, 34.0) | obj22706 Faustin's Alchemy Set (87.48, 35.19) | obj612088 Field Guide (78.3, 45.3) | obj673515 Memory of Valor (21.1, 55.6) | obj177280 Moonwell (49.2, 33.29) | source: objects.json

Argued exclusions:
- Classic rares WITHOUT the data flag (Mor'Ladim npc522 L35, Stitches npc412 L35, Stalvan Mistmantle npc315 L32, Eliza npc314 L31, Morbent Fel npc1200 L32 — all roles=undefined): the rule is the flag, and the flag is absent. Data wins over community memory; named here so the omission is deliberate, not an oversight.
- Quest-owned objects: Nightmare Moss (obj439557), Cold Iron Deposit (obj439558), Unhatched Green Dragon Egg (obj441119), Ogre Magi Text (obj441113) are objectives of the contracted Missions IX–XII/XVIII (81736–81741); Mound of Dirt (obj59) starts core 95/230, Weathered Grave (obj61) starts core 225/231, Eliza's Grave Dirt (obj51708) starts core 254, Battered Trunk (obj642320) starts core writ 94223, Spellbook (obj409735) starts core 78147, Mound of Dirt (obj19030) is core 1043's objective. None is companion content.
- Flavor/furniture surveyed but not shipped (no container or loot in the data): all signposts, chairs, campfires, anvils, forges, the mailbox, books on desks, Hyun... pumpkins/decor, doors, herbs (1620–1628), veins (1731–1738), leyline, portals.
- No contract quest has any of the 6 shipped rares as giver, ender, or kill objective (all 93 checked). The shared core-item drops (1130, 2251, 1015) are source notes, not quest ownership.
- Tame lines: none shipped. The data has no tameability flag; Lupos shows wolf evidence (Lean Wolf Flank) and Naraxis spider evidence (Spinnerets, Gooey Legs), but the core guide carries no tame corroboration (no Hunter taming chain in the 93-contract). All logged in docs/companion-unverified.md instead of shipped as fact.

## duskwood-recipes.guide — 9 vendor-sold + 5 in-zone drops

Vendor-sold (all vendors neutral or Alliance; profession from the item-name convention — no profession flag exists in the data):
- Recipe: Holy Protection Potion | item6053 | buy from Kzixx, npc3134 [AH], (81.82, 19.77) north-east | Alchemy (protection potion) | source: items.json vendors
- Recipe: Shadow Oil | item6068 | buy from Bliztik, npc2481 [AH], (18.04, 54.36) west | Alchemy (oil) | source: items.json vendors
- Pattern: Greater Adept's Robe | item6275 | buy from Sheri Zipstitch, npc2669 [A], (75.68, 45.57) Darkshire | Tailoring (robe) | source: items.json vendors
- Pattern: Dark Silk Shirt | item6401 | buy from Sheri Zipstitch (also Horde-sold elsewhere; the Alliance source is the shipped one) | Tailoring (shirt) | source: items.json vendors
- Schematic: Goblin Jumper Cables | item7561 | buy from Kzixx [AH] (also Horde-sold elsewhere) | Engineering (schematic) | source: items.json vendors
- Pattern: Bright Yellow Shirt | item14627 | buy from Danielle Zipstitch, npc2668 [A], (75.87, 45.56) Darkshire — SOLE ZONE [1431] | Tailoring (shirt) | source: items.json vendors
- Recipe: Elixir of Coalesced Regret | item210709 | buy from Kzixx [AH] | Alchemy (elixir) | source: items.json vendors
- Pattern: Linen Reagent Bag | item253665 | buy from Lohgan Eva / Danielle / Sheri Zipstitch [A], Darkshire row | Tailoring (bag) | source: items.json vendors
- Pattern: Woolen Reagent Bag | item253668 | buy from Lohgan Eva / Danielle / Sheri Zipstitch [A], Darkshire row | Tailoring (bag) | source: items.json vendors

Drops (in-zone droppers; sole-zone ones plain, the 3-zone one noted — the Dustwallow dual-zone precedent):
- Plans: Sterling Silver Leggings | item251336 | collect from the Skeletal Warrior, npc48 (L21, (76.88, 70.25), (76.91, 72.2)) — SOLE ZONE [1431] | Blacksmithing (plans + metal basis) | source: items.json drops
- Manual: Clever Poultice | item255724 | collect from the Defias Enchanter, npc910 (L26, (21.27, 71.96), (21.35, 73.36)) — SOLE ZONE [1431] | First Aid (manual basis) | source: items.json drops
- Recipe: Minor Cleric's Elixir | item250366 | collect from the Murloc Forager, npc46 (L9, (58.6, 9.8), (62.2, 11.1)) — 3 zones [1429, 1431, 1420], noted honestly | Alchemy (elixir) | source: items.json drops
- Pattern: Robes of Arcana | item5773 | collect from the Defias Enchanter, npc910 (L26, (21.27, 71.96), (21.35, 73.36)) — 4 zones [1431, 1439, 1413, 1441], noted honestly | Tailoring (pattern basis) | source: items.json drops
- Pattern: Invoker's Cord | item215369 | collect from the Skeletal Fiend, npc531 (L24, (15.04, 42.0), (15.28, 46.38)) — 4 zones [1454, 1438, 1457, 1431], noted honestly | Tailoring (pattern basis) | source: items.json drops

Every other Duskwood-dropping recipe drops in 5+ map-zones (generic world drops, Elwynn rule) — none shipped. Quest-reward recipes are unverifiable from quest records — none shipped. Professions with NO Duskwood source: Leatherworking, Cooking, Fishing, Enchanting — stated in the guide, not padded (Dun Morogh Blacksmithing precedent).

Argued exclusions:
- No Horde-vendor-exclusive in-zone recipes exist (all 1431 vendors are Alliance or neutral) — nothing to exclude under the Alterac precedent.
