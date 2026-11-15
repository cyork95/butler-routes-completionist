# Blasted Lands census (game data, accept-zone key 1419)

Source: local Forever game data (questie-forever quest/NPC/object/item
dumps). Key 1419 confirmed by zone-table lookup (Blasted Lands, areaId 4)
and a 33-record candidate set of classic Blasted Lands quests. Races
4294967373 = Alliance, races null = neutral (available to all); no
8589934770 (Horde) record accepts here — the Horde set-aside is 0, with
double evidence (zero Horde-mask records in-zone AND zero Horde-mask quests
from 1419-spawning givers anywhere; the mask itself is valid, 1601 records
carry it elsewhere).

## Band derivation

minLevel histogram over all 33 zone-keyed records: min1 x1 (8647, event),
min30 x1 (1423, repeatable), min40 x3 (the Grimshade chain 2991-2993),
min45 x20 (the bulk: Kum'isha, Drazial/Lynnore, Forever records, orphan
chain), min50 x2 (2783 Petty Squabbles, 4128 Ragnar Thunderbrew),
min60 x3 (the Warlock Dreadsteed chain 7581-7583), null x3 (87295, 91882,
93685, judged individually below). Band bottom is 40, not 45, because the
genuine Grimshade chain bottoms at min40; band top is 50, the two min50
finale-style quests (both ending outside the zone) still anchor in band.
Band: 40-50.

## IN - 21 quests (the contract)

| ID | Title | Lvl | Giver | Notes |
|----|-------|-----|-------|-------|
| 2521 | To Serve Kum'isha | 55 | Kum'isha the Collector (51.98,35.65) | complete 8244 Flawless Draenethyst Sphere @Dreadmaul camp |
| 2581 | Snickerfang Jowls | 50 | Bloodmage Drazial (50.55,14.20) | 8391x3/8392x2/8393x1 @snickerfangs/boars/scorpoks |
| 2583 | A Boar's Vitality | 50 | Bloodmage Drazial | 8392x3/8393x2/8394x1; no pre, hunt with 2581 |
| 2585 | The Decisive Striker | 50 | Bloodmage Drazial | 8393x3/8396x2/8392x1; no pre, hunt with 2581 |
| 2601 | The Basilisk's Bite | 50 | Bloodmage Lynnore (50.64,14.30) | 8394x10/8396x2; no pre |
| 2603 | Vulture's Vigor | 50 | Bloodmage Lynnore | 8396x10/8391x2; no pre |
| 3501 | Everything Counts In Large Amounts | 55 | Kum'isha the Collector | complete 10593 Imperfect Draenethyst Fragment @Dreadmaul camp |
| 2991 | Nekrum's Medallion | 47 | Thadius Grimshade (66.90,19.47) | pre 2990 (Hillsbrad, uncontracted) -> soft-pre mini-step; complete 9471 point-less (sole dropper 7796 Nekrum Gutchewer has no spawns anywhere; honest note, Badlands 713 precedent) |
| 2992 | The Divination | 47 | Thadius Grimshade | kill objective IS the giver (kill:8022 @his point); needs 2991 |
| 2993 | Return to the Hinterlands | 47 | Thadius Grimshade | no objectives; expedition turn-in to Gryphon Master Talonaxe @Hinterlands 1425 (9.75,44.47); needs 2992 |
| 2783 | Petty Squabbles | 57 | Ambassador Ardalan (67.57,19.29) | min50 finale; no objectives; expedition turn-in to Fallen Hero of the Horde @Swamp 1435 (34.29,66.14) |
| 4128 | Ragnar Thunderbrew | 55 | Enohar Thunderbrew (63.63,20.63) | min50 finale; no objectives; expedition turn-in to Ragnar Thunderbrew @Dun Morogh 1426 (46.83,52.36) |
| 81917 | Chains That Bind | 54 | Bloodmage Lynnore | pre 81900 (Searing Gorge, future/uncontracted) -> soft-pre mini-step; complete 220214 x5 @Shadowsworn clusters |
| 81919 | Brought to Heel | 54 | Bloodmage Lynnore | item-start 220216 Infernal Lasso has NO source in data (no drops, no vendors) -> bag note + optional sourcing, R2 expected; complete 220213 x1 @Calefactus (43.74,34.38, sole dropper) |
| 96798 | Into the Darkness | 54 | Lieutenant Connar (66.07,19.40) -> Sergeant Danneth-A (66.73,31.67) | no objectives; pre 96797 (Alterac, uncontracted) -> structural warning, chain named |
| 96799 | A Heavy Responsibility | 54 | Connar -> Sergeant Danneth-B (65.23,15.33) | pre 96811 (contracted); needs 96811 |
| 96811 | Escaping the Shadows | 54 | Danneth-A -> Connar | pre 96798 (contracted) |
| 96812 | Thicker Than Water | 54 | Danneth-B -> Orphan Matron Aria @Alterac 1416 (21.62,73.18) | pre 96799 (contracted); expedition turn-in; ends the orphan chain |
| 87295 | Deflective Surface | 52 | Bernie Heisten (63.51,17.01) | BORDERLINE IN (see 1): complete 280181 x10 @Redstone basilisks |
| 91882 | The Grand Alliance | 55 | Ardalan -> Sefira Everbright @Hyjal 2482 (15.67,54.66) | BORDERLINE IN (see 2): breadcrumb into Sefira's Hyjal chain; endgame expedition leg with honest note |
| 93685 | To Serve Kum'isha | 55 | Kum'isha -> Kum'isha | BORDERLINE IN (see 3): same title as 2521 but a different chain (pre 93684 Swamp, uncontracted); no objectives, accept+turnin only |

All 21 CONTRACTED. No class restrictions on any record (classes null
except the OUT warlock trio), no race gates needed (Alliance + neutral
only).

## OUT - 12 records with reasons

- Repeatables (8): 1423 The Lost Supplies (also item-start 6172, but the
  repeatable rule wins — Seal of the Earth precedent); the even-numbered
  Drazial/Lynnore/Kum'isha follow-ups 2522, 2582, 2584, 2586, 2602, 2604,
  3502 (their one-time odds 2521/2581/2583/2585/2601/2603/3501 stay IN and
  complete the set).
- Seasonal/event (1): 8647 Bellowrage the Elder (event=7, Lunar Festival).
- Above-band class chain (3): 7581 The Prison's Bindings, 7582 The
  Prison's Casing, 7583 Suppression (see BORDERLINE 4).
- Horde set-aside: 0 records (evidence above).

## BORDERLINE (argued, none decided silently)

1. Deflective Surface (87295) IN: lvl52, null minLevel, start+end Bernie
   Heisten, objective item 280181 Redstone Basilisk Scale exists and drops
   from two in-zone basilisks. The pack contracts thin null-min records
   routinely (32 across the pack, e.g. Darnassus 98096, Redridge 93551 —
   the latter lvl58 accept-only in a 14-26 zone, which kills any
   level-vs-band objection). Every ID in 87295 resolves to a real,
   placed entity, so it is contracted; its lvl52 sits just over the band
   top and is noted as such.
2. The Grand Alliance (91882) IN: lvl55, null minLevel, start Ardalan,
   end Sefira Everbright (Hyjal 2482), no objectives, objectiveText reads
   like a real breadcrumb ("Search Mount Hyjal for remnants of the Grand
   Alliance"), and Sefira's Hyjal follow-ups exist in the data (90750,
   92449, 92591, 94832 at min54-57). Structurally it matches contracted
   thin records (98096: start NPC, end NPC, no objectives). The chain
   ending outside is IN by rule; the Hyjal turn-in rides a labeled
   endgame expedition leg (Sefira's data-placed point), with an honest
   note that it is far above band. Expected R1 on that leg is accepted
   expedition residue.
3. To Serve Kum'isha (93685) IN: lvl55, null minLevel, start+end Kum'isha,
   no objectives, pre 93684 (Swamp of Sorrows) which itself chains from
   93679 with next-pointers — a linked Forever chain, not a stub. Same
   title as classic 2521 but a different chain (different pres,
   different objectives-or-none); the same-title-twin precedent
   (Harvesting 92910/92911, A Sign of Hope 720/721) routes both, so both
   2521 and 93685 are contracted. The uncontracted Swamp pre means a
   structural warning on the accept, chain named. This differs from the
   Badlands 97663/97821 OUTs: there the records failed to resolve
   (97821 no accept; 97663 flagged for re-census pending objectives),
   while here every referenced entity resolves — 87295's item drops from
   placed mobs, 91882's chain context exists, 93685's pre-chain links.
   (97663 could be re-examined under this lens in a later pass; not this
   round's call.)
4. Dreadsteed chain (7581/7582/7583) OUT: min60/lvl60, 10 over the band
   top, Warlock-only (classes=256; Hunter=4/Priest=16/Mage=128
   calibration). The objectives sit in endgame dungeon space (Satyr Blood
   18603 from Dire Maul satyrs, Tears of the Hederine 18604 from Felwood
   1452 mobs, Imprisoned Doomguard via object 179644), the sole 7583
   starter 18601 Glowing Crystal Prison has NO source anywhere in the
   data, and sole 7581 dropper 11451 Wildspawn Satyr has NO spawns in the
   data — the chain cannot be honestly placed or sequenced at 40-50, and
   would wedge on R2 as well as level. The minLevel rule is mechanical
   and exceptionless; the pack's answer for class chains that outgrow
   their zone is a class guide (Moonglade-Druid precedent), so this chain
   is logged as the seed of a future Warlock class guide, not forced into
   a 40-50 route. Daio's dual spawn (1419 + STV 1434) does not move it:
   q.zone keys 1419. If Butler rules otherwise, the three slot in as one
   `only Warlock` block (accepts from Daio + Dire Maul expedition
   completes).
5. Out-of-zone pres (2990 Hillsbrad, 96797 Alterac, 81900 Searing Gorge,
   93684 Swamp): none contracted anywhere (2990/96797 checked against
   their zones' contracts; 81900/93684 live in future/outside zones). The
   guide soft-pres the gated completes (2991 <- 2990, 81917 <- 81900) in
   dedicated `when onquest` mini-steps, and reports the ungateable
   accept-blocked records (96798 <- 96797, 93685 <- 93684) as structural
   warnings with the chain named. The orphan chain downstream of 96798
   (96811 <- 96798 <- 96811 <- 96799 <- 96812) is fully contracted, so it
   reads whole once the head is held.
6. No class gates, no race gates: verified — every contracted record
   carries classes null, and races are only Alliance or neutral.
