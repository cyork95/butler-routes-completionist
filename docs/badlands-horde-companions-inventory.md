# Badlands (Horde) companions inventory (game data, accept-zone key 1418)

Source: local Forever game data (questie-forever NPC/object/item dumps).
Method mirrors `docs/badlands-companions-inventory.md` with the faction
rule flipped: a rare friendly to Horde / unkillable by Horde players is
excluded with the reason logged (Ashenvale Falthis precedent); hostile
faction-A rares would ship as killable opposition with an honest note
(Stonetalon precedent) — none occur here (every rare on this key is
react-null to both factions). Working band 30–40, derived from the Horde
core contract (`badlands-horde`, 13 quests, levelBand 30-40) — the
Alliance 28–40 is not copied.

Rank calibration as established: rank 4 = Rare, rank 2 = Rare Elite. Loot
"sole dropper" means the item's drops.npc lists only that NPC and no
object source. Rates shown where the data gives a number; a null rate
does not disqualify a sole drop. Tameability has NO data flag anywhere:
a tame line ships only on drop evidence AND core-guide corroboration,
else it is logged in `docs/companion-unverified.md`.

## RARES — 9 flagged (5 Rare + 4 Rare Elite), 6 shipped, 3 excluded

| NPC | Lvl | Rank | Point(s) | Sole-drop signature | Guide step |
|-----|-----|------|----------|---------------------|------------|
| 2744 Shadowforge Commander | 40 | 4 | (41.49, 29.75) single | none (generics only) | single goto + kill note |
| 2749 Siege Golem | 40 | 2 | 14 pts, west (5.49, 59.53) to (40.03, 39.82) | 282561 Siegebreaker's Blaster (sole dropper, rate unnumbered) | loop + collect |
| 2751 War Golem | 36 | 4 | 3 pts (45.36, 33.53 / 49.38, 12.06 / 52.41, 19.48) | none (generics only) | loop + kill note |
| 2752 Rumbler | 45 | 4 | 4 pts, far south-west (1.98, 80.52 / 4.77, 81.78 / 13.86, 86.11 / 14.73, 89.33) | 282556 Groundshaker's Bindings (sole dropper, rate unnumbered) | loop + collect + come-back-later note |
| 2850 Broken Tooth | 37 | 4 | 4 pts, east (45.8, 36.5 / 53.65, 15.53 / 59.68, 26.92 / 59.69, 29.37) | none (generics only; 4580 Sabertooth Fang 9.3% drops from ~20 beasts — beast evidence, not a signature) | loop + kill note, NO tame line |
| 7057 Digmaster Shovelphlange | 38 | 2 | (34.6, 23.1) single | 9375 Expert Goldminer's Helmet 10%, 9378 Shovelphlange's Mining Axe 15%, 9382 Tromping Miner's Boots 65% (sole dropper on all three) | single goto + collects |

Notes:
- No contracted quest references any of the 9 structurally (start/end/
  objectives/sourceItem scanned over the 13 Horde-contract quests): the
  710/713/714 and 656/664+ hits on 2850 are item-ID collisions, verified
  field by field (same finding as the Alliance inventory). Nothing
  shipped is core content; nothing core is duplicated. A rare whose
  only significance is a core-contracted NON-item-start quest is not
  companion content (Dun Morogh precedent) — none of the 9 qualifies:
  Tho'grun (2944), Blacklash (2757), Hematus (2759), Scorched Guardian
  (2726) and Scalding Whelp (2725) are all rank-null/rank-1 (NOT rare-
  flagged), so the exclusion never triggers here.
- Above-band handling, per band 30–40: Rumbler (+5, sole signature)
  ships with an honest come-back-later note (Duskwood Nefaru pattern,
  same call as Alliance). Anathemus (npc2754, lvl 45 Rare Elite,
  single pt (23.7, 74.16), sole 282560 Earth-Infused Rockguards) is
  EXCLUDED — a level-45 elite is group content no note can make
  soloable (same call as Alliance; faction-neutral reasoning).
  7:XT (npc14224, lvl 41 Rare, 7 pts) is EXCLUDED — +1 with no sole
  drops (Hillsbrad/Arathi +1 precedent, same call). Zaricotl (npc2931,
  lvl 55 Rare Elite, 3 pts) is EXCLUDED — 15 over band; its 100% drop
  4613 Corroded Black Box starts the same 708 chain the Alliance
  inventory names (Ironforge-contracted, Alliance-side) — for Horde
  that chain is off-faction anyway; the band alone excludes.
- Rumbler's generic-pattern drops are NOT collected: 8389 Pattern:
  Big Voodoo Pants (0.12% off Rumbler among ~200 droppers) and 9293
  Recipe: Magic Resistance Potion (0.12%) are multi-zone generic world
  drops (hundreds of droppers each, verified by full scan) — only the
  sole signature 282556 rides a collect. Anathemus's recipe drops
  (3868 Plans: Frost Tiger Blade, 7975 Plans: Heavy Mithril Pants,
  10300 Pattern: Red Mageweave Vest) are likewise multi-zone generic
  (100+ droppers each) — never companion content, stated not harmonized.
- Broken Tooth tame ruling (named check): drop evidence EXISTS (4580
  Sabertooth Fang 9.3%, a cat-family beast drop). Corroboration FAILS:
  `badlands-horde.guide` carries zero `only Hunter` lines (verified by
  grep — the guide has no class gates at all). Per the standing bar
  (drop evidence AND core-guide corroboration), NO tame line ships.
  Logged in `docs/companion-unverified.md` (Hillsbrad/Duskwood pattern,
  same outcome as Alliance for the same reason). All other shipped
  rares are elementals/golems (Siege, War, Rumbler), a dwarf
  (Shovelphlange) and a humanoid commander — no tameable families;
  7:XT is a mechanical ("Long Distance Recovery Unit"), also not a
  beast. Only Broken Tooth was ever a candidate.
- Respawn timers: unconfirmed anywhere in the data; none stated.
- All 9 rares are react-null (neutral to both factions) — no Falthis
  or Stonetalon faction ruling triggers on this key.

## ITEM-START HUNTS — none

The Horde core contract contains ZERO item-starts (explicit start-item
scan in `docs/badlands-horde-census.md`: the only start-item in the
pool, 12563 Warlord's Command, belongs to the OUT above-band 4903).
"There are therefore NO item-start hunts in this companions round" is
stated after the scan, not assumed. No rare drops an item starting a
Horde-contracted quest (verified: none of the 13 contract quests has
an item start at all).

## TREASURES

- Generic "Solid Chest": object 2857 (10 fixed pts, camp cluster +
  east/south: 13.87,74.93 / 29.52,56.32 / 40.59,26.03 / 40.70,28.21 /
  41.49,26.23 / 42.45,28.85 / 50.75,68.08 / 53.12,34.94 / 53.62,29.65 /
  62.69,70.29) and object 4149 (4 fixed pts, far south-west: 6.35,90.31
  / 7.60,96.13 / 7.97,85.73 / 9.57,93.38). ONE loop step over all 14
  fixed points, said plainly as generic chests. Loot tables are shared
  generics; no quest takes any of it.
- "Battered Footlocker" 179490 (6 pts, camp cluster ~(40-43, 26-31)):
  (40.50,28.00 / 41.30,29.29 / 41.38,26.16 / 41.45,29.97 /
  42.15,31.01 / 43.79,29.74) + "Dented Footlocker" 179492 (4 pts:
  40.72,28.07 / 40.81,28.67 / 41.07,27.40 / 42.31,28.41). ONE loop step
  over all 10 fixed points, said plainly. Loot is generic gems/food/
  potions (1529 Jade, 3864 Citrine, 1645/1707/1710/3771); the 2763 Art
  of the Imbue / 356 / 1948 refs to 1529 and 3864 are item-ID
  collisions in other zones' quests, not these objects.
- "Carved Stone Urn" 2743: 14 fixed pts (north band: 32.23,15.95 /
  33.19,13.80 / 34.09,18.52 / 34.12,21.53 / 34.72,23.94 / 34.98,22.10 /
  35.52,16.36 / 35.89,11.64 / 37.97,13.92 / 39.57,18.47 /
  39.79,19.67 / 40.62,12.09 / 40.99,16.01 / 42.81,9.95). Loop step.
  The urns hold item 4610 (4 needed by quest 704 Agmond's Fate,
  contracted NOWHERE — Loch Modan left the whole Agmond chain out);
  the step notes that honestly.
- "Garrett Family Chest" 124388: single pt (34.19, 18.63). Own
  single-goto step; holds 8026 Garrett Family Treasure. 8026 is the
  objective of Horde quest 2342 Reclaimed Treasures (Undercity accept,
  uncontracted — belongs to Undercity content, noted not duplicated):
  the step notes that honestly. (Alliance-inventory delta, flagged
  below: their "quest 1360 ... Undercity turnin" misattributes the
  twin — see below.)
- "Krom Stoutarm's Chest" 124389: single pt (35.56, 23.51). Own
  single-goto step; holds 8027 Krom Stoutarm's Treasure (quest 1360
  Reclaimed Treasures, Alliance-only, Ironforge-contracted): the step
  notes that (same treatment as Alliance).
- Pillars: 2842 "Pillar of Diamond" (83.54, 32.84), 2848 "Pillar of
  Opal" (72.32, 66.94), 2858 "Pillar of Amethyst" (81.33, 64.28).
  Three single-goto steps; each drops its runestone (4845/4844/4843),
  which quests 779/795 Seal of the Earth take — both out of contract
  (779 the contracted-out repeatable; 795 repeatable) — the steps note
  that honestly.
- "Seal of the Earth" 2933 (1 pt): EXCLUDED with argued reason. Unlike
  the three pillars (whose runestones are collectible items with steps),
  the Seal offers only the repeatable 795 accept itself — shipping a
  step there would route out-of-contract repeatable content. The
  contracted Thor story ends at 793; the Seal is repeatable-cycle
  furniture, logged not shipped. (The Alliance inventory neither ships
  nor logs it — flagged below.)
- Excluded with reason (core owns the arrow, Dun Morogh precedent):
  2875 "Battered Dwarven Skeleton" (contracted 734 object-start —
  shared, main-guide-routed for Horde too). 2867 "Excavation Supply
  Crate" and 2868 "Crumpled Map": NO container loot anywhere in the
  data — 2868 starts Alliance-only 720 (dead furniture for Horde);
  2867's only significance was the Alliance core's 718 arrow (718 is
  Alliance-only; Horde has no equivalent) — both logged, not shipped,
  with the Horde-derived reasons (genuine faction deltas, stated not
  harmonized). 126049 + 128293 "Magenta Cap Clusters" (Hor?-contracted
  2202's objective objects — core-routed, Dun Morogh). 126260 "Ancient
  Chest" (shared 709's complete sits on it — main-guide-routed for
  Horde too).
- 3707 Food Crate (12 pts), 3960 Burning Embers (1 pt), 128196 Magenta
  Cap Clusters Trap (2 pts): no container loot in the data (decor/trap
  furniture) — the herbs/veins/campfires/decor bucket, never shipped.
- No other fixed container spawns on 1418 (192 objects scanned; the
  rest are herbs, veins, campfires and decor with no container loot).

## RECIPES — 8 shipped (vendor 2 + drops 6)

Vendor-sold (both vendors react-null/neutral, physically in-zone; no
faction lock either way — the faction rule bites neither side here):
- Engineering, Yuka Screwspigot (9544) at (4.9, 94.7), far south-west:
  10602 Schematic: Deadly Scope (also sold by Knaz Blunderflame in
  Stranglethorn 1434 — Yuka is the in-zone source). Pin every buy
  `npc 9544`.
- Blacksmithing, Jazzrik (9179) at (42.47, 52.5), Kargath
  (Blacksmithing Supplies): 10858 Plans: Solid Iron Maul (also sold by
  Jannos Ironwill in Arathi 1417 and by neutral Muuran in Desolace
  1443 — Jazzrik is the in-zone source). Pin every buy `npc 9179`.
- No stock-class flag in the data, so no limited marking either way.

Dropped (sole dropper anywhere in the data, dropper spawns in-zone —
genuinely zone content, Hillsbrad/Redridge exclusive-drop precedent;
all six verified single-dropper by full scan):
- Blacksmithing 251389 Plans: Hard Gold Coif <- 2906 Dustbelcher
  Warrior (36; 5 pts (64.36, 23.75 / 65.52, 22.05 / 65.66, 23.49 /
  67.13, 22.09 / 68.08, 25.08)).
- Blacksmithing 251394 Plans: Shining Mithril Boots <- 2894 Stonevault
  Shaman (40; 5 pts (48.27, 68.28 / 49.53, 69.80 / 49.66, 66.49 /
  49.89, 68.38 / 50.94, 67.25)).
- Blacksmithing 251461 Plans: Mithril Claws <- 2893 Stonevault
  Bonesnapper (39; 14 pts around (47-52, 64-72)).
- Tailoring 254034 Pattern: Earthen Silk Shoulders <- 2907
  Dustbelcher Mystic (36; 4 pts (12.87, 73.34 / 64.69, 25.55 /
  66.33, 22.05 / 66.67, 23.29)).
- First Aid 255726 Manual: Leather Tourniquet <- 2739 Shadowforge
  Tunneler (35; 11 pts around (52-55, 30-34)).
- Enchanting 249512 Formula: Dreambough Wand <- 2720 Dustbelcher Ogre
  Mage (43; sole dropper anywhere, but the mob is 3 over band and
  spans 3 zones 1418/1427/1428): ships with an honest come-back-later
  note (Westfall Safety Sheep precedent), argued BORDERLINE and kept.

Excluded with reason:
- 5428 An Exotic Cookbook — 10 droppers in 5 zones (multi-zone
  generic); and its only in-zone dropper 8155 Kargath Grunt
  (`faction: H`, lvl 55, Kargath 5 pts) is Horde-friendly and 15 over
  band — unkillable by Horde players and out of band regardless.
  (Faction-field note: the operative flag is the npc `faction: H`
  field, not reactH/reactA which read null — recorded here since the
  Alliance round cited it loosely.)
- 217271 Pattern: Turtle Scale Gloves — Tanaris-precedent multi-zone
  generic (argued there, not re-argued here).
- All other recipe drops: the full scan (734 drop-recipes) finds up
  to 646 droppers across up to 32 zones — everything not shipped here
  is multi-zone generic, excluded as a class under the Elwynn rule.
  Corroborating completeness: the recipes whose droppers spawn ONLY on
  1418 are exactly the 6 shipped narrow drops above (each a sole
  dropper); no other recipe is 1418-only.
- 3868/7975/10300 (Anathemus's Frost Tiger Blade / Heavy Mithril
  Pants / Red Mageweave Vest): each drops from 100+ mobs — generic,
  never companion content. (A reader seeing them on Anathemus's table
  might expect a recipe step; the scan says no.)
- 8389 Pattern: Big Voodoo Pants + 9293 Recipe: Magic Resistance
  Potion (Rumbler 0.12%): each drops from ~200 mobs — generic, so
  Rumbler's step collects ONLY the sole signature 282556 (Duskwood
  precedent: collect the signature, not the generics).
- Quest-reward recipes: quest records carry no reward data — never
  shipped, logged in the inventory (same class as Alliance).
- Trainer-taught staples excluded (Polestar's own profession guides).

Professions with NO in-zone Horde source, stated plainly in the
guide (Dun Morogh Blacksmithing precedent): Alchemy, Cooking, Fishing,
Leatherworking. (Leatherworking 5145 is a core quest gated on the
trade, not a recipe source — same distinction as Alliance.)

## TAMEABLES — none shipped

Only Broken Tooth is a tameable beast family among the shipped rares;
the bar (drop evidence AND core-guide corroboration) fails on the
second half as ruled above. Logged in `docs/companion-unverified.md`.
(The 7:XT "Long Distance Recovery Unit" is mechanical, not a beast.)

## ALLIANCE-DELTA FLAGS (for docs/companion-unverified.md, never
harmonized)

1. Guide headers/titles/bands are faction-mirrored (28-40 Alliance vs
   30-40 Horde) — structural, not a data delta.
2. Dustbelcher Mystic NPC ID: the Alliance inventory cites 2707
   (which is Shadra, lvl 55, no 1418 spawn); the data's 1418
   Dustbelcher Mystic is 2907 (lvl 36, the 4 listed points). Points
   agree; the ID is corrected here.
3. Garrett chest attribution: the Alliance inventory's "quest 1360
   ... Undercity turnin" conflates the same-name twins — 1360
   Reclaimed Treasures is Alliance-only (Ironforge, takes 8027
   only); the chest's 8026 is the objective of HORDE quest 2342
   Reclaimed Treasures (Undercity accept, uncontracted). Named here
   per ID.
4. 8155 Kargath Grunt's Horde-friendliness lives in its `faction: H`
   field (reactH/reactA read null) — recorded precisely since the
   Alliance round cited it loosely. Outcome identical (OUT).
5. 2933 Seal of the Earth: unshipped here with an argued reason; the
   Alliance inventory neither ships nor logs it — logged here so the
   absence is deliberate, not an oversight.
6. 2867 Excavation Supply Crate reasoning differs by faction (no loot
   in the data either way; for Horde there is additionally no core
   arrow since 718 is Alliance-only) — same outcome (OUT), honest
   reasons differ.
7. Vendor-pin rule (`npc <id>` on every buy) is a standing rule the
   Alliance file predates — the Horde guides pin; no content
   contradiction.
