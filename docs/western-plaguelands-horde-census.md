# Western Plaguelands (Horde) census (pack 0.133.0)

Source: local Forever game data (questie-forever `quests.json`, built with
`--product wowf` + QuestieDB). Accept-zone key **1423**: 235 quest records
carry zone-field 1423 (20 Horde-mask `races: 8589934770`, 14
Alliance-mask `races: 4294967373`, 201 null-mask shared) — the count
matches the Alliance census exactly. The city-rule sweep (a start NPC or
object spawning on the 1423 map with a different zone field) finds, on the
Horde mask, only the six Argent Outfitter crafting records (zone 1412,
OUT by rule below) — no other Horde accept hides off-key. The 20 banked
set-asides are all accounted for below. No record in the pool carries a
skill gate; class gates exist only on the eight Anthion variants (one
class each, data-mapped below); the only exclusivity flags in the pool sit
on records already OUT (noted, never decided silently).

## Band: 54–58

Horde minLevels over the 19 IN records: min54 ×3 (6022, 6042, 6133 —
the Nathanos openers), min55 ×1 (9665 — the tower captures), min56 ×7
(6135, 6136, 6144, 6146, 6147, 6148, 6163 — the Nathanos chain), min58
×8 (8957, 9016–9022 — the Anthion class variants). Own-levels run to
L60 on finales whose floor is in band. No Horde record clears min58 —
the Alliance 60-block (tier turn-ins, attunements, Icebane, Kel'Thuzad)
has no Horde mirror here. Derived band: **54–58** (same top as the
Alliance 50–58, higher floor — the Alliance low end is Darrowshire and
Argent content with no Horde mirror).

## IN ledger (19)

Nathanos chain (Nathanos Blightcaller, west 22.23, 63.51):
- 6022 L58 To Kill With Purpose (min54, no pre) — Nathanos; Coagulated
  Rot (15448, NO placed source anywhere in the data — bare complete +
  note, Blasted-5206 shape). Corin's Crossing grounds to the east.
- 6042 L58 Un-Life's Little Annoyances (min54, no pre) — Nathanos; 20
  Noxious Plaguebat (8601, 38.66, 57.14) + 10 Monstrous Plaguebat
  (8602, 15.54, 17.01).
- 6133 L60 The Ranger Lord's Behest (min54, no pre) — Nathanos; 8
  Pathstrider (8565, 44.69, 15.29) + 8 Ranger (8564, 44.13, 11.21) + 8
  Woodsman (8563, 43.85, 11.24) + Quel'Thalas Registry (15847, object
  177747 placed 1423 at 45.27, 12.7 — the record's EPL wording is
  overridden by the data placement, argued in BORDERLINE 4).
- 6135 L60 Duskwing, Oh How I Hate Thee... (min56, no pre) — Nathanos;
  Patch of Duskwing's Fur (15850, Duskwing 11897 placed 1423 at
  26.08, 59.03).
- 6136 L60 The Corpulent One (min56, no pre) — Nathanos; Borelgore
  (11896, placed 1423 at 47.69, 24.87 — same data-over-text call as
  the Registry).
- 6144 L60 The Call to Command (min56, no pre) — Nathanos; no
  objectives; ends at Varimathras (Undercity 56.25, 92.2 — dual-spawn
  1421/1458, the UC point routes with the 1421 point named):
  expedition turn-in. Next: 6145 The Crimson Courier
  (Dustwallow zone, Horde, UNDERCITY-CONTRACTED — chain-end handoff,
  not duplicated here).
- 6146 L60 Nathanos' Ruse (min56, pre 6145 — Undercity-contracted) —
  Nathanos; The Grand Crusader's Command (13852, NO placed source
  anywhere — bare collect + note); Tyr's Hand named in the step from
  the objective text. Accept rides a dedicated `when onquest 6145`
  mini-step. Next: 6147.
- 6147 L60 Return to Nathanos (min56, pre 6146) — Crusader Lord
  Valdelmar (1423 point 75.21, 71.17, placed); no objectives; ends at
  Nathanos. Next: 6148.
- 6148 L60 The Scarlet Oracle, Demetria (min56, pre 6147) — Nathanos;
  Vaelan's Gift (item 12339, NO placed source — but Demetria herself
  is NPC 12339, placed 1423 at 63.3, 67.22): complete at Demetria
  with the item gap noted. Ends at Nathanos.
- 6163 L60 Ramstein (min56, no pre) — Nathanos; Head of Ramstein the
  Gorger (15880, Ramstein 10439 spawnless — Stratholme dungeon
  objective): complete at the in-zone Strat markers (49.98, 29.37, per
  the Alliance census's placed-marker audit) with a dungeon note.

Anthion class variants (Anthion Harmon, north-west 26.11, 11.3):
- 8957 / 9016 / 9017 / 9018 / 9019 / 9020 / 9021 / 9022 — all L60
  Anthion's Parting Words (min58, pre 9015 The Challenge — NULL-mask,
  MAIN-GUIDE-contracted shared) — Anthion; three dungeon-set pieces
  each, ALL droppers spawnless in the data (verified across all 24:
  Gyth/Rivendare/Gizrul/Wyrmthalak/Frostwhisper/Solakar/Willey/
  Jandice/Kirtonos/Rend/Omokk/Urok/Smolderweb et al. — bare collects
  + notes, the Alliance twins' exact shape). Ends at Mokvar
  (Orgrimmar 34.95, 38.29): expedition turn-in. Class gates from the
  data (bitmask-verified against the Alliance census's Hunter 4 /
  Rogue 8 / Mage 128 / Priest 16): 9022 Warrior (1), 9017 Hunter (4),
  9020 Rogue (8), 9019 Priest (16), 8957 Shaman (64), 9018 Mage
  (128), 9021 Warlock (256), 9016 Druid (1024) — no Paladin variant
  exists (Paladin is not a Horde class; consistent). All eight accepts
  ride ONE dedicated `when onquest 9015` mini-step (each persona sees
  exactly its class line); all eight turnins ride one Orgrimmar
  expedition step (same gating). Contracting them here discharges the
  Orgrimmar guide's soft-pre turnin lines into a real contract
  (Stonetalon-6562 pattern); the Orgrimmar guide is NOT edited by this
  round — its lines stay as city-leg documentation.
 Next: 9032 Bodley's Unfortunate Fate (Orgrimmar-contracted —
 chain-end handoff, not duplicated here).
- 9665 L60 Bolstering Our Defenses (min55, no pre) — Emmisary Gormok
  (1423 point 70.37, 47.94, placed); four tower-capture objectives
  whose names carry `<TXT>` placeholders BUT whose doodads are all
  placed on 1423 (Crown Guard 34.09, 64.1; Eastwall 59.04, 39.41;
  Northpass 49.25, 18.2; Plaguewood 18.16, 25.06). The brokenness is
  text-only; the record is runnable (anchorable accept, placed
  objectives) — IN with the defect noted. The objectiveText's EPL
  claim is overridden by the data placement, argued in BORDERLINE 4.
  Ends at Gormok.

## Named-check rulings

1. Anthion variants (all eight): IN — every accept verified at
   Anthion Harmon's placed 1423 spawn (26.11, 11.3); min58 in band;
   pres satisfied via the shared, main-guide-contracted 9015 (soft-pre
   mini); class gates exactly as the data gates. The Orgrimmar soft-pre
   turnins are discharged, not duplicated (that guide untouched).
2. 9665: IN — the `<TXT>` brokenness is text-only (objective names),
   while accept, ender, and all four objective doodads are placed and
   the minLevel (55) sits in band. Excluding it would mistake a
   placeholder string for a broken record.
3. 97988: OUT broken — the record is STILL an empty husk (empty start,
   empty end, empty objectives; only an objectiveText pointer at
   Corswyn Aseril, Orgrimmar). No accept geometry exists to route.
   Unchanged since the Alliance census; revisit if the record gains a
   start.

## Item-start enumeration (explicit scan of all 20 + 6)

Start items appear on ZERO records; start objects appear on ZERO
records (every accept in the pool is a placed NPC). "No others" is
claimable after this scan (Mulgore lesson held).

## OUT list

Broken (1): 97988 Orgrimmar's Windshapers (empty husk — see Named
check 3).
Rule-excluded, verified in the city-rule sweep (6): 9320 Major Mana
Potion, 9333 Argent Dawn Gloves, 9334 Blessed Wizard Oil, 9335
Consecrated Sharpening Stones, 9336 Major Healing Potion, 9343 Tabard
of the Argent Dawn — ALL `repeatable: true` AND `event: 99`, zone-field
1412, pre 9153 (uncontracted). OUT three times over; the 1423 spawn of
their vendor (Argent Outfitter 16787, a five-map vendor) is noted but
moot — repeatable + seasonal/event already excludes (the Alliance
census's city-rule "caught nothing" is thus imprecise, corrected
here without effect).
Alliance-only set-asides for the record (14, all in the main guide's
contract — none duplicated here): 5246, 5247, 5248, 8951, 8952, 8953,
8954, 8955, 8956, 8958, 8959, 9664, 84330, 97987 (all mask 4294967373,
verified). Null-mask records stay in the main guide's contract (65 –
52 Alliance/neutral mix per the Alliance ledger) or out per the
Alliance census (repeatables, seasonal, broken, above-band, accept-
outside-zone — listed there, verified by mask where load-bearing).

## BORDERLINE (argued, none decided silently)

1. Band 54–58 with a min54 floor: the Alliance band bottoms at min50
   (Darrowshire/Argent content with no Horde mirror). The pack rule
   draws the line from the Horde records' own minLevels (54 low, 58
   top) — no copying, no stretching to include the 50-block.
2. Same-name twins 8957/9016–9022 (all titled Anthion's Parting Words,
   eight ways): NOT exclusive variants — they are parallel class
   records (distinct classes, distinct objective sets, no excl flags).
   All eight route, each behind its own class gate (Harvesting
   precedent for same-name twins, class variant of it).
3. No Paladin variant exists among the eight: consistent (Paladin is
   Alliance-only in this data), not a gap — no ninth record to hunt.
4. Data-over-text placements (6133's Registry, 6136's Borelgore,
   9665's tower doodads): objectiveTexts point at the Eastern
   Plaguelands, but every target spawns on 1423 in the data. Game data
   wins over text (and over the Alliance census's expedition framing
   of the same records) — the completes ride in-zone points, and the
   discrepancy is stated here, not hidden. If the data ever moves
   these spawns off-zone, the completes become EPL expedition legs.
5. 6144's Varimathras point: dual-spawn NPC (1421/1458); the objective
   text names the Undercity, and the chain's next (6145) accepts in
   the Undercity contract — the UC point routes, the 1421 point named.
6. Out-of-contract pres (6145 Undercity-contracted; 9015 shared
   main-guide): both bridged with dedicated `when onquest` mini-steps;
   chain exits (6145, 9032 Orgrimmar-contracted, 97988 broken) get
   handoff notes, never silent ends. 6147's Valdelmar accept is
   in-zone (75.21, 71.17), so the Ruse chain never leaves the map
   except for the two UC expedition turn-ins.
