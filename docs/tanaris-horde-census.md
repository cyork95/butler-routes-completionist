# Tanaris (Horde) census (game data, accept-zone key 1446)

Accept-zone key: **1446** (verified by count: 162 quest records carry
`zone=1446` in this data build - the same key and the same count the
Alliance census (`docs/tanaris-census.md`) examined). Race masks in the
data: 8589934770 = Horde, 4294967373 = Alliance, null = neutral (both
factions).

Method: every zone-1446 record examined against the packs inclusion
rules; the Alliance censuss 10 banked Horde set-asides reconciled one by
one against the Horde-mask pool; start-item AND start-object scan run over
the Horde pool; pres/exclusives and outside legs resolved from data
(`npcs.json`, `objects.json`, `items.json`, `quests.json`, `spawnz.json`
cross-checked).

Pool breakdown: 10 Horde-mask + 81 Alliance-mask + 71 null. The 10
banked set-asides are exactly the 10 Horde-mask zone-1446 records
(verified programmatically - no more, no fewer). Zero Horde-mask records
sit inside the Alliance `tanaris` contract (91 quests), so the
exclusive-contracts precedent holds with no directional check needed.

## Band: 38-50

minLevel histogram of the 10 Horde records: m38 x4 (379, 654, 841, 864),
m39 x1 (32), m40 x1 (97534), m45 x1 (2967), m50 x1 (4509), m55 x1 (5802),
m58 x1 (8978). The zone bulk is the m38 Bilgewhizzle chain cluster; the
m39 Fizzledowser report, the m40 Quinn job, and the m45 Stone Watcher
return ride the same combat range; the top is the m50 silithid-chain
finale 4509 (the Horde mirror of contracted 4508). m55+ is out: 5802
(min55, Fire Plume Ridge key mold) and 8978 (min58, ectoplasm-chain
return). Derived from the Horde histogram, not copied from the Alliance
38-50 - the edges coincide because both factions work the same hubs.

Contracted levels run 45 (97534) to 54 (4509); 4509s own level exceeds
the band top but its minLevel is in band - IN per the band rule as the
chain finale. No race header for the guide: no contracted quest is
locked to a single Horde race. No class gates, no profession gates, no
skill-gated records (the pool scan found no CLASS or SKILL flags on any
Horde record). No dungeon turn-in: every contracted turn-in sits in the
open world or a capital (capital legs ride honest expeditions below).

Reconciliation of the Alliance censuss banked set-asides: 7 IN, 3 OUT
(841 repeatable; 5802/8978 above-band - each ruled below).

Item-start enumeration (explicit start-item AND start-object scan over
the Horde pool): item-started Horde records are 654 (item 8524, Model
4711-FTZ Power Source - no mob, object, or vendor source anywhere in the
data: sourceless, ships with a bag note) and 2967 (object 142343, Uldum
Pedestal, single in-zone point - the 94895 object-start precedent).
**Exactly two Horde item/object-starts.** The 654 objectives add three
more sourceless items (9440/9441/9438 Acceptable Samples - no source
anywhere) plus the kit 8523 (buyable: Alessandro Luca 7683, Horde
vendor, Undercity) - all named in the guide with honest notes, never
invented sources. 97534s objective item 278191 (Desert Debris) names a
single object source 666694 that carries no spawn record anywhere -
phantom, treated as sourceless with the same honest note.

## IN (7)

Gadgetzan hub (Bilgewhizzle 7407 @52.46,28.51; Fizzledowser 7724
@50.21,27.48; Pestlezugg 5594 @50.89,26.96; Quinn 11756 @51.12,27.88 -
one tight hub):

| 379 Slake That Thirst | 46/38 | pre 243 (Undercity-accept, outside - soft-pre mini below) | 5 Wastewander Water Pouches 8483 off the Wastewander family (Rogue 5615 50%, Thief 5616 52%, Shadow Mage 5617 53%, Bandit 5618 52%, Assassin 5623 50%, all east camps 58-60, 22-40) -> Bilgewhizzle |
| `when onquest 243` soft-pre mini at Bilgewhizzle (turn in 243, accept 379) - the pre ends in-zone at the chains head (Kadrak pattern) |
| 654 Tanaris Field Sampling | 46/38 | pre 379 (IN) | ITEM-START 8524 (sourceless - bag note: have the Model in bags, R2 class); objectives 8 x basilisk/hyena/scorpid samples 9440/9441/9438 (all sourceless - no collect lines; honest note, R5 class) + return kit 8523 (buy: Alessandro Luca 7683, Undercity - rides the 864 expedition below); ends Bilgewhizzle; next 864 |
| 864 Return to Apothecary Zinge | 46/38 | pre 654 (IN) | no objectives; ends Zinge 5204, Undercity (1458 @50.14,67.97) - capital expedition turn-in |
| 32 Rise of the Silithid | 48/39 | pre 113 (shared, contracted in the MAIN guide - the ungated guide serves it to Horde; chain note, no mini - the 93045 pattern) | no objectives; ends Zilzibin Drumlore 7010, Orgrimmar (1454 @56.26,46.68) - capital expedition turn-in |
| 4509 Calm Before the Storm | 54/50 | pre 4507 (shared, contracted in the MAIN guide - chain note, no mini); own level exceeds band, minLevel in band - IN per the band rule as the chain finale (mirror of contracted 4508) | no objectives; ends Zilzibin 7010, Orgrimmar - same expedition leg as 32 |
| 97534 Gritty Business | 45/40 | no pre; excl [97536] (mutual - 97536 lists 97534 back; the twin is Alliance-only and unroutable for Horde, so no in-guide gate is needed) | 7 Desert Debris 278191 (phantom object source - honest note, no collect lines, R5 class) -> Quinn; the Horde twin of main-contracted 97536, each faction carrying its own twin |

Uldum Pedestal, the south-west (object 142343 @37.63,81.40, single in-zone point):

| 2967 Return to Thunder Bluff | 50/45 | pre 2954 (shared, contracted in the MAIN guide - chain note, no mini); OBJECT-START 142343 (the 94895 precedent) | no objectives; ends Nara Wildmane 5770, Thunder Bluff (1456 @75.65,31.61) - capital expedition turn-in |

## OUT (3)

- Repeatable (1): 841 Another Power Source? (rep=True) - OUT by rule. Its one-way excl of 654 ([654] with no mirror) is consistent with the repeatable-farm-variant reading: the one-time chain record is 654 (which unlocks 864), the repeatable is not contracted. No twin confusion in the guide (named, not routed).
- Above-band (2): 5802 Fire Plume Forged (L57/m55; accepts in-zone at Krinkle Goodsteel 5411 - ruled OUT on its OWN minLevel, not on 5801s; pre 5514 outside-uncontracted, ender 11057 EPL-side, chain dead either way); 8978 Return to Mokvar (L60/m58; accepts in-zone at Mux Manascrambler 16014; pre 8928 uncontracted in-zone ectoplasm chain, ender Mokvar 16012 in Orgrimmar - the Horde-side ectoplasm return, out of reach either way).

Alliance-only zone-1446 records (set aside for the record - none duplicated here): per the Alliance census, 81 Alliance-mask records sit in-zone; the contracted ones ride the main guide (being ungated this round), the rest are record-only. Null-mask shared records stay in the main guide by the Riverglades precedent (no duplication).

Gadgetzan city rule: Gadgetzan sits on Tanariss own map (1446) - zone content per the Ratchet precedent, not city content. All four hub givers spawn in-zone.

## BORDERLINE (all decided, none silent)

(a) 841 vs 654: decided by the rep flag, not silently. 841 carries rep=True (repeatable) while 654 carries none; the pack contracts the one-time record and excludes the repeatable (the 1707/1878 same-title precedent). The asymmetric excl (841 lists 654, no mirror) fits the farm-variant reading and is recorded as supporting evidence, not as the decision itself. 654 unlocks 864, so the chain-consistent record is also the contracted one - no tension remains.
(b) 4509 (L54/m50): own level exceeds the band top; minLevel 50 is in band - IN per the band rule as the chain finale, the Horde mirror of contracted 4508. If a future build moves the band top below 50, this contract shrinks by one with no other change.
(c) 2967: object-start (Uldum Pedestal, in-zone single point) with a main-contracted pre (2954) - IN per the 94895 object-start precedent, with a chain note instead of a mini (the 93045 pattern: the main guide serves 2954 to Horde players). If 2954 ever leaves the main contract, 2967 needs a soft-pre mini of its own.
(d) 97534 gating: no `only` gate on any line. The excl twin 97536 is Alliance-mask and unroutable for Horde, so the exclusion never fires for a Horde player; mutual excl confirmed both ways in the data. If a future build drops the masks, the twin pair needs joint gates then.
(e) Band top 50 on a single m50 member: derived from the Horde histogram (bulk m38-45 + finale m50 + m55+ out), not copied from the Alliance 38-50. The edges coincide; the reasoning does not.
(f) 654s kit (8523, Undercity Horde vendor): the guide buys it on the same Undercity leg that turns in 864 and accepts 243 - one expedition serving three chain needs, said plainly. The sourceless items (8524/9440/9441/9438/278191) ship as bag/measurement notes with no collect lines and no invented sources (the 8411-reagent pattern); the sim residue is argued in the round report.

