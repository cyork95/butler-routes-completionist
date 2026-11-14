# Butler Routes - Completionist

Completionist (all-quests) routes for [Polestar](https://polestar.guide), the guide addon for **WoW Forever**: every quest in a zone, in a sensible order. The opposite of speed-leveling routes — follow one of these and nothing gets left behind.

Pack id `butler-routes-completionist`. Title "Butler Routes - Completionist". Author Butler Muse. License CC-BY-4.0.

Status: **in development (pack v0.4.0), not published yet**. The first release (v1.0.0) is planned when the starting-zone set is complete.

## Routes so far

| Guide | Zone | Level band | Faction |
|---|---|---|---|
| `zephras-isle.guide` | Zephras Isle (Skyborne start) | 1–10 | Alliance (Skyborne) |
| `elwynn-forest.guide` | Elwynn Forest (Human start) | 1–10 | Alliance |
| `westfall.guide` (core built, pilot pending) | Westfall (follow-on zone) | 9–18 | Alliance |
| `zephras-isle-rares.guide` (pilot companion) | Zephras Isle rares and treasures | 1–12 | Alliance (Skyborne) |
| `zephras-isle-recipes.guide` (pilot companion) | Zephras Isle recipe sources | 1–12 | Alliance (Skyborne) |

Each quest guide takes every quest on the zone's tracker list exactly once: 145 accepts / 145 turn-ins for Zephras Isle, 83 / 83 for Elwynn Forest, 43 / 43 for Westfall. Class quests for other classes are included and gated with `only`, so they never show for a character they are not for.

The two pilot companions run in their own Polestar tab beside the Zephras core route: the rares guide sweeps all 8 confirmed rares plus the fixed Dented Chest placements (every goal optional, so a rare that is not up never holds the route), and the recipes guide collects the 12 vendor-sold recipe sources on the isle, gated by profession.

## Planned scope

All starting zones, both factions:

- Zephras Isle (Alliance) ✓, Elwynn Forest ✓, Westfall (core ✓, pilot pending)
- Dun Morogh / Coldridge Valley, Teldrassil
- Durotar, Mulgore, Tirisfal Downs
- Zephras Isle (Horde)

## Install

Once published: find "Butler Routes - Completionist" on the [polestar.guide](https://polestar.guide) listing, or install it through the Polestar Client.

## Development

Guides are plain-text `.guide` files at the repo root, next to `pack.json`. Publishing is via the repo's Publish to Polestar workflow: pushing a tag `vX.Y.Z` that matches `version` in `pack.json` uploads the source; the site compiles the addon. (`docs/` holds the quest contracts, authoring notes, and lint reports.)

Authored by Butler Muse for Cody.
