# Barrens (Alliance) census (pack butler-routes-completionist)

Source: local Forever game data (questie-forever quests/npcs/items/objects.json),
built with `--product wowf` + QuestieDB. Accept-zone key **1413** (verified:
the Horde census's own key; Ratchet sits on the zone map - the Booty Bay
precedent - so its accepts are zone content, per the standing ruling).
Alliance addendum route. Game data wins throughout.

Method (settled): a quest belongs to this addendum if it accepts/starts on
1413 and is available to Alliance players, and it is not already contracted
anywhere (no double-contract). Horde route: IN = Horde or neutral (fac
HORDE/ALL); Alliance-only (races 4294967373, Alliance+Skyborne) = set aside.
Null-mask records are shared, never duplicated - they stay in
`barrens.guide`, which this round does not touch. Race bitmask read off the
races field (4294967373 Alliance IN, 8589934770 Horde OUT, null shared).

## The banked Alliance set-asides (17, reconciled one by one)

| ID | title | lv/min | accept (1413 placed point) | ruling |
|----|-------|--------|----------------------------|--------|
| 1040 | Passage to Booty Bay | 30/25 | Wharfmaster Dizzywig (3453) @63.35,38.45 Ratchet | IN |
| 1252 | Lieutenant Paval Reethe | 40/30 | object Theramore Guard Badge (21042) @51,79 | IN |
| 1253 | The Black Shield | 35/30 | object Black Shield (20992) @50.9,79.1 | IN |
| 1284 | Suspicious Hoofprints | 35/30 | objects Hoofprints (21015/21016) @50.9,78.7 / @50.9,78.6 | IN |
| 1287 | The Deserters | 38/30 | Balos Jacken (5089) @54.2,82.1 (dual 1445 @36.09,54.31) | IN |
| 1738 | Heartswood | 20/20 | Takar the Seer (6244) @49.31,57.1 | IN, only Warlock |
| 1758 | Tome of the Cabal | 30/30 | Strahad Farsan (6251) @62.63,35.5 Ratchet | IN, only Warlock |
| 3370 | In Nightmares | 25/15 | Falla Sagewind (8418) @48.18,32.78 | IN |
| 3634 | Gnome Engineering | 47/30 | Tinkerwiz (3494) @62.67,36.31 Ratchet | IN, profession (skill 202) |
| 3861 | CLUCK! | 1/1 | Chicken (620), 10 placed 1413 points (e.g. 60.76,55.49, 61.29,53.53) | IN (named check 1) |
| 8268 | Ribbons of Sacrifice | 39/10 | Captain Shatterskull (14781) @46.6,8.41 | OUT battleground |
| 65602 | What Is Love? | 20/20 | Takar the Seer (6244) @49.31,57.1 | IN, only Warlock |
| 94375 | Call of Earth | 4/4 | Minor Manifestation of Earth (5891) @68.2,36.9 | IN, only Shaman (named check 4) |
| 97005 | Chol'aruk the Ravener | 21/15 | Bainham (267309) @61.88,39.44 Ratchet | IN |
| 98903 | The Battle for Darkspear Islands! | 39/30 | Brelinda McFarry (275273) @63.36,58.77 | OUT battleground |
| 98904 | The Battle for Darkspear Islands! | 49/40 | Brelinda McFarry (275273) @63.36,58.77 | OUT battleground |
| 98905 | The Battle for Darkspear Islands! | 60/50 | Brelinda McFarry (275273) @63.36,58.77 | OUT battleground |

IN 13, OUT 4. Every one of the 17 is ruled above; nothing banked is left
unaccounted.

Chain notes (all verified in this data build): 1040 pre 1039
(darnassus-city) > 1040 > next 1041 (stranglethorn-vale); 1252 preAny
1302 (wetlands) / 1282 (dustwallow-marsh), one of the pair required,
> next 1259
(dustwallow-marsh); 1253 > next 1319 (dustwallow-marsh); 1287 pre 1286
(dustwallow-marsh) > next 1288 (dustwallow-marsh); 1738 pre 1716
(stormwind-city) > next 1739 (stormwind-city); 65602 pre 1716 shared >
next 65603 (stormwind-city); 1758 pre 1798 (stormwind-city,
ironforge-city) > next 1802 (ironforge-city); 3370 pre 6981
(the-barrens, main guide) and 6981's own pre chain stays main-guide's;
3634 > next 3640 (ironforge-city); 94375 pre 94374 (dun-morogh, whose
pre 94373 is also dun-morogh). Contracted pres ride soft-pre minis in
the addendum guide; contracted nexts get handoff notes, never
duplication. 1252/1253/1284's preAny pair (1302 wetlands /
1282 dustwallow-marsh) is required-one-of per the data and the forge
check - the guide notes name both home guides at each accept rather
than a soft-pre mini (no OR-guard exists).

## Full-scan check ("no others" - claimed after the complete scan)

Alliance-mask sweep: every races=4294967373 record whose start NPC/object
spawns on 1413, plus every races=4294967373 record with zone=1413 - 17
records, exactly the banked set above. No others.

Non-standard mask sweep (Alliance subsets / Horde subsets / race+class
gates touching 1413): 854/6361/6362 (Tauren), 6365/6384 (Orc/Troll),
1524 (Shaman-gated), 6128/6129 (Druid-gated) - all already contracted in
the-barrens. One uncontracted record: 1946 Nether-lace Garment
(lvl26/min26, races Orc/Undead/Troll, class Warlock, above-band) - Horde
race-gated, not Alliance business, stays out (BORDERLINE B8).

Item-start scan (explicit, over the whole Alliance pool): no
Alliance-mask quest carries a start item whose giver context touches
1413 (all 60 Alliance item-start records home elsewhere). Drop-source
scan (start item dropping from a 1413-spawning NPC/object): exactly one
hit - 1100 Lonebrow's Journal (item 5791 from object 19861, 1413 point
[43.5,93.1] far-south spill) - already contracted in thousand-needles,
which owns it (361/635 precedent: the drop zone does not claim the
quest). No double-contract. The scan is complete; nothing asserted
without it.

## Named check 1 - 3861 CLUCK! (IN, Barrens-homed)

The Tirisfal census flagged 3861 as Westfall-homed (zone field 1436) and a
candidate for a future Westfall addendum. Accept geography in THIS data
build decides: Chicken (620) has 10 placed spawn points on 1413 (Ratchet
cluster 60.76,55.49 / 61.29,53.53 plus 61.63,23.74) beside its 24 on
1436. Per the brief's rule the Barrens spawn makes it Barrens content -
IN here, and the Westfall pointer is discharged with this note (a future
Westfall addendum must not re-contract it). The repeatable=true flag in
the data is no bar: 64 already-contracted pack records carry it
(813/822 Chen's Keg in the main guide among them), and 8993 (also
repeatable=true) is contracted in silverpine-forest-alliance - the flag
does not mark pack-repeatable content. No pre, no next, ends at the
chicken itself. Objective item Special Chicken Feed (11109) is a vendor
buy from Farmer Saldean (233, Westfall 1436) - ride a bag/vendor note,
never an invented point.

## Named check 2 - the Darkspear Islands trio (OUT, all three)

98903/98904/98905 (min30/40/50, lvl39/49/60): three same-name tiered
records, each on its own record. Ruled OUT as battleground-bracket
content, not three one-time quests: objective text "Win a Darkspear
Islands battleground" on all three (instanced PvP, B5 precedent - the
zone guides cover open-world quests; WSG brackets 8368/8389 stay out at
min19/10 the same way). Bracket shape (tiered min30/40/50 = bracket
pattern, cf. the Darkspear 98887-98891 brackets and WSG/AB tiers, all
OUT), and 98904/98905 carry EMPTY end lists - incomplete records, a
second independent reason. The Horde twins 98906/98907/98908 (giver
275276) are likewise uncontracted anywhere. No event or repeatable flag
is needed for the call; the battleground-objective + bracket + empty-end
evidence states it.

## Named check 3 - 3370 In Nightmares (IN, Darnassus expedition)

B11 settled the masks: 3369 is Horde (contracted in the main guide's
chain), 3370 is Alliance (races 4294967373). 3370 accepts at Falla
Sagewind (1413 @48.18,32.78), pre 6981 (contracted in the main guide -
soft-pre mini), ends at Mathrengyl Bearwalker (4217): spawns Teldrassil
1438 @24.6,48.7 and Darnassus 1457 @35.37,8.4; objective text "Bring the
Nightmare Shard to Mathrengyl Bearwalker in Darnassus" picks the
Darnassus point. CORRECTION to the round brief: the data does not end
this quest at Delgren in Alterac - the expedition leg rides to Darnassus,
and the guide is written that way. 3369 is not touched.

## Named check 4 - 94375 Call of Earth (IN, only Shaman)

Level-4 Shaman record (races Alliance+Skyborne, class 64) with a 1413
accept: Minor Manifestation of Earth (5891) spawns exactly one placed
point per starting map - 1411 @44.03,76.2, 1412 @51.99,80.4, 1413
@68.2,36.9, 1426 @24.84,61.86. The 1413 point is the same shape as the
other three (not noise), and the Horde twins 1518/1521 start at this same
NPC with the same 4-map spawn and are contracted IN the main guide - the
pack already treats the 1413 manifestation as a Barrens accept. So 94375
genuinely accepts in the Barrens for Alliance Shamans: IN, gated only
Shaman (the addendum header carries the Alliance faction). Pre 94374
(Teo Hammerstorm, Dun Morogh) is dun-morogh-contracted - soft-pre mini
completing at the Barrens manifestation point; 94375 itself ends back at
Teo in Anvilmar (1426 @28.79,66.18), a Dun Morogh expedition leg. The
zone field (1411) does not home it anywhere - accept geography rules, as
always. It is not a starting-zone anchor: the Dun Morogh leg of its own
chain (94373/94374) is already contracted there, and this record's
accept sits on 1413.

## OUT detail (the 4)

- 8268 Ribbons of Sacrifice (lvl39/min10, excl-twin 8267 Horde,
  uncontracted): OUT. Objective item "Warsong Gulch Ribbon of Sacrifice"
  (20256, sourceless - no droppers, no vendors) + excl-linked Horde twin
  + WSG-named objective = battleground turn-in content, B5 precedent
  (instanced-PvP stays out even where minLevel sits in band). The Horde
  twin 8267 is likewise uncontracted.
- 98903/98904/98905: OUT per named check 2 (battleground brackets +
  empty enders on 98904/98905).

## Span

Contracted records run min1 (3861) to min30 (1252/1253/1284/1287/1758/
3634), levels 1-47 (3634). Addendum band "1-47": the pool's min1-min50
range contracts to a min1/min4 opening (3861, 94375), a min15-25 middle
(3370 min15, 1738/65602 min20, 97005 min15, 1040 min25) and a min30 top
(Theramore chain, warlock Tome, Gnome Engineering).

## BORDERLINE (every unsure call argued, none decided silently)

B1 - 3861 vs Westfall + repeatable flag: IN, argued in named check 1.
The chicken's 10 Barrens points are placed Ratchet-cluster spawns, not
spill; the quest has no pre/next/event and ends where it starts. The
Westfall addendum pointer from Tirisfal is discharged here, not carried.

B2 - Darkspear trio one-time vs bracket: OUT, argued in named check 2.
A same-name twin rule would route variants, but battleground content is
out of scope for zone guides on both factions; the empty enders on
98904/98905 close the case.

B3 - 3370 destination vs brief: data wins (Darnassus, not Alterac),
argued in named check 3. The guide carries the Darnassus expedition; the
brief's Alterac leg is not written anywhere.

B4 - 94375 starting-zone anchor vs Barrens accept: IN, argued in named
check 4. Single-point-per-map manifestation pattern + Horde-twin
precedent (1518/1521 main-contracted) make the 1413 point genuine.

B5 - 65602 What Is Love? (seasonal name, no seasonal data): IN. No
event flag, no repeatable flag, class-gated Warlock chain link with a
contracted pre (1716) and contracted next (65603) - exactly the shape of
1512 Love's Gift, which the main census kept IN as "seasonal-named but
class-chained" (B7 there). Title alone does not exclude; the data shows
a genuine chain link. Objective item Wooden Figurine (190309) sources
from object 375544 (Ashenvale 1440 @26.61,22.03) - an Ashenvale
expedition complete with a placed point, not a bag note. Same for 1738:
Heartswood (6912) from object 93192 (Ashenvale @31.55,31.57).

B6 - Above-band top (min30s, lvl35-47) in a 10-25 zone's addendum: IN.
The addendum's span is its own (silverpine-forest-alliance precedent:
min24/lvl33 trio in a 10-20 zone). The min30 wall belonged to the Horde
band call (B1 there); faction-exclusive content above the zone band
still belongs to someone, and that someone is this addendum.

B7 - Dual-map Theramore objects (21042/20992/21015/21016 on 1413+1445)
and Balos Jacken (1413+1445): the Barrens claims the ACCEPT (placed
1413 points: badge @51,79, shield @50.9,79.1, hoofprints @50.9,78.7/78.6,
Balos @54.2,82.1); turn-ins and follow-ups (Vimes; 1259/1319/1288) stay
dustwallow-marsh's - verified contracted, never duplicated.

B8 - 1946 Nether-lace Garment (non-standard mask sweep): OUT. Races
Orc/Undead/Troll + class Warlock + min26 above-band: Horde race-gated,
not Alliance business; no Alliance addendum claims it. Noted so nobody
hunts it.

B9 - 1100 Lonebrow's Journal (item-start scan hit): OUT here, stays
thousand-needles'. The 1413 drop point is far-south border spill; home
zone owns (361/635 precedent).

B10 - 8268 min10 vs lvl39: the level spread does not save it - WSG
content is out at any level (8368/8389 precedent at min19/10).
