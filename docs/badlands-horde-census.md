# Badlands (Horde) census (pack 0.126.0)

Source: local Forever game data (questie-forever `quests.json`, built with
`--product wowf` + QuestieDB). Accept-zone key **1418** (the key the
Alliance census used): 77 quest records carry `zone: 1418` — 35 Horde-mask
(`races: 8589934770`), 13 Alliance-mask (`races: 4294967373`), 29 null-mask
(shared/neutral). The 35 Horde records are exactly the 35 banked set-asides;
no Horde-mask record on key 1418 falls outside the banked list. No record
in the pool carries a class restriction; the only profession gates are
skill 165 (Leatherworking, on 5145) and skill 171 (Alchemy, on 2203).

## Band: 30–40

Horde minLevels over the 13 IN records: min30 ×3 (728, 1419, 1420 —
Theldurin's digest pass-through and the Neeka Bloodscar on-ramp),
min36 ×2 (2258, 2202 — the Jarkal Mossmeld reagent chain),
min37 ×4 (2318, 2338, 2339, 2340 — the Translating the Journal necklace
chain), min40 ×4 (782, 793 — the Broken Alliances Thor finales; 2203 —
the Alchemy-gated reagent finale; 5145 — the Leatherworking finale).
Finale levels run to L55 (5145) with minLevel in band, so all IN per the
minLevel rule. Mirrors the Alliance 28–40 without copying it: the Horde
floor is min30 (no Martek on-ramp on this side) and the Horde ceiling is
min40 with nothing between min40 and the min48 Kargath upper cluster.

## IN ledger (13)

Kargath / Dustbowl NW cluster (all givers spawn on 1418):
- 1419 L40 Coyote Thieves (min30) — Neeka Bloodscar (6.49, 47.2);
  30 Coyote Jawbone (Crag Coyotes 2727/2728/2729/2730, central grounds).
- 1420 L40 Report to Helgrum (min30, pre 1418 — the Swamp-of-Sorrows
  record Neeka Bloodscar, in NO contract) — Neeka Bloodscar; no
  objectives; ends at Helgrum the Swift (Swamp of Sorrows 47.74, 55.2):
  expedition turn-in. Accept rides a dedicated `when onquest 1418`
  mini-step.
- 2258 L39 Badlands Reagent Run (min36) — Jarkal Mossmeld (2.42, 46.06);
  5 Buzzard Gizzard (2829/2830/2831) + 10 Crag Coyote Fang (same coyotes
  as 1419) + 5 Rock Elemental Shard (92/2735/2736/2745/2752/2791).
  Next: 2202.
- 2202 L42 Uldaman Reagent Run (min36, pre 2258) — Jarkal Mossmeld;
  12 Magenta Fungus Cap (Magenta Cap Clusters 126049, north grounds
  33–37, 12–24). Next: 2203.
- 2203 L44 Badlands Reagent Run II (min40, pre 2202, skill 171 =
  Alchemy) — Jarkal Mossmeld; 3 Vessel of Dragon's Blood (2726 Scorched
  Guardian, 12 pts east grounds 77–80, 47–53). Profession record:
  `optional` + `when skill Alchemy 1` in the guide.
- 2318 L42 Translating the Journal (min37, pre 2284 — Necklace Recovery,
  Take 2, Orgrimmar-contracted) — Remains of a Paladin (6912, NO placed
  spawn anywhere in the data: sourceless accept, R2-style honest note,
  accept + note, never wedges); no objectives; ends at Jarkal Mossmeld.
  Accept rides a dedicated `when onquest 2284` mini-step. Next: 2338.
- 2338 L42 Translating the Journal (min37, pre 2318) — Jarkal Mossmeld;
  no objectives (talk-through). Next: 2339.
- 2339 L44 Find the Gems and Power Source (min37, pre 2338) — Jarkal
  Mossmeld; 4 gem collects, ALL with no placed source anywhere in the
  data: 7669 Ruby (Shadowforge Cache 113757, zero spawns), 7670 Sapphire
  (Grimlok 4854, zero spawns), 7671 Topaz (Conspicuous Urn 125477, zero
  spawns), 7672 Power Source (Archaedas 2748, zero spawns). IN with
  honest collect lines + notes naming the gap (mid-chain R2/R3-analog
  residue, argued in BORDERLINE 4). Next: 2340.
- 2340 L44 Deliver the Gems (min37, pre 2339) — Jarkal Mossmeld; no
  objectives; ends at Dran Droffers (Orgrimmar 59.49, 36.57): expedition
  turn-in. Next: 2341 (Necklace Recovery, Take 3, Orgrimmar-contracted —
  chain-end handoff note).

Thor chain (Gorn, far west 2.91, 45.6):
- 782 L43 Broken Alliances (min40, no pre) — Gorn; 1 Sign of the Earth
  (sole dropper 2944 Boss Tho'grun, 1418 point 12.62, 75.49). Next: 793.
- 793 L50 Broken Alliances (min40, pre 782) — Gorn; Blacklash's Bindings
  (2757 Blacklash, 1418 point 81.88, 49.46) + Chains of Hematus (2759
  Hematus, 1418 point 82.03, 49.93). Next: 795 (repeatable, OUT —
  chain-end handoff note).

Theldurin the Lost (south camp 51.39, 76.87):
- 728 L40 To the Undercity for Yagyin's Digest (min30, pre 709 —
  Solution to Doom, neutral, Alliance-contracted, stays shared after
  ungating) — Theldurin the Lost; no objectives (carry-through); ends
  at Keeper Bel'dugur (Undercity 53.74, 54.46): expedition turn-in.
  Accept rides a dedicated `when onquest 709` mini-step. Next: 736
  (The Star, the Hand and the Heart, Undercity, in NO contract —
  chain-end handoff note).

Dragonscale outpost (Thorkaf Dragoneye, east 62.7, 57.4):
- 5145 L55 Dragonscale Leatherworking (min40, no pre, skill 165 =
  Leatherworking) — Thorkaf Dragoneye; 2 Tough Scorpid Breastplate +
  2 Tough Scorpid Gloves (BOTH crafted turn-ins, no source anywhere in
  the data: R5-style honest craft note) + 10 Worn Dragonscale (2725
  Scalding Whelp, 24 pts east grounds 69–72, 51–64). Profession record:
  `optional` + `when skill Leatherworking 1` in the guide. Mutually
  exclusive with 5146 (Elemental, Arathi zone 1417) / 5148 (Tribal,
  STV zone 1434) — neither in this zone's data; exclusivity noted here
  and in the guide (Named check 1).

## Named-check rulings

1. 5145 Dragonscale Leatherworking: IN — accepts in-zone for Horde
   players from a placed giver, min40 in band, no pre. Rides `optional`
   + `when skill Leatherworking 1` with an exclusivity note (5146
   Arathi-contracted per the Arathi round; 5148 in STV's data). The
   2×8203 + 2×8204 objectives are crafted turn-ins with no data source
   (R5 residue); the 10×8165 farm in-zone.
2. 97663 Supplies and Studies: re-examined in full against the current
   data and ruled OUT broken, closing the Alliance census flag. The
   record is unchanged: `minLevel: null`, `objectives: []`, start/end
   NPC 269647 Mus'hale (whose spawn IS placed: 1418 point 4.09, 46.22 —
   Kargath), with an objectiveText that reads real (Dustbowl ogres,
   stone etchings). A placed giver plus real text is not a runnable
   quest with no objectives and no band position. Stays OUT; revisit if
   the record ever gains objectives. (Also null-mask — if fixed, it
   belongs to the main guide, not this contract.)

## Item-start enumeration (explicit scan of all 35)

Start items appear on exactly one record: 4903 Warlord's Command (item
12563, which itself has no source anywhere in the data) — OUT
above-band (min55), so the scan changes nothing. Start objects appear on
exactly three records: 795 Seal of the Earth (object 2933, placed
1418 at 81.52, 49.94) — OUT repeatable; 4081 KILL ON SIGHT (object
164867 WANTED poster, placed 1418 at 3.74, 47.43) and 4082 (object
164868, placed 3.94, 46.73) — both OUT above-band (min48/50). **No
item- or object-starts among the IN 13** — stated after the scan, not
assumed (Mulgore lesson held).

## OUT list

Repeatable (1): 795 Seal of the Earth (L55/min40, Horde) — `repeatable:
true` (the Thor chain's turn-in cycle; parent 793; start object 2933
placed, all three runestone objectives placed: 4845 Diamond ← Pillar
of Diamond 2842 at 83.54, 32.84; 4844 Opal ← Pillar of Opal 2848 at
72.32, 66.94; 4843 Amethyst ← Pillar of Amethyst 2858 at 81.33, 64.28).
The one-time chain (782->793) is contracted without it — the exact
parallel of the Alliance 779 ruling.

Above-band (20, all min48+): min48 — 3821 Dreadmaul Rock, 3906
Disharmony of Flame, 3907 Disharmony of Fire, 3981 Commander Gor'shak
(ender Gor'shak 9020 spawnless; next 3982 in no contract), 4081 KILL
ON SIGHT, 7201 The Last Element; min50 — 4082 (pre 4081), 4134 Lost
Thunderbrew Recipe (pre 4133, Undercity, in no contract); min52 —
4061/4062/4063 The Rise of the Machines (4062 ends at X'anth in the
Searing Gorge 1428; 4063 accepts in-zone at Lotwil but min52),
4122 Grark Lorkrub (ends at Grark in 1428; pre 4082), 4132 Operation:
Death to Angerforge (pre 4121, in no contract); min55 — 4724 The Pack
Mistress, 4903 Warlord's Command (item-start 12563 sourceless), 4941
Eitrigg's Wisdom (ends at Thrall, Orgrimmar; next 4974 in no
contract), 4981 Operative Bijou (ender Bijou 10257 spawnless), 4983
Bijou's Reconnaissance Report (sourceless accept at Bijou; pre 4982 in
no contract), 98325 Blood and Thunder; min57 — 4768 The Darkstone
Tablet (pre 4769, in no contract).

Accepts outside the zone (1): 3822 Krom'Grul (L53/min48) — accepts at
Sha'ni Proudtusk in the Searing Gorge (1428), not Badlands content
(also above-band; primary reason is the accept geography).

Alliance-only set-asides for the record (13, none duplicated here):
706, 717, 718, 719, 720, 721, 724, 727, 732, 733, 739, 97617 (all 12
in the main guide's contract) + 779 Seal of the Earth (Alliance
repeatable turn-in leg, in no contract — the 779/795 parallel).
Null-mask records stay in the main guide's contract (23: 656, 692, 703,
705, 709, 710–716, 734, 777, 778, 1108, 1137, 1559, 2418, 94256, 94268,
94292, 94304) or out per the Alliance census (6: 2278 broken — accept
object 131474 zero spawns; 4136/4729/4862 above-band min48/55/55;
97663 broken — this census; 97821 broken — no accept at all).

## BORDERLINE (argued, none decided silently)

1. 795 OUT as repeatable while 782->793 stay IN: `repeatable: true` is
   set on the record (verified, not inferred from the name). The Seal
   object and all three runestone pillars are placed and the chain is
   otherwise runnable — this is the repeatable rule's exact target
   (the 779 parallel), not a data gap. If the flag ever clears,
   795 walks straight into this contract (min40, in-zone accept).
2. Band top min40 with L43–L55 finales (782 L43, 793 L50, 2203 L44,
   5145 L55): IN per the minLevel rule — finale levels above the band
   with minLevel in band are the rule's core case, not an exception.
3. 2318 IN with a sourceless accept: Remains of a Paladin (6912) has no
   placed spawn anywhere, but the quest is a talk-through link (no
   objectives) between the Orgrimmar-contracted 2284 and the in-zone
   2338. Excluding it would sever the chain; the R2 honest-note shape
   (accept + note, never wedged) covers it exactly.
4. 2339 IN with four sourceless collects: all four gem objectives lack
   any placed source (two spawnless Uldaman bosses, two spawnless
   cache objects). Same call as 2318 at larger scale — the chain is
   genuine in-zone content (accept + turn-in at Jarkal), so the census
   contracts it and the guide carries the gap in writing rather than
   dropping the chain's center.
5. 3822 OUT on accept geography first, band second: Krom'Grul accepts
   in the Searing Gorge even though its pre (4082) is Badlands content.
   It belongs to the Searing Gorge (Horde) round's pool, recorded here
   so that round picks it up.
6. 7321 Soothing Turtle Bisque (Horde, Cooking, min28) is NOT in this
   contract: its record carries zone 1416, not 1418 (the Alterac round's
   expectation per the Alliance census note — that round reconciles key
   1416 and rules on it). Recorded here so the ID is not lost between
   rounds.
7. Profession gates (2203 Alchemy, 5145 Leatherworking) ride
   `optional` + `when skill`, never bare and never dropped: the gate is
   what the data gates (skill fields 171/165, verified against
   Elixirs-for-the-Bladeleafs and the Leatherworking armor records).
8. Out-of-contract pres inside IN chains (709 neutral contracted,
   2284 Orgrimmar-contracted, 1418-quest uncontracted): the guide
   bridges each with a dedicated `when onquest` mini-step; uncontracted
   chain-exits (736, 2341 Orgrimmar-contracted, 795 repeatable) get
   handoff notes, never silent ends.
