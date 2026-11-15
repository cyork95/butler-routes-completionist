# Hillsbrad companions inventory (pack 0.29.0)

Every entry shipped in the two Hillsbrad Foothills companion guides, one line
each: name, NPC/item id, source type, coordinates or vendor, and the data source
verified against. All coordinates are the client's own (live) map frame on map
1424 (Hillsbrad Foothills). Game data is questie-forever npcs.json, items.json
and objects.json; quest linkage checked against the full quest table and the
37-quest core contract (`hillsbrad.guide`). The data carries explicit `rare`
role flags; 11 Hillsbrad NPCs hold the flag. Band cutoff: the core contract
band is 20-32, and the cutoff is drawn at 32 — everything above it is
out-of-band world content (the Westfall precedent).

## hillsbrad-rares.guide — 7 rares + fixed world containers

- Dalaran Spellscribe | npc1920 | level 21 rare humanoid caster, flagged rare in the data | single point (8.9, 23.8), the far west by the Dalaran crater | signature drops item4436 Jewel-encrusted Sash, item4437 Channeler's Staff (each dropped by nothing else) | source: npcs.json + items.json
- Tamra Stormpike | npc14275 | level 28 rare (rank 2 record, but role-flagged rare), flagged rare in the data | loop over 3 points (70.68, 78.05), (72.31, 82.34), (73.25, 81.09), the southeastern hills | signature drop item282710 Dun Garok Rifle (dropped by nothing else) | source: npcs.json + items.json
- Scargil | npc14276 | level 30 rare murloc (drops Tangy Clam Meat), flagged rare in the data; not tameable | single point (29.08, 73.56), the southwest shore | signature drop item282716 Imbued Scaled Cuffs (dropped by nothing else) | source: npcs.json + items.json
- Ro'Bark | npc14278 | level 28 rare gnoll (drops the Gnoll Shaman's Staff; humanoid), flagged rare in the data; not tameable | single point (65.72, 60.15), the eastern gnoll country | signature drop item282721 Gnoll Shaman's Staff (dropped by nothing else) | source: npcs.json + items.json
- Creepthess | npc14279 | level 24 rare spider (drops Crisp Spider Meat and Spider's Silk), flagged rare in the data | single point (38.6, 58.37), the western fields | signature drop item282720 Spider Swarm (dropped by nothing else) | source: npcs.json + items.json
- Big Samras | npc14280 | level 27 rare bear (drops Big Bear Meat; wears the Bearhide Pauldrons), flagged rare in the data | single point (86.03, 39.93), the Dun Garok approach, far east | signature drop item282717 Durable Bearhide Pauldrons (dropped by nothing else) | source: npcs.json + items.json
- Jimmy the Bleeder | npc14281 | level 23 rare, flagged rare in the data | single point (60.1, 9.1), the northern hills | signature drop item282713 Bloodstained Pants (dropped by nothing else) | source: npcs.json + items.json
- Fixed Chests — world containers | obj2039 (Hidden Strongbox, 7 pts) + obj2850/obj2852/obj2855 (Solid Chest, 4+6+8 pts) + obj3659 (Barrel of Melon Juice, 33 pts) + obj3694/obj3695/obj153470 (Food Crate, 5+33+6 pts) + obj3705 (Barrel of Milk, 5 pts) + obj3715/obj4096/obj105579/obj111095 (Alliance Chest, 7+5+4+10 pts) + obj105570 (Alliance Strongbox, 4 pts) + obj103815 (Ambermill Strongbox, 1 pt) + obj179486/obj179488 (Battered Footlocker, 10+8 pts at the Syndicate camp) + obj181302 (Camp Crate, 2 pts) + obj181620 (Unopened Crate, 1 pt) | one loop step, 159 fixed points, all ordinary low-level goods; no unique treasure confirmed (the Ambermill Strongbox is a single-point generic strongbox, not a unique) | source: objects.json
- No contract quest in the 37 has object-type objectives except 8373 (Forsaken Stink Bomb, routed in the core guide), so none of the shipped containers is quest-owned. No rare is a giver, ender, or objective of any contract quest (checked all 37 start/end records against the 11 rare ids).

Argued exclusions:
- Above the level-32 cutoff (out-of-band world content, Westfall precedent): Narillasanz (npc2447, lvl 44, 1 pt at 73.3, 5.6 — Mark of the Red Flight), Old Cliff Jumper (npc8211, lvl 42, 1 pt at 96.9, 14.6, no exclusive loot), Araga (npc14222, lvl 35, 1 pt at 35.3, 11.5 — Denmother's Hide), Lady Zephris (npc14277, lvl 33, 1 pt at 64.53, 79.71 — Naga Maiden's Gown).
- Tame lines: none shipped. Creepthess (spider: Crisp Spider Meat + Spider's Silk) and Big Samras (bear: Big Bear Meat + Bearhide Pauldrons) have drop evidence for beast type, but the core guide carries no tame lines or references to any of these rares, so the corroboration half of the rule is unmet — logged in docs/companion-unverified.md instead of shipped as fact. All other shipped rares are humanoid-caster, dwarf, murloc, or gnoll shapes, or item-only humanoids (Dalaran Spellscribe, Tamra Stormpike, Jimmy the Bleeder).

## hillsbrad-recipes.guide — 25 vendor-sold + 4 exclusive drops

Vendor-sold (profession from the item-name convention: Pattern-cloth = Tailoring, Pattern-leather = Leatherworking, Plans = Blacksmithing, Schematic = Engineering, Formula = Enchanting, Recipe food/fish/tea = Cooking, Recipe potion/elixir = Alchemy — the same basis as the earlier companions; no profession flag exists in the data):
- Pattern: Icy Cloak | item4355 | buy from Micha Yance, npc2381, Southshore (48.94, 55.03) | Tailoring | source: items.json vendors
- Pattern: Thick Murloc Armor | item5788 | buy from Micha Yance, npc2381 (also sold by Christoph Jeffcoat, npc2393) | Tailoring | source: items.json vendors
- Pattern: Red Woolen Bag | item5772 | buy from Zixil, npc3537 (55.38, 34.71) | Tailoring | source: items.json vendors
- Pattern: Blue Overalls | item6274 | buy from Mallen Swain, npc2394, north shore (61.9, 20.98) | Tailoring | source: items.json vendors
- Pattern: Dark Silk Shirt | item6401 | buy from Mallen Swain, npc2394 | Tailoring | source: items.json vendors
- Pattern: Linen Reagent Bag | item253665 | buy from Mallen Swain, npc2394 | Tailoring | source: items.json vendors
- Pattern: Woolen Reagent Bag | item253668 | buy from Mallen Swain, npc2394 | Tailoring | source: items.json vendors
- Recipe: Shadow Protection Potion | item6054 | buy from Christoph Jeffcoat, npc2393, north shore (62.29, 19.04) | Alchemy | source: items.json vendors
- Recipe: Fire Protection Potion | item6055 | buy from Nandar Branson, npc2380, Southshore (50.93, 57.1) | Alchemy | source: items.json vendors
- Recipe: Elixir of Coalesced Regret | item210709 | buy from Zixil, npc3537 | Alchemy | source: items.json vendors
- Recipe: Bristle Whisker Catfish | item6330 | buy from Lindea Rabonne, npc2383, Southshore shore (50.63, 60.95) | Cooking | source: items.json vendors
- Recipe: Rockscale Cod | item6369 | buy from Lindea Rabonne, npc2383 | Cooking | source: items.json vendors
- Recipe: Mithril Head Trout | item17062 | buy from Lindea Rabonne, npc2383 | Cooking | source: items.json vendors
- Recipe: Smoked Sagefish | item21099 | buy from Micha Yance, npc2381 (also sold by Derak Nightfall, npc2397) | Cooking | source: items.json vendors
- Recipe: Sagefish Delight | item21219 | buy from Micha Yance, npc2381 (also sold by Derak Nightfall, npc2397) | Cooking | source: items.json vendors
- Recipe: Tender Wolf Steak | item18046 | buy from Truk Wildbeard, npc4782, far east (99.8, 0.9) | Cooking | source: items.json vendors
- Recipe: Thistle Tea | item18160 | buy from Smudge Thunderwood, npc6779, east (84.2, 18.1) | Cooking | source: items.json vendors
- Formula: Enchant Boots - Minor Agility | item6377 | buy from Zixil, npc3537 | Enchanting | source: items.json vendors
- Formula: Enchant Bracer - Lesser Deflection | item11163 | buy from Micha Yance, npc2381 | Enchanting | source: items.json vendors
- Pattern: Green Leather Armor | item7613 | buy from George Candarte, npc2698, east (92.02, 38.23) | Leatherworking | source: items.json vendors
- Pattern: Earthen Leather Shoulders | item7362 | buy from Zixil, npc3537 | Leatherworking | source: items.json vendors
- Pattern: Nightscape Shoulders | item8409 | buy from Nioma, npc8160, far east (98.5, 2.2) | Leatherworking | source: items.json vendors
- Schematic: Goblin Jumper Cables | item7561 | buy from Zixil, npc3537 | Engineering | source: items.json vendors
- Schematic: Gnomish Cloaking Device | item7742 | buy from Zan Shivsproket, npc6777, east (84.1, 18.4) | Engineering | source: items.json vendors
- Plans: Mithril Scale Bracers | item7995 | buy from Harggan, npc8161, far east (98.7, 3.1) | Blacksmithing | source: items.json vendors

Exclusive drops (sole dropper anywhere in the data, genuinely Hillsbrad content):
- Recipe: Root Tea | item249881 | collect from the Torn Fin Oracle, npc2376 (level 30, 20 confirmed points on the southwest shore, bbox 35.7-48.3, 63.0-72.8) — the SOLE dropper anywhere | Cooking (name basis: tea, by analogy with Thistle Tea) | source: items.json drops
- Plans: Sterling Silver Boots | item251335 | collect from the Syndicate Watchman, npc2261 (level 20, Syndicate camp points) — the SOLE dropper anywhere | Blacksmithing | source: items.json drops
- Plans: Hard Gold Pauldrons | item251391 | collect from the Crushridge Ogre, npc2252 (level 34, 6 points at the far-north Alterac edge) — the SOLE dropper anywhere, but the mob outlevels the band: the step says to come back at high level (Westfall Shafety Sheep precedent) | Blacksmithing | source: items.json drops
- Schematic: Unsanctified Grenade | item284870 | collect from the Crushridge Warmonger, npc2287 (level 39, 1 point at the far-north Alterac edge) — the SOLE dropper anywhere, but the mob outlevels the band: come back at high level | Engineering | source: items.json drops

Every other Hillsbrad-dropping recipe drops across dozens to hundreds of zones (generic world drops, Elwynn rule) — none shipped. Quest-reward recipes are unverifiable from quest records — none shipped. Professions with NO Hillsbrad source: First Aid and Fishing — stated in the guide, not padded (Dun Morogh Blacksmithing precedent).

Profession gates use `when skill <Profession> 1` (supported by the format); stock class (limited vs unlimited) is not in the local data, so no recipe is marked limited.
