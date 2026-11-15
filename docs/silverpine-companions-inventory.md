# Silverpine Forest companions inventory (pack butler-routes-completionist)

Zone key 1421. Sources: local Forever data build (`--product wowf` +
QuestieDB): npcs.json (rank flags, spawns), objects.json (treasure spawns),
items.json (vendor/drop tables). These companions are Horde guides,
matching the Silverpine core.

## Rares (rank-flagged NPCs with 1421 spawns)

8 candidates: 7 rank-4 (roles ["rare"]) + Varimathras rank-3.

SHIPPED (7):

- Dalaran Spellscribe (1920, lvl 21, Alliance faction, rare) - 1421
  @63.54,63.35 (single point; also spawns Hillsbrad 1424 - dual-spawn
  noted, only the Silverpine point routed). Loot: shared world greens
  (Dalaran Sharp, scrolls, chain armor) - no signature item. Above the
  core band (10-20) by 1: ships with a come-back-later note (genuine zone
  rare; Westfall/Hillsbrad precedent, argued per rare).
- Rot Hide Bruiser (1944, lvl 22, neutral, rare) - 1421 @64.67,23.05
  (single point). Loot: shared world greens. Above band by 2: ships with
  a come-back-later note.
- Snarlmane (1948, lvl 23, neutral, rare) - 1421 @65.1,25.1 (single
  point). Loot: shared world greens. Above band by 3: ships with a
  come-back-later note.
- Ravenclaw Regent (2283, lvl 22, neutral, rare) - 1421 @56.83,70.18
  (single point, Beren's Peril). Loot: shared world greens. Above band by
  2: ships with a come-back-later note. Not a core quest target (the core
  hunts Guardians/Drudgers, not the Regent).
- Gorefang (12431, lvl 13, neutral, rare) - 1421 @59.53,7.64 (single
  point, north shore). Signature loot: Recipe: Swiftness Potion (2555) -
  a 30-zone world drop, but Gorefang's table names it, so it rides as the
  rare's optional signature collect with a note (points at the recipes
  guide's vendor/drop handling - the recipes guide does NOT list it as
  zone content per the Elwynn rule).
- Old Vicejaw (12432, lvl 14, neutral, rare) - 1421 @53.85,51.93 (single
  point). Signature loot: Pattern: Fine Leather Boots (2406, 29-zone
  world drop) + Plans: Runed Copper Breastplate (2881, 29-zone world
  drop) - both ride as optional signature collects with notes.
- Krethis Shadowspinner (12433, lvl 15, neutral, rare) - 1421 @35.7,8.25
  (single point, west woods). Signature loot: Pattern: White Leather
  Jerkin (2407, 30-zone world drop) - optional signature collect.

All 7 hold single points: every rare step is a plain single-goto step,
no loops. All goals optional. No respawn timers in the data - every step
notes the timer unconfirmed. No tame lines: the NPC records carry no
family flag, so tameability is unassessable from data; no drop evidence
and no core-guide corroboration (the core has no tame lines) - logged in
docs/companion-unverified.md, never shipped as fact.

EXCLUDED (1):

- Varimathras (2425, lvl 62, Horde, rank 3, NO rare role) - 1421
  @74.2,13.5. The dreadlord is a core-contracted quest NPC (5725 chain),
  not a rare spawn; no loot of his own. Out per the Dun Morogh precedent
  (a rare whose only significance is a core-contracted quest is not
  companion content).

## Treasures (objects spawning in-zone)

- Battered Chest (106319) - 23 fixed points, west/central woods
  (43-66 x 7-75). Generic chest: ONE loop step over all 23 points.
- Battered Chest (2849) - 6 fixed points, east shore (64-80 x 23-45).
  A second Battered Chest object ID (distinct loot table): its own loop
  step over all 6 points, labeled east shore.
- Alliance Chest (111095) - 7 fixed points, Pyrewood arc (62-63 x
  56-76). Generic-shape (one object, many points): ONE loop step.
- Hidden Strongbox (2039) - 2 fixed points (70.6,57.6 / 71.1,56).
  Two points: loop step.
- Alliance Strongbox (105570) + Alliance Chest (105579) - SHARE one
  point (71.3,55.2). One step naming both objects at the point.
- Ambermill Strongbox (103815) - 1 fixed point (63.71,65.24). Own step.
- Rusty Chest (409131) - 1 fixed point (45.2,67.2). Own step.

No spawn inventing: every point above is a data point. Alliance-named
chests are lootable objects, shipped plainly (the faction rule governs
vendors, not chests).

## Recipes (physically in-zone sources)

VENDOR-SOLD (all vendors Horde faction - no Alliance-only exclusions;
no limited-stock flags in the data, so none marked):

- Andrew Hilbert @43.22,40.66 (Sepulcher): Pattern: Red Linen Bag (5771,
  Tailoring), Pattern: Murloc Scale Belt (5786, Leatherworking), Pattern:
  Murloc Scale Breastplate (5787, Leatherworking), Pattern: Blue Linen
  Robe (6272, Tailoring), Recipe: Smoked Bear Meat (6892, Cooking).
- Killian Sanatha @33,17.85 (west coast): Recipe: Longjaw Mud Snapper
  (6328, Cooking), Recipe: Rainbow Fin Albacore (6368, Cooking).
- Lilly @43.02,50.82 (Sepulcher): Formula: Enchant Chest - Minor Mana
  (6342), Formula: Enchant Chest - Lesser Mana (6346), Formula: Minor
  Mana Oil (20752), Formula: Lesser Wizard Oil (20753), Formula: Minor
  Wizard Oil (20758), Pattern: Enchanted Mageweave Pouch (22307,
  Tailoring) - all Enchanting except the pouch.
- Leo Sarn @53.89,82.21: Formula: Enchant Chest - Minor Mana (6342),
  Formula: Enchant 2H Weapon - Lesser Intellect (6349), the three oils
  (20752/20753/20758), Pattern: Enchanted Mageweave Pouch (22307).
  Same stock shape as Lilly's, separate step per source.
- Algernon @73.2,9.5 (far north-east): Recipe: Elixir of Shadow Power
  (9301, Alchemy), Recipe: Superior Mana Potion (13477, Alchemy).

DROPPED - shipped (1):

- Recipe: Lesser Frenzy Potion (250983, Alchemy): data-exclusive to
  Silverpine (1 zone) - Raging Rot Hide camp loop (9 points, 65-66 x
  23-25), optional collect. Ships per the Shafety Sheep precedent (sole
  dropper genuinely spawning in-zone). Come-back-later n/a (in-band
  mob).

DROPPED - out (Elwynn rule: generic world drops, dozens of zones;
argued per item):

- All 20-30-zone patterns/plans/schematics/formulas (2406/2407/2408/
  2409/2553/2555/2598/2881/...): world-drop tables, not zone content.
  The three with rare signatures (2555 Gorefang, 2406+2881 Vicejaw,
  2407 Krethis) ride the rares guide as signature collects instead.
- Near-misses, out: Recipe: Cooked Crab Claw (2698, 9 zones, common
  Reef Frenzy mob), Formula: Enchant Bracer - Minor Intellect (249474,
  2 zones but a common-mob world pattern - the exclusivity line is drawn
  at data-exclusive), Formula: Scroll of Spatial Mending (223163,
  9 zones), Pattern: Comfortable Leather Hat (8384, 15 zones).

Quest-reward recipes: UNVERIFIABLE (quest records carry no reward data;
the census found no profession quests) - none shipped, nothing to log.

Professions with NO in-zone source (stated, not padded): Blacksmithing,
Engineering, First Aid, Fishing (the Sanatha fish recipes are Cooking),
plus gathering. Covered: Tailoring, Leatherworking, Cooking,
Enchanting, Alchemy.
