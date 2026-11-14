# Loch Modan companions inventory (pack 0.12.0)

Every entry shipped in the two Loch Modan companion guides, one line each: name,
NPC/item id, source type, coordinates or vendor, and the data source verified
against. All coordinates are the client's own (live) map frame on map 1432 (Loch
Modan). Game data is questie-forever npcs.json, items.json and objects.json;
quest linkage checked against the full quest table and the core guide text. The
data carries explicit `rare` role flags on seven Loch Modan NPCs, which settle
most true-rare calls.

## loch-modan-rares.guide — 10 rares + the Carved Figurine + fixed world containers

- Grizlak | npc1425 | level 15 rare, flagged rare in the data | single point (34.58, 27.07), the northwest | signature drops item2284 Rat Cloth Cloak, item6195 Wax-polished Armor (each dropped by nothing else) | source: npcs.json + items.json
- Large Loch Crocolisk | npc2476 | level 22 rare crocolisk (his drops are crocolisk meat, skins, scales and tears; not tameable), flagged rare in the data | loop over 2 points, the Loch (58.9, 31.07) and (60.3, 39.59) | signature drops item3563 Seafarer's Pantaloons, item6197 Loch Croc Hide Vest (each dropped by nothing else) | source: npcs.json + items.json
- Kackle | npc210107 | level 15 rare (not rare-flagged, but a distinct named record with 24 confirmed points and no quest, vendor or family-twin link — the Elwynn Rumbler shape) | loop over 24 points, the eastern shore (bbox 49.4-60.8, 42.3-60.9) | no unique loot; his pack holds a sniper's rune, a scroll, waylaid crates and pristine leather | source: npcs.json + items.json
- Shanda the Spinner | npc14266 | level 19 rare spider (her drops are spider meat, venom sacs, venom and ichor), flagged rare in the data | single point (78.09, 52.35), the east | signature drop item282636 Silkspun Gloves (dropped by nothing else), so hunters get an `only Hunter` tame line | source: npcs.json + items.json
- Emogg the Crusher | npc14267 | level 19 rare, flagged rare in the data | single point (73.09, 26.96), the northeast | signature drop item282639 Emogg's "Crusher" (dropped by nothing else) | source: npcs.json + items.json
- Boss Galgosh | npc1398 | level 22 rare, flagged rare in the data | single point (68.07, 65.93), the southeast Stonesplinter hold | signature drops item1215 Support Girdle, item1938 Block Mallet (each dropped by nothing else) | source: npcs.json + items.json
- Magosh | npc1399 | level 21 rare, flagged rare in the data | single point (70.12, 66.39), the southeast Stonesplinter hold | signature drops item2241 Desperado Cape, item3571 Trogg Beater (each dropped by nothing else) | source: npcs.json + items.json
- Lord Condar | npc14268 | level 16 rare, flagged rare in the data | loop over 4 points, the southeast hills (bbox 62.6-77.7, 66.9-78.5) | signature drop item282637 Shaking Egg (dropped by nothing else) | source: npcs.json + items.json
- Haren Swifthoof | npc2478 | level 20 rare (1-pt named record, no quest or vendor link; sole signature loot is exclusive — the Elwynn Ruklar-with-loot shape) | single point (55.45, 67.06) | signature drop item5319 Bashing Pauldrons (dropped by nothing else) | source: npcs.json + items.json
- Thragomm | npc7170 | level 20 rare (same shape as Haren, dens adjacent) | single point (55.3, 66.94) | signature drop item4949 Orcish Cleaver (dropped by nothing else) | source: npcs.json + items.json
- Carved Figurine | obj424007 at (49.42, 12.92), the dam's north bank — VERIFIED against the local data: the object record carries exactly this point (brief said ~(49.4, 12.9); difference is rounding, no discrepancy to report) and quest79975 Eagle's Fist (level 32, NOT in the core contract) starts from it; quest79974 Wet Job (level 32, zone 1442, also uncontracted) ends at it | one single-goto step with `optional` interact + bank-it-for-later note | source: objects.json + quests.json
- Fixed world containers | obj2849, Battered Chest, 11 fixed points (bbox 45.6-77.1, 13.5-66.5 — the Loch, the dam and the southeast) | one loop step, all ordinary low-level goods, no unique treasure; Loch Modan has no second fixed-chest record (obj106318 has no 1432 spawn) | source: objects.json

Band cutoff argued: the zone band is 10-20 and zone content tops out at 22 (Galgosh, the Large Crocolisk). The cutoff is drawn at level 22 per the Westfall band+2 rule — everything shipped is level 15-22, and everything above 22 (Obsidian Golem 38, Stonevault 36, Rugelfuss 40, Hinderweir 40, Ylva's... no, Ylva is 10) is OUT as out-of-band world content. Nothing at 21-22 is excluded on level alone; every shipped step states the rare's actual level.

Argued exclusions:
- Core quest objectives/item sources, every one core-guided (most contracted, hence tracker-backed): Chok'sul (contracted 256 — complete step in the core guide, even though the quest record carries no kill ref), Ol' Sooty (contracted 271), Daggerfang and Marek's Croc-Hunting Knife (contracted 86758), the Headsplitter (contracted 86585), Grawmug, Gnasher and Brawler (contracted 217).
- Core quest NPCs (givers/turn-ins): Magistrate Bluntnose (255/256), Daryl the Youngling and Vyrin Swiftwind (257/258/271/531), Marek Ironheart (385/86758), Magmar Fellhew (297/298/436/309 and uncontracted chains), Miran (309/454), Huldar (273/454), Saean (273 supply chain, confirmed by the core text), Mountaineer Ylva (86585), Prospector Ironband (298/86613), Norric Lochthane (86667/94495/94502), Bingles Blastenheimer (2038), Bailor Stonehand (uncontracted 1655 — Henze/Falkhaan precedent: quest giver either way).
- Vendors, trainers, flightmaster, stablemaster, innkeeper (service roles, not rares).
- Ambient family records (mob types with family twins elsewhere in the zone, even where a member holds an exclusive — the family, not an individual, drops it): all Stonesplinter troggs (including the Seer, whose Chewed Spell Notes are not a recipe and ship nothing), Tunnel Rat kobolds, Mo'grosh ogres, all bears (Patriarch/Elder/Grizzled), all boars (including the 1-pt Scarred Crag Boar), all crocolisks except the Large (Loch Crocolisk, Loch Frenzy — the core route farms generics for 385/278), Young Threshadon (juvenile, 21 pts — Westfall Goretusk precedent), all Lurkers (Cliff/Forest/Wood — core objectives for 418/278), plus critters, props, event/seasonal objects, signposts and unknown/placeholder records.
- Lootless single-point hub flavor (named but no drops at all, no rare flag, no quest or core link — the Dun Morogh Angus/Shorty rule): Torren Squarejaw, Kelt Thomasin, Dakk Blunderblast, Vidra Hearthstove, Thorvald Deepforge.
- Quest-owned treasure objects: the WANTED poster (obj256, contracted 256 starts from it — core-owned per the Westfall precedent) and Explosive Charges (obj1585, contracted 280/283).
- Unlinked quest-adjacent props (fixed, but named for NPC goods or flagged by the core guide's own tip — "Pick up Excavation Tools where they lie": Excavation Tools, Bailor's Ore, Bingles's Blastencapper, Shimmerweed-style Magenta Cap Clusters + trap).
- Unidentified fixed objects with no quest link and no container nature (left out rather than guessed — the Verigan's Fist precedent): Sunken Reliquary, Empty Trophy Display, Tangled Blight Pile, the Libram of Blessings object, Gnomish Tome (uncontracted Rumi quest 79093 — Darnassus).
- Gathering nodes, herbs, fishing debris, MFF/seasonal furniture, books, seats, bats, skulls, Leyline (Westfall precedent).

## loch-modan-recipes.guide — 10 recipes, all vendor-sold

- Recipe: Brilliant Smallfish | item6325 | buy from Khara Deepwater, npc1684, Thelsamar (40.28, 39.28) | Cooking | source: items.json vendors
- Recipe: Longjaw Mud Snapper | item6328 | buy from Khara Deepwater, npc1684 | Cooking | source: items.json vendors
- Recipe: Loch Frenzy Delight | item6329 | buy from Khara Deepwater, npc1684 | Cooking | source: items.json vendors
- Recipe: Smoked Bear Meat | item6892 | buy from Drac Roughcut, npc1465 (35.57, 49.15) | Cooking | source: items.json vendors
- Pattern: Red Woolen Bag | item5772 | buy from Rann Flamespinner, npc1474, Thelsamar (35.95, 45.87) | Tailoring (woolen) — also drops from a Westfall mob plus one elsewhere, but this vendor copy's source is physically in Loch Modan (the Westfall 5771 precedent) | source: items.json vendors
- Pattern: Greater Adept's Robe | item6275 | buy from Rann Flamespinner, npc1474 | Tailoring | source: items.json vendors
- Pattern: Linen Reagent Bag | item253665 | buy from Rann Flamespinner, npc1474 | Tailoring (linen) | source: items.json vendors
- Pattern: Woolen Reagent Bag | item253668 | buy from Rann Flamespinner, npc1474 | Tailoring (woolen) | source: items.json vendors
- Recipe: Rage Potion | item5640 | buy from Xandar Goodbeard, npc1685, Farstrider Lodge (82.47, 63.35) | Alchemy | source: items.json vendors
- Recipe: Holy Protection Potion | item6053 | buy from Xandar Goodbeard, npc1685 | Alchemy | source: items.json vendors

Every dropped recipe with any Loch Modan source also drops in 4+ other zones — all generic world drops, none shipped, so no drop recipe made the guide (unlike Westfall's Shafety Sheep and Dun Morogh's Peace Tea, Loch Modan has no exclusive-drop recipe). Profession gates use `when skill <Profession> 1`; stock class is unconfirmed, so nothing is marked limited. Professions with no Loch Modan source (Blacksmithing, Leatherworking, Engineering, Enchanting, First Aid, Fishing) are named as absent in the guide header per the Dun Morogh Blacksmithing precedent.
