# Feralas census (pack 0.41.0)

Accept-zone key **1444**. 107 quest records carry `zone: 1444` in the local
Forever data (questie-forever `quests.json`, built with `--product wowf` +
QuestieDB). Every start NPC verified to spawn on map 1444; every start
object verified on 1444. Faction decode used throughout: `races: 4294967373`
low bits = 77 = Alliance mask (1+4+8+64); `races: 8589934770` low bits = 178
= Horde mask (2+16+128+32); `races: null` = neutral/both.

## Band: 38–50

minLevel histogram (non-Horde candidates): min24: 2, min25: 1, min30: 7
(profession chain), min38: 4, min39: 2, min40: 22, min42: 3, min44: 2,
min45: 4, min46: 1, min47: 5, min54: 3, min60: 3, min1: 6 (4 writs + 2
seasonal), min null: 1 (broken). The open-world floor is min38 (the Kindal
Moonweaver chain: 2969/2970/2972/3841, all accepting in-zone); the top is
min47 (Morrowgrain, Videre Elixir, Haze of Evil). Finale quest levels run to
55 (3792, 7725/7726) but their minLevels (47/45) are in band, so they are IN
per the minLevel rule. Above-band OUT: min54+ (7441, 7482, 7488, the
Thunderfury chain 7785–7787).

## IN ledger (57)

OOX chain (neutral, item-start + escort):
- Q2766 L45 Find OOX-22/FE! — item8705 (OOX-22/FE Distress Beacon; 82
  droppers across 1444/1441, incl. Feralas Gordunni ogres, Woodpaw gnolls,
  Feral Scar yetis — see guide for the named sourcing area). Ends at the
  Homing Robot in Feralas. No pre.
- Q2767 L45 Rescue OOX-22/FE! — Homing Robot OOX-22/FE (1444); escort along
  the Forgotten Coast (objective at 45.63, ~coast in the data). Ends at
  Oglethorpe Obnoticus in Booty Bay (1434): chain ending outside, IN.

Yeti-hide line (Pratt McGrubben, Feathermoon-area buyer):
- Q2821 L46 The Mark of Quality — collect 10 Thick Yeti Hide. Next: 7733.
- Q7733 L48 Improved Quality — pre 2821; collect 10 Rage Scar Yeti Hide.
- Q7735 L48 Pristine Yeti Hide — item-start (item18969; droppers all on
  1444: Rage Scar Yeti, Elder Rage Scar, Ferocious Rage Scar, Lurking Feral
  Scar). Ends at Pratt. No pre.

Shay line:
- Q2844 L49 The Giant Guardian — Rockbiter; no objectives. Next: 2845.
- Q2845 L49 Wandering Shay — Shay Leafrunner; escort Shay (item9189 Shay's
  Bell + escort event in the data).

Wild Leather profession chain (Pratt McGrubben; skill=165 Leatherworking;
all `optional` + `when skill Leatherworking` gated in the guide):
- Q2847 L45 Wild Leather Armor (pre none) — 10 Thick Leather.
- Q2848 L45 Wild Leather Shoulders (pre 2847), Q2849 Vest (pre 2847),
  Q2850 Helmet (pre 2847), Q2851 Boots (pre none), Q2852 Leggings (pre
  none) — crafted-turn-in objectives (R5 handling: optional + skill gate +
  bag note).
- Q2853 L45 Master of the Wild Leather — pre all five; ends at Telonis in
  Darnassus (1438/1457): chain ending outside, IN. Next 5143 (outside).

Hatecrest chain (Feathermoon Stronghold):
- Q2866 L43 The Ruins of Solarsal — Shandris Feathermoon; ends at object
  Solarsal Gazebo (obj142179, 1444). Next: 2867.
- Q2867 L43 Return to Feathermoon Stronghold — object-start (Gazebo);
  ends at Shandris. Next: 3130.
- Q3130 L43 Against the Hatecrest — Shandris; ends at Latronicus
  Moonspear. Next: 2869.
- Q2869 L43 Against the Hatecrest — Latronicus; 10 Hatecrest items.
  Next: 2870.
- Q2870 L45 Against Lord Shalzaru — Latronicus; Lord Shalzaru's item.
  Next: 2871.
- Q2871 L45 Delivering the Relic — Latronicus; ends at Vestia Moonspear.

Troyas chain (Troyas Moonbreeze; middle links sit in Darnassus — see
BORDERLINE 1):
- Q2939 L47 In Search of Knowledge — Troyas; ends at Daryn Lightwind
  (Teldrassil/Darnassus map). Next: 2940 (Darnassus object — OUT).
- Q2879 L50 The Stave of Equinex — Troyas; pre 2943 (Darnassus — OUT);
  contracted with a `when onquest 2943` soft-pre (BORDERLINE 1). Ends at
  Equinex Monolith (obj144063, 1444). Next: 2942.
- Q2942 L50 The Morrow Stone — object-start (Equinex Monolith); ends at
  Troyas.

Kindal chain (min38 — the band floor):
- Q2969 L47 Freedom for All Creatures — Kindal Moonweaver; Sprite Darter
  rescue event at (67.27, 46.x) in the data. Next: 2970.
- Q2970 L47 Doling Justice — Jer'kai Moonweaver; Grimtotem kills.
  Next: 2972.
- Q2972 L47 Doling Justice — Jer'kai; ends at Tyrande Whisperwind in
  Darnassus: chain ending outside, IN. Next: 3841.
- Q3841 L47 An Orphan Looking For a Home — Kindal; ends at Quentin in
  Thousand Needles (1441): chain ending outside, IN. Next: 3842 (outside).

Alliance ogre line:
- Q2982 L44 The High Wilderness — Angelas Moonbreeze; Gordunni kills.
  No pre/next.

Sunken Temple breadcrumb:
- Q3445 L51 The Sunken Temple (min46 — in band) — Angelas Moonbreeze;
  ends at Marvon Rivetseeker in Tanaris (1446): chain ending outside, IN.
  Next: 3444 (outside). (Horde twin 3380 set aside.)

Low-level in-zone accepts (below-band, argued in BORDERLINE 2):
- Q3567 L25 To the Top — Marli Wishrunner (1444 point 45.82, 16.47).
  No objectives, no pre/next.
- Q98155 L29 Pristine Pesterhide Pelts — Kristy Grant (dual-spawn
  1441/1444; 1444 point 89.42, 45.99). Next: 98156.
- Q98156 L29 Packaged Pristine Pelts — Kristy Grant; ends at Kimberly
  Grant in Stormwind (1453): chain ending outside, IN.

Morrowgrain chain (Innkeeper Shyria / Quintis Jonespyre):
- Q3788 L50 Jonespyre's Request — Shyria; pre 3781 (Darnassus druid
  quest, contracted in darnassus.guide — outside this contract, so the
  accept rides a `when onquest 3781` soft-pre). Excl 3787 is the
  Stormwind-city twin (BORDERLINE 3). Next: 3791.
- Q3791 L50 The Mystery of Morrowgrain — Quintis; 10 Morrowgrain.
  Next: 3792.
- Q3792 L55 Morrowgrain to Feathermoon Stronghold — Quintis; 5
  Morrowgrain. (L55 finale, min47 in band — IN per the rule.)

Neutral lines (Gregan Brewspewer):
- Q4041 L52 The Videre Elixir (min47) — Gregan Brewspewer (neutral);
  pre 3909 (Winterscale/Winterspring 1452 — outside; soft-pre). Evoroot
  objective.
- Q4143 L52 Haze of Evil (min47) — Gregan Brewspewer; pre 4142 (Un'Goro
  1449 — outside; soft-pre). Ends at Muigin in Un'Goro (1449): chain
  ending outside, IN. Next: 4144 (outside).

Courier chain (Latronicus / Ginro Hearthkindle; object-mediated middle):
- Q4124 L43 The Missing Courier — Latronicus; ends at Ginro. Next: 4125.
- Q4125 L43 The Missing Courier — Ginro; ends at Wrecked Row Boat
  (obj164909, 1444). Next: 4127.
- Q4127 L44 Boat Wreckage — object-start (Row Boat); ends at Ginro.
  Next: 4129.
- Q4129 L44 The Knife Revealed — Ginro; ends at Quintis. Next: 4130.
- Q4130 L44 Psychometric Reading — Quintis; ends at Ginro. Next: 4131.
- Q4131 L44 The Woodpaw Gnolls — Ginro; ends at Large Leather Backpacks
  (obj164953, 1444). Next: 4135.
- Q4135 L46 The Writhing Deep — object-start (Backpacks); ends at
  Zukk'ash Pod (obj164954, 1444). Next: 4265.
- Q4265 L46 Freed from the Hive — object-start (Pod); Raschal escort
  event at (72.13, 63.84) in the data; ends at Ginro. Next: 4266.
- Q4266 L46 A Hero's Welcome — Ginro; ends at Shandris. Next: 4267.
- Q4267 L46 Rise of the Silithid — Shandris; ends at Gracina Spiritmight
  in Darnassus: chain ending outside, IN.

Zorbin chain (neutral goblin engineering):
- Q7003 L48 Zapped Giants (min45) — Zorbin Fandazzle; 15
  Miniaturization Residue. Next: 7725.
- Q7721 L48 Fuel for the Zapping (min45) — Zorbin; 10 Water Elemental
  Cores. Next: 7726.
- Q7725 L55 Again With the Zapped Giants (min45) — Zorbin; pre 7003.
- Q7726 L55 Refuel for the Zapping (min45) — Zorbin; pre 7721.

Druid class quest:
- Q81924 L50 Wisdom of the Guardians (min40; classes=1024, races=null)
  — Tyrisius (1444 point 57.16, 68.92). Gated `only Druid` in the guide.

WANTED poster:
- Q92858 L43 WANTED: Ohk'zi (min39) — object-start (WANTED! poster
  obj581918, 1444); Staff of Ohk'zi objective; ends at Latronicus. No pre.

Craftsman's Writs (item-started, end at Scout Raroul in Feralas
(72.41, 52.47); starter items have no placed source in the data — the
Wetlands precedent: contract with `optional` accept/turnin, bag note,
"at 60". See BORDERLINE 4):
- Q94260 L60 Catseye Draught, Q94272 L60 Blue Glittering Axe,
  Q94284 L60 Catseye Ultra Goggles, Q94296 L60 Wild Leather Shoulders.

## OUT list (50)

Horde set-aside (41 — for the Horde block's reconciliation):
2822 (Mark of Quality twin), 2854–2860 (Wild Leather twin chain, 7),
2862, 2863, 2902, 2903 (Hadoken Woodpaw chain, 4), 2973, 2974, 2976
(Krueg chain, 3), 2975, 2978, 2979, 2980 (Rok Orhan ogre chain, 4; 2978 is
the Gordunni Scroll item-start — sourceless in the data, Horde anyway),
2987, 3002, 3062, 3063 (Talo Thornhoof, 2), 3121, 3123–3129 (Uzer'i
muisek chain, 8), 3380 (Sunken Temple Horde twin), 4120, 7481 + 7489
(Elven Legends / Lethtendris Horde twins — also min54, above-band),
7730, 7731, 7732 (Hadoken Zukk'ash chain, 3), 7734 (Improved Quality
Horde twin), 7738 (Perfect Yeti Hide Horde twin), 92878 (Lost for Words).

Above-band (6, all min54+): 7441 (Pusillin, L58/min54, neutral), 7482
(Elven Legends Alliance twin, L60/min54), 7488 (Lethtendris's Web
Alliance, L57/min54, pre 7494 outside), 7785–7787 (Thunderfury chain,
L60/min60, neutral; 7785/7787 item-started with Silithus/MC sources).

Seasonal (2): 8679, 8685 (Lunar Festival elders, event=7).

Broken (1): 95599 The Old Key (L42/min null) — empty accept (no NPC,
object, or item start), no objectives, no pre/next; source is
questie-forever + webdb:xp with nothing routable. Unroutable, OUT.

## BORDERLINE

1. Troyas middle links (2940/2943/2944): 2939's next (2940) and 2879's
   pre (2943) both accept in Darnassus (2940 via the "Feralas: A History"
   object on map 1438; 2943 from Daryn Lightwind on 1438). The accept rule
   keeps them OUT of this contract, but the chain reads whole only if the
   guide bridges them: 2939 turns toward Darnassus with a note, and 2879's
   accept rides a `when onquest 2943` soft-pre mini-step standing alone.
   Contracted: 2939, 2879, 2942. Set aside, named, not silently dropped.
2. Below-band in-zone accepts (3567 min25; 98155/98156 min24): the band
   rule draws only the top line; the pack principle (every quest in its
   zone) keeps genuine in-zone accepts IN. Both givers have real 1444
   spawn points (Marli 45.82, 16.47; Kristy 89.42, 45.99). Contracted,
   flagged here so the low edge is a deliberate call.
3. Twins 3788/3787 (Jonespyre's Request): mutually exclusive variants
   (excl both ways); 3788 accepts in Feralas from Shyria, 3787 in
   Stormwind from Tannysa. Accept-zone rule contracts 3788 here (the
   94824/94817 precedent); 3787 stays Stormwind's. Chain-consistent:
   both share pre 3781 and next 3791, so no chain breaks either way.
4. Writs 94260/94272/94284/94296 (L60/min1, sourceless starters): the
   Wetlands round contracted its five writs on exactly this shape
   (in-zone ender, optional + bag note + "at 60"), and Scout Raroul
   spawns in Feralas at (72.41, 52.47). Contracted per that precedent.
5. min30 Wild Leather profession chain in a 38–50 zone: profession
   quests are IN per settled handling (optional + `when skill
   Leatherworking` gated); a level-38+ character can still work them,
   and the R5 craft-turn-in handling covers the objectives. Contracted.
6. 3445 vs 3380 (Sunken Temple, min46): faction twins, not same-name
   variants — 3445 (Angelas, Alliance) contracted, 3380 (Uzer'i, Horde)
   set aside. min46 is in band, so no band question.
7. 7481/7489 (Horde twins of 7482/7488): OUT as Horde; also min54,
   above-band. Listed in the Horde set-aside with the double reason.
