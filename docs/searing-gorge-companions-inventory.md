# Searing Gorge companions inventory (game data, accept-zone key 1427)

Source: local Forever game data (questie-forever NPC/object/item dumps).
All 9 flagged rares carry explicit roles ["rare"] and are faction null
(neutral spawns, no Horde lock). Loot "sole dropper" means the item's
drops.npc lists only this NPC and no object source. Tameability has NO
data flag anywhere: a tame line ships only on drop evidence PLUS
core-guide corroboration, else it is logged in
docs/companion-unverified.md. Objective types in this zone's data are
only item/kill/object, and every kill target of the 39-contract quests
was checked exactly.

## RARES — 9 flagged, 9 shipped

| NPC | Lvl | Point(s) | Sole-drop signature | Guide step |
|-----|-----|----------|---------------------|------------|
| 8279 Faulty War Golem | 46 | 5 pts, center-west to center (32-60,41-68) | none (generics only) | loop + kill note |
| 8280 Shleipnarr | 47 | 1 pt (58.57,56.55) | 282631 Xorothian Footwraps | single + collect |
| 8277 Rekk'tilac | 48 | 5 pts, west to east (30-62,28-73) | none (generics only) | loop + kill note |
| 8281 Scald | 49 | 2 pts (35.95,55.74 / 51.15,46.84) | none (generics only) | loop + kill note + overlap note |
| 8283 Slave Master Blackheart | 50 | 5 pts, center-north (41-46,23-44) | 282094 Blackheart's Vest | loop + collect |
| 8282 Highlord Mastrogonde | 51 | 4 pts, west (14-30,26-37) | 282633 Mastrogonde's Sinister Gown | loop + collect |
| 8278 Smoldar | 50 | 1 pt (29.53,62.44) | none (generics only) | single + kill note + overlap note |
| 8924 The Behemoth | 50 | 1 pt (25.6,87.7) | 11603 Vilerend Slicer | single + collect + note |
| 9046 Scarshield Quartermaster | 55 | 1 pt (43.3,99.2, Blackrock Mountain frame) | 13248 Burstshot Harquebus + 13254 Astral Guard + 18987 Blackhand's Command | single + collects + come-back note + bank note |

Notes:
- No core-contracted quest gives, ends at, or objectives any shipped
  rare (start/end/kill scanned exactly over the 39-contract quests).
- Real loot overlaps, handled by the Baron Marinous pattern (notes
  pointing at the core guide; the hunts live here): Smoldar drops 7075
  Core of Earth (5144 objective, many sources); Scald drops 7077 Heart
  of Fire and 10509 Heart of Flame (5144/3442 objectives, many
  sources); the Behemoth drops 11446 A Crumpled Up Note (4264's start
  item, 78 droppers) — the note names the 4264 chain and points at the
  core guide, which owns the accept/turnin.
- Above-band handling (band 40-52, Westfall/Hillsbrad precedent):
  Quartermaster (+3) SHIPS with a come-back note — three sole
  signatures argue for it (Magronos/Akubar end of the precedent range,
  not group content), plus a bank-it-for-later note for 18987, which
  starts the endgame Blackhand chain the pack does not route yet (the
  Loch Modan figurine precedent: the companion never accepts or turns
  in). No other shipped rare is above-band.
- The four no-sole rares (Rekk'tilac, Smoldar, Faulty War Golem, Scald)
  are all in-band and ship as kill-note rares (Fingat pattern: generic
  loot only, no quest items of their own, no quest links — pure
  kill-note rares with overlap notes where the data shows one).
- Tameability: no tame lines ship. The core guide carries zero `only
  Hunter` lines, so the corroboration half is unmet for everything;
  the shared tables show no beast-family evidence. Logged in
  docs/companion-unverified.md.
- Respawn timers: unconfirmed anywhere in the data; none stated.

## TREASURES

- Generic "Solid Chest", object 4149 (15 fixed pts: 17.64,38.08 /
  25.87,24.7 / 28.66,24.83 / 35.93,58.81 / 37.58,49.18 / 37.92,38.98 /
  40.12,41.51 / 41.71,21.12 / 44.3,62.76 / 44.34,33.81 / 44.77,52.01 /
  45.46,38.78 / 46.84,24.87 / 48.85,55.05 / 62.27,62.6). ONE loop step
  over all 15 fixed points, said plainly as generic chests. No
  contract quest takes the chest as an object.
- Generic "Dented Footlocker", objects 179494 (12 fixed pts:
  35.91,45.23 / 36.9,39.89 / 38,45.86 / 38.43,50.83 / 39.07,24.43 /
  40.4,38.18 / 40.61,52.84 / 40.73,31.17 / 42.28,29.48 / 42.3,54.08 /
  42.36,44.09 / 44.58,54.15) and 179496 (5 fixed pts: 42.91,31.17 /
  43.93,30.88 / 45.75,28.33 / 46.85,43.84 / 46.89,25.69). ONE loop
  step over all 17 fixed points with both interacts, said plainly as
  generic footlockers (the Blasted Lands "no footlockers in the data"
  line is why these ship: here they exist). No quest references either
  object anywhere in the data.
- Excluded with reason: Altar of Suntara / Torch of Retribution / Hoard
  / Outhouse / Letter / Wanted board (core accept/turn-in objects);
  Sentry Braziers + Tower Fire/Smoke (3463 core objectives); Goodsteel
  Ledger object 173266 (core-chain prop at the outhouse, no
  independent significance); Secret Plans object 179826 (core 7722's
  placed source — excluded here AND logged as a core-guide correction:
  the core guide's "no placed source" claim is wrong, the object sits
  at 40.45,35.74 in the Slag Pit per its name and the objective text);
  Dark Iron Pillow 179828 (name mismatch with item 18950 — possible
  but unconfirmed source, logged, shipped nowhere); Twilight Artifact
  148506 (no quest link, no loot — decor despite the name); Dark Iron
  Remains 153157-153160 (corpse scenery, no quest, no loot); Charred
  Oak, Door Lever/Door, Ghost Gate, Scaffold Cars, Quarry Gate, anvils,
  forges, campfires/bonfires (set dressing); Dark Iron/Iron/Mithril/
  Truesilver deposits (gathering nodes); Mailbox 163313 (mail);
  KILL ON SIGHT boards 164867/164868 (Horde quest objects); Hallow's
  End + Winter Veil objects (seasonal).

## RECIPES — 9 shipped (all drops, no in-zone vendor)

- Tailoring, in-zone mob drops: 14471 Pattern: Cindercloth Vest + 14476
  Pattern: Cindercloth Gloves <- 5861 Twilight Fire Guard (sole
  dropper, SG-only, 10 pts); 254076 Pattern: Earthenweave Gloves <-
  5852 Inferno Elemental (sole dropper, SG-only, 6 pts); 254685
  Pattern: Stormcloth Shoulders <- 5856 Glassweb Spider (sole
  dropper, SG-only, 10 pts). No quest takes any of them.
- Alchemy, in-zone mob drop: 21547 Recipe: Elixir of Greater Firepower
  <- 5844 Dark Iron Slaver + 5846 Dark Iron Taskmaster + 8637 Dark
  Iron Watchman (3 droppers, all SG-only). No quest takes it.
- Blacksmithing, in-zone mob drop: 251439 Plans: Blessed Plate Boots
  <- 8566 Dark Iron Lookout (sole dropper, SG-only, 10 pts). No quest
  takes it.
- Leatherworking, in-zone mob drops: 252859 Pattern: Blue Suede Shoes
  <- 5846 Dark Iron Taskmaster (sole dropper, SG-only); 252915
  Pattern: Charged Scorpid Helm <- 9318 Incendosaur (sole dropper,
  SG-only, 10 pts). No quest takes them.
- Engineering, in-zone mob drop: 264214 Schematic: SAF-T Casing <-
  5839 Dark Iron Geologist (sole dropper, SG-only, 8 pts). No quest
  takes it.
- Excluded with reason: 11615 Plans: Dark Iron Shoulders (14 droppers,
  mostly spawnless BRD-trash — a Dark Iron instance-table world drop,
  not SG content, 5773 precedent); the 228xxx endgame series (228250,
  228313, 228314, 228315, 228316, 228317, 228318, 228993 — 19-27
  droppers each across 2-5 zones, and every table names world bosses:
  Azuregos, Onyxia, Nefarian, Kazzak, the Nightmare dragons — the
  Blasted Lands Kazzak-table precedent: endgame world drops despite
  in-zone droppers Skarresh/Gazzran/Galenges, who are themselves
  level 58-62); 15742 Warbear Harness (72 droppers/20 zones, vendor
  elsewhere); 8384 Comfortable Leather Hat (29/15); 8385 + 217271
  Turtle Scale Gloves (world drops, vendors elsewhere); 249512
  Formula: Dreambough Wand (sole dropper 2720 Dustbelcher Ogre Mage:
  10 Badlands pts + 4 Burning Steppes + 1 SG point — a Badlands-family
  mob, incidental SG presence, not SG content); everything else
  (multi-hundred droppers across ~30 zones, Elwynn rule).
- Quest-reward recipes: quest records carry no reward data — none
  shipped, class-logged in companion-unverified.
- Trainer-taught staples excluded (Polestar's own profession guides).

Professions with NO Searing Gorge source (stated plainly in the guide,
Dun Morogh Blacksmithing precedent): Cooking, Enchanting, First Aid,
Fishing. (No recipe is sold by any in-zone vendor — every shipped
recipe is a mob drop.)
