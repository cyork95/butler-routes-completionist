# Feralas companions inventory (pack 0.42.0)

Every entry shipped in the two Feralas companion guides, one line each:
name, NPC/item id, source type, coordinates or vendor, and the data source
verified against. All coordinates are the client's own (live) map frame on
map 1444 (Feralas). Game data is questie-forever npcs.json, objects.json
and items.json; quest linkage checked against the full quest table and the
57-quest core contract (`feralas.guide`). The data carries an explicit
`rare` role flag; 12 Feralas NPCs hold it. Band cutoff: the core band is
38–50.

## feralas-rares.guide — 9 rares + 3 fixed containers

- Lady Szallah | npc5343 | level 46 rare | single point (28.2, 67.6), far south | signature: Naga Caster's Staff (item284850), sole drop; no quest takes it in the data | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Bloodroar the Stalker | npc5346 | level 48 rare | single point (52.03, 60.91), south | signature: Yeti Hide Stompers (item285047), sole drop; no quest takes it | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Antilus the Soarer | npc5347 | level 48 rare | single point (55.6, 74.15), south-east | signature: Hippogryph Down Leggings (item284847), sole drop; no quest takes it | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Arash-ethis | npc5349 | level 49 rare | single point (44.79, 25.02), north-center | signature: Windserpent Scaled Cloak (item284866), sole drop; no quest takes it | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Qirot | npc5350 | level 47 rare | single point (76.65, 66.24), far east | signature: Silithid Sinew Crossbow (item284859), sole drop; no quest takes it | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Old Grizzlegut | npc5352 | level 43 rare | single point (59.46, 59.44), east | signature: Sturdy Bearhide Legguards (item284843), sole drop; no quest takes it | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Snarler | npc5356 | level 42 rare | single point (80.22, 39.57), east | signature: Snarling Fang (item285043), sole drop; no quest takes it | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Diamond Head | npc5345 | level 45 rare | single point (36.6, 51.41), center | NO sole drop in the data — kill goal + note only | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Gnarl Leafbrother | npc5354 | level 44 rare | single point (69.24, 57.31), east | NO sole drop in the data — kill goal + note only | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Old Crate | obj442688 | single point (76.6, 48.0), east | no loot table confirmed | source: objects.json
- Grimtotem Chest | obj443727 | single point (69.6, 43.3), east | no loot table confirmed | source: objects.json
- Old Chest | obj642451 | single point (79.2, 49.35), far east | no loot table confirmed; this is the turn-in object of quest 95599 (The Old Key), which has no accept in the data and is OUT of the core contract as broken — the chest is real, the quest line is not routed anywhere | source: objects.json + quests.json

Argued exclusions:
- Above-band rares (Westfall/Hillsbrad precedent — excluded, Dire Maul area, far above the 38–50 band): Mushgog npc11447 L60 (62.5, 30.0; sole drop Black Lotus item13468 — logged below), The Razza npc11497 L60 (62.5, 29.9; no sole drop), Skarr the Unbreakable npc11498 L58 (62.5, 30.37; no sole drop).
- Quest-target lookalikes WITHOUT the data flag (roles=undefined): Lord Shalzaru npc8136 L47 (2870 objective), Woodpaw Alpha npc5258 L43, Gordunni Shaman/Warlock/Ogre Mage/Mage-Lord npc5236/5240/5237/5239 (2982 objectives), Ohk'zi (92858 objective mob). None is flagged rare; none has loot of its own beyond its quest role. Data wins over community memory.
- Quest-owned objects: Shay's Chest (obj144054) is 2845's objective; the Wrecked Row Boat, Backpacks, and Pod are courier-chain objects; the Wanted poster, Gazebo, Monolith are contracted starts/ends. None is companion content.
- Flavor/furniture surveyed but not shipped (no container or loot in the data): 2 mailboxes, 5 Burning Embers objects (12 east-side points — fire visuals, not containers).
- No contract quest has any of the 9 shipped rares as giver, ender, or kill objective (all 57 checked). No signature is a quest objective anywhere in the data (all 7 checked).
- Tame lines: none shipped. The data has no tameability flag and the core guide carries no tame corroboration (no `task` tame lines in `feralas.guide`). Logged in docs/companion-unverified.md instead of shipped as fact.

## feralas-recipes.guide — 13 vendor-sold + 11 in-zone drops

Vendor-sold (buy from the Alliance vendor named; Horde twin-sellers noted where the data shows them):
- Recipe: Nature Protection Potion | item6057 | buy from Logannas, npc8157 [A], (32.67, 44.03) Feathermoon (also sold by Horde vendor Bronk — the Alliance source is the shipped one) | Alchemy (potion basis) | source: items.json vendors
- Recipe: Ghost Dye | item9302 | buy from Logannas [A] (same) | Alchemy (dye basis) | source: items.json vendors
- Pattern: Azure Silk Cloak | item7089 | buy from Brienna Starglow, npc6576 [A], (88.96, 45.95) far east | Tailoring (pattern/silk basis) | source: items.json vendors
- Pattern: Linen Reagent Bag | item253665 | buy from Brienna Starglow [A] (same) | Tailoring (bag basis) | source: items.json vendors
- Pattern: Woolen Reagent Bag | item253668 | buy from Brienna Starglow [A] (same) | Tailoring (bag basis) | source: items.json vendors
- Pattern: Green Whelp Bracers | item7451 | buy from Pratt McGrubben, npc7852 [A], (30.63, 42.71) Feathermoon (also sold by Horde vendor Jangdor) | Leatherworking (whelp-scale basis) | source: items.json vendors
- Pattern: Turtle Scale Gloves | item8385 | buy from Pratt McGrubben [A] (also Horde-sold; also a 370-dropper world drop — the vendor source is the shipped one) | Leatherworking (scale basis) | source: items.json vendors
- Pattern: Living Shoulders | item15734 | buy from Pratt McGrubben [A] (also Horde-sold) | Leatherworking (pattern basis) | source: items.json vendors
- Recipe: Hot Wolf Ribs | item12229 | buy from Vivianna, npc7947 [A], (31.3, 43.46) Feathermoon (also Horde-sold) | Cooking (recipe/food basis) | source: items.json vendors
- Recipe: Lobster Stew | item13947 | buy from Vivianna [A] (also Horde-sold) | Cooking | source: items.json vendors
- Recipe: Mightfish Steak | item13948 | buy from Vivianna [A] (also Horde-sold) | Cooking | source: items.json vendors
- Recipe: Baked Salmon | item13949 | buy from Vivianna [A] (also Horde-sold) | Cooking | source: items.json vendors
- Schematic: Snake Burst Firework | item19027 | buy from Zorbin Fandazzle, npc14637 [AH neutral], (44.81, 43.42) center | Engineering (schematic basis) | source: items.json vendors

Drops (in-zone droppers; sole-zone ones plain, the one dual-zone noted):
- Formula: Enchant 2H Weapon - Lesser Strength | item249513 | collect from the Hatecrest Sorceress, npc5336 (L43, (23.78, 62.42), (24.35, 65.39)) — SOLE ZONE [1444] | Enchanting (formula basis) | source: items.json drops
- Recipe: Triage Tea | item249882 | collect from the Woodpaw Mystic, npc5254 (L42, (65.13, 52.68), (65.29, 51.89)) — SOLE ZONE [1444] | First Aid (triage basis) | source: items.json drops
- Recipe: Superior Frenzy Potion | item250986 | collect from the Northspring Roguefeather, npc5363 (L48, (37.44, 15.62), (38.18, 12.08)) — SOLE ZONE [1444] | Alchemy (potion basis) | source: items.json drops
- Plans: Mithril Claymore | item251462 | collect from the Woodpaw Mongrel, npc5249 (L40, (69.37, 51.35), (69.74, 50.85)) — SOLE ZONE [1444] | Blacksmithing (plans/mithril basis) | source: items.json drops
- Plans: Charged Mithril Battleaxe | item251464 | collect from the Gordunni Brute, npc5232 (L42, (58.58, 64.94), (59.31, 63.63)) — SOLE ZONE [1444] | Blacksmithing | source: items.json drops
- Pattern: Charged Scorpid Belt | item252909 | collect from the Rage Scar Yeti, npc5296 (L46, (51.8, 30.79), (52.38, 29.74)) — SOLE ZONE [1444] | Leatherworking (scorpid basis) | source: items.json drops
- Pattern: Supple Scorpid Bracers | item252916 | collect from the Groddoc Thunderer, npc5262 (L49, (37.68, 23.38), (39.92, 18.65)) — SOLE ZONE [1444] | Leatherworking | source: items.json drops
- Pattern: Earthen Leggings | item254000 | collect from the Gravelsnout Surveyor, npc4116 (L29, (91.9, 49.0)) — 2 zones [1441, 1444], noted honestly | Tailoring (pattern/earthen basis) | source: items.json drops
- Pattern: Earthenweave Boots | item254094 | collect from the Elder Rage Scar, npc5297 (L48, (54.05, 32.51), (54.89, 33.52)) — SOLE ZONE [1444] | Tailoring | source: items.json drops
- Pattern: Stormcloth Boots | item254686 | collect from the Hatecrest Serpent Guard, npc5333 (L44, (24.75, 72.57), (25.17, 72.74)) — SOLE ZONE [1444] | Tailoring | source: items.json drops
- Manual: Superior Healing Potion | item255725 | collect from the Gordunni Shaman, npc5236 (L44, (58.44, 67.55), (58.98, 69.92)) — SOLE ZONE [1444] | First Aid (manual basis) | source: items.json drops

Argued exclusions:
- Horde-vendor-exclusive (Alterac precedent — Alliance guide): Pattern: Nightscape Shoulders (item8409) and 5 armor-kit patterns (items 252783/252784/252811/252812/252942), sold ONLY by Jangdor Swiftstrider [H] (74.43, 42.91). No Alliance source in the data.
- Above-band/out-of-reach drops: Pattern: Bottomless Bag (item14510, single in-zone dropper Dreamroarer L62 world boss, 5 zones) and Plans: Sageblade (item22389, in-zone droppers the 4 Emerald Dragons L63, 5 zones). Logged, never shipped.
- Duplicate record: Pattern: Turtle Scale Gloves exists twice (items 8385 and 217271, same vendors, same content); the guide ships 8385 (classic ID), noted here so the omission is deliberate.
- Every other Feralas-dropping recipe is a generic world drop (6+ map-zones, up to 370 droppers) — none shipped. Quest-reward recipes are unverifiable from quest records — none shipped. Professions with NO Feralas source: Fishing — stated in the guide, not padded (Dun Morogh Blacksmithing precedent).
