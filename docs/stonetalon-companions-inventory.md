# Stonetalon Mountains companions inventory (pack 0.36.0)

Every entry shipped in the two Stonetalon Mountains companion guides, one line
each: name, NPC/item id, source type, coordinates or vendor, and the data source
verified against. All coordinates are the client's own (live) map frame on map
1442 (Stonetalon Mountains). Game data is questie-forever npcs.json, items.json
and objects.json; quest linkage checked against the full quest table and the
40-quest core contract (`stonetalon.guide`). The data carries an explicit
`rare` role flag; 9 Stonetalon NPCs hold the flag. Band cutoff: the core band
is 16–30.

## stonetalon-rares.guide — 9 rares + fixed world containers

- Pridewing Patriarch | npc4015 | level 25 rare | loop over 2 points (47.75, 46.75), (53.79, 36.31) | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Vengeful Ancient | npc4030 | level 30 rare (band top) | single point (30.45, 68.08) | no loot recorded at all; no quest linkage (it drops the multi-zone world-drop formula 11151 elsewhere — shared across 5 droppers, not a signature drop) | source: npcs.json + quests.json
- Nal'taszar | npc4066 | level 30 rare | single point (25.57, 11.48), north | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Brother Ravenoak | npc5915 | level 29 rare | single point (28.05, 12.23), north | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Sentinel Amarassan | npc5916 | level 27 rare | single point (35.25, 15.04), north | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Sorrow Wing | npc5928 | level 27 rare | single point (49.27, 36.18), center | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Sister Riven | npc5930 | level 28 rare | single point (29.64, 69.43), southwest | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Foreman Rigger | npc5931 | level 24 rare | single point (66.69, 52.33), east | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Taskmaster Whipfang | npc5932 | level 22 rare | single point (64.55, 54.19), east | no loot recorded at all; no quest linkage | source: npcs.json + quests.json
- Fixed world containers | obj2849 (Battered Chest, 10 pts) + obj2850 (Solid Chest, 7 pts) + obj3659/obj3695 (Barrel of Melon Juice + Food Crate, 1 shared pt) + obj3662/obj3705 (Food Crate + Barrel of Milk, 16 shared pts) + obj3715 (Alliance Chest, 4 pts) + obj179486/obj179488 (Battered Footlocker, 11 + 5 pts) + obj674126 (Hidden Stash, 2 pts) | one loop step, 56 unique points, all ordinary low-level goods | source: objects.json
- Unique treasures | obj19596 Sleepers' Cache (25.55, 11.36) + obj19597 Druids' Cache (29.55, 15.84) | one step over both Barrow Dens caches, said plainly | source: objects.json
- No contract quest has object-type objectives, so none of the shipped containers is quest-owned. No rare is a giver, ender, or objective of any contract quest (all 40 checked against the 9 rare ids). Apparent out-of-zone quest hits on the generic containers (404, 96102, 1618, 557, 486, Hillsbrad 540) are all cross-namespace id collisions — item or kill objectives that share an id with a chest object — none references the container itself.

Argued exclusions:
- Quest-owned singletons: Barrow Cache (obj19598, (27.96, 13.81)) and Talon Den Hoard (obj19599, (26.6, 10.87)) — the level-60 Stranglethorn quests 8102/8103 (The Pebble of Kajaro, accept Al'tabim) take their objective items from exactly these caches; the core route owns quest content, not here.
- Rares above the core band (16–30): none — the highest-flagged rare is exactly 30 (Vengeful Ancient, Nal'taszar), both shipped.
- Tame lines: none shipped. All 9 rares have zero loot records in the data (no beast-evidence typing possible), and the core guide carries no tame lines — its only pridewing mention is a contracted supply kill, not corroboration. Logged in docs/companion-unverified.md instead of shipped as fact.

## stonetalon-recipes.guide — 4 vendor-sold + 3 exclusive single-droppers

Vendor-sold (profession from the item-name convention — no profession flag exists in the data; listed vendors spawn on map 1442 and are Alliance or neutral faction):
- Pattern: Herbalist's Gloves | item7361 | buy from Harlown Darkweave, npc6731, Leatherworking Supplies (53.2, 16.9) north — the SOLE vendor anywhere (also spawns Ashenvale 1440; the 1442 point is used) | Leatherworking (gloves = leather; this exact item shipped the same way in Ashenvale) | source: items.json vendors
- Schematic: Goblin Jumper Cables | item7561 | buy from Veenix, npc4086, Venture Co. Merchant (58.22, 51.74), east | Engineering | source: items.json vendors
- Recipe: Mystery Stew | item12233 + Recipe: Heavy Kodo Stew | item12240 | buy from Janet Hommers, npc8150, Food & Drink (40.7, 81.7) south (also spawns 1443; the 1442 point is used) | Cooking (stew = food basis) | source: items.json vendors

Drops (sole dropper, genuinely Stonetalon content):
- Recipe: Royal Tea | item249880 | collect from the Windshear Geomancer, npc4003 (level 20, 6 eastern points) — the SOLE dropper anywhere | Cooking (drink basis, Alterac Thistle Tea precedent) | source: items.json drops
- Recipe: Elixir of Spirit | item250382 | collect from the Bloodfury Harpy, npc4022 (level 23, 12 western points) — the SOLE dropper anywhere | Alchemy (elixir basis) | source: items.json drops
- Plans: Brass Knuckles | item251454 | collect from the Gogger Rock Keeper, npc11915 (level 16, 18 southern points, also spawns 1443; the 1442 points are used) — the SOLE dropper anywhere | Blacksmithing (Plans + metal weapon basis) | source: items.json drops

Every other Stonetalon-dropping recipe drops in 4+ map-zones (generic world drops, Elwynn rule) — none shipped. Quest-reward recipes are unverifiable from quest records — none shipped. Professions with NO Stonetalon source: Tailoring, Enchanting, First Aid, Fishing — stated in the guide, not padded (Dun Morogh Blacksmithing precedent).

Argued exclusions:
- Horde-vendor-exclusive in-zone recipes (in-zone vendor is Horde-faction — never shipped on a guess, Alterac precedent): Recipe: Fire Protection Potion (item6055) — in-zone only Jeeda (npc4083, faction H; the Alliance source Nandar Branson is in Hillsbrad, another round's business); Formula: Enchant Cloak - Minor Agility (item11039) and Formula: Enchant Bracer - Lesser Strength (item11101) — in-zone only Kulwia (npc12043, faction H; the Alliance source Dalria is in Ashenvale, already shipped in that round's companions).
- Formula: Enchant Gloves - Herbalism (item11151): 5 droppers across 3 zone maps (Stonetalon + Ashenvale ancients) — multi-zone world drop, not Stonetalon content (consistent with the Ashenvale round's exclusion).
