# Burning Steppes census (pack butler-routes-completionist)

Census from local Forever game data (questie-forever quests/npcs/objects/items.json),
built with `--product wowf` + QuestieDB. Accept-zone key **1428** (verified:
52 quest records key 1428; next keys 1427 Searing Gorge 66, 1429 Elwynn 129).

Method (settled): a quest belongs to the zone if its accept/start is on 1428.
Chains ending outside are IN; objectives in-zone with accept elsewhere are OUT.
Item-started quests (including rare-drop starts) are IN. The giver-spawn test
was run on every giver; dual-spawn givers follow the Tirion precedent (EPL
census): a giver spawning on the key keeps the quest here (Corporal Keeshan
349 dual-spawns 1428+1433, so Missing in Action stays BS by the accept-zone
rule; Yuka Screwspigot, Kibler, Lothos Riftwaker and Bodley dual/triple-spawn
onto 1428, so their quests are candidates here).

Race masks: 4294967373 Alliance IN, 8589934770 Horde OUT (set aside),
null neutral IN (EPL precedent). Class 256 = Warlock, gated only Warlock.
No profession-skill quests in the data. Event 7 = Lunar Festival (seasonal OUT).

## Band: 48-60

Lowest contracted minLevel 48 (bulk cluster: Dark Iron Legacy, Firegut chain,
Dragonkin/Windsor chain, Pyron/Incendius). Highest quest level 60 everywhere.
MinLevel-60 quests (Dreadsteed chain 7563-7631, Egg/Doomrigger/Maxwell/Drakkisath
finales, Bodley chain, attunements) are IN: 60 is the band top, not above it
(the EPL census likewise kept max-minLevel records at its top edge).
Quest 219 (Missing In Action, minLevel 19) is contracted below-band as a noted
escort outlier: its accept (Keeshan at 65.6,88.4 on 1428) is in-zone, no OUT
rule fires, so the completionist rule keeps it; the header band describes the
bulk. Nothing is OUT on band.

## IN - 59 quests

| ID | title | lv/min | giver (accept) | turn-in | notes |
|----|-------|--------|----------------|---------|-------|
| 219 | Missing In Action | 25/19 | Keeshan @65.6,88.4 | Marris (Redridge) | below-band escort outlier; event escort to Redridge 28.27,48.7 |
| 3801 | Dark Iron Legacy | 52/48 | Franclorn @28.96,28.93 | Franclorn | no objectives; opener |
| 3802 | Dark Iron Legacy | 52/48 | Franclorn @28.96,28.93 | Monument of Franclorn (no spawn in data) | pre 3801; Ironfel from 9056; monument note-only complete |
| 3823 | Extinguish the Firegut | 52/48 | Oralius @84.56,68.68 | Oralius | Firegut ogres |
| 3824 | Gor'tesh the Brute Lord | 53/48 | Oralius | Oralius | pre 3823 |
| 3825 | Ogre Head On A Stick = Party | 53/48 | Oralius | Oralius | pre 3824; object plant |
| 4022 | A Taste of Flame | 54/52 | Cyrus @95.09,31.56 | Cyrus | main twin (molt + Cyrus); pre for 4024 |
| 4024 | A Taste of Flame | 58/52 | Cyrus | Cyrus | pre 4022/4023 (either); BRD Bael'Gar entrance complete + note |
| 4123 | The Heart of the Mountain | 55/50 | Maxwort @65.15,23.91 | Maxwort | |
| 4182 | Dragonkin Menace | 54/48 | Helendis @85.82,68.95 | Helendis | black dragonkin |
| 4183 | The True Masters | 54/48 | Helendis | Solomon (Redridge) | pre 4182; chain ends outside |
| 4224 | The True Masters | 54/48 | Maxwell @84.74,69.02 | Maxwell | pre 4223 (Redridge, uncontracted); structural note |
| 4241 | Marshal Windsor | 54/48 | Maxwell | Windsor (in-instance, no spawn) | pre 4224; interior-leg note |
| 4242 | Abandoned Hope | 54/48 | Windsor (in-instance) | Maxwell | pre 4241; interior-leg note |
| 4262 | Overmaster Pyron | 52/48 | Jalinda @85.41,70.06 | Jalinda | |
| 4263 | Incendius! | 56/48 | Jalinda | Jalinda | pre 4262 |
| 4283 | FIFTY! YEP! | 56/50 | Oralius | Oralius | 50 medallions |
| 4286 | The Good Stuff | 56/50 | Oralius | Oralius | 20 fanny packs |
| 4296 | Tablet of the Seven | 50/50 | Maxwort | Maxwort | |
| 4322 | Jail Break! | 58/50 | Windsor (in-instance) | Maxwell | pre 4282 (zone 242 instance quest, uncontracted); scripted event + interior-leg note |
| 4701 | Put Her Down | 59/55 | Helendis | Helendis | Halycon (LBRS) entrance complete + note |
| 4726 | Broodling Essence | 52/50 | Tinkee @65.24,24 | Tinkee | |
| 4734 | Egg Freezing | 60/57 | Tinkee | Tinkee | pre 4907 (Winterspring, uncontracted); Rookery egg spawnless - bare complete + note |
| 4735 | Egg Collection | 60/57 | Tinkee | Tinkee | pre 4734; same spawnless egg |
| 4764 | Doomrigger's Clasp | 60/57 | Mayara @84.84,69.12 | Mayara | pre 4766 (Stormwind-contracted); reference |
| 4765 | Delivery to Ridgewell | 60/57 | Mayara | Ridgewell (Stormwind) | pre 4764; chain ends outside |
| 4808 | Felnok Steelspring | 54/50 | Tinkee | Felnok (Winterspring) | pre 4726; chain ends outside |
| 4866 | Mother's Milk | 60/55 | Ragged John @65.01,23.76 | Ragged John | |
| 5002 | Message to Maxwell | 59/55 | Bijou (in-instance LBRS, no spawn) | Maxwell | pre 5001 (zone 253, uncontracted); interior-leg note |
| 5081 | Maxwell's Mission | 60/55 | Maxwell | Maxwell | pre 5002; Voone/Omokk/Wyrmthalak (instance) - entrance completes + note |
| 5089 | General Drakkisath's Command | 60/55 | item 12780 (Wyrmthalak 100%, no spawn) | Maxwell | item-start, in-instance source; R2 sourceless note |
| 5102 | General Drakkisath's Demise | 60/55 | Maxwell | Maxwell | pre 5089; Drakkisath (UBRS, no spawn) entrance complete + note |
| 5522 | Leonid Barthalomew | 60/57 | Tinkee | Leonid (EPL WPL-side 71.89,48.29) | pre 4735; chain ends outside |
| 6402 | Stormwind Rendezvous | 60/50 | Maxwell | Reginald Windsor (Stormwind) | pre 4322; chain ends outside |
| 4136 | Ribbly Screwspigot | 53/48 | Yuka @66.06,21.95 (dual 1418) | Yuka | Badlands above-band deferral; accepts on 1428 |
| 4729 | Kibler's Exotic Pets | 59/55 | Kibler @65.89,21.92 (dual 1418) | Kibler | Badlands above-band deferral; accepts on 1428 |
| 4862 | En-Ay-Es-Tee-Why | 59/55 | Kibler | Kibler | Badlands above-band deferral; accepts on 1428 |
| 7487 | Attunement to the Core | 60/55 | Lothos @26.4,24.5 (dual 1427) | Lothos | SG above-band deferral; Horde-side twin, neutral races |
| 7848 | Attunement to the Core | 60/55 | Lothos | Lothos | SG above-band deferral; Alliance-side twin, neutral races |
| 7761 | Blackhand's Command | 60/55 | item 18987 (Quartermaster 34.9,27.9 on 1428) | — | item-start, 1428-placed source; SG above-band deferral |
| 8961 | Three Kings of Flame | 60/58 | Bodley @32.2,25.8 (triple 1415/1427/1428) | Bodley | SG endgame deferral; pres 8960 (Ironforge-contracted) + 9032 (Horde, uncontracted) |
| 8962 | Components of Importance | 60/58 | Bodley | Bodley | lowest-ID variant path (see BORDERLINE 4) |
| 8966 | The Left Piece of Lord Valthalak's Amulet | 60/58 | Bodley | Bodley | path: 8962-leg (Mor Grayhoof, no spawn - note) |
| 8970 | I See Alcaz Island In Your Future... | 60/58 | Bodley | Bodley | pre any 8966-69; 20 Bloodkelp |
| 8985 | More Components of Importance | 60/58 | Bodley | Bodley | path: Starbreeze leg |
| 8990 | The Right Piece of Lord Valthalak's Amulet | 60/58 | Bodley | Bodley | path: pre 8985 (Isalien, no spawn - note) |
| 8994 | Final Preparations | 60/58 | Bodley | Bodley | pre any 8989-92; bracers + flask |
| 8995 | Mea Culpa, Lord Valthalak | 60/58 | Bodley | Spirit (no spawn) | Valthalak kill (UBRS, no spawn) + spirit turn-in; interior-leg notes |
| 8996 | Return to Bodley | 60/58 | Spirit (no spawn) | Bodley | pre 8995; Brazier; interior-leg accept note |
| 8997 | Back to the Beginning | 60/58 | Bodley | Deliana (Ironforge) | pre 8996; Alliance finale; chain ends outside |
| 7563 | Rage of Blood | 58/60 | Mor'zul @12.69,31.64 | Mor'zul | only Warlock; pre 7562 (Ironforge-contracted); 30 bloods |
| 7564 | Wildeyes | 58/60 | Mor'zul | Gorzeeki @12.44,31.63 | only Warlock; pre 7563 |
| 7623 | Lord Banehollow | 58/60 | Gorzeeki | Banehollow (Darkshore/Felwood) | only Warlock; pre 7564; chain ends outside |
| 7626 | Bell of Dethmoora | 60/60 | Mor'zul | Gorzeeki | only Warlock; pre 7564; 10 elixirs |
| 7627 | Wheel of the Black March | 60/60 | Mor'zul | Gorzeeki | only Warlock; pre 7564; shards + ore |
| 7628 | Doomsday Candle | 60/60 | Mor'zul | Gorzeeki | only Warlock; pre 7564; 35 dragonscale |
| 7629 | Imp Delivery | 60/60 | Gorzeeki | Gorzeeki | only Warlock; pre 7625 (Darkshore, uncontracted) + 7630; J'eevee spawnless (Scholomance lab) - bare complete + note |
| 7630 | Arcanite | 60/60 | Gorzeeki | Gorzeeki | only Warlock; pre 7626+7627+7628; 3 bars |
| 7631 | Dreadsteed of Xoroth | 60/60 | Mor'zul | Dreadsteed Spirit (no spawn) | only Warlock; pre 7629; dreadsteed kill spawnless - bare complete + note |

## OUT

Horde set-asides (3, for the Horde block's reconciliation): 4121 Precarious
Predicament (58/52, Grark Lorkrub, pre 4122); 3822 Krom'Grul (53/48, Sha'ni
Proudtusk - NOTE: Sha'ni spawns ONLY on 1428 at 79.95,45.4 while the record is
keyed 1418; Horde-only so OUT here either way; Horde block should rule its home);
8998 Back to the Beginning (60/58, Bodley Horde finale to Mokvar).

Exclusive variant (1): 4023 A Taste of Flame - the twin of contracted 4022
(see BORDERLINE 2).

Repeatables (5, `repeatable=true` in the data): 4463 Libram of Rumination,
4481 Libram of Constitution, 4482 Libram of Tenacity, 4483 Libram of
Resilience, 4484 Libram of Voracity.

Seasonal (2, `event=7` Lunar Festival): 8636 Rumblerock the Elder, 8683
Dawnstrider the Elder.

Above-band: none (max minLevel in the data is 60 = band top).

Broken/incomplete: none (every record has a placed or noted accept; ends all
present in data).

Accept-outside: none remaining - the outsider scan found 30 non-1428-keyed
quests with a 1428-spawning starter; of those, 7761 + the Badlands trio +
attunement twins + the Bodley path are contracted above (all accept on 1428
and sit in-band); 84396 Magma or Lava? stays Stormwind-contracted (noted link,
never double-contracted); 81953 Stonewrought Design stays OUT (Undercity-keyed,
minLevel 1, Undercity block's call); non-contracted Bodley variants stay OUT
(variant set-asides below); 4122 Grark Lorkrub stays OUT (Badlands-listed, pre
of OUT 4121, no BS role).

Non-contracted Bodley variants (11, set aside with reason): 8963, 8964, 8965
(Components), 8967, 8968, 8969 (Left Piece), 8986, 8987, 8988 (More
Components), 8991, 8992 (Right Piece) - see BORDERLINE 4.

Outside pre-quests (not contracted; guide references or soft-pres them):
4223 (Redridge, uncontracted), 4282 (zone 242 instance quest, uncontracted),
4907 (Winterspring, uncontracted), 5001 (zone 253, uncontracted), 7625
(Darkshore, uncontracted), 8960 (Ironforge-contracted, referenced), 9032
(Horde Bodley pre, uncontracted), 4122 (Badlands-listed, pre of OUT 4121),
4766 (Stormwind-contracted, referenced), 7562 (Ironforge-contracted, referenced).

## BORDERLINE

1. **219 Missing In Action (25/19).** The only sub-band record (minLevel 19 vs
   bulk floor 48). IN: Keeshan spawns on 1428 at 65.6,88.4 and the zone field
   is 1428, so the accept-zone rule fires exactly as it did for Tirion (EPL
   dual-spawn precedent); Alliance-available; escort event with placed
   Redridge endpoint. No OUT rule fires (not above-band, repeatable, seasonal,
   broken, or accept-outside). Contracted below-band as a noted outlier (the
   EPL census did the same for its min-48s per the WPL Front-letter precedent);
   the header band 48-60 describes the bulk.
2. **4022 vs 4023 (exclusive same-name twins).** Both feed 4024 (next=4024 on
   both; pre=[4022,4023] reads as either, since AND-semantics would make 4024
   uncompletable). The twin-routed precedent (Harvesting the Harvesters) had no
   exclusivity; here excl runs both ways, so one character completes one.
   Contract 4022 (obj=2: show the Kalaran Windblade molt AND defeat Cyrus,
   the fuller main flow) + 4024; set aside 4023 (obj=1, "unworthy" variant
   text) with reason. If play data ever shows both completable, 4023 is the
   first record back.
3. **In-instance accepts/turn-ins (4241T, 4242A, 4322A, 5002A) and spawnless
   turn-in targets (3802 monument, 7631 spirit).** All IN: the quests accept
   (by zone field + chain position) in BS; their interior legs ride at
   data-placed Blackrock anchors (Meeting Stones 179584/179585, Orb of Command
   179879, all on 1428) with honest notes naming the interior NPCs - the
   Scholomance-door precedent extended to accepts. Never an invented NPC or
   location.
4. **Bodley variant paths.** Four mutually exclusive legs (Components 8962-65,
   Left Piece 8966-69, More Components 8985-88, Right Piece 8989-92) converge
   through 8970 and 8994 (whose multi-ID pres read as either/or, since AND
   would be uncompletable). All four Left-Piece bosses and Valthalak lack
   outdoor spawns, so no location tie-break exists. Contract the lowest-ID
   consistently-linked path - 8962 > 8966 > 8970 > 8985 > 8990 > 8994 (each pre
   satisfied by the contracted predecessor, verified) - plus the shared spine
   8961 > ... > 8995 > 8996 > 8997. Mechanical tie-break, chain-verified, argued
   openly; the other 11 variants are set aside above, first back if data ever
   shows multi-path completion.
5. **7761 Blackhand's Command.** SG ruled it OUT as above-band (band 40-52);
   BS band 48-60 fits (minLevel 55), the item-start (18987, 100% from
   Scarshield Quartermaster, 1428 point at 34.9,27.9) is data-placed, so IN by
   the item-start rule. No conflict: it is uncontracted everywhere.
6. **8997/8998 finale pair.** Alliance 8997 IN (chain ends at Deliana,
   Ironforge); Horde 8998 set aside. Same split as the SG census ruled.
