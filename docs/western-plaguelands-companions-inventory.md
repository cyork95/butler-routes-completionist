# Western Plaguelands companions inventory (pack butler-routes-completionist)

Source: local Forever game data (questie-forever npcs/objects/items/quests.json),
built with `--product wowf` + QuestieDB. Accept-zone key **1423**, core band
**50-58**, Alliance route. The core contract (65 quests) is untouched by this
inventory. Game data wins over community sources throughout.

## RARES - 10 rare-flagged NPCs on 1423, all 10 shipped

Rank semantics per the Badlands calibration: rank 4 = Rare, rank 2 = Rare Elite.
Every point below is the data's spawn point verbatim. Signature = the item's
sole dropper anywhere in the data (drops.npc lists only this NPC).

| NPC | lvl | points (map 1423) | signature (sole drop, rate) | disposition |
|-----|-----|-------------------|-----------------------------|-------------|
| 10819 Baron Bloodbane | 45 | 1: 39.4,27 | 2043 Ring of Forlorn Spirits (20%) + 16999 Royal Seal of Alexis (60%) | SHIP single-goto + 2 collects + gray note |
| 10817 Duggan Wildhammer | 55 A | 7: 9.72,61.39 / 12.67,51.75 / 18.2,68.53 / 23.6,65.02 / 31.22,52.4 / 32.52,52.85 / 33.7,59.69 | none (generic greens only) | SHIP 7-pt loop, kill-only |
| 10825 Gish the Unmoving | 56 | 1: 65.23,43.94 | none | SHIP single-goto, kill-only |
| 10827 Deathspeaker Selendre | 56 | 1: 75.42,36.98 | none | SHIP single-goto, kill-only |
| 10821 Hed'mush the Rotting | 57 | 4: 34.02,64.1 / 48.16,18.65 / 58.13,40.72 / 59.49,42.2 | none | SHIP 4-pt loop, kill-only |
| 10826 Lord Darkscythe | 57 | 1: 21.95,25.76 | 16039 Ta'Kierthan Songblade (50%) | SHIP single-goto + collect + core-quest note |
| 10822 Warlord Thresh'jin | 58 | 1: 63.33,8.81 | none | SHIP single-goto, kill-only |
| 10823 Zul'Brin Warpbranch | 59 | 1: 63.31,11.45 | none | SHIP single-goto + CBL note |
| 10828 High General Abbendis | 59 Rare Elite | 1: 77.99,74.12 | none | SHIP single-goto + CBL note |
| 10824 Ranger Lord Hawkspear | 60 A | 1: 45.28,12.86 | none | SHIP single-goto + CBL note |

Notes applied in the guide:
- Lord Darkscythe is also the objective of core-contracted 9126
  (Bonescythe Digs - census: "Dark Caster ... + Darkscythe 21.95,25.76",
  core guide routes the same point). The Dun Morogh exclusion does NOT fire:
  the Songblade is exclusive loot with no quest use in the data, giving the
  rare significance beyond the quest. The step carries a note pointing at the
  core guide for the quest kill and never accepts.
- Baron Bloodbane (45) is 5 levels below the band: shipped with an honest
  gray-at-band note. Both signature drops are sole-source in the data, which
  is the shipping argument - a band player one-shots him on the way past.
- Zul'Brin (59), Abbendis (59) and Hawkspear (60) sit 1-2 above the band top:
  shipped with honest come-back-later notes (Westfall/Hillsbrad precedent).
  Nothing is far-above-band, so nothing is excluded on level.
- Duggan Wildhammer and Ranger Lord Hawkspear are faction=A
  (Alliance-aligned). They ship like any other rare: the data flags them rare
  with spawn points, and the guide takes no position on whether to attack
  beyond stating the alignment (Jalinde precedent).
- No other rare here is a giver, ender or objective of any core-contracted
  quest (checked quest objectives + core guide/census text), so the Dun Morogh
  exclusion fires nowhere else.
- TAME: no tame lines ship. The data has no tameability flag, and none of
  the 10 presents beast-drop evidence (their tables are generic greens plus
  the three signature weapons/ring/seal) with a core-guide beast-family kill
  to corroborate. Logged in docs/companion-unverified.md.
- Respawn timers are unconfirmed in the data - none stated.
- The three signature drops (Ring of Forlorn Spirits, Royal Seal of Alexis,
  Ta'Kierthan Songblade) are used by NO quest in the data (full objectives
  scan) - pure loot, noted as such, never as quest starters.

No rare-lookalike exclusions: nothing else on 1423 carries the rare flag,
and no world-boss-rank NPC spawns here.

## TREASURES

Generic fixed containers (THREE loop steps, said plainly - 35 fixed points):
- 153453 Solid Chest: 8 pts (22.64,23.18 / 22.73,72.88 / 32.68,79.31 /
  34.0,64.42 / 34.22,26.59 / 51.56,56.62 / 51.59,60.25 / 53.33,58.06).
  No contents listed in the data; shipped as interact-only loop.
- 153454 Solid Chest: 17 pts (33.67,40.01 / 33.78,44.5 / 35.99,41.33 /
  55.41,17.46 / 59.27,39.45 / 61.13,24.0 / 61.89,8.11 / 63.33,23.37 /
  63.78,12.48 / 68.66,64.96 / 71.11,72.98 / 73.15,31.23 / 73.31,67.62 /
  73.44,72.66 / 73.49,74.41 / 75.69,38.03 / 76.59,31.77).
  No contents listed in the data; shipped as interact-only loop.
- 179498 Scarlet Footlocker: 10 pts (68.07,68.37 / 68.48,64.91 /
  69.43,69.14 / 70.86,72.25 / 72.14,68.21 / 72.93,71.43 / 74.14,69.23 /
  74.55,67.97 / 76.72,69.44 / 77.38,74.41). No contents listed in the data;
  shipped as interact-only loop (Food Crate precedent).

Excluded quest-owned (verified against core guide/census):
- Pamela's Doll's Head/Trap/Left Side/Right Side + Pamela's Doll
  (176116/176117/176142/176143/176247): objects of the 5149 doll chain,
  core-contracted - core-owned, not companion content.
- Horgus' Skull + Shattered Sword of Marduk (176208/176209): objectives of
  core-contracted 5181 Villains of Darrowshire (census gives the same two
  points 44.34,41.18 + 46.86,55.43) - core-owned.
- Joseph's Chest (177544): end-object of core-contracted accept-only 5942
  (the chest IS the turn-in) - core-owned.
- Augustus' Receipt Book (177789): ground objective of core-contracted 6164
  (core guide completes at the same point 14.04,24.22) - core-owned.

Gathering/profession nodes, furniture, decor, seasonal and dungeon utility
are not treasures (excluded by class, no per-item logging): all veins/
deposits (324/1734/1735/2040/2047/175404), all herbs (1623/1628/142141/
142142/176583/176584/176586/176587/176589), campfires/
bonfires/cauldrons/braziers/forges/anvils/mailbox/benches/chairs/stools/
tables/rugs/MFF decor, road signposts (175654-175657, 176967-179986 tower/
town markers), Midsummer/seasonal objects (181288+), Meeting Stone 178831.

Logged to docs/companion-unverified.md (present on 1423, no shippable
loot-or-quest evidence): Blood of Heroes (176213/176214, 24+24 pts - no
contents, no quest refs), Third/Fourth Mosh'aru Tablet (175487/175488 -
out-of-contract chain objects by name), Quel'Thalas Registry (177747),
Aurora's Book/Aura (178229/178230), Symbol of Lost Honor (177264),
Tirion Fordring's Grave + Loose Dirt Mound (177239/177240), Darrowshire
Town Square spell focus DND (177528), Rancid Meat/Big Rancid Meat/Torn
Scroll/Mound of Dirt (177664/177665/177667/177675), Mangled Human Remains
x3 (177804/177805/177806), Shallow Grave (177677), Mark of Detonation
(177668), Tower Banner (182106), Lordaeron Shrines (181682/181955), Basin
of Holy Water (182063), The Argent Hold (176317), Horgus' Skull Trap
(176591), Sword of Marduk Trap (176865).

## RECIPES - 16 shipped (0 vendor buys + 16 drop collects)

No recipe vendor spawns in the Western Plaguelands: the vendor scan over all
items found zero in-zone vendors (every recipe's vendors list is empty for
key 1423). All 16 ship as drop collects off narrow in-zone droppers.

| item | profession | dropper (lvl, points on 1423) |
|------|-----------|-------------------------------|
| 13479 Recipe: Elixir of the Sages | Alchemy | 9449 Scarlet Cleric (54) / 9450 Scarlet Curate (55) / 9451 Scarlet Archmage (55) / 9452 Scarlet Enchanter (53) / 15162 Scarlet Inquisitor (61) - Tyr's Hand |
| 13499 Recipe: Greater Shadow Protection Potion | Alchemy | 8546 Dark Adept (59) / 8550 Shadowmage (59) - Andorhal |
| 17709 Recipe: Elixir of Frost Power | Alchemy | 8598 Frenzied Plaguehound (57) |
| 251444 Plans: Blessed Plate Belt | Blacksmithing | 8600 Plaguebat (53) |
| 250175 Recipe: Bat Hachee | Cooking | 8602 Monstrous Plaguebat (56) |
| 16222 Formula: Enchant Shield - Superior Spirit | Enchanting | 9447 Scarlet Warder (53) - Tyr's Hand |
| 16242 Formula: Enchant Chest - Major Mana | Enchanting | 9452 Scarlet Enchanter (53) - Tyr's Hand |
| 16252 Formula: Enchant Weapon - Crusader | Enchanting | 9451 Scarlet Archmage (55) - Tyr's Hand (second dropper 4494 spawns in 1422, unused) |
| 16056 Schematic: Flawless Arcanite Rifle | Engineering | 8561 Mossflayer Shadowhunter (58) |
| 252885 Pattern: Tooled Leather Bracers | Leatherworking | 8534 Putrid Gargoyle (54) |
| 252934 Pattern: Charged Scorpid Leggings | Leatherworking | 11291 Unliving Mossflayer (53) |
| 14477 Pattern: Ghostweave Gloves | Tailoring | 8538 Unseen Servant (55) (second dropper 7864 spawns in Azshara 1447, unused) |
| 14480 Pattern: Ghostweave Vest | Tailoring | 8538 Unseen Servant (55) |
| 14485 Pattern: Wizardweave Leggings | Tailoring | 8551 Dark Summoner (55) |
| 14500 Pattern: Wizardweave Robe | Tailoring | 8526 Dark Caster (56) |
| 14505 Pattern: Wizardweave Turban | Tailoring | 8526 Dark Caster (56) |

Notes:
- Dropper points are taken from the Scholomance/Andorhal/Tyr's Hand spawn
  sets in the data; the guide places each collect at the dropper's points.
- 13499's only droppers are both level 59, one above the band top: shipped
  with an honest come-back-later note. 15162 (61) is one of five droppers
  for 13479, the other four in-band, so no note needed there.
- Professions with NO in-zone source say so in the guide (Dun Morogh
  Blacksmithing precedent): First Aid, Fishing. (All seven recipe
  professions above have at least one source.)
- Quest-reward recipes are UNVERIFIABLE (no reward data in quest records):
  none shipped, none logged - the established class finding stands with no
  new candidates.
- Generic world drops (the hundreds of greens on half the zone's mobs, e.g.
  the 500-dropper recipes on Bloodbane's table) are not zone content (Elwynn
  rule): excluded by class, no per-item logging.
