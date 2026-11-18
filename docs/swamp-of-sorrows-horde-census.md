# Swamp of Sorrows (Horde) census (game data, accept-zone key 1435)

Accept-zone key: **1435** (verified by count: 52 quest records carry
`zone=1435` in this data build - the same key and the same count the
Alliance census (`docs/swamp-of-sorrows-census.md`) examined). Race
masks in the data: 8589934770 = Horde, 4294967373 = Alliance, null =
neutral (both factions).

Method: every zone-1435 record examined against the packs inclusion
rules; the Alliance censuss banked 17 Horde set-asides reconciled one
by one against the Horde-mask pool (the 17 IDs survive in that doc);
start-item AND start-object scan run over the Horde pool;
pres/exclusives and outside legs resolved from data (`npcs.json`,
`objects.json`, `items.json`, `quests.json`, `spawnz.json`
cross-checked).

Pool breakdown: 17 Horde-mask + 17 Alliance-mask + 18 null. The 17
Horde-mask zone-1435 records are exactly the 17 banked set-asides
(verified programmatically - no more, no fewer): 698, 699, 1418, 1422,
1424, 1426, 1427, 1428, 1429, 1430, 1445, 2621, 2622, 2623, 2784, 87451,
93663. Zero Horde-mask records sit inside the Alliance
`swamp-of-sorrows` contract (19 quests), so the exclusive-contracts
precedent holds with no directional check needed.

## Band: 30-38

Contracted minLevels run 30 (1418, 93663 - in-zone intros, free entry
per precedent) through 38 (1424, 1429, 1445 - the Atalai chain top),
with the m35 bulk (698/699/1422/1426/1427/1428/1430) between. m45+ is
OUT: the Fallen Hero chain links (2621/2622/2623/2784, m45) and 87451
(m45). Derived from the Horde histogram, not copied from the Alliance
30-38 - the edges coincide because both factions work the same floor
and the same chain top.

No race header for the guide: no contracted quest is locked to a single
Horde race. No class gates, no profession gates, no skill-gated records
(the pool scan found no CLASS or SKILL flags on any Horde record).
Capital legs ride honest expedition steps below (Badlands for 1418,
Hinterlands for 1429, Undercity-adjacent? no - see legs).

Reconciliation of the Alliance censuss banked set-asides: 12 IN, 5 OUT
(2621/2622/2623/2784 above-band m45; 87451 above-band m45 - each ruled
below).

Item-start enumeration (explicit start-item AND start-object scan over
the Horde pool): NO Horde item-starts and NO Horde object-starts (87451
carries a `sourceItem` field 280390 - Carved Stone Trinket - with an
empty start record, i.e. an auto-accept-style record; it is OUT
above-band regardless, so the mechanism is noted, not resolved).
93663s objective item (260452 Couriers Shipment, count null) names no
source anywhere in the data - sourceless, ships with an honest bag note.
The 654-style sourceless accept does not occur here (93663 accepts from
an NPC, only its objective item is sourceless).

## IN (12)

Stonard hub (Dar 5591 @44.7,57.21; Helgrum the Swift 1442 @47.74,55.2;
Felzerul 1443 @47.93,54.78):

| 698 Lack of Surplus | 40/35 | no pre | 8 Unprepared Sawtooth Flank 6169 off Sawtooth Crocolisk 1082 (25%, 24 pts west-center) + Sawtooth Snapper 1087 (25%, 24 pts east) -> Dar |
| 699 Lack of Surplus | 42/35 | pre 698 (IN) | 6 Sawtooth Snapper Claw 6168 off Snapper 1087 (80%, east) -> TokKar 5592 (@81.32,80.97, east); unlocks the Threat chain below |
| 1418 Neeka Bloodscar | 35/30 | no pre; starter Helgrum 1442 in-zone | no objectives; ends Neeka Bloodscar 5394, Badlands (1418 @6.49,47.2) - Badlands expedition turn-in |
| 1422 Threat From the Sea | 45/35 | pre 699 (IN) | no objectives; ends Katar 5593 (@83.76,80.41, east) |
| 1426 Threat From the Sea | 43/35 | pre 1422 (IN) | 10 Marsh Murloc 747 + 10 Marsh Inkspewer 750 + 10 Marsh Flesheater 751 (east clusters: 747s at 82-83,88-94; 750s at 62-64,80-87; 751s at 60-62,81-84) -> Katar |
| 1427 Threat From the Sea | 43/35 | pre 1426 (IN) | no objectives; ends TokKar 5592 (@81.32,80.97, east) |
| 1428 Continued Threat | 45/35 | pre 1427 (IN) | 10 Inkspewer 750 + 10 Flesheater 751 + 10 more (same east clusters) -> Katar; chain finale |
| 1430 Fresh Meat | 44/35 | no pre | 10 Monstrous Crawler Leg 6184 off Monstrous Crawler 1088 (12%, 24 pts far east/south) -> Dar |
| 93663 Lost in Transit | 35/30 | no pre | objective item 260452 Couriers Shipment (count null, NO source anywhere - honest bag note, R5 class); ends Magtoor 1776 (@25.98,31.4, in-zone) -> Magtoor |

Felzerul post (1443 @47.93,54.78, Stonard edge):

| 1424 Pool of Tears | 43/38 | no pre | 10 Atalai Artifact 6175 off objects 30854/30855/30856 (100% each, shared east-center cluster ~61-65,49-57) -> Felzerul |
| 1429 The Atalai Exile | 44/38 | pre 1424 (IN) | no objectives; ends Atalai Exile 5598, Hinterlands (1425 @33.75,75.21) - Hinterlands expedition turn-in |
| 1445 The Temple of AtalHakkar | 50/38 | pre 1444 (Horde, Hinterlands-accept 5598, uncontracted - soft-pre mini below; the return link the brief names sits in the Hinterlands Horde set-aside pool, homed there and cited here) | 20 Fetish of Hakkar 6181 off the in-zone Atalai family (Cursed 5243, Enthralled 5261, Mummified 5263, Priest 5269, Veyzhak 5399, Zekkis 5400, Kazkaz 5401 - all 1435, 40%; dungeon-side sharers noted, not used); ends Felzerul (in-zone) |
| `when onquest 1444` soft-pre mini at Felzerul (turn in 1444, accept 1445) - the pre ends in-zone at the chains head (Kadrak pattern; 1444 accepts at the Exile in the Hinterlands and lives outside every contract) |

## OUT (5)

- Above-band (5): 2621 The Disgraced One, 2622 The Missing Orders, 2623 The Swamp Talker, 2784 Fall From Grace (all L50-55/m45, Fallen Hero chain) + 87451 Memories of Rockard (L55/m45, empty start record with `sourceItem` 280390 noted but moot - minLevel alone excludes it). The Alliance census outed its own Fallen Hero chain (2681+ etc., m45) on the same rule; the mirror holds.

Alliance-only zone-1435 records (set aside for the record - none duplicated here): per the Alliance census OUT ledger the shared/null-mask records stay in the main guides contract, which this round ungates. The Horde-side Timbermaw... (none - no Timbermaw Horde records exist; the Alliance 6131/8460 twins are null-mask shared, homed in the main contract).

## BORDERLINE (all decided, none silent)

(a) 1418s Badlands ender: 1418 accepts in-zone (Helgrum) and ends at Neeka Bloodscar 5394, Badlands - an expedition turn-in, IN (chains that start here and end anywhere are IN; the Badlands leg is a short hop, said plainly). Same shape as 1429s Hinterlands ender - both expedition turn-ins, both IN.
(b) 1445s dungeon adjacency: 1445s objectives are farmed off in-zone droppers at 40% (7 mob types); the spawnless dungeon-side sharers are noted, never used. No dungeon-entrance complete is needed because no objective requires the dungeon - if a future build moves the drops dungeon-only, the step gains the entrance handling.
(c) 87451: ruled OUT on minLevel (m45) with the empty-start/sourceItem shape explicitly left undecided-but-documented (auto-accept item-start vs broken). The minLevel rule disposes of it either way; a future build that lowers its minLevel would need the mechanism ruling first.
(d) 93663s sourceless objective: NPC-accept (normal, in-zone) with a sourceless objective item - R5 bag-note handling, no collect lines (the 8411-reagent pattern). Not an item-start (contrast 654), so no R2 exposure.
(e) Band 30-38: derived from the Horde histogram (floor m30 intros, bulk m35, top m38 chain; m45+ out). Coincides with the Alliance edges; the reasoning is independent.

