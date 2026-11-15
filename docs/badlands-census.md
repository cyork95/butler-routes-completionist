# Badlands census (game data, accept-zone key 1418)

Source: local Forever game data (questie-forever quest/npc/object dumps).
Faction decode (settled rounds): races 4294967373 = Alliance-only,
races 8589934770 = Horde-only, races null = neutral (available to all,
contracted on the Alliance route per the Stranglethorn neutral-giver
ruling). No quest in the candidate set carries a class restriction, so
the guide needs no `only <Class>` gates; no race-exclusive records
beyond the Horde set-aside, so no `only <Race>` gates either.

## Band derivation

Non-Horde minLevel histogram over the 77 zone-keyed records:
min1 x4 (the four level-60 writs), min28 x2, min30 x8, min33 x1,
min35 x17, min40 x5, min48 x1, min55 x2, null x2 (broken, see below).
The working cluster runs min28-min40: the min28 Martek the Exiled
on-ramp at the bottom, the min40 finale cluster (Fiery Blaze
Enchantments, both Tremors of the Earth legs, the Seal of the Earth
turn-in record, the Platinum Discs record) at the top. min48 (Ribbly
Screwspigot, whose objective leg runs into the Burning Steppes) and
min55 (the two Kibler pet-vs-pet records) are above the band. Derived
band: **28-40**.

## IN — 35 quests (the contract)

| ID | Title | Lvl | min | Giver (accept) | Notes |
|----|-------|-----|-----|----------------|-------|
| 656 | Summoning the Princess | 50 | 30 | Theldurin the Lost (51.39,76.87) | turn-in at the Shards of Myzrael object, which spawns in Arathi (1417) — expedition turn-in |
| 692 | The Lost Fragments | 41 | 30 | Theldurin the Lost | pre 687 (Ironforge quest Theldurin the Lost) sits outside the contract — structural, chain named |
| 703 | Barbecued Buzzard Wings | 40 | 33 | Rigglefuzz (42.39,52.93) | |
| 705 | Pearl Diving | 37 | 30 | Rigglefuzz | pre for Flash Bomb Recipe |
| 706 | Fiery Blaze Enchantments | 45 | 40 | Sigrun Ironhew (53.8,43.3), Alliance | finale cluster |
| 709 | Solution to Doom | 40 | 30 | Theldurin the Lost | pre for the Yagyin chain |
| 710 | Study of the Elements: Rock | 37 | 35 | Lotwil Veriatus (25.95,44.87) | chain 710->711->712 |
| 711 | Study of the Elements: Rock | 39 | 35 | Lotwil Veriatus | pre 710 |
| 712 | Study of the Elements: Rock | 42 | 35 | Lotwil Veriatus | pre 711 |
| 713 | Coolant Heads Prevail | 37 | 35 | Lotwil Veriatus | pre for Gyro |
| 714 | Gyro... What? | 37 | 35 | Lotwil Veriatus | pre 713 |
| 715 | Liquid Stone | 37 | 35 | Lucien Tosselwrench (25.82,44.24) | pre 714 |
| 716 | Stone Is Better than Cloth | 42 | 35 | Lucien Tosselwrench | pre 712 |
| 717 | Tremors of the Earth | 50 | 40 | Garek (61.94,54.26), Alliance | finale, pre 732; the repeatable Seal turn-in (779) is NOT contracted |
| 718 | Mirages | 38 | 35 | Sigrun Ironhew, Alliance | pre for the Tremors/Scrounging legs |
| 719 | A Dwarf and His Tools | 35 | 35 | Prospector Ryedol (53.42,43.39), Alliance | |
| 720 | A Sign of Hope | 35 | 35 | Crumpled Map object (53.03,33.94), object-start | same-name twin with 721, both routed (Harvesting precedent) |
| 721 | A Sign of Hope | 35 | 35 | Prospector Ryedol | pre 720 |
| 724 | Prospect of Faith | 40 | 35 | Prospector Ryedol, Alliance | pre 723 (Loch Modan quest Prospect of Faith, not contracted anywhere) — structural, chain named; turn-in to Historian Karnik (Ironforge) ends the chain outside |
| 727 | To Ironforge for Yagyin's Digest | 40 | 30 | Theldurin the Lost, Alliance | pre 709; turn-in to Gerrig Bonegrip (Ironforge) ends outside |
| 732 | Tremors of the Earth | 43 | 40 | Garek, Alliance | pre 718; sourceItem 4640 rides the accept |
| 733 | Scrounging | 40 | 35 | Sigrun Ironhew, Alliance | pre 718 |
| 734 | This Is Going to Be Hard | 42 | 35 | Lotwil Veriatus | triple chain 734->777->778, needs both 712 and 714 done |
| 739 | Murdaloc | 42 | 30 | Battered Dwarven Skeleton object (50.89,62.4), object-start | pre 738 (Loch Modan quest Find Agmond, not contracted anywhere) — structural, chain named; turn-in to Prospector Ironband (Loch Modan) ends outside; kill objectives 2945/2893 placed in-zone |
| 777 | This Is Going to Be Hard | 42 | 35 | Lucien Tosselwrench | pre 734; sourceItem 4846 rides the accept |
| 778 | This Is Going to Be Hard | 45 | 35 | Lotwil Veriatus | pre 777, finale of the triple |
| 1108 | Indurium | 39 | 28 | Martek the Exiled (42.22,52.69) | pre 1106 (Thousand Needles quest Martek the Exiled) sits outside — structural, chain named; bottom of the band |
| 1137 | News for Fizzle | 38 | 28 | Martek the Exiled | pre 1108; turn-in to Fizzle Brassbolts (Thousand Needles) ends outside |
| 1559 | Flash Bomb Recipe | 37 | 30 | Rigglefuzz | pre 705 |
| 2418 | Power Stones | 36 | 30 | Rigglefuzz | |
| 94256 | Craftsman's Writ: Frost Protection Potion | 60 | 1 | item-start (writ in bags) | turn-in to Lotwil in-zone; bag note, never wedges (Tanaris writ precedent) |
| 94268 | Craftsman's Writ: Steel Plate Helm | 60 | 1 | item-start | turn-in to Furious Shadowforge Digger (44.29,11.42) in-zone; bag note |
| 94292 | Craftsman's Writ: Comfortable Leather Hat | 60 | 1 | item-start | turn-in to Garek in-zone; bag note |
| 94304 | Craftsman's Writ: Mageweave Bag | 60 | 1 | item-start | turn-in to Rigglefuzz in-zone; bag note |
| 97617 | Safety Checks | 40 | 35 | Dorgaron (54.63,12.87), Alliance | objectives are item collects 278402-4, placed per the item-drop audit at guide time |

## OUT — 7 non-Horde records with reasons

- 779 Seal of the Earth (lvl50 min40): repeatable (rep=true) — the turn-in leg of a repeatable cycle; the one-time chain (718->732->717) is contracted without it.
- 2278 The Platinum Discs (lvl47 min40): broken/incomplete — its accept/end object (The Discs of Norgannon, 131474) has zero spawns anywhere in the data, so the route cannot point at it; revisit if the data ever places it.
- 4136 Ribbly Screwspigot (lvl53 min48): above-band per the minLevel rule; its giver Yuka Screwspigot spawns in-zone (4.9,94.7) but the record's own level and its Burning Steppes objective leg mark it as next-zone content.
- 4729 Kibler's Exotic Pets (lvl59 min55): above-band; giver Kibler spawns in-zone (4.7,94.6).
- 4862 En-Ay-Es-Tee-Why (lvl59 min55): above-band; same giver.
- 97663 Supplies and Studies (lvl40, minLevel null): broken/incomplete — null minLevel with an empty objectives array against an objectiveText that describes objectives; unroutable as stated.
- 97821 Mirage Mirror (lvl42, minLevel null): broken/incomplete — no accept/start at all (empty start), so no route can take it; turn-ins at Dorgaron/Mus'hale noted but not contracted.

## OUT — Horde set-aside, 35 records (for the Horde block's reconciliation)

728, 782, 793, 795, 1419, 1420, 2202, 2203, 2258, 2318, 2338, 2339, 2340,
3821, 3822, 3906, 3907, 3981, 4061, 4062, 4063, 4081, 4082, 4122, 4132,
4134, 4724, 4768, 4903, 4941, 4981, 4983, 5145, 7201, 98325.
All carry races 8589934770. Includes the Kargath-side chains, the
Jarkal Mossmeld reagent chain, the Warlord Goretooth/Shadowmage Vivian
chains, the Dragonscale Leatherworking record 5145 (mutually exclusive
with Alliance records 5146/5148, neither in this zone's data), and the
Blood and Thunder record 98325.

## BORDERLINE (argued, none decided silently)

1. The min28 bottom: Martek records 1108 (min28) and 1137 (min28) sit
   below the min30 bulk, but Martek spawns in-zone and the chain is
   genuine Badlands content (its pre 1106 lives in Thousand Needles,
   its turn-in leg for 1137 lands back in Thousand Needles — chains
   ending outside are IN). The band bottom is 28, not 30.
2. The min1/lvl60 writs (94256, 94268, 94292, 94304): contracted IN per
   the Tanaris writ precedent and the pack's item-start rule — one-time
   records, all four turn-ins spawn in-zone, sequenced with bag notes
   so the route never wedges on the drop.
3. Ribbly Screwspigot (4136) OUT: a Badlands-spawning giver is not
   enough — min48 is above the band by the mechanical rule, and the
   objectiveText sends the player to the Burning Steppes, the next
   zone east. If the band ever widens, this is the first record back.
4. The Platinum Discs (2278) OUT as broken rather than IN as a finale:
   the min40 finale cluster would otherwise hold it, but an accept
   object with no spawns anywhere cannot be pointed at. This is a data
   gap, not a design call.
5. Supplies and Studies (97663) and Mirage Mirror (97821) OUT as
   broken: both are Forever records (questie-forever source) with null
   minLevel; 97821 additionally has no accept. The Dustbowl objective
   text on 97663 reads real, so flag it for re-census if the record
   gains objectives.
6. Seal of the Earth (779) OUT as repeatable while its chain stays IN:
   the one-time Tremors chain (718->732->717) completes the story; the
   rep=true turn-in cycle is the repeatable rule's exact target.
7. Same-name twins 720/721 (A Sign of Hope) both IN: one object-start,
   one NPC follow-up — the Harvesting the Harvesters precedent.
8. Out-of-contract pres (723 and 738 in Loch Modan's map but in no
   contract, 687 an Ironforge quest, 1106 a Thousand Needles quest):
   the guide routes the Badlands sides normally and reports the
   resulting structural warnings with the chain named; 4324 IS
   Tanaris-contracted but 4136 (its dependent) is out on band, so no
   link is needed in either direction.
9. No class gates, no race gates: verified — every non-Horde record
   carries classes null, and the only races values present are null
   (neutral, available to all) and the Alliance mask. The guide needs
   no `only` lines for class or race.
