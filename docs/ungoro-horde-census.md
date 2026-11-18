# Un'Goro Crater (Horde) census (game data, accept-zone key 1449)

Source: local game data (`--product wowf` + QuestieDB). Method mirrors the
Alliance census (`docs/ungoro-census.md`): a quest accepts on 1449 if a
start NPC, start object, or start-item dropper spawns on 1449; the `zone`
field is a cross-check only. Race mask 8589934770 = Horde-only,
4294967373 = Alliance-only, anything else (null included) = shared
(Duskwood ruling). Shared/neutral quests are NOT duplicated here — they
stay in the main guide's contract, which this round ungates.

## Pool

58 records have a placed accept point on 1449: **4 Horde-only** (4145,
4147, 4148, 98093), 3 Alliance-only (4141, 4142, 4144 — the Muigin chain,
contracted in the main guide), 51 shared-or-other. 7 further records
carry `zone: 1449` with no placed start point anywhere: 87494 + the 4
writs (contracted, shared), 94399 (Horde, broken — below), 95790
(Alliance, broken per the Alliance census).

## 8-vs-5 accounting

A full-mask scan finds exactly **5** Horde-mask records touching the
zone: the 4 placed above plus sourceless 94399. No Horde-mask record
hides in the repeatable, seasonal, broken, or above-band classes. The
checklist's 8 was a pre-census estimate; the census's named 5 stand.

## IN (3) — band 47-53

| ID | Title | lvl | min | Accept | Notes |
| 4145 | Larion and Muigin | 52 | 47 | Larion (45.54, 8.72) | bloodpetal kills placed |
| 4147 | Marvon's Workshop | 52 | 47 | Larion | pointer; turn-in Liv Rizzlefix, Ratchet expedition |
| 4148 | Bloodpetal Zapper | 53 | 47 | Larion (pre 4146, mini below) | sprout drops in-zone; turn-in Larion |

Band: the three contracted minLevels are all 47; own-levels run 52-53
on finales whose floor is in band. **Band 47-53**, stated plainly as
resting on three records.

## OUT

- 94399 (Ravasaur Provisions, Horde, min58): OUT broken. Full record has
  no start NPC/object/item, no end, no pre/next, and no objective
  source — nothing to anchor an accept or turn-in to. Same verdict as
  the Alliance census; the data has grown no anchor since. Appealable if
  better data surfaces.
- 98093 (Field to Clear, Horde, min18): OUT below-band + Barrens-zone
  content. Giver Sulhasa dual-spawns 1449 (21.2, 15.7) and 1451 (80,
  17), but `qzone: 1413` and min18 (29 below the band floor) both point
  away. Not in any pack contract — flagged for the Barrens (Horde)
  future, which may home it without touching this contract.
- Tanaris-owned Torwa legs stay Tanaris-owned (symmetric with the
  Alliance no-double-contract ruling): 351/648 OOX pair, 4289-4301,
  9051-9053.

## Item-start scan (explicit)

Pool scan finds two item-starts: 351 (OOX, Tanaris-owned) and 3884
(journal, Alliance-contracted). **Zero Horde-mask item-starts.** The
Larion chain is NPC-started throughout. Nothing asserted without the
scan.

## BORDERLINE (argued, none decided silently)

1. **4146 (Zapper Fuel, Horde, min47) — OUT, the load-bearing call.**
   Start Liv Rizzlefix (Ratchet, 1413-only spawn), end Larion (1449),
   pre 4147, next 4148, `qzone: 1413`. By the accept rule it is Barrens
   content and OUT here — same rule that homed Torwa to Tanaris, Kargath
   to the Badlands, and every capital accept to its city. It is
   uncontracted pack-wide (not in the 157 Barrens contract), so flagging
   it matters: the chain reads 4145 → 4147 → [4146 at Liv] → 4148, and
   4148's pre rides a `when onquest 4146` mini with the complete +
   turn-in, plus a note at Liv's turn-in sending the player to take
   4146. The route never wedges (mini hidden until onquest; 4148's
   accept carries the pre note, the main-guide 4144/4143 shape). Breaking
   the accept rule for chain-convenience would risk a double-contract
   the day the Barrens (Horde) future takes 4146. Appeal path: a Barrens
   (Horde) addendum can home 4146 without touching this contract.
2. **98093's 1449 spawn.** A dual-spawn giver with an in-zone point is
   normally in-zone accept geography — but min18 keeps it out of this
   contract regardless, and qzone 1413 names its zone. OUT on two
   independent grounds; the Barrens flag preserves it.
3. **Band on three records.** Floor and members coincide at min47; the
   top (53) is 4148's own level on an in-band floor, per the zone-finale
   rule. 94399 (min58) and 98093 (min18) are out on band plus their
   independent reasons above.

## Contract

`ungoro-horde`, order 70 (next free at commit time; 69 taken by Swamp of Sorrows (Horde)), band 47-53: **4145, 4147, 4148**.
