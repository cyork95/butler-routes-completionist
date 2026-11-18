# Un'Goro Crater (Horde) companions inventory (game data, accept-zone key 1449)

Source: local Forever game data (questie-forever NPC/object/item/quest
dumps), enumerated fresh for the Horde side. Rank semantics per the
Feralas/Azshara calibration: rank 4 = Rare, rank 2 = Rare Elite. The
Horde core contract is 3 quests (4145/4147/4148, band 47-53,
`ungoro-horde`); the core guide owns every
core-contracted objective — nothing below duplicates it.

## RARES — 3 rank-4 flagged, all shipped (one with a come-back-later note)

Every spawn on key 1449 carrying rank 2/4 or a roles flag was enumerated:

| NPC | Lvl | Rank | Point(s), verified | Drops of note | Guide step |
|-----|-----|------|--------------------|---------------|------------|
| 6581 Ravasaur Matriarch | 50 | 4 | (62.35, 65.95) single | 286616 Matriarch's Prowlers — SOLE dropper (null rate; Feralas calibration: null rate does not disqualify) | single goto + collect |
| 6582 Clutchmother Zavas | 54 | 4 | (48.73, 85.35) single | none sole (journal/soil/bits generics) | single goto + kill note, come-back-later (1 over the Horde band) |
| 6585 Uhk'loc | 53 | 4 | (68.48, 12.66) single | 285284 Balanced Knives of the Bandit — SOLE dropper (null rate) | single goto + collect |

Notes:
- The two sole-drop signatures are genuine deltas vs the Alliance
  inventory (which reads all three as signature-less): each was verified
  by scanning every item's drop table for single-dropper lists, and both
  ship here with their null rates stated honestly. Flagged in
  docs/companion-unverified.md, never silently harmonized.
- Zavas at 54 sits one level above the Horde band top (47-53): she ships
  with a come-back-later note rather than being cut (Safety Sheep
  precedent — the point is verified, the note is honest). The Alliance
  band ran 47-54 and shipped her clean; the band difference is the only
  reason for the different handling.
- No rare in this list is a giver, ender, or objective of any
  HORDE-contracted quest (4145/4147/4148: starts all NPC 9118, ends
  9118/8496; objectives are bloodpetal kills, no objectives, and the
  Sprout item — no rare drops 11315 or starts a Horde quest, verified by
  scan). The Dun Morogh exclusion does not fire.
- Loot tables otherwise are shared world loot (journals, soil, gems,
  Thorium plans with 500+ sources) — kill notes, nothing to collect.

### Rare exclusions

- Gruff (6583, level 57) and King Mosh (6584, level 60): roles ["rare"]
  but rank 2, not rank 4 — excluded as rank-2 elites per the
  Felwood/Azshara rank rule. Both are also above the band top. Mosh's
  Devilcore patterns (228119/228120) still ship in the RECIPES guide —
  that guide keys on drop sources, not mob rank, so the patterns are
  unaffected by this call (same as the Alliance round).
- Blazerunner, Lar'korwi pair, Gorishi pair: unflagged (and Blazerunner is
  a core quest target) — out per the Alliance round's calls, which the
  data confirms unchanged.
- Rares excluded as rank-2 are NOT companion content anywhere in this
  round; the recipes-cover note for Mosh is the documented exception.

## ITEM-START HUNTS — none

All three Horde contracts accept from NPC 9118 (no item starts in the
pool — start-item scan empty). The 4148 Sprout objective drops at 100%
from devilsaurs and the Sprout object — no rare is involved (verified by
scan). Zero hunts ship, stated with the scans behind it.

## TREASURES — none confirmed (rares-only guide, same as Alliance)

- Ornate Chest (164910): Alliance 3962's quest objective — quest
  furniture, and no lootability flag exists in the data for a Horde
  reading either. Not companion treasure.
- Un'Goro Dirt Pile (157936, 24 pts, also spawns 1451), Dinosaur Bone
  (161527, 18 pts), Power Crystal formations (164658-81), Fresh/Preserved
  Threshadon Carcasses (166863/169216), Shallow Grave (489943, 1 pt),
  mining veins, herb nodes, Fire Elemental Rifts, Whipweed: fixed objects
  with no lootability flag anywhere in the data — unconfirmable as
  treasure, never invented.
- Raft, pack, pylons, JD crystals, Damaged Blue Crystal, hot spot,
  posters, J.D.'s Manual, Muigin's Sprout, Bloodpetal Sprout object,
  Hive Hatchery, Flat Rock: core-contracted quest objects — the Horde
  core guide owns the Sprout leg; the rest belong to the main guide.
- Midsummer / Winter Veil props: seasonal event furniture, not treasure.

## RECIPES — 10 shipped (vendor 3 + drops 7)

Vendor faction field "AH" reads as both-faction (both vendors sit in the
crater serving whoever walks up); no Horde-only exclusion fires. No
limited-stock flag exists in the data; no stock is marked limited.

Vendor-sold (npc-pinned buys):

- 15724 Pattern: Heavy Scorpid Bracers (Leatherworking) — Zannok
  Hidepiercer (12956), @23.00, 16.40, south-west crater (sole vendor).
- 15762 Pattern: Heavy Scorpid Helm (Leatherworking) — Zannok
  Hidepiercer, same point (sole vendor).
- 15758 Pattern: Devilsaur Gauntlets (Leatherworking) — Nergal (12959),
  @43.27, 7.73, Marshal's Refuge (sole vendor).

Mob-dropped (optional collects at data-placed droppers):

- 15772 Pattern: Devilsaur Leggings (Leatherworking) — the four Un'Goro
  oozes, ALL droppers in-zone and nowhere else: Muculent @57.19, 38.36 /
  @60.92, 37.60, Primal @38.52, 17.34 / @43.47, 65.21, Glutinous @25.62,
  45.47 / @28.21, 35.87, Cloned @45.44, 66.04 / @56.20, 18.13 (rates
  ~1%, two points per ooze in the loop).
- 228119 Pattern: Devilcore Gauntlets + 228120 Pattern: Devilcore
  Leggings (Leatherworking) — SOLE source King Mosh @35.30, 35.99
  (rank-2, above band — recipes key on the drop, come-back note rides).
- 250181 Recipe: Raging Raptor Ribs (Cooking) — SOLE dropper Venomhide
  Ravasaur 6508 (loop points @62.43, 50.52 / @64.45, 50.48 / @65.46,
  46.81; the same-named 269206 spawns in-zone but drops nothing — named,
  not routed).
- 252882 Pattern: Tooled Leather Crown (Leatherworking) — SOLE dropper
  Scorching Elemental 6520 (loop points @45.71, 51.58 / @47.35, 53.23 /
  @49.74, 44.05; the same-named 272319 has NO spawns anywhere — named,
  not routed).
- 252914 Pattern: Supple Scorpid Leggings (Leatherworking) — SOLE
  dropper Ravasaur 6505 (loop points @57.36, 77.14 / @59.16, 74.72 /
  @60.60, 78.14).
- 252927 Pattern: Charged Scorpid Bracers (Leatherworking) — SOLE
  dropper Tar Creeper 6527 (loop points @47.20, 31.91 / @48.57, 33.12 /
  @49.12, 33.90).

### Recipe exclusions

- ~200 recipes with in-zone mob droppers but dozens to 600+ total
  sources (Thorium/Mithril plans, Frostweave/Brightcloth/Runecloth
  patterns, transmutes, protection potions, schematics): generic world
  drops under the Elwynn rule. Uhk'loc's four patterns and the formula
  (500-646 each) are the named instances here.
- Trainer-taught staples: out of scope (Polestar's profession guides own
  progression).
- Quest-reward recipes: UNVERIFIABLE (quest records carry no reward data)
  — logged in docs/companion-unverified.md, never shipped.
- Professions with NO Un'Goro Horde source in the data: Alchemy,
  Blacksmithing, Tailoring, Enchanting, Engineering, First Aid, Fishing
  — the recipes guide says so plainly (Dun Morogh Blacksmithing
  precedent).

## DEVILSAUR TAME CANDIDACY (named check — bar fails, logged, nothing shipped)

- Candidates: Devilsaur 6498 (3 pts), Ironhide Devilsaur 6499 (1 pt),
  Tyrant Devilsaur 6500 (2 pts) — all rank 1, unflagged; plus King Mosh
  (6584), which the data does NOT label a devilsaur (no family flag on
  any NPC record — family is unverifiable in this build, so Mosh's
  candidacy rests on his name alone).
- Drop evidence: devilsaurs drop 11315 Bloodpetal Sprout at 100% — but
  that is the Horde core's kill objective (the core guide kills them for
  it), which is explicitly NOT taming corroboration per precedent.
- Core corroboration: none — `ungoro-horde.guide` carries no Hunter lines
  and no references to any devilsaur outside kill objectives.
- No tameability flag exists anywhere in the NPC data. Bar fails on all
  three legs that matter (flag, corroboration, evidence-as-taming):
  NO `only Hunter` task ships. Logged here and in
  docs/companion-unverified.md; promote only with a data flag or a core
  tame line.

## DELTAS vs the Alliance inventory

1. Two sole-drop signatures (286616 on the Matriarch, 285284 on Uhk'loc)
   verified by full drop-table scan — the Alliance inventory reads all
   three rank-4s as signature-less. Both ship in the Horde rares guide
   with null rates stated; flagged in companion-unverified (the Alliance
   guide may adopt or decline — never silently harmonized).
2. Zavas handling differs by band only (Alliance 47-54 clean ship; Horde
   47-53 come-back-later note). Same point, same data.
3. No other deltas: exclusions, treasures verdict, recipe set (10),
   vendor pins, and no-source profession list are identical.
