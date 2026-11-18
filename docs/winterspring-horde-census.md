# Winterspring (Horde) census (pack 0.135.0)

Source: local Forever game data (questie-forever `quests.json`, built with
`--product wowf` + QuestieDB). Accept-zone key **1452**: 64 quest records
carry zone-field 1452 (5 Horde-mask `races: 8589934770`, 14 Alliance-mask
`races: 4294967373`, 45 null-mask shared). The Alliance census worked a
wider candidate set (78 giver/object accepts + 4 item-start discoveries,
counting dual-spawn border points); this census counts the zone field
strictly (64) and rules the border/dual cases by spawn frame below — the
difference is method, not drift. The 7 banked set-asides are all
accounted for. No record in the pool carries a class restriction, a skill
gate, or an exclusivity flag.

## Band: 49–55

Horde minLevels over the 7 IN records: min49 ×1 (6605, Harlo's
wildkin opener), min50 ×1 (6029, Gregor's Everlook Report), min52 ×1
(4882, the owlbeast-necklace item-start), min53 ×4 (5054–5057, the
Storm Shadowhoof chain). No Horde record clears min55 — the Alliance
55–60 top (Hydraxis, Arcanist, Thorium) has no Horde mirror. Derived
band: **49–55** (same floor family as the Alliance 47–60, far lower
ceiling — nothing above-band to exclude).

## IN ledger (7)

- 6605 L54 A Strange One (min49, no pre) — Harlo Wigglesworth (placed
  1452 at 61.12, 38.43); no objectives (talk-through); ends at Winna
  Hazzard (Timbermaw Hold, Felwood frame 1448 at 34.21, 52.34 — the
  1439 dual point named in the census): expedition turn-in. Next: 4505
  Well of Corruption (UNCONTRACTED remainder — chain-end handoff, not
  duplicated here).
- 5054 L56 Ursius of the Shardtooth (min53, no pre) — Storm Shadowhoof
  (placed 1452 ONLY, at 61.93, 38.38 — the zone tag says Darkshore
  1439, the giver stands in Winterspring; accept-geography wins per
  the Kargath/Hinterlands-7847 rule); Ursius (10806, 1452 point
  60.92, 32.9). Record zone 1439, area 618. Next: 5055.
- 5055 L58 Brumeran of the Chillwind (min53, pre 5054) — Storm
  Shadowhoof; Brumeran (10807, 1452 point 62.54, 57.9). Next: 5056.
- 5056 L60 Shy-Rotam (min53, pre 5055) — Storm Shadowhoof; Shy-Rotam
  (10737, 1452 point 49.81, 9.8). Next: 5057.
- 5057 L60 Past Endeavors (min53, pre 5056) — Storm Shadowhoof; no
  objectives (talk-through).
- 6029 L52 The Everlook Report (min50, no pre) — Gregor Greystone
  (placed 1452 at 61.35, 38.97); no objectives; ends at Argent Officer
  Garush (EPL Andorhal 26.6, 55.5 — dual-spawn; the Tirisfal point
  83.19, 68.45 named in the census): expedition turn-in. The Horde end
  of Gregor's triple (6028 Alliance / 6030 neutral stay in the main
  guide, ungated — no mutual-exclusion issue in the data).
- 4882 L59 Guarding Secrets (min52, no pre) — ITEM-START (Blue-feathered
  Necklace 12558; droppers Crazed/Moontouched/Berserk Owlbeast 7452/
  7453/7454, ALL spawning on 1452 — the accept geography is in-zone by
  the item-start rule); no objectives (talk-through item record); ends
  at Trull Failbane (Timbermaw Hold, Felwood frame 1448 at 34.73,
  52.79 — the 1439 dual point named): expedition turn-in. Next: 4883
  Guarding Secrets (UNCONTRACTED remainder — chain-end handoff).

## Named check — the Timbermaw cluster, record by record

Givers Winna Hazzard (9996), Trull Failbane (10306), Dreka'Sur (9620)
each dual-spawn on Darkshore-frame 1439 and Felwood-frame 1448 points
(Timbermaw Hold country both sides); NONE spawns on 1452. Storm
Shadowhoof (10303) spawns ONLY on 1452. Nara Wildmane (5770) spawns
only on 1412 (Thousand Needles-side) and 1456 (Thunder Bluff).
- 4505 Well of Corruption (zone 1439, m49, pre 6605) — accepts at
  Winna (off-zone both frames). OUT accepts-outside-zone. Named
  remainder: Felwood frame primary (its next 4506's event objective is
  map-pinned at Felwood 1448: 34.26, 52.32, on top of Winna's Hold
  point) with the 1439 dual noted; no Horde guide holds it.
- 4506 Corrupted Sabers (zone 1439, m49, pre 4505) — accepts at Winna
  (off-zone). OUT, same remainder (Felwood frame).
- 4521 / 4741 / 4721 Wild Guardians (zone 1439, m52 chain) — accept at
  Trull (off-zone both frames). OUT accepts-outside-zone, although
  most owlbeast objectives spawn on 1452 (objectives in-zone with
  accepts elsewhere stay OUT per the Riverglades/Duskwood rule).
  Named remainder, same frames.
- 4883 Guarding Secrets (zone 1439, m52, pre 4882) — accepts at Trull
  (off-zone). OUT accepts-outside-zone; its pre IS contracted here
  (4882), and its ender (Nara, off-zone both frames) is noted — a
  clean sever, not a strand. Named remainder.
- 6162 A Husband's Last Battle (zone 1439, m46) — accepts at Dreka'Sur
  (off-zone both frames). OUT accepts-outside-zone; its objective
  dropper (Overlord Ror 9464, Felwood-only spawn) is doubly off-zone.
  Named remainder.
- 4882 (above) is the cluster's exception that proves the geography
  rule: its accept is the in-zone ITEM drop, so it contracts here even
  though its turnin and next live in the remainder frames.
If a future micro-round (Darkshore-Horde or Felwood-Horde-companions
scope) picks up 4505/4506/4521/4741/4721/4883/6162, this census is its
handoff manifest: every ID, both frames, chain links, and the two
contracted bridge-ends (6605's next, 4882's next) are named above.

## Named-check rulings (banked set)

1. 7847-analog check (5054–5057): zone-tagged Darkshore 1439, but the
   giver's ONLY spawn renders on the 1452 frame and every objective
   target spawns on 1452 — accept-geography wins outright (stronger
   than the Hinterlands 7847 case, where the giver dual-spawned). IN.
2. 98203-analog check: none needed — no neutral-giver Horde record in
   this pool.
3. The three empty-start records (97264 Shardtooth Pulling, 97403
   Two-Headed Ravagers, 97404 Too Bad to Bear — all Horde, all zone
   1452, m55): OUT broken. Objectives reference placed in-zone mobs
   (Elder Shardtooth, Chillwind Ravager, Kuroma/Kamuro — all 1452), but
   the records carry NO accept and NO turnin (the 91611 shape, argued
   the same way). Noted, not contracted; revisit if the records gain
   endpoints.
4. 97988 is OUT broken (empty husk, brief's named check 3 — record
   unchanged: empty start/end/objectives; only an objectiveText
   pointer at Corswyn Aseril, Orgrimmar).

## Item-start enumeration (explicit scan of all 20 + 6)

Start items appear on exactly ONE record: 4882 Guarding Secrets (item
12558, Blue-feathered Necklace — in-zone droppers verified above).
Start objects appear on ZERO records. "No others" is claimable after
this scan. (The six Argent Outfitter crafting records carry NPC starts
at the multi-frame vendor 16787 — noted under OUT, not item-starts.)

## OUT list

Accepts outside the zone (6 + 1 husk-adjacent): 4505, 4506, 4521,
4741, 4721, 4883 (Timbermaw remainder, Felwood frame primary — see
above); 6162 (same, plus off-zone objective). Broken (4): 97988 (empty
husk); 97264, 97403, 97404 (no accept/end — see Named check 3).
Rule-excluded (6, verified by flag, NOT by geography): 9320 Major Mana
Potion, 9333 Argent Dawn Gloves, 9334 Blessed Wizard Oil, 9335
Consecrated Sharpening Stones, 9336 Major Healing Potion, 9343 Tabard
of the Argent Dawn — ALL `repeatable: true` AND `event: 99`, zone-field
1412, pre 9153 (uncontracted). Their vendor's 1452 spawn is noted and moot
spawn is noted and moot: repeatable + seasonal/event excludes
regardless of accept frame (the Alliance census's city-rule "caught
nothing" is corrected here without effect).
Alliance-only set-asides for the record (14, all in the main guide's
contract — none duplicated here): 4861, 4863, 4864, 4901, 4970, 5201,
5244, 5245, 5252, 5253, 5981, 6028, 6502, 6604 (all mask 4294967373,
verified). Null-mask records stay in the main guide's contract (65 contracted = 12 Alliance + 53 shared per the ledger's own arithmetic) or out per
the Alliance census (repeatables 4801-4807/4970/5201/5981/5063/5067/
5068/8467/8469/9266, seasonal 8672/8726, broken 5047/5103/5160,
contracted-elsewhere 6031/6032/6241/8461/8462/8464/8465/8471/5083/
84399, above-band none).

## BORDERLINE (argued, none decided silently)

1. 5054–5057 IN although zone-tagged 1439: the zone tag is the ONLY
   Darkshore fact about these records (giver, all four objectives
   in-zone on 1452). The pack's accept-geography rule
   (3461-Azhara, Badlands-3504-inverse, Hinterlands-7847) resolves tag-
   vs-spawn conflicts toward the spawn. If the data ever moves Storm
   Shadowhoof off 1452, these four follow him.
2. 4882 IN although zone-tagged 1439 and turnin/ender off-zone: the
   item-start rule places the accept where the item drops (1452 owl-
   beasts). The off-zone turnin rides an expedition leg like any other
   (Badlands-2340 shape); the uncontracted next (4883) gets a handoff
   note, not a silent end.
3. 4505's pre (6605) IS contracted while 4505 itself is OUT: the chain
   crosses the contract boundary mid-link (accept geography changes
   hands at Winna). 6605's turnin + handoff carry the player to the
   boundary; the remainder manifest picks them up. No different from
   any expedition-into-uncontracted-next shape, except the next is a
   named remainder rather than a contracted guide.
4. 9665's `<TXT>` names vs placed doodads: text-only brokenness, IN
   with the defect noted (BORDERLINE 2 of the brief's named checks).
   The EPL objectiveText is overridden by the data placement — same
   call as the WPL Registry/Duskwing/Borelgore rulings last round.
5. 97988 vs 97264/97403/97404: two flavors of
   broken. 97988 is empty in EVERY field (husk); the trio have real
   objectives on placed mobs but no endpoints. Both OUT, distinguished
   in the ledger so a future data fix routes each correctly (endpoints
   added → contractable; husk gains content → re-rule).
6. No soft-pre minis were needed: every IN-record pre is either empty
   or contracted in-route... (verified: 5055←5054, 5056←5055,
   5057←5056 — all in-contract, all routed in chain order). The
   technique stands ready but untriggered; the guide states this
   rather than inventing minis.
