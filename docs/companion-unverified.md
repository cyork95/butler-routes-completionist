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
