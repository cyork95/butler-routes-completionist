# Eastern Plaguelands companions inventory (pack butler-routes-completionist)

Source: local Forever game data (questie-forever npcs/objects/items/quests.json),
built with `--product wowf` + QuestieDB. Accept-zone key **1422**, core band
**50-60**, Alliance route. The core contract (76 quests) is untouched by this
inventory. Game data wins over community sources throughout.

## RARES - 11 rare-flagged NPCs on 1422, all 11 shipped

Rank semantics per the Badlands calibration: rank 4 = Rare, rank 2 = Rare Elite.
Every point below is the data's spawn point verbatim. Signature = the item's
sole dropper anywhere in the data (drops.npc lists only this NPC).

| NPC | lvl | points (map 1422) | signature (sole drop, rate) | disposition |
|-----|-----|-------------------|-----------------------------|-------------|
| 1847 Foulmane | 52 | 1: 46.27,52.43 | none (generic greens only) | SHIP single-goto, kill-only |
| 1848 Lord Maldazzar | 56 | 1: 54.16,80.43 | 284065 Crown of Maldazzar (rate null in data) | SHIP single-goto + collect |
| 1844 Foreman Marcrid | 58 | 1: 49.04,32.73 | 12836 Plans: Frostguard (100%) | SHIP single-goto + collect + recipes note |
| 1850 Putridius | 58 | 1: 48.05,67.39 | none (generic greens only) | SHIP single-goto, kill-only |
| 1885 Scarlet Smith | 59 | 1: 44.36,13.54 | 12719 Plans: Runic Plate Leggings (100%) | SHIP single-goto + collect + recipes note |
| 1837 Scarlet Judge | 60 | 1: 42.21,18.5 | none (generic greens only) | SHIP single-goto, kill-only |
| 1841 Scarlet Executioner | 60 | 1: 45.71,18.78 | none (generic greens only) | SHIP single-goto, kill-only |
| 1838 Scarlet Interrogator | 61 | 1: 45.15,15.27 | none (generic greens only) | SHIP single-goto + come-back-later note |
| 1843 Foreman Jerris | 62 | 1: 45.56,9.21 | none (generic greens only) | SHIP single-goto + come-back-later note |
| 1851 The Husk | 62 | 1: 62.15,36.31 | none (generic greens only) | SHIP single-goto + come-back-later note |
| 1839 Scarlet High Clerist | 63 | 3: 42.34,18.9 / 44.5,19.3 / 56.94,34.81 | none (generic greens only) | SHIP 3-pt loop + come-back-later note |

Notes applied in the guide:
- No core-contracted quest carries a kill objective on any of the 11 (checked all
  76 contract quests' objectives), so the Dun Morogh exclusion does not fire
  anywhere. No quest-target lookalikes carry the rare flag.
- The four above-band rares (61/62/62/63, band tops at 60) ship with honest
  come-back-later notes per the Westfall/Hillsbrad precedent; none is far
  enough above band to exclude.
- All other drops in the data are generic green world loot shared across many
  mobs; the guide says so plainly with no goals for them.
- No tame lines: ten are humanoid/undead by name and structure (Scarlet
  humanoids, Maldazzar, Putridius, the Husk); Foulmane is the only
  possibly-tameable-shaped name, but the data carries no creature-type flag and
  neither drop evidence nor core-guide corroboration qualifies it, so the tame
  question for Foulmane goes to docs/companion-unverified.md, never guessed.

## TREASURES - fixed-spawn containers on 1422

| object | points | disposition |
|--------|--------|-------------|
| 153453 Solid Chest | 14 scattered (37.93,54.35 / 39.35,66.73 / 40.79,51.96 / 41.94,73.08 / 43.15,72.91 / 45.1,65.22 / 45.19,34.09 / 46.65,66.53 / 47.36,49.66 / 49.16,67.71 / 50.79,40.7 / 53.8,65.07 / 54.87,23.1 / 64.63,59.41) | SHIP one 14-pt loop, said plainly as generic fixed placements |
| 153471 Food Crate | 23 scattered (38.8,55.7 / 39.21,67.92 / 40.66,51.87 / 41.9,72.22 / 42.96,18.61 / 43.14,20.64 / 43.2,63.45 / 44.35,33.87 / 44.51,12.4 / 45.61,18.9 / 45.88,62.39 / 46.54,73.17 / 47.34,50.86 / 47.76,22.79 / 47.95,69.38 / 48.31,32.81 / 51.18,40.43 / 51.84,28.2 / 51.91,44.13 / 52.05,65.4 / 53.11,36.62 / 62.71,60.29 / 65.93,47.71) | SHIP one 23-pt loop, said plainly |
| 153463 Large Solid Chest + 153468 Large Mithril Bound Chest | 3 shared (41.69,14.92 / 42.32,17.96 / 46.94,13.17), Hearthglen | SHIP one 3-pt loop naming both chest types |
| 3658 Water Barrel + 153472 Food Crate | 4 shared (20.3,49.2 / 26.8,55.2 / 26.8,59.5 / 26.9,56.7), Dalson farmsteads | SHIP one 4-pt loop naming both |
| 3662 Food Crate + 3705 Barrel of Milk | 2 shared (8,66.7 / 8.3,64.6), far west edge | SHIP one 2-pt loop naming both |
| 3706 Barrel of Sweet Nectar + 3707 Food Crate | 3 shared (32.3,92.1 / 32.7,93 / 32.8,93.7) | SHIP one 3-pt loop naming both |
| 2855 Solid Chest | 6 clustered (31.5,91.4 / 32.3,91.6 / 32.5,93.3 / 32.7,93.9 / 32.8,94.6 / 32.9,93.4), Uther's Tomb south | SHIP one 6-pt loop |
| 176092 Box of Incendiaries | 1: 26.5,56.2 | SHIP plain goto + note |
| 177490 Northridge Lumber Mill Crate | 1: 48.35,32 | SHIP plain goto + note |
| 178464 Dark Cleric Salem's Chest | 1: 30.6,28.9 | SHIP plain goto + note |
| 442742 Box of Scarlet Dye | 1: 45.2,15.2 | SHIP plain goto + note |
| 461632 Marked Crate | 1: 45.8,18.4 | SHIP plain goto + note |
| 461633 Belavus' Safe Box | 1: 46.5,14.1 | SHIP plain goto + note |
| 463540 Scarlet Toolbox | 1: 45,14.1 | SHIP plain goto + note |

Excluded with reasons:
- 175802 Small Lockbox (20 Andorhal points): the 100% source of the Andorhal
  Watch for core-contracted 4972/4973 - core content, not companion content
  (Dun Morogh precedent applied to containers).
- 177491 Termite Barrel: the turn-in object of core-contracted 5904 - core content.
- Mining veins, herb nodes: gathering content, not treasure; Polestar's own
  profession guides cover gathering.
- Landmark/lore objects with no loot (Uther's Tomb Statue, Uther the
  Lightbringer, Andorhal/Warning signs): not containers.
- Campfires, warm/blazing fires: flavor objects, no loot.
- Respawn timers: no timer data anywhere in the local data; the guide states
  the timers are unconfirmed.

## RECIPES - 21 shipped (19 vendor, 2 drop)

Vendor stock (stock class limited vs unlimited is not in the local data; the
guide carries the pack's standard stock note):

| item | profession | vendor (faction, place) | disposition |
|------|-----------|------------------------|-------------|
| 8030 Plans: Ebon Shiv | Blacksmithing | 11278 Magnus Frostwake (AH, Light's Hope 68.12,77.57) | SHIP buy |
| 12703 Plans: Storm Gauntlets | Blacksmithing | Magnus Frostwake | SHIP buy |
| 12819 Plans: Ornate Thorium Handaxe | Blacksmithing | Magnus Frostwake | SHIP buy |
| 12823 Plans: Huge Thorium Battleaxe | Blacksmithing | Magnus Frostwake | SHIP buy |
| 228313 Plans: Tempest Gauntlets | Blacksmithing | Magnus Frostwake | SHIP buy |
| 13485 Recipe: Transmute Water to Air | Alchemy | Magnus Frostwake | SHIP buy |
| 13501 Recipe: Major Mana Potion | Alchemy | Magnus Frostwake | SHIP buy |
| 13482 Recipe: Transmute Air to Fire | Alchemy | 10856 Argent Quartermaster Hasana + 10857 Argent Quartermaster Lightspark (AH; 26.6,55.2 and 42.84,83.72) | SHIP buy (same stock both vendors) |
| 19203 Plans: Girdle of the Dawn | Blacksmithing | both Argent Quartermasters | SHIP buy |
| 19205 Plans: Gloves of the Dawn | Blacksmithing | both Argent Quartermasters | SHIP buy |
| 19216 Pattern: Argent Boots | Leatherworking | both Argent Quartermasters | SHIP buy |
| 19217 Pattern: Argent Shoulders | Leatherworking | both Argent Quartermasters | SHIP buy |
| 19328 Pattern: Dawn Treaders | Tailoring | both Argent Quartermasters | SHIP buy |
| 19329 Pattern: Golden Mantle of the Dawn | Tailoring | both Argent Quartermasters | SHIP buy |
| 19442 Recipe: Powerful Anti-Venom | First Aid | both Argent Quartermasters | SHIP buy |
| 19446 Formula: Enchant Bracer - Mana Regeneration | Enchanting | both Argent Quartermasters | SHIP buy |
| 19447 Formula: Enchant Bracer - Healing | Enchanting | both Argent Quartermasters | SHIP buy |
| 15725 Pattern: Wicked Leather Gauntlets | Leatherworking | 12942 Leonard Porter (A, Light's Hope 43.08,84.31) | SHIP buy |
| 15741 Pattern: Stormshroud Pants | Leatherworking | Leonard Porter | SHIP buy |
| 12836 Plans: Frostguard | Blacksmithing | dropped by 1844 Foreman Marcrid (sole dropper anywhere, 100%) | SHIP collect at 49.04,32.73 |
| 12719 Plans: Runic Plate Leggings | Blacksmithing | dropped by 1885 Scarlet Smith (sole dropper anywhere, 100%) | SHIP collect at 44.36,13.54 |

Excluded with reasons:
- 15725/15741 as sold by 12943 Werg Thickblade (Horde, 26.7,56.8): Horde-faction
  vendor excluded per the Alterac precedent; the same two patterns ship from the
  Alliance vendor Porter, so nothing is lost.
- Pattern: Frostweave Pants (520 droppers, 23 zone maps) and Pattern: Felcloth
  Shoulders (476 droppers, 19 zone maps): generic world drops per the Elwynn
  rule, not zone content.
- Quest-reward recipes: quest records carry no reward data, so none can be
  verified - never shipped (see docs/companion-unverified.md).
- Trainer-taught staples: excluded; Polestar's own profession guides cover them.
- Engineering schematics, Cooking recipes, Fishing lures: no in-zone source in
  the data - the guide says so in notes (Dun Morogh Blacksmithing precedent).
