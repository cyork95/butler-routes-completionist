# Un'Goro Crater companions inventory (pack butler-routes-completionist)

Verified against the local Forever game data (`--product wowf` + QuestieDB:
npcs.json, objects.json, items.json, quests.json). Accept-zone key 1449.
Core contract is 42 quests, band 47-54 (docs/ungoro-census.md); the core
guide owns every core-contracted quest object and objective - nothing below
duplicates it.

## Rares (rank-flagged, spawn in 1449)

Five NPCs carry `roles: ["rare"]` with 1449 spawns, but the pack's "flagged
rare" means the RANK flag (rank 4), per the Felwood precedent as applied in
Azshara (Monnos/Scalebeard carry roles ["rare"] but rank 2 and stay out as
elites). Three are rank 4 and ship, each as a single-point plain step (no
rare has 2+ points, so no loop steps). None is a core-contracted quest
objective (grep of ungoro.guide for 6581/6582/6585: no hits), so the Dun
Morogh exclusion does not fire.

- Ravasaur Matriarch (6581), level 50, @62.35,65.95. 9 drops, all shared
  world loot (Mangled Journal, Un'Goro Soil, raptor bits, Wicked Claw):
  no signature loot - kill-note, ordinary shared drops only.
- Clutchmother Zavas (6582), level 54, @48.73,85.35. 4 drops, all shared
  (journal, soil, insect bits): kill-note.
- Uhk'loc (6585), level 53, @68.48,12.66. 14 drops, all shared (gems, Thorium
  Ore, generic world-drop recipes with 500+ sources each): kill-note.

Tame lines: NONE. No data flag exists; none of the three drops taming
evidence, and the core guide corroborates no taming (it kills these
families, which is not taming corroboration). Logged in
docs/companion-unverified.md, never shipped as fact.

### Rare exclusions

- Gruff (6583, level 57, @38.05,75.50) and King Mosh (6584, level 60,
  @35.30,35.99): both carry roles ["rare"] but rank 2, not rank 4 -
  excluded as rank-2 elites per the Felwood/Azshara rank rule (same call
  as Monnos/Scalebeard). Both are also above the band top
  (Westfall/Hillsbrad). Mosh's sole-source Devilcore patterns (228119,
  228120) still ship in the RECIPES guide - that guide keys on drop
  sources, not mob rank, so the patterns are unaffected by this call.
- Blazerunner (9376, rank 1, @49.41,49.33): core-contracted quest target
  (core 3962) and not rank-flagged - Dun Morogh precedent, out.
- Lar'korwi (9684, unflagged, @79.65,49.83) and Lar'korwi Mate (9683,
  unflagged, 12 pts): named but not rank/role-flagged, no loot of their own
  beyond shared raptor drops - out (Azshara unflagged-mob precedent).
- Gorishi Hive Guard (10040) / Hive Queen (10041, both unflagged, 1 pt
  each): named but not rank/role-flagged - out, same precedent.

## Treasures

VERDICT: none confirmed - the rares guide ships rares-only. The data holds
no chest-named object in 1449 besides 164910 Ornate Chest (core-owned:
core 3962's objective). Considered and excluded:

- Un'Goro Dirt Pile (157936, 24 fixed points), Dinosaur Bone (161527,
  18 pts), Blue/Green/Red/Yellow Power Crystal formations (164658-81,
  8 x 24 pts), Fresh/Preserved Threshadon Carcass (166863/169216, 1 pt
  each), Shallow Grave (489943, 1 pt): fixed objects with no lootability
  flag anywhere in the data - unconfirmable as treasure, never invented.
- Mining veins, herb nodes, Fire Elemental Rifts, Whipweed: resource nodes,
  not treasure content.
- Raft, pack, pylons, JD crystals, Ornate Chest, Damaged Blue Crystal,
  hot spot, poster, J.D.'s Manual, Muigin's Sprout, Bloodpetal Sprout,
  Hive Hatchery, Flat Rock: core-contracted quest objects - the core
  guide owns them.
- Midsummer / Winter Veil props (bonfires, pavilions, flames): seasonal
  event furniture, not treasure.

## Recipes (source PHYSICALLY in 1449)

Ten ship: Leatherworking 9, Cooking 1. Vendor faction field "AH" reads as
both-faction (Nergal and Zannok both serve the core Alliance route), so no
Horde-only exclusion fires. No limited-stock flag exists in the data, so no
stock is marked limited (unconfirmed class).

Vendor-sold (buy goals):

- 15724 Pattern: Heavy Scorpid Bracers (Leatherworking) - Zannok
  Hidepiercer (12956), @23.00,16.40, south-west crater.
- 15762 Pattern: Heavy Scorpid Helm (Leatherworking) - Zannok Hidepiercer,
  same point.
- 15758 Pattern: Devilsaur Gauntlets (Leatherworking) - Nergal (12959),
  @43.27,7.73, Marshal's Refuge.

Mob-dropped (optional collect goals at data-placed droppers):

- 15772 Pattern: Devilsaur Leggings (Leatherworking) - oozes, ALL four
  sources in-zone: Muculent Ooze @57.19,38.36, Primal Ooze @38.52,17.34,
  Glutinous Ooze @25.62,45.47, Cloned Ooze @45.44,66.04.
- 228119 Pattern: Devilcore Gauntlets (Leatherworking) - SOLE source King
  Mosh @35.30,35.99 (see rares pointer above).
- 228120 Pattern: Devilcore Leggings (Leatherworking) - SOLE source King
  Mosh @35.30,35.99.
- 250181 Recipe: Raging Raptor Ribs (Cooking) - SOLE source Venomhide
  Ravasaur @62.43,50.52, east crater.
- 252882 Pattern: Tooled Leather Crown (Leatherworking) - SOLE source
  Scorching Elemental @45.71,51.58, central crater.
- 252914 Pattern: Supple Scorpid Leggings (Leatherworking) - SOLE source
  Ravasaur @57.36,77.14, east crater.
- 252927 Pattern: Charged Scorpid Bracers (Leatherworking) - SOLE source
  Tar Creeper @47.20,31.91, central crater.

### Recipe exclusions

- ~200 recipes with in-zone mob droppers but dozens to 600+ total sources
  (Thorium/Mithril plans, Frostweave/Brightcloth/Runecloth patterns,
  transmutes, protection potions, schematics): generic world drops under
  the Elwynn rule - not zone content. Spot checks: 3875 Golden Scale
  Boots (31 sources, 1 in-zone), 11168 Lesser Block (42, 1 in-zone),
  217260 Big Voodoo Mask (56, 1 in-zone), 3395 Limited Invulnerability
  (521), 13490 Greater Stoneshield (534), all four Uhk'loc patterns and
  the formula (500-646 each).
- Trainer-taught staples: out of scope (Polestar's profession guides own
  progression).
- Quest-reward recipes: UNVERIFIABLE (quest records carry no reward data)
  - logged in docs/companion-unverified.md, never shipped.
- Professions with NO Un'Goro source in the data: Alchemy, Blacksmithing,
  Tailoring, Enchanting, Engineering, First Aid, Fishing - the recipes
  guide says so plainly (Dun Morogh Blacksmithing precedent).
