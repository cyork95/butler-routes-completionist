# Silithus (Horde) census

Method: the established Horde-side census shape (Duskwood / Riverglades /
WPL Horde). Accept-zone key **1451**, verified by count against the local
data build (`--product wowf` + QuestieDB): 145 quest records carry the
zone field, the same pool the Alliance census worked
(`docs/silithus-census.md`, 112 candidates, 52 IN at band 54-60). A second
pass over giver-spawn geography (every giver spawning on map 1451: 108
candidate records) confirms the pool from the other side; the two scans
agree on every Horde-mask record below.

## Horde-mask records on key 1451 (19 — the full scan)

Every record below carries races mask `8589934770` (Horde-only) with a
Silithus accept. "No others" is claimable: the scan covered all 145
zone-field records plus all 108 giver-1451 records, and these 19 are the
complete Horde-mask set.

### IN (3)

- **8380 Armaments of War** (60/min58, Shaman). Accept + turn-in Geologist
  Larksbane (49.67, 37.46, map 1451). Pre 8315 (The Calling chain) is a
  shared-mask record contracted in the main guide — bridged by a dedicated
  `when onquest 8315` mini-step, never duplicated. Every line
  `only Shaman` per data.
- **9416 Report to General Kirika** (60/min1). Accept Scout Bloodfist
  (48.95, 36.69, map 1451), turn-in General Kirika (50.75, 69.54, deep
  south). No pre. Below-band entry breadcrumb, same shape as the Alliance
  side's min1 outliers (3884/9415/9419) — IN as the natural Horde zone
  entry.
- **9422 Scouring the Desert** (60/min1). Pre 9416 (in-contract above).
  Accept + turn-in General Kirika; objective is the Horde dust-turnin
  doodad (18199) beside her. Same-name faction twin of the Alliance 9419
  (both called "Scouring the Desert") — each twin lives in its own
  faction's guide; the guide carries a `note` so the player is not
  confused by the twin names (Harvesting the Harvesters precedent).

### OUT — event-gated (4)

- **8690 / 8698 / 8706** (Shaman class armor: Hood, Leggings, Bindings;
  min50-56). All carry seasonal/event flag **86** (AQ-gate event set).
  The Alliance census excluded the entire ev86 class-armor set on both
  factions' sides the same way; these three are that set's Shaman
  members. OUT by the event rule.
- **8731 Field Duty** (Horde, min50). Carries event flag **86**; the
  Alliance census excluded its Alliance twin 8507 for exactly this
  reason. OUT by the event rule.

### OUT — event-chain dependent (1, BORDERLINE-argued)

- **8732 Field Duty** (Horde). Its own record carries NO event flag — but
  its sole pre is **8731**, excluded above, with no alternate path in the
  data. Outside the AQ-gate event the pre is unobtainable, so 8732 is
  unobtainable with it: a soft-pre mini on 8731 would ride dead in every
  non-event playthrough, and the pack never contracts a quest whose only
  path runs through an excluded event record. OUT as event-chain
  dependent. Appeal path: if 8731 ever re-enters (a future
  event-content round), 8732 follows it without touching this contract.

### OUT — war-effort repeatable turn-ins (10)

- **8785 / 8786 / 8787** (Orgrimmar Legion needs: Fibers, Parchment,
  Glands) and **8804 / 8805 / 8806 / 8807 / 8808 / 8809 / 8810** (Guns,
  Iron Bars, Stones, Oils, Chops, Morsels, Fillets). Repeatable
  material hand-ins of the war-effort class. Precedent: their six
  Alliance mirrors (8778-8783, Ironforge Brigade / Stormpike Guard /
  Darnassus Sentinel needs) are likewise uncontracted in the main guide
  (verified against `docs/quest-contracts.json`). Symmetric OUT.

### OUT — Barrens-tagged (1): the 98093 closure

- **98093 Field to Clear** (23/min18, Horde). Full record: accept + turn-in
  Sulhasa (NPC 14242), no pre, kill objectives (Hecklefang Stalker x7,
  Stormhide x7), no event flag — a complete record, NOT broken. But it is
  not Silithus content on three independent grounds: (1) its quest zone
  field is **1413** (Barrens), not 1451; (2) in this build Sulhasa spawns
  on key **1449 only** — no 1451 spawn point exists locally, so the
  "giver's 1451 spawn" reading does not reproduce (the Un'Goro (Horde)
  census's 1451 point at (80, 17) is a single-source claim this build
  cannot confirm — marked unconfirmed, not relied on); (3) min18 sits 40
  below the Horde band floor. Already adjudicated OUT by the Un'Goro
  (Horde) census (`docs/ungoro-horde-census.md`: below-band +
  Barrens-zone content, flagged for the Barrens future). Checked against
  the built `the-barrens` contract (157 quests): absent there too. This
  round does not home it and does not touch other contracts — the
  Barrens (Horde) future may home it without touching this contract.
  CLOSED with pointers; it does not leave this round
  uncontracted-and-unexplained.

### Noted, staying in the main guide (no duplication)

- **8305 Vessel of Rebirth** (null mask, shared): accept Anachronos on the
  Tanaris map, main-guide soft-pre mini. **1124** (null mask, shared):
  Moonglade accept, main-guide mini. **8275** (Alliance-only): Ironforge
  accept, main-guide mini (gated `only Alliance` by the ungating).
- **94316** (null mask, shared): accepts from Archmage Xylem on the Azshara
  map (1447-only giver) — already contracted in `azshara` (documented
  accept-only record). Not Horde content, not duplicated here.

## Item-start scan

Explicit start-item scan over the Horde pool: **zero** start-item fields
across all 19 Horde-mask records (every accept is an NPC accept: 15183,
17079, 17081). No dropper-hunt belongs to this core — "no item-starts" is
stated WITH the scan run, not asserted without one (Mulgore lesson honored).

## Band

Contracted minLevels: 58 (8380) with two below-band entry outliers (9416,
9422, min1 each) — the same shape as the Alliance band statement (54-60
with min48/min1 outliers). Horde band: **58-60**.

## BORDERLINE

1. **8732** (above): the only record whose own flags are clean but whose
   chain is event-rooted. Excluded with the appeal path named, not
   silently.
2. **9422's complete point**: its doodad (18199) has no spawn record in
   objects.json — exactly like its Alliance twin's doodad (17090), which
   the main guide places beside the turn-in NPC (Marshal Bluewall).
   This guide mirrors that documented convention: the complete rides at
   General Kirika's data-placed point with the derivation stated in the
   step note. No invented spawn; the convention is cited, not hidden.
3. **98093** (above): three readings converged; ruled OUT here with the
   Un'Goro ruling and the Barrens-contract check both cited. Nothing
   about this record is left undecided.

## Contract

`silithus-horde`, order 79 (next free at commit time; 78 taken by
`shendralas-horde`), band 58-60: **8380, 9416, 9422**.
