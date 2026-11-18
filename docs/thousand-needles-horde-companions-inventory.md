# Thousand Needles (Horde) companions inventory (game data, accept-zone key 1441)

Source: local Forever game data (questie-forever NPC/object/item dumps), same
build the Alliance inventory used. Rank semantics as before: rank 2/4 with
roles ["rare"]. All 7 flagged TN rares are faction null (neutral spawns, no
Horde lock) — no Falthis-type exclusion. Loot "sole dropper" means the item's
drops.npc lists only that NPC and no object source, verified per item below
(all 7 Alliance-reported signatures re-verified sole in this build).
Tameability has NO data flag anywhere: a tame line ships only on drop
evidence PLUS core-guide corroboration, else it is logged in
docs/companion-unverified.md. The Horde core guide
(`thousand-needles-horde.guide`) carries zero `only Hunter` lines, so the
corroboration half is unmet for everything.

Horde band is 20-32 (Alliance ran 25-35). Above-band handling per
Westfall/Hillsbrad/Duskwood: a rare a few levels above band ships with an
honest come-back-later note when a sole-drop signature argues for it
(the Blasted Lands Akubar +4 / Magronos +6 end of the scale); far-above-band
would be excluded. Nothing here is far above: the three overs (+3, +5, +5)
all ship with notes.

## RARES — 7 flagged, 7 shipped

| NPC | Lvl | Point(s) | Sole-drop signature | Guide step |
|-----|-----|----------|---------------------|------------|
| 5933 Achellios the Banished | 31 | 1 pt (22.73,37.46) | 285191 Banished Centaur's Pauldrons | single + collect |
| 5934 Heartrazor | 32 | 1 pt (16.75,41.49) | 285190 Wyvern Heart Band | single + collect; tame logged unverified (wyvern, no core Hunter corroboration) |
| 14426 Harb Foulmountain | 27 | 1 pt (32.55,26.78) | 285212 Foulmountain Family Hammer | single + collect |
| 14427 Gibblesnik | 28 | 1 pt (55.62,50.45) | 285192 Kobold Firestarter | single + collect |
| 5937 Vile Sting | 35 | 1 pt (70.55,72.92) | 285177 Nature's Sting Legguards + shared 5794 note (below) | single + collect + come-back note (+3 over band top) |
| 4132 Silithid Ravager | 37 | 3 pts, Flats east (67.26,86.1 / 68.38,82.32 / 70.03,86.22) | 8224 Silithid Ripper | loop + collect + come-back note (+5) |
| 5935 Ironeye the Invincible | 37 | 1 pt (87.19,78.39) | 8223 Blade of the Basilisk | single + collect + come-back note (+5) |

Notes:
- No shipped rare is a giver, ender, or objective of any Horde-core-contracted
  quest (start/end/kill scanned over the 26-contract quests; the same check
  the Alliance inventory ran over its 34).
- Loot overlap, Baron Marinous pattern: Vile Sting drops 5794 Salty Scorpid
  Venom (16%) alongside two common in-zone scorpids (4139 Scorpid Terror,
  4140 Scorpid Reaver). The venom is the objective of 1104 Salt Flat Venom,
  contracted in the MAIN guide (shared) — the Horde player sees it through
  the ungated main file, so the step carries a note naming the quest and
  pointing at the main guide; the hunt lives here, the accept/turnin there.
- Tameability: no tame lines ship (zero `only Hunter` lines in the Horde
  core). Heartrazor (wyvern) and Vile Sting (scorpid) logged in
  docs/companion-unverified.md. Silithid/basilisk/centaur/kobold families
  are not tameable game; Achellios/Harb/Gibblesnik/Ravager/Ironeye need no
  log entry beyond this line.
- Respawn timers: unconfirmed anywhere in the data; none stated.
- Excluded with reason (not rares, no own loot): 216474 Ravaging Tempest
  (rank 1, no rare flag; sole significance is Horde-core 79366's Eye
  objective — Dun Morogh precedent, core owns it); 4499 Rok'Alim the
  Pounder (no rare flag; 1150 is a Dorn NPC-accept, NOT an item-start —
  the brief's "Rok'Alim starter" attribution is overturned by the data:
  the core routes `accept 1150` from Dorn Plainstalker); 10617 Galak
  Messenger (no rare flag; starter-dropper for 4881 — ships as a hunt,
  below, not as a rare).

## ITEM-START HUNTS (Horde core: 1148, 4881)

The Horde core's item-started quests are 1148 and 4881. The brief also
named 4821, 1150 and 79366 as item-starts — the data overturns all three:
4821 Alien Egg and 1150 Test of Endurance are plain NPC accepts (Hagar
Lightninghoof and Dorn Plainstalker; the core routes both as accepts),
and 79366 Heed My Call is a Prate NPC-accept whose Eye (item 212792) is
an OBJECTIVE off the rank-1 Ravaging Tempest (excluded above). No hunts
for those three; the inventory records the correction so the delta is
auditable.
- 4881 Assassination Plot: starter 12564 Assassination Note, 100% drop
  off 10617 Galak Messenger, in-zone point (39.43,33.1) — the point the
  core guide already uses. Hunt step: kill + optional collect 12564 + a
  note pointing at the core guide (accept/turnin live there).
- 1148 Parts of the Swarm: starter 5877 Cracked Silithid Carapace, 50%
  off the 4130-4133 Silithid family (Searcher 5 pts, Invader 8 pts, Hive
  Drone 24 pts, Ravager 3 pts — all south, 63-72/81-89). Hunt step: loop
  over the family grounds + optional collect 5877 + pointer note. (The
  Intact Carapace 5853 is the 80% parallel drop, not the starter.)
- 94930 Lost Shipping Crate (OUT, above-band m36 — not contracted):
  starter crate object 658117 data-placed @45.33,49.18 on 1441, turn-in
  Friz Frazzlespark in the Riverglades. The census flagged it for this
  round: it ships as a note-only step (goto + honest above-band note,
  come back at 36) — no accept/turnin, companions never carry quest lines.

## TREASURES

- Generic "Solid Chest": object 2852 (14 fixed pts: west cluster
  13.94,38.82 / 17.63,41.79 / 17.84,21.29 / 18.56,20.9 / 18.92,23.23 /
  19.36,21.74, north cluster 26.58,54.02 / 27.18,52.55, east-center
  cluster 42.21,31.7 / 42.24,37.39 / 42.94,39.31 / 43.02,36.81 /
  43.45,33.28 / 44.91,32.27) and object 2855 (4 fixed pts, Shimmering
  Flats 65.25,87 / 68.47,82.95 / 69.69,85.84 / 71.2,85.19). Points
  byte-identical to the Alliance inventory's list, re-dumped here. ONE
  loop step over all 18 fixed points, said plainly as generic chests. No
  contract quest takes either chest as an object (quest-JSON hits on
  2852/2855 are item-ID collisions — e.g. 404's objective is ITEM 2855
  "Putrid Claw"; verified by record shape, same as the Alliance finding).
- Excluded with reason: 19861 Journal, 19878 Parts Crate, 19897 Cask,
  20447 Harpy Foodstuffs, 19868-19873 Rocket Car Rubble series (Mirage
  Raceway wreckage scenery); 20805/179888 Rizzle's Plans (core 1190/
  1194); 176115 Wanted Poster (core 5147's accept object); 175565/175567
  Alien Egg objects + 175384 Wyvern Egg (core-quest furniture/scenery —
  4821's accept is Hagar, not the objects); 176344/190483/190484 Document
  Chests (Horde-core 5064's Secret-Note furniture — the core owns them);
  423895 Scrolls (start-object of 79947, an uncontracted Undercity-zone
  quest — quest furniture for content in no contract); 20737 barrel
  (quest link is the ITEM id — Singed Corestone for L60 AQ repeatables
  8530/8617; the object itself is scenery); seasonals (pumpkins, ghost,
  candy, bats, apples); MFF fireworks and raceway panels (scenery);
  elevators/taxi signs (travel furniture); mines/herbs/veins (gathering
  nodes, not companion treasure). 421568 Weathered Cache, 423920
  Warrior's Bounty, 423930 Sizable Stolen Strongbox, 499988 Spellbook,
  89635 Sunscorched Shell (9 pts), 92423 Damaged Chest: fixed spawns with
  no loot table and no quest link anywhere in the data — unscopable as
  treasure (nothing to goal at), logged here, not shipped (Deadwind/Gaea
  precedent applied to lootless fixed objects).

## RECIPES — 9 shipped (4 vendor + 5 drop)

- Tailoring, Jandia 4877 (Horde, Freewind Post @46.21,51.51 — SOLE
  in-zone vendor): 5973 Pattern: Barbaric Leggings. Genuine faction
  difference: the Alliance guide excluded this vendor (Horde-only) and
  shipped Brienna's 7089 instead — stated, not harmonized.
- Alchemy, Montarr 4878 (Horde, Freewind Post @45.15,50.79 — SOLE
  in-zone vendor): 6068 Recipe: Shadow Oil. Same faction-difference shape
  as 5973.
- Alchemy, in-zone mob drop: 250389 Recipe: Elixir of Intellect <-
  4095 Galak Mauler (sole dropper; 1413+1441 — both zones named).
- Engineering, Jinky Twizzlefixxit 6730 (neutral, Mirage Raceway
  @77.68,77.9): 7560 Schematic: Gnomish Universal Remote, 13309
  Schematic: Lovingly Crafted Boomstick. One step carries both buys.
  (7560 additionally lists sourceless dropper 7800 Mekgineer Thermaplugg
  with no spawn data anywhere — unplaceable, so buy-only, said plainly.)
- Engineering, Maximillian "The Greaser" 222261 (neutral, Mirage
  Raceway @79.8,77.2 — SOLE vendor anywhere): 221336 Schematic: Goblin
  Mining Helmet.
- Blacksmithing, in-zone mob drops: 251385 Plans: Hard Gold Cuirass <-
  4101 Screeching Roguefeather (sole dropper, 1441-only, 11 pts);
  251457 Plans: Steel Spear <- 4151 Saltstone Crystalhide (sole
  dropper, 1441-only, 40 pts); 251339 Plans: Sterling Silver
  Breastplate <- 10758 Grimtotem Bandit (sole dropper, 1413+1441, 7 TN
  pts — both zones named).
- Leatherworking, in-zone mob drop: 254000 Pattern: Earthen Leggings
  <- 4116 Gravelsnout Surveyor (sole dropper; 5 TN pts + 1 Feralas pt —
  the loop covers the 5 in-zone points and the note names Feralas).
- Excluded with reason: 7089 Pattern: Azure Silk Cloak (in-zone vendor
  6576 Brienna Starglow is faction A — Alliance-only, Alterac rule
  flipped); 253665/253668 Linen/Woolen Reagent Bag (34 vendors each —
  generic stock, Elwynn rule); 5773 Pattern: Robes of Arcana (3 droppers
  across 3 zones: 910 Duskwood, 2337 Darkshore, 10760 here — a world
  drop, not zone content); everything else recipe-dropping in-zone
  (143 candidates scanned) drops across dozens of zones each — generic
  world drops, NOT zone content (Elwynn rule).
- Quest-reward recipes are unverifiable from data — none shipped, class
  logged in companion-unverified.
- Trainer-taught staples excluded (Polestar's own profession guides).

Professions with NO Thousand Needles Horde source (stated plainly in
the guide, Dun Morogh precedent): Cooking, Enchanting, First Aid,
Fishing.

## Deltas vs the Alliance inventory (flagged, never harmonized)

1. Horde additions: 5973 + 6068 (Horde-vendor exclusives the Alliance
   guide excluded by faction; this guide ships them).
2. Horde subtraction: 7089 (Alliance-vendor exclusive the Alliance
   guide shipped; this guide excludes it by faction).
3. Band shift 25-35 -> 20-32: Vile Sting sits +3 over the Horde top
   (at-band for Alliance) — ships with a come-back note either way;
   Ravager/Ironeye +5 (were +2) — still ship with notes per the
   Blasted Lands +4/+6 end of the scale, not group content.
4. Brief corrections (data over brief, recorded above, not Alliance
   deltas): 4821/1150 are NPC accepts; 79366 is an NPC accept with an
   objective Eye; 4881 (not 4821) is the Assassination Note item-start.
