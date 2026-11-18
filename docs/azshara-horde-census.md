# Azshara (Horde) census (pack 0.129.0)

Source: local Forever game data (questie-forever `quests.json`, built with
`--product wowf` + QuestieDB). Candidate rule (the Alliance census method):
every quest record with `zone == 1447` OR `area == 16`. That sweep finds **82**
records with `zone == 1447` (23 Horde-mask `races: 8589934770`, 19
Alliance-mask `races: 4294967373`, 40 null-mask shared) plus the area-16
Horde records keyed elsewhere (3562 zone 1412, 3563/91735 zone 1454,
3564/91734 zone 1458, 91737 zone 1456). Cross-checked against the
Alliance 95-ledger (52 IN + 43 OUT IDs, all named there, none missing
from the data): 82 sit on key 1447 now and 13 sit off-key (3461,
5535, 5536, 8575, 8729, 96246 — Alliance-side context; 3504, 3562,
3563, 3564, 91734, 91735, 91737 — the Horde off-key set, ruled here).
82 + 13 = 95 exactly — no drift, no missing records. The 30 banked
set-asides are the 23 on-key Horde records + the 6 area-16 off-key
Horde records + 3504 (banked for its chain position, ruled here). No
Horde-mask record in either sweep falls outside the 30. No record in
the pool carries a class restriction or a skill gate; the only
exclusivity flag is 91608's `excl [89013]` (data, noted).

## Band: 44–50

Horde minLevels over the 22 IN records: min44 ×8 (3505, 3506, 3507 —
the Betrayed chain; 91497, 91500, 91531, 91538, 91547 — the Sin'dorei
seal/tome chain), min45 ×13 (3517, 3518, 3541, 3542, 3561, 3565 — the
Jediga delivery chain; 91488, 91568, 91569, 91608, 91610 — the
Kurll/Izvi beach hub; 91685; 92346), min50 ×1 (91607, the turn-in-only
Pay Dirt! twin). Own-levels run to L56 on finales whose floor is in
band — the long-standing rule, not an exception. Below-floor: none
(3504's m44 sits outside on geography, not band). Above-band: nothing
in the Horde pool clears min50 — the Alliance 55–60 top (Hydraxis,
Xylem, Azuregos content) has no Horde mirror here. Derived band:
**44–50**.

## IN ledger (22)

Betrayed chain (Ag'tor Bloodfist, west hub 22.26, 51.48):
- 3505 L53 Betrayed (min44, pre 3504 — Orgrimmar, OUTSIDE) — Ag'tor
  Bloodfist; 10 Blood Elf Reclaimer (6199, east camp 55, 27-30) + 10
  Blood Elf Surveyor (6198, same grounds) + Rimtori's camp event
  (59.53, 31.47); ends at the Kaldorei Tome object (151286, placed
  1447 at 59.51, 31.3). Accept rides a dedicated `when onquest 3504`
  mini-step (Belgrom Rockmaul, Orgrimmar 75.23, 34.24). Next: 91497.
- 3506 L56 Betrayed (min44, pre 3505) — OBJECT-START (Kaldorei Tome
  151286, placed); Head of Magus Rimtori (10597, sole dropper 8578
  Rimtori, 1447 point 59.51, 31.37 — same ground as the event); ends
  at Ag'tor. Next: 3507.
- 3507 L56 Betrayed (min44, pre 3506) — Ag'tor; no objectives; ends at
  Belgrom Rockmaul (Orgrimmar 75.23, 34.24): expedition turn-in.

Sin'dorei chain (Tome 247449, east camp 59.52, 31.31):
- 91497 L53 Seals of the Sin'dorei (min44, pre 3505) — Sin'dorei Tome
  of Summoning; Seal of the Warden (246725 ×1, Lieutenant Suncrest
  247006, 65-66, 26-29) + Seal of the Warrior (246721, Magister
  Hawkhelm 246991, 55-56, 26-29) + Seal of the Ranger (246722, Ranger
  Lydrea 247013, 68-69, 27-30) — all east camp. Next: 91500 + 91538.
- 91500 L55 An Explosive Gambit (min44, pre 91497) — Tome; Head of
  Magus Rimtori (10597 — a SECOND head; Rimtori re-drops it, noted in
  the guide); ends at Ag'tor. Next: 91531.
- 91531 L55 Revenge Exacted (min44, pre 91500) — Ag'tor; no
  objectives; ends at Belgrom Rockmaul (Orgrimmar): expedition turn-in.
- 91538 L55 Sin'dorei Tome of Summoning (min44, pre 91497) — Tome; no
  objectives; ends at Jediga (west hub 22.56, 51.42): talk-through.
  Next: 91547.
- 91547 L55 Sin'dorei Tome of Summoning (min44, pre 91538) — Jediga;
  no objectives; ends at Zevrost (Orgrimmar 48.47, 45.43): expedition
  turn-in. Next: 91548 Vek'zol (Orgrimmar-contracted — chain-end
  handoff, not duplicated).

Jediga delivery chain (Jediga, west hub 22.56, 51.42):
- 3517 L52 Stealing Knowledge (min45, no pre) — Jediga; 4 tablets off
  placed Azshara objects (Beth'Amara 148516, Jin'yael 148513, Markri
  148514, Sael'hai 148515 — center ruins 34-36, 49-59). Next:
  3518/3541/3542/3561 (four parallel deliveries).
- 3518 L52 Delivery to Magatha (min45, pre 3517) — Jediga; no
  objectives; ends at Magatha Grimtotem (record zone 1412, point
  44, 23.1; also Thunder Bluff 69.85, 30.91): expedition turn-in via
  `zone map 1412`. Next: 3562 (accepts at Magatha, OUT — handoff).
- 3541 L52 Delivery to Jes'rimon (min45, pre 3517) — Jediga; no
  objectives; ends at Jes'rimon (Orgrimmar 55.52, 34.08): expedition
  turn-in. Next: 3563 (accepts at Jes'rimmon, OUT — handoff).
- 3542 L52 Delivery to Andron Gant (min45, pre 3517) — Jediga; no
  objectives; ends at Andron Gant (Undercity 54.81, 76.33): expedition
  turn-in. Next: 3564 (accepts at Andron, OUT — handoff).
- 3561 L52 Delivery to Archmage Xylem (min45, pre 3517) — Jediga; no
  objectives; ends at Archmage Xylem (1447 point 29.25, 40.21).
  Next: 3565 (IN — the chain continues home).
- 3565 L52 Xylem's Payment to Jediga (min45, pre 3561) — Xylem; no
  objectives; ends at Jediga.

Beach hub (Kurll 3621, 21.82, 52.1; Izvi Gildfizz 247473, 22.46, 51.89):
- 91488 L48 Home on the Range (min45, no pre) — Kurll; 5 Mosshoof Hide
  (238463: Runner 8759, Stag 8760, Courser 8761 — south grounds
  12-33, 75-82 + center). Twin of Alliance 89001 (untouched); ALSO the
  Horde alt-pre of Alliance 89013/89228 (BORDERLINE 7 — no duplication,
  ruled here by its own accept).
- 91608 L48 Gettin' Buzzed (min45, pre [89001, 91488] alt) — Kurll;
  5 Wild Honey (238503, Honey Wasp 236028, west grounds 15-17, 49-54).
  Twin of 89013; `excl [89013]` is data exclusivity, noted — the Horde
  path runs via 91488 in-guide. No mini (pre satisfied in-contract).
- 91610 L48 Winter Frontier Fishery (min45, pre [89001, 91488] alt) —
  Kurll; 10 Winter Squid (13755, NO source anywhere in the data —
  fished, same R2 as twin 89228's squid). Twin of 89228; Horde path
  via 91488, no mini.
- 91568 L51 Long Walks on the Beach (min45, no pre) — Izvi; 10
  Highborne Treasure Fragment (246684, Makrinni Burrower 247470,
  center-east 44-45, 45-55).
- 91569 L53 Blue Gold (min45, no pre) — Izvi; Mana-Siphoning Wand
  (246680, Blood Elf Arcanist 246920, east camp 65-66, 26-28; two
  off-zone droppers exist, the Azshara one routes). Next: 91685.
- 91685 L54 Ley of the Land (min45, pre 91569) — Izvi; Tear of Mennar
  (246938, sole dropper 247972 Celegosa, far south 38.27, 81.58).
- 91607 L53 Pay Dirt! (min50, no pre) — TURN-IN-ONLY (empty start, end
  Izvi; the 90813 shape, twin of Alliance 90813); Humongous Crystal
  (246888, Cliff Walker 6148 — west point 16.82, 53.81 routes).

Far north (Nara Wildmane dual-spawn; Thunder Bluff point chosen):
- 92346 L55 Beneath Nordrassil (min45, no pre) — Jediga; no
  objectives; ends at Nara Wildmane (Thunder Bluff 75.65, 31.61 —
  dual-spawn 1412/1456, TB point stated): expedition turn-in. Twin of
  Alliance 92345 (untouched); next 92343 Get to the Roots of It
  (Thunder-Bluff-contracted — handoff, not duplicated).

## Named-check rulings

1. Twin family (all ruled by own ID): 91488/91608/91610/91611 IN-or-OUT
   below on their own accepts (91488, 91608, 91610 IN; 91611 OUT
   broken); 91607 IN turn-in-only (90813 precedent); 92346 IN
   (expedition + handoff). In no case does the twin's disposition
   decide: 91611 is OUT although its twin 89015 is contracted (the
   Horde record has no accept at all), and 91607 is IN although it has
   no accept either (its turn-in exists in-zone with a placed-objective
   source — the exact 90813 shape).
2. 91488 is the ALT pre of Alliance 89013/89228 alongside 89001. That
   relationship changes nothing here: 91488 is ruled by its own accept
   (IN), the Alliance quests stay in the main guide where the ungating
   keeps them Alliance-visible only, and my 91608/91610 route via the
   91488 alt-leg with no mini needed.

## Item-start enumeration (explicit scan of all 30)

Start items appear on ZERO records; start objects on exactly ONE:
3506 Betrayed (Kaldorei Tome object 151286, placed 1447) — routed
normally as the chain's object-start leg. 91607 and 91611 carry EMPTY
starts (no npc/object/item at all): 91607 is turn-in-only (IN, honest
note), 91611 has no end either (OUT broken). "No others" is claimable
after this scan (Mulgore lesson held).

## OUT list

Accepts outside the zone (7): 3504 Betrayed (L53/min44) — accepts at
Belgrom Rockmaul in Orgrimmar (1454 point 75.23, 34.24); 3505's pre, so
the guide bridges it with a dedicated `when onquest 3504` mini-step.
3562 Magatha's Payment (L52/min45) — accepts at Magatha Grimtotem
(record zone 1412); 3518's next, handoff note. 3563 Jes'rimmon's
Payment (L52/min45) — accepts at Jes'rimmon in Orgrimmar; 3541's next,
handoff note. 3564 Andron's Payment (L52/min45) — accepts at Andron
Gant in the Undercity; 3542's next, handoff note. 91734/91735/91737
Remote Contact (L52/min44, Andron/Jes'rimmon/Magatha city accepts,
UC/Org/TB zones) — the city-side remote pointers; 91734 additionally
has an empty end and no objectives (degenerate, second reason).
Broken (1): 91611 Deadliest Catch (L56/min50) — no accept AND no
turn-in anywhere in the record (empty start and end) against an
objective (1 Mammoth Shark Steak) whose dropper (12125 Mammoth Shark,
placed 1447 at 61.11, 52.25 — the Alliance guide's point, verified in
the dump) does exist. The gap is the missing accept/turnin, not the
objective — still unroutable as stated. Twin 89015's contracted
accept-only shape does not transfer (97821 Mirage Mirror precedent).
Revisit if the record gains an accept.
Alliance-only quests for the record (20, all in the main guide's
contract — none duplicated here): 3461 (Return to Tymor — banked
nowhere as Horde, being Alliance-mask; gated in the ungating) plus
5141, 88807, 88809, 88812, 88813, 88821, 88857, 88884, 88917, 89001,
89013, 89015, 89037, 89038, 89053, 89228, 89470, 90813, 92345. Null-mask records stay in the main guide's
contract or out per the Alliance census (repeatables 3382/3421/3503,
above-band 6821/6822/6823/6824/7486/9362/9364/8575/8729, broken
96246) — the Alliance ledger accounts for every one; nothing null-mask
is duplicated here.

## BORDERLINE (argued, none decided silently)

1. Band 44–50 with a single min50 record (91607): the band bottom
   (m44 Betrayed/Sin'dorei openers) and top (m50 turn-in-only twin)
   are both genuine in-zone accepts; the Alliance 45–55 is not copied
   (no Horde record clears min50, so there is no Horde 55-block).
2. 3504 OUT while its whole chain stays IN: accept geography is the
   pack's first rule (3461/BORDERLINE-2 precedent in reverse — there
   the Azshara accept-spawn won; here the Orgrimmar accept loses).
   The chain is not severed: the mini bridges the pre openly.
3. 3562/3563/3564 OUT while their pres (3518/3541/3542) are IN: same
   call at the chain ends — a delivery ending off-zone ends the
   contracted story there, with the next ID named so a later round
   (or player) can pick it up. 3565 is the contrast that proves the
   rule (ends at Xylem in-zone → IN).
4. 91611 OUT broken although twin 89015 is IN: the twin's accept
   (Berdun 240482) does not transfer across faction records. The steak
   objective even has a placed dropper — but a quest with no accept
   and no turn-in cannot be pointed at regardless. Data over symmetry.
5. 91607 IN turn-in-only although it has no accept either: the
   difference from 91611 is the placed ender (Izvi in-zone) plus a
   placed objective source (Cliff Walkers) — the exact contracted
   shape of 90813 and 86747. The asymmetry with 91611 is argued, not
   silent.
6. Null-count objectives (91497's Warrior/Ranger seals, 91500's Head):
   the data states no count; the guide writes the collects without an
   invented xN and lets lint/playtest report. No count is invented to
   satisfy the repair format.
7. 92346's Nara point: dual-spawn NPC (1412 + Thunder Bluff); the
   Thunder Bluff point routes (Horde-hub consistent, and 92343's TB
   contract starts at Nara there). The 1412 point is named here so the
   choice is auditable.
8. Out-of-contract pres/exits: 3504 (OUT, mini-bridged); 91548
   (Orgrimmar-contracted) and 92343 (Thunder-Bluff-contracted) as
   named handoffs; 3562/3563/3564 as named off-zone nexts. Nothing
   silent at either end of any chain.
