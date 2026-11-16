# Burning Steppes companions inventory (pack butler-routes-completionist)

Source: local Forever game data (questie-forever npcs/objects/items/quests.json),
built with `--product wowf` + QuestieDB. Accept-zone key **1428**, core band
**48-60**, Alliance route. The core contract (59 quests) is untouched by this
inventory. Game data wins over community sources throughout.

## RARES - 11 rare-flagged NPCs on 1428, all 11 shipped

Rank semantics per the Badlands calibration: rank 4 = Rare, rank 2 = Rare Elite.
Every point below is the data's spawn point verbatim. Signature = the item's
sole dropper anywhere in the data (drops.npc lists only this NPC).

| NPC | lvl | points (map 1428) | signature (sole drop, rate) | disposition |
|-----|-----|-------------------|-----------------------------|-------------|
| 584 Kazon | 27 | 1: 71.1,85 (+1433 Redridge side) | 2058 Kazon's Maul (25%), 3231 Cutthroat Pauldrons (75%) | SHIP single-goto + 2 collects; below-band grey, trivially killable |
| 8976 Hematos | 60 | 1: 22.38,60.03 | none (generic loot only) | SHIP single-goto, kill-only |
| 8978 Thauris Balgarr | 57 | 9: 54.2,39.11 / 55.47,36.09 / 60.92,36.46 / 61.72,37.6 / 65.03,42.83 / 65.73,43.71 / 66.12,41.93 / 71.04,35.82 / 71.27,36.94 | none | SHIP 9-pt loop, kill-only |
| 8979 Gruklash | 59 | 7: 15.21,30.42 / 39.68,35.86 / 40.56,34.61 / 40.7,32.6 / 41.47,53.9 / 42.14,54.77 / 44.13,56.33 | none | SHIP 7-pt loop, kill-only |
| 8981 Malfunctioning Reaver | 56 | 5: 79.17,29.71 / 85.81,57.07 / 88.06,31.77 / 88.6,57.35 / 90.02,45.99 | none (mechanical) | SHIP 5-pt loop, kill-only |
| 9046 Scarshield Quartermaster | 55 | 1: 34.9,27.9 (+1415/1427) | 13248 Burstshot Harquebus (50%), 13254 Astral Guard (50%), 18987 Blackhand's Command (100%, core 7761 starter) | SHIP single-goto + 2 loot collects + core note |
| 9602 Hahk'Zor | 54 | 4: 80.54,47.97 / 81.7,43.77 / 81.73,41.91 / 81.91,48.25 | none | SHIP 4-pt loop, kill-only |
| 9604 Gorgon'och | 54 | 5: 77.16,43.14 / 77.88,41.49 / 79.45,45.37 / 79.82,42.32 / 80.46,41.45 | none | SHIP 5-pt loop, kill-only |
| 10077 Deathmaw | 53 | 4: 75.54,32.89 / 81.51,56.7 / 82.73,30.35 / 87.36,50.45 | 282049 Deathmaw's Guise (rate null, SOLE); also drops 11467 Blackrock Medallion (33%, core 4283 objective) | SHIP 4-pt loop + Guise collect + core note |
| 10078 Terrorspark | 55 | 8: 41.86,46.53 / 42.3,44.74 / 45.88,43.46 / 49.08,43.12 / 51.2,42.92 / 63.57,37.79 / 68.39,31.45 / 69.03,31.61 | none | SHIP 8-pt loop, kill-only |
| 10119 Volchan | 60 | 1: 74.3,37.82 | 12828 Plans: Volcanic Hammer (65%, carried by the recipes companion) | SHIP single-goto kill + recipes note, no loot collect here |

Notes applied in the guide:
- Core-contract cross-check (all 59 quests' objectives): no rare is the kill
  objective of any contract quest, so the Dun Morogh exclusion does not fire on
  kill targets. Deathmaw drops a core objective item (11467 medallion, one of
  many sources) and the Quartermaster drops the core item-start (18987): both
  keep their steps because each has standalone exclusive loot of its own, and
  the steps point at the core guide for the quest side. Volchan's only
  significance besides the kill is the recipe, which is routed in the recipes
  companion with a cross-note - not a core quest, so the exclusion does not
  fire. No quest-target lookalikes carry the rare flag.
- Nothing above band (max 60 = band top); Kazon (27) is far below band and
  ships as a trivial kill, no come-back note needed.
- All other drops in the data are generic world loot shared across many mobs;
  the guide says so plainly with no goals for them.
- No tame lines: NPC records carry no family/tame flags, and no rare has both
  drop evidence and core-guide corroboration (the core's kill families are
  dragonkin, orcs, ogres and elementals - none tameable). The tame questions
  for Kazon, Hahk'Zor, Gorgon'och, Deathmaw, Terrorspark and Volchan go to
  docs/companion-unverified.md, never guessed.

## TREASURES - fixed-spawn container objects on 1428

| object | points | disposition |
|--------|--------|-------------|
| 2850 Solid Chest | 3: 64.1,85.2 / 69.5,84.8 / 71.6,84.8 (also spawns multi-zone) | SHIP one 3-pt loop, said plainly as generic fixed placements |
| 4149 Solid Chest | 2: 68.3,23.2 / 70,20.8 (also multi-zone) | SHIP one 2-pt loop, generic |
| 153453 Solid Chest | 19 scattered (21.78,47.41 / 31.22,62.38 / 36.04,48.18 / 38.8,54.36 / 40.76,34.39 / 42.93,37.52 / 43.28,33.99 / 44.66,58.34 / 51.07,53.13 / 55.46,53.74 / 57.63,61.16 / 76.18,55.9 / 77.04,61.88 / 80.69,48.87 / 81.86,44.81 / 82.86,46.15 / 84.46,26.59 / 88.28,37.84 / 92.24,53.39) | SHIP one 19-pt loop, generic |
| 153556 Thaurissan Relic | 24 (52.49,39.05 / 53.94,35.06 / 54.18,40.87 / 55.41,37.29 / 55.77,39.4 / 57.32,41.66 / 57.41,36.38 / 57.87,39.06 / 59.32,43.93 / 59.64,37.69 / 60.31,35.13 / 61.5,41.21 / 61.85,36.72 / 62.71,39.6 / 63.46,35.59 / 64.12,44.14 / 64.63,37.23 / 65.26,34.81 / 66.11,40.44 / 67.2,38.07 / 67.59,43.73 / 68.25,40.86 / 69.88,38.12 / 72.39,33.93), spawns ONLY on 1428 | SHIP one 24-pt loop, noted as the zone-exclusive fixed object with contents unconfirmed in the data |
| 160445 Sha'ni Proudtusk's Remains | 1: 79.79,45.53, spawns only here | SHIP plain goto + note (Horde-quest furniture for OUT quest 3822, nothing to collect for Alliance) |
| 702301 A Small Pack | 1: 37.3,26.6, spawns only here | SHIP plain goto + note (contents unconfirmed in the data) |

Excluded with reasons: core-quest objects (160839 Gor'tesh's Head, 160840
Soft Dirt Mound, 169294 Tablet, 175246-175249 Kibler's Cages, 175264 Broodling
Essence) - core content, never companions; resource nodes (all veins, deposits,
herbs, 181098 Volcanic Ash) - profession materials, not treasure; functional
and flavor objects (Meeting Stones, Orb of Command, forges, anvils, cauldrons,
campfires, bonfires, altars, books, Ghost Gate, skill circles, skull piles) -
not containers, no loot; joke/custom objects with no loot or linkage
(456814, 456815, 457101).

## RECIPES - 10 shipped (1 vendor, 9 zone-exclusive/narrow drops)

| recipe | profession | source | disposition |
|--------|-----------|--------|-------------|
| 10602 Schematic: Deadly Scope | Engineering | vendor 9544 Yuka Screwspigot @66.06,21.95, faction neutral | SHIP buy, npc-pinned |
| 12828 Plans: Volcanic Hammer | Blacksmithing | drop: 10119 Volchan @74.3,37.82 @65%, sole dropper anywhere | SHIP collect |
| 13476 Recipe: Mighty Rage Potion | Alchemy | drop: 7027 Blackrock Slayer @55.29,53.96 @4%, sole dropper anywhere | SHIP collect |
| 14482 Pattern: Cindercloth Cloak | Tailoring | drop: 7037 Thaurissan Firewalker @61.11,41.95 @1.78%, sole dropper anywhere | SHIP collect (same step as 14490, same dropper) |
| 14490 Pattern: Cindercloth Pants | Tailoring | drop: 7037 Thaurissan Firewalker @61.11,41.95 @1.96%, sole dropper anywhere | SHIP collect (same step as 14482, same dropper) |
| 15732 Pattern: Volcanic Leggings | Leatherworking | drop: 7035 Firegut Brute @78.17,40.37 @3.9%, sole dropper anywhere | SHIP collect (same step as 227908, same dropper) |
| 227908 Pattern: Masterwork Volcanic Leggings | Leatherworking | drop: 7035 Firegut Brute @78.17,40.37, rate null, sole dropper anywhere | SHIP collect with rate-unconfirmed note (same step as 15732) |
| 15738 Pattern: Heavy Scorpid Gauntlets | Leatherworking | drop: 7025 Blackrock Soldier @42.33,56.02 @3.74%, sole dropper anywhere | SHIP collect |
| 15748 Pattern: Heavy Scorpid Leggings | Leatherworking | drop: 7027 Blackrock Slayer @39.33,55.58 @3.84%, sole dropper anywhere | SHIP collect |
| 15774 Pattern: Heavy Scorpid Shoulders | Leatherworking | drop: 7029 Blackrock Battlemaster @39.82,32.8 @0.97%, sole dropper anywhere | SHIP collect |

Profession coverage: Engineering 1, Blacksmithing 1, Alchemy 1, Tailoring 2,
Leatherworking 5. No Cooking, Fishing, First Aid or Enchanting source exists in
the data - the guide says so in a note (Dun Morogh precedent).

Excluded with reasons: ~150 recipe drops with hundreds of droppers each at
0.02% (Elwynn rule - generic world drops, not zone content); 11615 Plans:
Dark Iron Shoulders (14 droppers, not narrow); 223163 Formula: Scroll of
Spatial Mending (4 Fel Interloper droppers spread across 9 zones - multi-zone,
not narrow); quest-reward recipes (UNVERIFIABLE - quest records carry no
reward data, class logged in companion-unverified); no Horde-only vendor
exclusion arises (the single vendor recipe is sold by neutral Yuka; no other
in-zone vendor sells recipes).
