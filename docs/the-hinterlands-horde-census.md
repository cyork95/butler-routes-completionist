# The Hinterlands (Horde) census (pack 0.130.0)

Source: local Forever game data (questie-forever `quests.json`, built with
`--product wowf` + QuestieDB). Candidate rule (the Alliance census method):
`zone == 1425` (38 records: 23 Horde-mask `races: 8589934770`, 8
Alliance-mask `races: 4294967373`, 7 null-mask shared) plus the city-rule
sweep (a start NPC/object spawning on the 1425 map). The sweep finds every
banked set-aside plus the 34 battleground-bracket/repeatable Warbringer
records (OUT by rule, excluded from the reconciliation by the brief) and
nothing else Horde — no beyond-25 Horde records exist. No record in the
pool carries a class restriction, a skill gate, or an exclusivity flag.
The 25 banked set-asides are all accounted for below.

## Band: 38–46

Horde minLevels over the 25 IN records: min38 ×1 (1444, the Fel'zerul
return), min40 ×1 (2933, the Venom Bottles object-start), min42 ×4 (77,
81 — the OOX honey chain; 2742, 2782 — the Rin'ji escort chain), min44
×11 (7815, 7816, 7828, 7829, 7830, 7839, 7840, 7841, 7842, 7843, 7844 —
the Revantusk core), min45 ×1 (98203, the Ti'ik hunt), min46 ×7 (7845,
7846, 7847 — the Torntusk chain; 7849, 7850; 7861, 7862 — the wanted
posters). Own-levels run to L51 on finales whose floor is in band. No
Horde record clears min46, so there is no Horde above-band set. Derived
band: **38–46** (same floor as the Alliance 38–51, lower ceiling — the
Alliance top is Hydamis/Aerie content with no Horde mirror here).

## IN ledger (25)

OOX honey chain (Gilveradin Sunchaser, west 26.71, 48.59):
- 77 L48 A Sticky Situation (min42, pre 650 — Ripple Recovery,
  Orgrimmar-contracted) — Gilveradin; 10 Hinterlands Honey Ripple
  (8684, off Venom Bottle-cluster objects 142191, west grounds
  45-47, 37-41). Accept rides a dedicated `when onquest 650` mini-step.
  Next: 81.
- 81 L48 Ripple Delivery (min42, pre 77) — Gilveradin; no objectives;
  ends at Dran Droffers (Orgrimmar 59.49, 36.57): expedition turn-in.

Fel'zerul return (Atal'ai Exile, south 33.75, 75.21):
- 1444 L44 Return to Fel'Zerul (min38, pre 1429 — The Atal'ai Exile,
  Swamp-Horde-contracted) — Atal'ai Exile; no objectives; ends at
  Fel'zerul (Swamp of Sorrows 47.93, 54.78): expedition turn-in. Accept
  rides a dedicated `when onquest 1429` mini-step. Next: 1445 The
  Temple of Atal'Hakkar (Swamp-Horde-contracted — the chain's head,
  handoff note, not duplicated here).

Rin'ji chain (Rin'ji, west 30.73, 46.9):
- 2742 L47 Rin'ji is Trapped! (min42, no pre) — Rin'ji; escort event
  (map-placed 34.58, 56.33); ends at Rin'ji's Secret object (142127,
  placed 1425 at 86.3, 59.01 — far east coast). Next: 2782.
- 2782 L47 Rin'ji's Secret (min42, pre 2742) — OBJECT-START (Rin'ji's
  Secret 142127, placed); no objectives; ends at Oran Snakewrithe
  (Undercity 73.06, 32.85): expedition turn-in. Next: 8273 Oran's
  Gratitude (UC zone, Horde, UNCONTRACTED — handoff note).

Venom Bottles (object-starts, west dens):
- 2933 L43 Venom Bottles (min40, no pre) — TWELVE object-starts (Venom
  Bottles 142702–142714, two west-den clusters at 23, 57-59 and 31.5,
  57.7); no objectives; ends at Apothecary Lydon (Tarren Mill,
  Hillsbrad 61.44, 19.06 — dual-spawn; the 1416 point named in the
  census): expedition turn-in. Next: 2934 Undamaged Venom Sac
  (Alterac-Horde-contracted — handoff, not duplicated).

Revantusk core (Revantusk Village, east-coast hub ~77-80, 78-81):
- 7815 L50 Snapjaws, Mon! (min44) — Katoom the Angler (80.33, 81.54);
  15 Saltwater Snapjaw (2505, shore grounds 74-77, 61-84).
- 7816 L48 Gammerita, Mon! (min44) — Katoom; Katoom's Best Lure
  (19023, Gammerita 7977, bay point 80.4, 58.23).
- 7828 L48 Stalking the Stalkers (min44) — Huntsman Markhor (79.16,
  79.53); 10 Silvermane Stalker (2926) + 10 Silvermane Howler (2925,
  wolf grounds 37-54, 42-63).
- 7829 L48 Hunt the Savages (min44) — Markhor; 20 Savage Owlbeast
  (2929, owl grounds 51, 45-63).
- 7830 L48 Avenging the Fallen (min44) — Markhor; Skylord Plume
  (19025, Razorbeak Skylord 2659, rookery points 47-51, 43-57).
- 7839 L48 Vilebranch Hooligans (min44) — Smith Slagtree (77.23,
  80.13); Slagtree's Lost Tools (19033, tools objects 179908, troll
  grounds 53-71, 38-48).
- 7840 L49 Lard Lost His Lunch (min44) — Lard (78.14, 81.38); Lard's
  Lunch (19034, Vilebranch Kidnapper 14748 at 84.6, 41.2 + Picnic
  Basket object 179910 at 84.47, 41.22).
- 7841 L48 Message to the Wildhammer (min44) — Otho Moji'ko (79.38,
  79.08); 15 Highvale Scout (2692) + 15 Highvale Outrunner (2691) + 15
  Highvale Ranger (2694) + 15 Highvale Marksman (2693) (Highvale
  grounds 28-31, 43-51). Next: 7842.
- 7842 L48 Another Message to the Wildhammer (min44, pre 7841) —
  Otho; 10 Long Elegant Feather (4589, Witherbark Hideskinner 2651,
  the 1425 dropper, west 27-29, 56-59). Next: 7843.
- 7843 L50 The Final Message to the Wildhammer (min44, pre 7842) —
  Otho; delivery event (map-placed 14.34, 48.07, Aerie side).
- 7844 L48 Cannibalistic Cousins (min44) — Mystic Yayo'jin (78.8,
  78.25); 30 Vilebranch Scalper (4466) + 15 Vilebranch Soothsayer
  (4467, ruins grounds 44-47, 62-68).

Torntusk chain (Primal Torntusk, hub 78.2, 81.18; Elder Torntusk,
Jintha'Alor 59.69, 77.84):
- 7845 L51 Kidnapped Elder Torntusk! (min46, no pre) — Primal
  Torntusk; no objectives; ends at Elder Torntusk. Next: 7846.
- 7846 L51 Recover the Key! (min46, pre 7845) — Elder Torntusk; Shackle
  Key (19064, Hitah'ya the Keeper 10802 — 1425 point 57.32, 86.64
  routes; the 1417 point named). Record zone 1417 (Arathi), accept at
  the 1425 spawn: IN by the dual-spawn rule (Named check 1). Next:
  7847.
- 7847 L51 Return to Primal Torntusk (min46, pre 7846) — Elder
  Torntusk; no objectives; ends at Primal Torntusk. Same dual-spawn
  ruling: IN (zero Arathi-Horde overlap verified — the Arathi-Horde
  census ruled both OUT above-band with the Hinterlands accept noted,
  so this census is the chain's home, argued in BORDERLINE 1).
- 7849 L50 Separation Anxiety (min46) — Markhor; Huntsman Malkhor's
  Skull (19069, Pile of Skulls 179915 at 58.56, 64.76) + Bones (19070,
  Pile of Bones 179914 at 62.11, 75.35).
- 7850 L50 Dark Vessels (min46) — Primal Torntusk; 10 Vessel of Tainted
  Blood (19071, vessel objects 179922, grounds 57-58, 65-76).

Wanted posters (Call to Arms! 179913, placed hub at 79.08, 78.99):
- 7861 L51 Wanted: Vile Priestess Hexx (min46, no pre) —
  OBJECT-START (poster, placed); Vile Priestess Hexx (7995, Jintha'Alor
  59.47, 78.26) + 20 Vilebranch Aman'zasi Guard (2648, terraces
  54-56, 82-84); ends at Primal Torntusk.
- 7862 L51 Job Opening: Guard Captain (min46, no pre) —
  OBJECT-START (same poster, placed); 20 Vilebranch Berserker (2643)
  + 20 Shadow Hunter (2645) + 20 Blood Drinker (2646) + guards
  (2644/2647, terraces 58-64, 65-84); ends at Primal Torntusk.

Ti'ik hunt (Qujo, hub 77.95, 77.83 — neutral giver, Horde mask):
- 98203 L49 Witch Doctor Ti'ik (min45, no pre) — Qujo; Ti'ik's Head
  (279913, count null in data — written without an invented count;
  Witch Doctor Ti'ik 270772, west grounds 24-26, 62-66); ends at Qujo.
  Mask decides over giver tag (Named check 2).

## Named-check rulings

1. 7847 (and 7846): IN. The 1425 spawn of Elder Torntusk is real
   (Jintha'Alor 59.69, 77.84, same terraces as its objectives), the
   Arathi-Horde contract on master holds NEITHER record (verified by
   ID — zero overlap is absolute), and the Arathi-Horde census ruled
   both OUT above-band there while naming the Hinterlands accept. A
   giver spawning in-zone is in-zone accept geography; no contract
   holds them; so they contract here. The Arathi rounds lose nothing —
   their census already pointed this way.
2. 98203: IN. Giver Qujo is neutral-tagged but the record mask is
   Horde 8589934770 — the mask decides faction availability (Duskwood
   ruling). Accepts in-zone at a placed giver; no gate beyond the
   mask the guide header already carries.
3. 7861/7862: IN. Wanted-poster object-starts with the poster placed
   in-zone at the hub; sequenced at the hub so the route never wedges.
4. 1444: IN. Accepts in-zone at a placed giver (Atal'ai Exile); its
   pre (1429, Swamp zone, uncontracted) rides a dedicated `when
   onquest 1429` mini-step; its turnin (Fel'zerul, Swamp) rides a
   Swamp expedition; its next (1445, Swamp zone, uncontracted — the
   Swamp pool's head) gets a handoff note. Followed, not re-contracted.

## Item-start enumeration (explicit scan of all 25)

Start items appear on ZERO records. Start objects appear on exactly
FOUR: 2782 (Rin'ji's Secret 142127, placed), 2933 (twelve Venom
Bottles, placed in two west-den clusters), 7861 + 7862 (shared Call
to Arms! poster 179913, placed). "No others" is claimable after this
scan (Mulgore lesson held).

## OUT list

Standing exclusions (nothing banked, verified by mask/flag):
- Battleground brackets + repeatables (34, all Horde Warbringer starts
  spawning on 1425 — the brief's count verified in the city-rule
  sweep): 8367, 8368, 8369, 8370, 8387, 8388, 8389, 8390, 8426-8435,
  8436-8443, past-victories 8566/8568/8570, Darkspear clash
  98887-98891 (98890 also broken: Lnull/minnull). OUT by rule.
- Alliance-only (8, all in the main guide's contract — none
  duplicated): 1452, 1469, 2877, 2880, 2881, 86615, 86616, 86620
  (all mask 4294967373, verified).
- Seasonal (2): 8643 (event 7, Lunar Festival), 9029 (event 8,
  Hallow's End).
- Accepts outside the zone (12, zone field wins per the Alliance
  census): 1450, 1451, 2988, 2989, 2990, 2994, 4297, 4298 (all zone
  1424 Hillsbrad, Alliance-mask — Hillsbrad-ruled); 6701 (repeatable),
  8234, 96779 (zone 1416 Alterac, null-mask — Alterac-ruled); 81954
  (zone 1458, null-mask — OUT per BORDERLINE 2, zone field wins).

## BORDERLINE (argued, none decided silently)

1. 7846/7847 IN here although zone-tagged Arathi: the dual-spawn
   rule is mechanical (giver spawns on 1425 → in-zone accept), the
   Arathi-Horde contract holds neither (checked by ID on master), and
   the Arathi-Horde census explicitly deferred them ("above-band"
   there, "Hinterlands accept" named). Contracting them here completes
   that handoff instead of stranding the chain between zones. If a
   later Arathi round wants them, zero-overlap forces a negotiation —
   recorded here so the conflict would be visible, not silent.
2. 1444's pre (1429) and next (1445) are both Swamp-Horde-contracted:
   the accept and turnin geography are both Hinterlands-adjacent
   (Exile in-zone, Fel'zerul a short Swamp frame away), so the quest
   belongs here with the soft-pre bridge + expedition, and the Swamp
   contract keeps its head and tail. Same shape as the Badlands 2284
   (Orgrimmar) bridge. The alternative (leaving a placed in-zone
   accept uncontracted) contradicts the pack principle.
3. Null-count objectives (98203's Ti'ik's Head): the data states no
   count; the guide writes the collect without an invented xN and lets
   lint/playtest report. Same handling as the 91497 seals (Azshara).
4. Batch exclusivity: none of the 25 carries excl/class/skill gates
   (verified null across the pool), so the guide needs no `only` or
   `when skill` lines at all.
