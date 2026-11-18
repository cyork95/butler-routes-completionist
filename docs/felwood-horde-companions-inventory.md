# Felwood (Horde) companions inventory

Scope: accept-zone key **1448**, Horde core band **45–48**, faction **Horde**.
Built from the local data dumps (`upstream-polestar/data/forever/*.json`:
`npcs.json`, `objects.json`, `items.json`, `quests.json`) — game data wins
over the Alliance inventory (`docs/felwood-companions-inventory.md`)
wherever they differ; every delta is flagged inline AND logged in
`docs/companion-unverified.md`, never silently harmonized.

The Horde core contract is 8 quests (`docs/felwood-horde-census.md`):
4102/5887-5891 (Maybess salve chain), 8485 (Gorn peace-brokering),
86612 (Statue of Malorne object-start). No Horde-contracted quest is
item-started, so there is no writable in-zone item-start hunt — stated,
not padded.

## Rares — 7 rank-flagged on 1448, 7 shipped

Rare basis in this build: `rank` field (rank 4 = Rare, established on the
Blasted Lands round); `roles` confirms `["rare"]` on all seven shipped.
Tameability has NO data flag anywhere in the pack — no tame line ships
without drop evidence plus core-guide corroboration (core
`felwood-horde.guide` carries no tame lines), so all beast-looking rares
are logged to `docs/companion-unverified.md`, never tamed in the guides.

| NPC | Lvl | Points (1448) | Loot of note | Disposition |
|-----|-----|---------------|--------------|-------------|
| 7017 Lord Sinslayer | 16 | 1: 40.5,9.5 | 14146 Gloves of Spell Mastery + 284177 Sinslayer's Smasher, SOLE droppers anywhere | SHIP below-band (one-shottable at band, noted); both sole signatures as optional collects |
| 14339 Death Howl | 49 | 4: 47.86,74.82 / 48.34,78.18 / 50.03,77.11 / 56.16,89.26 | no soles; drops 11172 Silvery Claws (core 4084-equivalent family objective) + 11515 Corrupted Soul Shard (Horde-core 5887 objective, one of ~60 droppers) | SHIP loop, kill-note + core pointer, ABOVE-BAND come-back-later note (49 > 48) |
| 14340 Alshirr Banebreath | 54 | 1: 40.25,85.21 | no soles; drops 11515 (Horde-core 5887 objective) | SHIP single-goto, kill-note, ABOVE-BAND come-back-later note |
| 14342 Ragepaw | 51 | 1: 47.74,93.06 | no soles; the core-6032 objective 14342 is the Mooncloth ITEM (same number, different table) — NPC has no core role | SHIP single-goto, kill-note, ABOVE-BAND come-back-later note |
| 14343 Olm the Wise | 52 | 1: 50.17,32.81 | no soles; drops 11515 (Horde-core 5887 objective) | SHIP single-goto, kill-note, ABOVE-BAND come-back-later note |
| 14344 Mongress | 50 | 4: 39.77,80.34 / 42.15,75.22 / 43.32,76.62 / 47.05,83.96 | no soles; drops 11172 Silvery Claws | SHIP loop, kill-note + core pointer, ABOVE-BAND come-back-later note |
| 14345 The Ongar | 51 | 1: 42.22,49.9 | no soles; drops 11515 (Horde-core 5887 objective) | SHIP single-goto, kill-note, ABOVE-BAND come-back-later note |

No core overlap beyond item drops: no Horde-contracted quest names any
shipped rare as giver, ender, or kill objective (5887's objective is the
11515 ITEM off ~60 droppers including regular mobs — same shape as the
Alliance 4084 ruling: the rare itself stays companion content with a
core pointer). Faction: all seven are faction-null (hostile to both) —
engageable by Horde. DELTA vs Alliance (band 45–55, all seven plain):
the Horde band is 45–48, so six of the seven ship with come-back-later
notes; only Sinslayer keeps its one-shot note on both sides.

Excluded: 7104 Dessecus L56 and 7137 Immolatus L56 are rank 2
(elites), not rank-flagged rares — quest-target lookalikes stay out per
the Dun Morogh precedent. Dessecus is additionally a Horde-core item
feeder (drops 11503 for 4102 and 11515 for 5887) and Immolatus feeds
5887's 11515 — neither is a companion hunt (no core quest STARTS from
their drops). Both are above-band regardless. Respawn timers: none in
the data — every step says so.

## Item-start hunts

**None ship, and why:** the Horde census found no item-started
Horde-mask records at all (86612 is object-started; the rest start at
Maybess/Gorn NPCs). No rare drops an item starting a Horde-contracted
quest — the reverse-index over every item drop table confirms zero
start-item links. Stated in the rares guide so the absence is
deliberate, not an omission.

## Treasures — 5 objects, same set as Alliance

| Object | Points (1448) | Shape |
|--------|---------------|-------|
| 178144 Troll Chest | 13: 38.8,97.2 / 39.1,97.4 / 39.3,95.3 / 39.5,97.5 / 39.6,96.5 / 39.6,98.7 / 39.9,97.1 / 40,97.9 / 40.1,95.9 / 40.4,98.5 / 40.6,99 / 40.8,100 / 41.2,98.4 | generic loop |
| 106319 Battered Chest | 3: 39.7,10.8 / 40.6,10 / 41.9,8.8 | generic loop |
| 2850 Solid Chest | 2: 39.6,96.1 / 41.4,99.1 | generic loop |
| 19022 Worn Chest | 1: 53.6,99.7 | single-goto (loop needs 2+) |
| 176225 Arko'niran's Chest | 1: 37.84,52.75 | unique: sits in Shadow Hold by Arko'niran (core 5202/5203 ground); own step, interact + honest note, no invented loot |

All five verified unreferenced by any quest record in this build
(start/end/objective scan) — no quest furniture, no core overlap.

Excluded (all verified against this build's quest table):

- 661778 Statue of Malorne: start-object of Horde-core 86612 (and the
  Alliance twin 86611) — core furniture, not treasure.
- 142141 Arthas' Tears / 324 Small Thorium Vein: gathering nodes AND
  core 5889/5888 objective sources — nodes, not treasure.
- 176091 Deadwood Cauldron: end-object of 5084 / start-object of 5085
  (Falling to Corruption / Mystery Goo) — someone else's quest
  furniture.
- 463209 Book (Timbermaw Hold @65.2,3.3): start-object of 84397
  (out-of-zone quest) — someone else's quest furniture.
- 178147 Ruul Snowhoof Cage (@40.6,98.8, same point as Ruul Snowhoof
  12818): furniture of Horde 6482 Freedom to Ruul (zone 1440,
  contracted in ashenvale-horde) — another round's content, pointer
  noted, not duplicated. DELTA vs Alliance (silent): the link is named
  here, not harmonized.
- 179677 / 3000491 Kroshius' Remains (@45.7,34.76 / @45.3,35.3, on
  Kroshius 14467's own point): remains, not a lootable chest; no
  contents and no quest refs in the data — examined, not shippable.
  7603 (Kroshius' Infernal Core, contracted) starts at 14470, not here.
- 410220 / 464128 Gift of the Wisp (12/24 pts), 457092 The Fury of
  Stormrage (1 pt), 445042 Extraplanar Eye (1 pt): display/lore objects
  with no loot table and no quest refs — scenery, not treasure.
- Songflower family (cleansed/corrupted songflowers, night dragons,
  windblossoms, whipper roots, incl. 164881-164884 spot singles):
  buff/turn-in objects, not lootable treasure.
- Moonwells (177275/177276 + DND focus 148501), braziers, cages,
  candles, campfires/bonfires, gathering nodes (herbs/veins), fishing
  nodes, signposts, memorials and MFF display objects: scenery or
  profession nodes — never companion content.

## Recipes — shipped (9 drop + 15 vendor, Meilosh full stock settled)

Item records carry no profession field — professions assigned by the
pack's settled item-name convention (Recipe = Cooking, Pattern =
cloth/leather wear, Formula = Enchanting, Plans = Blacksmithing, Manual
= Alchemy/First Aid by name), stated per item below. Item records carry
no standing/reputation field either (verified: full-record dumps of all
23 Meilosh recipe items show `vendors` only) — see the Meilosh ruling.

Vendor-sold (in-zone Horde-usable vendors; every buy line pins the
vendor by NPC ID):

Meilosh (11557, Timbermaw Hold faction 576, neutral, Felwood spawn
1448 @65.69,2.81; Winterspring-frame spawn is a border-cave rendering,
correctly excluded by the Winterspring rounds as Felwood's). Full
recipe stock — 14 items, each vendors==[11557] (sole vendor anywhere),
all buyable by Horde (neutral vendor, no faction gate in the data):

| Item | Profession | Standing (per the data) |
|------|------------|-------------------------|
| 13484 Recipe: Transmute Earth to Water | Alchemy | none encoded — see ruling |
| 15742 Pattern: Warbear Harness | Leatherworking | none encoded (world drop across 20 zones — vendor is the Felwood source) |
| 15754 Pattern: Warbear Woolies | Leatherworking | none encoded (also drops 7156/7158; table names 11663/13021 with NO spawns anywhere — disclosed, not relied on) |
| 19202 Plans: Heavy Timbermaw Belt | Blacksmithing | none encoded |
| 19204 Plans: Heavy Timbermaw Boots | Blacksmithing | none encoded |
| 19215 Pattern: Wisdom of the Timbermaw | Leatherworking | none encoded |
| 19218 Pattern: Mantle of the Timbermaw | Tailoring | none encoded |
| 19326 Pattern: Might of the Timbermaw | Leatherworking | none encoded |
| 19327 Pattern: Timbermaw Brawlers | Leatherworking | none encoded |
| 19445 Formula: Enchant Weapon - Agility | Enchanting | none encoded |
| 20253 Pattern: Warbear Harness (same-name twin of 15742; drops from STV object 179697, out-of-zone — vendor is the Felwood source) | Leatherworking | none encoded |
| 20254 Pattern: Warbear Woolies (same-name twin of 15754; no drops anywhere — vendor-only) | Leatherworking | none encoded |
| 22392 Formula: Enchant 2H Weapon - Agility | Enchanting | none encoded |
| 228982 Formula: Enchant Shield - Law of Nature | Enchanting | none encoded |

NAMED CHECK (Meilosh ruling): the Alliance Felwood companion shipped
exactly one of these (15754). The other 13 mirror it exactly —
same sole vendor, same neutral faction, no gates in the data — so all
14 ship here; the gap is flagged as a DELTA in
`docs/companion-unverified.md`, not harmonized. Meilosh's remaining
stock is NOT recipes and does NOT ship: 227803/227804/227805/227807/
227808/227809/227810 (Dire/Dense Timbermaw gear), 227862 Incandescent
Mooncloth Boots, 228190 Knowledge of the Timbermaw (finished goods, no
recipe prefix), 233209 Firewater Cauldron + 233217 Tunneler's Incense
(non-recipe vendor goods, also on commendation officers 15734/15736),
plus threads/dyes/runes (generic trade goods). Standing: no Timbermaw
standing requirement is encoded anywhere in the toolchain dumps (item
records: vendors only; Timbermaw quests 6131/8460-8465: no reward/rep
fields) — every Meilosh buy line therefore carries the vendor pin plus
an honest note: check Timbermaw Hold standing in game, the data encodes
none. DELTA logged in `docs/companion-unverified.md`.

Bale (2806, Horde, Felwood spawn 1448 @34.75,53.23):

| Item | Profession |
|------|------------|
| 16110 Recipe: Monster Omelet | Cooking (also on Malygen 2803 Alliance + 11187 elsewhere — Horde buys from Bale) |

DELTA vs Alliance (logged, not harmonized): the Alliance inventory
claims "no vendor in Felwood sells any recipe", but Malygen (2803,
Alliance-faction, 1448 @62.32,25.64) sells this same recipe in-zone —
buyable by Alliance in this build. Either their build lacked the spawn
or the line was missed; Butler's call whether the Alliance guide gains
a Malygen step.

Narrow drops (dropper spawns all on 1448; sole droppers unless noted):

| Item | Profession | Dropper (1448 points) |
|------|------------|-----------------------|
| 15752 Pattern: Living Leggings | Leatherworking | sole 7158 Deadwood Shaman (north village, 15 pts) |
| 249514 Formula: Enchant Bracer - Greater Agility | Enchanting | sole 7154 Deadwood Gardener (south village, 10 pts) |
| 251440 Plans: Blessed Plate Gauntlet | Blacksmithing | sole 7155 Deadwood Pathfinder (south village, 5 pts) |
| 252865 Pattern: Tooled Leather Boots | Leatherworking | sole 7158 Deadwood Shaman |
| 252866 Pattern: Blue Suede Gloves | Leatherworking | sole 7153 Deadwood Warrior (south village, 17 pts) |
| 252879 Pattern: Wicked Leather Boots | Leatherworking | sole 9878 Entropic Beast (Shatter Scar Vale, 21 pts) |
| 254126 Pattern: Earthenweave Leggings | Tailoring | sole 7139 Irontree Stomper (Irontree Vale, 24 pts) |
| 264228 Schematic: EZ-Thro Mana Bomb | Engineering | sole 9862 Jaedenar Legionnaire (Shadow Hold, 8 pts) |

Empty professions (stated, not padded): First Aid, Fishing (no vendor
sells them in-zone and no in-zone mob drops them; trainer staples
excluded per the standing rule). Alchemy HAS an in-zone source (13484
via Meilosh); Blacksmithing HAS sources (3 narrow plans above);
Cooking HAS a source (16110 via Bale).

## Recipes — excluded (with reasons)

- Generic world drops by the Elwynn rule (dozens of droppers or zones,
  unlisted individually): all 2406-line lowbie patterns, the
  mithril/thorium/radiant plans series, voodoo and mageweave patterns,
  transmute/flask/P Mongoose-line alchemy recipes, and every other
  recipe in the sweep with 80+ droppers — including 15742's 20-zone drop
  leg (ships vendor-only via Meilosh, no drop step).
- Narrow-but-shared borderline calls (argued, OUT — verified in THIS
  build): 13491 Mongoose (droppers on 1439/1447/1448 — Felwood is a
  third leg, not the home), 15739/15744/251442/252926 (single droppers
  dual-spawning 1439/1448 — shared with Darkshore's ground, same call as
  Alliance), 11151 (1440/1442/1448), 250977 (1413/1439/1448), 250989
  (1413/1439/1445/1448).
- Alliance-vendor-only in-zone: none — no recipe is sold in Felwood
  ONLY by an Alliance-faction vendor (Mylini 15315 sells weapons, not
  recipes; Malygen's one recipe is also on Bale). Genuine Horde gap:
  none at vendor level. Stated, not padded.
- Quest-reward recipes: quest records carry no reward data — none
  verifiable, none shipped (standing rule).
- Trainer-taught staples: out of scope per the pack rule.
