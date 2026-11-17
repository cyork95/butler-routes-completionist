# Tirisfal Glades census (pack butler-routes-completionist)

Zone key **1420** verified by counting: 159 quest records carry
`zone=1420`, and 171 start-NPC spawn refs land on 1420. The city key
**1458 (Undercity)** verified the same way: 124 quest records carry
`zone=1458`, 235 start-NPC refs land on 1458. The city rule applies
as in Durotar (Orgrimmar 1454) and Mulgore (Thunder Bluff 1456): a
giver spawning on BOTH 1420 and 1458 is a city NPC, even where its
1420 point sits on the open map (the dual points cluster at
57-66,67-69, the Undercity footprint). Those quests belong to the
future Undercity city census, NOT this contract.

Method: every quest with an accept/start touching 1420 - start NPC
spawning on 1420, start object spawning on 1420, or start item whose
drop source spawns on 1420 - was enumerated (175 candidates), then
filtered by the pack rules. Item-starts are enumerated explicitly
below (the Mulgore lesson); no absence is asserted without a
start-item scan.

Band **1-13**: lowest contracted minLevel 1 to highest contracted
quest level 13 (99156 Rear Guard Patrol, min6 - finale rule, same
shape as Durotar/Mulgore). The minLevel cluster is dense 1-10 (96
candidates), then 12 (the 5-quest Divinity paladin line), then a
gap: min15+ quests are chains whose working levels belong to the
10-20 bracket and are OUT by the minLevel line.

## IN (109)

Open-world Horde quests accepting on 1420 (and not on 1458),
minLevel in band, unhomed. Same-name twin IDs both routed (none in
this zone beyond the noted chains). Race gates follow the data
exactly (race bits: 16 Undead; Horde-all flag 8589934770). Class
quests carry the pack's `only <Class>` gating; the Undead-paladin
class line (classes=2) gates `only Paladin` + `only Undead` per line.

- 8 A Rogue's Deal (5/1) - 590 A Rogue's Deal (5/1; pre 8)
- 354 Deaths in the Family (11/7) - 355 Speak with Sevren (10/7;
  pre 354)
- 356 Rear Guard Patrol (11/6) - 99156 Rear Guard Patrol (13/6;
  pre 356; band-top finale)
- 358 Graverobbers (8/4) - 359 Forsaken Duties (9/6; pre 358) -
  360 Return to the Magistrate (9/6; pre 359)
- 361 A Letter Undelivered (7/4; ITEM-START: item 2839 from
  Rattlecage/Darkeye/Cracked Skull troops and Shadowvale Mystics,
  all 1420; no objectives; turn-in 1560)
- 362 The Haunted Mills (10/7)
- 363 Rude Awakening (1/1; races 16) - 364 The Mindless Ones (2/1;
  pre 363)
- 365 Fields of Grief (7/4) - 407 Fields of Grief (7/4; pre 365)
- 367 A New Plague (6/6) - 368 A New Plague (9/6; pre 367) -
  369 A New Plague (11/6; pre 368) - 492 A New Plague (11/6;
  pre 369)
- 427 At War With The Scarlet Crusade (8/5; pre 383) - 370 (9/5;
  pre 427) - 371 (10/5; pre 370) - 372 (12/5; pre 371) -
  374 Proof of Demise (7/5; pre 427)
- 380 Night Web's Hollow (4/2; pre 376) - 381 The Scarlet
  Crusade (4/2; pre 380) - 382 The Red Messenger (5/2; pre 381)
  - 383 Vital Intelligence (5/2; pre 382)
- 375 The Chill of Death (8/7)
- 376 The Damned (2/2) - 6395 Marla's Last Wish (5/3; pre 376)
- 398 WANTED: Maggot Eye (10/6; OBJECT-START: board 711
  @60.74,51.5 Brill)
- 404 A Putrid Task (6/4) - 426 The Mills Overrun (8/6; pre 404)
- 405 The Prodigal Lich (8/5; pre 358)
- 408 The Family Crypt (13/7; pre 355)
- 409 Proving Allegiance (12/5; pre 366, which is city-accepted
  and out of contract - structural pre, Darkshore handling in the
  guide) - 410 The Dormant Shade (10/5; pre 409; OBJECT-START:
  1557) - 411 The Prodigal Lich Returns (12/5; pre 409) -
  431 Candles of Beckoning (10/5; pre 409; OBJECT-START: 1586)
- 441 Raleigh and the Undercity (16/10; pre 440, which accepts in
  Silverpine 1421 and is out of contract - structural pre)
- 445 Delivery to Silverpine Forest (10/9)
- 5481 Gordo's Task (5/5) - 5482 Doom Weed (6/5; pre 5481) -
  99142 Tomb Weed (11/5; pre 5482)
- 99134 Discipline (6/4) - 99141 Patience (6/4)
- 86784 Sticks and Bones (7/4)
- 3901 Rattling the Rattlecages (3/1; pre 364) - 3902 Scavenging
  Deathknell (3/2; pre 376)
- 3095 Simple Scroll (1/1; Warrior; pre 364) - 3096 Encrypted
  Scroll (1/1; Rogue; pre 364) - 3097 Hallowed Scroll (1/1;
  Priest; pre 364) - 3098 Glyphic Scroll (1/1; Mage; pre 364) -
  3099 Tainted Scroll (1/1; Warlock; pre 364)
- 98601 A Difficult Path (1/1; Paladin; pre 364)
- 90902 Rediscovering the Light (2/2; Paladin; pre 364) -
  91208 Coming to Terms (4/4; Paladin; pre 90902) - 91209
  Continue Your Training (4/4; Paladin; pre 90902)
- 98389 A Light in the Darkness (4/2; pre 376)
- 1470 Piercing the Veil (3/1; Warlock; excl Durotar 1485 -
  Tirisfal variant IN)
- 1478 Halgar's Summons (10/10; Warlock; excl Durotar 1506 -
  Tirisfal variant IN)
- 1818 Speak with Dillinger (10/10; Warrior; excl Durotar 1505
  and Barrens 1498 - Tirisfal variant IN) - 1819 Ulag the
  Cleaver (10/10; Warrior; excl 1498) - 1820 Speak with Coleman
  (10/10; Warrior; pre 1819) - 1821 Agamand Heirlooms (11/10;
  Warrior; pre 1820) - 1822 Heirloom Weapon (11/10; Warrior;
  pre 1821)
- 1881 Speak with Anastasia (10/10; Mage; excl Durotar 1883/1884
  - Tirisfal variant IN)
- 1885 Mennet Carkad (10/10; Orc Rogue; excl Durotar 1859 -
  Tirisfal variant IN)
- 5650 Garments of Darkness (4/5; Undead Priest; pre 5651) -
  5651 In Favor of Darkness (4/5; Undead Priest)
- 97558 Hides for the Forsaken (11/6)
- 99144 Seeking Refuge (7/5)
- 99152 As Above, So Below (12/10; pre 96896) - 99153 The One
  That Got Away (12/10; pre 96896)
- 96895 The Argent Emissary (12/10) - 96897 The Cult of the
  Damned (12/10; pre 96895) - 96898 Remnants of War (12/10;
  pre 96895) - 96899 Bandarion Keep (12/10; pre 96897/96898) -
  96896 A Righteous Cause (12/10; pre 96899) - 98545 Leonid's
  Letter (12/10; pre 96896)
- Paladin west line (all races 16): 91282 A Second Home (11/8) -
  91285 Murlocs at the Gates (11/7) - 91294 Touring the Grounds
  (11/8; pre 91285) - 91316 Making Repairs (11/8; pre 91294) -
  91317 The Tarnished (12/9; pre 91294) - 95803 A Token of Good
  Faith (12/9; pre 91317; turn-in 10181 in Undercity - city
  expedition close) - 94427 A Lesson in Divinity (12/12) -
  94436 A Lesson in Divinity (12/12; pre 94435, which is
  city-accepted and out of contract - structural pre) - 94438
  (12/12; pre 94436) - 94440 (12/12; pre 94438) - 94441 (12/12;
  pre 94440)
- Camping chain, optional + `when skill` gated per the
  Durotar/Mulgore handling (only the operative one functional;
  sequenced so the route never wedges): 96656 The Adventurer
  (6/4; pre 382) - 96607 The Great Outdoors (6/4; pre 96656) -
  96658 Camping 101: Cooking (6/4) + 97951-97961 the eleven
  Camping 101 profession quests (6/4 each, skill-gated)
- 95314 That Shadowvale Green Elixir (10/7)
- 79095 The Apothecary's Metaphysical Primer (20/1; OBJECT-START:
  primer 405879 @59.4,52.3 Brill; turn-in 211022 Undercity -
  admitted by the finale rule's minLevel clause as the band's
  documented high-level exception; see BORDERLINE)
- 95328 Whispering Horror Residue (13/7; ITEM-START: item 268812
  from Whispering Horror 260396 on 1420; see BORDERLINE)

## OUT by rule

City-key exclusions (dual 1420+1458 spawn = city NPC; belong to the
future Undercity census): 357, 366, 446 (Bethor Iceshard); 1882,
1943, 1947, 1953, 1960, 1961 (Anastasia Hartwell); 4489, 4739,
4969 (Kaal Soulreaper); 5643, 5657, 5658, 5679 (Aelthalyste);
65593 (Godrick Farsan). Matches of already-OUT quests (1718,
1823, 1947, 1953, 7562, 8250, 8417, 8419) also resolve to city
NPCs and stay out.

Accept-outside: 1718 (city-homed via dual starter; zonefield
1412); 1823 (Orgrimmar 1454); 635 (Arathi-homed - Arathi contracts
it as a no-turn-in record; its 1420 dropper is Scarlet mob spill);
3861 CLUCK! (Westfall-homed, zonefield 1436 - and contracted
NOWHERE; finding for a future Westfall addendum, the 934 pattern);
7562 (Stormwind 1453); 8250 (Ironforge 1455); 8417 (Orgrimmar
1454); 8419 (Stormwind 1453).

Above-band (minLevel above 1-13): 105, 838, 964, 5096, 5098, 5228,
5229, 5231, 5233, 5235, 5238, 5341, 5342, 5405, 5406, 5407, 5408,
5504, 5511, 5514, 5524, 5804, 5901, 5902, 97319 (all min 48-55,
endgame); 1943 (26); 1947 (30); 1953 (35); 1959, 1960, 1961 (15,
mage Alchemist chain); 92422 (15, follow-up of contracted 99156 -
chain stub noted); 91858 (18); 4489 (40); 4739 (31); 4969 (35);
94971 (40); 96997, 97203 (40, mount exchanges - also
repeatables); 2861 (40); 1657, 8322 (25/30, also seasonal event
12).

Seasonal/event: 1657, 8322 (event 12); 8652 (event 7 Lunar
Festival); 8827, 8828 (event 21); 8860, 8861 (event 34); 8902
(event 8).

Repeatables: 96997, 97203 (mount exchanges); 5405 (Argent
commission; also above-band).

Broken/incomplete: 1476 Hearts of the Pure (level -1).

[PH] placeholders: none found.

Alliance set-asides: NONE - no Alliance-only quest accepting on
1420 was found; every candidate mask is Horde-compatible
(8589934770, 16, 146, 144, 128) or neutral-seasonal
(4294967373 on the excluded event quests).

## BORDERLINE

- 79095 vs the city rule: zonefield 1458 and city turn-ins, but
  the primer object sits at Brill on 1420 and the Sealed Supply
  Crate precedent (751) contracts object-starts by physical
  location. IN, turn-in as a city expedition leg.
- 95328 vs the city rule: zonefield 1458, but the start item
  drops only from a 1420 mob. The Mulgore 98424 lesson (item
  starts are IN by source location) says IN. IN.
- 92422: direct follow-up of contracted 99156 but min15, above
  the band. The minLevel line holds (Durotar/Mulgore above-band
  precedent) - OUT with the stub noted, not silently.
- The 1959 mage chain (1959/1960/1961, min15): same line - OUT
  above-band; 1960/1961 are city-accepted anyway.
- 5643/5657/5658/5679: min20 AND city-accepted (Aelthalyste) -
  double reason OUT. The Tirisfal priest intro the guide DOES
  carry is 5650/5651 (Deathknell, Undead Priest, in-band).
- 3861: Westfall-homed but homeless - OUT here, flagged for a
  Westfall addendum ruling.
- 409/441/94436: IN with out-of-contract pres (city 366,
  Silverpine 440, city 94435) - structural pre warnings in the
  guide, Darkshore handling, not silent.
- 635: Arathi-homed despite 1420 Scarlet droppers - OUT, home
  guide owns it.
