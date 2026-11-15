# Companion unverified (pack 0.12.0)

Recipe and source candidates for Zephras Isle that could NOT be confirmed from the
local Forever game data, so they are NOT in the guides. Promote an entry into a
guide only with a game-data citation (item/vendor/drop record) or a named source.

## Quest-reward recipes: class unverifiable locally

- Quest records in the local build carry no reward data (quests.json has start/end/
  objectives but no rewards field), so no quest-reward recipe on Zephras can be
  confirmed or denied from the toolchain. The 12 shipped recipes are all
  vendor-sold. If a Zephras quest is later found to reward a recipe, add it as a
  `note`/`task` step at the relevant hub (the quest itself stays core-only).
- What was checked: all 145 core quests resolve through the contract script; the
  only profession-linked Zephras quests are the Camping 101 intro quests
  (97963-97973, 98284-98286, skill + skillLevel, no recipe evidence).

## Dropped recipes: verified empty, nothing held back

- Full scan of every recipe/pattern/plans/schematic/design/manual/formula item
  against all 315 Zephras Isle NPC drop tables, all Zephras objects, and both fixed
  Dented Chest placements: zero links. No dropped recipe is missing from the
  guide; the dropped-recipe class on Zephras is empty per current data.

## Stock class: unverifiable locally

- Local item/vendor records carry no limited-vs-unlimited stock flag, so no recipe
  is marked limited in the guide. Each vendor step notes that stock class is
  unconfirmed.

## Tameability and pet mechanics: brief-sourced, data-silent

- NPC records carry no family/tame flags, so tameable vs not (Fernfeather and
  Mystmane tameable, Snapbeak not; Slydris an opportunistic trophy tame) and pet
  details (Fernfeather: Bite, Dust Cloud; foxes not learning Growl yet) rest on
  the round brief and the core guide's own Thendal Village note, not on game
  data. Correct the guides if the game contradicts them.

## Respawn timers: unconfirmed everywhere

- No respawn data for any rare or chest exists in the local build. Every rare and
  chest step says the timer is unconfirmed. Add a number only with data or a
  named source.

---

# Elwynn Forest (pack 0.9.0)

Recipe and source candidates for Elwynn Forest that could NOT be confirmed from
the local Forever game data, so they are NOT in the guides. Same promotion rule
as above: game-data citation or a named source.

## Quest-reward recipes: class unverifiable locally

- Quest records in the local build carry no reward data, so no quest-reward
  recipe in Elwynn can be confirmed or denied from the toolchain. The 4 shipped
  recipes are all vendor-sold. If an Elwynn quest is later found to reward a
  recipe, add it as a `note`/`task` step at the relevant hub (the quest itself
  stays core-only).

## Dropped recipes: confirmed world drops, none shipped

- Full scan of every recipe/pattern/plans/schematic/design/manual/formula item
  against all 279 Elwynn-spawning NPC drops and all Elwynn object drops: every
  recipe that drops in Elwynn also drops from 1 to 571 NPCs elsewhere. All are
  generic multi-zone world drops, none Elwynn-sourced, so none shipped. Nearest
  misses, kept out for the same reason: Recipe: Minor Spellblasting Potion
  (item250976, Kobold Geomancer + 1 other zone) and Recipe: Minor Cleric's
  Elixir (item250366, Murloc Forager and Elder Finseer + 2 other zones).

## Stock class: unverifiable locally

- Same finding as Zephras: local item/vendor records carry no
  limited-vs-unlimited stock flag, so no Elwynn recipe is marked limited. Each
  vendor step notes that stock class is unconfirmed.

## Tameability: family-evidenced, no tame flags in data

- NPC records carry no family/tame flags. The four `only Hunter` tame lines rest
  on drop-table evidence (Elmpaw and Matriarch Bristlefur drop bear parts and the
  core guide's Helene note names both as tameable bears; Longsnout drops boar
  meat and tusks; Mother Fang drops spider limbs and ichor) — not on a data
  tame flag. Croaky and Elder Finseer drop murloc fins and are kill-only
  (murlocs are not hunter pets). Correct the guides if the game contradicts them.

## Respawn timers: unconfirmed everywhere

- Same finding as Zephras: no respawn data for any of the 24 Elwynn rares or any
  fixed container exists in the local build. Every step says the timer is
  unconfirmed.

---

# Westfall (pack 0.10.0)

Recipe and source candidates for Westfall that could NOT be confirmed from the
local Forever game data, so they are NOT in the guides. Same promotion rule as
above: game-data citation or a named source.

## Quest-reward recipes: class unverifiable locally

- Quest records in the local build carry no reward data, so no quest-reward
  recipe in Westfall can be confirmed or denied from the toolchain. The 10
  shipped recipes are 9 vendor-sold plus 1 exclusive mob drop. If a Westfall
  quest is later found to reward a recipe, add it as a `note`/`task` step at
  the relevant hub (the quest itself stays core-only).

## Dropped recipes: world drops, one exclusion argued

- Full scan of every recipe/pattern/plans/schematic/design/manual/formula item
  against all 179 Westfall-spawning NPC drops and all Westfall object drops:
  every Westfall-dropping recipe except two is a generic multi-zone world drop.
  Pattern: Red Woolen Bag (item5772) drops from the Westfall Defias Renegade
  Mage plus one mob elsewhere — a two-zone world drop, not Westfall content per
  the Elwynn rule, so not shipped. The one shipped drop is Schematic: Shafety
  Sheep (item264210), whose sole dropper anywhere is the Westfall Venture Co.
  Miner.

## Stock class: unverifiable locally

- Same finding as before: local item/vendor records carry no
  limited-vs-unlimited stock flag, so no Westfall recipe is marked limited.
  Each vendor step notes that stock class is unconfirmed.

## Tameability: no tame lines shipped

- NPC records carry no family/tame flags, and none of the 14 shipped Westfall
  rares is drop-evidenced as a tameable beast family (murloc, ghoul/undead,
  machine, elemental, humanoid). Every rare step is kill-only. If a Westfall
  rare is later confirmed tameable, add an `only Hunter` task line per the
  Elwynn pattern.

## Respawn timers: unconfirmed everywhere

- No respawn data for any of the 14 Westfall rares or any fixed container
  exists in the local build. Every step says the timer is unconfirmed.

---

# Dun Morogh (pack 0.11.0)

Recipe and source candidates for Dun Morogh that could NOT be confirmed from
the local Forever game data, so they are NOT in the guides. Same promotion rule
as above: game-data citation or a named source.

## Quest-reward recipes: class unverifiable locally

- Quest records in the local build carry no reward data, so no quest-reward
  recipe in Dun Morogh can be confirmed or denied from the toolchain. The 3
  shipped recipes are 2 vendor-sold plus 1 exclusive mob drop. If a Dun Morogh
  quest is later found to reward a recipe, add it as a `note`/`task` step at
  the relevant hub (the quest itself stays core-only).

## Dropped recipes: world drops, one exclusion argued

- Full scan of every recipe/pattern/plans/schematic/design/manual/formula item
  against all 272 Dun Morogh-spawning NPC drops and all Dun Morogh object
  drops: every Dun Morogh-dropping recipe except two is a generic multi-zone
  world drop. Recipe: Minor Mageblood Elixir (item250375) drops from the Dun
  Morogh Young Wendigo plus one mob elsewhere — a two-zone world drop, not Dun
  Morogh content per the Elwynn rule, so not shipped. The one shipped drop is
  Recipe: Peace Tea (item249879), whose sole dropper anywhere is the Dun Morogh
  Frostmane Seer. No Blacksmithing plan has any Dun Morogh source in the data.

## Stock class: unverifiable locally

- Same finding as before: local item/vendor records carry no
  limited-vs-unlimited stock flag, so no Dun Morogh recipe is marked limited.
  Each vendor step notes that stock class is unconfirmed.

## Tameability: one task line, drop-evidenced

- NPC records carry no family/tame flags. The single `only Hunter` tame line
  (Bjarn) rests on drop-table evidence — his drops are bear paws, teeth and
  meat. No other shipped Dun Morogh rare is drop-evidenced as a tameable beast
  family, so every other step is kill-only. If another Dun Morogh rare is later
  confirmed tameable, add an `only Hunter` task line per the Elwynn pattern.

## Respawn timers: unconfirmed everywhere

- No respawn data for any of the 11 Dun Morogh rares or any fixed container
  exists in the local build. Every step says the timer is unconfirmed.

---

# Loch Modan (pack 0.12.0)

Recipe and source candidates for Loch Modan that could NOT be confirmed from
the local Forever game data, so they are NOT in the guides. Same promotion rule
as above: game-data citation or a named source.

## Quest-reward recipes: class unverifiable locally

- Quest records in the local build carry no reward data, so no quest-reward
  recipe in Loch Modan can be confirmed or denied from the toolchain. The 10
  shipped recipes are all vendor-sold. If a Loch Modan quest is later found to
  reward a recipe, add it as a `note`/`task` step at the relevant hub (the
  quest itself stays core-only).

## Dropped recipes: all world drops, none shipped

- Full scan of every recipe/pattern/plans/schematic/design/manual/formula item
  against all 173 Loch Modan-spawning NPC drops and all Loch Modan object
  drops: every Loch Modan-dropping recipe also drops in 4+ other zones. All are
  generic multi-zone world drops, none Loch Modan content per the Elwynn rule,
  so none shipped — unlike Westfall (one exclusive drop) and Dun Morogh (one
  exclusive drop), Loch Modan has no exclusive-drop recipe. Professions with no
  Loch Modan source at all (Blacksmithing, Leatherworking, Engineering,
  Enchanting, First Aid, Fishing) are named as absent in the guide header.

## Stock class: unverifiable locally

- Same finding as before: local item/vendor records carry no
  limited-vs-unlimited stock flag, so no Loch Modan recipe is marked limited.
  Each vendor step notes that stock class is unconfirmed.

## Tameability: one task line, one ambiguity logged

- NPC records carry no family/tame flags. The single `only Hunter` tame line
  (Shanda the Spinner) rests on drop-table evidence — her drops are spider
  meat, venom sacs, venom and ichor. Lord Condar drops a buzzard beak and his
  Shaking Egg, which suggest a bird — but a harpy fits that evidence just as
  well, and harpies are not hunter pets, so his step is kill-only; add a task
  line only if the game confirms a tameable bird. Every other shipped Loch
  Modan rare is kill-only.

## Respawn timers: unconfirmed everywhere

- No respawn data for any of the 10 Loch Modan rares, the Carved Figurine, or
  any fixed container exists in the local build. Every step says the timer is
  unconfirmed.

## Teldrassil tameability: three task lines, rest kill-only (pack 0.13.0)

- NPC records carry no family/tame flags. The three `only Hunter` tame lines
  rest on drop evidence plus core-guide corroboration: Lady Sathrah (spider
  limbs, spinnerets), Nightscreech (owl bills, feathers, eggs, leg meat),
  Duskstalker (cat hide; Nightsabers are hunter-tameable and the core route's
  own taming chain tames a Nightsaber Stalker). Every other shipped Teldrassil
  rare is kill-only, including Mowgh (rune only) and Sylassa (no loot at all).
- No Condar call exists for Teldrassil: npc14268 Lord Condar spawns on Loch
  Modan (1432) only. His Loch Modan kill-only disposition stands as written.

## Teldrassil quest-reward recipes: class unverifiable locally

- Quest records carry no reward data, so no quest-reward recipe on Teldrassil
  can be confirmed or denied from the toolchain. The 6 shipped recipes are all
  vendor-sold. If a Teldrassil quest is later found to reward a recipe, add it
  as a `note`/`task` step at the relevant hub (the quest itself stays
  core-only).

## Teldrassil dropped recipes: all world drops, none shipped

- Full scan of every recipe/pattern item against all Teldrassil-spawning NPC
  drops: every Teldrassil-dropping recipe also drops elsewhere. All are generic
  multi-zone world drops, none Teldrassil content per the Elwynn rule, so none
  shipped — Teldrassil has no exclusive-drop recipe (no come-back-later drop
  either, unlike Westfall and Dun Morogh).

## Teldrassil stock class: unverifiable locally

- Local item/vendor records carry no limited-vs-unlimited stock flag, so no
  Teldrassil recipe is marked limited. Each vendor step notes that stock class
  is unconfirmed.

## Teldrassil respawn timers: unconfirmed everywhere

- No respawn data for any of the 19 Teldrassil rares or any fixed container
  exists in the local build. Every step says the timer is unconfirmed.

## Teldrassil `more` arrays and the Stashbox: excluded with reason

- Nightscreech (npc276101) carries 24 `pts` plus a 49-entry `more` array;
  Wrathvine (npc276099) carries 24 `pts` plus a 30-entry `more`. The toolchain
  reads `pts` and nothing reads `more`, so `pts` is authoritative and the
  `more` entries ship nowhere. If Butler rules `more` are real alternates, the
  loops grow.
- No Stashbox of any name (Sordac's included) has a Teldrassil-spawn record in
  the local build; the named stashboxes sit on maps 1429 and 1411. Nothing
  secret-stash-like loops in the guide.

## Darkshore tameability: four task lines, rest kill-only (pack 0.14.0)

- NPC records carry no family/tame flags, and unlike Teldrassil the Darkshore
  core guide has no taming chain to corroborate against. The four `only Hunter`
  tame lines rest on drop evidence plus the brief: Clutchmother (Strider Meat
  in her table), Shadowclaw (Small Furry Paw; brief asserts tameable),
  Ghost Saber (brief-mandated tame-on-sight; cat plus Haunch of Meat), Lunaclaw
  (Haunch of Meat; bear). Every other shipped Darkshore rare is kill-only.
- Paxnozz (210482) is OUT despite the Kackle-shaped 24-point named record: it
  drops nothing but two Season-of-Discovery runes shared with other NPCs — a
  rune source, not a rare. If the game confirms a true rare there, promote it.

## Darkshore Ghost Saber: what the data does and does not confirm

- Confirmed: npc3619 Ghost Saber (level 19) holds 3 Darkshore points; obj13359
  Cat Figurine holds 3 Ruins-of-Mathystra points and obj13873 holds 1; the
  saber drops item5332 Glowing Cat Figurine and nothing else exclusive. The
  figurine loop, the interact lines and the collect are all data.
- Not in the data: the summon-and-despawn mechanic itself. It is the brief's
  report and the step says so. If the game shows the figurines work
  differently (or the saber roams), the step gets rebuilt from that.

## Darkshore quest-reward recipes: class unverifiable locally

- Quest records carry no reward data, so no quest-reward recipe on Darkshore
  can be confirmed or denied from the toolchain. The 13 shipped recipes are
  all vendor-sold. If a Darkshore quest is later found to reward a recipe, add
  it as a `note`/`task` step at the relevant hub (the quest itself stays
  core-only).

## Darkshore dropped recipes: all world drops, none shipped

- The two candidate drop recipes are both generic: Recipe: Cooked Crab Claw
  (2698) drops from 117 NPCs and Feet of the Lynx (1121) from 384. Per the
  Elwynn rule both stay out, so no drop recipe made the guide.

## Darkshore stock class: unverifiable locally

- Local item/vendor records carry no limited-vs-unlimited stock flag, so no
  Darkshore recipe is marked limited. Each vendor step notes that stock class
  is unconfirmed.

## Darkshore respawn timers: unconfirmed everywhere

- No respawn data for any of the 18 Darkshore rares, the Ghost Saber
  figurines, or any fixed container exists in the local build. Every step says
  the timer is unconfirmed.

## Darkshore excluded objects and NPCs: logged with reason

- Xabraxxis' Demon Bag (obj177624): unlinked prop co-located with a shipped
  rare, no quest link, no loot data — left out rather than guessed.
- Narassin's Strongbox (obj676349) and Bough of Altek (obj411715): Tower of
  Althalaxx area props, chain-adjacent — not companion content.
- Sapphires of Aku'Mai (obj178184/178185/178186): Blackfathom dungeon-side —
  not zone content for an open-world sweep.
- Gnarled Harpoons (obj408802), Remnant (obj414646), Field Guide (obj612088):
  unidentified fixed props with no container nature and no quest link — the
  Verigan's Fist precedent.
- Moonkin Stone (obj177525): unconfirmable single object, no quest link.
- Skeletal Sea Turtle (obj176189): beached-series-adjacent; the core guide owns
  the beached series.
- Scrolls (obj409496): starts uncontracted quest 78124 (Nar'thalas Almanac,
  level 20) — quest-owned, not companion content.
- Strange Orb (obj409289): starts uncontracted druid-30 chain 78088 — above
  band and quest-owned.
- Crate of Elunite, Armor/Weapon/Food Crates, Barrel of Milk (obj86492, 3660,
  3661, 3662, 3705): Auberdine town and Tower-chain-adjacent props.
- Ruuzel (npc3943, level 22, single remote Mist's-edge point, zero exclusive
  loot): level alone never ships a step.
- Incubus (npc185317), Thamarian (npc12656), Una Ji'ro (npc11816): zero drops,
  no quest link — summon/prop or unconfirmable, never into the guide.
- Ghostpaw Runner (npc3823): spawns on Darkshore (2 pts), Ashenvale (24 pts)
  and map 1442 alongside Howler/Alpha — a cross-zone family, not a rare.
- Jai'vhanel pair: contracted quest subject (98025) with an ambient 24-point
  spawn — core-owned. Note: the quest's item objective 28103 does not exist in
  items.json; that is the core route's data gap, reported not fixed.


## City recipes: quest-reward candidates (pack 0.18.0)

- The same limitation covers all three capitals: quest records carry no reward data, so no city quest can be confirmed or denied as a recipe source from the toolchain. Nothing shippable was found: every recipe in the three city guides is vendor-confirmed, and no city quest is cited anywhere as a recipe source. Promote a candidate only with a game-data citation or a named source.

## Hillsbrad tame lines: drop evidence without corroboration (pack 0.29.0)

- Creepthess (npc14279, spider: drops Crisp Spider Meat item1081 + Spider's Silk item3182) and Big Samras (npc14280, bear: drops Big Bear Meat item3730 + Durable Bearhide Pauldrons item282717) have drop evidence for a tameable beast type, but the Hillsbrad core guide carries no tame lines and no references to any Hillsbrad rare, so the corroboration half of the tame rule is unmet. No only Hunter task ships for either; both stay kill-or-skip. Promote only with core-guide corroboration or a named source.


## Redridge tame lines: nothing to corroborate (pack 0.30.0)

- All 8 shipped Redridge rares have zero loot records in the data, so no drop-evidence beast typing exists for any of them, and the only "Tame" hits in the Redridge core guide are the NPC name Tamelyn. No only-Hunter task ships; all eight steps are kill-or-skip. Promote only with drop evidence plus core-guide corroboration or a named source.


## Arathi tame lines: nothing to corroborate (pack 0.32.0)

- All 11 Arathi rares have zero loot records in the data, so no drop-evidence beast typing exists for any of them, and the Arathi core guide carries no tame lines or references to any Arathi rare. No only-Hunter task ships; all nine steps are kill-or-skip. Promote only with drop evidence plus core-guide corroboration or a named source.


## Ashenvale lookalikes and tame lines (pack 0.33.0)

- Samophlange Manual Cover (item11147, sole dropper Boss Copperplug npc9336) and Samophlange Manual Page (item11148, droppers Venture Co. Enforcer npc3283 and Overseer npc3286) matched the Manual regex but carry `questItem:true` — they are quest items, not recipes. No quest in the data references either item, so their chain is unverifiable; neither ships anywhere. Promote only with a quest record or a named source.
- Formula: Enchant Gloves - Herbalism (item11151): 5 droppers across three zone maps (Ashenvale/Stonetalon ancients) — a multi-zone world drop, not Ashenvale content under the Elwynn rule. Not shipped. Promote only with data showing an Ashenvale-exclusive source.
- All 13 Ashenvale rare-flagged NPCs have zero loot records in the data, so no drop-evidence beast typing exists for any of them (npc records carry no classification flag), and the Ashenvale core guide carries no tame lines or references to any Ashenvale rare. No only-Hunter task ships; all twelve steps are kill-or-skip. Promote only with drop evidence plus core-guide corroboration or a named source.

## Alterac Horde-vendor exclusives, world drops and tame lines (pack 0.35.0)

- Pattern: Thick Murloc Armor (item5788) and Recipe: Shadow Protection Potion (item6054): in-zone only Christoph Jeffcoat (npc2393, faction Horde); Pattern: Blue Overalls (item6274) and Pattern: Dark Silk Shirt (item6401): in-zone only Mallen Swain (npc2394, faction Horde); Recipe: Bristle Whisker Catfish (item6330): in-zone only Derak Nightfall (npc2397, faction Horde). All three vendors sit deep on the Horde side (60-62, 80-83) and the data cannot confirm Alliance buyability — none shipped. Promote only with live verification that Alliance characters can buy from them.
- Pattern: Black Silk Pack (item5775): 3 droppers across 4 map-zones (Alterac Spy, Hillsbrad Shadowy Assassin, Theramore Infiltrator) — multi-zone world drop, not Alterac content (Elwynn rule). Not shipped.
- Formula: Enchant Cloak - Lesser Agility (item11206): 3 droppers, 2 of them Wastewander mobs in Tanaris — the Tanaris farm is the known source; the single Alterac Assassin is incidental, not zone content. Not shipped.
- All 8 Alterac rare-flagged NPCs have zero loot records in the data, so no drop-evidence beast typing exists for any of them, and neither core guide (Alterac 0 tame hits, Hillsbrad no tame lines or rare-name references) corroborates any. No only-Hunter task ships; all seven steps are kill-or-skip. Promote only with drop evidence plus core-guide corroboration or a named source.

## Stonetalon Horde-vendor exclusives, world drops and tame lines (pack 0.36.0)

- Recipe: Fire Protection Potion (item6055): in-zone only Jeeda (npc4083, faction Horde; the Alliance source Nandar Branson is in Hillsbrad, another round's business). Formula: Enchant Cloak - Minor Agility (item11039) and Formula: Enchant Bracer - Lesser Strength (item11101): in-zone only Kulwia (npc12043, faction Horde; the Alliance source Dalria is in Ashenvale, already shipped in that round's companions). None shipped — Alterac precedent. Promote only with live verification that Alliance characters can buy from these vendors.
- Formula: Enchant Gloves - Herbalism (item11151): 5 droppers across three zone maps (Stonetalon + Ashenvale ancients, including rare-flagged Vengeful Ancient npc4030) — multi-zone world drop, not zone content; the rare ships as a pure kill. Consistent with the Ashenvale round's exclusion. Not shipped.
- All 9 Stonetalon rare-flagged NPCs have zero loot records in the data, so no drop-evidence beast typing exists for any of them, and the core guide carries no tame lines (its only pridewing mention is a contracted supply kill, not corroboration). No only-Hunter task ships; all nine steps are kill-or-skip. Promote only with drop evidence plus core-guide corroboration or a named source.

## Dustwallow tame lines (pack 0.39.0)

- The 10 shipped Dustwallow rares DO have loot records, and some drops suggest beast typing (Darkmist Widow npc4380: Thick Spider's Silk item4337, Dripping Spider Mandible item4585), but npc records carry no classification flag and the Dustwallow core guide carries no tame lines and no references to any Dustwallow rare. Drop evidence alone is not the bar (Stonetalon/Teldrassil precedent needs core-guide corroboration too). No only-Hunter task ships; all ten steps are kill-or-collect. Promote only with core-guide corroboration or a named source.

## Duskwood tame lines and lookalikes (pack 0.40.0)

- The 6 shipped Duskwood rares DO have loot records, and two drops suggest beast typing (Lupos npc521: Lean Wolf Flank item1015, Sharp Claw item5635; Naraxis npc574: Fist-sized Spinneret item878, Gooey Spider Leg item2251), but npc records carry no classification flag and the Duskwood core guide (93-contract) carries no tame lines and no references to any Duskwood rare. Drop evidence alone is not the bar (Stonetalon/Teldrassil/Dustwallow precedent needs core-guide corroboration too). No only-Hunter task ships; all six steps are kill-or-collect. Promote only with core-guide corroboration or a named source.
- Classic Duskwood names without the rare flag in the data (Mor'Ladim npc522 L35, Stitches npc412 L35, Stalvan Mistmantle npc315 L32, Eliza npc314 L31, Morbent Fel npc1200 L32; all roles=undefined) are quest-target lookalikes, not companion content: the flag is the rule and the data wins over community memory. Promote only with data showing the flag.

## Feralas tame lines, above-band loot, and excluded recipes (pack 0.42.0)

- Several of the 9 shipped Feralas rares read as beasts by name and shape in the data (Old Grizzlegut the bear, Bloodroar the Stalker, Antilus the Soarer, Arash-ethis the wind serpent, Snarler, Gnarl Leafbrother the treant, Qirot the silithid), but npc records carry no tameability flag and the Feralas core guide (57-contract) carries no tame lines and no references to any Feralas rare. Name-and-shape alone is not the bar (Stonetalon/Teldrassil/Dustwallow/Duskwood precedent needs drop evidence plus core-guide corroboration). No only-Hunter task ships; all nine steps are kill-or-collect. Promote only with core-guide corroboration or a named source.
- Black Lotus (item13468) is the sole drop of Mushgog (npc11447 L60, Dire Maul area) - a real in-zone source that cannot ship because its only source is an above-band excluded rare. Logged, never invented as a herb node.
- Pattern: Bottomless Bag (item14510, single in-zone dropper Dreamroarer L62 world boss, 5 zones) and Plans: Sageblade (item22389, in-zone droppers the 4 Emerald Dragons L63, 5 zones) are above-band/out-of-reach drops, not zone content for a 38-50 guide. Logged, never shipped.
