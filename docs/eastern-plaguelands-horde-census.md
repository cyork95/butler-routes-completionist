# Eastern Plaguelands (Horde) census (pack butler-routes-completionist)

Source: local Forever game data (questie-forever quests/npcs/items/objects.json),
built with `--product wowf` + QuestieDB. Accept-zone key **1422** (verified:
97 quest records key 1422 — matches the Alliance census's 97 exactly).
Horde route. Game data wins throughout.

Method (settled): a quest belongs to the guide if it accepts/starts on 1422
and is available to Horde players. Chains ending outside are IN; objectives
in-zone with accept elsewhere are OUT. Race masks: 8589934770 Horde IN,
4294967373 Alliance OUT (set aside for the record), 16 Undead OUT (homed —
see below), 5 Human+Dwarf paladin OUT. Null-mask records are shared, not
Horde (Duskwood ruling) — they stay in the main guide, never duplicated.

## Band: 50-60

Contracted minLevels: 50 x5 (5023, 5230, 5232, 5234, 5236), 51 (4987),
55 x2 (6569, 6570), 48 (6390). Highest quest level 60 throughout. Band 50-60
mirrors the Alliance side; 6390 (min48) rides the same below-band precedent
the Alliance census applied to its own 5903/5904 (WPL Front-letter rule:
completionism over tidiness, chain runs up into the band).

## IN - 9 quests

| ID | title | lv/min | accept | turn-in | notes |
|----|-------|--------|--------|---------|-------|
| 4987 | Glyphed Oaken Branch | 56/51 | Mulgris Deepriver @1422 [53.73,64.66] | Nara Wildmane, Thunder Bluff [75.65,31.61] | Horde twin of contracted 4986; pre 4985 shared-contracted (soft-pre); starter item 12663 sourceless in data (R2 bag note: rides 4985's line) |
| 5023 | Better Late Than Never | 52/50 | Janice's Parcel object @1422 [38.73,55.24] | Royal Overseer Bauhaus, Undercity [69.79,43.16] | Horde twin of contracted 5022; pre 5021 shared-contracted (soft-pre); parcel placed in-zone; next 5049 accepts in Undercity, UNCONTRACTED (chain note, no duplication) |
| 5230 | Return to the Bulwark | 53/50 | Scourge Cauldron (Felstone) @1422 [37.25,56.78] | Vandis, Bulwark @1422 [26.4,59.1] | pre 5229 accepts Tirisfal (1420, UNCONTRACTED) — soft-pre mini + pickup note |
| 5232 | Return to the Bulwark | 55/50 | Scourge Cauldron (Dalson's) @1422 [46.18,51.9] | Vandis, Bulwark | pre 5231 Tirisfal UNCONTRACTED — soft-pre mini |
| 5234 | Return to the Bulwark | 55/50 | Scourge Cauldron (Writhing) @1422 [53.02,65.61] | Vandis, Bulwark | pre 5233 Tirisfal UNCONTRACTED — soft-pre mini |
| 5236 | Return to the Bulwark | 58/50 | Scourge Cauldron (Gahrron's) @1422 [62.54,58.47] | Vandis, Bulwark | pre 5235 Tirisfal UNCONTRACTED — soft-pre mini; next 5237 is Alliance-only (Horde fork ends at 5236, noted) |
| 6390 | A Plague Upon Thee | 55/48 | Termite Barrel @1422 [48.34,31.99] | Mickey Levine, Bulwark @1422 [26.7,59.6] | Horde twin of contracted 6389 (chain 5903>5904>6389 Alliance fork); pre 5902 accepts Tirisfal (UNCONTRACTED, pre 5901 also Tirisfal UNCONTRACTED) — soft-pre mini + pickup note |
| 6569 | Oculus Illusions | 60/55 | Myranda the Hag @1422 [50.79,77.85] | Myranda | pre 6568 accepts Stonetalon (1442, UNCONTRACTED, ruled above-band there) — soft-pre mini; objective 20x Black Dragonspawn Eye (16786), all 16 droppers sourceless in data (unplaced complete + family note) |
| 6570 | Emberstrife | 60/55 | Myranda the Hag | Emberstrife, Dustwallow [56.66,87.72] | pre 6569 IN; starter item 16787 sourceless (R2 bag note); next 6582 accepts Dustwallow (UNCONTRACTED) — chain note |

## OUT

Rogue block homed in undercity-city (6, NOT duplicated): 1886, 1898, 1978
(The Deathstalkers I-III, Undead rogue, Mennet Carkad), 1998 Fenwick Thatros
+ 1999 Tools of the Trade (Undead rogue follow-ups), 2378 Find the Shattered
Hand (Horde rogue). Rationale: Mennet Carkad spawns dual 1422 [8,67.4] +
1458 [83.51,69.11]; by the dual-spawn city-NPC rule (Durotar 1411+1454 and
Mulgore 1412+1456 precedents) he is a city NPC and his quests homed to the
Undercity contract (order 51), which already routes them. The Alliance EPL
census noted the dual spawn but left the home open (quests were OUT for the
Alliance route either way); the Undercity census closed it. Quest zone
fields read 1422, but the giver-based city rule governs dual spawns — the
same rule that moved 1412-zone quests into Thunder Bluff. No double-contract:
verified zero overlap (all 9 IN above are UNCONTRACTED everywhere).

Horde set-aside reconciliation (15 banked): the 6 rogue-block records land
as above (homed, not contracted here); the other 9 (4987, 5023, 5230, 5232,
5234, 5236, 6390, 6569, 6570) are ALL IN. Nothing banked is left unaccounted.

Seasonal/event (2): 8714 Moonstrike the Elder, 8722 Meadowrun the Elder
(event=7 Lunar Festival). Broken (1): 7790 REUSE (null level, Fallen
Skyborne giver, next-pointer into missing 8152). Repeatables (3): 5402/5403/
5404 Minion's/Invader's/Corruptor's Scourgestones (no chain links, classic
repeatable turn-in shape; one-time 5401 stays in main).

Alliance-only / shared (76): every record the main contract routes (55
Alliance-mask + 21 shared/null incl. 92842). Stay in the main guide, which
this round ungates — never duplicated. Cross-check: 5237 Mission
Accomplished! is Alliance-only (5236's next); the Horde cauldron fork ends
at 5236's turn-in.

Accept-outside chain links (noted, not contracted): 5229/5231/5233/5235 +
5228 (pre 5096, all Tirisfal 1420 Horde, UNCONTRACTED); 5901/5902 (Tirisfal
Horde, UNCONTRACTED); 6568 (Stonetalon 1442 Horde, UNCONTRACTED above-band);
5049 (Undercity 1458 Horde, UNCONTRACTED); 6582 (Dustwallow 1445 Horde,
UNCONTRACTED). All handled in-guide via soft-pre minis (in-zone accepts)
and chain notes (out-of-zone follow-ups).

Item-start scan (explicit, over all 15 set-asides + pool): start items found
on 1898 (7231, dropper Astor Hadren 6497 Silverpine — rogue block, homed),
1978 (7294, object Andron's Bookshelf 103600 Undercity — homed), 1998
(objective 7306, dropper Fenwick Thatros 6570 Silverpine — homed), 1999
(objective 7309, object Ambermill Strongbox 103815 Silverpine; required
5060 Thieves' Tools, object 103774 sourceless — homed), 5023 (12724 parcel
object placed in-zone — IN, routed), 4987 (12663 sourceless — IN, R2 bag
note), 5230/5232/5234/5236 (13190-13193 filled bottles, sourceless — IN,
R2 bag notes; the cauldron tap objects ARE placed), 6390 (15044 barrel
sourceless, tap object 177491 placed — IN, routed), 6569 (objective 16786,
all droppers sourceless — IN, unplaced complete + note), 6570 (16787
sourceless — IN, R2 bag note). No other pool record carries a start item.
The scan is complete; nothing asserted without it (Mulgore lesson).

## BORDERLINE (all argued, none silent)

- Rogue block home (1886/1898/1978/1998/1999/2378): EPL-contract vs
  Undercity-contract. Decided: Undercity stands (dual-spawn city-NPC rule,
  Mulgore/Thunder Bluff precedent). The quest zone field (1422) does not
  override the giver rule for dual spawns — the same logic that homed
  1412-zone quests to Thunder Bluff. Mennet's EPL spawn [8,67.4] is recorded
  as-read (far-west point, odd but data); no guide action rides on it from
  this round.
- 2378's excl 2380: mutual, but 2380 is Horde-mask (Durotar accept,
  UNCONTRACTED) — the excl is an alternate-start fork, not a faction twin.
  2378 routes here (EPL accept); 2380 stays uncontracted (Durotar census's
  call, not revisited). A pack-following player never holds 2380, so the
  excl never fires on this route. Undercity guide owns 2378's routing.
- Same-name twins: 5230/5232/5234/5236 are four distinct chain links (Return
  to the Bulwark I-IV, alternating with Tirisfal Target links) — all route,
  no exclusivity in the data.
- Faction twins 4987/4986, 5023/5022, 6390/6389: standard faction-twin
  shape (Felwood 86611/86612 precedent) — each side routes its own; no excl
  links; verified no cross-contract overlap.
- 6569/6570 with uncontracted pre 6568: Desolace 93045 shape — an
  uncontracted pre does not sink an in-zone accept; soft-pre mini + note.
- 5236>5237 (Alliance-only next): Horde fork ends at 5236's turn-in; the
  guide says so rather than routing a quest the player cannot take.
- Below-band: only 6390 (min48), mirroring the Alliance census's own three
  min-48 inclusions; band stays 50-60.
- 2379/5049/6582 follow-ups: out-of-zone accepts, all UNCONTRACTED — chain
  notes only, never contracted, never duplicated.
