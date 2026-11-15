# Azshara census — Alliance route (order 31)

Source: local game data (`--product wowf` + QuestieDB), zone key **1447**
(Azshara, areaId 16). Candidate rule: every quest record with `zone == 1447`
OR `area == 16` (catches the cross-keyed records below), plus the null-zone
pointer 96246 examined as chain context. Game data wins over all else.

Examined: **95** (86 accept/zone-keyed + 9 area-16/broken context records).
IN (contract): **52**. OUT: **43** (repeatable 3, Horde 30, above-band 9,
broken 1).

## Band derivation

Contracted minLevels cluster 45-55: the 45 block (Loramus chain, Sanath,
Kim'jael, Loh'atu, Truesong/Saria/Berdun hub chains, Ekkal), the 47 block
(Kim'jael follow-ups, Saria tablets chain), the 50 block (Ogtinc/Xylem class
chains, Berdun Deadliest Catch, Pay Dirt!), the 55 top (Hydraxis 6804/6805),
plus 5141 (min 40, Dragonscale spec with in-zone scale source), two min-1
records (8720 Lunar elder, 94316 writ), and five null-min records (86746,
86747, 91877, 92069, 97327 — no floor stated, objectives placed in-zone).
Own-levels run to 60 on finales whose floor is in band — that is the
long-standing rule, not an exception. **Band: 45-55.**

## IN ledger (52)

| ID | Title | lvl | min | Giver | Notes |
| 3141 | Loramus | 57 | 45 | Loramus Thalipedes L60 | pre 2744 Swamp (structural) |
| 3381 | A Meeting with the Master | 48 | 45 | Sanath Lim-yo L50 | feathers, hippogryphs in-zone |
| 3461 | Return to Tymor | 52 | 45 | Pilot Xiggs Fuselighter L45 | BORDERLINE 2; turn-in Tymor Ironforge |
| 3508 | Breaking the Ward | 58 | 45 | Loramus Thalipedes L60 | pre 3141 |
| 3509 | The Name of the Beast | 58 | 45 | Loramus Thalipedes L60 | turn-in Arkkoroc |
| 3510 | The Name of the Beast | 58 | 45 | Lord Arkkoroc L60 | 3 Hetaera heads, Hetaera placed |
| 3511 | The Name of the Beast | 58 | 45 | Lord Arkkoroc L60 | turn-in Loramus; next 3602 |
| 3601 | Kim'jael Indeed! | 53 | 47 | Kim'jael L46 | 4 items, one ground-spawn object, 13 pts |
| 3602 | Azsharite | 58 | 45 | Loramus Thalipedes L60 | 20x azsharite, 4 objects, south ruins |
| 3621 | The Formation of Felbane | 58 | 45 | Loramus Thalipedes L60 | turn-in Galvan, Stranglethorn (1434, not Stonetalon - data wins) |
| 5141 | Dragonscale Leatherworking | 55 | 40 | Peter Galen L50 | R5; excl 5143/5144 (other zones); Mageweaver scales in-zone |
| 5534 | Kim'jael's "Missing" Equipment | 53 | 47 | Kim'jael L46 | Some Rune, Spitelash in-zone |
| 5535 | Spiritual Unrest | 47 | 45 | Loh'atu L45 | BORDERLINE 1; kills placed Azshara |
| 5536 | A Land Filled with Hatred | 47 | 45 | Loh'atu L45 | BORDERLINE 1; Haldarr all Azshara |
| 6804 | Poisoned Water | 56 | 55 | Duke Hydraxis L60 | EPL bracer expedition |
| 6805 | Stormers and Rumblers | 57 | 55 | Duke Hydraxis L60 | Feralas expedition (BORDERLINE 11) |
| 8153 | Courser Antlers | 52 | 50 | Ogtinc L45 | only Hunter; pre 8151 outside (structural) |
| 8231 | Wavethrashing | 52 | 50 | Ogtinc L45 | only Hunter |
| 8232 | The Green Drake | 52 | 50 | Ogtinc L45 | only Hunter; Tooth R2 (Morphaz unplaced) |
| 8235 | Encoded Fragments | 52 | 50 | Archmage Xylem L60 | only Rogue; pre 8234 Alterac (structural) |
| 8236 | The Azure Key | 52 | 50 | Archmage Xylem L60 | only Rogue; key R2; turn-in Ravenholdt (BORDERLINE 9) |
| 8251 | Magic Dust | 52 | 50 | Archmage Xylem L60 | only Mage; pre 8250 IF (structural) |
| 8252 | The Siren's Coral | 52 | 50 | Archmage Xylem L60 | only Mage |
| 8253 | Destroy Morphaz | 52 | 50 | Archmage Xylem L60 | only Mage; shard R2 |
| 8255 | Of Coursers We Know | 52 | 50 | Ogtinc L45 | only Priest; pre 8254 IF (structural) |
| 8256 | The Ichor of Undeath | 52 | 50 | Ogtinc L45 | only Priest; ichor off Azshara ghosts |
| 8257 | Blood of Morphaz | 52 | 50 | Ogtinc L45 | only Priest; blood R2; turn-in Greta, Felwood |
| 86746 | The Legashi Threat | 53 | null | Ekkal L50 | null-min precedent; kills placed |
| 86747 | Legashi Horns | null | null | NONE (turn-in-only; end Ekkal) | 95795 mirror; accept+turnin Ekkal |
| 8720 | Skygleam the Elder | 60 | 1 | Elder Skygleam L60 | BORDERLINE 4; optional + seasonal note |
| 88807 | Slay the Spitelash | 48 | 45 | Commander Truesong L45 | kills 24-38 x |
| 88809 | Preserving Eldarath | 52 | 45 | Commander Truesong L45 | 12 relics + Sarthiss head, placed |
| 88812 | Reclaiming Ravencrest | 55 | 47 | Commander Truesong L45 | no objectives; pointer to 88813 |
| 88813 | The Head of the Serpent | 55 | 47 | Commander Truesong L45 | Krellian head, placed |
| 88821 | Making Contact | 51 | 47 | Commander Truesong L45 | no objectives; turn-in Saria |
| 88857 | Saving a Sentinel | 47 | 45 | Sentinel Keldara Sunblade L45 | no objectives; turn-in Truesong |
| 88884 | Highborne Tablets | 52 | 47 | Saria Fairmoon L55 | 3 tablets R2 (objects unplaced) |
| 88917 | Slithering Looters | 52 | 47 | Saria Fairmoon L55 | staff R2 (object unplaced) |
| 89001 | Home on the Range | 48 | 45 | Berdun Cliffbrew L45 | hides, Mosshoof placed |
| 89013 | Gettin' Buzzed | 48 | 45 | Berdun Cliffbrew L45 | honey, wasps placed; alt-pre Horde (BORDERLINE 7) |
| 89015 | Deadliest Catch | 56 | 50 | Berdun Cliffbrew L45 | accept-only; sharks placed |
| 89037 | Murloc Thieves | 52 | 47 | Saria Fairmoon L55 | crystal, Razorgill east coast |
| 89038 | A Monumental Task | 55 | 47 | Saria Fairmoon L55 | mark R2 (object unplaced) |
| 89053 | Your Final Reward | 55 | 47 | Saria Fairmoon L55 | turn-in at knapsack object |
| 89228 | Winter Frontier Fishery | 48 | 45 | Berdun Cliffbrew L45 | squid R2 (fished, no source); alt-pre Horde |
| 89470 | Ill Tidings | 55 | 47 | knapsack object (start) | object-handoff from 89053; turn-in Truesong |
| 90813 | Pay Dirt! | 53 | 50 | NONE (turn-in-only; end Berdun) | crystal, Cliff Walkers placed |
| 91877 | Demon Hunter's Hunter | 55 | null | Loramus Thalipedes L60 | accept-only; no objectives |
| 92069 | Claws That Rend, Tusks that Gore | 58 | null | Ogtinc L45 | BORDERLINE 3; both droppers unplaced (R2) |
| 92345 | Beneath Nordrassil | 55 | 45 | Commander Truesong L45 | turn-in Bearwalker, Darnassus (BORDERLINE 10) |
| 94316 | Craftsman's Writ: Potion of Demonslaying | 60 | 1 | Archmage Xylem L60 | accept-only writ; R5 handling |
| 97327 | Blackmaw Pouches | 60 | null | Ekkal L50 | BORDERLINE 3; pouches placed; next 96246 dead |

## OUT (43)

Repeatables (3): 3382, 3421, 3503 (3503 repeats 3381).
Above-band (9): 6821 (min 56), 6822 (min 57), 6823/6824/7486
(min 60, Hydraxis endgame), 9362/9364 (min 60, Xylem), 8575 (min 60;
Azshara accept-pin via Spirit of Azuregos and area 16, but the floor is
60 — BORDERLINE 5), 8729 (min 60, Tanaris accept).
Broken (1): 96246 (null zone/level; dead next-pointer of 97327).
Horde set-aside (30): 3504, 3505, 3506, 3507, 3517, 3518, 3541, 3542,
3561, 3562, 3563, 3564, 3565, 91488 (twin of 89001), 91497, 91500,
91531, 91538, 91547, 91568, 91569, 91607 (twin of 90813), 91608 (twin
of 89013), 91610 (twin of 89228), 91611 (twin of 89015), 91685,
91734, 91735, 91737, 92346 (twin of 92345).

## BORDERLINE (argued, nothing silent)

1. 5535/5536 ownership. Loh'atu dual-spawns Ashenvale/Azshara and the
records carry qzone 1440 — but their area is 16 (Azshara), the Azshara
spawn sits at the west-coast hub, 5536's kills (Haldarr 6125/6126/6127)
spawn ONLY in Azshara, and 5535's kills are Azshara-placeable. Ashenvale's
census did not contract them. IN Azshara (Felwood-968 precedent).
2. 3461 ownership. qzone 1455 (Ironforge) but the ONLY accept-spawn in
the data is Xiggs at 77.81,91.4 in Azshara; Ironforge contracted only the
pre-quest 3449. Accept-spawn wins over the zone tag. IN Azshara, with a
structural pre-warning and an Ironforge turn-in expedition.
3. Null-min stretch: 92069 (lvl 58) and 97327 (lvl 60). No floor stated;
both objectives are placed in-zone. Felwood contracted null-min records
at its band top; these stretch the precedent one and two own-levels
higher. IN, flagged for Butler's appeal.
4. 8720 (Elder Skygleam, min 1 / lvl 60, no event flag in data). Lunar
Festival content by name but the data carries no seasonal flag, and the
minLevel floor is 1. IN as optional + seasonal-timing note.
5. 8575 OUT. The accept-pin IS Azshara (Spirit of Azuregos, area 16) and
the chain ends in Tanaris — but minLevel is 60, above the 45-55 band.
Above-band wins over accept-pin. Appealable: contracting it would mean
taking min-60s, which the band rule exists to exclude.
6. Split/degenerate records (86747, 90813 turn-in-only; 91877, 89015,
94316 accept-only): contracted with honest notes, no invented lines
(Redridge 95795 / Ironforge accept-only precedent).
7. 89013/89228 carry Horde 91488 as an ALT pre alongside 89001. The
Alliance route satisfies the pre via 89001; noted, not gated.
8. 5141 vs 5143/5144: the data marks them mutually exclusive
(excl[5143,5144]). Accept-zone decides — Dragonscale (Azshara) is ours;
Tribal (Thousand Needles) and Elemental (Searing Gorge) belong to their
zones. No silent choice; the exclusion is data, the pick is geography.
9. 8236 turn-in: Ravenholdt triple-spawns (Alterac/Hillsbrad/Hinterlands
points). Ravenholdt Manor is the Hillsbrad holding — turn-in at the
1424 point with an expedition note. The other two data points are named
here so the choice is auditable.
10. 92345 turn-in: Bearwalker dual-spawns Teldrassil/Darnassus. The
Cenarion Enclave (Darnassus) is the druid-hub spawn — turn-in at the
1457 point with an expedition note.
11. 6805 expedition: Stormers/Rumblers spawn in Feralas AND Silithus.
Feralas (Alliance hub, Feathermoon) is the route-consistent pick; both
data clusters are named here.
12. Class gates: Hunter 8153/8231/8232, Rogue 8235/8236, Mage
8251/8252/8253, Priest 8255/8256/8257 (class-mask data). Nothing contracted
is race-locked — no race header. Profession: 5141 optional +
when-skill gated + bag note (R5); 94316 writ likewise (Alchemy).
No Shaman/Paladin/Druid class quests accept in Azshara in this data.

## Residue the guide must carry

R2 (sourceless objectives, bag notes): Morphaz trio (8232/8253/8257),
Azure Key (8236), tablets trio (88884), Selwyn staff (88917), Queen's
mark (89038), Winter Squid (89228, fished), Withermaw/Bonesnout pair
(92069). Structural pre-warnings: 3141 (2744 Swamp), 8153 (8151),
8235 (8234 Alterac), 8251 (8250 IF), 8255 (8254 IF), 3461 (3449 IF).
Expeditions: Ironforge (3461), Stranglethorn (3621), Felwood (8257),
EPL (6804), Feralas (6805), Hillsbrad (8236), Darnassus (92345).
