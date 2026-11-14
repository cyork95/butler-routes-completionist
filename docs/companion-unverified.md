# Companion unverified (pack 0.10.0)

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
