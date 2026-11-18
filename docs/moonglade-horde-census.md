# Moonglade (Horde) census (game data - class-guide territory: the Tauren druid chains, not the map)

This round is the Horde (Tauren + Horde-side Skyborne) druid class
guide - the form quests and druid class chains centred on Moonglade
and Thunder Bluff. The accept-in-zone rule is relaxed by design here:
territory is the druid chains, not the map (the Alliance Moonglade
census, docs/moonglade-census.md, establishes this design). Horde-mask
records below are Tauren-druid content unless the races field says
otherwise; Skyborne-Horde druid content rides the same chains where the
data puts it.

## Pool and reconciliation

The Alliance census banks 18 Horde druid set-asides, each reconciled
one by one below: 27, 28, 30, 31 (bear/aquatic forms), 5922, 5930,
5932, 6002 (Moonglade chain), 6126, 6127, 6128, 6129, 6130 (cure
chain), 98340, 98342, 98362, 98405, 98739 (great-cat chain). Every one
is IN this contract except where ruled OUT with its reason stated - the
pool scan found all 18 with Horde-side masks and no disqualifiers. A
pool-wide scan for further Horde druid class quests (classes=1024 with
Horde-side races) found: 5926/5927/5928 Heeding the Call (homed -
contracted in thunder-bluff-city / orgrimmar-city / mulgore), 3094
Verdant Note (homed - mulgore), 8913/8927/9007 (homed -
orgrimmar-city), 9016 Anthions Parting Words (OUT below), 7506 (OUT
below), 8192 (OUT below). Nothing else uncontracted belongs here.

The Alliance guides own contracts stay untouched: 26/5921/6001/6121/
9063 (Darnassus-homed pres, pointed at not duplicated), 98393
(Darnassus-homed twin pre of 98340, pointed at), the 98341/98404/98738
Skyborne-both Windborne chain (main-contracted, Horde-visible after
this rounds ungating - the 98362 branch it serves is argued below),
2521-zone Skyborne records (homed in zephras-isle).

## Span: 10-20

Contracted minLevels run 10 (Moonglade chain: 5922/5930/5932/6002)
through 20 (great-cat chain: 98340/98342/98405/98739/98362), with the
bear/aquatic forms at 16 (27/28/30/31) and the cure chain at 14
(6126-6130). Derived from the Horde records own levels (the Alliance
spans 10-52 on the back of its Torwa chain; there is no Horde Torwa
chain, so this span stops at 20). No class header question: every line
is druid content; per-line `only` gates do the work.

No race header for the guide beyond faction: two race shapes exist in
the pool - races=32 (Tauren-only: 5922/5930/5932/6002/98342/98405/
98739) gated `only Tauren,Druid`, and races=8589934624
(Tauren + Skyborne-Horde, bit-verified against the races table:
2^33 Skyborne-Horde + 32 Tauren: 27/28/30/31/6126/6127/6128/6129/6130/
98340/98362) gated `only Tauren,Skyborne,Druid`. Never blanket-gated
beyond the data; the engine treats comma lists as race-OR plus class
(verified in fits()). No profession gates, no skill-gated records.

## IN (18 - the full set-aside pool)

Thunder Bluff hub (Turak Runetotem 3033 @76.48,27.22):

| 5922 Moonglade | 10/10 | pre 5926/5927/5928 Heeding the Call (homed in thunder-bluff-city / orgrimmar-city / mulgore - pre-note naming all three, no mini; the Alliance 5921-pattern) | no objectives; ends Dendrite Starblaze (Moonglade expedition) |
| 27 A Lesson to Learn | 16/16 | no pre | no objectives; ends Dendrite Starblaze (expedition); form chain head |
| 6126 Lessons Anew | 14/14 | no pre (accepts at Turak; Hana Lighthoof 262560 in Mulgore is the alternate starter, noted) | no objectives; ends Dendrite Starblaze (expedition) |
| 98340 The Great Cat Spirit | 20/20 | no pre; twin of Darnassus-homed 98393 (only one is takeable - the pack twin shape; no gate needed on this side since 98393 is unroutable for Horde) | no objectives; ends Dendrite Starblaze (expedition) |

Moonglade village (Dendrite Starblaze 11802 @56.21,30.64; Tajarri 11799 @36.52,40.1; Great Cat Spirit 11957 @54.5,75):

| 5930 Great Bear Spirit | 10/10 | pre 5922 (IN) | event objective (seek out the spirit - bare complete at Dendrite) |
| 28 Trial of the Lake | 16/16 | pre 27 (IN) | object 15885 Shrine of Remulos, in-zone single point @36,41.42 (bare complete at the shrine) |
| 30 Trial of the Sea Lion | 16/16 | pre 28 (IN) | item 15885 Pendant of the Sea Lion (sourced from the shrine object per the data - bare complete at the shrine, mirror of the Alliance pendant rite; no halves hunt: the objective counts one pendant) |
| 6127 The Principal Source | 14/14 | pre 6126 (IN) | item 15843 Filled Dreadmist Peak Sampler off object 19464 Dreadmist Peak Pool (Barrens @48.4,18.9 - Crossroads leg) -> ends Tonga Runetotem 3448, Crossroads (1413 @52.26,31.93) |
| 6130 Power over Poison | 14/14 | pre 6129 (IN) | no objectives; ends Turak (Thunder Bluff expedition) |
| 98405 The Great Cat Spirit | 20/20 | pre 98340 (IN) | event objective (seek out the Spirit - bare complete at the Spirit) |

Crossroads leg (Tonga Runetotem 3448 @52.26,31.93; Barrens kodos/gazelles):

| 6128 Gathering the Cure | 14/14 | pre 6127 (IN) | 5 Kodo Horns 15852 off Lost Barrens Kodo 3234 / Barrens Kodo 3236 (1413 clusters) + 5 Earthroot 2449 (gatherable/buyable - honest note, no gate needed) -> ends Tonga |
| 6129 Curing the Sick | 14/14 | pre 6128 (IN) | use the salve on 10 Sickly Gazelles 12296 (1413 clusters ~41-42,15-25) -> ends Dendrite (Moonglade expedition) |

Stormrage trio (relic objects 672821 @72.4,66 / 673093 @75.2,67.2 / 673094 @74.4,65.4, Moonglade):

| 98342 The Great Cat Spirit | 20/20 | pre 98405 (IN); excl [98396, 98404] (the Alliance variants - parallel chains, in-game exclusive, each side contracted) | 1 Relic of the Fang 280502 + 1 Relic of the Claw 280679 + 1 Relic of the Silent Shadow 280680 (bare complete at the Spirit with a note naming the three dens - mirror of the Alliance relic handling) |

Finale (Dendrite -> Avatar -> Turak):

| 98739 Blessings of the Great Cat Spirit | 20/20 | pre 98342 (IN); excl [98731, 98738] (parallel variants) | no objectives; ends Dendrite (note: the Skyborne path continues via main-contracted 98738, Horde-visible after ungating) |
| 98362 To Thunder Bluff | 20/20 | pre [98739, 98738] (either/or - multi-pre reads as any: Tauren druids via 98739, Skyborne-Horde druids via 98738; excl [98397] the Alliance finale) | no objectives; ends Turak (Thunder Bluff expedition) - the Horde finale |

Tracker-adjacent (accepted at Turak, resolved at the Moonkin Stone between Mulgore and the Barrens):

| 5932 Back to Thunder Bluff | 10/10 | pre 5930 (IN) | no objectives; ends Turak (in-hand turn-in) |
| 6002 Body and Heart | 10/10 | pre 5932 (IN) | kill Lunaclaw Spirit 12144 (event summon, no placed spawn anywhere in the data - note the Moonkin Stone area + the Cenarion Lunardust 15710 bag note, which itself names no source) |

## OUT (homed or out-of-scope - none of the 18)

- Homed elsewhere (pointed at, never duplicated): 5926/5927/5928 (thunder-bluff-city / orgrimmar-city / mulgore), 3094 (mulgore), 8913/8927/9007 (orgrimmar-city), 81924 (feralas), 92485/94006/94638 (zephras-isle).
- Out of scope: 9016 Anthions Parting Words (Horde druid, but a m58 Silithus-accept dungeon-set chain link homed by geography - Silithus content, not a Moonglade chain; uncontracted anywhere, noted for the record); 7506 The Emerald Dream (broken: zone 234 unresolvable, no objectives); 8192 Animists Caress (ZulGurub dungeon turn-in, not a Moonglade chain).
- The 19 non-druid Moonglade zone quests (incl. the five writs 94261-94297) stay out by the class-guide design - named once here per the brief and moved past (a Final QA question, not this round).

## BORDERLINE (all decided, none silent)

(a) 98738: races 12884901888 decodes as Skyborne-both (bit-verified: 2^32 + 2^33), Horde-reachable via Skyborne-Horde druids - NOT duplicated here (it lives in the main contract). The brief feared an Alliance-only record; the data shows a Skyborne-gated shared record instead. After this rounds ungating (faction header dropped), its lines stay bare (`only Skyborne,Druid` like the Alliance file) and Horde Skyborne druids can take it. Tauren druids cannot - but they do not need to: 98362s pre reads either/or (multi-pre = any, per the Tanaris either/or precedent and the linters own one-of rendering), so the Tauren path runs 98739 alone. Verified: no character needs both branches.
(b) Skyborne-Horde druids stall after 98340 (98405 is Tauren-locked; no Skyborne 98405-variant exists in the data) - documented data gap, not a routing choice. The Horde chain as contracted is complete for Tauren druids; the Skyborne branch is open-ended in the data.
(c) 98340 vs 98393 (twin pre of the MAIN guides 98341): either/or confirmed - the Alliance side already contracts 98341 on that basis (Alterac 92459 precedent). No duplication: each faction carries its own twin.
(d) 9016: the one Horde-druid-shaped record left out - m58 dungeon-set chain, Silithus-accept, Org-ender, uncontracted. If a future round contracts the Anthion chain, 9016 homes there; this class guide does not stretch to 58 for it. Data wins over the class-only reading: chains, not the class flag alone, define territory.
(e) Span 10-20: derived from the Horde minLevels (10 Moonglade chain, 14 cure, 16 forms, 20 cat); no Torwa tail on this side. No band rule needed beyond stating it.
(f) Bag-noted objectives (sampler-adjacent relics, Lunardust, 6128s earthroot): named source-or-absence in every note; no collect lines for quest items without placed mob droppers (mirrors the Alliance class-guide shape, which carries zero collects).

