# Badlands companions inventory (game data, accept-zone key 1418)

Source: local Forever game data (questie-forever NPC/object/item dumps).
Rank semantics calibrated in earlier rounds: rank 4 = Rare, rank 2 = Rare
Elite. Loot "sole dropper" means the item's drops.npc lists only this NPC
and no object source. Rates shown where the data gives a number; a null rate
does not disqualify a sole drop (Feralas/Tanaris calibration). Tameability has
NO data flag anywhere: a tame line ships only on drop evidence PLUS core-guide
corroboration, else it is logged in docs/companion-unverified.md.

## RARES — 9 flagged (6 Rare + 3 Rare Elite), 6 shipped, 3 excluded

| NPC | Lvl | Rank | Point(s) | Sole-drop signature | Guide step |
|-----|-----|------|----------|---------------------|------------|
| 2744 Shadowforge Commander | 40 | 4 | (41.49,29.75) single | none (generics only) | single goto + kill note |
| 2749 Siege Golem | 40 | 2 | 14 pts, west (5.49,59.53) to (40.03,39.82) | 282561 Siegebreaker's Blaster | loop + collect |
| 2751 War Golem | 36 | 4 | 3 pts (45.36,33.53 / 49.38,12.06 / 52.41,19.48) | none (generics only) | loop + kill note |
| 2752 Rumbler | 45 | 4 | 4 pts, far south-west (1.98,80.52 / 4.77,81.78 / 13.86,86.11 / 14.73,89.33) | 282556 Groundshaker's Bindings | loop + collect + come-back-later note |
| 2850 Broken Tooth | 37 | 4 | 4 pts, east (45.8,36.5 / 53.65,15.53 / 59.68,26.92 / 59.69,29.37) | none (generics only; 4580 Sabertooth Fang 9.3% is beast evidence, not a signature) | loop + kill note, NO tame line |
| 7057 Digmaster Shovelphlange | 38 | 2 | (34.6,23.1) single | 9375 Expert Goldminer's Helmet 10%, 9378 Shovelphlange's Mining Axe 15%, 9382 Tromping Miner's Boots 65% | single goto + collects |

Notes:
- No contracted quest references any of the 9 structurally (start/end/
  objectives/sourceItem scanned over the 35-contract quests): the 3 loose
  xref hits on 2850 (quests 710/713/714) are item-ID collisions, verified
  field by field. Nothing shipped is core content; nothing core is duplicated.
- Above-band handling, per rare (band 28-40, Westfall/Hillsbrad/Duskwood
  precedents — above band ships only with a sole-drop signature arguing for
  it): Rumbler (+5, sole signature) ships with an honest come-back-later
  note (Duskwood Nefaru pattern). Anathemus (npc2754, lvl 45 Rare Elite,
  single pt (23.7,74.16), sole 282560 Earth-Infused Rockguards, no quest
  takes it) is EXCLUDED — a level-45 elite is group content no note can make
  soloable. 7:XT (npc14224, lvl 41, 7 pts, no sole drops) is EXCLUDED — +1
  with no signature, Hillsbrad/Arathi +1 precedent. Zaricotl (npc2931, lvl
  55 Rare Elite, 3 pts) is EXCLUDED — 15 over band; its 100% drop 4613
  Corroded Black Box starts quest 708 The Black Box, which IS contracted in
  the Ironforge city guide, so the finding points there and no step ships here.
- Tameability: Broken Tooth drops 4580 Sabertooth Fang (9.3%) — beast
  evidence — but badlands.guide carries zero `only Hunter` lines, so the
  corroboration half of the rule is unmet. No tame lines ship; logged in
  docs/companion-unverified.md (Hillsbrad/Duskwood pattern). All other
  shipped rares are elemental/golem/dwarf shapes or humanoids.
- Respawn timers: unconfirmed anywhere in the data; none stated.
- All 9 rares are faction null (neutral spawns, no Horde lock).

## TREASURES

- Generic "Solid Chest": object 2857 (10 fixed pts, camp cluster +
  east/south) and object 4149 (4 fixed pts, far south-west). ONE loop step
  over all 14 fixed points, said plainly as generic chests. Loot tables are
  shared greens (791/863/864/etc.); no quest takes any of it.
- "Battered Footlocker" 179490 (6 pts) + "Dented Footlocker" 179492 (4 pts),
  one camp cluster ~(40-44, 26-31). ONE loop step over all 10 fixed points,
  said plainly. Loot is generic gems/food/potions (1529 Jade, 3864 Citrine,
  1645/1707/1710/3771); the 2763 Art of the Imbue / 356 / 1948 refs to 1529
  and 3864 are item-ID collisions in other zones' quests, not these objects.
- "Carved Stone Urn" 2743: 14 fixed pts (north band). Loop step. The urns
  hold item 4610 (4 needed by quest 704 Agmond's Fate, contracted NOWHERE —
  Loch Modan left the whole Agmond chain out); the step notes that honestly.
- "Garrett Family Chest" 124388: single pt (34.19,18.63). Own single-goto
  step; holds 8026 Garrett Family Treasure (quest 2342 Reclaimed Treasures,
  Undercity turn-in, no guide contracts it — note says so).
- "Krom Stoutarm's Chest" 124389: single pt (35.56,23.51). Own single-goto
  step; holds 8027 Krom Stoutarm's Treasure (quest 1360 Reclaimed Treasures,
  contracted in the IRONFORGE city guide — note points there).
- Pillars: 2842 "Pillar of Diamond" (83.54,32.84), 2848 "Pillar of Opal"
  (72.32,66.94), 2858 "Pillar of Amethyst" (81.33,64.28). Three single-goto
  steps; each drops its runestone (4845/4844/4843), which quests 779/795
  Seal of the Earth take — both out of contract (779 the contracted-out
  repeatable) — the steps note that honestly.
- Excluded with reason (core owns them, Dun Morogh precedent): 2868
  "Crumpled Map" (contracted 716 objective + 720 object-start), 2875
  "Battered Dwarven Skeleton" (contracted 739 object-start), 2867 "Supply
  Crate" (core complete 718 sits exactly on its point (66.6,22)), 126260
  "Ancient Chest" (core complete 709 sits exactly on its point
  (39.34,18.82)). No step duplicates a core arrow; the two family chests
  above are the only quest-linked containers that ship, with notes.
- 192 objects spawn in the zone; the rest are herbs, veins, campfires and
  decor with no container loot in the data.

## RECIPES — 8 shipped (vendor 2 + drops 6)

Vendor-sold (both vendors Alliance-safe, no Horde-only vendor in the set;
no stock-class flag in the data, so no limited marking):
- Engineering, Yuka Screwspigot (4.9,94.7, far south-west; also spawns in
  zone 1428 — the Badlands spawn is the in-zone source): 10602 Schematic:
  Deadly Scope (also sold by Knaz Blunderflame in Stranglethorn 1434).
- Blacksmithing, Jazzrik (42.47,52.5, Blacksmithing Supplies): 10858 Plans:
  Solid Iron Maul (also sold by Jannos Ironwill in Arathi 1417 and the
  Horde-faction Muuran in Desolace 1443 — Jazzrik is the Alliance in-zone
  source, Alterac precedent).

Dropped (sole dropper anywhere, dropper spawns in-zone — genuinely zone
content, Hillsbrad/Redridge exclusive-drop precedent):
- Blacksmithing 251389 Plans: Hard Gold Coif <- 2906 Dustbelcher Warrior
  (36; 5 pts around (64-68,22-25)).
- Blacksmithing 251394 Plans: Shining Mithril Boots <- 2894 Stonevault
  Shaman (40; 5 pts around (48-51,66-70)).
- Blacksmithing 251461 Plans: Mithril Claws <- 2893 Stonevault Bonesnapper
  (39; 14 pts around (47-52,64-72)).
- Tailoring 254034 Pattern: Earthen Silk Shoulders <- 2907 Dustbelcher
  Mystic (36; 4 pts (12.87,73.34) + (64-67,22-26)).
- First Aid 255726 Manual: Leather Tourniquet <- 2739 Shadowforge Tunneler
  (35; 11 pts around (52-55,30-34)).
- Enchanting 249512 Formula: Dreambough Wand <- 2720 Dustbelcher Ogre Mage
  (43; 10 pts around (7-10,85-92)) — sole dropper anywhere, but the mob is
  3 over band and spans 3 zones: ships with an honest come-back-later note
  (Westfall Shafety Sheep precedent), argued BORDERLINE and kept.

Excluded with reason:
- 5428 An Exotic Cookbook — 10 droppers in 5 zones (multi-zone generic),
  and its only in-zone dropper 8155 Kargath Grunt is Horde-faction (fac H)
  and level 55: double reason, Alterac precedent.
- 217271 Pattern: Turtle Scale Gloves — 32 droppers, 9 zones: explicit
  Tanaris-precedent multi-zone generic (argued there, not re-argued here).
- All other recipe drops (100+ lines scanned): 25–640 droppers across
  8–32 zones each — generic world drops under the Elwynn rule, excluded as
  a class (full scan in temp work files, counts per line).
- Quest-reward recipes: quest records carry no reward data — none shipped,
  class-logged in companion-unverified.
- Trainer-taught staples excluded (Polestar's own profession guides).

Professions with NO Badlands source (stated plainly in the guide, Dun
Morogh Blacksmithing precedent): Alchemy, Cooking, Fishing, Leatherworking.
