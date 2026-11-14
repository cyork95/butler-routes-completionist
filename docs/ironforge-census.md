# Ironforge census (pack 0.16.0)

Every quest in the local data (questie-forever, `--product wowf` + QuestieDB)
whose accept/start is in Ironforge (zone 1455, confirmed from the data —
Stormwind City is 1453, Darnassus is 1457): **345 candidates**.

A capital is not a leveling band, so there is no band cutoff; the census span
is quest level 1-60 (min-levels 1-60), no null-level or negative-level records
among the contracted set (60860, the one null-level record, is OUT as broken).

Disposition: **188 IN**, 157 OUT. The contract (`docs/quest-contracts.json`,
slug `ironforge-city`, order 9, levelBand `1-60`) holds exactly the 188.

## Method

Accept/start decides: an NPC start with a 1455 spawn, an in-city object start,
or an item start whose source is city-bound. Multi-starter quests keep every
city starter (7494/8415/8419/7562/1798 precedent — the Stormwind census
already notes 1798 as a dual Ironforge/Stormwind accept; both guides route
their own accept). A quest that merely turns in here but accepts elsewhere is
not an Ironforge quest (3461, 3645, 8796, 8797). Same-name sequential twins
are both contracted (Harvesting the Harvesters precedent: 1073/1074,
3451/3483, 1179/2769 Brassbolts). Mutually exclusive variants are decided
once — the BORDERLINE section argues each pick (4485/4486, 3629/3632,
5283/5284). Item starts with no source in the data ship with a bag note and
no collect line (Stormwind 1642/1649 precedent). Zone-flag quirks defer to
the giver map: 4485 is flagged 1453 but its giver Tiza spawns only on 1455,
so it is Ironforge's; 8151/8233/8417 are flagged 1454 (Mulgore) but accept
in the city, so they are Ironforge's with the flag noted.

## IN (188)

Stormpike/Uldaman arc: 302 (pre 301, contracted in the Loch Modan guide —
chain from Loch Modan), 525 (pre 514 Hillsbrad — structural), 707, 2398
(objectives in Uldaman — complete at the entrance with a note), 2439 (pre
2279, OUT in Uldaman — structural), 2963 (pre 2439), 2946 (pre 2963), 1050,
762 (pre 726), 726 (pre 725), 725 (pre 724 Wetlands — structural), 1139
(pre 762).

Balloo/Magni tribute chain: 637*, 683 (pre 637), 686 (pre 683), 689
(pre 686), 700 (pre 689).

Gerrig chain: 687 (pres 653 sourceless / 688 Horde — structural), 971, 735
(pre 727 Wetlands — structural), 737 (pre 735, excl 736 Horde variant).

Item singles: 708* (Black Box), 968* (Powers Below).

Frontier and breadcrumbs: 1019 (ends at Arch Druid Fandral Staghelm —
breadcrumb toward Darnassus; excl 1015 Stormwind-contracted / 1047), 5090
(excl 5066 Stormwind-contracted), 8275 (excl 8276 Mulgore), 1453, 1578, 1618.

Dwarf Paladin Divinity chain: 1645, 1646*, 1647, 1648, 1778, 1779, 1783,
1785 (pre 1784, a Stormwind accept uncontracted anywhere — structural),
1789; Valor twin 1794 (excl 1793 Stormwind-contracted); Nobility 4485 (excl
4486, OUT as the giver-choice twin — see BORDERLINE; ends at Duthorian Rall
in Stormwind, an expedition turnin); 2999 (excl 2997 Dun Morogh-contracted /
2998 / 3000); Human 3681 (excl 2998); 7639 (pre 7637 Stormwind-contracted);
7670 (excl 7638 Stormwind-contracted); 8415 (also contracted in Stormwind —
Stormwind-overlap, Ironforge starter routed here).

Warrior: 1678 (excl 1639 Stormwind-contracted / 1683 Kalimdor), 1680, 1681,
1682, 1698 (chain ends outside the city), 1708 (pre 1704
Stormwind-contracted), 1709, 1718 (Fray Island leg), 8417 (zone-1454 flag
noted — accept decides).

Warlock: 1715 (excl 1685 Elwynn-accept uncontracted / 1688
Stormwind-contracted), 1717 (excl 1716 Stormwind-contracted), 1798
(Stormwind-overlap — Lago Blackwrench spawns only on 1455, so the
Ironforge accept is contracted here too), 1802 (pre 1758 Razorfen — structural),
1804, 1360, 4487 (excl 3631/4488/4489), 4736 (excl 4737/4738/4739), 4965
(excl 4967/4968/4969), 8419 (Stormwind-overlap — Briarthorn spawns only on
1455), 7562 (Stormwind-overlap — Jubahl Corpseseeker spawns only on 1455,
zone-1453 flag noted like 1798).

Mage: 1880 (Human/Gnome, excl 1861), 1919 (Human/Gnome), 1939, 1947, 1953,
2861, 8250.

Gnoarn: 2039, 2041 (ends at Shoni the Shilent in Stormwind — breadcrumb),
2927.

Talvash necklace chain: 2198*, 2199, 2200, 2204 (pre 2201, OUT — accept in
Uldaman, structural), 2361 (pre 2204), 3375 (pre 2201 — structural), 2948
(pre 2947, OUT — accept in Gnomeregan, structural).

Rogue: 2238, 2298 (pre 2299, a Dun Morogh accept uncontracted anywhere —
structural; excl 2260 Kalimdor / 2300 Elwynn-accept), 6681* (item start by
pickpocketing Hulfdan, Ormyr or Fenthwick in the city — tagged), 8233
(zone-1454 flag noted — accept decides).

Klockmort: 2922 (pre 2923 Stormwind-contracted), 2924 (pre 2925, a
Darnassus/Desolace accept — structural), 2769; Brassbolts same-name twins
1179 (Pilot Longbeard) and 2769 — both IN.

Tinkmaster engineering: 2929, 2930 (pre 2931 Stonetalon — structural),
3640 (excl 3638 Tanaris / 3642 Horde), 3641 (excl 3638 / 3639 Tanaris),
3632 Gnome (excl list includes OUT twin 3629 — see BORDERLINE), 3647
(pre 3643 STV — structural; the Ironforge accept of the STV chain).

Karnik/Tymor/Xiggs: 3448, 3449, 3450, 3451, 3483 (3451/3483 are same-name
sequential twins — both IN), 2964 (pre 2977 Tanaris — structural).

Thorius: 3701, 3702, 3201 (pre 3182, a Loch Modan accept uncontracted
anywhere — structural), 3371 (pre 3368 Searing Gorge — structural), 95924,
95925.

Magni endgame: 4341 (pre 3701), 4362 (pre 4361, OUT — accept unplaceable,
structural).

Slime: 4512, 4513.

Priest racials: Dwarf 5639, Dwarf 5641 (excl 5645/5647), Night Elf 5675
(excl 5672/5673/5674), Human 5677 (excl 5676/5678), Human 94778, 8254
(null-races record — gated Priest only).

Hunter: Dwarf 6074 (excl 6075/6076), Night Elf 6721 (excl 6071/6072/6073/
6722), Night Elf 5633, 8151 (zone-1454 flag noted — accept decides).

Gryphon chain: 6388 (pre 6391 Dun Morogh-contracted), 6392.

Hinterlands trio: 6609, 6612, 6625. Silithus/Twilight: 7261, 7342.

Feathermoon 7494 (Stormwind-overlap — Hammerfall spawns only on 1455).

Donations: 7802, 7803, 7804, 7805 (Mistina Steelshield), 7807, 7808, 7809,
7811 (Bubulo Acerbus); 7806/7812 are the repeatable Additional Runecloth
turn-ins — OUT.

Shaman: 94449, 94494, 94789 (Eldrun Stormbreaker), 96243 (Dwarf/Gnome —
gated per the data), 96264 (pre 94789), 79358 (pre 96264 — Veyric
Thunderhame spawns in the city), 96135 (pre 79358, excl 79366 Thousand
Needles), 96016 (pre 79366 Thousand Needles / 96135 alternative pres,
excl 79442 Thousand Needles).

Gnome Priest: 94817 (High Priestess Mims dual-spawns Dun Morogh and
Ironforge — the city accept is contracted here; Dun Morogh does not
contract it; excl the other-race twins), 94818 (pre 94819
Stormwind-contracted, alternative 94820 Darnassus uncontracted).

Camping 101: 96045 Alchemy, 96059 Enchanting (optional + `when skill`
gated; pres include 95998 Elwynn-contracted, the rest out-of-scope —
structural).

Afadra/Thom: 96394, 96403. Longbeard opener: 467. Moonglade link: 3790
(excl 3763 Darnassus / 3789 Stormwind).

Object/item starts: 97263* (Misplaced Packages object, ends at Eldrun in
the city — self-contained), 98423* (Treaty of Understanding, no source in
the data — bag note), 79091* (Library Book object in the Hall of
Explorers; the Uldaman and Stormwind co-starters are uncontracted —
see BORDERLINE).

Deliana dungeon-tier set: 8905, 8906, 8907, 8908, 8909, 8910, 8911, 8912
(one per class), 8922, 8926, 8931, 8932, 8933, 8934, 8935, 8936, 8937 (pre
8977 Tanaris — structural), 8929 (pre the eight class variants), 8960
(pre 8951-8959 Eastern Plaguelands — structural), 8999, 9000, 9001, 9002,
9003, 9004, 9005, 9006 (pre 8997 — structural).

Starred (*) quests are item- or object-started; sourceless ones ship with a
bag note and no collect line.

## OUT (157)

- 2201 | Find the Gems | lvl43/min37 | (zone-flagged 1455 only) — DUNGEON-OUT: accept is the Remains of a Paladin inside Uldaman (no city spawn data) — chain continues via contracted 2204/3375 (structural pres)
- 2240 | The Hidden Chamber | lvl40/min35 | (zone-flagged 1455 only) — DUNGEON-OUT: accept is Baelog inside Uldaman (no city spawn data) — chain continues via contracted 2439 (structural pre)
- 2279 | The Platinum Discs | lvl47/min40 | (zone-flagged 1455 only) — DUNGEON-OUT: accept is the Discs of Norgannon object inside Uldaman (no city spawn data) — chain continues via contracted 2439 (structural pre)
- 2947 | Return of the Ring | lvl34/min28 | (zone-flagged 1455 only) — DUNGEON-OUT: accept is the Sparklematic 5200 object inside Gnomeregan (no city spawn data) — 2924 contracted with structural pre
- 3461 | Return to Tymor | lvl52/min45 | (zone-flagged 1455 only) — NOTCITY-OUT: accept Pilot Xiggs Fuselighter @1447 Wetlands (outside city); Tymor chain contracted through 3451/3483
- 3629 | Goblin Engineering | lvl47/min30 | npc5174:Springspindle Fizzlegear@[[68.46,43.54]] — TWIN-OUT: Goblin Engineering — mutually exclusive with contracted Gnome 3632 (pack-consistent Gnome pick per Stormwind 3630)
- 3645 | Membership Card Renewal | lvl47/min30 | (zone-flagged 1455 only) — NOTCITY-OUT: accept Oglethorpe Obnoticus @1434 STV (outside city); Tinkmaster chain contracted through 3641
- 4361 | The Bearer of Bad News | lvl59/min50 | (zone-flagged 1455 only) — DUNGEON-OUT: accept NPC Kharan Mighthammer has no spawn data anywhere — cannot place accept in Ironforge; chain continues via contracted 4362 (structural pre)
- 4363 | The Princess's Surprise | lvl59/min50 | (zone-flagged 1455 only) — DUNGEON-OUT: accept NPC Princess Moira Bronzebeard has no spawn data anywhere — cannot place accept in Ironforge
- 4486 | The Tome of Nobility | lvl40/min40 | npc5149:Brandur Ironhammer@[[23.13,6.14]] — TWIN-OUT: mutually-exclusive giver-choice twin of contracted 4485 (same name/eligibility/destination) — guide routes 4485, note names the swap
- 5284 | The Way of the Weaponsmith | lvl40/min40 | npc11146:Ironus Coldsteel@[[50.33,43.56]] — TWIN-OUT: Way of the Weaponsmith — mutually exclusive with contracted 5283 (lower-ID pick, no chain differentiator) — guide routes 5283, note names the swap


- 7022 | Greatfather Winter is Here! | lvl60/min10 | npc13433:Wulmort Jinglepocket@[[33.7,67.23]] — EVENT-OUT (event flag 2)
- 7025 | Treats for Greatfather Winter | lvl60/min10 | npc13444:Greatfather Winter@[[33.2,65.41]] — EVENT-OUT (event flag 2)
- 7042 | Stolen Winter Veil Treats | lvl60/min30 | npc13433:Wulmort Jinglepocket@[[33.7,67.23]] — EVENT-OUT (event flag 2)
- 7045 | A Smokywood Pastures' Thank You! | lvl60/min30 | npc13433:Wulmort Jinglepocket@[[33.7,67.23]] — EVENT-OUT (event flag 2)
- 7062 | The Reason for the Season | lvl60/min10 | npc1365:Goli Krumn@[[30.26,59.38]] — EVENT-OUT (event flag 2)
- 7063 | The Feast of Winter Veil | lvl60/min10 | npc2916:Historian Karnik@[[77.54,11.82]] — SEASONAL-OUT: Feast of Winter Veil (no event flag in data; seasonal by name + chain from flagged 7062)
- 7806 | Additional Runecloth | lvl60/min50 | npc14723:Mistina Steelshield@[[43.22,31.57]] — REPEATABLE-OUT: repeatable cloth turn-in
- 7812 | Additional Runecloth | lvl60/min50 | npc14724:Bubulo Acerbus@[[74.09,48.22]] — REPEATABLE-OUT: repeatable cloth turn-in
- 7905 | The Darkmoon Faire | lvl60/min6 | npc14842:Melnan Darkstone@[[29.65,75.25]] — EVENT-OUT (event flag 4)
- 8228 | Could I get a Fishing Flier? | lvl60/min35 | (zone-flagged 1455 only) — EVENT-OUT (event flag 14)
- 8229 | Could I get a Fishing Flier? | lvl60/min35 | npc15119:Barrus@[[28.17,74.95]] — EVENT-OUT (event flag 14)
- 8353 | Chicken Clucking for a Mint | lvl60/min10 | npc5111:Innkeeper Firebrew@[[18.15,51.45]] — EVENT-OUT (event flag 12)
- 8355 | Incoming Gumdrop | lvl60/min10 | npc6826:Talvash del Kissel@[[36.38,3.61]] — EVENT-OUT (event flag 12)
- 8371 | Concerted Efforts | lvl60/min51 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground mark turn-in
- 8372 | Fight for Warsong Gulch | lvl19/min10 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8374 | Claiming Arathi Basin | lvl29/min20 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8375 | Remember Alterac Valley! | lvl60/min51 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8383 | Remember Alterac Valley! | lvl60/min51 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8384 | Claiming Arathi Basin | lvl29/min20 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8385 | Concerted Efforts | lvl60/min51 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground mark turn-in
- 8386 | Fight for Warsong Gulch | lvl19/min10 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8391 | Claiming Arathi Basin | lvl39/min30 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8392 | Claiming Arathi Basin | lvl49/min40 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8393 | Claiming Arathi Basin | lvl39/min30 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8394 | Claiming Arathi Basin | lvl49/min40 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8395 | Claiming Arathi Basin | lvl59/min50 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8396 | Claiming Arathi Basin | lvl60/min60 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8397 | Claiming Arathi Basin | lvl59/min50 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8398 | Claiming Arathi Basin | lvl60/min60 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8399 | Fight for Warsong Gulch | lvl29/min20 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8400 | Fight for Warsong Gulch | lvl39/min30 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8401 | Fight for Warsong Gulch | lvl49/min40 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8402 | Fight for Warsong Gulch | lvl59/min50 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8403 | Fight for Warsong Gulch | lvl60/min60 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8404 | Fight for Warsong Gulch | lvl29/min20 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8405 | Fight for Warsong Gulch | lvl39/min30 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8406 | Fight for Warsong Gulch | lvl49/min40 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8407 | Fight for Warsong Gulch | lvl59/min50 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8408 | Fight for Warsong Gulch | lvl60/min60 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground quest
- 8492 | The Alliance Needs Copper Bars! | lvl60/min1 | npc15383:Sergeant Stonebrow@[[64.1,65.5]] — EVENT-OUT (event flag 22)
- 8493 | The Alliance Needs More Copper Bars! | lvl60/min1 | npc15383:Sergeant Stonebrow@[[64.1,65.5]] — EVENT-OUT (event flag 22)
- 8494 | The Alliance Needs Iron Bars! | lvl60/min1 | npc15431:Corporal Carnes@[[65.5,63.9]] — EVENT-OUT (event flag 22)
- 8495 | The Alliance Needs More Iron Bars! | lvl60/min1 | npc15431:Corporal Carnes@[[65.5,63.9]] — EVENT-OUT (event flag 22)
- 8499 | The Alliance Needs Thorium Bars! | lvl60/min1 | npc15432:Dame Twinbraid@[[63.9,68.2]] — EVENT-OUT (event flag 22)
- 8500 | The Alliance Needs More Thorium Bars! | lvl60/min1 | npc15432:Dame Twinbraid@[[63.9,68.2]] — EVENT-OUT (event flag 22)
- 8503 | The Alliance Needs Stranglekelp! | lvl60/min1 | npc15434:Private Draxlegauge@[[70.3,74.3]] — EVENT-OUT (event flag 22)
- 8504 | The Alliance Needs More Stranglekelp! | lvl60/min1 | npc15434:Private Draxlegauge@[[70.3,74.3]] — EVENT-OUT (event flag 22)
- 8505 | The Alliance Needs Purple Lotus! | lvl60/min1 | npc15437:Master Nightsong@[[71.9,70.4]] — EVENT-OUT (event flag 22)
- 8506 | The Alliance Needs More Purple Lotus! | lvl60/min1 | npc15437:Master Nightsong@[[71.9,70.4]] — EVENT-OUT (event flag 22)
- 8509 | The Alliance Needs Arthas' Tears! | lvl60/min1 | npc15445:Sergeant Major Germaine@[[71.3,71.4]] — EVENT-OUT (event flag 22)
- 8510 | The Alliance Needs More Arthas' Tears! | lvl60/min1 | npc15445:Sergeant Major Germaine@[[71.3,71.4]] — EVENT-OUT (event flag 22)
- 8511 | The Alliance Needs Light Leather! | lvl60/min1 | npc15446:Bonnie Stoneflayer@[[58,75.9]] — EVENT-OUT (event flag 22)
- 8512 | The Alliance Needs Light Leather! | lvl60/min1 | npc15446:Bonnie Stoneflayer@[[58,75.9]] — EVENT-OUT (event flag 22)
- 8513 | The Alliance Needs Medium Leather! | lvl60/min1 | npc15448:Private Porter@[[58.7,75]] — EVENT-OUT (event flag 22)
- 8514 | The Alliance Needs More Medium Leather! | lvl60/min1 | npc15448:Private Porter@[[58.7,75]] — EVENT-OUT (event flag 22)
- 8515 | The Alliance Needs Thick Leather! | lvl60/min1 | npc15450:Marta Finespindle@[[57.1,75]] — EVENT-OUT (event flag 22)
- 8516 | The Alliance Needs More Thick Leather! | lvl60/min1 | npc15450:Marta Finespindle@[[57.1,75]] — EVENT-OUT (event flag 22)
- 8517 | The Alliance Needs Linen Bandages! | lvl60/min1 | npc15451:Sentinel Silversky@[[54.5,77.9]] — EVENT-OUT (event flag 22)
- 8518 | The Alliance Needs More Linen Bandages! | lvl60/min1 | npc15451:Sentinel Silversky@[[54.5,77.9]] — EVENT-OUT (event flag 22)
- 8520 | The Alliance Needs Silk Bandages! | lvl60/min1 | npc15452:Nurse Stonefield@[[57.6,75.8]] — EVENT-OUT (event flag 22)
- 8521 | The Alliance Needs More Silk Bandages! | lvl60/min1 | npc15452:Nurse Stonefield@[[57.6,75.8]] — EVENT-OUT (event flag 22)
- 8522 | The Alliance Needs Runecloth Bandages! | lvl60/min1 | npc15453:Keeper Moonshade@[[55.7,75.9]] — EVENT-OUT (event flag 22)
- 8523 | The Alliance Needs More Runecloth Bandages! | lvl60/min1 | npc15453:Keeper Moonshade@[[55.7,75.9]] — EVENT-OUT (event flag 22)
- 8524 | The Alliance Needs Rainbow Fin Albacore! | lvl60/min1 | npc15455:Slicky Gastronome@[[71.6,69.2]] — EVENT-OUT (event flag 22)
- 8525 | The Alliance Needs More Rainbow Fin Albacore! | lvl60/min1 | npc15455:Slicky Gastronome@[[71.6,69.2]] — EVENT-OUT (event flag 22)
- 8526 | The Alliance Needs Roast Raptor! | lvl60/min1 | npc15456:Sarah Sadwhistle@[[72.1,69.6]] — EVENT-OUT (event flag 22)
- 8527 | The Alliance Needs More Roast Raptor! | lvl60/min1 | npc15456:Sarah Sadwhistle@[[72.1,69.6]] — EVENT-OUT (event flag 22)
- 8528 | The Alliance Needs Spotted Yellowtail! | lvl60/min1 | npc15457:Huntress Swiftriver@[[73,68.5]] — EVENT-OUT (event flag 22)
- 8529 | The Alliance Needs More Spotted Yellowtail! | lvl60/min1 | npc15457:Huntress Swiftriver@[[73,68.5]] — EVENT-OUT (event flag 22)
- 8565 | Past Victories in Arathi | lvl1/min1 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground mark turn-in
- 8567 | Past Victories in Warsong Gulch | lvl1/min1 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground mark turn-in
- 8569 | Past Efforts in Warsong Gulch | lvl1/min1 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground mark turn-in
- 8744 | A Carefully Wrapped Present | lvl1/min1 | obj180743:Carefully Wrapped Present@[[33.86,65.69]] — EVENT-OUT (event flag 21)
- 8762 | Metzen the Reindeer | lvl60/min40 | npc13433:Wulmort Jinglepocket@[[33.7,67.23]] — EVENT-OUT (event flag 2)
- 8763 | The Hero of the Day | lvl60/min40 | npc13433:Wulmort Jinglepocket@[[33.7,67.23]] — EVENT-OUT (event flag 2)
- 8767 | A Gently Shaken Gift | lvl1/min1 | obj180746:Gently Shaken Gift@[[33.46,65.57]] — EVENT-OUT (event flag 21)
- 8768 | A Gaily Wrapped Present | lvl20/min20 | obj180747:Gaily Wrapped Present@[[33.78,66.4]] — EVENT-OUT (event flag 21)
- 8769 | A Ticking Present | lvl40/min40 | obj180748:Ticking Present@[[33.9,66.68]] — EVENT-OUT (event flag 21)
- 8788 | A Gently Shaken Gift | lvl1/min1 | obj180746:Gently Shaken Gift@[[33.46,65.57]] — EVENT-OUT (event flag 21)
- 8795 | The Alliance Needs Your Help! | lvl60/min1 | npc15707:Master Sergeant Fizzlebolt@[[27.5,73.3]] — EVENT-OUT (event flag 22)
- 8796 | The Alliance Needs Your Help! | lvl60/min1 | (zone-flagged 1455 only) — EVENT-OUT (event flag 22)
- 8797 | The Alliance Needs Your Help! | lvl60/min1 | (zone-flagged 1455 only) — EVENT-OUT (event flag 22)
- 8803 | A Festive Gift | lvl10/min10 | obj180793:Festive Gift@[[33.96,65.86]] — EVENT-OUT (event flag 21)
- 8811 | One Commendation Signet | lvl60/min1 | npc15731:Darnassus Commendation Officer@[[61.23,69.36]] — EVENTCHAIN-OUT: commendation turn-in, pre 8795 is the AQ event quest
- 8812 | One Commendation Signet | lvl60/min1 | npc15733:Gnomeregan Commendation Officer@[[58.61,72.65]]; npc15764:Officer Ironbeard@[[43.25,46.48]]; npc15763:Officer Porterhouse@[[69.72,46.01]] — EVENTCHAIN-OUT: commendation turn-in, pre 8795 is the AQ event quest
- 8813 | One Commendation Signet | lvl60/min1 | npc15734:Ironforge Commendation Officer@[[61.11,76.97]]; npc15764:Officer Ironbeard@[[43.25,46.48]] — EVENTCHAIN-OUT: commendation turn-in, pre 8795 is the AQ event quest
- 8814 | One Commendation Signet | lvl60/min1 | npc15735:Stormwind Commendation Officer@[[63.33,69.32]]; npc15763:Officer Porterhouse@[[69.72,46.01]] — EVENTCHAIN-OUT: commendation turn-in, pre 8795 is the AQ event quest
- 8819 | Ten Commendation Signets | lvl60/min1 | npc15731:Darnassus Commendation Officer@[[61.23,69.36]] — EVENTCHAIN-OUT: commendation turn-in, pre 8795 is the AQ event quest
- 8820 | Ten Commendation Signets | lvl60/min1 | npc15733:Gnomeregan Commendation Officer@[[58.61,72.65]]; npc15764:Officer Ironbeard@[[43.25,46.48]]; npc15763:Officer Porterhouse@[[69.72,46.01]] — EVENTCHAIN-OUT: commendation turn-in, pre 8795 is the AQ event quest
- 8821 | Ten Commendation Signets | lvl60/min1 | npc15734:Ironforge Commendation Officer@[[61.11,76.97]]; npc15764:Officer Ironbeard@[[43.25,46.48]] — EVENTCHAIN-OUT: commendation turn-in, pre 8795 is the AQ event quest
- 8822 | Ten Commendation Signets | lvl60/min1 | npc15735:Stormwind Commendation Officer@[[63.33,69.32]]; npc15763:Officer Porterhouse@[[69.72,46.01]] — EVENTCHAIN-OUT: commendation turn-in, pre 8795 is the AQ event quest
- 8830 | One Commendation Signet | lvl60/min1 | npc15731:Darnassus Commendation Officer@[[61.23,69.36]] — EVENT-OUT (event flag 52)
- 8831 | Ten Commendation Signets | lvl60/min1 | npc15731:Darnassus Commendation Officer@[[61.23,69.36]] — EVENT-OUT (event flag 52)
- 8834 | One Commendation Signet | lvl60/min1 | npc15764:Officer Ironbeard@[[43.25,46.48]] — EVENT-OUT (event flag 52)
- 8835 | Ten Commendation Signets | lvl60/min1 | npc15764:Officer Ironbeard@[[43.25,46.48]] — EVENT-OUT (event flag 52)
- 8836 | One Commendation Signet | lvl60/min1 | npc15735:Stormwind Commendation Officer@[[63.33,69.32]] — EVENT-OUT (event flag 52)
- 8837 | Ten Commendation Signets | lvl60/min1 | npc15735:Stormwind Commendation Officer@[[63.33,69.32]] — EVENT-OUT (event flag 52)
- 8838 | One Commendation Signet | lvl60/min1 | npc15763:Officer Porterhouse@[[69.72,46.01]] — EVENT-OUT (event flag 52)
- 8839 | Ten Commendation Signets | lvl60/min1 | npc15763:Officer Porterhouse@[[69.72,46.01]] — EVENT-OUT (event flag 52)
- 8846 | Five Signets for War Supplies | lvl19/min10 | npc15701:Field Marshal Snowfall@[[61.3,74.2]] — EVENT-OUT (event flag 22)
- 8847 | Ten Signets for War Supplies | lvl29/min20 | npc15701:Field Marshal Snowfall@[[61.3,74.2]] — EVENT-OUT (event flag 22)
- 8848 | Fifteen Signets for War Supplies | lvl39/min30 | npc15701:Field Marshal Snowfall@[[61.3,74.2]] — EVENT-OUT (event flag 22)
- 8849 | Twenty Signets for War Supplies | lvl49/min40 | npc15701:Field Marshal Snowfall@[[61.3,74.2]] — EVENT-OUT (event flag 22)
- 8850 | Thirty Signets for War Supplies | lvl60/min50 | npc15701:Field Marshal Snowfall@[[61.3,74.2]] — EVENT-OUT (event flag 22)
- 8866 | Bronzebeard the Elder | lvl60/min1 | npc15871:Elder Bronzebeard@[[29.2,17.05]] — EVENT-OUT (event flag 7)
- 8867 | Lunar Fireworks | lvl60/min1 | npc15895:Lunar Festival Harbinger@[[28.85,16.23]] — EVENT-OUT (event flag 7)
- 8870 | The Lunar Festival | lvl60/min1 | npc15892:Lunar Festival Emissary@[[30.93,61.59]] — EVENT-OUT (event flag 7)
- 8871 | The Lunar Festival | lvl60/min1 | npc15892:Lunar Festival Emissary@[[30.93,61.59]] — EVENT-OUT (event flag 7)
- 8872 | The Lunar Festival | lvl60/min1 | npc15892:Lunar Festival Emissary@[[30.93,61.59]] — EVENT-OUT (event flag 7)
- 8883 | Valadar Starsong | lvl60/min1 | npc15895:Lunar Festival Harbinger@[[28.85,16.23]] — EVENT-OUT (event flag 7)
- 8898 | Dearest Colara, | lvl60/min1 | npc16009:Tormek Stoneriver@[[32.64,66.23]] — EVENT-OUT (event flag 8)
- 8981 | Gift Giving | lvl60/min1 | npc16075:Kwee Q. Peddlefeet@[[40.3,56.6]] — EVENT-OUT (event flag 110)
- 8993 | Gift Giving | lvl60/min1 | npc16075:Kwee Q. Peddlefeet@[[40.3,56.6]] — EVENT-OUT (event flag 110)
- 9094 | Argent Dawn Gloves | lvl60/min50 | npc16786:Argent Quartermaster@[[29.37,60.01],[29.59,61.42],[33.91,67.8]] — EVENT-OUT (event flag 99)
- 9154 | Light's Hope Chapel | lvl60/min50 | npc16241:Argent Recruiter@[[29.82,61.65],[34.07,68.14]] — EVENT-OUT (event flag 17)
- 9261 | Investigate the Scourge of Ironforge | lvl10/min1 | npc16484:Lieutenant Nevell@[[53,35]] — EVENT-OUT (event flag 17)
- 9317 | Consecrated Sharpening Stones | lvl60/min50 | npc16786:Argent Quartermaster@[[29.37,60.01],[29.59,61.42],[33.91,67.8]] — EVENT-OUT (event flag 99)
- 9318 | Blessed Wizard Oil | lvl60/min50 | npc16786:Argent Quartermaster@[[29.37,60.01],[29.59,61.42],[33.91,67.8]] — EVENT-OUT (event flag 99)
- 9319 | A Light in Dark Places | lvl60/min50 | npc16788:Festival Flamekeeper@[[63.54,24.67]] — EVENT-OUT (event flag 1)
- 9321 | Major Healing Potion | lvl60/min50 | npc16786:Argent Quartermaster@[[29.37,60.01],[29.59,61.42],[33.91,67.8]] — EVENT-OUT (event flag 99)
- 9322 | Wild Fires in Kalimdor | lvl60/min1 | npc16788:Festival Flamekeeper@[[63.54,24.67]] — EVENT-OUT (event flag 1)
- 9323 | Wild Fires in the Eastern Kingdoms | lvl60/min1 | npc16788:Festival Flamekeeper@[[63.54,24.67]] — EVENT-OUT (event flag 1)
- 9331 | Stealing Ironforge's Flame | lvl60/min50 | item23183:Flame of Ironforge <=1455:obj181333:Flame of Ironforge — HORDE-OUT
- 9337 | Major Mana Potion | lvl60/min50 | npc16786:Argent Quartermaster@[[29.37,60.01],[29.59,61.42],[33.91,67.8]] — EVENT-OUT (event flag 99)
- 9339 | A Thief's Reward | lvl60/min50 | npc16817:Festival Loremaster@[[63.81,25.31]] — EVENT-OUT (event flag 1)
- 9341 | Tabard of the Argent Dawn | lvl60/min50 | npc16786:Argent Quartermaster@[[29.37,60.01],[29.59,61.42],[33.91,67.8]] — EVENT-OUT (event flag 99)
- 9365 | A Thief's Reward | lvl60/min50 | npc16817:Festival Loremaster@[[63.81,25.31]] — EVENT-OUT (event flag 1)
- 9367 | The Festival of Fire | lvl60/min1 | npc16817:Festival Loremaster@[[63.81,25.31]] — EVENT-OUT (event flag 1)
- 9386 | A Light in Dark Places | lvl60/min50 | npc16788:Festival Flamekeeper@[[63.54,24.67]] — EVENT-OUT (event flag 1)
- 9388 | Flickering Flames in Kalimdor | lvl25/min1 | npc16817:Festival Loremaster@[[63.81,25.31]] — EVENT-OUT (event flag 1)
- 9389 | Flickering Flames in the Eastern Kingdoms | lvl25/min1 | npc16817:Festival Loremaster@[[63.81,25.31]] — EVENT-OUT (event flag 1)
- 60860 | Your Reward has Arrived! | lvlnull/minnull | npc5111:Innkeeper Firebrew@[[18.15,51.45]] — BROKEN-OUT: null level, no objectives — incomplete record
- 79482 | Stolen Winter Veil Treats | lvl60/min25 | npc216902:Wulmort Jinglepocket@[[32.4,67.4],[33,68.6],[33.4,65.4],[33.4,66.4],[33.4,67],[33.4,67.6],[33.6,66],[33.6,66.8],[33.6,67.8]] — SEASONAL-OUT: Stolen Winter Veil Treats (no event flag in data; seasonal by name + giver Wulmort Jinglepocket)
- 79492 | Metzen the Reindeer | lvl60/min25 | npc216902:Wulmort Jinglepocket@[[32.4,67.4],[33,68.6],[33.4,65.4],[33.4,66.4],[33.4,67],[33.4,67.6],[33.6,66],[33.6,66.8],[33.6,67.8]] — SEASONAL-OUT: Metzen the Reindeer (no event flag in data; seasonal by name + giver Wulmort Jinglepocket)
- 84147 | An Earnest Proposition | lvl60/min58 | npc230319:Deliana@[[43.56,52.65]] — DUP-OUT: data-duplicate of contracted 8905 (Druid Earnest Proposition, same spot, zone-1455 record canonical)
- 84148 | An Earnest Proposition | lvl60/min58 | npc230319:Deliana@[[43.56,52.65]] — DUP-OUT: redundant ungated duplicate — all classes covered by contracted 8905-8912 set
- 84149 | An Earnest Proposition | lvl60/min58 | npc230319:Deliana@[[43.56,52.65]] — DUP-OUT: redundant ungated duplicate — all classes covered by contracted 8905-8912 set
- 84150 | An Earnest Proposition | lvl60/min58 | npc230319:Deliana@[[43.56,52.65]] — DUP-OUT: data-duplicate of contracted 8908 (Paladin Earnest Proposition, same spot, zone-1455 record canonical)
- 84154 | An Earnest Proposition | lvl60/min58 | npc230319:Deliana@[[43.56,52.65]] — DUP-OUT: redundant ungated duplicate — all classes covered by contracted 8905-8912 set
- 95817 | Rotgath Stonebeard | lvl60/min1 | (zone-flagged 1455 only) — BROKEN-OUT: no start record at all
- 97447 | An Earnest Proposition | lvl60/min58 | (zone-flagged 1455 only) — BROKEN-OUT: no start record at all
- 98895 | Darkspear Islands Clash | lvl39/min30 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground mark turn-in
- 98896 | Darkspear Islands Clash | lvl39/min30 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground mark turn-in
- 98897 | Darkspear Islands Clash | lvl49/min40 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground mark turn-in
- 98898 | Darkspear Islands Clash | lvlnull/minnull | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground mark turn-in
- 98899 | Darkspear Islands Clash | lvl59/min50 | npc15351:Alliance Brigadier General@[[70.41,91.12]] — REPEATABLE-OUT: battleground mark turn-in

## BORDERLINE (argued, nothing decided silently)

1. 4485 vs 4486 (Tome of Nobility): both accept in the city (Tiza vs
Brandur), both Human+Dwarf Paladin, both end at Duthorian Rall in
Stormwind, and they exclude each other — a pure giver-choice pair.
Contracted 4485 (lower ID, deterministic rule); 4486 OUT with a swap note.
2. 3629 vs 3632 (engineering specializations): mutually exclusive.
Contracted 3632 Gnome — the pack-consistent pick (Stormwind contracted
Gnome 3630, Goblin 4181 out); 3629 OUT with a swap note.
3. 5283 vs 5284 (smithing specializations): mutually exclusive, no chain
differentiator (neither has pres nor nexts), both level 40 in the Military
Ward. Contracted 5283 Armorsmith (lower-ID deterministic rule); 5284 OUT
with a swap note.
4. 2201/2240/2279: accept NPC/object has no spawn data anywhere; the only
known location is inside Uldaman (dungeon). OUT as dungeon accepts; the
city chains keep going through contracted 2204/3375/2398/2439 with
structural pre-notes.
5. 2947: accept is the Sparklematic 5200 object with no spawn data; the
Sparklematic lives in Gnomeregan (dungeon). OUT; 2924 contracted with a
structural pre-note.
6. 4361/4363: accept NPCs (Kharan Mighthammer, Princess Moira
Bronzebeard) have no spawn data anywhere in the data, so the accept
cannot be placed in Ironforge. OUT; the Magni chain keeps 4341 and 4362
with a structural pre-note on 4362.
7. 97447/95817: quest records carry no start at all — broken. OUT.
8. 7494/7562/8415/8419/1798: also contracted in Stormwind, but each has a
genuine Ironforge accept (Hammerfall, Jubahl Corpseseeker, Brandur,
Briarthorn, Lago Blackwrench — all 1455-only spawns). IN here too; each
guide routes its own accept, and the ledger notes the overlap. (1798 was
already flagged as a dual accept in the Stormwind census.)
9. 8151/8233/8417: zone-flagged 1454 (Mulgore) but accept in the city
(Olmin, Hulfdan, Kelv). Accept decides — IN, with the flag noted; the
guide treats them as expedition/breadcrumb legs.
10. 1646/2198/637/708/968/98423: item-starts with no source anywhere in
the data. IN with a bag note and no collect line (Stormwind 1642/1649
precedent). 6681 is item-started by pickpocketing city rogues (Hulfdan,
Ormyr, Fenthwick all spawn here) — IN tagged. 97263 is object-started in
the city and ends in the city — IN. 79091 starts at the Library Book
object in the Hall of Explorers (@1455 [76,10.4]); its Uldaman and
Stormwind co-starters are uncontracted anywhere — IN as the city-starter
leg, noted.
11. 8565/8567/8569 (Past Victories/Efforts, min-level 1): one-time-looking
intros, but they feed the repeatable battleground mark turn-ins and live
on the same Brigadier General. OUT with the repeatable class.
12. 687 (pres 653 with no start record, 688 Horde-only), 735 (pre 727
Wetlands), 737 (pre 735 plus 736 Horde), 94818 (pre 94819
Stormwind-contracted, alternative 94820 Darnassus), 96016 (pre 79366
Thousand Needles, alternative 96135 contracted): all IN with the
uncontracted alternatives named as structural notes — multi-entry pres
read as alternatives, and no persona can satisfy a Horde or dungeon
pre.
13. 94817/94818: Mims dual-spawns Dun Morogh [55.05,22.38] and Ironforge
[24.59,10]; Dun Morogh does not contract them. The city rule contracts
the Ironforge accept — IN, gated Gnome Priest.
14. 467/1179: Pilot Longbeard spawns in the city [72.73,94.01]; Dun Morogh
does not contract these. IN, no overlap.
15. 4485 carries a stale 1453 zone flag but its giver Tiza spawns only on
1455 — giver map wins, IN as Ironforge's (Stormwind never contracted it).
16. 8254 (Priest-gated "Cenarion Aid", null races), 1880/1919
(Human+Gnome Mage), 96243 (Dwarf+Gnome Shaman): unusual eligibility
combos, but the data fields are explicit — IN gated exactly per the
data.
17. 301 (pre of 302), 1704 (pre of 1708), 2923 (pre of 2922), 7637 (pre of
7639), 6391 (pre of 6388), 95998 (pre of the Camping pair), 94819 (pre
of 94818), 1015 (excl of 1019): contracted in the Loch Modan, Stormwind,
Dun Morogh and Elwynn guides respectively — the Ironforge legs carry
"pre in X guide" notes, the pack's established cross-guide pattern.
18. 84147-84154: five "An Earnest Proposition" records from the duplicate
Deliana (230319) at the same spot as the canonical Deliana (16013).
84147/84150 duplicate contracted 8905/8908 class-for-class; 84148/84149/
84154 are redundant ungated records fully covered by the contracted
8905-8912 eight-class set. OUT as data duplicates.
19. 3461/3645: accepts sit at 1447 and STV respectively — home guides own
them; noted as chain-links, not contracted.
20. 8796/8797: the Stormwind and Darnassus accepts of the AQ event quest —
outside the city and event-flagged; OUT twice over.

## Companion question (no building)

City-vendor recipes: 46 unique recipe items sold by vendors spawning
inside Ironforge (50 vendor links). By inferred profession — Alchemy 3
(Free Action Potion, Elixir of Superior Defense, Lesser Arcane Elixir),
Cooking 8 (incl. Gingerbread Cookie and Egg Nog from seasonal vendor
Wulmort Jinglepocket), Enchanting 5 (Chest Minor Mana, 2H Lesser
Intellect, three oils), Engineering 5 (Gnomish Universal Remote, Thorium
Grenade, Thorium Widget, Blue Firework, Soul Vessel), Tailoring 8 (three
Mageweave shirts, Tuxedo set, Enchanted Mageweave Pouch, two reagent
bags), Leatherworking 14 (Heavy Leather Ball, four whelp-scale boots,
two armor kits, seven belts), Blacksmithing 1 (Plans: Mantle of the
Second War), unclassified 2 (Pattern: Phoenix Bindings, Argent Training
Manual — the latter from the event-gated commendation officer).
Ironforge vendors: Soolie Berryfizz, Tansy Puddlefizz, Tilli
Thistlefuzz, Gearcutter Cogspinner, Outfitter Eric, Bombus Finespindle,
Emrul Riknussun, Wulmort Jinglepocket (seasonal), Tamelyn Aldridge,
Ironforge Commendation Officer (event chain), Granny Finespindle,
Poranna Snowbrow, Ellie Stonebrow. Ironforge is smithing country in
flavor, but the vendor data holds only one Blacksmithing plan.

City rares: none confirmed. NPC records carry no rare flag; a subName
scan over all 270 NPCs spawning on 1455 shows trainers, vendors,
battlemasters, guards and quest NPCs only — no rare markers.

## Notable non-candidates (never in scope)

1155/3482 ([NYI] placeholders, no 1455 presence); 3111 (Glyphic Rune —
sourceless item, zone null, pre in Dun Morogh); 6661/6662 (Deeprun Tram
rat quests, zone null, no 1455 start); 1076/167 (the Debris/Badge pair —
Stormwind accepts at zone 1453, Stormwind-contracted, correctly out of
scope here); 1688/1716 (Gakin, Stormwind-contracted); 1793 (Duthorian,
Stormwind-contracted); 3000 (Grayson, Stormwind accept); 2997 (Azar, Dun
Morogh-contracted); 2998 (Wilhelm, Elwynn accept); 7638 (Duthorian,
Stormwind-contracted); 6391/2299 (Dun Morogh accepts, Dun Morogh
contracts 6391); 94819 (Stormwind-contracted).
