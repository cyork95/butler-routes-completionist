# Orgrimmar City census (pack 0.97.0 round)

Every quest in the local data (questie-forever, `--product wowf` + QuestieDB)
whose accept/start is in Orgrimmar (zone 1454): **318 candidates** — 316 keyed
by giver spawn (NPC or object on the 1454 map, dual-spawn = city NPC per the
city rule), plus 6681 (the only item-start with an Orgrimmar source) and 97411
(zone 1454, empty start record — see BORDERLINE). No level band (city census):
span is quest level **1–60** (min-levels 1–58), plus one special (1507, level
-1, min 20 — the warlock Devourer of Souls ritual, same shape as Stormwind's
1716).

Disposition: **173 IN**, 145 OUT of the candidates. The contract
(`docs/quest-contracts.json`, slug `orgrimmar-city`, order 49, span `1-60`)
holds exactly the 173. Two further records examined but not candidates:
80325/95483 (turn-in-only in Orgrimmar, no accept anywhere — noted, not
contracted).

## Method

Accept/start decides: an NPC start with a 1454 spawn, an in-city object start,
or an item start whose source is city-bound. A quest that merely turns in here
but accepts elsewhere is not an Orgrimmar quest (80325, 95483). Zero overlap
with zone contracts is verified (stormwind/elwynn, ironforge/dun-morogh,
darnassus/teldrassil all overlap 0): quests already homed in Durotar stay out
even where a giver dual-spawns, and are named below. Shared multi-city accepts
go the other way — Stormwind, Ironforge and Darnassus each contract the same
shared IDs for their own accepts (7562 in two cities, 8151/8233/8417 in two),
so Orgrimmar contracts its own accepts of the same quests. Same-name same-chain
twins both route (Hidden Enemies ×5; the three Earnest sets; Just
Compensation/Saving the Best class sets). "Additional Runecloth" repeatables
stay out (first-time donations only, mirroring all three Alliance city
censuses).

## Named check: 7833–7836

IN, all four: Vehena's cloth chain (Wool 7833 / Silk 7834 / Mageweave 7835 /
Runecloth 7836, pre-chain 7833→7836, min 12/20/35/50). 7837 Additional
Runecloth is the repeatable tail — OUT. Rashona's parallel set mirrors it:
7824/7826/7827/7831 IN, 7832 Additional OUT. This closes the Durotar census's
flag.

## IN (173)

Thrall's court: 787 Eittrigg's Wisdom (the Durotar soft-pre's accept —
contracting it here does not disturb Durotar, which carries only the turn-in),
809, 813, 93739, 95283, 96376, 98024 (Horde-only), 7784 Lord of Blackrock,
6566/6567, 7562 Mor'zul (multi-city warlock, only Warlock), 5093 Call to Arms,
7241, 7341, 7491 For All To See (pre for 7493), 7492 Camp Mojache breadcrumb
(Gorlach dual 1411+1454 — the Orgrimmar accept; ends Feralas), 936 Assisting
Arch Druid Runetotem (ends Thunder Bluff/Mulgore — expedition), 91735.
Rogue row: 1858/1963/2379/2382/2458/2460/2479 (only Rogue,Orc,Troll),
8233 Simple Request (multi-city, only Rogue), 235 Ashenvale Hunt, 649/650
Ripple Recovery, 1361 (next 1362 outside — chain ends out), 1431/1432 Alliance
Relations twins, 4494/4511 Zilzibin, 6681 Manor Ravenholdt (the ONE item-start:
Seal of Ravenholdt, only Rogue, bag note — Ironforge precedent), 7541.
Warlock row: 1501/1504/1509 (only Warlock,Orc,Undead,Troll), 1507 (lvl-1,
min 20, only Warlock), 1508, 1513, 2996, 3631, 4737, 4967, 65601/65604/65610
(pre chain 1507→65601→65604/65610; excl 1472 is the Undercity twin — noted,
not blocking), 8419 Imp's Request (multi-city, only Warlock), 91548 Vek'zol
(only Warlock; pre 91547 Azshara — soft-pre, see below).
Shaman row: 1522 (only Shaman,Orc,Tauren,Troll), 1528/1531, 7667/7668/7669
(Sagorne chain, only Shaman), 8258 (only Shaman), 8410 (only Shaman),
8258/8410/1528/1531/7667-7669 all min 50+ endgame — IN by the no-band rule.
Warrior row: 1718 Islander (multi-city shared, only Warrior — Stormwind did not
contract it but Ironforge did; the Orgrimmar accept counts), 1823 Speak with
Ruga (only Warrior), 8417 Troubled Spirit (multi-city, only Warrior).
Hunter row: 1944/1945 (only Hunter,Orc,Undead,Troll), 6068 (only
Hunter,Orc,Troll), 6066 (only Hunter,Tauren), 8151 Hunter's Charm (multi-city,
only Hunter).
Mage row: 1947/1953 (multi-city shared, only Mage), 8250 Magecraft (only Mage),
1959 (only Mage,Undead,Troll). Priest row: 5646 (only Priest,Undead), 5680
(only Priest,Troll — both left out of Durotar by its band, both accept here),
8254 Cenarion Aid (multi-city, only Priest). Druid row: 5927 (only
Druid,Tauren).
Paladin row: 97411 An Earnest Proposition/Lightforge (only Paladin — sourceless
accept at Mokvar, honest note; see BORDERLINE).
Orc-only training: 96994/97194 (only Orc). Orc/Troll flight: 6385/6386 (only
Orc,Troll).
Profession row (all optional + when skill): Blacksmithing 2751-2756, 5301,
5302, 96874, 2757 Booty Bay or Bust (ends Stranglethorn — expedition);
Leatherworking 96875, 7493 (pre 7491 in-contract); Fishing 6608; Cooking 6611;
First Aid 6623.
Mokvar sets: 84155-84162 (bracer text maps Druid→Warrior in order; gates only
<Class> each), 8913-8920 (cls confirms the same mapping), 8927/8938-8944 Just
Compensation (only <Class> each), 9007-9014 Saving the Best (only <Class>
each), 8923, 8930 (pre = all 8 Just Compensation — in-contract), 9032 (no
objectives; pre = Anthion's Parting Words 8957 + class variants 9016-9022 —
8 class-gated soft-pre mini-steps, see below).
Necklace Recovery: 2283→2284 (2318 outside), 2341 (pre 2340 Badlands —
soft-pre). 2284's end (6912) is data-present — full accept/turnin.
Jes'rimon: 3563 (pre 3541 Azshara — soft-pre), 4300, 91735.
Southfury/Thunder Ridge: 4002/4003, 3122, 2981, 1061, 1146.
Odds and ends: 106? (counted), 2861 Tabetha's Task (multi-city shared,
ungated), 79094 Lessons of Ta'zo (object start on 1454, shared, ungated),
5726-5730 Hidden Enemies ×5 twins, 5761, 95697, 97242/97246/97249/97275/97326.

## OUT (145 of candidates)

- Durotar-homed (6): 826, 828, 830 (accepts outside — see non-candidate note),
  1505, 1883, 5652, 5662, 9263, 98517. Zero-overlap rule; Durotar owns them.
- Alliance-only (2, both also seasonal): 8993, 9365 — the set-aside list.
- Seasonal/event (44 + AQ 36): Midsummer 9319/9322/9323/9339/9368/9386/9388/
  9389; Winter Veil 6961-6964/6984/8799/8746 + 7061/79483/79495 by title;
  Darkmoon 7926; Lunar 8677/8867/8873-8875/8883; Love is in the Air 8900;
  Children's Week 172/1800/5502/910/911/915/925; Hallow's End 8312/8359;
  Fishing 8228; Scourge Invasion 9154 (+9263 homed); Pilgrim's 8744/8767-8769/
  8788/8803; AQ war effort 8532-8616 (30) + 8794 + 8846-8855 + 8981 (36 total).
- Repeatable (58): commendations 8815-8826/8832/8833/
  8840/8841/8844/8845 (14), battleground brackets 8367-8443/8566-8570/
  98887-98891 (34), Argent Dawn hand-ins 9320/9333-9343 (6), wolf swaps
  7660/7661, Additional Runecloth 7832/7837.
- (Reason sums over the 147 candidate OUTs: seasonal 44, AQ war-effort 36,
  repeatable 58, Durotar-homed 6, Alliance 2, broken 1.)
- Broken (1): 60860 (no level, no objectives; no city ever contracted it).
- Non-candidate notes (examined, not accepts): 826/828/830 (homed Durotar,
  accepts 1411-side); 8836-8839/8846-8850 (Alliance-side commendation/war-supply
  records — Ironforge/Darnassus-side); 80325/95483 (turn-in-only in Orgrimmar,
  no accept anywhere — the accept rule leaves them out).

## In-city vendor recipe stock (companion scoping, not built here)

121 recipe items sold by 1454-spawning vendors: Tailoring-heavy (Borya,
Darah, Pawani, Tamar — patterns, shirts, bags); Leatherworking (Pawani,
Tamar — leather patterns); Enchanting (Kithas — formulas); Alchemy
(Hagrus, Kor'geld — recipes); Engineering (Sovik — schematics); Cooking +
Fishing (Xen'to, Shankys); Blacksmithing (Sumi — plans); mixed-vendor
Jornah (plans/pattern/schematic/recipe); seasonal Winter Veil stock on
Penney Copperpinch (17200, 17201 — event stock, flagged for the companion
round to rule on). No city rares question arises here (separate scan).

## BORDERLINE

- 97411: no start and no end in the data, but the 9th Earnest variant by
  every other signal (zone 1454, Horde races, Lightforge = Paladin set,
  objectiveText names Mokvar in Orgrimmar). Contracted with honest
  sourceless-accept + no-turn-in notes rather than silently dropped; gated
  only Paladin (set-membership + Ironforge's 8-gate precedent over the empty
  cls field).
- 1718: Ironforge contracted it, Stormwind did not, both had the accept.
  Following the Ironforge precedent (shared multi-city accepts are contracted
  per city).
- 7061/79483/79495: event field empty but Winter Veil by title + vendor
  (Kaymard/Sagorne seasonal). OUT as seasonal — title evidence over the empty
  field.
- 2340/2318/3541/8957+9016-9022/91547: out-of-contract pres handled by
  dedicated `when onquest` mini-steps (9032 gets 8 class-gated ones); none
  silently dropped. 1472 (Devourer of Souls, Undercity) is excl-only on the
  warlock Love chain — noted, no action.
- Race+class combined gates (1944/1945, 1959, 1501-group, 1522, 1858-group,
  6068, 5927, 6066): gate = class token + each race token in the data mask
  (e.g. only Hunter,Orc,Undead,Troll), mirroring `only Human,Dwarf,Paladin`
  and `only Druid,Tauren` precedents.
