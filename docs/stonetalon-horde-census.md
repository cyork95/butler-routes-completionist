# Stonetalon Mountains (Horde) census (pack 0.103.0)

Accept-zone key: **1442** (69 quest records carry zone=1442 — verified by counting
quests.json; same key the Alliance census used).

Method: every zone-1442 quest examined against the pack's inclusion rules; the
Alliance census's 32 banked Horde set-asides reconciled one by one; six
zone-1413 set-asides checked against the Barrens contract; start-item/object
scan run over all Horde-mask candidates; pres/exclusives resolved from data.

Race masks in the data: 8589934770 = Horde, 4294967373 = Alliance, null =
neutral (both factions). Exclusive-contracts precedent (Ashenvale round: zero
quest overlap between the Alliance and Horde contracts) applies: neutral quests
already contracted in `stonetalon` (Alliance) are NOT duplicated here.

## Band: 12-30

Lowest contracted minLevel is 12 (6523 Protect Kaya); highest contracted quest
level is 30 (1154/1159/6627 Test of Lore). Quest 94216 (Craftsman's Writ,
lvl 60, min 1) is IN as the L60 writ special class via the minLevel rule — same
treatment the Alliance census gave the four neutral writs.

## IN (23)

| ID | Title | Lvl/min | Accept | Notes |
|----|-------|---------|--------|-------|
| 1058 | Jin'Zil's Forest Magic | 26/20 | Witch Doctor Jin'Zil 3995 (74.54, 97.94) | 4 item drops, all droppers in-zone (Sap Beast, Twilight Runner, Coursers, Fey Dragons, north) |
| 1087 | Cenarius' Legacy | 25/20 | Braelyn Firehand 4198 (45.94, 60.42) | kills in-zone (Sons/Daughters/Botanists) |
| 1088 | Ordanus | 29/20 | Braelyn Firehand | complete at Keeper Ordanus 4273, Ashenvale (62.05, 51.37) — expedition; spawnz world spawn and npcs.json 1440 pts agree exactly |
| 1089 | The Den | 29/20 | Braelyn Firehand | accept-only (no end in data) — contracted with honest note; the three keys (5689/5690/5691) have no droppers anywhere — R2 bag notes |
| 1154 | Test of Lore | 30/25 | Braug Dimspirit 4489 (78.8, 45.69) | Legacy of the Aspects 5860 has no droppers — R2 bag note; pre 1152 accepts from Dorn Plainstalker in Thousand Needles (zone 1441, Horde, out-of-contract) — soft-pre mini-step |
| 1159 | Test of Lore | 30/25 | Braug Dimspirit | expedition turn-in to Parqual Fintallas 4488, Undercity (57.8, 65.42); pre 6627 in-contract |
| 1511 | Ken'zigla's Draught | 20/20, Warlock | Ken'zigla 4197 (73.25, 95.13) | expedition turn-in to Grunt Logmar 5911, Camp Taurajo (44.62, 59.27); pre 1510 is Barrens-contracted (pack-homed); excl 1472 — see BORDERLINE |
| 5881 | Calling in the Reserves | 28/23 | Maggran Earthbinder 11860 (47.2, 61.16) | expedition turn-in to Grish Longrunner 12576, Great Lift (44, 92) |
| 6282 | Harpies Threaten | 26/18 | Maggran Earthbinder | harpy kills in-zone (northwest cluster) |
| 6283 | Bloodfury Bloodline | 26/18 | Maggran Earthbinder | Ripper's Remains off Bloodfury Ripper 12579, single in-zone point (30.75, 61.91) |
| 6284 | Arachnophobia | 21/15 | object-start Wanted Poster: Besseleth 177904 at (59.06, 75.71), turn-in Maggran | object-started; Besseleth 11921 has 3 in-zone points (51.96, 73.85) cluster for the Fang |
| 6301 | Cycle of Rebirth | 23/17 | Tammra Windfield 11864 (47.46, 58.38) | Gaea Seeds 16205 have no droppers — R2 bag notes |
| 6381 | New Life | 25/17 | Tammra Windfield | object 177929, 34 in-zone points (southwest mounds) |
| 6393 | Elemental War | 25/19 | Tsunaman 11862 (47.36, 64.25) | Incendrites off fire elementals, all in-zone |
| 6421 | Boulderslide Ravine | 18/14 | Mor'rogal 11861 (47.22, 64.05) | event placed (58.22, 89.51); Resonite Crystals 16581 have no droppers — R2 bag notes |
| 6461 | Blood Feeders | 19/13 | Xen'Zilla 12816 (71.25, 95.03) | Deepmoss kills in-zone (southeast) |
| 6481 | Earthen Arise | 20/14 | Mor'rogal | Goggeroc 11920 at (57.4, 89.4) per npcs.json 1442 pts (spawnz carries no entry — source noted in guide) |
| 6523 | Protect Kaya | 18/12 | Kaya Flathoof 11856 (73.48, 85.59) | escort event at Camp Aparaje (77.1, 90.85); follow-up 6401 is Barrens-contracted — handoff noted |
| 6542 | Report to Kadrak | 19/17 | Darn Talongrip 11821 (73.25, 94.89) | expedition turn-in to Kadrak 8582, N. Barrens (48.12, 5.42); excl 6541 (Alliance twin) — chain-consistent Horde pick |
| 6562 | Trouble in the Deeps | 22/17 | Tsunaman | expedition turn-in to Je'neu Sancrea 12736, Ashenvale (11.56, 34.29) — NAMED CHECK: contracted here; the Ashenvale soft-pre mini now resolves end to end |
| 6627 | Test of Lore | 30/25 | Braug Dimspirit | event at Braug (78.75, 45.63); pre 1154 in-contract |
| 86576 | Bloodfury Trinkets | 26/18 | Maggran Earthbinder, turn-in Mor'rogal | Sunstones off harpies incl. Ripper, all droppers in-zone |
| 94216 | Craftsman's Writ: Elixir of Lesser Agility | 60/1 | item-start 264016 (no droppers/vendors anywhere — R2 bag note) | writ special class, minLevel rule; turn-in Ziz Fizziks 4201 (58.99, 62.6) |

## OUT

32 banked set-asides — 23 IN above; OUT (9):
- Above-band: 6568, 6602 (L60 Onyxia attunement, min 55; zone-field quirk noted — giver Rexxar @1443 Desolace, accepts outside in any case).
- Mount/broken: 97446 (Tauren-only mount, no start/end data, long excl list — mount-exchange class).
- Accept-outside (zone 1413, all six verified already homed in the Barrens contract — no double-contract): 6401 (follow-up of 6523), 6548, 6629 (Kaya chain), 1062, 1063, 1068 (Barrens chain).

Neutral zone-1442 quests already contracted in the Alliance `stonetalon` guide — NOT
duplicated here (Ashenvale exclusive-contracts precedent): 1090, 1092, 1093,
1094, 1096 (Gerenzo line), 78270 (Rogue), 79974, 79980, 80001 (Eagle's Fist
chain), 94225, 94234, 94243, 94252 (writs).

Alliance-only zone-1442 quests (set aside for the record): 1057, 1059, 1071,
1072, 1075, 1079, 1080, 1082, 1083, 1084, 1085, 1091, 1382, 1385, 1387, 1437,
1438, 1454, 1456, 1457, 1458, 1459, 1466, 1467, 2931, 86574; above-band
Alliance: 261, 1052 (min 34), 7041 (min 41), 7065 (min 45).

Candidates examined: 69 zone-1442 + 6 zone-1413 set-asides = 75. IN 23, OUT 52.

## BORDERLINE

(a) 1511 vs 1472 (mutually exclusive Warlock variants): 1472 (Devourer of
Souls) accepts in Undercity (zone 1458), shows level -1 (broken/PH-class
record), and sits outside the Stonetalon chain, while 1511 continues the
Barrens-contracted 1510 and the Sun Rock chain. Contract 1511, exclude 1472
(city-accept + broken level + off-chain). Chain-consistent pick, decided openly.

(b) Null-mask neutrality is not a Horde ticket: the Gerenzo line, 78270, the
Eagle's Fist links and the four neutral writs are all takeable by Horde
characters but live in the Alliance contract by the settled exclusive-contracts
design (a quest is contracted exactly once; cf. Ashenvale 0 overlap). A Horde
player wanting those lines uses the Alliance file's steps. Logged, not
duplicated.

(c) 1088's cross-zone kill is data, not a stretch: the npc record's 1440 pts
and the spawnz world spawn convert to the identical Ashenvale point (62.05,
51.37 vs 62.05, 51.36). Expedition step with a deliberate frame switch.
