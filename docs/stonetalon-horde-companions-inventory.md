# Stonetalon Mountains (Horde) — companions inventory

Contract: the Horde core `stonetalon-horde.guide` (23 quests, band 12–30).
Zone key 1442. Sources: `npcs.json`, `objects.json`, `items.json`,
`quests.json` from the local Forever data build
(`--product wowf` + QuestieDB). Game data wins everywhere below.

## Rares — 9 flagged on key 1442, all shipped

Every NPC spawn on key 1442 carrying the data's rare flag. None of the nine
appears anywhere in `stonetalon-horde.guide` (grep for all nine IDs: zero
hits), so none is giver, ender, or objective of a core-contracted quest —
all nine are companion content, not core content (Dun Morogh rule satisfied).
The data records no loot on any of the nine, so there are no signature drops
to chase and no tame lines ship either (no loot evidence; the core guide
carries no beast-family corroboration — see `docs/companion-unverified.md`).
Respawn timers are unconfirmed anywhere, so none are stated.

- Taskmaster Whipfang | npc 5932 | level 22 rare | single point
  (64.55, 54.19), Windshear east | no loot; no quest linkage
- Foreman Rigger | npc 5931 | level 24 rare | single point (66.69, 52.33),
  Windshear east | no loot; no quest linkage
- Pridewing Patriarch | npc 4015 | level 25 rare | TWO points (47.75, 46.75),
  (53.79, 36.31), center — the only multi-point rare, loop step | no loot;
  no quest linkage
- Sentinel Amarassan | npc 5916 | level 27 rare, faction A | single point
  (35.25, 15.04), north | no loot; no quest linkage. Alliance-aligned in the
  data, so an enemy to Horde players; northern Stonetalon is Alliance-held
  ground, so the guide says so.
- Sorrow Wing | npc 5928 | level 27 rare | single point (49.27, 36.18),
  center | no loot; no quest linkage
- Sister Riven | npc 5930 | level 28 rare | single point (29.64, 69.43),
  far southwest | no loot; no quest linkage
- Brother Ravenoak | npc 5915 | level 29 rare, faction A | single point
  (28.05, 12.23), north | no loot; no quest linkage (same enemy-note as
  Amarassan)
- Vengeful Ancient | npc 4030 | level 30 rare | single point (30.45, 68.08),
  southwest, top of band | no loot; no quest linkage. It shares the
  multi-zone world-drop formula 11151 with four other droppers — not a
  signature drop, not ridden here.
- Nal'taszar | npc 4066 | level 30 rare, faction A | single point
  (25.57, 11.48), northwest, top of band | no loot; no quest linkage (same
  enemy-note as Amarassan)

Rares above the core band (12–30): none — the highest-flagged rare is
exactly 30. Excluded for faction: none — the three faction-A rares are
killable opposition for Horde, not friendlies (Falthis-style exclusion does
not apply; nothing friendly-to-Horde is flagged rare in this zone).

## Item-start hunts — nothing ships

- 6284 starts from the Wanted Poster object 177904, data-placed at
  (59.06, 75.71). The core guide routes the accept itself at that point, so
  there is nothing to hunt — no companion step, at most this pointer.
- 94216 is a sourceless writ (R2 bag-note handling in the core). No source
  exists in the data, so no hunt can be routed.

## Treasures — all fixed world objects on key 1442 with no quest linkage

Quest-linkage scan (quest objective objects in `quests.json`): none of the
objects below is any quest's objective. The Barrow Cache / Talon Den Hoard
pair from the Alliance round belongs to Stranglethorn's Pebble of Kajaro
quests and has no 1442 spawn — not covered here. The Pylon objects are core
quest-accept furniture, not treasure — not covered here. Gaea Seed 674121
and object 4358 do not exist in `objects.json` — nothing to ship, logged
here instead of guessed.

- Battered Chest (obj 2849) — 10 fixed points, one loop step, said plainly:
  (43.26, 38.71), (63.56, 40.17), (66.57, 50.79), (72.2, 60.3),
  (73.07, 59.97), (73.3, 58.9), (74.08, 59.35), (77.07, 91.62),
  (80.65, 89.41), (84.32, 84.19)
- Battered Footlocker (obj 179486) — 11 fixed points, one loop step:
  (59.73, 53.51), (61.36, 55.56), (61.9, 51.51), (62.91, 53.18),
  (63.3, 51.21), (66.09, 50.89), (67.84, 56.58), (70.18, 48.74),
  (71.37, 52.63), (71.5, 56.79), (71.86, 49.53)
- Battered Footlocker (obj 179488, distinct object) — 5 fixed points, one
  loop step, Windshear: (72.15, 61.04), (72.51, 63.13), (73.67, 60.02),
  (74.15, 59.15), (74.24, 59.54)
- Solid Chest (obj 2850) — 7 fixed points, one loop step, west:
  (28.35, 64.23), (29.14, 70.26), (31.69, 58.82), (32.61, 65.99),
  (34.53, 61.97), (35.02, 68.87), (36.99, 68.79)
- Food Crate (obj 3662) + Barrel of Milk (obj 3705) — 16 SHARED fixed
  points, one loop step riding both collects, said plainly: (45.67, 59.07),
  (47.47, 62.49), (59.08, 62.6), (66.47, 51.58), (71.31, 94.3),
  (72.64, 95.48), (73.33, 85.7), (73.62, 95.03), (74.36, 85.84),
  (76.49, 91.95), (76.91, 89.76), (78.35, 85.22), (78.67, 86.09),
  (80.75, 88.78), (82.51, 88), (84.92, 84.6)
- Barrel of Melon Juice (obj 3659) + Food Crate (obj 3695) — 1 shared point
  (36.64, 6.72), far north: rides the single zone-wide container loop with its
  own interacts.
- Sleepers' Cache (obj 19596) — 1 point (25.55, 11.36), northwest; Druids'
  Cache (obj 19597) — 1 point (29.55, 15.84), north; Gatekeeper's Hold (obj
  19595) — 1 point (29.9, 15.39), north: one non-loop Barrow Dens step with
  all three interacts (the Alliance guide's shape). Lootless and
  quest-unused; contents unconfirmed.
- Hidden Stash (obj 674126) — 2 points (40.7, 52.4), (40.7, 52.7): rides the
  zone-wide loop. Lootless and quest-unused; contents unconfirmed.
- EXCLUDED for faction: Alliance Chest (obj 3715, 4 northern points (25.44,
  11.72), (28.38, 12.29), (29.78, 15.27), (30.41, 15.37)) — Alliance-faction
  object, not openable by Horde players. Shipped in the Alliance guide; the
  Horde guide names the exclusion instead.

## stonetalon-horde-recipes.guide — 3 vendor-sold + 4 narrow drops

Vendor scan: recipe-named goods of every vendor spawning on key 1442.
Phantom IDs from the first filter pass (605, 6217 as a recipe, 7413, 7418,
3012 as recipes, vendor IDs 4839/13159) were re-checked against names and
dropped — 605 does not exist (the real item is 6055), 6217 Copper Rod is a
tool, 3012 Scroll of Agility is a consumable, 7413/7418 are armor greens,
and the real Jeeda/Kulwia records are npc 4083/12043. Lesson logged: match
names, not bare IDs.

- Alchemy — Sun Rock Retreat (Jeeda 4083, Horde, Apprentice Witch Doctor,
  (47.61, 61.59)): buy 6055 "Recipe: Fire Protection Potion" npc 4083.
- Enchanting — the south (Kulwia 12043, Horde, Trade Supplies,
  (45.39, 59.33)): buy 11039 "Formula: Enchant Cloak - Minor Agility"
  npc 12043; buy 11101 "Formula: Enchant Bracer - Lesser Strength" npc 12043.
  (Copper Rod 6217 from the same vendor is a tool, not a recipe — not
  shipped.)
- Engineering — Windshear east (Veenix 4086, neutral AH, Venture Co.
  Merchant, (58.22, 51.74)): buy 7561 "Schematic: Goblin Jumper Cables"
  npc 4086. Same step the Alliance guide ships; the vendor serves both.
- Cooking — Windshear drop: collect 249880 "Recipe: Royal Tea" optional,
  dropped only by the Windshear Geomancer (npc 4003, level 20), 6 points:
  (73.13, 61.06), (73.53, 58.74), (73.8, 59.26), (73.92, 59.62),
  (74.43, 58.39), (75.67, 59.2). Nowhere else in the data.
- Alchemy — west drop: collect 250382 "Recipe: Elixir of Spirit" optional,
  dropped only by the Bloodfury Harpy (npc 4022, level 23), 12 points:
  (30.18, 64.33), (30.93, 59.23), (31.34, 60.42), (31.83, 58.76),
  (31.95, 66.51), (32.57, 60.66), (32.75, 64.45), (33.36, 64.99),
  (34.51, 60.8), (35.25, 63.21), (37.36, 49.09), (37.79, 44.11). Nowhere
  else in the data.
- Blacksmithing — south drop: collect 251454 "Plans: Brass Knuckles"
  optional, dropped only by the Gogger Rock Keeper (npc 11915, level 16),
  18 points: (58.15, 90.75), (58.28, 89.89), (58.51, 91.47), (58.74, 89.58),
  (59.03, 89.94), (59.57, 90.25), (59.61, 92.77), (60, 90.26),
  (60.08, 92.07), (60.44, 90.99), (60.57, 91.43), (61.08, 92.46),
  (61.28, 90.98), (61.93, 93.42), (62.14, 93.05), (62.22, 93.59),
  (62.44, 92.25), (62.67, 92.57). Nowhere else in the data.
- Enchanting — Charred Vale drop: collect 11151
  "Formula: Enchant Gloves - Herbalism" optional, dropped by the Charred
  Ancient (npc 4028, 3 points), Blackened Ancient (npc 4029, 2 points) and
  Vengeful Ancient (npc 4030, 1 point) — a tight in-zone family — plus two
  out-of-zone droppers (3834, 3919). Narrow, not zone-exclusive; said so.

Excluded with reasons: Pattern 7361 (Harlown Darkweave 6731, faction A —
Alterac rule, flipped); Recipes 12233/12240 (Janet Hommers 8150, faction
A — same rule); Sovik's 16041/16042/18647 (vendor 3413 spawns only on key
1454 Orgrimmar — no in-zone source); 250383 Elixir of Greater Spirit
(vendors on keys 1413/1433 — out of zone); 251443 Blessed Plate Leggings
(sole dropper npc 7451 on key 1452 — out of zone); every other
Stonetalon-dropping recipe is a generic multi-zone world drop (Elwynn
rule); quest-reward recipes are unverifiable (no reward data); trainer
staples excluded (Polestar's profession guides cover those).

Professions with NO in-zone Horde source, stated in the guide, not padded:
Tailoring, Leatherworking, First Aid, Fishing.
