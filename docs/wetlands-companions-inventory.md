# Wetlands companions inventory (pack 0.43.0)

Every entry shipped in the two Wetlands companion guides, one line each:
name, NPC/item id, source type, coordinates or vendor, and the data source
verified against. All coordinates are the client's own (live) map frame on
map 1437 (Wetlands). Game data is questie-forever npcs.json, objects.json
and items.json; quest linkage checked against the full quest table and the
87-quest core contract (`wetlands.guide`). The data carries an explicit
`rare` role flag; 8 Wetlands NPCs hold it. Band cutoff: the core band is
20–30.

## wetlands-rares.guide — 8 rares + fixed world containers

- Ma'ruk Wyrmscale | npc2090 | level 23 rare | single point (48.06, 74.7), south | signatures: Scythe Axe (item5749) + Warchief's Girdle (item5750), both sole drops; no quest takes either | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Leech Widow | npc1112 | level 24 rare | single point (47.27, 59.22), south-center | signatures: Black Husk Shield (item4444) + Black Widow Band (item6199), both sole drops; no quest takes either | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Gnawbone | npc14425 | level 24 rare | loop over 6 points (30.08, 30.74) … (38.89, 34.13), north-center | signature: Gnawed Bone (item282654), sole drop; no quest takes it | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Mirelow | npc14424 | level 25 rare | loop over 21 points (16.0, 31.8) … (27.52, 32.48), north-west marsh | signature: Bog Pickers (item282655), sole drop; no quest takes it | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Garneg Charskull | npc2108 | level 29 rare | single point (38.42, 46.06), center | signatures: Ringed Helm (item3392) + Garneg's War Belt (item6200), both sole drops; no quest takes either | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Dragonmaw Battlemaster | npc1037 | level 30 rare | single point (45.34, 44.41), center — band top, no come-back note needed | signature: Dragonmaw Battle Shroud (item282658), sole drop; no quest takes it | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Sludginn | npc14433 | level 30 rare | single point (12.62, 67.5), far west — band top, no come-back note needed | signature: Dissolved Locket (item282653), sole drop; no quest takes it | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Razormaw Matriarch | npc1140 | level 31 rare, ONE OVER BAND — shipped with an honest come-back-later note | single point (69.93, 29.22), east | signatures: Beaded Raptor Collar (item4463) + Jurassic Wristguards (item6198), both sole drops; no quest takes either | also drops ordinary greens | source: npcs.json + items.json + quests.json
- Fixed world containers | obj2850 (Solid Chest, 27 pts) + obj2852 (Solid Chest, 13 pts) + obj3659/obj3695 (Barrel of Melon Juice + Food Crate, 46 shared pts) + obj19018 (Giant Clam, 23 pts) + obj179486/obj179488 (Battered Footlocker, 11 + 8 pts) | four loop steps, 40 + 46 + 23 + 19 unique points; the two same-name Footlocker objects loop together (Darkshore precedent) | ordinary low-level goods | source: objects.json
- Unique containers | obj259 Half-buried Barrel (13.94, 34.81), north-west | obj261 Damaged Crate (13.52, 41.38), north-west | obj2734 Waterlogged Chest (12.11, 64.19), west | obj112948 Intrepid's Locked Strongbox (14.38, 24.04), north-west | obj142151 Sealed Barrel (13.6, 38.22), north-west | each its own step | source: objects.json

Argued exclusions:
- No above-band exclusions: the highest flagged rare is L31, shipped with a note. No classic-name lookalikes carry the flag without being flagged — the zone's named quest mobs (Balgaras the Foul npc1364, Captain Halyndor npc1160) are roles=undefined and stay out as quest/dropper NPCs, not rares.
- Quest-owned objects: none of the fixed containers is a core-contracted objective (all 87 checked).
- Flavor surveyed but not shipped: Mailbox obj142094 (Menethil), no container or loot in the data.
- Tame lines: none shipped. The data has no tameability flag and the core guide carries no tame/task lines at all. All logged in docs/companion-unverified.md instead of shipped as fact.

## wetlands-recipes.guide — 12 vendor-sold + 4 in-zone drops

Vendor-sold (all vendors Alliance; profession from the item-name convention):
- Pattern: Red Woolen Bag | item5772 | buy from Jennabink Powerseam, npc1454 [A], (8.12, 55.84) Menethil Harbor | Tailoring | source: items.json vendors
- Pattern: Greater Adept's Robe | item6275 | buy from Jennabink Powerseam [A] (same) | Tailoring | source: items.json vendors
- Pattern: Linen Reagent Bag | item253665 | buy from Jennabink Powerseam [A] (same) | Tailoring | source: items.json vendors
- Pattern: Woolen Reagent Bag | item253668 | buy from Jennabink Powerseam [A] (same) | Tailoring | source: items.json vendors
- Recipe: Rainbow Fin Albacore | item6368 | buy from Stuart Fleming, npc3178 [A], (8.02, 58.35) Menethil Harbor | Cooking | source: items.json vendors
- Recipe: Rockscale Cod | item6369 | buy from Stuart Fleming [A] (same) | Cooking | source: items.json vendors
- Recipe: Mithril Head Trout | item17062 | buy from Stuart Fleming [A] (same) | Cooking | source: items.json vendors
- Pattern: Azure Silk Gloves | item7114 | buy from Wenna Silkbeard, npc2679 [A], (25.61, 25.8) Dun Modr | Tailoring | source: items.json vendors
- Pattern: Red Whelp Gloves | item7290 | buy from Wenna Silkbeard [A] (same) | Leatherworking | source: items.json vendors
- Pattern: Green Leather Armor | item7613 | buy from Wenna Silkbeard [A] (same) | Leatherworking | source: items.json vendors
- Schematic: Lovingly Crafted Boomstick | item13309 | buy from Fradd Swiftgear, npc2682 [A], (26.4, 25.76) Dun Modr | Engineering | source: items.json vendors
- Schematic: Minor Recombobulator | item14639 | buy from Fradd Swiftgear [A] (same) | Engineering | source: items.json vendors

Drops (in-zone droppers; multi-zone ones noted honestly):
- Pattern: Thick Murloc Armor | item5788 | collect from Captain Halyndor, npc1160 (L30, (15.45, 23.61)) — 2 zones [1434, 1437] (other dropper Kurzen Commando in Stranglethorn), noted honestly | Leatherworking | source: items.json drops
- Formula: Enchant Gloves - Mining | item11150 | collect from the Dark Iron clan, Dun Modr (npc1051 L27, npc1052 L28, npc1053 L29, npc1054 L30; (45.65–48.01, 14.73–18.74)) — 2 zones [1417, 1437] (also Arathi), noted honestly; the fifth listed dropper (Balgaras L34) is above-band and not routed | Enchanting | source: items.json drops
- Recipe: Tasty Raptor Bites | item250187 | collect from the Mottled Raptor, npc1020 (L22, (19.77, 52.47), (20.72, 48.8), (21.37, 51.91)) — 2 zones [1413, 1437] (other dropper L13 in Durotar), noted honestly | Cooking | source: items.json drops
- Schematic: SAF-T Jumbo Dynamite | item264208 | collect from the Dark Iron Demolitionist, npc1054 (L30, (46.5, 18.74), (47.39, 14.99), (47.57, 14.73)) — SOLE ZONE [1437]; the second listed dropper (Dragonmaw Saboteur npc275045) has no spawn points in the data, noted | Engineering | source: items.json drops

Every other Wetlands-dropping recipe drops in 6+ map-zones (generic world drops, Elwynn rule) — none shipped. Quest-reward recipes are unverifiable from quest records — none shipped. Professions with NO Wetlands source: Blacksmithing, First Aid, Fishing — stated in the guide, not padded (Dun Morogh Blacksmithing precedent).

Argued exclusions:
- No Horde-vendor exclusions: every in-zone recipe vendor is Alliance.
