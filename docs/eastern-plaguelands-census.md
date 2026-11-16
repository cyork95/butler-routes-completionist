# Eastern Plaguelands census (pack butler-routes-completionist)

Source: local Forever game data (questie-forever quests/npcs/objects.json),
built with `--product wowf` + QuestieDB. Accept-zone key **1422** (verified:
97 quest records key 1422; next keys 1421 Silverpine 78, 1423 WPL 235).
Alliance route. Game data wins throughout.

Method (settled): a quest belongs to the zone if its accept/start is on 1422.
Chains ending outside are IN; objectives in-zone with accept elsewhere are OUT.
Race masks: 4294967373 Alliance IN, 8589934770 Horde OUT (set aside), 16
Undead OUT (set aside), 5 Human+Dwarf IN (paladin line, gated), null neutral
IN. The giver-spawn test (city rule) was run on every giver: all accept-givers
spawn on 1422 (Tirion Fordring 1855 dual-spawns 1422+1423, so the Tirion chain
stays EPL by the accept-zone rule; Mennet Carkad 6467 dual-spawns 1422+1458
but his quests are Undead-only and OUT regardless).

## Band: 50-60

Lowest contracted minLevel 50 (bulk cluster: cauldron chain, watchtowers,
scourgestones, paladin line, Unfinished Business); three min-48 quests
(5903/5904/6389 A Plague Upon Thee) contracted below-band per the WPL
Front-letter precedent. Highest quest level 60 everywhere; min-57 finales
(chromatic 5164/5166/5167, Ras chain 5461/5462/5466) IN by the zone-finale
rule. Nothing is OUT on band (max minLevel in data is 57).

## IN - 76 quests

| ID | title | lv/min | giver (accept) | turn-in | notes |
|----|-------|--------|----------------|---------|-------|
| 211 | Alas, Andorhal | 60/50 | Ashlam Valorfist @1422 | Ashlam @1422 | pre 5097 IN |
| 4971 | A Matter of Time | 56/53 | Chromie @1422 | Chromie | chain 4971>4972>4973 |
| 4972 | Counting Out Time | 56/53 | Chromie | Chromie | twin name, chained, both routed |
| 4973 | Counting Out Time | 56/53 | Chromie | Chromie | twin name, chained, both routed |
| 4984 | The Wildlife Suffers Too | 54/51 | Mulgris @1422 | Mulgris | chain 4984>4985 |
| 4985 | The Wildlife Suffers Too | 56/51 | Mulgris | Mulgris | pre 4984 IN; feeds 4986 |
| 4986 | Glyphed Oaken Branch | 56/51 | Mulgris | Mathrengyl @1438/1457 | Alliance twin (4987 Horde OUT); Darnassus turn-in leg |
| 5021 | Better Late Than Never | 52/50 | Janice Felstone @1422 | Janice's Parcel object @1422 | neutral pre for faction twins |
| 5022 | Better Late Than Never | 52/50 | pre 5021 (IN) | Bathrilor @1453 | Alliance twin (5023 Horde OUT); Stormwind turn-in leg |
| 5051 | Two Halves Become One | 54/50 | Janice Felstone | Janice | pre 5050 Stormwind OUTSIDE - soft-pre |
| 5058 | Mrs. Dalson's Diary | 55/52 | diary object @1422 | diary object | item-start, placed |
| 5059 | Locked Away | 55/52 | Outhouse object @1422 | Outhouse | twin name, distinct ends, both routed |
| 5060 | Locked Away | 55/52 | Locked Cabinet object @1422 | Locked Cabinet | twin name, distinct ends, both routed |
| 5092 | Clear the Way | 52/50 | Ashlam @1422 | Ashlam | pres 5066/5090/5091 outside - soft-pre; feeds 5097+5215 |
| 5097 | All Along the Watchtowers | 56/50 | Ashlam | Ashlam | pre 5092 IN; feeds 211+5533 |
| 5142 | Little Pamela | 55/50 | Marlene @1422 | Pamela @1423 | WPL 5149's pre (excl 5601 noted) |
| 5153 | A Strange Historian | 56/50 | Marlene | Chromie @1422 | pre 5152 WPL-contracted - soft-pre |
| 5154 | The Annals of Darrowshire | 56/50 | Chromie | Chromie | pre 5153 IN; feeds 5210 |
| 5164 | Catalogue of the Wayward | 60/57 | catalogue object @1422 | catalogue object | finale, pre 5162 outside - soft-pre |
| 5166 | Breastplate of the Chromatic Flight | 60/57 | pre 5164 IN | Jeziba @1422 | finale |
| 5167 | Legplates of the Chromatic Defier | 60/57 | pre 5164 IN | Jeziba @1422 | finale |
| 5210 | Brother Carlin | 56/50 | Chromie | Carlin @1423 | pre 5154 IN; WPL turn-in leg |
| 5215 | The Scourge Cauldrons | 53/50 | Ashlam | MacDonnell @1422 | pre 5092 IN; feeds 5216 |
| 5216 | Target: Felstone Field | 53/50 | MacDonnell | cauldron object @1422 | pre 5215 IN |
| 5217 | Return to Chillwind Camp | 53/50 | pre 5216 IN | MacDonnell | - |
| 5218 | Felstone Field Cauldron | 53/50 | cauldron object @1422 | cauldron object | standalone, no pre |
| 5219 | Target: Dalson's Tears | 55/50 | MacDonnell | cauldron object @1422 | pre 5217 IN |
| 5220 | Return to Chillwind Camp | 55/50 | pre 5219 IN | MacDonnell | - |
| 5221 | Dalson's Tears Cauldron | 55/50 | cauldron object @1422 | cauldron object | standalone, no pre |
| 5222 | Target: Writhing Haunt | 55/50 | MacDonnell | cauldron object @1422 | pre 5220 IN |
| 5223 | Return to Chillwind Camp | 55/50 | pre 5222 IN | MacDonnell | - |
| 5224 | Writhing Haunt Cauldron | 55/50 | cauldron object @1422 | cauldron object | standalone, no pre |
| 5225 | Target: Gahrron's Withering | 58/50 | MacDonnell | cauldron object @1422 | pre 5223 IN |
| 5226 | Return to Chillwind Camp | 58/50 | pre 5225 IN | MacDonnell | feeds 5237 |
| 5227 | Gahrron's Withering Cauldron | 58/50 | cauldron object @1422 | cauldron object | standalone, no pre |
| 5237 | Mission Accomplished! | 58/50 | Ashlam | Ashlam | pre 5226 IN |
| 5343 | Barov Family Fortune | 60/52 | Weldon Barov @1422 | Weldon | feeds 5344 |
| 5344 | The Last Barov | 60/52 | pre 5343 IN | Weldon | - |
| 5382 | Doctor Theolen Krastinov | 60/55 | Eva Sarkhoff @1422 | Eva | feeds 5515 |
| 5384 | Kirtonos the Herald | 60/55 | Eva | Eva | pres 5383+5515 (5515 IN, 5383 outside) - soft-pre; feeds 5461 |
| 5401 | Argent Dawn Commission | 55/50 | Pureheart @1422 | Pureheart | one-time; excl 5405/5503 are the Tirisfal/WPL sister commissions |
| 5461 | The Human, Ras Frostwhisper | 60/57 | Marduke @1422 | Marduke | pre 5384 IN; feeds 5462 |
| 5462 | The Dying, Ras Frostwhisper | 60/57 | Marduke | Leonid @1423 | pre 5461 IN; WPL turn-in leg (feeds WPL 5463) |
| 5466 | The Lich, Ras Frostwhisper | 60/57 | Marduke | Marduke | pre 5465 WPL-contracted - soft-pre |
| 5505 | The Key to Scholomance | 60/55 | Arbington @1422 | Arbington | pre 5803 IN |
| 5507 | Mantles of the Dawn | 60/55 | Lightspark @1422 | Lightspark | excl 5504/5513 (WPL-contracted sisters) noted |
| 5515 | Krastinov's Bag of Horrors | 60/55 | Eva | Eva | pre 5382 IN; feeds 5384 |
| 5521 | Chromatic Mantle of the Dawn | 60/55 | Lightspark | Lightspark | excl 5517/5524 (WPL-contracted sisters) noted |
| 5533 | Scholomance | 55/55 | Ashlam | Arbington | pre 5097 IN; feeds 5537 |
| 5537 | Skeletal Fragments | 57/55 | Arbington | Arbington | pre 5533 IN; feeds 5538 |
| 5538 | Mold Rhymes With... | 57/55 | Arbington | Krinkle @1446 | pre 5537 IN; Tanaris turn-in leg |
| 5542 | Demon Dogs | 56/52 | Tirion @1422/1423 | Tirion | starter 1 of 3, all feed 5742 |
| 5543 | Blood Tinged Skies | 56/52 | Tirion | Tirion | starter 2 of 3 |
| 5544 | Carrion Grubbage | 56/52 | Tirion | Tirion | starter 3 of 3 |
| 5721 | The Battle of Darrowshire | 60/55 | Chromie | Pamela @1423 | pre 5941 outside - soft-pre; WPL 5942's pre |
| 5742 | Redemption | 56/52 | Tirion | Tirion | pre 5542 (also 5543/5544) IN; feeds 5781 |
| 5781 | Of Forgotten Memories | 57/52 | Tirion | Tirion | pre 5742 IN; feeds 5845 |
| 5803 | Araj's Scarab | 60/55 | Arbington | Arbington | pre 5801 outside - soft-pre; feeds 5505 |
| 5845 | Of Lost Honor | 58/52 | Tirion | Tirion | pre 5781 IN; feeds 5846 |
| 5846 | Of Love and Family | 58/52 | Tirion | Renfray @1422 | pre 5845 IN; feeds 5848 |
| 5848 | Of Love and Family | 60/52 | Renfray | Tirion | pre 5846 IN; feeds 5861 |
| 5861 | Find Myranda | 60/52 | Tirion | Myranda @1422 | pre 5848 IN; feeds 5862 |
| 5862 | Scarlet Subterfuge | 60/52 | Myranda | Taelan @1422 | pre 5861 IN; feeds 5944 |
| 5944 | In Dreams | 60/52 | Taelan | Lord Tirion @1422 | pre 5862 IN |
| 5903 | A Plague Upon Thee | 55/48 | Dumah @1422 | Dumah | below-band IN (Front-letter precedent); feeds 5904 |
| 5904 | A Plague Upon Thee | 55/48 | Dumah | Termite Barrel object @1422 | below-band IN; pre 5903 IN; feeds 6389 |
| 6389 | A Plague Upon Thee | 55/48 | pre 5904 IN | Dumah | below-band IN (6390 Horde twin OUT) |
| 6004 | Unfinished Business | 56/50 | Kirsta @1422 | Kirsta | chain 6004>6023>6025, all routed |
| 6023 | Unfinished Business | 57/50 | Kirsta | Kirsta | pre 6004 IN |
| 6025 | Unfinished Business | 58/50 | Kirsta | Kirsta | pre 6023 IN |
| 6185 | The Eastern Plagues | 60/56 | Shadowmore @1422 | Shadowmore | pre 6184 outside - soft-pre; feeds 6186 |
| 6186 | The Blightcaller Cometh | 60/56 | Shadowmore | Bolvar @1453 | pre 6185 IN; Stormwind turn-in leg (feeds 6187, Stormwind-contracted) |
| 8414 | Dispelling Evil | 52/50 | Thel'danis @1422 | Thel'danis | paladin Human/Dwarf (race 5 class 2); pre 8415 Stormwind OUTSIDE - soft-pre |
| 8416 | Inert Scourgestones | 52/50 | Thel'danis | Ashlam | paladin Human/Dwarf; pre 8414 IN |
| 8418 | Forging the Mightstone | 52/50 | Ashlam | Ashlam | paladin Human/Dwarf; pre 8416 IN |
| 92842 | A Cousin Abroad | 55/null | Pureheart @1422 | Wainworth @2482 | null minLevel, lv 55 in-band; Riverglades turn-in leg |

## OUT - 21 quests

Horde set-asides (15, for the Horde block's reconciliation): 1886, 1898,
1978 (The Deathstalkers I-III, Undead rogue, Mennet Carkad); 1998 Fenwick
Thatros + 1999 Tools of the Trade (Undead rogue follow-ups); 2378 Find the
Shattered Hand (Horde-mask rogue, excl 2380 noted); 4987 Glyphed Oaken Branch
(Horde twin of IN 4986); 5023 Better Late Than Never (Horde twin of IN 5022,
onward to 5049 Undercity); 5230/5232/5234/5236 Return to the Bulwark (Horde
twins of IN 5217/5220/5223/5226, onward chain 5229>5231>5233>5235 all Horde);
6390 A Plague Upon Thee (Horde twin of IN 6389); 6569 Oculus Illusions + 6570
Emberstrife (Horde-mask, Myranda giver, chain in from Horde 6568 Testament
of Rexxar).

Seasonal/event (2): 8714 Moonstrike the Elder, 8722 Meadowrun the Elder
(event=7 Lunar Festival, minLevel 1).

Broken (1): 7790 REUSE (null level/minLevel, Fallen Skyborne giver, next
pointer into missing 8152).

Repeatables (3): 5402 Minion's Scourgestones, 5403 Invader's
Scourgestones, 5404 Corruptor's Scourgestones - no pre, no next, same-NPC
stone turn-ins: the classic repeatable Argent rep turn-ins. One-time 5401
kept.

Accept-outside: none remaining - every other 1422-keyed record accepts on
1422 (giver-spawn test run on all givers; Tirion 1855 dual-spawns
1422+1423 and stays EPL by the accept-zone rule).

## BORDERLINE (all argued, none silent)

- Same-name twins, all routed together: 4972/4973 (chained, not exclusive),
  5059/5060 (distinct end-objects), 6004/6023/6025 (I/II/III chain),
  5021+5022 (neutral pre + Alliance follow-up; 5023 is the Horde fork, OUT),
  5903>5904>6389 (chain; 6390 is the Horde fork, OUT). Data shows no excl
  links between any routed pair.
- Repeatable call (5402/5403/5404): no chain links in either direction plus
  the classic repeatable-turn-in shape (stone counts into one NPC). Pack rule
  excludes repeatables; the one-time commission 5401 stays.
- 92842 null minLevel: contracted on accept-in-zone + neutral + level 55
  (inside the band). The null is a data gap, not an above-band signal.
- 8414/8416/8418 dual restriction (race 5 + class 2): gated only Paladin
  per line with a note naming the Human/Dwarf race lock (no Skyborne
  paladin can hold them per the mask).
- 5903/5904/6389 below band (min 48): IN per the WPL Front-letter
  precedent - completionism over tidiness; they chain into the band.
- Finales at min 57 (5164/5166/5167, 5461/5462/5466): IN by the zone-finale
  rule (minLevel in band); no minLevel sits above 57, so nothing is OUT on
  band.
- Cross-contract turns (not double-contracted - verified zero overlap with
  all 38 contracts): 4986 Darnassus, 5022 Stormwind, 5210/5462/5142/5721
  WPL, 5538 Tanaris, 6186 Stormwind, 92842 Riverglades. Each rides an
  expedition turn-in leg in the guide.
- 5466's pre 5465 is WPL-contracted; 5153's pre 5152 is WPL-contracted:
  both get Darkshore-technique soft-pre minis, never inline.
- Tirion triple start (5542/5543/5544 all feed 5742): all three routed;
  efficiency shapes order, never selection.
