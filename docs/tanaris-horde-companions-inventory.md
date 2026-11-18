# Tanaris (Horde) companions inventory (game data, accept-zone key 1446)

Source: local Forever game data (questie-forever NPC/object/item dumps),
enumerated fresh for the Horde side — nothing copied from the Alliance
inventory without re-verification. Rank semantics per the Feralas
calibration: rank 4 = Rare, rank 2 = Rare Elite. Loot "sole dropper" means
the item's drops.npc lists only this NPC and no object source.

## RARES — 10 flagged (7 Rare + 3 Rare Elite), all in band 38-50, all shipped

Every rare-flagged NPC spawning on key 1446 was enumerated from the data:
exactly the same 10 the Alliance inventory lists, and every point below
was re-read from the spawn data (not carried over). All ten are
faction-null — no Falthis exclusion applies; Horde players can engage all
of them.

| NPC | Lvl | Rank | Point(s), verified | Sole-drop signature | Guide step |
|-----|-----|------|--------------------|---------------------|------------|
| 8201 Omgorn the Lost | 50 | 4 | (38.72, 55.59) single | 17055 Changuk Smasher 20% | single goto + collect |
| 8202 Cyclok the Mad | 48 | 4 | (41.26, 54.70) single | 286572 Ogre Casting Cloak (null rate; sole dropper — Feralas calibration) | single goto + collect |
| 8203 Kregg Keelhaul | 47 | 4 | (73.22, 48.71) single | none (generics only) | single goto + kill note |
| 8204 Soriid the Devourer | 50 | 4 | (34.07, 44.72) single | none (generics only) | single goto + kill note |
| 8205 Haarka the Ravenous | 50 | 4 | (53.30, 73.79) single | 286570 Silithid Flesh Bindings (sole dropper) | single goto + collect |
| 8207 Greater Firebird | 46 | 4 | (49.39, 36.04) single | 286569 Firebird Leggings (sole dropper) | single goto + collect |
| 8208 Murderous Blisterpaw | 43 | 4 | (52.32, 33.29) single | none (generics only) | single goto + kill note |
| 8199 Warleader Krazzilak | 45 | 2 | (38.79, 21.72) single | 286554 Warleader's Signet (sole dropper) | single goto + collect |
| 8200 Jin'Zallah the Sandbringer | 46 | 2 | (36.57, 24.61) single | none (generics only) | single goto + kill note |
| 222243 Zopilote | 43 | 2 | 38 pts (24 + 14 more), east | 220687 Rune of the Raptor (sole in-zone mob drop; Rune Brokers outside Tanaris also sell it — noted, Zopilote stays) | loop + collect |

Notes:
- The rare SET is genuinely identical to the Alliance inventory's — verified
  point-for-point from the spawn data, not harmonized. Deltas: none.
- Quest-link scan over the Horde contract (32/379/654/864/2967/4509/97534:
  starts, ends, and objective IDs): no rare in this list is a giver, ender,
  or objective of any HORDE-contracted quest. The 94301/8200 item-ID
  collision noted in the Alliance inventory belongs to an
  Alliance-contracted quest and does not touch the Horde contract.
- Andre Firebeard (7883, rank unset — NOT rare-flagged) stays out; he is a
  mob-drop source for two shipped recipes (named at the drop, not routed).
- No above-band rares: all 10 are 43-50, inside the 38-50 Horde band.
- Tameability: NO data flag exists; tanaris-horde.guide carries no tame
  lines and no references to any Tanaris rare. No `only Hunter` tame lines
  ship (same bar as the Alliance side, logged in
  docs/companion-unverified.md).
- Respawn timers: unconfirmed anywhere in the data; none stated.

## ITEM-START HUNTS — none

- 654 Tanaris Field Sampling starts from item 8524 (Model 4711-FTZ Power
  Source), which has NO source anywhere in the data (no droppers, no
  vendors, no object) — a core R2 bag-note case, and no rare drops it.
- 2967 Return to Thunder Bluff starts from the Uldum Pedestal object
  (142343, single point 37.63, 81.4 on 1446) — a fixed object-start, core
  content, not a rare hunt.
- The other five Horde contracts accept from NPCs. No rare drops any
  Horde-contract starter: zero hunts ship, stated with the scans behind it.

## TREASURES

- Generic "Solid Chest": object 4149 (14 fixed pts, west + east clusters)
  and object 153451 (13 fixed pts, north-center + cove clusters) — counts
  re-verified. ONE loop step over all 27 fixed points, said plainly.
- 142184 "Captain's Chest": single fixed point (76.47, 45.73), Lost Rigger
  Cove. Own single-goto step.
- 142194 "Pirate's Treasure!": 6 fixed points on the far-south island
  (50.70, 90.78 / 52.16, 94.39 / 53.09, 95.89 / 54.06, 93.03 / 54.54, 95.09 /
  55.56, 92.28). Loop step.
- 179496 "Dented Footlocker": 7 fixed points around the cove
  (70.86, 47.39 / 71.28, 48.37 / 72.87, 45.86 / 74.20, 46.96 / 74.64, 47.31 /
  74.82, 45.51 / 75.63, 45.10). Loop step.
- 442728 "Chest": single fixed point (45.80, 37.60), center. Own
  single-goto step, named as found.
- None of the six is referenced by any Horde-contracted quest objective.

## RECIPES — 25 shipped (vendor 16 + drops 9)

All six recipe vendors are faction AH (neutral) with in-zone spawns —
Gadgetzan's Steamwheedle neutrality confirmed in the data, not assumed.
Neutral stock is not a delta: where the data shows the same vendor selling
to both factions, the buy pins to that same vendor and this inventory says
so. Every stock line below was re-read from the item vendor tables.

- Alchemy, Alchemist Pestlezugg (5594 @50.89, 26.96, Gadgetzan):
  6057 Recipe: Nature Protection Potion (also sold by Glyx Brewright AH in
  STV, Logannas A + Bronk H in Feralas — Pestlezugg is the in-zone neutral
  source), 9303 Recipe: Philosopher's Stone, 9304 Recipe: Transmute Iron to
  Gold, 9305 Recipe: Transmute Mithril to Truesilver, 12958 Recipe:
  Transmute Arcanite (Pestlezugg sole vendor on all four).
- Tailoring, Vizzklick (6568 @51.01, 27.36, Gadgetzan): 7088 Pattern:
  Crimson Silk Robe, 21358 Pattern: Soul Pouch (both also sold by Stitch
  Pinwizzle AH in zone 2548 — out of zone; Vizzklick is the in-zone
  source), 217244 Pattern: Crimson Silk Robe (same-title twin of 7088,
  Vizzklick-sole — both ship with a note), 253665 Pattern: Linen Reagent
  Bag, 253668 Pattern: Woolen Reagent Bag (30+ vendors elsewhere;
  Vizzklick is the in-zone source — Feralas/Pratt precedent).
- Cooking, Gikkix (8137 @66.64, 22.08, Steamwheedle Port): 13939 Recipe:
  Spotted Yellowtail, 13942 Recipe: Grilled Squid, 13945 Recipe: Nightfin
  Soup, 13946 Recipe: Poached Sunscale Salmon (Gikkix sole vendor on all
  four).
- Cooking, Jabbey (8139 @67.01, 21.99, port): 16767 Recipe: Undermine Clam
  Chowder (also sold by Grizzek AH in 2548 — out of zone; Jabbey is the
  in-zone source).
- Cooking, Innkeeper Fizzgrimble (7733 @52.51, 27.91) + Dirge Quikcleave
  (8125 @52.63, 28.11), Gadgetzan: 18046 Recipe: Tender Wolf Steak (both
  sell it; also sold by Truk Wildbeard A in Hillsbrad/Alterac and Zizplink
  AH in 2548 — the Gadgetzan neutral pair is the in-zone Horde source).

Dropped (genuinely zone content — single or in-zone-only droppers, zones
re-verified: every dropper below spawns ONLY on 1446):
- Leatherworking 8395 Pattern: Tough Scorpid Breastplate <- 5618
  Wastewander Bandit (13 pts, east). 8397 Bracers <- 5617 Shadow Mage
  (22 pts, east). 8398 Gloves <- 5616 Thief (20 pts, east). 8399 Boots
  <- 5615 Rogue (20 pts, east). 8401 Leggings <- 5615 Rogue (same camp).
  8400 Shoulders + 8402 Helm <- 5623 Assassin (10 pts) / 7805 Scofflaw
  (single 66.16, 34.99) / 7883 Andre Firebeard (73.37, 47.14).
- Leatherworking 17722 Pattern: Gloves of the Greatfather <- 7856
  Southsea Freebooter (22 pts, cove pirates), sole dropper.
- Leatherworking 252908 Pattern: Supple Scorpid Boots <- 5471 Dunemaul
  Ogre (10 pts, south-west), sole dropper.

Excluded with reason:
- 15742 + 20253 Pattern: Warbear Harness — sole vendor Meilosh (11557)
  spawns outside Tanaris (Alterac precedent: out-of-zone vendor = out).
- All 100+ dropper recipes (Big Voodoo set, Frostweave/Runecloth/
  Brightcloth/Mooncloth/Felcloth/Chimeric/Runic/Chromatic sets, alchemy
  transmutes and potions with 100-600 droppers) — generic world drops.
- 8384 Comfortable Leather Hat (29 droppers, 15 zones) and 217271
  Pattern: Turtle Scale Gloves (32 droppers, 9 zones) — multi-zone
  generics under the Elwynn rule.
- 6663 Elixir of Giant Growth (113 droppers), 13489 Transmute Earth to
  Life (110 droppers) — generic despite one in-zone dropper each.
- 286153 Recipe: Plated Armorfish — source object 694054 spawns in
  zone 1430, not Tanaris.
- Quest-reward recipes: quest records carry no reward data — none
  shipped, logged in companion-unverified.
- Trainer-taught staples excluded (Polestar's own profession guides).

Professions with NO in-zone Horde source (stated plainly in the guide,
Dun Morogh Blacksmithing precedent): Blacksmithing, Engineering,
Enchanting, First Aid, Fishing.

## DELTAS vs the Alliance inventory — none

Rare set, rare points, treasure objects and points, recipe set, vendor
pins, and the no-source profession list are all identical between the two
faction inventories — each verified independently from the data on this
round (spawns, vendor tables, drop tables all re-read). No silent
harmonization was needed because no difference was found; had any
appeared it would be flagged in docs/companion-unverified.md.
