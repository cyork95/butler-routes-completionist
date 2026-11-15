# Thousand Needles companions inventory (game data, accept-zone key 1441)

Source: local Forever game data (questie-forever NPC/object/item dumps).
Rank semantics calibrated in earlier rounds. All 7 flagged rares are plain
rank "rare" with explicit roles ["rare"]; all are faction null (neutral
spawns, no Horde lock). Loot "sole dropper" means the item's drops.npc
lists only this NPC and no object source. Tameability has NO data flag
anywhere: a tame line ships only on drop evidence PLUS core-guide
corroboration, else it is logged in docs/companion-unverified.md.

## RARES — 7 flagged, 7 shipped

| NPC | Lvl | Point(s) | Sole-drop signature | Guide step |
|-----|-----|----------|---------------------|------------|
| 5933 Achellios the Banished | 31 | 1 pt (22.73,37.46) | 285191 Banished Centaur's Pauldrons | single + collect |
| 5934 Heartrazor | 32 | 1 pt (16.75,41.49) | 285190 Wyvern Heart Band | single + collect |
| 14426 Harb Foulmountain | 27 | 1 pt (32.55,26.78) | 285212 Foulmountain Family Hammer | single + collect |
| 14427 Gibblesnik | 28 | 1 pt (55.62,50.45) | 285192 Kobold Firestarter | single + collect |
| 5937 Vile Sting | 35 | 1 pt (70.55,72.92) | 285177 Nature's Sting Legguards | single + collect + venom note |
| 4132 Silithid Ravager | 37 | 3 pts, Shimmering Flats east (67-70,82-86) | 8224 Silithid Ripper | loop + collect + come-back note |
| 5935 Ironeye the Invincible | 37 | 1 pt (87.19,78.39) | 8223 Blade of the Basilisk | single + collect + come-back note |

Notes:
- No core-contracted quest references any shipped rare structurally
  (start/end/kill scanned over the 34-contract quests; objective types in
  this zone's data are only item/kill and every kill target was checked).
  No shipped rare is a giver, ender, or objective of any core quest.
- One real loot overlap, handled by the Baron Marinous pattern: Vile Sting
  drops 5794 Salty Scorpid Venom, the objective item of contracted core
  quest 1104 Salt Flat Venom — alongside two common in-zone scorpids
  (4139 Scorpid Terror, 4140 Scorpid Reaver), so the core quest never
  depends on the rare. The step carries a note naming the quest and
  pointing at the core guide; the hunt lives here, the accept/turnin
  lives there.
- Above-band handling (band 25-35, Westfall/Hillsbrad/Duskwood
  precedents — excluded, or shipped with an honest come-back-later note
  when a sole-drop signature argues for it): Silithid Ravager (+2, sole
  Ripper) and Ironeye the Invincible (+2, sole Basilisk blade) SHIP with
  come-back notes — reachable signatures, not group content (the milder
  end of the Akubar +4 / Magronos +6 Blasted Lands precedent). Vile
  Sting sits exactly at the band top (35) and ships as normal.
- Tameability: no tame lines ship. The core guide carries zero `only
  Hunter` lines, so the corroboration half is unmet for everything
  (Silithid Ravager, Heartrazor, Vile Sting included). Logged in
  docs/companion-unverified.md.
- Respawn timers: unconfirmed anywhere in the data; none stated.

## TREASURES

- Generic "Solid Chest": object 2852 (14 fixed pts: west cluster
  13.94,38.82 / 17.63,41.79 / 17.84,21.29 / 18.56,20.9 / 18.92,23.23 /
  19.36,21.74, north cluster 26.58,54.02 / 27.18,52.55, east-center
  cluster 42.21,31.7 / 42.24,37.39 / 42.94,39.31 / 43.02,36.81 /
  43.45,33.28 / 44.91,32.27) and object 2855 (4 fixed pts, Shimmering
  Flats 65.25,87 / 68.47,82.95 / 69.69,85.84 / 71.2,85.19). ONE loop
  step over all 18 fixed points, said plainly as generic chests. No
  contract quest takes either chest as an object (quest-JSON hits on
  2852/2855 are item-ID collisions — e.g. 404's objective is ITEM 2855
  "Putrid Claw", not the chest object).
- Excluded with reason (decor/scenery, no loot in the data, no quest
  links): 19861 "Henrig Lonebrow's Journal" (1 pt), 19878 "Parts Crate"
  (1 pt), 19897 "Cask of Fool's Stout" (1 pt), 20447 "Harpy Foodstuffs"
  (1 pt), 19868-19873 "Rocket Car Rubble" series (76-103 pts each —
  Mirage Raceway wreckage scenery). Object 20805 "Rizzle's Unguarded
  Plans" is core-contracted content (quests 1190/1194, and 1190 is the
  documented no-turn-in record) — the core guide owns it, not this one.
  Mines/herbs/veins are gathering nodes, not companion treasure.

## RECIPES — 9 shipped (4 vendor + 5 drop)

- Tailoring, Brienna Starglow (7,18, Tailoring Supplies, faction A —
  Alliance-safe; 2 of the 3 vendors selling it are elsewhere): 7089
  Pattern: Azure Silk Cloak.
- Engineering, Jinky Twizzlefixxit (77.68,77.9, Mirage Raceway, faction
  AH neutral — buyable by Alliance; each sold by 2 vendors total):
  7560 Schematic: Gnomish Universal Remote, 13309 Schematic: Lovingly
  Crafted Boomstick. One step per source, so one step carries both buys.
  (7560 additionally lists sourceless dropper 7800 Mekgineer Thermaplugg
  with no spawn data anywhere — unplaceable, so buy-only, said plainly.)
- Engineering, Maximillian "The Greaser" (79.8,77.2, Mirage Raceway,
  faction AH neutral; SOLE vendor anywhere): 221336 Schematic: Goblin
  Mining Helmet.
- Blacksmithing, in-zone mob drops: 251385 Plans: Hard Gold Cuirass <-
  4101 Screeching Roguefeather (sole dropper, 1441-only, 11 pts);
  251457 Plans: Steel Spear <- 4151 Saltstone Crystalhide (sole
  dropper, 1441-only, 40 pts); 251339 Plans: Sterling Silver
  Breastplate <- 10758 Grimtotem Bandit (sole dropper, 1413+1441, 7
  TN pts — narrow 2-zone drop, shipped with both zones named).
- Alchemy, in-zone mob drop: 250389 Recipe: Elixir of Intellect <-
  4095 Galak Mauler (sole dropper, 1413+1441, 21 TN pts — narrow
  2-zone drop, shipped with both zones named).
- Leatherworking, in-zone mob drop: 254000 Pattern: Earthen Leggings
  <- 4116 Gravelsnout Surveyor (sole dropper; 5 TN pts + 1 Feralas pt
  — the TN loop covers the 5 in-zone points and the note names the
  Feralas point).
- Excluded with reason: 5973 Pattern: Barbaric Leggings (in-zone vendor
  4877 Jandia is faction H — Horde-only, Alterac precedent) and 6068
  Recipe: Shadow Oil (in-zone vendor 4878 Montarr is faction H);
  253665 Pattern: Linen Reagent Bag + 253668 Pattern: Woolen Reagent
  Bag (34 vendors each — generic tailoring-supplier stock, Elwynn rule
  by analogy despite the in-zone vendor); 5773 Pattern: Robes of Arcana
  (3 droppers across 4 zones incl. Duskwood and Darkshore — a world
  drop, not zone content); everything else on the list (multi-hundred
  droppers across ~30 zones each, Elwynn rule — worked example: 3870
  Plans: Green Iron Shoulders names in-zone Heartrazor among 382
  droppers in 29 zones, so in-zone drop alone does not make zone
  content).
- Quest-reward recipes: quest records carry no reward data — none
  shipped, class-logged in companion-unverified.
- Trainer-taught staples excluded (Polestar's own profession guides).

Professions with NO Thousand Needles source (stated plainly in the
guide, Dun Morogh Blacksmithing precedent): Cooking, Enchanting,
First Aid, Fishing.
