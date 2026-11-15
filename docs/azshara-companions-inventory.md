# Azshara companions inventory (game data, zone key 1447)

Source: local Forever game data (questie-forever NPC/object/item dumps,
built with `--product wowf` + QuestieDB). Rank flag is the `rank` field
(rank 4 = Rare, established on the Blasted Lands round); `roles`
confirms `["rare"]` on all eight shipped. Tameability has NO data flag
anywhere - no tame line ships without drop evidence plus core-guide
corroboration (core `azshara.guide` carries zero only-Hunter lines and
no references to any flagged rare), so all eight steps are
kill-or-collect. Anything unverifiable is logged in
`docs/companion-unverified.md`, never in a guide as fact.

## Rares - 10 flagged, 8 shipped

| NPC | Lvl | Points (1447) | Loot of note | Disposition |
|-----|-----|---------------|--------------|-------------|
| 6118 Varo'then's Ghost | 48 | 1: 13.23,74.2 | none sole; drops 7972 Ichor of Undeath (core 8256 objective, 1 of ~120 world droppers) | SHIP single-goto, kill-note + core pointer (Felwood claw-precedent) |
| 6647 Magister Hawkhelm | 52 | 1: 58.46,30.89 | none sole (9295 Invisibility Potion is a 560-dropper world drop) | SHIP single-goto, kill-note |
| 6648 Antilos | 50 | 1: 16.6,54.1 | none sole | SHIP single-goto, kill-note |
| 6649 Lady Sesspira | 51 | 1: 35.39,55.69 | none sole (rank-4 one is the rare; 239942 same-name regular is the quest-target lookalike, stays out per Dun Morogh) | SHIP single-goto, kill-note |
| 6650 General Fangferror | 51 | 1: 41.31,53.96 | SOLE 17054 Joonho's Mercy (starts nothing, objective of nothing) | SHIP single-goto, kill + optional signature collect |
| 6651 Gatekeeper Rageroar | 50 | 1: 38.27,32.08 | none sole | SHIP single-goto, kill-note |
| 6652 Master Feardred | 52 | 3: 61.35,24.92 / 61.55,24.25 / 66.3,16.72 | none sole | SHIP loop over all 3 |
| 8660 The Evalcharr | 48 | 1: 17.87,65.6 | none sole | SHIP single-goto, kill-note |

Excluded: 6646 Monnos the Elder L54 and 13896 Scalebeard L52 are rank 2
(elites), not rank-4 rares - quest-target lookalikes stay out per the
Dun Morogh precedent, despite both carrying roles ["rare"] (anomaly
logged for review). Unflagged but named (no rank flag, logged for
review, none shipped): 14462 Thundering Invader L55, 14464 Avalanchion
(rank 1) L58, 244188 Scalebeard L55, 235906 Elder Bramblesnap L55,
235909 Furze L50, 236770 Korsa L50. Above-band and unflagged (world-boss
tier): 6109 Azuregos L63, 15481 Spirit of Azuregos L63, 15571 Maws L63.
No core-contracted quest names any shipped rare as giver, ender, or
kill objective. Respawn timers: none in the data - every step says so.

## Treasures - 3 generic objects, 46 points

| Object | Points (1447) | Shape |
|--------|---------------|-------|
| 153451 Solid Chest | 13 | generic loop |
| 153453 Solid Chest | 12 | generic loop (second same-name object, own step) |
| 179497 Mossy Footlocker | 21 | generic loop |

Mining/herb nodes are gathering, not treasure. Fishing pools/schools
are not fixed treasure. Quest and flavor objects stay out: Azsharite
formations, Kim'jael's Equipment, Saria's Knapsack, Hydraxis' Coffer
(all core content), the Ravencrest tablets/runes, tide pools, campfire
and furniture objects (no loot). Never inventoried a spawn point: every
point above is a data point.

## Recipes - 21 shipped (17 drops + 4 vendor)

Vendors (both neutral AH, 1447-only spawns): 8678 Jubie Gadgetspring
(45.28,90.95) sells 10607 Schematic: Deepdive Helmet (vendor-exclusive,
zero droppers). 12957 Blimo Gadgetspring (45.21,90.85) sells 15729
Pattern: Chimeric Gloves, 15751 Pattern: Blue Dragonscale Breastplate,
227898 Pattern: Honed Blue Dragonscale Breastplate (all vendor-exclusive,
zero droppers). Stock class (limited vs unlimited) is not in the data;
no line is marked limited.

Every shipped drop is a SOLE in-zone dropper with zero object drops:

| Item | Profession | Sole dropper (all spawns 1447) |
|------|------------|--------------------------------|
| 14473 Pattern: Ghostweave Belt | Tailoring | 7864 Lingering Highborne |
| 254074 Pattern: Ghostweave Cord | Tailoring | 6126 Haldarr Trickster |
| 15728 Pattern: Wicked Leather Bracers | Leatherworking | 6201 Legashi Rogue |
| 15753 Pattern: Stormshroud Armor | Leatherworking | 6138 Arkkoran Oracle |
| 15763 Pattern: Blue Dragonscale Shoulders | Leatherworking | 6146 Cliff Breaker |
| 15764 Pattern: Stormshroud Shoulders | Leatherworking | 6144 Son of Arkkoroc |
| 227899 Pattern: Honed Blue Dragonscale Shoulders | Leatherworking | 6146 Cliff Breaker |
| 252886 Pattern: Blue Suede Belt | Leatherworking | 7885 Spitelash Battlemaster |
| 252929 Pattern: Supple Scorpid Belt | Leatherworking | 6198 Blood Elf Surveyor |
| 252932 Pattern: Charged Scorpid Vest | Leatherworking | 6195 Spitelash Siren |
| 16219 Formula: Enchant Gloves - Greater Agility | Enchanting | 6201 Legashi Rogue |
| 249516 Formula: Enchant Gloves - Advanced Skinning | Enchanting | 6196 Spitelash Myrmidon |
| 250189 Recipe: Clam Linguine | Cooking | 7886 Spitelash Enchantress |
| 235645 Legashi Firewater Recipe | unknown (no skill tag in data, ungated with disclosure) | 6200/6201/6202/236867/236874/236876 Legashi (all 1447) + 244129 phantom record with no spawns (disclosed) |
| 250980 Recipe: Superior Spellblasting Potion | Alchemy | 6193 Spitelash Screamer |
| 251441 Plans: Imperial Plate Gauntlets | Blacksmithing | 6199 Blood Elf Reclaimer | (sole Blacksmithing source in-zone)
| 16045 Schematic: Spellpower Goggles Xtreme Plus | Engineering | 6195 Spitelash Siren |

First Aid and Fishing have NO Azshara source - stated in the guide, not
padded. Excluded: ~150 generic multi-zone world drops (Elwynn rule -
including every Varo'then-table recipe: 7989/7992/12683/14479/11225/16043
at 400-650 droppers across ~25 zones, and 9295 at 560 droppers despite
rare Hawkhelm dropping it); near-misses 13491 (Felwood second dropper),
14477 (EPL second dropper), 251438 and 252858 (sole droppers 6117/6116
spawn Ashenvale as well as Azshara - dual-zone single-droppers stay out
per the Felwood precedent); quest-reward recipes (unverifiable -
no reward data in quest records); trainer-taught staples.
