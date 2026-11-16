# Deadwind Pass companions inventory (pack butler-routes-completionist)

Source: local Forever game data (questie-forever npcs/objects/items/quests.json),
built with `--product wowf` + QuestieDB. Accept-zone key **1430**, core band
**60-60**, Alliance route. The core contract (1 quest, 94355) is untouched by
this inventory. Game data wins over community sources throughout.

## RARES - none in data

All 34 NPCs spawning on 1430 were scanned for the data's rare flag (rank 2 =
Rare Elite, rank 4 = Rare, per the Badlands calibration). Result: 33 carry no
rank at all; the single ranked NPC is 276246 Mistmantle Prowler at rank 1
(normal mob, 60, 1 pt 35.5,35.73) — not rare-flagged, not a quest target, just
a normal mob, so not companion content and not a lookalike case. **Zero
rare-flagged spawns exist on 1430 in the data.** The rares companion therefore
ships as a treasures-only guide, said plainly in its header note (Moonglade
precedent: ship honestly what exists, never pad). No tame lines ship anywhere
(no rares, no beast-drop evidence, no core beast-family kills — the core's one
quest kills nothing). Nothing to log beyond this paragraph.

## TREASURES - 3 fixed unique objects, no generic chests

No chest-type object spawns on 1430 at all, so there is no generic-chest loop
to ship. The three fixed uniques below each get a plain single-goto step
(EPL single-unique precedent: goto + note, no loop — a loop needs 2+ points).

| object | points (map 1430) | disposition |
|--------|-------------------|-------------|
| 181963 Charred Bone Fragment | 1: 45,78.96, spawns only here | SHIP single goto + note (contents unconfirmed in the data) |
| 457088 Advanced Swordplay | 1: 43,74.4, spawns only here | SHIP single goto + note (a fixed book; contents unconfirmed in the data) |
| 694054 Recipe: Raw Plated Armorfish | 1: 52.4,34.5, spawns only here | SHIP single goto + note (fixed recipe object; the recipe itself is routed as the Cooking source in the recipes companion) |

Excluded with reasons: campfires/bonfires/cauldrons/pews (~10 flavor objects) —
not containers, no loot; ~20 Karazhan doors/gates/portcullises + 2 warning
signs — functional architecture, no loot; Spirit Healer 6491 — service NPC.
Quest 9205 (Craftsman's Writ - Plated Armorfish, repeatable, zone field 1423,
turn-in at Light's Hope) was checked against this zone: its accept item 22623
is sourceless and it accepts nowhere in-zone, so it stays OUT of the Deadwind
contract on the accept rule (and on repeatability) — noted here so the
Plated Armorfish connection is on the record.

## RECIPES - 2 shipped (0 vendor, 2 narrow/sole-source drops)

| recipe | profession (prefix convention) | source | disposition |
|--------|-------------------------------|--------|-------------|
| 286153 Recipe: Plated Armorfish | Cooking | drop: object 694054 @52.4,34.5, sole dropper anywhere (rate null) | SHIP collect |
| 16246 Formula: Enchant Bracer - Superior Strength | Enchanting | drop: 7372 Deadwind Warlock @60.51,61.69 @0.9%, sole dropper anywhere | SHIP collect |

Profession gating follows the pack's prefix convention (Plans = Blacksmithing,
Formula = Enchanting, Recipe: food dish = Cooking), the same basis the
Burning Steppes recipes guide used. All other professions have no Deadwind
source — the guide says so in a note (Dun Morogh precedent).

Excluded with reasons: 65 in-zone-dropped recipes with 72-646 droppers each
(Elwynn rule — generic world drops, not zone content; narrowest held back:
11226 Formula: Enchant Gloves - Riding Skill at 76 droppers, 13518/14499 at
100+); 0 vendor recipes (nothing is sold by any in-zone vendor, so the
Alterac Horde-vendor check has nothing to act on); quest-reward recipes
(UNVERIFIABLE — quest records carry no reward data, class logged in
companion-unverified).
