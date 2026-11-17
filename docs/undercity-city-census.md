# Undercity city census

City key **1458** verified by counting: 124 quest records carry
`zone=1458`, and 235 start-NPC refs land on 1458 (reproduces the Tirisfal
census counts; the Tirisfal census keyed the open zone on 1420 with 159
zone records and 171 start refs). The city rule applies as in Orgrimmar
(1454) and Thunder Bluff (1456): a giver spawning on BOTH the open-zone
key (1420) and the city key (1458) is a city NPC, even where the 1420
point sits on the open map.

Method: every quest with an accept/start touching 1458 - start NPC
spawning on 1458, start object spawning on 1458, or start item whose
source spawns on 1458 - was enumerated (240 UC-linked records), then
filtered by the pack rules. Item-starts are enumerated explicitly below
(the Mulgore lesson); no absence is asserted without a start-item scan.
Zone field alone never decides: 84395-84402 key zone 1453 but start
from Oran Snakewrithe (1458) and are contracted here; 357/366/446 key
zone 1420 but start from dual-spawn Bethor Iceshard and are contracted
here. Conversely 9265/9154 key zone 1458 but are event-gated and OUT.

No level band (city rule): the contract is every quest accepting on
1458, span **1-60** (lowest minLevel 1, the library books; highest level
60, the donation/event-era records).

## IN (107)

Open-world Horde quests accepting on 1458 (or via a 1458-sourced
item/object), unhomed. Same-name twin IDs both routed (1474/65593-era
twins; the Seeping Corruption triple 3568/3569/3570). Race gates follow
the data exactly (race bits: 16 Undead, 128 Troll, 146 Orc/Undead/Troll;
Horde-all flag 8589934770). Class quests carry `only <Class>`; the
Undead Mage line gates `only Mage,Undead,Troll` / `only
Mage,Orc,Undead,Troll` per line; the Undead Priest line gates `only
Priest,Undead` (+`only Priest,Troll` where the data gates Troll).

City NPC starter chains (dual 1420+1458 = city NPC):
- 357 The Lich's Identity (8/5; pre 405 Tirisfal) - 366 Return the
  Book (8/5; next 409 Tirisfal) - 446 Thule Ravenclaw (16/10; pre 444
  Silverpine, next 448 Silverpine): Bethor Iceshard
  (1458 @84.07,17.45). 357's objective (Gunther's Books object, Tirisfal
  @67.96,42.09) and 366's turn-in (Gunther Arcanus, Tirisfal @68.2,41.92)
  ride a Tirisfal expedition leg; 446 turns in at Renferrel, Silverpine.
- 1882 The Balnir Farmstead (10/10) - 1943 Speak with Deino (26/26;
  next 1944 Durotar, uncontracted) - 1947 Journey to the Marsh (38/30)
  - 1953 Return to the Marsh (40/35; next 1954 Dustwallow,
  uncontracted) - 1960 Investigate the Alchemist Shop (16/15; pre 1959
  Org/TB, soft-pre mini-step) - 1961 Gathering Materials (15/15; pre
  1960): Anastasia Hartwell (1458 @85.14,10.03). 1882's objective
  (Balnir Snapdragons object, Tirisfal) rides the Tirisfal leg; 1943
  turns in at Deino, Durotar; 1947/1953 turn in at Tabetha, Dustwallow;
  1960's objectives split placed (Chest of Containment Coffers object,
  UC @85.48,9.9) and bag (Filled Containment Coffer, sourceless);
  1961's objectives split bag (Linen Cloth) and placed (Dalaran Mana
  Gem, Dalaran Apprentices, Silverpine).
- 4489 Summon Felsteed (40/40; next 4490 Barrens, uncontracted) -
  4739 In Search of Menara Voidrender (31/31; next 1796 Barrens,
  uncontracted) - 4969 Knowledge of the Orb of Orahil (35/35; next 1799
  Barrens, uncontracted): Kaal Soulreaper (1458 @86.21,15.93). Turn-ins
  at Strahad Farsan / Menara Voidrender, Barrens (expedition).
- 5643 Shadowguard (20/20) - 5657 Hex of Weakness (10/10) - 5658 Touch
  of Weakness (10/10) - 5679 Dark Sacrifice (20/20): Aelthalyste
  (1458 @49.26,17.12). 5643/5657 turn in at Ur'kyo, Durotar
  (expedition); 5658/5679 turn in at Aelthalyste.
- 65593 Hearts of the Lovers (20/20; pre 1472) - 65597 The Binding
  (20/20; pre 65593): Godrick Farsan (1458 @84.81,14.83) / Carendin
  Halgar (1458 @85.06,25.99). Objectives in Silverpine (Avelina Lilly)
  and Barrens (Isaac Pearson); 65597 completes on a summoned Incubus
  (bare complete + note).
- 1472 Devourer of Souls (-1/20) - 1476 Hearts of the Pure (-1/20; pre
  1472) - 1474 The Binding (20/20; pre 1476): Carendin / Godrick.
  Objectives from Dalin Forgewright (Silverpine) and Comar Villard
  (Arathi); 1474 completes on a summoned Succubus (bare complete).

Multi-city class chains (starter spawns on 1458; per-city legs per the
8151/8250/8417 Orgrimmar+Thunder Bluff precedent):
- 1718 The Islander (30/30; next 1719) - 1823 Speak with Ruga (20/20;
  next 1824) - 8417 A Troubled Spirit (50/50; next 8423): warrior,
  `only Warrior`; starters Baltus Fowler / Christoph Walker
  (1458 points). Turn-ins at Klannoc Macleod / Ruga Ragetotem (Barrens)
  and the Fallen Hero of the Horde (Swamp of Sorrows).
- 8233 A Simple Request (52/50; next 8234): rogue, `only Rogue`;
  starter Miles Dexter (1458 @85.21,71.57). Turn-in at Lord Jorach
  Ravenholdt (Hillsbrad).
- 8250 Magecraft (52/50; next 8251): mage, `only Mage`; starter Pierce
  Shackleton (dual, 1458 @85.45,13.51). Turn-in at Sanath Lim-yo
  (Azshara).
- 1947/1953 (above) share starters with Orgrimmar legs; contracted here
  for the UC leg.
- 7562 Mor'zul Bloodbringer (58/60; next 7563 Searing, uncontracted):
  warlock, `only Warlock`; starter Martha Strain (1458 @85.7,16.08).
  Turn-in at Mor'zul Bloodbringer, Searing Gorge (expedition).
- 8419 An Imp's Request (52/50; next 8421 Felwood, uncontracted):
  warlock, `only Warlock`; starter Kaal Soulreaper. Objective Felcloth
  (generic world drop, bag note); turn-in at Impsy, Felwood.
- 1959 Report to Anastasia stays OUT (no 1458 starter; Orgrimmar and
  Thunder Bluff contract it). 1960 carries a soft-pre mini-step for it.

Rogues' Quarter chain (Mennet Carkad, dual 1422+1458, 1458
@83.51,69.11; Undead-only `only Rogue,Undead`):
- 1886/1898/1998/1999 The Deathstalkers line + 2378 Find the
  Shattered Hand (next 2379, uncontracted) + 1978 The Deathstalkers
  (pre 1899, uncontracted - structural warning, accept-only mini-step
  for the turn-in). Objectives from Astor Hadren (Silverpine),
  Fenwick Thatros (Silverpine) and the Ambermill Strongbox (Silverpine);
  1886's letter and 1998/1999 ride the Silverpine leg. 2378 turns in at
  Shenthul, Orgrimmar (expedition); 1978 turns in at Varimathras.
Apothecarium chains (all starters in the Apothecarium, in-city completes
unless noted):
- 1109 Going, Going, Guano! (33/30) - 1113 Hearts of Zeal (33/30; pre
  1109): Faranell (1458 @48.82,69.28). 1109's objective (Kraul Guano)
  has no placed source (bats spawnless) - R2 bag note; 1113's objective
  (Heart of Zeal, Scarlet Preservers, Tirisfal @81-83,29-35) rides the
  Tirisfal leg.
- 3568/3569/3570 Seeping Corruption (52/45): Chemist Cazarez
  (1458 @48.71,71.39) to Cazarez / Thersa Windsong
  (1458 @49.04,70.8). Objectives fill at the Azshara tide pools
  (expedition).
- 96988 Source of Power (33/24): Doctor Felben (1458 @46.61,74.09).
  Objective (Cracked Sentry Core) sourceless - R2 bag note.
- 97049 Essence of Seeping Slimes (60/55): Chemist Fuely
  (1458 @47.45,73.35). Objective sourceless - R2 bag note.
- 4293 A Sample of Slime (52/48) - 4294 ... and a Batch of Ooze
  (56/48) - 4642 Melding of Influences (55/48; pre 4293+4294): Fuely
  (dual 1421+1458 = city NPC). Objectives from the Testing Equipment
  objects (in-city, UC @47.85,73.48 / @47.74,73.57) and Primal/Gargantuan
  Oozes (Un'Goro expedition).
- 95216 The New Plague (22/15; pre 451 Silverpine-contracted):
  Theodore Griffs (1458 @46.31,71.91). Objective (Highly Toxic
  Strain, Witherfang spawnless) - R2 bag note; accept carries a
  structural out-of-contract-pre note.
- 95204 Crest of Lordaeron (22/15): item-start (Crest of Lordaeron, its
  object spawnless) - R2 bag accept; turn-in Oran Snakewrithe (UC).
- 95328 Whispering Horror Residue (13/7): item-start (Whispering Horror,
  Tirisfal @8-10,58-66, optional sourcing kill); turn-in Father
  Lankester (1458 @49.14,14.61).
- 97985 Thundering Hearts (33/25): Calder Gray (1458 @49.11,70.14).
  Objective (Stormheart's Still-beating Heart, Stormheart, Thousand
  Needles - expedition sourcing, optional).

War Quarter and trade (expedition turn-ins noted):
- 1846 Dragonmaw Shinbones (30/20; pre 1841 Barrens-contracted,
  soft-pre mini-step) - 1847 Brutal Legguards (30/20; pre 1846):
  warrior, Velora Nitely (1458 @62.14,39.14). Objective (Sturdy
  Dragonmaw Shinbone, Dragonmaw Raiders, Wetlands) rides a Wetlands
  expedition leg.
- 1004 The New Frontier (55/54; next 1123 Thunder Bluff-homed):
  Balthazad (1458 @63.9,44.08). Turn-in Carendin Halgar,
  Thunder Bluff (expedition).
- 5094 A Call to Arms: The Plaguelands! (50/50; next 5096 Tirisfal,
  uncontracted): Balthazad. Turn-in High Executor Derrington,
  Tirisfal (expedition).
- 7492 Camp Mojache (57/54; next 7489 Feralas, uncontracted):
  Balthazad (+Org/TB co-starters; UC leg). Turn-in Talo Thornhoof,
  Feralas (expedition).
- 7813/7814/7817 A Donation of Wool/Silk/Mageweave (60/12-40) - 7818 A
  Donation of Runecloth (60/50; pre the three): Ralston Farnsley
  (1458 @71.66,29.23). Objectives are generic cloth (bag notes, the
  TB 768/769 precedent). 7819 Additional Runecloth is OUT (repeatable).
- 3526 Goblin Engineering (47/30) - 3635 Gnome Engineering (47/30):
  `optional` + `when skill Engineering 1`; Graham Van Talen
  (1458 @75.34,73.13). Turn-ins Nixx Sprocketspring (Tanaris) and
  Oglethorpe Obnoticus (Booty Bay) ride expeditions.
- 4133 Vivian Lagrave (55/50; next 4134 Badlands, uncontracted) - 4769
  Vivian Lagrave and the Darkstone Tablet (60/57; next 4768 Badlands,
  uncontracted): Zinge (1458 @50.14,67.97). Turn-ins at
  Shadowmage Vivian Lagrave, Badlands (expedition).
- 5961 The Champion of the Banshee Queen (56/54): Sylvanas
  (1458 @58.05,91.79). Turn-in Nathanos Blightcaller, WPL (expedition).
- 6145 The Crimson Courier (60/56; pre 6144 WPL, uncontracted -
  soft-pre mini-step): Varimathras (dual, 1458 @56.25,92.2).
  Objective (Grand Crusader's Command, Crimson Courier, WPL) rides a
  WPL expedition leg; turn-in Nathanos, WPL.

The Owen Thadd library (Mage Quarter, Owen 1458 @73.4,33; turn-ins
Owen / Garion Wendell, Stormwind - the Stormwind leg is a hostile-city
expedition, routed honestly with the risk noted):
- Primer chain: 78150 Friend of the Library (20/1) - 79536 Greater
  Friend of the Library (35/20; pre 78150) - 82208 Greater Friend of
  the Library (45/35; pre 79536). No objectives; pure hand-ins.
- 40-book Research Access chain, every book accepted from Owen (or
  Oran for the eight), objective from its book object, turn-in back:
  78124, 78127, 78142, 78143, 78145, 78146, 78147, 78148, 78149,
  79091, 79092, 79093, 79094, 79095, 79096, 79097, 79535, 79947,
  79948, 79949, 79950, 79951, 79952, 79953 (79953's item sourceless -
  R2 bag note), 81947, 81949, 81951, 81952, 81953, 81954, 81955,
  81956, 84395, 84396, 84397, 84398, 84399, 84400, 84401, 84402 -
  then capstone 97286 Research Access (20/1; pre all 40 books, `only
  Mage`). Book objects span Darkshore, Silverpine (x2), Westfall, Barrens (x3),
  Wetlands, Duskwood, Loch Modan (x2), Stonetalon, Ironforge, Elwynn,
  Orgrimmar, Tirisfal, Tanaris, Feralas, Azshara, Searing Gorge, Burning
  Steppes (x2), Hillsbrad, Blasted Lands, EPL (x2), Felwood, WPL (x3),
  Winterspring, Stranglethorn, Thousand Needles, Alterac, Arathi, Desolace,
  Badlands, Dustwallow, Swamp of Sorrows -
  grouped into expedition legs by destination; the 84395-84402
  turn-ins use the Oran (UC) end.

## Tirisfal-17 reconciliation

The Tirisfal census set aside 17 dual-spawn quests to this city; all
17 are contracted here: 357, 366, 446 (Bethor); 1882, 1943, 1947,
1953, 1960, 1961 (Anastasia); 4489, 4739, 4969 (Kaal); 5643, 5657,
5658, 5679 (Aelthalyste); 65593 (Godrick). Tirisfal also noted matches
of already-OUT quests resolving to city NPCs (1718, 1823, 1947, 1953,
8250, 8417): those are IN here as their own UC legs (multi-city
precedent). Tirisfal's BORDERLINE notes on 79095 (kept here - the
primer object sits in Brill but the quest accepts from Owen on 1458)
and 95328 (kept here - the residues drop in Tirisfal but the quest
accepts via the item and turns in at Biet) are concurred.

97022 stays in Thunder Bluff (homed there last round; dual 1456+1458
starter). Zero zone-contract overlap: not contracted here.

## OUT by rule

- Seasonal/event: 7024 (Winter Veil); 8648 (Lunar elder); 8867, 8873,
  8874, 8875, 8883 (Lunar); 8904, 8979, 8980, 8981, 8982, 8983, 8984,
  8993 (Love is in the Air); 9322, 9323, 9368, 9386, 9388, 9389, 9339,
  9365 (Midsummer); 8793 (AQ war effort); 8816, 8817, 8824, 8826, 8840,
  8841 (commendation signets, war-effort turn-ins); 1657, 8322 (ev12,
  calibrated seasonal by 8354 Chicken Clucking); 9265, 9154 (ev17,
  Scourge Invasion event).
- Repeatables: 7819 (Additional Runecloth); 9333, 9334, 9335, 9336,
  9343, 9320 (Argent turn-ins); 98887, 98888, 98889, 98891 (Darkspear
  battleground marks; 98890 also broken - no level/end).
- Battleground brackets: 8367-8443, 8566, 8568, 8570 (not open-world
  completionist content, Alterac precedent).
- Broken/incomplete: 60860 (no level/min, multi-city starter mush -
  same call as prior cities); 9310 (starter resolves to the unrelated
  Blood Guard's Chain Boots item, no placed source); 98890;
  1547/1811/1812 (nonexistent IDs from an early scan).
- Accepts outside: 1778 (Ironforge paladin), 611 (STV Alliance), 844
  (Barrens), 1654 (Dun Morogh paladin), 596 (STV), 1945 (Durotar),
  1948/1952/1954/1958 (Dustwallow mage line), 1959 (no 1458 starter;
  Orgrimmar+Thunder Bluff's), 6144/6146/6147/6148 (WPL chain),
  4490/1796/1799 (Barrens warlock follow-ups), 7489 (Feralas),
  4134/4768 (Badlands), 5096 (Tirisfal), 5093 (Orgrimmar), 5095
  (Thunder Bluff), 1841 (Barrens), 3638/3642 (engineering follow-ups),
  444/448 (Silverpine), 405/409 (Tirisfal), 7563 (Searing), 8421
  (Felwood), 1944 (Durotar), 2379 (uncontracted follow-up), 1719,
  1824, 8234, 8251, 8423 (uncontracted chain follow-ups).
- Wrong faction: 611 (Alliance-only; accepts in STV, noted).
- Already homed elsewhere (noted, never double-contracted): 451
  (Silverpine), 1123 (Thunder Bluff), 1899 (uncontracted pre of 1978 -
  structural warning), 1959 (Orgrimmar+Thunder Bluff), 6071
  (Darnassus), 97022 (Thunder Bluff).

## BORDERLINE (argued, none silent)

- 84395-84402 zonefield 1453 + Stormwind co-starter/end: IN by the UC
  starter (Oran) under the accept rule; the Jennea ends are the
  Alliance legs of a shared record. The guide uses the Oran ends only.
- 7813-7818 (AQ-adjacent cloth, no event/repeat flags): IN as one-time
  quests with bag-note completes (TB 768/769 precedent); 7819 OUT.
- 9310: excluded as broken (starter is an unrelated item ID), not as
  an item-start - the record has no valid source anywhere.
- 1657/8322: ev12 calibrated seasonal via 8354 (known Noblegarden),
  not open-world content.
- 9265/9154: ev17 is the Scourge Invasion event set (9085/9153 WPL
  60s, 9260/9261 faction twins) - event-gated, OUT despite 1458 keys.
- 1960's split objective (one placed UC object, one sourceless item):
  placed complete + bag note in the same mini-step.
- 1472/1476 level -1: scaling records, IN; XP-model noise class.
- 4293/4294/4642 zonefield 1421: IN by the dual-spawn city-NPC starter
  (Mulgore-Thunder Bluff precedent for dual starters).
- 1959: OUT three ways (no 1458 starter; homed in Org+TB; Tirisfal's
  above-band note moot here). 1960's soft-pre mini-step covers the gap.
- Multi-city legs (1718/1823/8233/8250/8417/1947/1953/7562/8419):
  contracted per-city per the 8151/8250/8417 precedent. Single-starter
  quests never double (97022 stays Thunder Bluff's).

## In-city vendor recipe stock (for the future Horde city recipes round)

33 recipe items sold by vendors spawning on 1458, by profession:
Tailoring 13 (Millie Gregorian 8: Red Woolen Bag, Greater Adept's
Robe, Tuxedo set x3, Linen/Woolen Reagent Bags x2 shared with Angela
Ward; Joseph Moore 3: Green Whelp Bracers, Barbaric Bracers,
Mystic/Forceful Medium Armor Kits x2; Gishah 1: Phoenix Bindings;
Thaddeus Webb 1: Enchanted Mageweave Pouch); Cooking 10 (Lizbeth
Cromwell 4: Brilliant Smallfish, Longjaw, Rockscale Cod, Mithril Head
Trout; Ronald Burch 4: Bristle Whisker, Rainbow Fin, Smoked Sagefish,
Sagefish Delight; Nardstrum Copperpinch 2 SEASONAL: Gingerbread
Cookie, Egg Nog); Alchemy 3 (Algernon 2: Elixir of Shadow Power,
Superior Mana Potion; Gishah 1: Lesser Arcane Elixir); Enchanting 5
(Thaddeus Webb 4: Minor Mana, Minor/Lesser Wizard Oil, Minor Mana
Oil; Daniel Bartlett 1: Greater Stamina); Blacksmithing 1 (Gishah:
Mantle of the Second War); Engineering 1 (Gishah: Soul Vessel).
No city rares (no 1458 spawn carries a rare flag in the data).

## Addendum - quest 1899 contracted; 1472/1476 turn-in corrections (chain-order audit)

- 1899 The Deathstalkers (13/10, only Rogue,Undead): accept Andron Gant
  (1458 @54.81,76.33), objective Andron's Ledger from Andron's Bookshelf
  (object 103600, 1458 @55.4,76.96), turn-in Mennet Carkad (1458
  @83.51,69.11). The census listed 1899 only as "uncontracted pre of 1978"
  without evaluating it; the chain-order audit showed it is an in-band
  city-key accept, so it contracts here by the accept rule (Mulgore
  781/98424 precedent). It routes in the returns block between 1898's
  turn-in and 1978's accept, which also clears 1978's structural warning.
  Contract: 107 -> 108 quests.
- 1472 Devourer of Souls: the census called this accept-only, but the data
  carries end.npc Godrick Farsan (1458 @84.81,14.83) and the compiler
  demands its turn-in for 1476/65593. Corrected: talk leg Carendin ->
  turn in to Godrick in the Magic Quarter hub step; no addendum quest,
  contract count unchanged, and the 1476/65593 chain warnings clear.
- 1476 Hearts of the Pure: turn-in is Carendin Halgar (1458 @85.06,25.99),
  not Godrick - the guide turns it in to Carendin in the returns block.
- 1899's evaluation corrects the rogue mini-step note that claimed
  "1899 accepts nowhere in the data": it accepts at Andron Gant on the
  city key. The Varimathras 1978 mini-step is removed (1978 routes in
  the returns block after 1899's turn-in).
