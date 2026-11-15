# Blasted Lands companions inventory (game data, accept-zone key 1419)

Source: local Forever game data (questie-forever NPC/object/item dumps).
Rank semantics calibrated in earlier rounds: rank 4 = Rare, rank 2 = Rare
Elite (no rank-2 NPC spawns in 1419 — all 10 flagged rares are rank 4 with
explicit roles ["rare"]). Loot "sole dropper" means the item's drops.npc
lists only this NPC and no object source. Rates shown where the data gives
a number; a null rate does not disqualify a sole drop (Feralas/Tanaris
calibration). Tameability has NO data flag anywhere: a tame line ships only
on drop evidence PLUS core-guide corroboration, else it is logged in
docs/companion-unverified.md.

## RARES — 10 flagged (all rank 4), 5 shipped, 5 excluded

| NPC | Lvl | Point(s) | Sole-drop signature | Guide step |
|-----|-----|----------|---------------------|------------|
| 8296 Mojo the Twisted | 48 | 4 pts, north-west (41-45, 12-16) | 282014 Twisted Shadow Staff | loop + collect + sphere note |
| 8297 Magronos the Unyielding | 56 | 1 pt (47.2,47.14) | 282026 Unyielding Battle Signet | single + collect + come-back note |
| 8298 Akubar the Seer | 54 | 8 pts, center-south (45-61, 44-54) | 282019 Braided Seer Stones | loop + collect + come-back note |
| 8302 Deatheye | 49 | 13 pts, west (43-50, 18-30) | 282020 Stonegaze Wand | loop + collect + brain note |
| 14446 Fingat | 43 | 1 pt (71.4,15) | none (generics only, no quest items) | single + kill note, NO tame line |

Notes:
- No core-contracted quest references any shipped rare structurally
  (start/end/objectives/sourceItem scanned over the 21-contract quests).
- The shipped rares also drop core quest items (Mojo 8244, Magronos
  8244/10593, Deatheye 8244/8394/10593) — those items have dozens of
  in-zone droppers each, so the rares are not anyone's only source; the
  notes name the overlap honestly and point at the core guide (Darkshore
  Baron Marinous pattern), and the core hunt circuit already routes them.
- Above-band handling (band 40-50, Westfall/Hillsbrad/Duskwood
  precedents — excluded, or shipped with an honest come-back-later note
  when a sole-drop signature argues for it): Magronos (+6, sole signet)
  and Akubar (+4, sole stones) SHIP with come-back notes (Duskwood Nefaru
  +6 pattern — reachable signatures, not group content; both are rank 4,
  not elites). Spiteflayer (52, +2), Ravage (51, +1), Clack the Reaver
  (53, +3), Dreadscorn (57, +7) are EXCLUDED — no sole drops, so nothing
  argues for them (Hillsbrad/Arathi +1 precedent for Ravage; the higher
  three fail harder). Spiteflayer/Clack/Ravage additionally overlap core
  objective mobs, cited as the secondary reason.
- Grunter (npc8303, lvl 50, 18 pts, no sole drops, drops 8392 Blasted Boar
  Lung) is EXCLUDED although in-band: with no loot of its own its only
  distinctive significance is the core quest item — a quest-target
  lookalike without loot of its own (Dun Morogh rule, stated plainly).
  The lungs stay routed in the core hunt circuit.
- Fingat keeps the Shadowforge Commander pattern: flagged rare, generic
  loot only, no quest items at all in its table, no quest links — a pure
  kill-note rare.
- Tameability: no tame lines ship. The core guide carries zero `only
  Hunter` lines, so the corroboration half is unmet for everything
  regardless; and the shared tables show no meat/fang-family evidence
  (only generic leather gear). Logged in docs/companion-unverified.md.
- Respawn timers: unconfirmed anywhere in the data; none stated.
- All 10 rares are faction null (neutral spawns, no Horde lock).

## TREASURES

- Generic "Solid Chest": object 4149 (3 fixed pts, far east
  71-74,13-15) and object 153451 (5 fixed pts: 42.5,14.33 / 44.38,12.01 /
  62.41,34.26 / 65.46,33.37 / 66.83,29.61). ONE loop step over all 8
  fixed points, said plainly as generic chests. Loot is the classic
  shared chest table (greens, food, potions, gems, and ultra-wide world
  recipes that also drop from hundreds of mobs — no chest-exclusive
  claims). No quest takes either chest as an object (the 1618/1619-era
  item-ID collisions are items, not these objects).
- Excluded with reason (no loot in the data, not containers): 181302
  "Camp Crate" (2 pts), 181191-181194 "Skullpile 01-04" (24/23/21/24
  pts + more — decor piles), 153359/153360 "Rune of Return" (same point
  47.5,27.7 — decor/event), 3772 "Potbelly Stove" (2 pts — stove),
  164618 "Mailbox" (mail, not treasure). The other ~150 objects are herbs,
  veins, braziers, banners, altars and Dark Portal architecture. No
  footlockers, clams,-jars or caches exist in the zone data — the Solid
  Chest loop is the whole treasure yield, stated plainly in the guide.

## RECIPES — 2 shipped (vendor 1 + drop 1)

- Alchemy, Nina Lightbrew (66.87,18.24, Nethergarde, Alchemy Supplies,
  faction A — Alliance-safe; also sold by 1 vendor elsewhere): 9300
  Recipe: Elixir of Demonslaying. No stock flag in the data; unmarked
  (unverified log notes the stock class).
- Leatherworking, in-zone mob drop: 15727 Pattern: Heavy Scorpid Vest <-
  5981 Portal Seeker + 6005 Shadowsworn Thug (2 droppers, 1 zone — both
  spawn only in 1419: genuinely zone content, Hillsbrad-exclusive-drop
  precedent). No quest takes it.
- Excluded with reason (all multi-hundred-dropper world drops under the
  Elwynn rule — full scan: 100+ lines, 76–646 droppers across 5–32 zones
  each): everything else, including 12716 Helm of the Great Chief (9
  droppers/2 zones — a Lord Kazzak-table world drop, not zone content
  despite the in-zone boss), 12717 Lionheart Helm (18/8), 14509 Mooncloth
  Circlet (22/7), 14510 Bottomless Bag (12/5), 14511 Gloves of Spell
  Mastery (17/7), 223163 Scroll of Spatial Mending (4/9 — Tanaris-217271
  territory), 228317 Incandescent Mooncloth Circlet (19/4), and every
  Mithril/Thorium/Radiant/Thorium-era plan, frostweave/runecloth pattern,
  transmute/flask recipe and enchant formula on the list. Kazzak himself
  is above-band endgame content either way.
- Quest-reward recipes: quest records carry no reward data — none shipped,
  class-logged in companion-unverified.
- Trainer-taught staples excluded (Polestar's own profession guides).

Professions with NO Blasted Lands source (stated plainly in the guide, Dun
Morogh Blacksmithing precedent): Blacksmithing, Cooking, Enchanting,
Engineering, First Aid, Fishing, Tailoring.
