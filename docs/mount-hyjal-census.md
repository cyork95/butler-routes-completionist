# Mount Hyjal census (accept-zone key 2482, Alliance route)

Method: local game data (`upstream-polestar/data/forever`, built with
`--product wowf` + QuestieDB), as in all previous zones. The accept-zone key
was NOT assumed: the playtest simulator's map table labels key 2482
"Mount Hyjal" (earlier lead), verified here by counting — **157 NPC spawns
and 16 object spawns live on key 2482**, including Hyjal-named NPCs (Hyjal
Bear/Stag/Owl/Dryad/Sentinel/Protector/Grovewalker/Druid). No competing key
exists: every Hyjal-named NPC spawns on 2482 or nowhere. No Silithus-style
side-bucket: the only non-2482 keys touched are objective/turn-in locations
in other zones (expedition legs), never accepts. Candidate set: every quest
whose start NPC, start object, or start-item dropper has a 2482 spawn.
Result: **137 candidates**.

Band: recorded contracted minLevels cluster at 54 (one at 57); quest levels
run 55-60. Band set to **54-60**: lowest recorded contracted minLevel to
highest contracted quest level. The many minnull records ride along (B1).

Contract: **123 quests** (see `docs/quest-contracts.json`, zone
`mount-hyjal`, order 44). No class gates and no profession gates anywhere in
the contract (every record has classes=null, skill=null); Alliance-gated
lines ride inline by quest races, everything else is neutral.

## IN ledger (123)

Giver points are map-2482 spawns from the data dump in front of me, grouped
by hub/chain.

Western post (Sefira Everbright 15.67,54.66; Daythor Brellan 15.55,52.07;
Mirt 15.93,52.72; Hnaz Blunderflame 15.64,49.99; Kal'tinzan 13.77,53.06):
- 92449 Blight No More (58/54, Alliance; kills in-zone)
- 90750 More Work? (55, pre 92449; Horde twin pre 95026 stays out, B2)
- 95218 More of the Same (56/54, pre 90750)
- 94832 Belle's Ring (58/54, Alliance, pre 95218, next 96077)
- 96077 Belle's Ring (58/54, Alliance, pre 94832; accept-only, no turn-in in
  the data — honest note, Ironforge precedent)
- 92591 Final Death (59/57, Alliance; Reanimator's Amulet in-zone)
- 91688 To the Summit of Eternity (59/54, Alliance, pres 92449+92591;
  turn-in Thisalee Crow far east)
- 90854 Leather for Inclement Weather (57, neutral; Zet'gan post, B2)
- 92433 Now We're Cooking (57, neutral; Hnaz; no objectives)
- 95027 Feathers in Flight (57/54, Alliance; Owl Feather in-zone)
- 96674 Ewe Wandered Off (56/54, Alliance; sheep in-zone)
- 95769 Threading a Solution (57, neutral; Bolt of Runecloth is
  Tailoring-crafted / generic world drop — bag note at turn-in, no complete)

Southwest furbolg/barkskin (Brerufa 20.56,71.73; Osi 21.08,80.19; Elder
Mistpaw 21.77,78.98; Pinespeaker turn-in 21.77,79.37; Suma 20.82,79.81;
Thobon 18.52,78.6; Fenwick 25.31,75.87; Survival Pack 25.46,74.62;
Shalla'kal 31.3,50.3; Kala'th 28.68,43.04; Matriarch 31.5,58.59):
- 93952 Balance Through Strength (57; Den Guardians in-zone)
- 92111 Of Friend and Fur (57, pre 93952; turn-in Osi)
- 93831 Sweetpaw Jam (57, pre 92111; Bear Berries have no droppers — R2 note)
- 91697 Meet the Elders (57, pre 93831; turn-in Elder Mistpaw)
- 93825 Barkbound Blessings (57, pre 91697; Moonveil Moss no droppers — note)
- 93826 Deal Dread to Deadwood (57, pre 91697; two kill sets in-zone)
- 93827 Windswept Wards (58, pre 91697; Harpy Amulets in-zone)
- 94504 Barkskin Beginnings (57; Elder Mistpaw, no objectives)
- 92702 Branch Out (56/54, Alliance; Sturdy Branch no droppers — note)
- 92064 Tree Free (56/54, Alliance, pre 92702)
- 96559 Supply Drop (57/54, Alliance, pre 92064; turn-in Survival Pack)
- 93383 Contents Under Pressure (57/54, Alliance, pre 96559; Pack, no obj)
- 91698 Barkskin Breakout (58; Deadwood Key in-zone)
- 91696 Open Season (58; Matriarch; accept-only, no turn-in — honest note)
- 93615 Kits and Cats (57; Shalla'kal, no objectives)
- 93617 Prey and Predator (57, pre 96978; Predatory Stags in-zone)
- 96978 Violent Venison (57, pre 96931; turn-in Kala'th)

Elder grove (Hyacinth 54.05,84.39; Fraxinus 53.4,84.33; Thylaen 54.83,84.56;
Curious Crow 48.26,85.72; Felflick 48.58,73.54; Bone Pile 40.83,80.24):
- 91754 Rub Some Dirt In It (56; Untainted Soil no droppers — note)
- 91755 Leaves to Ligatures (56; Verdant Leaves in-zone)
- 91770 Bark Bite (56, pres 91754+91755; Fraxinus visit flagged as kill
  xnull — treated as a visit, Anachronos-pattern, B9)
- 92959 The Dying Ancients (56, pre 91770; Fraxinus, no objectives)
- 95766 Fine Feathered Friend (56, pre 91770; Fraxinus to Crow)
- 91883 Spear of the Skylord (59; Omnuron's Spear in-zone 2 droppers)
- 91923 Celastrus the Bitter (57; Broken Frond in-zone)
- 95320 A Curious Question (57; Crow to Felflick)
- 95318 Taste of Ash (57, pre 95320; Ashen Acolytes in-zone)
- 95319 Crystalline Collection (57, pre 95318; both crystals no droppers —
  note)
- 95378 The Hydra's Head (58, pre 95319; three Bones items in-zone)
- 95379 A Revenge So Sweet (58, pre 95319; Brashann in-zone)
- 96435 A Fitting End (58, pre 95378; turn-in Bone Pile object)
- 96255 Amalgamated Marrow (58, pre 96435; accept Bone Pile, slime kill)
- 96322 A Revenge Now Bitter (58, pre 96255; Felflick to Crow)
- 95317 Notation, Notation, Notation (57; Experimentation Notes in-zone)
- 95380 A Prolific Source (57, pre 95317; Fel-Slime Ooze in-zone 2 droppers)
- 96262 Prickly Pinecones (57, pre 95317; Pinecones no droppers — note)
- 95316 The Experimental Method (57, pres 95380+96262; Crow)
- 91881 The Western Post (57/54, Alliance, pre 95316; Crow to Sefira)
- 96930 The Capricious Corvid (58, pre 93773; Ketharas to Crow)
- 96931 Heading Up the Mountain (58, pre 96930; Crow to Jereman)
- 96321 The Dying God (58; Velician 36.69,78.25 to Crow)
- 96131 An Oldstone But An Old Friend (58, pre 96321; Crow to Ketharas; next 92612)
- 92612 Aid from Moonglade (58, pre 96131; Ketharas; turn-in Dendrite Starblaze in Moonglade - chain ends outside)

Ketharas hub (Ketharas 73.34,81.88) and the summit chain:
- 95568 Seeds for a New Season (56; Untainted Seed — 1 dropper with no
  spawns anywhere — note)
- 95569 Hope for Hatchlings (56; Owl Eggs no droppers — note)
- 93747 Violence Into Verdure (56, pre 95568)
- 94479 One Person's Trash (56; accept Loose Cog object 75.28,77.38)
- 96796 Woods Workshop (56, pre 94479; Ketharas to Kaylaena)
- 93759 The Bounty of Nature (56, pres 94479+95568+95569; Venison in-zone,
  Dart Tubers no droppers — note)
- 95611 Rites of Respect (56, pre 93759, next 90487)
- 90487 Ancient Allies (56, pres 93747+95611; turn-in Fraxinus)
- 96833 Venom Maws (56/54, Alliance; Quintus to Ketharas)
- 92171 Taking to New Heights (58, pre 93773-Moonglade-mini; Ketharas to
  Omnuron)
- 92500 A Bit of the Sky (58, pre 92171; Jewel no droppers — note; turn-in
  Ketharas)
- 90647 The Staff of the Mountain (57, pres 92317+92335+92500; Ketharas to
  Tiala)
- 92169 Paying Back the Pact (59, pre 90647; Tiala)
- 92833 Ve'han's Fall (60, pre 92169; Ve'han in-zone)
- 93848 Work Well Done (60, pre 92833; Tiala to Ketharas)
- 99670 Return to Jereman (60; Tiala to Jereman)

Tiala/Thisalee northeast (Tiala 68.85,50.6; Thisalee 68.99,49.99; Marn
68.3,46.71; Fayran 68.71,46.8; Rhylin 70.66,51.25; Toron 68.88,48.35;
Sebelia 70.87,51.55; Renalard 60.04,49.35; Maerion 63.28,25.85; Yashiro
49.33,32.63):
- 93127 Summit Sentries (60; Tiala, no objectives)
- 93407 A Thorn in the Paw (60; Thorn Seed no droppers — note, next 93547)
- 93547 A Thorny Solution (60, pre 93407; Tiala)
- 93584 Cult Closure (60; Cultists+Adepts in-zone, next 96303)
- 96303 Memory Mist (60, pre 93584; Thisalee)
- 93521 Challenger of the Gods (60; accept Bookshelf object 76.92,35.36,
  turn-in Tiala)
- 92017 Cleansing Winds (59; Feathers + Chimaera Hair in-zone)
- 92016 Rootwork (60, pre 92017; Nordrassil roots event in-zone 74.23,36.58)
- 96302 Arch Absolution (60, pre 92017; Marn)
- 96301 Power Wash (60; Vacant Heart no droppers — note; Well of Eternity
  event in-zone 73.64,39.24)
- 93444 Bait the Beast (60; Fayran, no objectives)
- 93422 Blackthorne Blackout (60; Couriers + Intelligence in-zone)
- 95793 Stemming the Demon Tide (59; Felguard Sentinels in-zone; turn-in to
  Witherbeard AND Elaena — both lines ride, B10)
- 96003 Drawing Down the Malevolent (60, pre 92960; Bethra'zel + Mazzogore
  in-zone)
- 96025 As the Crow Flies (59, pre 96003; Elaena to Thisalee)
- 92960 Siphoned Ephemeral Essence (59; Essence in-zone)
- 92335 Ashes of the Legion Ascent (59, pre 96964; Azgalor's Ashes — raid
  boss, no placed spawn — note-only naming; turn-in Ketharas)
- 92317 Stolen Life (58, pre 96939; Drop of Stolen Life in-zone 4 droppers;
  Marrosis to Ketharas)
- 96964 A Clever Creature (59, pre 96931; Jereman to Renalard)
- 96971 To Outfox a Demon (59, pre 96964; Abandoned Supplies no droppers —
  note)
- 97009 Maerion's Misery (59; Felhound Spikes in-zone)
- 97010 Blind Vengeance (59, pre 97009; Maerion)
- 96959 Blademaster's Bonfires (59; Yashiro, no objectives)
- 96983 Yashiro's Windwalk (60, pre 96959; Yashiro)
- 92533 Twisted Tools (60; Kris + Staff in-zone 2 droppers)
- 93197 Mending Communications (58; Sebelia; turn-in Innkeeper Vizzie in
  Winterspring — expedition leg, R1)
- 96991 Trail Assist (59, pre 96979; Galvinquam to Marn)

Veterans / remembrance (Veteran 20.49,60.08 + 8.8,46.48; scabbard 8.73,46.45;
anchor/carving; Battle Cache 29,52.8; Veteran 27.5,50.9):
- 92100 Anywhere But Here (58; Veteran to Scabbard object)
- 96550 Battle Recall (58, pre 92100; Scabbard to Veteran)
- 92101 Lifted by Legacy (58/54, pre 96550; Tobin's spot event in Thousand
  Needles 31.89,24.04 + turn-in to Carving object on 1441 — expedition, R1)
- 93510 Wake Memories (58/54, pre 96550; Lake Everstill event in Redridge
  30.19,57.51 + turn-in to Anchor object on 1433 — expedition, R1)
- 93567 Ends Meet (58; Veteran, no objectives)
- 96558 Soldier's Solace (60; Veteran to Battle Cache object)

Demon front (Johun 43.91,37.81; Kaylaena 60.1,61.18; Witherbeard
43.77,32.09; Elaena 43.77,32.24; Galvinquam 32.89,54.44; Phoebe 54.48,63.91;
Lisbael 42.07,52.05; Skylord 54.31,63.95):
- 92015 Area Denial Skunks (56/54, Alliance; Johun)
- 92014 Fox Hole (57/54, Alliance, pre 92015; Fox Tails in-zone 1452+2482)
- 96992 Resupply (57/54, Alliance, pre 92014; Nails+Brackets no droppers —
  note)
- 92593 Avalanche of Corruption (59/54, Alliance, pre 96992; tower scout
  event in-zone 53.74,33.55)
- 96494 Gathering Storm (59/54, Alliance, pre 92593; summit entrance event
  in-zone 83.65,32.48)
- 96529 A Shaw Deal (59/54, Alliance, pre 96494; turn-in Master Mathias Shaw
  in Stormwind — expedition, R1)
- 92008 Premiere Parts (56; Kaylaena; turn-in Nami in Winterspring —
  expedition, R1; Winterspring's soft-pre lives here in reverse)
- 92011 Rubble Rummage (58, pre 92009-Winterspring-mini; three rubble items
  no droppers — note)
- 92328 Siegecraft (56, pre 92011; Kaylaena)
- 92329 Drum Up Trouble (60, pre 92328; Kaylaena)
- 92594 Kindling, Kinda (56; Tainted Shrubbery in-zone)
- 92147 Highfeather Helper (58; Pinfeathers in-zone 7 droppers)
- 96252 Tarnished Treasures (58; Bangles no droppers — note)
- 96296 Fetid Corruption (58; accept Corrupted Growth object, objective is
  the same object — interact complete at 48.55,56.4; turn-in Phoebe)
- 96145 Past Wing and Claw (58; Lisbael to Phoebe, no objectives)
- 96979 Sacred Refreshment (57; Galvinquam, no objectives)
- 96939 The Balance of Life and Death (58, pre 96931; Jereman to Marrosis)
- 96957 Bone Sweet Bone (58, pre 96939; Sun-Bleached Bones no droppers —
  note)
- 96978 Violent Venison (57, pre 96931; Jereman to Kala'th)
- 93925? No — OUT, see below.

## OUT ledger (14)

- Horde-only set-asides (13, for the Horde block): 91794 Flags of Our
  Forebears, 92446 Head Scratcher, 92592 Final Death, 92609 Feathers in
  Flight, 94782 The Western Post, 95026 Blight No More, 95248 To the Summit
  of Eternity, 96616 Herbs for the Bruised and Weary, 96622 A Rest Without
  Pain, 96830 Farsight Guided, 96998 Tribal Colors, 96999 Wrap Return, 97119
  Now We're Cooking.
- Broken/incomplete (1): 93925 Beads for Brerufa — level null and no
  objectives; unbandable and unlintable as written.
- Above-band: none. Repeatables: none. Seasonal/event: none (no record
  carries an event flag).
- Accept-outside ledger notes (not candidates): 92009 Crate Expectations
  (Winterspring, Nami — soft-pre mini for 92011), 93773 The Pact (Moonglade,
  Dendrite — soft-pre mini for 92171/96930), 96209 The Ancient, Orokai
  (Moonglade — 92612's chain ends outside).

## BORDERLINE

- B1 (minnull): 90+ records carry minLevel null. Treated as no-minimum, not
  as zero: the band derives from recorded minLevels (floor 54) and the top
  quest level (60). Every minnull quest's own level (55-60) fits the zone;
  none is above-band per the rule. If Butler's data build ever fills these
  in, the band recomputes — until then this is the honest reading.
- B2 (neutral quests at shared posts): Zet'gan (90854), Sefira/ Kaylaena/
  Daythor/Hnaz and the AH-flagged hub NPCs serve both factions' chains, but
  every giver in the IN set is faction null/A/AH — the full sweep found zero
  H-flagged givers — so quest races govern and 90854 (races=null) is
  contracted. Horde-flagged variants stay out by their own races field.
- B3 (93925 OUT): null level breaks banding, lint and playtest alike; a
  talk quest with no data to hang a step on. Logged for Butler; contracts if
  the data ever fills it in.
- B4 (accept-only notes): 91696 and 96077 have no turn-in anywhere in the
  data — contracted with honest notes, never invented turn-ins (Ironforge
  precedent).
- B5 (twins): Final Death, Western Post, Blight No More, Feathers in
  Flight, To the Summit of Eternity, Now We're Cooking split Alliance/Horde
  — Alliance sides IN, Horde sides set aside. Belle's Ring (94832/96077)
  are BOTH Alliance — both routed (twin precedent).
- B6 (sourceless objectives): 91754, 92011 x3, 92335 (raid boss, no spawn —
  note-only), 92500, 92702, 93407, 93759-tubers, 93825, 93831, 95568,
  95569, 96252, 96262, 96957, 96971, 96992 x2, 95319 x2, 96301-heart ride
  honest notes with no invented completes or places. 95769's Bolt of
  Runecloth is the Ashenvale-R5 shape (buy/craft/farm-outside bag note at
  turn-in).
- B7 (expeditions): TN (92101), Redridge (93510), Stormwind (96529),
  Winterspring (92008, 93197 turn-ins) ride grouped expedition legs with
  deliberate frame switches — R1 by design.
- B8 (soft-pre minis): 92009 (Winterspring accept; timed Hyjal delivery +
  turn-in ride the mini) and 93773 (Moonglade accept; mini carries the
  Ketharas turn-in only) each stand alone in dedicated steps.
- B9 (91770): its objective flags Fraxinus as kill xnull — the Anachronos
  shape (a visit miscoded as a kill). Treated as a visit complete at
  Fraxinus with no kill language.
- B10 (95793): two turn-in NPCs in the data (Witherbeard + Elaena, same
  spot) — both turnin lines ride.
- B11 (out-of-zone tails): 92101's turn-in object lives on 1441 and 93510's on
  1433 — those tails play out-of-zone; the accepts keep them Hyjal quests
  per the accept rule.
