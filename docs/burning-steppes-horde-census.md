# Burning Steppes (Horde) census (game data, accept-zone key 1428)

Accept-zone key: **1428** (verified by count: 52 quest records carry
`zone=1428` in this data build - the same key and the same count the
Alliance census (`docs/burning-steppes-census.md`) examined). Race
masks in the data: 8589934770 = Horde, 4294967373 = Alliance, null =
neutral (both factions).

Method: every zone-1428 record examined against the packs inclusion
rules; the Alliance censuss 3 banked Horde set-asides reconciled one
by one (4121 Precarious Predicament, 3822 Krom'Grul, 8998 Back to
the Beginning); the full 1428 pool enumerated by races mask for Horde
records beyond the 3 (found: none - the pool holds exactly 1 Horde-mask
record, which is 4121); start-item AND start-object scan run over the
Horde set; pres/exclusives and outside legs resolved from data
(`npcs.json`, `objects.json`, `items.json`, `quests.json`, `spawnz.json`
cross-checked).

Pool breakdown: 1 Horde-mask + 50 Alliance-mask + 1 null (8961 Three
Kings of Flame, shared - checked, not Horde). The 2 named set-asides
live on other zone keys with Burning Steppes accept geography and are
ruled on their own records below.

## Band: 48-58

Contracted minLevels run 48 (3822 Krom'Grul) through 58 (8998 Back
to the Beginning), with 4121 at m52 between. With three records the
band rests on three points and says so: bottom m48 (Krom'Grul),
middle m52 (Precarious Predicament), top m58 (the Bodley finale).
Derived from the Horde records, not copied from the Alliance 48-60
(the Alliance top is 60, ours is 58 - both honest to their own pools).

No race header for the guide beyond faction: all three contracted
quests are Horde-mask, none is race-locked further. No class gates, no
profession gates, no skill-gated records (the pool scan found no CLASS
or SKILL flags on any of the three).

## IN (3)

Grark Lorkrub camp (Grark 9520 @40.2,34.24, in-zone single point):

| 4121 Precarious Predicament | 58/52 | pre 4122 Grark Lorkrub (Horde, zone 1418 Badlands, uncontracted anywhere - soft-pre mini below; its own pre 4081 uncontracted Badlands BRD chain is named, not routed) | ESCORT: Thorium Shackles item 11286 + event Prisoner Transport at (25.73, 27.1) on 1428; ends Lexlort 9080, Badlands (1418 @5.88,47.63) - Badlands expedition turn-in |
| `when onquest 4122` soft-pre mini at Grark (turn in 4122, accept 4121) - the pre turns in in-zone at the chains head (Kadrak pattern; 4122 accepts at Lexlort in the Badlands and lives outside every contract) |

Sha'ni Proudtusk camp (Sha'ni 9136 @79.95,45.4, in-zone single point - her ONLY spawn anywhere in the data):

| 3822 Krom'Grul | 53/48 | pre 3821 Dreadmaul Rock (Horde, zone 1418 Badlands, uncontracted - soft-pre mini below; no pre of its own) | 1 Sha'ni's Nose-Ring 11058 off Krom'Grul 8977 (100%, in-zone single point @79.66,47.43 next to Sha'ni); ends Thal'trak 9082-NPC, Badlands (1418 @3.36,48.1; also spawns 1427) - Badlands expedition turn-in |
| `when onquest 3821` soft-pre mini at Sha'ni (turn in 3821, accept 3822) - the pre turns in in-zone at the chain head (Kadrak pattern; 3821 accepts at Thal'trak in the Badlands and lives outside every contract) |

Bodley camp, Blackrock Mountain frame (Bodley 16033 @32.2,25.8 on the 1428 frame - one of his three placed spawns: 1415 @48.9,63.9, 1427 @39.8,96.5, 1428 @32.2,25.8):

| 8998 Back to the Beginning | 60/58 | pre 8996 Return to Bodley (shared, contracted in the MAIN guide - chain note, no mini; the 93045 pattern: the main guide serves 8996 through its own Bodley turn-in, and this guide names that leg) | no objectives (talk quest); ends Mokvar 16012, Orgrimmar (1454) - Orgrimmar expedition turn-in; the Horde finale of the Bodley chain the Searing Gorge round deferred here |

## OUT: none of the pool; noted non-contracted (homed or set aside with reason)

- Reverse scan (Horde-mask quests with 1428-spawning starters on other zone keys): only the two named set-asides above (3822 zone 1418, 8998 zone 1427) - no further Horde records start on this zone frame.
- The Alliance censuss Badlands trio + attunement twins + Bodley path + Dreadsteed chain are the main guides contracted content (shared or Alliance) - untouched here.
- 11 non-contracted Bodley variants (8963-8965/8967-8969/8986-8988/8991/8992): same set-aside as the Alliance census (mechanical twin-paths, argued there) - not Horde content, not contracted.
- 9032 Bodley's Unfortunate Fate (Horde, Org-contracted) and 8960 (Alliance, IF-contracted): the twin Bodley pres, each homed in its city guide - named, not duplicated. 8998s own pre is 8996 (shared), not these.
- 4082 KILL ON SIGHT (Horde, Badlands, uncontracted BRD chain via object-start 4081): 4122s pre-chain context, Badlands-homed, uncontracted anywhere - named for the record; a future Badlands addendum may take the 4081>4082>4122 shape whole, at which point 4121s mini gains a contracted pre and this census gets a pointer update.

## Item-start enumeration

Explicit start-item AND start-object scan over the Horde set (4121, 3822, 8998): all three accept from NPC givers (Grark 9520, Sha'ni 9136, Bodley 16033) - no item/object starts. The 8998 turn-in (Mokvar, Org) rides the existing Orgrimmar soft-pre line (untouched by this round). No sourceless bag-note cases: every objective item names a placed source (Thorium Shackles via the escort event; Nose-Ring 100% in-zone; 8998 has no objectives).

## BORDERLINE (all decided, none silent)

(a) 8998s zone home: its record key is 1427 (Searing Gorge) but its giver Bodley holds a placed 1428-frame point (32.2,25.8, Blackrock Mountain - the same frame the Alliance census contracts Bodley quests on, including the 8995>8996 spine). The accept geography decides per the Tirion dual-spawn precedent: a placed in-zone giver is an in-zone accept. The Searing Gorge round deferred exactly this decision here ("a Burning Steppes-side or endgame-round decision"); the data answers it - Blackrock Mountain frame, in-zone accept, Horde finale, m58 in-band: IN. If a future endgame round wants the whole Bodley path, this contract cedes 8998 with a pointer update.
(b) 3822s zone home (the Kargath mirror, decided the other way): the record is keyed 1418 (Badlands) but Sha'ni Proudtusk spawns ONLY on 1428 (single point @79.95,45.4 - verified exhaustive). The Badlands round kept 1418-keyed DUAL-frame records home by qzone; this record has no Badlands frame at all, so the qzone rule would orphan it (a Horde quest no Horde guide can route). The accept-geography rule (Tirion precedent, exercised by the Alliance census itself for Keeshan dual-spawns) keeps it here: IN, with the 1418 key and the Badlands turn-in (Thal'trak @3.36,48.1) both named. If a future Badlands addendum claims 1418-keyed single-frame-1428 records as a class, this contract cedes 3822 the same way.
(c) 4121s pre chain through uncontracted Badlands records (4081 object-start > 4082 BRD kills > 4122 Badlands accept > in-zone 4122 turnin): the mini keys on 4122 (the direct pre, holdable by playing Badlands content), not on the deeper links - the Kadrak pattern (same as Tanaris 243, which also sat behind uncontracted pres). The deeper links are named, not routed.
(d) Band 48-58 on three records: stated as a three-point span (bulk language would be dishonest - there is no bulk). The top is a finale (8998), the bottom a chain head (3822); either could stand alone and the band still covers the third.
(e) No guide-shape borrowing: the Temple/BRD interior legs that the Alliance guide notes (Orb of Command etc.) belong to the main guides contracted interior work; this guides three chains need no interior notes (escort event is open-world at placed coords; Krom'Grul is an open-world single point).

