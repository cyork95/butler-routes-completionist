# Dustwallow Marsh (Horde) census (pack 0.114.0 base; Horde block)

Accept-zone key: **1445** (areaId 15, parent 1414 Kalimdor; key space
with Ashenvale 1440 / Thousand Needles 1441 / Stonetalon 1442 / Desolace
1443 / Moonglade 1450). **69** quest records carry zone=1445,
verified by counting quests.json; same key the Alliance census used.
Contested zone: the Alliance census keys on Alliance accepts; the 15
Horde records it set aside are reconciled below, every one of them by ID.

Method: every zone-1445 quest examined against the pack's inclusion
rules; the Alliance census's 15 banked Horde set-asides reconciled one
by one; a starter sweep over all quests (Horde-mask records with
1445-spawn NPC starters, item drops, or object starts touching 1445 but
zoned elsewhere) to catch Horde content beyond the 15; pres/exclusives/
object-sources resolved from data. Game data wins throughout. (Note: one
early read of docs/dustwallow-census.md in this session returned
corrupted content; every Alliance-census fact below was re-verified
against the live file before writing.)

## Band: 30–45

Derived from the Horde records, not copied from the Alliance band. The 15
Horde minLevels: 30×4 (1238, 1239, 1270, 1273 — the Brackenwall opener
cluster), 38×1, 48×5, 55×5. No Horde records exist below m30.
minLevel draws the line: floor **30** (the opener cluster), ceiling
**45** (the zone's finale scale). The L43 98192 (m38) is IN per the
minLevel rule as the zone finale. The L53 Ulka chain (m48) and the L60
Test of Skulls chain (m55) sit above the band and are OUT — argued
below; no band-stretching to fit them in. The highest contracted
minLevel is 38 (98192).

## IN (5)

| ID | Title | Lvl/min | Accept | Notes |
|----|-------|---------|--------|-------|
| 1238 | The Lost Report | 35/30 | — (object-start) | Loose Dirt 20985 placed on 1445 [55.44, 25.92]; ends Nazeer Bloodpike (1424+1445; 1445 pt [35.21, 30.66]); no objectives; next 1240 (Barrens — chain exit, handoff note, never contracted here) |
| 1239 | The Severed Head | 35/30 | — (object-start) | Same Loose Dirt object; pre 1238 (in-contract); ends Nazeer; no objectives |
| 1270 | Stinky's Escape | 37/30 | "Stinky" Ignatz (1445-only [46.88, 17.52]) | Horde version of the Alliance-contracted Stinky escort (same-title mirrors, enders diverge: Mebok vs Stern — faction split decides); event objective "Help Stinky find Bogbean Leaves" placed on 1445 [48.87, 24.58] — escort Stinky→Bogbean in-zone, expedition leg only for the Mebok turn-in; ender Mebok Mizzyrix on map 1413 [62.37, 37.62]; no pre |
| 1273 | Questioning Reethe | 37/30 | Ogron (1445 [40.96, 36.69]) | kill Paval Reethe 1445 [42.65, 38.07] + event "Question Reethe with Ogron" placed on 1445 [42.47, 38.07] (same compound — both objectives complete there); pre 1269 (Barrens object-start, outside) → soft-pre mini; ends Krog (1413+1445; 1445 pt [36.42, 31.88]) |
| 98192 | Skin Careful, Skin Sharp | 43/38 | Krak (1424+1445; 1445 pt [36.4, 30.85]) | 8 Intact Raptor Hides off Bloodfen Razormaw/Lashtail, in-zone [31-33, 64-66]; no pre; ends Krak |

No class, race, skill, event, or repeatable flags on any of the 5 — no
gates needed. No excl flags in the 5 (scanned). No same-name twins within
the 5.

Item/object-start scan over the 15 + sweep: exactly ONE in-zone
object-start pair (1238/1239's Loose Dirt 20985); zero item-starts.
The sweep found no Horde item-starts dropping on 1445 in any zone — "no
others" is claimed only after this scan. 1269's starter (Theramore Guard
Badge 21042, 1413 + 1445 [29.83, 48.24]) is zone-field 1413 → Barrens
pool per the Kristy rule; named in 1273's mini note, not contracted.

Spawn audit: every giver and ender referenced by the 5 spawns on map
1445 (dual-map NPCs are routed at their 1445 points; Mebok's 1413 point
rides the escort expedition). The only spawnless-adjacent record is
none — no 1046-pattern completes needed; 93680-analogs do not occur
here. Kill/objective points verified: Paval Reethe 1445, Razormaw/
Lashtail 1445, Dirt 20985 1445, vials n/a.

## OUT

Of the Horde 15, OUT above-band (10):
- 6582/6583/6584/6585/6601 Test of Skulls + Ascension (all L60/min55,
  Emberstrife 1445 [56.66, 87.72] start/ender): OUT above-band per the
  minLevel rule — same call as the Stonetalon (Horde) census's L60 Onyxia
  links 6568/6602 (min 55), and the Alliance census already names the
  m55 Test of Skulls as above the cluster. Skulls drop from Scryer/
  Somnus/Chronalis/Axtroz per objectives; the chain runs 6570 (1422,
  outside) → 6582 → 6583 → 6584 → 6585 → 6601 → 6602 (1442, the
  Stonetalon-OUT link, ends Rexxar on map 1443). Named in full so the
  call is transparent; no band-stretch to fit them in.
- 95284/95285/95309/96332/96334 Sergeant Ulka chain (all L53/min48,
  Nazeer → Ulka [70.3, 18.85] → Ulka → Ulka/Masoj-ends; 96334 ends
  Eitrigg on map 1454; 95309 has no ender, next 95454 zone-None):
  OUT above-band per the minLevel rule — same call as the Alliance
  census's m48 Sully-chain OUT. Ulka's 1445 point and the bandana
  droppers (Alcaz/Defias mobs) are logged with the exclusion; the chain
  exits to uncontracted 95454/96369, named not routed.

Not duplicated here (main-guide contracts; Duskwood ruling: null-mask is
shared, not Horde — all 24 already contracted in the Alliance
`dustwallow` guide): 1203, 1206, 1218, 1288, 1948, 1949, 1952, 1954,
1955, 1956, 1957, 1958, 2846, 4961, 4976, 6607, 94258, 94270, 94282,
94294, 94306, 98205, 98215, 98231.

Alliance-only zone-1445 quests (set aside for the record): the 6
above-band Alliance-mask records (95196, 95198, 95262, 95263, 95264,
96381 — Sully→Shaw chain + Wet Work, min48), 8227 (min58 object-start),
81570 (bare no-objective twin of 1203, repeatable-style — the
chain-consistent 1203 is contracted Alliance-side), 98166 (Human-only
mount, no objectives — Loch Modan mount precedent). The 21
Alliance-mask Alliance-IN records are untouched, not listed.

Belongs elsewhere (sweep dispositions, flagged not contracted):
- 7321 Soothing Turtle Bisque: zone field 1416, accept npc 2393
  Christoph Jeffcoat (1416 [61.1, 80.7] + 1424 [62.29, 19.04]) — NOT a
  1445 accept by the Kristy rule (starter not only on 1445, zone field
  wins) — plus a Cooking-skill (185) record and Horde twin of the
  Alliance 555. Ruled OUT of this contract by ID as instructed; belongs
  to the Alterac (1416) pool, which picks it up with the 1424 point
  logged here.
- 1391 Nothing But The Truth: zone 1431, already contracted in
  `duskwood-horde` (verified in the contracts file) — turns in at
  Marksen (map 1435, ender record), not Dustwallow content, never
  duplicated.
- Barrens-pool chains with 1445-placed givers (zone-field 1413 wins,
  starters not only on 1445): Nazeer Bloodpike's 1201/1202 Theramore
  lines + 1240 Troll Witchdoctor (1239's next — the named chain exit) +
  1262 Report to Zor; Krog's 1276/1321/1322/1323 Black Shield links;
  Mok'Morokk/Draz'Zilb/Tharg Onyxia brood chain (1166-1173); Lydon
  elixir chain (496-524); 1269 Paval Reethe (1273's soft-pre key;
  object-start badge on 1413 + 1445); 857 Tear of the Moons; 1168-1170
  brood chain; 2934/2935/2938 venom chain; 1066/1067; 2938/1361/2480;
  Feegly 3421; Voggah 7142/8272; Bath'rah 8411-8413 shaman chain;
  79361/79364 (1441 Thousand Needles). None contracted here; the
  soft-pre minis name the two this route needs (1269 for 1273).
- Repeatable/seasonal: 6701 Syndicate Emblems (repeatable, neutral).
- 95454 (zone-None, pre 95309, no givers): 95309's chain exit,
  uncontracted anywhere; named, not routed. 6602 likewise (1442,
  Stonetalon-OUT link).

Candidates examined: 69 zone-1445 records + the starter sweep (all
Horde-mask 1445 touches zoned elsewhere). IN (Horde contract) 5, OUT of
the Horde 15 above-band 10, Alliance-only 9 named above, neutral-
not-duplicated 24, belongs-elsewhere dispositions as listed, each with
its reason.

## BORDERLINE (argued openly; nothing borderline is decided silently)

(a) Band 30–45 vs the Alliance 35–45: derived, not copied. Floor 30 is
the Brackenwall opener cluster (four m30 records: 1238/1239/1270/1273)
with no Horde content below it anywhere in the dumps; ceiling 45 holds
the zone's finale scale with the L43 98192 IN per the minLevel rule.
The Alliance band's higher floor reflects their 28–40 cluster with
below-band grey accepts; the Horde pool has no below-band records, so
floor == lowest minLevel. Both bands agree on the ceiling and on
cutting m48/m55/m58.
(b) Test of Skulls OUT (6582/6583/6584/6585/6601, min 55): the
Stonetalon (Horde) precedent rules L60 Onyxia links with min 55 OUT
above-band (6568/6602), and the Alliance census already places the m55
Test of Skulls above its cluster. Contracting these would require
stretching the ceiling from 45 to 55 for five quests whose chain head
(6570, 1422) and finale ender (Rexxar, 1443) both sit outside the zone
— the band rule says no. OUT with the full chain named.
(c) Ulka chain OUT (95284/95285/95309/96332/96334, min 48): same move
as the Alliance census's m48 Sully-chain OUT. The chain's L53 finale
scale and its exits (95454 zone-None, Eitrigg on the Orgrimmar map, Ulka
as a self-contained hub) all sit outside the band; minLevel draws the
line.
(d) 1270's cross-key ender: the quest accepts in-zone (Stinky is
1445-only), so it is ours; the Bogbean event is placed in-zone (1445
[48.87, 24.58]) so the escort runs Stinky→Bogbean on the map, and only
the Mebok turn-in (1413 [62.37, 37.62]) rides an expedition leg.
Accept-based contracting cuts the other way too — the twin 1222 stays
Alliance-side on its Stern ender.
(e) 1273's pre 1269: an out-of-contract Barrens object-start whose
badge also sits on 1445 [29.83, 48.24] — the Kristy rule still assigns
the quest to zone 1413 (starter not only on 1445), so 1273's completes
(kill at [42.65, 38.07], questioning placed at [42.47, 38.07]) ride a
`when onquest 1269` mini, never inline.
(f) 96334's bandana item (274028, Alcaz/Defias droppers): logged with
the m48 OUT, not sourced in-guide — above-band records get reasons,
not routes.
(g) 6601's Rexxar ender on map 1443 and 6602's 1442 zone: confirm the
chain was already routed out (Stonetalon round) — consistent, no
double-contract.
