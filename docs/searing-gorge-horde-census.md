# Searing Gorge (Horde) closure census (game data, accept-zone key 1427)

Source: local Forever game data (questie-forever quest/NPC/object/item
dumps, built with `--product wowf` + QuestieDB). Method mirrors the
Alliance census (`docs/searing-gorge-census.md`): a quest accepts on 1427
if a start NPC, start object, or start-item dropper spawns on 1427; the
`zone` field is a cross-check only. Race mask 8589934770 = Horde-only,
4294967373 = Alliance-only, anything else (null included) = shared.

This round is shaped differently by design: the Alliance census banked 19
Horde set-asides but noted 18 of them accept on key 1418 (Badlands, the
Kargath side). This census verifies that claim record by record instead of
assuming a normal Horde core.

## Pool: 88 records keyed to 1427

81 have a placed accept point on 1427; 7 are sourceless-start records with
`zone: 1427` and no placed start point anywhere (7704 pillow starter,
writs 94263/94275/94287/94299/94311, and 8996 whose start NPC 16073 has
zero spawns). All 7 are already dispositioned: 7704 + the 5 writs are
contracted (Alliance/shared, bag-note handling); 8996 is the shared
min58 pre of the Bodley finale, above-band OUT with its chain. Placed
pool mask split: **19 Horde-only, 10 Alliance-only, 52 shared**.

## Reconciliation 1 — the 18 Kargath records: Badlands content, confirmed

782, 793, 2202, 2203, 2258, 2338, 2339, 2340, 3821, 3906, 3907, 4061,
4062, 4081, 4082, 4134, 4768, 7201. Every one carries `qzone: 1418`.
Every start point resolves to the Kargath camp: the 1418 point sits at
~(2.4-3.7, 45.6-48.3) and the 1427 point at ~(81.4-82.9, 36.7-39.4)
(Gorn 1068, Jarkal 6868, Thal'trak 9082, Thunderheart 9084, Theodora
9079, Vivian 9078, WANTED boards 164867/164868 — one point per frame
each). That is ONE physical camp at the Badlands/Searing Gorge border
pass, recorded on both map frames — not two quest hubs. The `qzone:
1418` field agrees. They do not accept in Searing Gorge; this round does
not contract them and does not duplicate them.

Disposition in the Badlands (Horde) contract (order 66, band 30-40,
`docs/badlands-horde-census.md`, verified on master): 8 IN — 782, 793,
2202, 2203, 2258, 2338, 2339, 2340. 10 OUT above-band (BH census "Above-
band (20, all min48+)" section, quoted): 3821, 3906, 3907, 4081, 7201
(min48); 4082, 4134 (min50); 4061, 4062 (min52); 4768 (min57). All 18
accounted for; none left homeless.

## Named check 2 — quest 8998 (Back to the Beginning): ruled OUT, no addendum

Full record: L60/min58, races Horde-only, start NPC **16033 Bodley**,
end NPC **16012 Mokvar**, pre 8996, objective text "Speak with Mokvar at
Grommash Hold in Orgrimmar's Valley of Wisdom", `zone: 1427`. Bodley
spawns on 1415 (48.9, 63.93), 1427 (39.8, 96.5), and 1428 (32.2, 25.8);
Mokvar spawns only on 1454 (Orgrimmar, 34.95, 38.29).

The brief's premise — that 8998 accepts from Mokvar in Orgrimmar — is
falsified by the start data: 8998 ACCEPTS from Bodley (Blackrock
Mountain ground, qzone 1427) and only TURNS IN at Mokvar. The accept
rule governs, so the Orgrimmar addendum does NOT ship: a turn-in-only
presence is noted, never contracted (turn-in-only-in-city stays out per
the city censuses). The Searing Gorge band (40-52) independently rules
it OUT (min58, same as its Alliance twin 8997 was for this zone). Twin
8997 (Bodley -> Deliana/Ironforge, min58) is contracted in
burning-steppes (band 48-52 per its census; the guide routes the Bodley
accept with an Ironforge expedition turn-in). 8998's chain-consistent
future home is therefore symmetric with its twin — a Burning Steppes-
side or endgame-round decision for the Bodley chain, out of scope for a
round that may not touch the closed Burning Steppes guide. 8998 stays
uncontracted pack-wide, with the reason and the pointer recorded here.
The flag closes.

## Item-start scan (explicit, over the 1427 pool)

4 item-starts: 3181 (Horn, Margol SG-only — Alliance, contracted),
4264 (Note, Anvilrage droppers incl. in-zone — Alliance, contracted),
4451 (Key, in-zone Dark Iron droppers — shared, contracted), 7761
(Blackhand's Command, min55 — shared, above-band OUT per the Alliance
census). Zero Horde-mask item-starts. Nothing asserted without the scan.

## Contract outcome: no new contract

Zero in-band Horde-only accepts exist on 1427: the 18 Kargath records
are Badlands content (8 contracted there, 10 above-band OUT there) and
8998 is above-band with its accept outside any contractible home open
to this round. This census doc is the deliverable that closes the
Searing Gorge (Horde) section — no `searing-gorge-horde` contract entry,
no micro-guide. Regression baseline moves only by the parallel
Badlands (Horde) addition (13 quests), reported explicitly in this
round's regression output.

## BORDERLINE (argued, none decided silently)

1. **Kargath dual-frame points.** Taken at face value, 18 Horde quests
   "touch" 1427. The coordinates + qzone settle it: one camp, two
   frames, qzone 1418 throughout. Counting frames instead of camps
   would double-contract Badlands content — the accept rule keys on
   where the quest is, not on how many map frames render its giver.
2. **8998 vs the Orgrimmar addendum.** The addendum shape (Undercity
   1899 precedent) requires a city accept. 8998's accept is Bodley, so
   the shape does not apply; a turn-in-only addendum would contradict
   the accept rule every city census applied. Ruled OUT with the
   symmetric-with-8997 pointer instead of silently dropping it.
3. **88 vs 81.** The 7-record delta is the sourceless-start set, each
   named above with its existing disposition. No record disappears.
