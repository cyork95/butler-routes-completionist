# Shen'dralas (Horde) revisit census (pack 0.137.0)

Revisit shape (not a full zone census): the Alliance census
(`docs/shendralas-census.md`) contracted 28 quests and set aside four
records as its "OUT (4) — Horde-gated pre chain". This round rules on
exactly that chain from current data, plus a full-pool sweep for
anything else Horde-fireable on the key. Source: local Forever game
data (questie-forever `quests.json`, `--product wowf` + QuestieDB).
Accept-zone key **2652** (Shen'dralas, inside Maraudon): 32 quest
records carry zone-field 2652 — all `races: null` (race-open). Zero
Horde-mask and zero Alliance-mask records exist on the key; the
faction gating here is entirely pre-chain, not mask.

## The four banked records (all IN)

- 93058 L42 Saving Our Own (min30, no pre... pre 93045 Test Your
  Theory — Horde-only, Desolace-Horde-contracted) — Nerlokh (placed
  2652 at 20.93, 22.68); no objectives (talk-through); ends at
  Nerlokh. Next: 93122.
- 93062 L42 Bone Burying (min30, pre 93045) — Nerlokh; no objectives;
  ends at Nerlokh. Next: 93122.
- 93122 L43 Checking Things Out (min35, pre 93058 + 93062, preAll the
  same) — Nerlokh; Investigate the Outcast Hideaway event (map-placed
  2652 at 34.85, 74.78); ends at Nerlokh. Next: 93128.
- 93128 L42 Khan Jehn (min35, pre 93122) — Nerlokh; no objectives;
  ends at Uthek the Wise (Desolace 1443 at 36.22, 79.25): expedition
  turn-in. No next (chain end).
Band from their own minLevels: **30–35** (m30 ×2 openers, m35 ×2
closers; own-levels run to 43 with minLevels in band — finales IN per
the minLevel rule; the main guide's 30–49 span is not copied).

## Full-pool sweep: Horde-fireable but Alliance-unfireable

- Horde-mask records on 2652: NONE (all 32 are null).
- Pres across all 2652 records that are Horde-only by mask: ONLY
  93058 → 93045 and 93062 → 93045 (both `pre` and `preAny` fields
  agree). No other 2652 record has a Horde-only pre.
- Conclusion: the banked four are the complete Horde-fireable set —
  "no others" is claimable after this sweep (not assumed).
- 93128's twin 93196 (Khan Jehn, pre 93188) lives in the Desolace
  (Alliance) contract — reachable there, untouched here; no twin
  conflict (verified, not assumed).

## Named-check rulings

- 93045 (Test Your Theory, zone 1443, Horde 8589934770, m30) is homed
  in `desolace-horde` (verified by ID — the census line calling it
  "uncontracted anywhere" is STALE, superseded). It is NOT
  re-contracted here: the mini points at its home (`when onquest
  93045`, tip names Uthek's Desolace accept), and its accept/turnin
  stay exactly as contracted there. The Desolace guide is not edited
  by this round.
- Chain fireability for Horde rests on pre-enforcement working as the
  data describes (93045 completable by Horde → 93058/93062 offered →
  93122 → 93128). The playtest section below reports the honest sim
  result; if the chain cannot fire even for Horde personas, the census
  does not stand in the way of that evidence.

## Item-start enumeration (explicit scan of all 2652)

Start items appear on ZERO records. Start objects appear on exactly
ONE: 92914 Strange Pylons (577959/577960 — shared, main-guide-
contracted, not duplicated). "No others" is claimable after this
scan.

## OUT list

Standing exclusions referenced, none banked: the Alliance contract
holds the other 28 (all null-mask shared); 93196 is Desolace's. No
repeatable/seasonal/broken records were found among the Horde-fireable
set (empty OUT beyond the standing references — stated, not silent).

## BORDERLINE (argued, none decided silently)

1. Accept-geography vs zone-field: all four accept at Nerlokh's placed
   2652 point (20.93, 22.68); no dual-spawn analogue is needed — the
   single spawn is in-zone and every accept is race-open.
2. 93045 contracted elsewhere while its dependents contract here: the
   standard cross-contract pre shape (Badlands-2284 / Hinterlands-1429
   / WPL-9015 precedent) — one dedicated `when onquest` mini bridges
   it; the Desolace guide is untouched.
3. 93122's pre is a same-contract pair (93058 + 93062, preAll) — no
   mini needed; turn-in-before-accept file order covers it (the
   Alliance guide's own chain-order dialect).
4. 93128's turnin rides a plain Desolace expedition step:
   its accept is NOT mini-gated (pre 93122 satisfied in-route), so no
   `when onquest <self>` gate is required — a plain turnin draws no
   "accepted earlier only in steps with when" warning (verified in
   lint: this exact shape produced zero such warnings).
5. Null-count objectives: none in the pool (all four IN records are
   talk-through or event-complete; no invented xN anywhere).
