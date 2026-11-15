# Felwood companions inventory (game data, zone key 1448)

Source: local Forever game data (questie-forever NPC/object/item dumps,
built with `--product wowf` + QuestieDB). Rank flag is the `rank` field
(rank 4 = Rare, established on the Blasted Lands round); `roles`
confirms `["rare"]` on all seven shipped. Tameability has NO data flag
anywhere in the pack — no tame line ships without drop evidence plus
core-guide corroboration (core `felwood.guide` carries no tame lines),
so all beast-looking rares are logged to `docs/companion-unverified.md`,
never tamed in the guides.

## Rares — 7 found, 7 shipped

| NPC | Lvl | Points (1448) | Loot of note | Disposition |
|-----|-----|---------------|--------------|-------------|
| 7017 Lord Sinslayer | 16 | 1: 40.5,9.5 | 14146 Gloves of Spell Mastery + 284177 Sinslayer's Smasher, SOLE droppers anywhere | SHIP below-band (one-shottable at band, noted); both sole signatures as optional collects |
| 14339 Death Howl | 49 | 4: 47.86,74.82 / 48.34,78.18 / 50.03,77.11 / 56.16,89.26 | no soles; drops 11172 Silvery Claws (core 4084 objective) | SHIP loop, kill-note + core pointer |
| 14340 Alshirr Banebreath | 54 | 1: 40.25,85.21 | no soles, no core role | SHIP single-goto, kill-note |
| 14342 Ragepaw | 51 | 1: 47.74,93.06 | no soles; core 6032's objective id 14342 is the Mooncloth ITEM (same number, different table) — NPC has no core role | SHIP single-goto, kill-note |
| 14343 Olm the Wise | 52 | 1: 50.17,32.81 | no soles, no core role | SHIP single-goto, kill-note |
| 14344 Mongress | 50 | 4: 39.77,80.34 / 42.15,75.22 / 43.32,76.62 / 47.05,83.96 | no soles; drops 11172 Silvery Claws (core 4084 objective) | SHIP loop, kill-note + core pointer |
| 14345 The Ongar | 51 | 1: 42.22,49.9 | no soles, no core role | SHIP single-goto, kill-note |

Excluded: 7104 Dessecus L56 and 7137 Immolatus L56 are rank 2
(elites), not rank-flagged rares — quest-target lookalikes stay out per
the Dun Morogh precedent (no core-contracted quest names any shipped
rare as giver, ender, or kill objective; 11172 is an ITEM objective off
regular mobs, so the claw-dropping rares stay companion content with a
core pointer). Respawn timers: none in the data — every step says so.

## Treasures — 5 objects

| Object | Points (1448) | Shape |
|--------|---------------|-------|
| 178144 Troll Chest | 13: 38.8,97.2 / 39.1,97.4 / 39.3,95.3 / 39.5,97.5 / 39.6,96.5 / 39.6,98.7 / 39.9,97.1 / 40,97.9 / 40.1,95.9 / 40.4,98.5 / 40.6,99 / 40.8,100 / 41.2,98.4 | generic loop |
| 106319 Battered Chest | 3: 39.7,10.8 / 40.6,10 / 41.9,8.8 | generic loop |
| 2850 Solid Chest | 2: 39.6,96.1 / 41.4,99.1 | generic loop |
| 19022 Worn Chest | 1: 53.6,99.7 | single-goto (loop needs 2+) |
| 176225 Arko'niran's Chest | 1: 37.84,52.75 | unique: sits in Shadow Hold by Arko'narin (core 5202/5203 ground); own step, interact + honest note, no invented loot |

## Recipes — 9 shipped (all drops, 1 also vendor)

No vendor in Felwood sells any recipe (zero NPCs with 1448 spawns
carry vendor stock). Every shipped recipe is a mob drop whose PLACED
droppers are all 1448-only. Two sold elsewhere do not exist; 15754 is
also bought from Meilosh (11557, Timbermaw, neutral, Felwood spawn
65.69,2.81) — buy step plus drop step.

| Item | Profession | Source (all placed droppers 1448) |
|------|------------|-----------------------------------|
| 15752 Pattern: Living Leggings | Leatherworking | sole 7158 Deadwood Shaman (north village) |
| 15754 Pattern: Warbear Woolies | Leatherworking | 7156/7158 Deadwood furbolgs + buy Meilosh (11557); table also names 11663/13021 with NO spawns — disclosed in the step note |
| 249514 Formula: Enchant Bracer - Greater Agility | Enchanting | sole 7154 Deadwood Gardener (south village) |
| 251440 Plans: Blessed Plate Gauntlet | Blacksmithing | sole 7155 Deadwood Pathfinder (north village) |
| 252865 Pattern: Tooled Leather Boots | Leatherworking | sole 7158 Deadwood Shaman |
| 252866 Pattern: Blue Suede Gloves | Leatherworking | sole 7153 Deadwood Warrior (south village) |
| 252879 Pattern: Wicked Leather Boots | Leatherworking | sole 9878 Entropic Beast (Shatter Scar Vale) |
| 254126 Pattern: Earthenweave Leggings | Tailoring | sole 7139 Irontree Stomper (Irontree Vale) |
| 264228 Schematic: EZ-Thro Mana Bomb | Engineering | sole 9862 Jaedenar Legionnaire (Shadow Hold) |

Empty professions (stated, not padded): Alchemy, Cooking, First Aid,
Fishing (no vendor sells them in-zone and no in-zone mob drops them;
trainer staples excluded per the standing rule).

Excluded by the Elwynn rule (dozens-to-hundreds of droppers across
10–30 zones — generic world drops, not Felwood content): all 2406-line
lowbie patterns, the mithril/thorium/radiant plans series, voodoo and
mageweave patterns, transmute/flask/p Mongoose-line alchemy recipes and
every other recipe in the sweep with 80+ droppers. Narrow-but-shared
borderline calls (argued, OUT): 13491 Mongoose (2 droppers, Azshara +
Felwood — the Azshara leg has equal claim), 15739/15744/251442/252926
(single droppers dual-spawning 1439/1448 — shared with Darkshore's
ground), 11151/250977/250989 (5/2/2 droppers across 3–5 zones), 15754's
two spawn-less table entries (disclosed, not relied on). Quest-reward
recipes: quest records carry no reward data — none verifiable, none
shipped (standing rule).
