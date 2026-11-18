# Felwood (Horde) census (game data, accept-zone key 1448)

Accept-zone key: **1448** (verified by count: 106 quest records carry
`zone=1448` in this data build - the same key the Alliance census
(`docs/felwood-census.md`) used, which counted 162 records in its older
build; the key is stable, the record count drifted with the build, and
the data wins).

Method: every zone-1448 record examined against the packs inclusion
rules; the Alliance censuss banked Horde set-asides reconciled by count
against the Horde-mask pool (the individual IDs do not survive in that
doc - the Mulgore/Thunder Bluff precedent: the count is the target, the
enumeration comes from the data); start-item AND start-object scan run
over the Horde pool; pres/exclusives and outside legs resolved from data
(`npcs.json`, `objects.json`, `items.json`, `quests.json`, `spawnz.json`
cross-checked).

Pool breakdown: 13 Horde-mask + 29 Alliance-mask + 64 null. The 13
Horde-mask zone-1448 records are: 4102, 4108, 4109, 4110, 4111, 4112,
5887, 5888, 5889, 5890, 5891, 8485, 86612. Zero Horde-mask records sit
inside the Alliance `felwood` contract (59 quests), so the
exclusive-contracts precedent holds with no directional check needed.

## Band: 45-48

Contracted minLevels run 45 (8485, the Gorn finale) through 48 (the
bulk: 4102, 5887-5891, 86612). Nothing sits between 48 and 55; m55+ is
OUT (see below). Derived from the Horde histogram, not copied from the
Alliance 45-55 - the edges coincide at the bottom because both factions
work the same floor. The L55-60 own levels ride the band rule (minLevel
in band = IN).

No race header for the guide: no contracted quest is locked to a single
Horde race. No class gates (the pool scan found no CLASS flags on any
Horde record). Profession gates: Mining 186 (5888), Herbalism 182
(5889), Skinning 393 (5890), Enchanting 333 (5891) - `optional` and
gated `when skill <Profession> 1` per the settled handling. One
dungeon-adjacent note: none - every contracted turn-in sits in the open
world or a capital (capital legs ride honest expeditions below).

Reconciliation of the Alliance censuss banked set-asides: the doc banks
21 by count with no surviving IDs. This build holds 13 Horde-mask
zone-1448 records (all 13 accounted for below: 8 IN / 5 OUT) plus 8
Horde records that START in-zone but carry other zone keys - 4505/4506/
4521/4721/4741/4883/6162 (zone 1439 Darkshore, uncontracted anywhere)
and 6482 (zone 1440 Ashenvale, contracted in ashenvale-horde). 13 + 7 +
1 = 21. The arithmetic matches the banked count exactly, which argues
these 8 records sat on key 1448 in the Alliance build and were re-zoned
since (their givers keep real Felwood spawn points alongside the zoned
ones). Either way the data wins: zone-key discipline governs (the
Riverglades precedent - no cross-zone duplication), so the 8 stay homed
to the Darkshore (Horde) and Ashenvale (Horde, already contracted)
rounds, and this contract holds exactly the 13 in-zone records.

Item-start enumeration (explicit start-item AND start-object scan over
the Horde pool): the ONLY Horde item/object-start is 86612
(object 661778 Statue of Malorne, in-zone single point - the 94895
object-start precedent). No item-started Horde records. The salve
feeders need farmed/dug/grown/skinned/disenchanted reagents (see per-
quest notes); two of the five name no source anywhere (11512 Tainted
Skin, 11174 Nether Essence - both flagged `questItem` with empty drop
tables) and ship with honest bag notes, never invented sources.

## IN (8)

Maybess hub (Maybess Riverbreeze 9529 @46.75,83.13, south):

| 4102 Cleansing Felwood | 55/48 | no pre | 15 Blood Amber 11503 off the Warpwood family (Moss Flayer 7100 100% x18 pts, Shredder 7101 100% x11 pts, Dessecus 7104 100% single @57.76,22.33, east ~54-57,15-22) -> Maybess; the Alliance mirror 4101 (same name, Alliance-only, excl [] both - faction variants, no tension) rides the main guide |
| 5887 Salve via Hunting | 55/48 | pre 4102 (IN) | 6 Corrupted Soul Shards 11515 off the ooze/owl/satyr family (Cursed Ooze 7086 4.6% x24, Tainted Ooze 7092 10.6% x24, Vile Ooze 7093 29.7% x9, Ironbeak Owl 7097 23.8% x14, Screecher 7098 10.1% x13, Hunter 7099 14.5% x19, Jadefire Satyr 7105 21% x24, plus Warpwood/Shredder/Dessecus shares) -> Maybess; the Alliance mirror 5882 rides the main guide; next 4108 repeatable (noted, out of scope) |
| 5888 Salve via Mining | 55/48 | pre 4102 (IN); skill Mining 186, optional + gated | 4 Tainted Vitriol 11513 from Small Thorium Vein 324 (2 Felwood pts [34.69,61.76] + [47.84,14.2]) -> Maybess; mirror 5883 rides the main guide; next 4109 repeatable (noted) |
| 5889 Salve via Gathering | 55/48 | pre 4102 (IN); skill Herbalism 182 (skill id 182), optional + gated | 4 Fel Creep 11514 off Arthas Tears 142141 (21 Felwood pts, e.g. [37.26,61.42]) -> Maybess; mirror 5884 rides the main guide; next 4110 repeatable (noted) |
| 5890 Salve via Skinning | 55/48 | pre 4102 (IN); skill Skinning 393, optional + gated | 5 Patch of Tainted Skin 11512 - questItem with NO source anywhere in the data (bag note, same handling as the main guides skinning line); mirror 5885 rides the main guide; next 4111 repeatable (noted) |
| 5891 Salve via Disenchanting | 55/48 | pre 4102 (IN); skill Enchanting 333, optional + gated | 1 Lesser Nether Essence 11174 - questItem with NO source anywhere in the data (bag note, same handling as the main guides disenchanting line); mirror 5886 rides the main guide; next 4112 repeatable (noted) |

Gorn legs (Gorn One Eye 11555 @65.18,2.68, far north):

| 8485 The Brokering of Peace | 60/45 | pre 8481 (shared, contracted in the MAIN guide - chain note, no mini; the 93045 pattern); own level exceeds the band, minLevel in band - IN per the band rule | no objectives; ends Thrall 4949, Orgrimmar (1454 @31.73,37.82) - capital expedition turn-in; the Alliance mirror 8484 (Alliance-only ender Magni) rides the main guide |

Statue leg (object 661778 Statue of Malorne @42.03,47.36, center):

| 86612 Stag Lords Bauble | 55/48 | no pre; OBJECT-START 661778 (in-zone single point) | no objectives; ends Winna Hazzard 9996, Bloodvenom Post (Felwood point @34.21,52.34) -> Winna; the Alliance twin 86611 (same object family, Alliance-contracted) stays untouched in the main guide - the standard faction-twin shape, not a duplication |

## OUT (5)

- Repeatables (5): 4108 Salve via Hunting, 4109 Salve via Mining, 4110 Salve via Gathering, 4111 Salve via Skinning, 4112 Salve via Disenchanting (all rep=True) - OUT by rule. Their one-time feeders 5887-5891 are contracted above and name them as noted out-of-scope nexts (the 4103-4107 handling in the Alliance round).

Alliance-only zone-1448 records (set aside for the record - none duplicated here): the Alliance contract holds the Alliance side (incl. the 4101/5882-5886 one-time chain and the 86611 twin); the null-mask shared records stay in the main guides contract, which this round ungates. Horde-side Timbermaw content: none exists (the Timbermaw quests 6131/8460/8461/8462/8464/8465 are all null-mask shared, homed in the main guide - noted, not duplicated).

## BORDERLINE (all decided, none silent)

(a) Banked 21 vs found 13: decided by the zone key, not the count. The 8-record delta is fully itemized above (7 Darkshore-zone + 1 Ashenvale-zone, the latter already contracted); the 13+8 partition reproduces the banked 21 exactly, which supports the re-zoning reading but the ruling does not depend on it - even without a history, zone-key discipline keeps cross-zone records out of this contract. If a future build re-zones any of the 8 back to 1448, this census gets an addendum round.
(b) Same-name faction variants (4102/4101, 5887-5891/5882-5886): both sides contracted, no tension - excl [] both ways, and each sides pres/nexts stay inside its own faction (4102 has no pre; 5887-5891 pre 4102; Horde repeatables follow). Not the exclusive-twin shape (97534/97536); closer to the Timbermaw twin handling (6131/8460), but cleaner - faction masks already separate them.
(c) 8485s pre 8481 (shared, main-contracted): chain note, no mini. The Horde player serves 8481 through the ungated main guide first; 8485s accept carries the note. If 8481 ever leaves the main contract, 8485 needs a soft-pre mini of its own (the mini would turn in 8481 - verify the ender then).
(d) Band 45-48: derived from the Horde histogram (bulk m48, floor m45, nothing 49-54, m55+ out) - not copied from the Alliance 45-55. A 3-wide band is what the data draws; no exceptions are needed beyond the band rules own L60 clause (8485).
(e) 86612/86611: same object family, different IDs (different objects - 661778 vs Alliance twin object), each factions own pre-less object-start. No shared lines, no duplication.
(f) 5890/5891 keep their skill gates despite sourceless objectives: the SKILL requirement is real data (the gate is honest), the ITEM source is missing (the bag note is honest). Dropping the gate would misstate the quest; inventing a source would misstate the data.

