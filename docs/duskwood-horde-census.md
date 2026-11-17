# Duskwood census (Horde route)

Accept-zone key: **1431** (verified by count: 100 records carry zone 1431
in the local data dumps — the same key the Alliance census used; plus a
spawn-pull that found exactly one more record, 3861, ruled OUT below).

The Alliance census (`docs/duskwood-census.md`) examined 102 candidates on
this key and contracted 93 at band 17–28. This census reconciles every
record against that contract. Standing rule (Ashenvale precedent):
shared-mask records already contracted by the Alliance guide are NOT
duplicated here; the ungating of `duskwood.guide` (same round, Part 3) makes
them visible to Horde players as shared lines.

## Candidate pool: 100 zone-field records + 1 spawn-pull

Mask census of the 100 (key `races` in `quests.json`):

- Horde mask 8589934770: **5** — 1372, 1383, 1388, 1391 (Nothing But The
  Truth chain), 94241 (Horde writ). All five were the Alliance census's
  banked Horde set-asides. All five land IN.
- Null mask: **23** — the 18 Missions (81730–81747), the 4 Alliance writs
  (94214, 94223, 94232, 94250), twin 98372. Every one is already routed in
  the Alliance guide. See the null-mask ruling below — none duplicated.
- Alliance mask 4294967373: **70** — 67 already routed in the Alliance
  guide (including twin 99267), plus 1395, 171, 990 (OUT everywhere, with
  reasons below).
- Mask 77 (Alliance races): **2** — 236, 245, both routed in the Alliance
  guide, not duplicated.
- Spawn-pull (start-NPC spawns on 1431, zone field elsewhere): **1** — 3861
  (zone 1436, repeatable, OUT).

## The Horde contract: 5 quests, band 37–42 (+ L60 special)

| ID | Title | Lvl | min | Accept | Turn-in | Objectives |
|----|-------|-----|-----|--------|---------|------------|
| 1372 | Nothing But The Truth | 42 | 37 | Deathstalker Zraedus 5418 (H, in-zone 87.81,35.63) | Apothecary Faustin 5414 (H, in-zone 87.45,35.25) | none (talk) |
| 1383 | Nothing But The Truth | 42 | 37 | Faustin 5414 (pre 1372) | Faustin 5414 | 5x Shadow Panther Heart 6080, 1x Mire Lord Fungus 6081, 1x Deepstrider Tumor 6082 — ALL droppers out-of-zone (see expeditions) |
| 1388 | Nothing But The Truth | 42 | 37 | Faustin 5414 (pre 1383) | Zraedus 5418 | none (talk) |
| 1391 | Nothing But The Truth | 42 | 37 | Zraedus 5418 (pre 1388) | Infiltrator Marksen 5416 (neutral AH, NO 1431 spawn — spawns only on key 1435 Swamp of Sorrows, 44.29,52.43) | none (talk) |
| 94241 | Craftsman's Writ: Dark Leather Tunic | 60 | 1 | item 264041, sourceless (no vendors, no droppers — R2 bag note) | Kzixx 3134 (neutral AH, in-zone 81.82,19.77) | writ itself + craft Dark Leather Tunic 2317 (R5 craft residue; optional + when skill Leatherworking 1, Alliance-writ handling) |

Band: minLevels 37 (chain) run the band **37–42**; the chain's L42 sits at
the top as the finale (Ashenvale rule — minLevel draws the line, and all
four minLevels are in band). 94241 rides as the L60 special class
(minLevel 1, same writ-pattern shape as the Alliance census's four writs
plus twins) — noted separately, not band-setting. The band deliberately
stretches above the Alliance 17–28: the chain's minLevel 37 demands it.
That is expected, not an error.

Expeditions (accept rule — chains starting here are IN wherever they go):

- 1383's three objective items drop nowhere in Duskwood. 6080 drops off
  Shadow Panther 768 (35%, spawns only on key 1435 Swamp of Sorrows, 24
  points) — 229984 Siopi has no spawn in any zone and ships nothing.
  6081 drops off Mire Lord 1081 (100%, only on 1435 at 5.5,31.38). 6082
  drops off Deepstrider Giant 4686 (100%, only on key 1443 Desolace at
  66.26,32.79) and Deepstrider Searcher 4687 (100%, only on 1443 at
  32.07,24.66). The guide routes Swamp of Sorrows + Desolace expedition
  legs with travel steps from the data.
- 1391 turns in at Marksen on key 1435 (44.29,52.43) — a Swamp of Sorrows
  expedition leg.

## Reconciliation of the five banked set-asides

- 1372, 1383, 1388, 1391 (Nothing But The Truth, L42/m37, H-mask): all four
  IN, chain order preserved. Pres are chain-internal (1372 → 1383 → 1388 →
  1391), so no out-of-contract soft-pre minis are needed.
- 94241 (Horde writ, L60/m1, H-mask, writ-class exception like Stonetalon's
  94216): IN as the L60 special, optional + when skill Leatherworking 1
  with the Alliance-writ bag-note shape.

## Null-mask ruling (explicit, per the brief)

Null ≠ Horde (Alliance census borderline (b): 98372's null mask "matches
the writ pattern, not the Horde mask"). All 23 null records are already
routed in the Alliance guide — 18 Missions, 4 writs, twin 98372 — and after
this round's ungating their lines carry no faction gate, so Horde players
see them as shared content. Duplicating them here would double-contract
shared quests. Twin 99267 (Alliance mask) stays Alliance-side; null twin
98372 stays where the Alliance guide routed it.

## Item-start scan (explicit — Mulgore lesson)

Six item-starts exist among the 100: the five writs (94214/94223/94232/
94241/94250, starters 264014–264050, all sourceless) and 96138 Merrick's
Bow (Alliance, starter 281142 off Lost Watchers — Alliance-contracted, not
duplicated). The Horde contract's only item-start is 94241: sourceless
writ, R2 bag-note handling, never wedged. No other in-band Horde
item-start exists on this key.

## OUT ledger (nothing disappears silently)

- Already contracted in the Alliance guide, not duplicated: 92 (67
  Alliance-mask incl. twin 99267, 2 mask-77, 18 Missions, 4 writs, null
  twin 98372) + 78147 Crimes Against Anatomy (zone 1458 cross-faction
  record, Alliance-contracted) = 93 reconciled.
- Above-band: 1395 (L45/min40, Nethergarde chain to Blasted Lands — the
  Alliance census's call stands).
- Accepts outside the zone: 171 (Stormwind orphan accept), 990 (Darkshore
  accept, the Ashenvale handoff — home guides own both).
- Repeatable: 3861 CLUCK! (repeatable=true; spawn-pull only; the Alliance
  census's homeless flag stands — not contracted anywhere).
- Broken/phantom: none found in the Horde-mask set. Siopi 229984 (no spawn
  anywhere) is a dead dropper reference inside 1383's table, not a quest
  record — disclosed, not shipped as a source.

## BORDERLINE

(a) The whole Horde route executes mostly out-of-zone (1383's objectives,
1391's turn-in). Contracted anyway: the accept rule governs (accepts are
on 1431), and expeditions are the pack's standing pattern for chains that
start here and end elsewhere.
(b) Band 37–42 for a 5-quest contract with a single hub pair (Zraedus/
Faustin at 87,35) plus Kzixx: small contract, correct outcome — no
padding (Deadwind precedent).
(c) 94241's `when skill Leatherworking 1` gate mirrors the Alliance writs'
`when skill <Profession> 1` shape; the quest record itself carries no
skill field. Stated, not silent.
(d) No soft-pre minis: every pre of every contracted quest is itself
contracted (chain-internal). Nothing to mini.
