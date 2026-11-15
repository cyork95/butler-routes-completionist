# Moonglade census (pack 0.37.0)

This round is not a zone route: it is the Alliance (Night Elf) druid class
guide — the form quests and druid class chains centred on Moonglade. The
accept-in-zone rule is relaxed by design here: territory is the druid chains,
not the map. Horde (Tauren) druid content is counted and set aside for the
Horde block, like every other round.

- Accept-zone key used: **1450** (Moonglade; Kalimdor key space with the
  Teldrassil 1438 / Darkshore 1439 / Ashenvale 1440 / Stonetalon 1442 family).
- Total candidates: **56** zone-field records, plus the inherited flag list
  (Darnassus/Teldrassil/Alterac set-asides) and the reconciliation check
  against `docs/quest-contracts.json`.
- IN: **19** (19 accepts, 19 turn-ins — every contracted quest has an ender;
  no accept-only records). Level span **10–52** (bear/aquatic/cure/cat chains
  at 10–20, the Torwa chain at 50–52).
- OUT of the zone set: 11 Horde druid + 19 non-druid + 12 seasonal/repeatable.
  Homed elsewhere (stay — pointer notes only): 14.

## Reconciliation — every inherited flag

Stay contracted where they are (never double-contracted; the guide carries a
pointer note where a chain needs it):
- Darnassus-city: 26 (→29 here), 5921 (→5929 here), 5923, 6001 (←5931 here),
  6121 (→6122 here), 9063 (→9052 here), 98393 (→98394 here), 3763, 3764, 3781,
  3785 (the Morrowgrain line — non-druid, homed, ends here only as a note).
- Teldrassil: 5925 (→5921, homed).
- Darkshore: 6123, 6124 (→6125 here).
- Teldrassil's Moonglade Druid line (26/5921/6121/6001): accounted for — all
  four homed in Darnassus per the Teldrassil census's deferral; nothing
  additional outstanding.
- 6124 (turn-in at Dendrite in Moonglade): homed in Darkshore; stays. The
  6125 step here carries the pre-note.
- 94912 (Alterac set-aside, Child of Nature): contracted NOWHERE — contracted
  here.

## IN ledger (19)

| ID | Quest | L/m | Disposition |
|----|-------|-----|-------------|
| 29 | Trial of the Sea Lion | 16/16 | pre 26 (Darnassus, homed) — pre-note; Shrine of Remulos objective (36, 41.42) |
| 272 | Trial of the Sea Lion | 16/16 | pre 29; Pendant of the Sea Lion from the shrine |
| 5061 | Aquatic Form | 16/16 | pre 272; ends Mathrengyl Bearwalker (Darnassus expedition) |
| 5924 | Heeding the Call | 10/10 | Stormwind accept (Theridran); ends Bearwalker; feeds homed 5921 — pointer note |
| 5929 | Great Bear Spirit | 10/10 | pre 5921 (Darnassus, homed) — pre-note; event objective (bare complete at Dendrite) |
| 5931 | Back to Darnassus | 10/10 | pre 5929; ends Bearwalker (expedition); 6001 lives in the Darnassus guide — pointer note |
| 6122 | The Principal Source | 14/14 | pre 6121 (Darnassus, homed) — pre-note; sampler has no source (bag note, bare complete); ends Alanndarian (Darkshore expedition) |
| 6125 | Power over Poison | 14/14 | pre 6124 (Darkshore, homed) — pre-note; no objectives; ends Bearwalker |
| 94912 | Child of Nature | 10/10 | Alterac accept (Ansirem); ends Sheldras Moontree (Stormwind expedition); no objectives |
| 98394 | The Great Cat Spirit | 20/20 | pre 98393 (Darnassus, homed) — pre-note; ends Great Cat Spirit (in-zone) |
| 98396 | The Great Cat Spirit | 20/20 | pre 98394; relics have no source (bag notes, bare complete); ends Great Cat Spirit |
| 98731 | Blessings of the Great Cat Spirit | 20/20 | pre 98396; ends Dendrite |
| 98341 | The Great Windborne Cat Spirit | 20/20 | pre [98340 Horde twin, 98393 ✓] — twin note (Alterac 92459 precedent); ends Avatar of Saeyleenan |
| 98404 | The Great Windborne Cat Spirit | 20/20 | pre 98341; relics bag + bare complete; ends Avatar |
| 98738 | Blessings of the Great Windborne Cat Spirit | 20/20 | pre 98404; ends Dendrite |
| 98397 | To Darnassus | 20/20 | pre [98731 ✓, 98738 ✓]; ends Bearwalker (expedition) |
| 9052 | Bloodpetal Poison | 52/50 | pre 9063 (Darnassus, homed) — pre-note; Gorishi Stings (Un'Goro placed) + Bloodcap sourceless (bag); ends Torwa (Un'Goro expedition) |
| 9051 | Toxic Test | 52/50 | pre 9052; Devilsaur kill (Un'Goro placed); ends Torwa |
| 9053 | A Better Ingredient | 52/50 | pre 9051; Putrid Vine dropper spawnless (bag note, bare complete); ends Torwa; finale |

Race gates (per-line, Teldrassil lesson): the races=8 and races=4294967304
records are Night-Elf-locked and gated `only Night Elf` per line; the
races=null records (5924? no — 5924 is races=8; null: 9052/9051/9053) and the
both-factions 12884901888 branch carry no race gate. No `race` header
question arises — the header is `class Druid` per the brief, and per-line
gates do the rest.

## OUT ledger

Horde druid set-aside (18, for the Horde block — note 98738 is contracted
here and the Horde chain 98362 needs it, the mirror of our 79975
situation): 27, 28, 30, 31, 5922, 5930, 5932, 6002, 6126, 6127, 6128, 6129,
6130, 98340, 98342, 98362, 98405, 98739.

Non-druid zone-1450 quests (out of scope by this guide's design — its
territory is the druid chains; several have no other home, which is the
design's known gap, as with the 3763 line): 1124, 1185, 6845, 5526, 5527,
7066 (also broken: Zaetar's Spirit has no spawn anywhere), 8446, 8447, 8735,
8736, 8741, 93773, 95006, 96209, 94261, 94273, 94285, 94297, 94309 (the five
Moonglade writs — non-druid despite item-starts and in-zone enders).

Seasonal/repeatable (12, Lunar Festival event=7, most explicitly repeatable):
8862, 8863, 8864, 8865, 8868, 8876, 8877, 8878, 8879, 8880, 8881, 8882.

## Companions question

- Rare-flagged NPCs spawning on 1450: none (0).
- Treasures: one object (GunShopFireworksBarrel, Lunar Festival seasonal) —
  no year-round treasure.
- In-zone recipe sources: 8 recipes from 2 plain year-round vendors, both
  Alliance-or-neutral faction with 1450-only spawns and no event linkage:
  Darnall (npc7940, Tailoring Supplies, (51.47, 33.25)): Pattern: Runecloth
  Robe 14469, Pattern: Runecloth Cloak 14472, Pattern: Runecloth Boots 14488,
  Pattern: Linen/Woolen Reagent Bag 253665/253668; Lorelae Wintersong
  (npc12022, Trade Supplies, (48.24, 40.14)): Pattern: Felcloth Pants 14483,
  Formula: Enchant Cloak - Superior Defense 16224, Formula: Runed Arcanite
  Rod 16243.
- Answer: no rares companion warranted; a small recipes companion (8
  recipes, Tailoring 6 + Enchanting 2) is real content for a separate small
  round — not this one.

## BORDERLINE (all decided, none silent)

1. 9052/9051/9053 (neutral-druid Tanaris chain, 50–52, pre homed in
   Darnassus) — IN. Druid-gated, uncontracted, chained to homed 9063; the
   relaxed accept rule covers the out-of-zone accepts, and the brief defines
   IN by class, not band. The span stretches to 52 — that is what the data
   covers.
2. Moonglade writs 94261–94309 — OUT. Non-druid by design despite
   item-starts and in-zone enders (the item-start rule loses to the
   druid-design rule here, as with 8446). Design gap noted, not silently
   dropped.
3. 3763–3785 — already homed in Darnassus (reconciliation outcome); 3803 is
   repeatable in any case. The Darnassus "open chain" flag is thereby
   closed with no action needed here beyond this note.
4. 98341's pre [98340, 98393] — IN with the twin note. 98340 (Horde
   "The Great Cat Spirit") and 98393 (NE same title, Darnassus-homed) are
   same-title variants; the chain-consistent one is contracted/homed and
   98341 follows it (Alterac 92459 precedent). Any lint warning naming
   98340 is accepted as structural.
5. The 12884901888 branch (98341/98404/98738) — treated as both-factions:
   both the NE finale 98397 and the Horde finale 98362 require 98738, so
   both factions must be able to do it. IN for Alliance use; Horde
   references it.
6. 8446 (item-start, ends Remulos, non-druid) — OUT by design (see 2).
