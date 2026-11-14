# Stormwind City census (pack 0.15.0)

Every quest in the local data (questie-forever, `--product wowf` + QuestieDB)
whose accept/start is in Stormwind City (zone 1453): **238 candidates**.
A capital is not a leveling band, so there is no band cutoff — the census span
is quest level 1-60 (min-levels 1-60), plus one special (1716, level -1, min 20)
and one null-min record (99435, OUT as unroutable — see below).

Disposition: **189 IN**, 49 OUT. The contract (`docs/quest-contracts.json`,
slug `stormwind-city`, order 8, levelBand `1-60`) holds exactly the 189.

## Method

Accept/start decides: an NPC start with a 1453 spawn, an in-city object start,
or an item start whose source is city-bound. A quest that merely turns in here
but accepts elsewhere is not a Stormwind quest (4485, 7781). Mutually exclusive
variants are decided once: the zone-level variant already contracted in an
earlier round wins and the Stormwind twin stays out (94824/94817 precedent).
Same-name same-chain twins are both contracted (Harvesting the Harvesters
precedent: 72/74, 335/336).

## IN (191)

Stalvan twins 72, 74 (74 starts at the Sealed Crate obj1561 @1453); Messenger
121; the NAMED Wilder pair 167, 168 (data still says 1453 starts — contracted);
212; 270; 325; wine-shop errands 332, 333, 334; Noble Brew twins 335, 336;
343, 344; 350; 353 (pre 1097 out-of-zone — structural); Stockade chain 387,
388, 389 (pre 373 is OUT — structural), 391, 392, 393; Defias endgame 394, 395,
396 (434 pre 2746, both IN); 397 (Warlock); 399; 434, 2745, 2746; 538 (pre 337
is OUT — structural); 543; library chain 579, 97234, 97237; 690; 1015;
the NAMED Collin Mauren pair 1076 (pre 1075 out-of-zone — structural), 1077,
plus 1078; Missing Diplomat chain 1274, 1241, 1242, 1243, 1246 (pre 1245
out-of-zone — structural), 1447, 1247, 1248; Angus Stern 1260, 1271 (pre
1222/1258 out-of-zone — structural); 1363, 1364; Brohann chain 1448, 1449,
1475 (pre 1469 out-of-zone — structural), 1477; Bartleby warrior chain 1639,
1640, 1665, 1666; Human paladin Divinity chain 1641, 1642*, 1643, 1644, 1780,
1781, 1786, 1788 (pre 1787 uncontracted Elwynn — structural), 1790; Valor chain
1649*, 1650, 1653 (pre 1652 uncontracted Westfall — structural), 1793; 1661;
Gakin warlock chain 1688 (pre out-of-zone), 1689, 1739 (pre out-of-zone),
65603 (pre out-of-zone), 1798 (dual Ironforge/Stormwind accept — the Stormwind
accept counts); Furen/Grimand warrior chain 1700 (Human), 1701 (pre 1702
out-of-zone Redridge — structural), 1703 (Night Elf), 1704 (Dwarf+Gnome), 1705,
1706, 1782; 1716 (level -1, min 20, Warlock infernal ritual); Jennea mage chain
1861, 1920 (pre 1919 out-of-zone — structural), 1921, 1938 (pre 1939
out-of-zone — structural), 1940, 1941, 1942; 2040 (pre 2041 out-of-zone —
structural); 2923; 2928; SI:7 rogue chain 2206, 2281 (pre out-of-zone —
structural), 2360, 2607 (pre 2359 out-of-zone — structural), 2608, 2609; Hank
2758, 2759; 3630 Gnome Engineering (excl list is all uncontracted); 3636;
3765; 3787 (pre 3781 out-of-zone — structural); 3789; Bolvar True Masters
4185 (pre 4184 out-of-zone — structural), 4186; warlock mount chain 4488, 4738,
4968 (their Ironforge/Gnome/Barrens twins are uncontracted — the Stormwind
variants are the Alliance-Human ones); 4766; Emma chain 5048 (pre 5022
out-of-zone — structural), 5050 (pre 5049 Undercity — structural); 5066;
Laurena priest singles 5645 (Dwarf), 5673 (Night Elf), 5676 (Human), 94819
(Gnome — its twins 94818/94820 are uncontracted Dun Morogh/Darnassus); 6141;
dragon chain 6182, 6183, 6184, 6187 (pre 6186 out-of-zone — structural); Human
flight pair 6261 (pre 6281 Westfall-contracted — structural), 6285; Windsor
chain 6403 (pre 6402 out-of-zone Redridge — structural), 6501; 7494; 7562
(multi-city warlock accept — the Stormwind accept counts); epic-mount paladin
chain 7637, 7638, 7640 (pre 7639 out-of-zone — structural), 7641, 7642, 7643,
7646 (pre 7644 is OUT — structural), 7647, 7648, 7666; 7782 (pre 7781 is OUT —
structural); cloth donations 7791, 7793, 7794, 7795; 8415; 8419 (multi-city
warlock accept); 92415* (item start, see BORDERLINE), 92456, 92489; 93963
(Skyborne, pre 94947 out-of-zone — structural); 94914 (Skyborne Druid); 95065
(optional — profession unconfirmed, see BORDERLINE); 95161 (pre 92415);
95194; 96676; Philmor pair 97220, 97222; 97894; 97926 (pre 97914 uncontracted
Darkshore — structural); 98191 (pre 98190 out-of-zone Wetlands — structural);
98219; Katherine chain 78090 (pre 78089 uncontracted Ashenvale — structural),
78091, 78092, 79940 (pre 79939 out-of-zone — structural), 96438; 81762, 81764;
book quests 84395-84402 (NPC accept in-city; book objects out-of-zone —
expedition completes); Colara chain 8897, 8903, 9024, 9025, 9026, 9027, 9028.

\* 1642, 1649, 92415 are item-starts whose items have NO source in the data
(no drops, no vendors, no object). They are chain links (1641→1642→1643,
→1649→1650, 92415→95161): the items are presumed granted by the pre-quest
line (quest rewards are not in quest records). They ship with a note saying so
and their accepts sit immediately after the pre-quest turnin. The honest
playtest's R2 findings on them are accepted data-gap noise.

## OUT (49)

- Seasonal/event (15): Children's Week 558, 1468, 1479, 1558, 1687, 4822;
  Winter Veil 7023; Hallow's End 8311, 8356; Lunar Festival 8646; Scourge
  Invasion 9260, 9292 (9292's starter is also spawnless); AQ war-event 7495
  (accept is the raid-drop Head of Onyxia, not the city), 7496, 7497.
- Repeatables (3): 8814, 8822 (commendation signets), 7796 (Additional
  Runecloth — the one-time 7791/7793/7794/7795 stay IN).
- Broken/unroutable (10): 373 (item source npc639 Edwin VanCleef has no spawns
  anywhere); 7644 (starter npc14566 Ancient Equine Spirit has no spawns —
  7646's pre goes structural); 79970 (starter npc217996 Aeonas has no spawns);
  79946 (pre 79945 is OUT-broken AND its turnin is the same spawnless Aeonas —
  double-broken); 79945, 81766, 96377 (empty start records); 95189 (item from
  obj614679, which has no spawns); 95195 (item drops from spawnless SoD NPCs);
  99435 (no turnin in the data — accept-only records cannot satisfy the
  contract).
- Accept not in the city (3): 4485 (accept is Tiza Battleforge @Ironforge —
  the Ironforge guide will own it; its turnin here is noted as a chain-link);
  7781 (accept is the raid-drop Head of Nefarian); 337 (An Old History Book
  drops from dozens of low-level NPCs zone-wide — a generic world-drop start,
  so the accept is not city-bound; 538's pre goes structural).
- Already routed in another guide (7): 141, 92749, 92750, 92751, 92752 (all in
  the Westfall contract); 98021 (routed in westfall.guide accept 143/turnin
  249 — the Stormwind guide notes the flight chain but does not re-route it).
- Mutually exclusive, zone variant wins (11): 3000 (Dun Morogh 2997
  contracted); 5631, 5632 (Teldrassil 5629 / Dun Morogh 5630 contracted);
  5634, 5638 (Teldrassil 5636 / Dun Morogh 5637 contracted); 5924 (Teldrassil
  5925 contracted); 6073 (Teldrassil 6072 contracted); 6076 (Dun Morogh 6075
  contracted); 94773, 94777 (Elwynn 94774 / Dun Morogh 94776 / Teldrassil 94775
  contracted); 94821 (Teldrassil 94823 / Dun Morogh 94824 contracted).
- Twin not picked (1): 4181 Goblin Engineering (Gnome 3630 contracted).

## BORDERLINE (argued inline, none decided silently)

1. **1642 / 1649 / 92415 (sourceless item-starts): IN.** The items (6775 Tome
   of Divinity, 6776 Tome of Valor, 251270/251520 parchments) have no drops,
   vendors or objects anywhere in the data, yet each sits mid-chain with
   contracted neighbors on both sides (1641→1642→1643, →1649→1650,
   92415→95161). The only consistent reading is that the item is granted by
   the pre-quest line (rewards are not in quest records). Out would gut three
   real chains; in with an honest note preserves them. Accepted risk: the
   honest sim flags their accepts (R2) — reported, not fixed.
2. **84395-84402 (book quests with out-of-zone object starts): IN.** Each
   lists BOTH a Stormwind NPC accept (Jennea Cannon) and a book-object start
   on another continent. The NPC accept satisfies the accept rule; the books
   become expedition completes. No seasonal/repeatable/excl markers anywhere.
3. **8897-9028 (Colara chain): IN, regular.** Level 60 min 1 looks event-ish,
   but the chain carries faction twins (8898 Ironforge, 8899 Teldrassil, 8984
   Horde-side) — events do not ship mirrored faction twins with pres chains.
   Regular chain, all seven IN.
4. **95065 (Fishin' Time): IN, optional, ungated.** From Gilbert Gray with no
   class lock and no profession marker in the data. Gating it Fishing would
   hide a quest a non-fisher could do; leaving it ungated and optional never
   wedges anyone.
5. **94819 (Contingency Plan): IN.** Its excl twins (94818 Dun Morogh, 94820
   Darnassus) are both uncontracted, so the Stormwind Gnome variant is the
   only contracted one — no conflict.
6. **5645 / 5673 / 5676: IN.** Their excl twins are all uncontracted
   (Ironforge/Darnassus/Teldrassil variants), so no contracted twin exists.
7. **335/336 and 72/74 (same-name twins): BOTH IN** per the Harvesters
   precedent — same chain, both doable, player-told-apart by note.
8. **6261/6285 (Human flight pair): IN, only Human.** 6281 is
   Westfall-contracted; 6261's pre is structural. Skyborne use 98021 (already
   routed in westfall.guide) — the guide notes this instead of re-routing.
9. **93963 (Exploring the Alliance): IN, only Skyborne.** Races bit32 is the
   Skyborne bit (98021 carries the same mask and the Westfall round reads it
   Skyborne-only). Objectives kill the four Alliance leaders — the data says
   kill; the step notes what that means rather than editorializing.
10. **99435: OUT.** Accept-only record (no turnin in the data) cannot satisfy
    the accept-once-turn-in-once contract.
11. **3000 / 94821 / 5924 / 6073 / 6076 / 5631-5638 / 94773-94777: OUT.**
    Each is mutually exclusive with a variant already contracted in a zone
    guide, and the zone variant is chain-consistent (players meet it first in
    level order). The Stormwind twin stays out with this reason, not silently.

## Companion question (no building this round)

- City-vendor recipes: **30 distinct recipes** sold by 1453-spawning vendors
  (32 vendor links), incl. Kendor Kabonka's 13-recipe Cooking stock, Alexandra
  Bolero's tailoring, Catherine Leland's and Erika Tate's fish recipes, Kaita
  Deepforge's plans, Darian Singh's firework schematics, Maria Lumere's
  elixir, Jessara Cordell's pouch pattern, Jillian Tanner's armor kits, the
  Boleros' reagent bags. Deserves its own recipes companion later.
- City rares: **360 NPCs** spawn on 1453, but the dump is all trainers,
  vendors, quest NPCs and guards on inspection — no rare sweep was run (out
  of scope). Count reported, sweep deferred to a companion round if one is
  ever scoped.
