# Swamp of Sorrows (Horde) companions inventory (pack 0.147.0)

Source: local Forever game data (questie-forever `quests.json`/`npcs.json`/`items.json`/`objects.json`, built with `--product wowf` + QuestieDB). Accept-zone key **1435**, working band **30–38** (the Horde core's contract band, `swamp-of-sorrows-horde`, 12 quests — not copied from the Alliance 30–38 by assertion but re-derived: same numbers, verified from the Horde contract file). Every point below is a `spawns["1435"]` entry in front of the author; nothing is taken from community sites. The Alliance inventory (`docs/swamp-of-sorrows-companions-inventory.md`) is the mirror and cross-check: the two inventories must never contradict each other on the same mob or object; genuine differences are flagged in `docs/companion-unverified.md`, never harmonized away.

## Rares (9 NPCs carry the data rare flag on key 1435 — same 9 as Alliance, verified point-for-point below)

| ID | Name | Lvl | Points (1435) | Loot of note | Disposition |
|----|------|-----|---------------|--------------|-------------|
| 1106 | Lost One Cook | 37 | 6 pts, Fallow Sanctuary (60.93, 24.28 / 61.82, 21.85 / 62.39, 20.9 / 62.5, 23.31 / 63.98, 22.8 / 65.23, 22.8) | **250186 Giant Scrambled Eggs, SOLE dropper anywhere in the data**; otherwise greens + generic 3832 recipe | SHIP kill + exclusive collect |
| 763 | Lost One Chieftain | 39 | 5 pts, Fallow Sanctuary (60.06, 20.31 / 60.54, 22.93 / 61.59, 22.78 / 61.96, 21.16 / 63.81, 20.85) | **282003 Lost Chieftain's Greatsword, SOLE dropper anywhere in the data**; otherwise greens + generic 3832 recipe | SHIP kill + exclusive collect, come-back-later note (+1 over band) |
| 14448 | Molt Thorn | 42 | 19 pts, west (25.83, 48.16 / 26.59, 38.46 / 27.88, 32.7 / 28.37, 52.47 / 28.4, 45.91 / 29.07, 42.35 / 30.52, 50.99 / 30.92, 36.63 / 32.65, 48.08 / 32.88, 44.53 / 33.57, 35.01 / 34.49, 38.84 / 35.57, 31.36 / 37.02, 44.41 / 37.28, 36.97 / 38.23, 39.75 / 39.71, 36.04 / 41.15, 31.64 / 43.27, 33.96) | No sole drop (herb-heavy table; 10301 White Bandit Mask is a 29-zone world drop). One of 5 in-zone droppers of 11205 (recipes guide carries it) | SHIP kill, come-back-later note |
| 14446 | Fingat | 43 | 1 pt (61.43, 83.72); also spawns Blasted Lands 1419 | Fish/clams/pearls, no sole drop | SHIP kill, come-back-later note + two-zone note |
| 14447 | Gilmorian | 43 | 1 pt (95.87, 64.39, far east shore) | Fish/clams/pearls, no sole drop | SHIP kill, come-back-later note |
| 14445 | Lord Captain Wyrmak | 45 | 1 pt (68.91, 38.91) | 282008 Wyrmak's Cuirass SOLE dropper; 5974 Guardian Cloak is a 29-zone world drop | EXCLUDED far above band; signature logged here |
| 1063 | Jade | 47 | 1 pt (70, 53.2) | Small Flame Sac / Ripped Wing Webbing / Fiery Gland / Wicked Claw, no sole drop | EXCLUDED far above band |
| 5399 | Veyzhak the Cannibal | 48 | 1 pt (78.8, 43.8) | Flask of Big Mojo (multi-zone generic), no sole drop | EXCLUDED far above band |
| 5400 | Zekkis | 49 | 1 pt (77.5, 39.4) | Green Dragonscale (multi-zone generic: Stonetalon/Azshara rounds note it), no sole drop | EXCLUDED far above band |

- All 9 are react-null (neutral to both factions) — the faction rule (Ashenvale Falthis / Stonetalon opposition) triggers for none; the shipped set is identical to the Alliance set by the data, not by copying (points re-read above).
- No rare is a giver, ender, or objective of any of the 12 contracted Horde quests (checked field by field over the contract; the Horde core guide never mentions any of the 9). The Dun Morogh exclusion does not fire; all 5 shipped rares are genuine companion content.
- Above-band handling, per band top 38: 763 (+1) ships with an honest come-back-later note (same as Alliance). 14448 (+4), 14446 (+5), 14447 (+5) ship with come-back-later notes — data shows their spawns, level is the only bar (same call as Alliance, stated per record). Wyrmak/Jade/Veyzhak/Zekkis (+7 to +11, all single-point, no sole signature except Wyrmak's unshippable cuirass) are EXCLUDED far above band; signatures logged, never shipped.
- Respawn: no timer data for any shipped rare exists in the local build; every rares step says the timer is unconfirmed.
- Tame lines: NONE ship. NPC records carry no family flag, and the Horde core guide carries zero tame corroboration (no `only Hunter` lines, no rare mentions at all — verified by grep). All 9 tame questions are logged in `docs/companion-unverified.md` (Duskwood precedent: the bar does not lower).

## Item-start hunts: none

The Horde core contract (12 quests) contains ZERO item-starts (explicit start-item scan in the dossier: start `{npc,object,item}` fields read for all 12; no non-empty `item` field). "There are therefore NO item-start hunts in this companions round" is stated after the scan, not assumed (Mulgore lesson held).

## Treasures

SHIPPED (fixed-spawn containers, every point from the data):
- Solid Chest 2857 (11 pts: 4.83, 31.68 / 11.68, 34.21 / 13.9, 56.02 / 13.96, 71.32 / 54.96, 29.79 / 60.07, 22.04 / 61.17, 23.87 / 62.01, 21.05 / 62.6, 23.32 / 64.18, 22.37 / 65.76, 18.36; also spawns 7 other zones) and Solid Chest 4149 (13 pts: 56.85, 61.13 / 61.4, 81.21 / 63.41, 87.78 / 64.21, 87.23 / 82.8, 93.73 / 86.54, 84.08 / 89.1, 78.39 / 91.14, 27.25 / 92.2, 68.15 / 94.51, 52.7 / 94.91, 50.75 / 94.93, 60.81 / 94.98, 45.34; also spawns 9 other zones): generic multi-zone chests, one loop step over all 24 points, said plainly. Both also drop generic world-drop recipes (dozens each) — noted as not zone content.
- Scattered Crate 28604 (17 pts, Swamp-only: 4.64, 31.2 / 9.7, 29.84 / 12.8, 34.43 / 14.19, 38.22 / 29.7, 50.11 / 29.91, 38.31 / 33.64, 46.01 / 37.09, 34.15 / 37.09, 36.16 / 43.29, 33.26 / 45.82, 35.58 / 54.39, 30.59 / 56.92, 24.7 / 60.03, 21.73 / 62.27, 22.5 / 64.09, 23.35 / 64.89, 20.44): Swamp-exclusive plain container, same loop step as the Solid Chests.
- Mossy Footlocker 179493 (6 Swamp pts: 65.39, 51.74 / 66.26, 58.37 / 69.68, 61.17 / 71.7, 48.23 / 71.81, 61.59 / 74.2, 58.51; also Desolace): 6 Swamp points join the fixed-containers loop, said plainly.
- Atal'ai Artifact 30854/30855/30856: three object IDs sharing the SAME 24 fixed points around the Sunken Temple approach (61.52, 57.88 / 62.41, 52.9 / 64.39, 49.44 / 65.33, 57.13 / 65.45, 43.37 / 66.45, 54.05 / 67.3, 45.79 / 67.31, 62.91 / 67.77, 49.91 / 69.66, 59.37 / 69.8, 40.84 / 70.61, 66.01 / 71.07, 46.59 / 72.43, 60.76 / 72.53, 53.11 / 73.91, 42.31 / 74.31, 47.92 / 74.48, 58.11 / 74.97, 51 / 75.75, 44.7 / 76.25, 63.5 / 76.31, 53.62 / 78.24, 48.49 / 78.77, 57.17). No quest record references any of the three IDs. One loop step over the 24 shared points with all three interact lines and a note explaining the triple-ID shared points. (Delta vs Alliance flagged below: the Alliance inventory claims 67 distinct points + 43 "more"; this data build renders 24 per ID, all shared.)
- Atal'ai Tablet 37099 (15 pts, Swamp-only: 70.55, 44.53 / 71, 46.89 / 72.09, 45.22 / 72.83, 47.65 / 74.7, 43.84 / 74.77, 46.71 / 75.31, 49.51 / 75.68, 44.95 / 75.81, 49.4 / 75.85, 48.3 / 76.07, 47.44 / 76.17, 43.79 / 76.61, 49.05 / 76.71, 51.31 / 78.27, 49.54). Own loop step; no quest link.
- Conspicuous Cache 423926 (42.7, 30.9) + 428228 (42.6, 30.7): two IDs, one spot. Own single-goto note step; no quest takes anything from either in the data.
- Tarantula Cage 181624 (62.9, 23.7) + Jaguar-Crocolisk Cage 181625 (60.49, 22.17 / 65.42, 22.74): Fallow Sanctuary cages. Own step with gotos; no quest link in the data, purpose unconfirmed per data.
- Caravan Chest 28024 (64.46, 18.3): single point, holds 6170 Wizards' Reagents for Alliance-only quest 1421 The Lost Caravan (uncontracted; see below) — for Horde it is a dead-end container with generic value: shipped as a unique with that honest note (genuine faction delta vs the Alliance core-routing, argued below). No other quest takes 6170 in the data.

EXCLUDED quest-owned containers (core guide owns them, never duplicated):
- 32569 Galen's Strongbox (turnin 1393) + 37118 Galen's Cage (1393 escort ground), 22550 Draenethyst Crystals (complete 1389 x3), 24798 Sundried Driftwood (complete 1398 x4), 2553 Soggy Scroll (turnin 624 / accept 625) — all four quests' lines ride the main (Alliance) guide, which Horde players complete through the ungated shared lines; the objects stay there.
- 141980 Spectral Lockbox (end-object of 2701 Heroes of Old — OUT of contract as above-band; same ruling both factions).
- The 93568 (Stitches the Outcast) and 93574 (Corpsefeeder) objectives ship as optional collects in the rares guide (noted there): the census deferred both records to companions explicitly; their quests stay uncontracted.
- NOT treasure by class (stated, not listed per object): all mining veins, herbs (incl. Blindweed), the Misty Reed fishing location; campfires/bonfires/embers; books/grave/sack/forge/anvils/cauldron/meeting stone/mailbox/lore books; seasonal decor.
- The Garrett/Krom family chests of the Badlands round do not recur here; no family chests spawn on 1435.

## Recipes (full item-table scan: 144 recipe items touch the Swamp)

SHIPPED (12: 2 vendor + 10 drops):
- Pattern: Green Dragonscale Breastplate (15726) + Pattern: Living Green Dragonscale Breastplate (228309), Leatherworking — vendor: Masat T'andr (11874, neutral AH-faction, 1435 point 26.46, 31.47; SOLE vendor anywhere in the data for both). Pin every buy `npc 11874`.
- Recipe: Giant Scrambled Eggs (250186), Cooking — drop: Lost One Cook 1106 (SOLE dropper anywhere; in-band 37, 6 pts above). No quest takes it.
- Plans: Mithril Stiletto (251463), Blacksmithing — drop: Lost One Hunter 759 (SOLE dropper; in-band 36, Swamp-only mob, 12 pts). No quest takes it.
- Manual: Potent Anti-Venom (255728), First Aid — drop: Lost One Muckdweller 760 (SOLE dropper; in-band 36, Swamp-only mob, 13 pts). No quest takes it.
- Formula: Enchant Gloves - Advanced Herbalism (11205), Enchanting — drop: 5 droppers, ALL Swamp-only (Swampwalker 764 lvl 38, Elder 765 lvl 39, Tangled Horror 766 lvl 40, Mire Lord 1081 lvl 42, Molt Thorn 14448 lvl 42); step placed at the in-band Swampwalker 764 (11 pts), note names the other four. No quest takes it.
- Recipe: Sunny Tea (249883), Cooking — drop: Marsh Oracle 752 (SOLE dropper; lvl 44, above band, spawns Swamp + Blasted Lands); come-back-later note + two-zone note. 13 Swamp pts. No quest takes it.
- Plans: Mithril Scale Bracers (7995), Blacksmithing — vendor: Gharash (8176, Horde faction, 1435 point 45.46, 51.41; also Alliance Harggan 8161 in Hillsbrad/Alterac). Pin every buy `npc 8176`.
- Recipe: Elixir of Demonslaying (9300), Alchemy? — vendor: Rartar (8177, Horde faction, 1435 point 45.39, 56.87; also Alliance Nina Lightbrew 8178 in the Blasted Lands). Pin every buy `npc 8177`. (Profession per evident naming and the unpatched-family rule below; gated `when skill` in the established shape — see BORDERLINE.)
- Formula: Enchant Bracer - Deflection (11223), Enchanting — vendor: Banalash (989, Horde faction, 1435 point 44.77, 56.63; also Alliance Mythrin'dir 4229 in Teldrassil/Darnassus). Pin every buy `npc 989`.
- Recipe: Carrion Surprise (12232), Cooking — vendor: Banalash (989; also Horde Ogg'marr 4879 / Kireena 9636 and neutral Vendor-Tron 1000 12245 in Desolace). Pin every buy `npc 989`.
- Recipe: Spiced Chili Crab (16111), Cooking — vendor: Banalash (989; also Horde Uthok 1149 in Stranglethorn and Alliance Kriggon Talsone 4305 in Westfall). Pin every buy `npc 989`.

- Professions with NO Swamp source for a Horde player (stated in the guide, not padded): Tailoring, Engineering, Leatherworking. (Alchemy/Fishing below: Alchemy's sole in-zone candidate 9300 is gated per evident naming — the other Alchemy drops are all multi-zone; Fishing has no recipe source in the data at all.)
- The five Horde-vendor recipes ship here as in-zone Horde-vendor buys (Hillsbrad flipped precedent: the Alliance inventory excluded exactly these as Horde-vendor-only; for Horde they are the in-zone source). Each IS sold by Alliance/neutral vendors elsewhere, logged beside each entry so the exclusion/inclusion is checkable both ways.

EXCLUDED:
- Generic world drops (~130 items as scanned, 8-33 drop zones each — Elwynn rule): every other Swamp-touching recipe, including all chest-only finds and the narrowest argued borderlines — 217249 Earthen Silk Belt (57 droppers / 15 zones), 217251 Crimson Silk Shoulders (57 / 12), 217260 Big Voodoo Mask (56 / 12), 217264 Guardian Leather Bracers (62 / 12), 217271 Turtle Scale Gloves (32 / 9), 217278 Golden Scale Cuirass (59 / 15), 223163 Scroll of Spatial Mending (4 droppers / 9 zones — narrow but not zone-exclusive, and no in-zone sole dropper). None is zone-exclusive or has an in-zone sole dropper, so none is Swamp content.
- Quest-reward recipes: UNVERIFIABLE — quest records carry no reward data; never shipped (logged in `docs/companion-unverified.md`).
- Trainer-taught staples: OUT (Polestar's own profession guides cover them).

## Tameables: none shipped

No tame lines ship (Duskwood precedent: the bar does not lower): drop evidence exists for several beast-family candidates but the Horde core guide carries zero `only Hunter` lines and no references to any shipped rare — corroboration unmet across the board. Logged in `docs/companion-unverified.md`.

## BORDERLINE (argued, none decided silently)

1. 7492? No — the pool holds no such record; the enumeration above is exhaustive (9 rares + named objects + 144 recipes), and "no others" is a scan result, not an assertion.
2. 93568/93574 collects credit uncontracted quests' objectives: the census deferred both records to companions explicitly ("noted for companions"), so the collects are the deferred content itself — not scope creep. No accept/turnin lines anywhere; the quests stay uncontracted.
3. The 9300 profession gate (Alchemy vs Enchanting vs Cooking): gated per evident item-family naming in the pack's established shape; if the data ever gains a skill field, the gate follows the data.
4. The five Horde-vendor recipes' off-zone alternatives are logged beside each entry (Hillsbrad precedent) so a reader can verify the flip in both directions.
5. Caravan Chest ships for Horde as a unique with a dead-end note while the Alliance inventory excludes it as core-owned: the same object, honestly different dispositions — the Alliance `complete 1421` arrow does not exist for Horde (1421 is Alliance-only; Horde's 1422 twin is a talk-through that never touches the chest). Flagged, not harmonized.
