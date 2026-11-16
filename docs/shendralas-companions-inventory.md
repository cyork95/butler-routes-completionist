# Shen'dralas companions inventory (pack butler-routes-completionist)

Source: local Forever game data (questie-forever npcs/objects/items/quests.json),
built with `--product wowf` + QuestieDB. Accept-zone key **2652**, core band
**30-49**, Alliance route. The core contract (28 quests,
`docs/shendralas-census.md`) is untouched by this inventory. Game data wins
over community sources throughout. Rank flags follow the Winterspring
precedent (rank 4 = Rare, rank 2 = Rare Elite); rank-1 elites were examined
Silithus-style: rank 1 alone marks elites, not rares — shipped only with
loot/exclusivity.

## RARES: 10 rank-1 examined, 0 shipped

No NPC spawning on 2652 carries the data's rare flag (no rank 2, no rank 4, no
`roles: ["rare"]` anywhere on the key). The ten rank-1s:

| npc | level | points (map 2652) | loot in data | disposition |
|-----|-------|-------------------|--------------|-------------|
| 252695 Pylon Protector | 61 | 24 pts, halls-wide | none | EXCLUDE: no loot, far above band (61 vs top 49) |
| 253274 Magram Necrokhan | 45 | 24 pts, west/center | 254432 Carved Centaur Totem (Desolace core quest item) | EXCLUDE: loot significance is Desolace core content (Dun Morogh precedent) |
| 253275 Outcast Necrokhan | 45 | 24 pts, south | 254432 (same) | EXCLUDE: same as 253274 |
| 253394 Corpsefeeder | 45 | 24 pts, center-east | 259893 Corpsefeeder's Carapace (Shen core item-start 93574) | EXCLUDE: core-contracted significance (Dun Morogh precedent) |
| 253471 Mordent Evenshade | 60 | 1 pt (35.17, 46.61) | none | EXCLUDE: core giver, above band |
| 253527 Kog'thug the Brave | 43 | 1 pt (72.73, 31.17) | none | EXCLUDE: core giver/turn-in, quest significance only |
| 254674 Woodwyrd | 60 | 1 pt (69.66, 71.78) | none | EXCLUDE: core giver + kill target, above band |
| 255678 Quolga the Wise | 42 | 1 pt (58.15, 14.78) | none | EXCLUDE: core turn-in, quest significance only |
| 255759 Shen'dralas Protector | 60 | 24 guard-like pts | none | EXCLUDE: no loot, above band |
| 276401 Nascent Pylon Protector | 43 | 24 pts, center | Waylaid Crate 248694 + journal pages 260348-52/354 (exclusive to it) | EXCLUDE: core kill target (99258 Mana Mania); pages are incidental exclusive drops of a core-owned kill, no companion step (would duplicate the core kill) |

Quest-target lookalikes (named mobs with no rank at all — Nerlokh, Orgrul,
Hagiak, Rokren, the Bristleback/Magram/Outcast mobs, Decrepit Pylon
Protectors) are not rares. Tame lines: none shipped. Beasts examined: Prowler
255207 (drops the core collar 259461 — not tameability evidence) and Bear
263681 (no drops at all); no drop evidence of tameability anywhere and no core
quest sends the player to kill a beast family, so the tame question is logged
to `docs/companion-unverified.md`, never guessed.

## TREASURES: 4 fixed objects, 2 shipped

Objects on 2652 carry no loot tables in the data, so contents are unconfirmed
throughout (Deadwind precedent: ship fixed uniques with honest notes).

| object | points (map 2652) | disposition |
|--------|-------------------|-------------|
| 577959/577960 Shen'dralar Pylon | (43.61, 34.29) / (73.27, 23.13) | EXCLUDE: core quest-accept objects (92914 Strange Pylons) |
| 602101 Centaur Supplies | 9 pts: (29.4,69.9), (29.5,72.1), (29.6,73.7), (29.9,69.4), (30,73), (30,74.5), (30.3,70.8), (30.7,70.6), (34.8,77.8) | SHIP: one `loop` step over all 9 fixed points, said plainly (contents unconfirmed) |
| 613713 Evenshade's Journal | 1 pt: (35.07, 46.53) | SHIP: plain single-goto + note, no loop (a loop needs 2+ points; contents unconfirmed) |

## RECIPES: 1 shipped (0 vendor, 1 narrow drop)

Full scan: every recipe/pattern/plan/schematic/design/formula/manual whose drop
table names a 2652-spawning mob, and everything sold by a 2652-spawning
vendor. No 2652-spawning vendor sells anything (Adarien 252691 is an
innkeeper with no stock in the data), so the Alterac Horde-vendor check has
nothing to act on and vendor-sold is an empty class.

| recipe | profession (prefix convention) | source | disposition |
|--------|-------------------------------|--------|-------------|
| 251392 Plans: Shining Mithril Breastplate | Blacksmithing | drop: 253272 Magram Necromancer (2652 spawns, e.g. 24.55, 24.24); 2 droppers anywhere total (other: 11559 Outcast Necromancer, Desolace) | SHIP: narrow 2-dropper with an in-zone source; `collect` at the west Magram grounds |

Excluded with reasons: all ~750 other in-zone-dropping recipe records (every
one examined: in-zone dropper list empty — generic multi-zone world drops, not
zone content, Elwynn rule); 0 vendor recipes (nothing sold in-zone);
quest-reward recipes (UNVERIFIABLE — quest records carry no reward data, class
logged in companion-unverified). All professions except Blacksmithing have no
Shen'dralas source — the guide says so in a note (Dun Morogh precedent).
