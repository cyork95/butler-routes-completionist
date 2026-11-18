# Feralas (Horde) companions inventory (pack 0.144.0)

Every entry shipped in the two Feralas (Horde) companion guides, one line
each: name, NPC/item id, source type, coordinates or vendor, and the data
source verified against. All coordinates are the client's own (live) map
frame on map 1444 (Feralas). Game data is questie-forever npcs.json,
objects.json and items.json; quest linkage checked against the full quest
table and the 39-quest Horde core contract (`feralas-horde.guide`,
band 38-50). The data carries an explicit `rare` role flag; 12 Feralas NPCs
hold it, all with faction null (no Falthis-style Horde exclusion anywhere).

This inventory mirrors `docs/feralas-companions-inventory.md` with the
vendor-faction rule flipped. Genuine faction differences are stated as
differences, not harmonized; anything the two inventories disagree on is
flagged in `docs/companion-unverified.md`.

## feralas-horde-rares.guide — 9 rares + 1 item-start hunt + 6 fixed containers

- Lady Szallah | npc5343 | level 46 rare | single point (28.2, 67.6), far south | signature: Naga Caster's Staff (item284850), sole dropper in the data; no quest takes it | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Diamond Head | npc5345 | level 45 rare | single point (36.6, 51.41), center | NO sole drop in the data — kill goal + note only | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Bloodroar the Stalker | npc5346 | level 48 rare | single point (52.03, 60.91), south | signature: Yeti Hide Stompers (item285047), sole drop; no quest takes it | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Antilus the Soarer | npc5347 | level 48 rare | single point (55.6, 74.15), south-east | signature: Hippogryph Down Leggings (item284847), sole drop; no quest takes it | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Arash-ethis | npc5349 | level 49 rare | single point (44.79, 25.02), north-center | signature: Windserpent Scaled Cloak (item284866), sole drop; no quest takes it | also drops ordinary greens | NO tame line: the data has no tameability flag, no drop carries pet evidence, and the Horde core guide has no Hunter line referencing this rare (grep for 5349/Arash in `feralas-horde.guide` returns nothing outside the header comment) — candidacy logged in docs/companion-unverified.md | source: npcs.json + items.json + quests.json + feralas-horde.guide
- Qirot | npc5350 | level 47 rare | single point (76.65, 66.24), far east | signature: Silithid Sinew Crossbow (item284859), sole drop; no quest takes it | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Old Grizzlegut | npc5352 | level 43 rare | single point (59.46, 59.44), east | signature: Sturdy Bearhide Leggings (item284843), sole drop; no quest takes it | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Gnarl Leafbrother | npc5354 | level 44 rare | single point (69.24, 57.31), east | NO sole drop in the data — kill goal + note only | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Snarler | npc5356 | level 42 rare | single point (80.22, 39.57), east | signature: Snarling Fang (item285043), sole drop; no quest takes it | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Perfect Yeti Hide hunt | item18972 (starts Horde-contracted quest 7738) | dropped by Rage Scar Yeti npc5296 L46 (8 points, south-center grounds), Elder Rage Scar npc5297 L48, Ferocious Rage Scar npc5299 L47, Lurking Feral Scar npc7848 L46 — the only 4 droppers anywhere in the data | the guide loops the 8-point Rage Scar grounds and names the other three droppers; optional collect + note pointing at the core guide (accept/turnin live in `feralas-horde.guide`) | source: items.json + npcs.json + quests.json
- Old Crate | obj442688 | single point (76.6, 48.0), east | no loot table confirmed | source: objects.json
- Grimtotem Chest | obj443727 | single point (69.6, 43.3), east | no loot table confirmed | source: objects.json
- Old Chest | obj642451 | single point (79.2, 49.35), far east | no loot table confirmed; this is the turn-in object of quest 95599 (The Old Key), which has no accept in the data (start npc/object/item all empty) and is OUT as broken — the chest is real, the quest line is not routed anywhere | source: objects.json + quests.json
- Hippogryph Egg | obj141931 | 9 fixed points (53.66, 74.37), (55.91, 76.03), (56.65, 75.89), (57.01, 78.22), (57.31, 77.35), (57.98, 76.3), (58.27, 76.71), (58.48, 76.11), (58.62, 75.53), south | no quest link and no loot table in the data — shipped as a loop step with contents-unconfirmed note (Deadwind/Shen'dralas precedent for real fixed objects); the Alliance inventory did not evaluate this object — delta flagged in companion-unverified | source: objects.json + quests.json
- Woodpaw Bag | obj443728 | single point (66.4, 50.9), Woodpaw grounds | no quest link and no loot table in the data — shipped single-goto with contents-unconfirmed note; Alliance inventory silent on it — delta flagged | source: objects.json + quests.json
- Extraplanar Eye | obj445041 | single point (57.2, 68.8) | no quest link and no loot table in the data — shipped single-goto with contents-unconfirmed note; Alliance inventory silent on it — delta flagged | source: objects.json + quests.json

Argued exclusions:
- Above-band rares (Westfall/Hillsbrad precedent — excluded, Dire Maul area, far above the 38–50 band): Mushgog npc11447 L60 (62.5, 30.0; sole drop Black Lotus item13468 — logged below), The Razza npc11497 L60 (62.5, 29.9; no sole drop), Skarr the Unbreakable npc11498 L58 (62.5, 30.37; no sole drop).
- Quest-target lookalikes WITHOUT the data flag: Lord Shalzaru npc8136 L47 (2870 objective), Woodpaw Alpha npc5258 L43, Gordunni Shaman/Warlock/Ogre Mage/Mage-Lord npc5236/5240/5237/5239 (2982 objectives), Ohk'zi (92858 objective mob). None is flagged rare; none has loot of its own beyond its quest role. Data wins over community memory.
- Quest-owned objects: Shay's Chest (obj144054, at Shay's camp — 2845 Wandering Shay's furniture; 2845 is Alliance-only mask 4294967373, so doubly out for a Horde guide), the WANTED! poster (obj581918, furniture of Alliance-only quest 92858), the Tear of Theradras (obj22246, turn-in-adjacent object of the level-60 neutral writ 94308 at the dungeon mouth — out-of-band writ object, not companion content). None is companion content.
- Gordunni Scroll object (obj143980, 3 points (74.52, 27.9), (75.13, 29.73), (80.55, 34.29)): name-matches the start item (item9370) of Horde-contracted quest 2978, which has NO mob droppers anywhere — but the data carries no object-to-item link, so shipping it as the source would be a guess. The core guide routes 2978 as sourceless (bag note) and stays the authority. No step shipped; hypothesis logged in docs/companion-unverified.md.
- Probable quest furniture with no data link, not shippable as clean treasure: the three Twilight Tablet Fragment objects (no quest refs in this build), the three Gordunni Cauldrons (flavor/ritual, no refs). Stated, not shipped.
- Flavor/furniture surveyed but not shipped: mailboxes, Burning Embers, braziers, torches, doors, Moonwells, campfires, books/notes singles — no container or loot evidence in the data.
- Seasonal/event (never companion content): the Hallow's End set (pumpkins, candy, eggs) and the Midsummer set (MFF objects at Feathermoon and Camp Mojache).
- Resource nodes (herbs, veins, fishing pools): never treasure content in this pack — not shipped.
- No Horde contract quest has any of the 9 shipped rares as giver, ender, or kill objective (all 39 checked; every quest-linkage hit list is empty). No signature is a quest objective anywhere in the data (all 7 checked).
- Tame lines: none shipped. The data has no tameability flag on any Feralas rare and the Horde core guide carries no tame corroboration. Arash-ethis logged in docs/companion-unverified.md instead of shipped as fact.

## feralas-horde-recipes.guide — 16 vendor-sold + 11 in-zone drops

Vendor-sold (buy from the Horde vendor named, npc-pinned; Alliance twin-sellers noted where the data shows them):
- Pattern: Green Whelp Bracers | item7451 | buy from Jangdor Swiftstrider, npc7854 [H], (74.43, 42.91) Camp Mojache (also sold by Alliance vendor Pratt) | Leatherworking | source: items.json vendors
- Pattern: Turtle Scale Gloves | item8385 | buy from Jangdor [H] (also Alliance-sold; also a 370-dropper world drop — the vendor source is the shipped one) | Leatherworking | source: items.json vendors
- Pattern: Nightscape Shoulders | item8409 | buy from Jangdor [H] ONLY — no Alliance source anywhere in the data (genuine Horde gain; the Alliance inventory logged it as Horde-exclusive) | Leatherworking | source: items.json vendors
- Pattern: Living Shoulders | item15734 | buy from Jangdor [H] (also Alliance-sold) | Leatherworking | source: items.json vendors
- Pattern: Rugged Armor Kit line, 5 items (252783, 252784, 252811, 252812, 252942) | buy from Jangdor [H] ONLY — no Alliance source anywhere in the data (genuine Horde gain) | Leatherworking | source: items.json vendors
- Recipe: Nature Protection Potion | item6057 | buy from Bronk, npc8158 [H], (76.06, 43.28) Camp Mojache (also Alliance-sold) | Alchemy | source: items.json vendors
- Recipe: Ghost Dye | item9302 | buy from Bronk [H] (also Alliance-sold) | Alchemy | source: items.json vendors
- Recipe: Hot Wolf Ribs | item12229 | buy from Sheendra Tallgrass, npc8145 [H], (74.49, 42.73) Camp Mojache (also Alliance-sold) | Cooking | source: items.json vendors
- Recipe: Lobster Stew | item13947 | buy from Sheendra [H] (also Alliance-sold) | Cooking | source: items.json vendors
- Recipe: Mightfish Steak | item13948 | buy from Sheendra [H] (also Alliance-sold) | Cooking | source: items.json vendors
- Recipe: Baked Salmon | item13949 | buy from Sheendra [H] (also Alliance-sold) | Cooking | source: items.json vendors
- Schematic: Snake Burst Firework | item19027 | buy from Zorbin Fandazzle, npc14637 [AH neutral], (44.81, 43.42) center | Engineering | source: items.json vendors

Drops (in-zone droppers; every one a sole dropper in the data unless noted):
- Formula: Enchant 2H Weapon - Lesser Strength | item249513 | collect from the Hatecrest Sorceress, npc5336 (L43) — sole dropper anywhere | Enchanting | source: items.json drops
- Recipe: Triage Tea | item249882 | collect from the Woodpaw Mystic, npc5254 (L42) — sole dropper | First Aid | source: items.json drops
- Recipe: Superior Frenzy Potion | item250986 | collect from the Northspring Roguefeather, npc5363 (L48) — sole dropper | Alchemy | source: items.json drops
- Plans: Mithril Claymore | item251462 | collect from the Woodpaw Mongrel, npc5249 (L40) — sole dropper | Blacksmithing | source: items.json drops
- Plans: Charged Mithril Battleaxe | item251464 | collect from the Gordunni Brute, npc5232 (L42) — sole dropper | Blacksmithing | source: items.json drops
- Pattern: Charged Scorpid Belt | item252909 | collect from the Rage Scar Yeti, npc5296 (L46) — sole dropper | Leatherworking | source: items.json drops
- Pattern: Supple Scorpid Bracers | item252916 | collect from the Groddoc Thunderer, npc5262 (L49) — sole dropper | Leatherworking | source: items.json drops
- Pattern: Earthen Leggings | item254000 | collect from the Gravelsnout Surveyor, npc4116 (L29, single 1444 point (91.9, 49.0)) — sole dropper; the mob also spawns on 1441, noted honestly (below-band source, trivial at Horde levels) | Tailoring | source: items.json drops + npcs.json
- Pattern: Earthenweave Boots | item254094 | collect from the Elder Rage Scar, npc5297 (L48) — sole dropper | Tailoring | source: items.json drops
- Pattern: Stormcloth Boots | item254686 | collect from the Hatecrest Serpent Guard, npc5333 (L44) — sole dropper | Tailoring | source: items.json drops
- Manual: Superior Healing Potion | item255725 | collect from the Gordunni Shaman, npc5236 (L44) — sole dropper | First Aid | source: items.json drops

Argued exclusions:
- Alliance-vendor-exclusive (Alterac precedent, flipped — Horde guide): Pattern: Azure Silk Cloak (item7089), Pattern: Linen Reagent Bag (item253665), Pattern: Woolen Reagent Bag (item253668), sold ONLY by Brienna Starglow [A]. No Horde source in the data. Genuine faction gap: Horde Tailoring has NO vendor source in Feralas — stated in the guide, not padded.
- Duplicate record: Pattern: Turtle Scale Gloves exists twice (items 8385 and 217271, same vendors, same content); the guide ships 8385 (classic ID), mirroring the Alliance inventory's deliberate omission.
- Narrow-but-generic: Plans: Searing Golden Blade (item12261, 26 droppers) — not narrow enough to be zone content. Formula: Scroll of Spatial Mending (item223163, 4 Fel Interloper droppers across 9 zone keys, no assignable profession) — multi-zone family, excluded with reason.
- Above-band/out-of-reach drops: Pattern: Bottomless Bag (item14510, single in-zone dropper Dreamroarer L62 world boss, 5 zones) and Plans: Sageblade (item22389, in-zone droppers the 4 Emerald Dragons L63, 5 zones). Logged, never shipped.
- Every other Feralas-dropping recipe is a generic world drop (6+ map-zones, up to 370 droppers) — none shipped. Quest-reward recipes are unverifiable from quest records — none shipped.
- Professions with NO Feralas Horde source: Fishing — stated in the guide, not padded (Dun Morogh Blacksmithing precedent). Enchanting has no vendor (Quintis Jonespyre [A] sells goods, not recipes — verified stock 11020/11022) but HAS the 249513 drop, so it is covered, not no-source. Tailoring has drops but no vendor (above).
