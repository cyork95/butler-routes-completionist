# Dustwallow Marsh companions inventory (pack 0.39.0)

Every entry shipped in the two Dustwallow Marsh companion guides, one line
each: name, NPC/item id, source type, coordinates or vendor, and the data
source verified against. All coordinates are the client's own (live) map
frame on map 1445 (Dustwallow Marsh). Game data is questie-forever npcs.json,
objects.json and items.json; quest linkage checked against the full quest
table and the 45-quest core contract (`dustwallow.guide`). The data carries
an explicit `rare` role flag; 12 Dustwallow NPCs hold it. Band cutoff: the
core band is 35–45.

## dustwallow-rares.guide — 10 rares + fixed world containers

- Brimgore | npc4339 | level 45 rare (band top) | single point (42.12, 75.94), far south | signature: Black Brood Battleguards (item285063, sole dropper anywhere) | no quest linkage (not a giver/ender/objective of any contract quest; its drop 6444 Forked Tongue is a different item from the core 1204 objective 5883) | source: npcs.json + items.json + quests.json
- Darkmist Widow | npc4380 | level 40 rare | single point (31.15, 20.4), west | signature: Darkmist Dirk (item285102, sole dropper) | also drops Unpopped Darkmist Eye (5884, the core 1206 objective — the hunt lives in the core guide, noted, never accepted here) | source: npcs.json + items.json + quests.json
- Burgle Eye | npc14230 | level 38 rare | single point (59.04, 9.37), north-east shore | signature: Twitching Eye (item285095, sole dropper; no quest takes it in the data) | source: npcs.json + items.json + quests.json
- Drogoth the Roamer | npc14231 | level 37 rare | single point (39.5, 18.92), west | signature: Swamp Roamer's Band (item285089, sole dropper; no quest takes it) | source: npcs.json + items.json + quests.json
- Dart | npc14232 | level 38 rare | single point (47.27, 18.38), west | signatures: Serrated Raptor Teeth (item285100) + Serrated Axes (item285283), both sole-dropped; no quest takes either | source: npcs.json + items.json + quests.json
- Ripscale | npc14233 | level 39 rare | loop over 5 points (37.8, 50.29), (42.35, 55.0), (44.08, 50.17), (47.26, 54.65), (49.06, 57.33), south-center | no sole drops — ordinary greens get a note, not a goal | source: npcs.json + items.json + quests.json
- Hayoc | npc14234 | level 41 rare | single point (52.02, 62.87), south | signature: Marsh Serpent's Scales (item285103, sole dropper; no quest takes it) | source: npcs.json + items.json + quests.json
- The Rot | npc14235 | level 43 rare | single point (52.9, 57.4), south | signature: Rot-Fused Greaves (item285101, sole dropper; no quest takes it) | source: npcs.json + items.json + quests.json
- Lord Angler | npc14236 | level 44 rare | single point (57.83, 61.62), south-east | signature: Ravaged Fishing Pole (item285094, sole dropper; a fishing pole, noted as flavor) | source: npcs.json + items.json + quests.json
- Oozeworm | npc14237 | level 42 rare | loop over 3 points (34.95, 70.86), (36.03, 63.07), (39.12, 63.05), far south | no sole drops — ordinary greens get a note | source: npcs.json + items.json + quests.json
- Fixed world containers | obj2857 (Solid Chest, 12 pts) + obj4149 (Solid Chest, 19 pts) + obj3714/obj3715 (Alliance Strongbox/Chest, 3 shared pts) + obj111095 (Alliance Chest, 1 pt) + obj20925 (Captain's Footlocker, 1 pt — the bookshelf, shipped in the loop, said plainly) + obj153470 (Food Crate, 8 pts) + obj3707 (Food Crate, 14 pts) + obj3702/obj3689/obj3695 (Armor/Weapon/Food Crate cluster, 8 unique pts) + obj3662/obj3705 (Food Crate + Barrel of Milk, 1 shared pt) + obj174728 (Damaged Crate, 1 pt) | one loop step, 68 unique points, ordinary low-level goods | source: objects.json
- Unique treasures | obj3646 General Twinbraid's Strongbox (26.3, 58.5), west | obj19904/19905/19906 Mok'Morokk's Snuff/Grog/Strongbox (44.53, 66.04), (38.66, 65.57), (36.64, 69.57), ogre mound | obj2871/2872 Seaworn Altar + Enchanted Sea Kelp (59.36, 9.63)/(59.35, 9.6), east coast | obj21128 Orc Spy Report (68.18, 48.63), Theramore (noted, no loot in the data) | each its own step or note | source: objects.json

Argued exclusions:
- Malgin Barleybrew (npc5848, L25) + Captain Gerogg Hammertoe (npc5851, L27): both hold the rare flag but are faction=A (Alliance-friendly; Malgin is also a vendor). An Alliance player cannot kill them — not companion content. Below band either way.
- Quest-owned singletons: Egg of Onyxia (obj20359, 6 pts) is the objective of the Horde quest 1172; the Black Shield (obj20992), Theramore Guard Badge (obj21042), Musty Scroll (obj2555) and Waterlogged Book (obj423900) START quests (1253/1251, 1252/1269, 626, 79952); the Barrel of Sweet Nectar (obj3706) starts Hillsbrad quest 551, so its 7 points ship only via the overlapping Food Crate obj3707. None is companion loot.
- Flavor markers with no container/loot in the data (surveyed, not shipped): Hyal Family Monument (obj186322), Grave (obj424264), Wanted Poster (obj186426); herb/ore veins, campfires, chairs, anvils, flight-point and instance-portal objects are not treasure.
- Rares above the core band (35–45): none — the highest-flagged rare is exactly 45 (Brimgore), shipped.
- No contract quest has any of the 10 shipped rares as giver, ender, or kill/objective (all 45 checked). The Darkmist Widow's shared drop (5884) is a source note, not quest ownership.
- Tame lines: none shipped. The data has no tameability flag; beast-family evidence exists for some (Widow spider silk/mandible drops) but the core guide carries no tame corroboration (no Hunter taming chain in the 45-contract). All logged in docs/companion-unverified.md instead of shipped as fact.

## dustwallow-recipes.guide — 4 vendor-sold + 5 single/dual-zone drops

Vendor-sold (profession from the item-name convention — no profession flag exists in the data; listed vendors spawn on map 1445 and are Alliance-faction):
- Pattern: Murloc Scale Bracers | item5789 | buy from Helenia Olden, npc4897, (66.44, 51.46) Theramore | Leatherworking (scale bracers) | source: items.json vendors
- Recipe: Roast Raptor | item12228 | buy from Helenia Olden (also sold by Horde vendor Ogg'marr — the Alliance source is the shipped one) | Cooking (raptor roast) | source: items.json vendors
- Recipe: Mystery Stew | item12233 | buy from Helenia Olden | Cooking (stew) | source: items.json vendors
- Recipe: Dragonbreath Chili | item12239 | buy from Helenia Olden (also Horde-sold) | Cooking (chili) | source: items.json vendors

Drops (sole-zone droppers genuinely in-zone, or a dual-zone dropper with dense in-zone spawns — the Westfall/Shafety honest-note handling where noted):
- Plans: Mithril Shortsword | item251459 | collect from the Mirefin Coastrunner, npc4362 (L36, 2 in-zone points (53.96, 15.18), (54.19, 15.66)) — the SOLE dropper anywhere (sole zone 1445) | Blacksmithing (Plans + metal weapon basis) | source: items.json drops
- Pattern: Earthen Silk Cuffs | item254020 | collect from the Mirefin Murloc, npc4359 (L35, (53.78, 15.15), (54.19, 15.66)) — sole dropper, sole zone | Tailoring (silk basis) | source: items.json drops
- Pattern: Stormcloth Headband | item254684 | collect from the Firemane Flamecaller, npc4334 (L43, (48.16, 76.29), (48.54, 73.17)) — sole dropper, sole zone | Tailoring (cloth basis) | source: items.json drops
- Formula: Enchant 2H Weapon - Lesser Agility | item249511 | collect from the Firemane Scout, npc4329 (L41, 52 in-zone points (36.8–51, 64–82), far south) — sole dropper, also drops in the Barrens (noted honestly) | Enchanting (Formula basis) | source: items.json drops
- Recipe: Raptor Rouladen | item250184 | collect from the Bloodfen Lashtail, npc4357 (L40, 15 in-zone points (31–38, 64–72)) — sole dropper, also drops in the Barrens (noted honestly) | Cooking (raptor basis, Alterac Raptor Rouladen pattern) | source: items.json drops

Every other Dustwallow-dropping recipe drops in 4+ map-zones (generic world drops, Elwynn rule) — none shipped. Quest-reward recipes are unverifiable from quest records — none shipped. Professions with NO Dustwallow source: Engineering, First Aid, Fishing, Alchemy — stated in the guide, not padded (Dun Morogh Blacksmithing precedent).

Argued exclusions:
- Horde-vendor-exclusive in-zone recipes (in-zone vendor is Horde-faction — never shipped on a guess, Alterac precedent): Pattern: Icy Cloak (item4355, Ghok'kah); Recipe: Carrion Surprise (item12232, Ogg'marr); Manual: Heavy Silk Bandage + Manual: Mageweave Bandage (items 16112/16113, Balai Lok'Wein); Recipe: Heavy Crocolisk Stew (item20075, Ogg'marr); Pattern: Linen Reagent Bag + Pattern: Woolen Reagent Bag (items 253665/253668, Ghok'kah on 1445 — the Alliance sources live on other maps including Moonglade 1450, another round's business).
