# Wetlands (Horde) census — accept-zone key 1437

Date: 2026-11-18. Data: local `upstream-polestar/data/forever`
(`--product wowf` + QuestieDB). Game data wins over brief and community
sources. Method: every record with `zone == 1437`, classified by races
mask (Horde-only 8589934770, Alliance-only 4294967373, else shared;
null-mask records are shared — the Duskwood ruling).

## Pool

90 records carry `zone == 1437`: **84 Alliance-only**, **5 null-mask**,
**1 mask-1** (97171, ruled below), **0 Horde-only by zone field**.

The 5 null-mask records are the Craftsman's Writ item-starts 94219,
94228, 94237, 94246, 94255 — all already contracted in the main
`wetlands` guide. Shared content stays there (Riverglades precedent);
none duplicate here.

The Alliance census (`docs/wetlands-census.md`, OUT ledger) banked
exactly **1 Horde set-aside**: 95682 Open the Maw. Reconciled below —
the pool holds nothing else Horde.

## IN (1) — band 24-31

**95682 Open the Maw** (Horde-only mask 8589934770; level 31,
minLevel 24). The quest record carries `zone: None`, but its accept
NPC — Deathstalker Agent 13155 — spawns at exactly one point in the
data: key 1437 (51.41, 59.23). Single-spawn giver on 1437 is in-zone
accept geography (the dual-spawn/city-rule test applied in reverse):
IN. Band: single record, min24 in the Alliance 20-30 band, own level
31 one above via the zone-finale rule — **24-31**.

- Accept: Deathstalker Agent 13155, Wetlands (51.41, 59.23). The
  Alliance census called this an "object starter"; the record shows
  `start.npc = [13155]`, no object — NPC start, data wins.
- Objectives: 2x Dragonmaw Saboteur (275045) + 4x Dragonmaw Warder
  (275044) kills, 1x Dragonmaw Dispatch (284844, drops from Dragonmaw
  Thaumaturgist 275046). All three source NPCs have **empty spawn
  tables** — no data-placed source anywhere. The micro-guide carries
  no invented coordinates; the objectives ride as a prose note.
- Turn-in: the same Deathstalker Agent (single 1437 spawn). The brief
  expected an Undercity expedition leg; the record shows
  `end.npc = [13155]` — fully in-zone, data wins, no expedition.
- Chain: `pre = [95663]` (Dragonmaw Rumors, Horde, Arathi accept at
  Zaruk 2787 [74.54, 35.64] on key 1417). 95663 IS contracted in
  `arathi-horde`, whose guide already routes its turn-in at the same
  agent (arathi-horde.guide line 146, @51.41,59.23). The chain reads
  whole across the two guides; the micro-guide notes the premise, no
  double-contract.

## OUT

- **97171** (mask 1, level 40, minLevel 40): hollow record — no name,
  no start, no end, no pre, no objectives. OUT broken (no anchorable
  accept or turn-in) AND above-band (min40 > 31). The mask-1 bit reads
  as a single-race bit (Human, per the contracted 6281 precedent in
  Westfall — mask 1 rides on 23 contracted records pack-wide, so it is
  not itself a broken signal), but the record is unroutable on its own
  facts either way.
- The 84 Alliance-only records: set aside for the record (the main
  guide's contract; this round ungates it). Not listed by ID here —
  the main census and contract own that ledger.
- Item-start scan over the 1437 pool: 6 records (94219/94228/94237/
  94246/94255 shared writs, 95810 Alliance-only) — all contracted in
  the main guide. **Zero Horde-mask item-starts.** 95682 is
  NPC-started. No "absence without scan" — the scan ran.

## BORDERLINE

(a) 95682's `zone: None` vs in-zone accept: the quest table's zone
field is empty, but the accept test is geographic — its only giver
spawn in the data sits on key 1437, and the pack already plays this
exact agent as a Wetlands point (arathi-horde's 95663 turn-in leg).
Contracted on the geography, argued here, not silent.
(b) Unplaced objectives (275044/275045/275046): shipped as a note,
never as invented points. Lint/playtest residue from this thinness is
reported, not hidden.
(c) 97171's mask-1: interpreted via the contracted-6281 precedent
rather than asserted; ruling rests on hollow-record + above-band in
any case.

## Contract

`wetlands-horde`, order 72, band 24-31: **[95682]**.
