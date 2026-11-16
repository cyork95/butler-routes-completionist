# The Hinterlands census (pack 0.69.0)

Accept-zone key **1425**, from the local Forever game data (built with
`--product wowf` + QuestieDB). 90 candidates: 38 with zone-field 1425 plus
52 caught by the city-rule test (a start NPC/object spawning on the 1425 map).
Race masks read off the settled precedent (Blasted Lands/Silverpine):
`4294967373` = Alliance, `8589934770` = Horde, null = neutral.

Band derived from the data: contracted minLevels run 38-45 with quest levels
to 51 (plus the L60/min1 writ special class, which never sets the band - Swamp
precedent). Low end 38 = the lowest contracted minLevel (1446/1452/1469);
top 51 = the highest contracted non-writ quest level (86615 L51/min40 and
86620 L51, both Aerie Peak hub quests); 1446 at L53 rides the finale rule via
min38. **Band 38-51.**

## IN ledger (14)

| ID | Title | Level/min | Giver (accept point) | Disposition |
|----|-------|-----------|----------------------|-------------|
| 485 | Find OOX-09/HL! | 48/43 | Item 8704 OOX-09/HL Distress Beacon (53 droppers incl. Vilebranch/Witherbark on 1425; same mobs also drop it in Arathi) | IN, item-start; note + optional sourcing kill, never wedges |
| 836 | Rescue OOX-09/HL! | 48/43 | Homing Robot OOX-09/HL @49.35,37.66; escort event @79.14,61.36; turnin Oglethorpe Obnoticus, Booty Bay (1434) | IN; STV expedition turnin |
| 1446 | Jammal'an the Prophet | 53/38 | Atal'ai Exile @33.75,75.21 (neutral); turnin same | IN; finale-over-band via min38. Boss 5710 spawnless in data: bare complete + honest note (Blasted 2991 precedent) |
| 1452 | Rhapsody's Kalimdor Kocktail | 43/38 | Rhapsody Shindigger @26.94,48.59 | IN. Pre 1451 out-of-contract (Hillsbrad-OUT): structural warning + pick-up note. Objectives all out-of-zone (Tanaris rocs, Thousand Needles/Feralas livers): expedition completes |
| 1469 | Rhapsody's Tale | 43/38 | Rhapsody; turnin Brohann Caskbelly, Stormwind (1453) | IN; pre 1452 in-contract; Stormwind expedition turnin |
| 2877 | Skulk Rock Clean-up | 48/40 | Fraggar Thundermantle @14.83,44.57 (Aerie Peak) | IN; kills 2655/2656 at Skulk Rock |
| 2880 | Troll Necklace Bounty | 45/40 | Fraggar; same-name twin of 2881 | IN (twin precedent: both) |
| 2881 | Troll Necklace Bounty | 45/40 | Fraggar; pre 2880 | IN (twin precedent: both) |
| 86615 | Treaty Obligations | 51/40 | Tove Redstone @11.84,46.7 (neutral giver, Alliance mask) | IN. Satchel object 668515 MISSING from data: bare complete + honest note |
| 86616 | Repurposed Totems | 48/45 | Farseer Maret Firetend @14.4,42.6 | IN; 12 totems off Soothsayer 4467 cluster |
| 86620 | Fledgling Rescue | 51/min null | Gryphon Master Talonaxe @9.75,44.47 | IN (see BORDERLINE 1). Egg objects 669115 MISSING: bare complete + honest note |
| 94266 | Craftsman's Writ: Elixir of Agility | 60/1 | Item-start, no source in data (sourceless); end Juo @80.13,55.39 | IN (Swamp writ precedent); R2 + R5 residue |
| 94290 | Craftsman's Writ: Mechanical Repair Kit | 60/1 | Item-start, sourceless; end Rhapsody | IN; R2 + R5 residue |
| 94302 | Craftsman's Writ: Turtle Scale Breastplate | 60/1 | Item-start, sourceless; end Juo | IN; R2 + R5 residue |

No class quests, no profession quests, no race-exclusive quests in the IN set:
nothing contracted needs `only`/`when skill` gating.

## OUT ledger

Horde set-asides (25, for the Horde block's reconciliation): 77, 81 (OOX
pre-chain via Gilveradin), 1444 (Return to Fel'Zerul), 2742, 2782 (Rin'ji),
2933 (Venom Bottles), the Revantusk block 7815, 7816, 7828, 7829, 7830, 7839,
7840, 7841, 7842, 7843, 7844, 7845, 7846, 7847 (Elder Torntusk dual 1417/1425,
chain home Arathi), 7849, 7850, 7861, 7862 (wanted-poster object-starts),
98203 (Witch Doctor Ti'ik; neutral giver Qujo, Horde mask rules).

Seasonal/event (2): 8643 Highpeak the Elder (event=7, Lunar Festival);
9029 A Bubbling Cauldron (event=8, Hallow's End cauldron, multi-zone object).

Battleground brackets + repeatables (34, all Horde Warbringer starts):
8367, 8368, 8369, 8370, 8387, 8388, 8389, 8390, 8426-8435 (10), 8436-8443
(8), past-victories 8566, 8568, 8570, Darkspear clash 98887-98891 (98890 also
broken: Lnull/minnull).

Accept-outside-zone, zone field wins (11 + 1 borderline):
- Zone-field 1424 (Hillsbrad), ruled above-band OUT there and not re-homed
  here per the Hillsbrad sweep rule (starter-not-only-on-one-map, zone field
  wins): 1450, 1451 (Gryphon Master chain), 2988, 2989, 2990, 2994 (Altar of
  Zul chain; 2993 pre-link lives in Badlands), 4297, 4298 (Agnar chain).
  Consequence: 1452 carries its out-of-contract pre 1451 (note + structural
  warning, Hillsbrad-554 precedent). 2994's pre 2993 is Badlands-contracted.
- Zone-field 1416 (Alterac), Alterac-ruled, not re-homed here: 6701
  Syndicate Emblems (repeatable, Alterac OUT), 8234 Sealed Azure Bag
  (above-band 52/50, Alterac OUT; also above this band), 96779 Syndicate
  Sabotage (below-band 24/24, Alterac OUT). 96781/96782/96783 are
  Alterac-contracted (Ravenholdt chain) and stay there: no double-contract.
- 81954 Venomous Journeys: see BORDERLINE 2 (OUT).

## BORDERLINE (all decided, none silent)

1. **86620 Fledgling Rescue (L51, minLevel null) - IN.** Hillsbrad's sweep
   explicitly deferred this record here ("86620 (Hinterlands)"). It accepts
   at the contracted Aerie Peak hub from a contracted NPC, and its level 51
   matches the contracted 86615 (L51/min40) at the same hub, so the band top
   51 covers both without special pleading. The egg objects are missing from
   the data (see IN ledger), handled with the honest bare-complete note, not
   an invented point.
2. **81954 Venomous Journeys - OUT (accept-outside-zone).** For IN: its book
   object 441252 spawns on 1425 (@36,72.8), so one accept path is physically
   here. For OUT, three weights: the zone field says 1458; the other two
   accept paths are NPCs in 1458 (Owen Thadd, Horde) and Stormwind (Garion
   Wendell, Alliance); and the chain's next (97286 Research Access) lives in
   1458, so the chain's home is elsewhere. Per the Hillsbrad triple-map rule
   (starter-not-only-here, zone field wins), OUT. If Butler's reconciliation
   wants the book path covered, it belongs to the 1458 zone's census, not
   this contract.
3. **Band top 51 vs 50 - 51.** The two L51 Aerie Peak quests (86615 min40,
   86620 level-only) are hub-consistent zone content, not finales; capping
   the band at 50 would misdescribe the contract. 51 it is.
4. **Rhapsody objective zones - no double-contract.** The 1452 ingredients
   come from Tanaris (rocs), Thousand Needles (bears), and Feralas (apes);
   those kills are expedition completes in this guide, owned by no other
   contract (no other guide routes Rhapsody's items).
