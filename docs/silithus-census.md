# Silithus census (accept-zone key 1451, Alliance route)

Method: local game data (`upstream-polestar/data/forever`, built with
`--product wowf` + QuestieDB), same as all previous zones. Candidate set:
every quest whose start NPC, start object, or start-item dropper has a spawn
on map key 1451. Result: **112 candidates**. Accept-zone key verified by
counting: 104 giver-NPC candidates + 4 object-start discoveries + 4 item-start
discoveries.

Band: the contracted minLevels cluster at 54/57/58/60 (quest levels 50-60).
Band set to **54-60**: lowest clustered contracted minLevel to highest
contracted quest level, the zone-finale rule. Three contracted records sit
below the cluster (3884 min48; 9415/9419 min1) and are documented as
below-band outliers in BORDERLINE (B5, B6) — the formula's floor is the
cluster, not the outliers.

Contract: **52 quests** (see `docs/quest-contracts.json`, zone `silithus`,
order 43).

## IN ledger (52)

Giver locations are map-1451 points from the data dump in front of me.

Southwind chain (Layo Starstrike, 81.87,18.93, far east):
- 1125 The Spirits of Southwind (55/54, pre 1124 Moonglade OUT -> soft-pre)
- 1126 Hive in the Tower (57/54; Encrusted Silithid Object from Hive'Ashi Ambusher 60.2,52.4)
- 6844 Umber, Archivist (57/54; turn-in Umber in Moonglade — chain ends outside, still IN)

Thunderaan chain (Highlord Demitrian dual-spawns Feralas/Silithus; Silithus point 21.71,8.57):
- 7785 Examine the Vessel (60/60, item-start: Vessel of Rebirth drops from Demitrian in-zone)
- 7786 Thunderaan the Windseeker (60/60; Essence of the Firelord + 2 Bindings + 10 Elementium Bars have no placed spawns in the data — raid-interior/crafted, honest note-only naming at Demitrian, the winterspring precedent)

Cenarion Hold west (Beetix Ficklespragg 51.61,38.63):
- 8277 Deadly Desert Venom (55/54; Stonelash Scorpid + Sand Skitterer grounds, in-zone)
- 8278 Noggle's Last Hope (57/54; Flayer/Pincer/Rock Stalker grounds, in-zone)
- 8282 Noggle's Lost Satchel (58/54, from Noggle 51.63,38.50; satchel has no dropper in the data — ground pickup, R2 note)

Windcaller Proudhorn (51.15,38.29):
- 8280 Securing the Supply Lines (55/54, pres 8275+8276 accept in Ironforge/Orgrimmar OUT -> soft-pre mini; Dredge Strikers)
- 8281 Stepping Up Security (57/54; Dredge Crushers)

Wanted (object 180448 Wanted Poster: Deathclasp 51.35,38.27):
- 8283 Wanted - Deathclasp, Terror of the Sands (59/54; Deathclasp 45.07,92.31, turn-in Vish Kozus 50.75,33.65)

Twilight/geologist chain (Geologist Larksbane 49.67,37.46):
- 8284 The Twilight Mystery (58/54; Twilight Tablet Fragments from Dust Stormer/Desert Rumbler/Whirling Invader, all in-zone)
- 8285 The Deserter (59/54; turn-in Hermit Ortell 67.19,69.76 — its next 8279 is event-gated OUT, chain parks honestly)
- 8287 A Terrible Purpose (60/54, pre 8279 OUT -> soft-pre mini with the event caveat, B7)
- 8314 Unraveling the Mystery (60/58, pres 8309+8310; turn-in back at Larksbane)
- 8315 The Calling (60/58; Crystal Unlocking Mechanism from Emissary Roman'khan 48.77,58.14)
- 8316 Armaments of War (60/58, only Warrior; talk, no objectives)
- 8376 Armaments of War (60/58, only Paladin; Alliance-gated talk)
- 8377 Armaments of War (60/58, only Hunter)
- 8378 Armaments of War (60/58, only Rogue)
- 8379 Armaments of War (60/58, only Priest)
- 8381 Armaments of War (60/58, only Mage + only Warlock lines; talk)
- 8382 Armaments of War (60/58, only Druid)

Scepter chain (Baristolth of the Shifting Sands 49.45,36.45):
- 8286 What Tomorrow Brings (60/60; Anachronos visit + "Discover the Brood of Nozdormu" event objective at Tanaris CoT 64.6,50.42 — Tanaris expedition leg)
- 8288 Only One May Rise (60/60; Broodlord Lashlayer's Head has no placed spawn — BWL interior, note-only naming at Baristolth)
- 8301 The Path of the Righteous (60/60; 200 Silithid Carapace Fragments from Hive'Ashi mobs, in-zone)
- 8303 Anachronos (60/60; turn-in Anachronos in Tanaris 65.27,50.03 — chain ends outside, still IN)

Natalia chain (Commander Mar'alith 49.2,34.18):
- 8304 Dearest Natalia (60/58; Frankal Stonebridge 40.81,88.86 + Rutgar Glyphshaper 41.28,88.45, far south)
- 8306 Into The Maw of Madness (60/58; Mistress Natalia Mar'alith 44.4,86.11)
- 8309 Glyph Chasing (60/58, from Rutgar; 3 hive rubbings have no droppers in the data — R2 note naming the hives)
- 8310 Breaking the Code (60/58, from Frankal; silithid brains from Ashi/Zora/Regal hives, in-zone)

Cooking chain (Calandrath 51.89,39.16; profession-gated, optional):
- 8307 Desert Recipe (57/54; turn-in to object Sandy Cookbook 37.94,45.31)
- 8313 Sharing the Knowledge (57/54; accept from the Sandy Cookbook object)
- 8317 Kitchen Assistance (57/54; 10 Smoked Desert Dumplings, no droppers — player-crafted R5, optional + when-skill Cooking + bag note)

Twilight texts (Bor Wildmane 48.57,37.78):
- 8318 Secret Communication (60/57; 10 Encrypted Twilight Texts, 11 droppers all in-zone; next 8319 is repeatable OUT)

Abyssal council chain (Huum Wildmane 48.62,37.87; Bor; Aurel Goldleaf 51.96,38.16):
- 8320 Twilight Geolords (60/60; 10 Twilight Geolords, in-zone)
- 8321 Vyral the Vile (60/60; Vyral's Signet Ring from Vyral 72.39,15.58 — spawns in-zone, not a dungeon case)
- 8331 Aurel Goldleaf (60/60; opener, talk)
- 8343 Goldleaf's Discovery (60/60; handoff to Aurel)
- 8332 Dukes of the Council (60/60; Large Brilliant Shard — no droppers, disenchant product, bag note + complete at Aurel; 3 Abyssal Crests from Templars, in-zone)
- 8341 Lords of the Council (60/60; 5 shards bag note; 3 Abyssal Signets from Dukes, in-zone)
- 8349 Bor Wildmane (60/60; handoff to Bor; next 8348)
- 8348 Signet of the Dukes (60/60, from Bor; 1 Abyssal Signet)
- 8351 Bor Wishes to Speak (60/60; handoff to Bor; next 8352)
- 8352 Scepter of the Council (60/60, from Bor; Abyssal Scepter from Skaldrenox/Whirlaxis/Kazum/Skwol, in-zone)
- 9248 A Humble Offering (60/58, from Aurel; 1 Abyssal Scepter, same droppers — standalone)

Crystalline Tear (object 180633, 28.68,89.14, far south):
- 8519 A Pawn on the Eternal Board (60/60, pre 8305 accepts in Tanaris OUT -> soft-pre mini at Anachronos + Tear turn-in 8305; event objective "The War of the Shifting Sands" at 29.04,92.09 in-zone; turn-in Anachronos in Tanaris — chain ends outside)

Rogue poison (Dirk Thunderwood 52.13,39.14):
- 9023 The Perfect Poison (60/60; Venoxis's + Kurinnaxx's Venom Sacs have no placed spawns — ZG bosses; Gates of Zul'Gurub at 1434 (53.9,17.6) carry the completes with a note)

Entry breadcrumbs (Rifleman Torrig 50.68,34.71; Marshal Bluewall 33.29,51.06; Alliance-only):
- 9415 Report to Marshal Bluewall (60/min1; talk Torrig -> Bluewall; below-band outlier, B6; natural zone entry)
- 9419 Scouring the Desert (60/min1; kill quest doodad 32.95,50.81, turn-in Bluewall; below-band outlier, B6)

Item-start outlier:
- 3884 Williden's Journal (50/min48; A Mangled Journal drops from Frenzied Pterrordax 79,43.2/80,62.7 in-zone east, plus 47 Un'Goro + 1 Tanaris droppers — B5; turn-in Williden Marshal in Un'Goro — chain ends outside; below-band outlier)

## OUT ledger

Event-gated one-time records (35 total counting the rep+event overlap once; data `event` field set):
- AQ gate-event cluster ev85/86 (30): 8743 Bang a Gong! (ev85, pre 8742 Tanaris); 8745 Treasure of the Timeless One; 8800 Cenarion Battlegear; 8556/8557/8558 Signet/Drape/Sickle of Unyielding Strength (Warrior); 8689-8712 the 24 class-armor set (incl. Horde Shaman 8690/8698/8706); 8654/8719 are ev7, counted below. Rep+event members (8507/8508 Field Duty pair, 8548/8572/8573/8574 battlegear, 8731/8732 Horde Field Duty) are listed under repeatables with the event reason attached.
- Hive-phase ev62/63/64 (3): 8857/8858/8859 Secrets of the Colossus (Ashi/Regal/Zora). Each carries a unique event id no other quest uses.
- Lunar Festival ev7 (2): 8654 Primestone the Elder (Elder Primestone 23.08,11.84), 8719 Bladesing the Elder (Elder Bladesing 48.96,37.66).

Repeatable (18): 8302, 8319, 8324, 8333, 8342, 8362, 8363, 8364, 8770 (item-start repeatable, Hive'Ashi Defenders), 9338 (Allegiance), plus the 8 ev86 reps (8507, 8508, 8548, 8572, 8573, 8574, 8731 Horde, 8732 Horde).

Horde set-asides (9, for the Horde block): 8380 Armaments of War (Shaman); 8690/8698/8706 Shaman class armor; 8731/8732 Field Duty pair (also rep+event); 9416/9422 the Horde intro mirrors (Report to General Kirika / Scouring the Desert); 98093 Field to Clear (also broken — see B10).

Above-band: none (highest quest level 60, no contracted minLevel above 60).

Accept-outside ledger notes (not candidates; named for chain bookkeeping): 8275 Taking Back Silithus (Ironforge), 8276 Taking Back Silithus (Orgrimmar), 1124 Wasteland (Moonglade), 6845 Uncovering Past Secrets (Moonglade), 8305 Long Forgotten Memories (Tanaris, Anachronos), 8742 The Might of Kalimdor (Tanaris, Anachronos).

## BORDERLINE

- B1 (AQ gate-event cluster OUT): the data flags 30 one-time quests (plus 8 repeatables) with events 85/86 — the gong singleton, the battlegear chain, Field Duty, the 24-strong class-armor set, Treasure of the Timeless One. The pack excludes event quests by rule, and these ids appear on nothing obtainable outside the gate event (the cluster shape matches one server-phase: 85 = the gong itself, 86 = the opened-gate content, paralleling war-effort ev22). If Butler verifies gates-open content is permanently available, 30 quests come back in a later round.
- B2 (hive-phase events OUT): 8857-8859 each carry a unique event id (62/63/64) no other record uses — event-gated per the data, so OUT. Same re-verification path as B1 (3 quests, min51).
- B3 (elders OUT vs older-zone precedent): 8654/8719 are genuine Silithus accepts (points above) but Lunar Festival seasonals. Older zone rounds contracted elders (TN 8682/8724, SG 8651, Felwood 8723, Azshara 8720); this round follows the brief's OUT rule for seasonal/event quests and the immediately-previous Winterspring call (which set its 2 elders OUT with the same reason). Flagging the inconsistency rather than deciding silently.
- B4 (Thunderaan IN): 7785's start item drops in-zone (Demitrian's Silithus spawn 21.71,8.57) and 7786 accepts/turns in at Demitrian's Silithus spawn — accept-in-zone is met. Raid-fetched objectives (Ragnaros essence, 2 Bindings — no placed spawns anywhere in the data; Elementium Bars crafted) ship as honest note-only naming at the turn-in, the winterspring dungeon-interior precedent. Legendary chain stays routable without inventing a single coordinate.
- B5 (3884 IN): the journal's 48 droppers are mostly Un'Goro (44
...[truncated 2085 chars]
