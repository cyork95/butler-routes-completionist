# Winterspring census (pack butler-routes-completionist)

Census from local Forever game data (questie-forever quests/npcs/objects/items.json),
built with `--product wowf` + QuestieDB. Accept-zone key **1452** (verified: the
map key carrying Everlook, Donova Snowden, Jaron Stoneshaper, Wynd Nightchaser,
Ranshalla, Haleh, Lorax, the Donova/Winterfall mob sets and the Kel'Theril ruin
objects; 78 giver/object candidates accept here, plus 4 item-start discoveries).

Method (settled): a quest belongs to the zone if its accept/start is on 1452 —
giver spawn, start object, or an item whose drop source spawns in-zone. Chains
ending outside are IN; objectives in-zone with accept elsewhere are OUT.
Item-started quests (including rare-drop starts) are IN. Race masks: null and
Alliance neutral IN; Horde-only OUT (set aside below). No class, skill, event,
pre, excl or next field anywhere bars an IN quest from gating — gates are
per-line in the guide.

## Band: 47-60

Lowest contracted minLevel 47 (Donova's opener pair 3909/3912, genuine
early-zone content leading into the 52 cluster) to highest contracted quest
level 60. Bulk floor is effectively 50 (ten quests); nothing sits above the
band. The six custom quests with null minLevel (levels 56-60) are treated by
quest level and sit inside the band — argued in BORDERLINE.

## Named check 1 — Felwood set-asides (all OUT, all already contracted)

| ID | title | accept location (data) | Felwood? |
|----|-------|------------------------|----------|
| 6031 | Runecloth | Meilosh @1448 Timbermaw Hold + @1452 border point | yes |
| 6032 | Sacred Cloth | Meilosh, same dual spawn | yes |
| 6241 | Winterfall Activity | Salfa @1448 + @1452 border point | yes |
| 8461 | Deadwood of the North | Nafien @1448 + @1452 border point | yes |
| 8462 | Speak to Nafien | Grazle @1448 only (pure Felwood accept) | yes |
| 8464 | Winterfall Activity | Salfa, same dual spawn | yes |
| 8471 | Winterfall Ritual Totem | item 20742, in-zone drops | yes |
| 5083 | Winterfall Firewater | item 12771, in-zone drops | yes |

Meilosh, Salfa and Nafien each hold one 1448 Timbermaw Hold spawn and one
1452 border spawn (25.6,31.9 / 27.73,34.5 / 24.9,36.2). All eight are
contracted in the Felwood guide, so the no-double-contract rule keeps them
there; they are set-asides here, and the bookkeeping closes. (8465, also
Felwood-contracted, and the repeatables 8467/8469 below, complete the
Timbermaw picture.)

## Named check 2 — Burning Steppes pre pair (both IN)

4810 Return to Tinkee (Felnok @1452, min50) and 4907 Tinkee Steamboil (Felnok
@1452, min57) both accept in Winterspring and fit the band — contracted here.
Their chain reads whole across the guides the Alterac way: 4809's pre 4808 is
Burning-Steppes-contracted (reference note), and 4810/4907 turn in at Tinkee
@1428. The Steppes guide's structural warnings stand as cross-guide notes, but
the chain is now completable end to end.

## IN - 48 quests

Everlook hub: 969, 975 (Mau'ari; pre 6606/969), 977, 3783, 5163, 8798
(Umi chain; 8798 skill-gated Engineering), 4809, 4810, 4907 (Felnok),
6603 (Meggi → Donova), 6606 (Harlo → Mau'ari), 5124 (Malyfous, skill-gated
Blacksmithing, structural pre 5103), 5126 (Lorax, only Warrior/Paladin/Shaman
+ Blacksmithing), 5127 (Lorax, skill-gated Blacksmithing), 5305, 5306, 5307
(Lilith/Kilram/Seril, skill-gated Blacksmithing, dungeon-fetched objectives),
5601 (Jessica → Pamela @WPL), 6028 (Gregor → Pureheart @EPL, Alliance),
6030 (Gregor → Duke @WPL, neutral), 92009 (Nami → Kaylaena @2482, pre outside),
92859, 98462 (Evie Shroud twins), 93269 (Vizzie → Sebelia @2482),
93406 (Vizzie, pre outside), 97490 (Umaron, Hailspite in-zone).
Donova west: 3909 (pre outside, contracted), 3912, 4842 (pre outside,
contracted), 5082 (pre 6603), 5084 (pre Felwood-contracted), 5086
(pre Felwood-contracted), 5087, 5121 (High Chief in-zone), 5123 (item-start
Crudely-written Log, sole dropper the Chief @100%), 5128 (→ Kelek @Felwood).
Southwest: 4861 (Jaron → Damaged Crate object), 4863 (Crate → Wagon object),
4864 (Wagon → Jaron), 6604 (Harlo → Jaron), 5244 (Wynd; pres Felwood-contracted
+ outside), 5245 (Jaron → Aurora @WPL), 5252 (Remorseful → Wynd, pre
WPL-contracted), 5253 (Wynd → Fandral @Darnassus).
Southeast/south: 4901 (Ranshalla → Erelas @Teldrassil, pre via soft-pre mini),
5161 (Haleh, structural pre 5160), 5162 (Haleh → Jeziba @EPL),
6502 (Haleh, skill-neutral, UBRS-fetched objective).

## OUT - 38 quests

Horde-only (7, set aside for the Horde block with IDs): 6605 (The Enraged
Wildkin, Harlo), 5054/5055/5056/5057 (Storm Shadowhoof chain), 6029 (Everlook
Report, Horde end), 4882 Guarding Secrets (item 12558, in-zone owlbeast drops
@50% — sourcing for the Horde block: 7452/7453/7454).
Repeatables (16): 4801-4807 (the seven E'ko turn-ins), 4970, 5201, 5981
(Rivern chain), 5063, 5067, 5068 (Argent catalogue chain), 8467, 8469
(Timbermaw tails), 9266 Making Amends.
Seasonal/event (2): 8672, 8726 (Lunar Festival, event 7).
Broken/unplaced (3): 5047 (Pip Quickwit has no spawn anywhere), 5103 (Human
Remains object has no spawn anywhere), 5160 (Awbee has no spawn anywhere).
Contracted elsewhere (10): the eight Felwood quests above + 8465 (Felwood) +
84399 Ka-Boom! (Stormwind-contracted; its Winterspring book object is a remote
accept of a Stormwind quest).

## BORDERLINE

1. **Band 47-60.** Literal lowest contracted minLevel (47) to highest contracted
   quest level (60). Bulk floor is 50; the Donova opener pair at 47 is genuine
   early-zone content, not an outlier, so no outlier machinery. Null-minLevel
   customs (levels 56-60) treated by quest level, all inside. Nothing above-band.
2. **Repeatables are OUT even where they sting.** The E'ko turn-ins (4801-4807),
   the Rivern chain, the Argent catalogue and the Timbermaw tails are all
   flagged repeatable in the data — the rule fires regardless of chain charm.
   The guide notes the E'ko turn-ins at Mau'ari and the Horde-variant 6029 at
   Gregor so players know what was left out and why.
3. **6028/6030 vs 6029.** Same giver, three faction ends: 6028 ends Alliance,
   6029 Horde-locked (races flag), 6030 neutral. Contract the two an Alliance
   player can turn in; 6029 is a Horde set-aside. No mutual-exclusion issue in
   the data (separate quest records, no excl links).
4. **5126 classes=67.** Bitmask decodes to Warrior+Paladin+Shaman (single bits
   1/2/64 confirmed against known single-class quests), so `only
   Warrior,Paladin,Shaman` plus the Blacksmithing skill gate. Only two quests
   in the DB carry 67 (5126, 95217); both skill-gated the same way.
5. **5124/5161/5162 contracted despite unobtainable pres.** 5103's start object
   and 5160's giver have no spawn anywhere in the data, so the pres can never
   be taken — but 5124/5161/5162 themselves accept from placed Everlook NPCs.
   Contracted with honest structural pre notes (nothing invented); if spawn
   data appears, the pres route normally.
6. **4901/93406/92009/5244 soft-pre minis.** Their blocking pres (978, 93197,
   92008, 5250) accept outside any contract but turn in here (Ranshalla,
   Vizzie, Nami, Wynd) — each gets a dedicated `when onquest` mini-step
   carrying its in-zone turn-in (and 979's accept at Erelas), the Arathi-79975
   pattern. 978's own pre 3661 (Erelas, Teldrassil-side, uncontracted) is noted
   as the chain's true start: without it the mini skips cleanly.
7. **Cross-guide contracted pres are reference notes, not warnings.** 3909 ←
   3908 and 4842 ← 980 (both Ungoro-contracted), 4809 ← 4808 and 4810/4907
   chain (Burning-Steppes-contracted), 5084 ← 5083 and 5086 ← 5085
   (Felwood-contracted), 5244 ← 5249 (Felwood), 5252 ← 5248 and 6502 ← 6501
   (WPL/Stormwind-contracted): the guides that own the pres turn them in; this
   guide just points at them.
8. **Dungeon-interior objectives have no data placement.** 5305/5307/5127 (BRD
   NPCs), 5306 (Sunken Temple), 6502 (UBRS) target NPCs with zero spawns
   anywhere — dungeon interiors are not in the spawn data, and no entrance
   object carries a spawn either. Per the standing rule (never invent coords)
   their completes ship as honest note-only dungeon namings, the BS-4241
   precedent — not at invented entrances. Expected lint class: "no earlier
   goal gets X" on five turn-ins, argued here.
9. **3909/5086 fetch outside the zone.** Videre Elixir drops solely from Gregan
   Brewspewer @1444 Feralas; Toxic Horror Droplet solely from Toxic Horror
   @1448 Felwood (@80%) — both ride grouped expedition completes in their
   zones. 5163 splits three ways: Legacki in-zone, Sprinkle @1446 Tanaris,
   Quixxil @1449 Un'Goro.
10. **5244's dual pre.** 5249 contracted in Felwood (reference), 5250
    uncontracted Teldrassil-side (above Teldrassil's band, correctly out there).
    The pack treats multi-pre accepts normally (Zephras 92515 precedent);
    5250's turn-in rides a `when onquest` mini at Wynd, and any residual
    structural warning is accepted.
11. **2482 legs are real.** `zone map 2482` is established pack dialect
    (Blasted Lands/Felwood/Stormwind/Ungoro guides); Kaylaena and Sebelia share
    the point 70.87,51.55. 92009's timed-delivery event objective and 93269's
    delivery turn-in ride one grouped 2482 leg (R1 residue accepted).
12. **No above-band, no twin IDs, no city-rule cases.** The Timbermaw dual
    spawns resolve to Felwood contracts (named check 1); nothing else is dual.
