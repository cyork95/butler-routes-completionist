# Tanaris companions inventory (game data, accept-zone key 1446)

Source: local Forever game data (questie-forever NPC/object/item dumps).
Rank semantics calibrated against the Feralas round: rank 4 = Rare,
rank 2 = Rare Elite. Loot "sole dropper" means the item's drops.npc lists
only this NPC and no object source. Rates shown where the data gives a
number; Feralas-round calibration: the shipped signatures there also carry
null rates, so a null rate does not disqualify a sole drop.

## RARES — 10 flagged (7 Rare + 3 Rare Elite), all in band 38-50, all shipped

| NPC | Lvl | Rank | Point(s) | Sole-drop signature | Guide step |
|-----|-----|------|----------|---------------------|------------|
| 8201 Omgorn the Lost | 50 | 4 | (38.72,55.59) single | 17055 Changuk Smasher 20% | single goto + collect |
| 8202 Cyclok the Mad | 48 | 4 | (41.26,54.7) single | 286572 Ogre Casting Cloak | single goto + collect |
| 8203 Kregg Keelhaul | 47 | 4 | (73.22,48.71) single | none (generics only) | single goto + kill note |
| 8204 Soriid the Devourer | 50 | 4 | (34.07,44.72) single | none (generics only) | single goto + kill note |
| 8205 Haarka the Ravenous | 50 | 4 | (53.3,73.79) single | 286570 Silithid Flesh Bindings | single goto + collect |
| 8207 Greater Firebird | 46 | 4 | (49.39,36.04) single | 286569 Firebird Leggings | single goto + collect |
| 8208 Murderous Blisterpaw | 43 | 4 | (52.32,33.29) single | none (generics only) | single goto + kill note |
| 8199 Warleader Krazzilak | 45 | 2 | (38.79,21.72) single | 286554 Warleader's Signet | single goto + collect |
| 8200 Jin'Zallah the Sandbringer | 46 | 2 | (36.57,24.61) single | none (generics only) | single goto + kill note |
| 222243 Zopilote | 43 | 2 | 38 pts (24 + 14 more), east | 220687 Rune of the Raptor | loop + collect |

Notes:
- Zopilote is a Forever-original NPC (high ID). Its signature Rune of the
  Raptor is also sold by Rune Broker vendors spawning OUTSIDE Tanaris
  (233335 in 1426/1429/1438/1455/1457, 233428 in 1411/1420/1454/1456/1458);
  the guide notes that, Zopilote stays the sole in-zone mob source.
- Quest-link false positive checked and cleared: contracted quest 94301
  (Craftsman's Writ: Big Voodoo Robe) has objectives of type item with
  id 8200 ("Big Voodoo Robe") — an item/NPC ID collision, NOT Jin'Zallah
  as a quest objective. No rare in this list is a giver, ender, or
  objective of any core-contracted quest (objectives arrays scanned).
- Andre Firebeard (7883, the WANTED target) is NOT rare-flagged
  (rank unset) and is a core quest objective — stays out of the companion.
- No above-band rares: all 10 are 43-50, inside the 38-50 core band.
- Tameability: NO data flag exists; the Tanaris core guide carries no tame
  corroboration lines. No `only Hunter` tame lines ship. Logged in
  docs/companion-unverified.md.
- Respawn timers: unconfirmed anywhere in the data; none stated.

## TREASURES

- Generic "Solid Chest": object 4149 (14 fixed pts, west + east clusters)
  and object 153451 (13 fixed pts, north-center + cove clusters). ONE loop
  step over all 27 fixed points, said plainly as generic chests.
- 142184 "Captain's Chest": single fixed point (76.47,45.73), Lost Rigger
  Cove. Own single-goto step.
- 142194 "Pirate's Treasure!": 6 fixed points on the far-south island
  (50.7,90.78 / 52.16,94.39 / 53.09,95.89 / 54.06,93.03 / 54.54,95.09 /
  55.56,92.28 — same ground the Treasure Hunting Pirates work). Loop step.
- 179496 "Dented Footlocker": 7 fixed points around the cove
  (70.86,47.39 / 71.28,48.37 / 72.87,45.86 / 74.2,46.96 / 74.64,47.31 /
  74.82,45.51 / 75.63,45.1). Loop step.
- 442728 "Chest": single fixed point (45.8,37.6), center. Own single-goto
  step, named as found.
- None of the six is referenced by any core-contracted quest objective.

## RECIPES — 25 shipped (vendor 16 + drops 9)

Vendor-sold (all vendors spawn in-zone; all faction AH = Alliance-safe,
no Horde-only vendor in the set):
- Alchemy, Alchemist Pestlezugg (50.89,26.96, Gadgetzan): 6057 Recipe:
  Nature Protection Potion, 9303 Recipe: Philosopher's Stone, 9304 Recipe:
  Transmute Iron to Gold, 9305 Recipe: Transmute Mithril to Truesilver,
  12958 Recipe: Transmute Arcanite.
- Tailoring, Vizzklick (51.01,27.36, Gadgetzan): 7088 Pattern: Crimson
  Silk Robe, 21358 Pattern: Soul Pouch, 217244 Pattern: Crimson Silk Robe
  (same-title twin of 7088, also sold here — both ship with a note),
  253665 Pattern: Linen Reagent Bag, 253668 Pattern: Woolen Reagent Bag
  (also sold by 30+ vendors elsewhere; Vizzklick is the in-zone source —
  Feralas/Pratt precedent).
- Cooking, Gikkix (66.64,22.08, Steamwheedle Port): 13939 Recipe: Spotted
  Yellowtail, 13942 Recipe: Grilled Squid, 13945 Recipe: Nightfin Soup,
  13946 Recipe: Poached Sunscale Salmon.
- Cooking, Jabbey (67.01,21.99, port): 16767 Recipe: Undermine Clam Chowder.
- Cooking, Innkeeper Fizzgrimble (52.51,27.91) + Dirge Quikcleave
  (52.63,28.11), Gadgetzan: 18046 Recipe: Tender Wolf Steak (both sell it).

Dropped (genuinely zone content — single or in-zone-only droppers):
- Leatherworking 8395 Pattern: Tough Scorpid Breastplate <- 5618
  Wastewander Bandit (13 pts, east). 8397 Bracers <- 5617 Shadow Mage
  (22 pts, east). 8398 Gloves <- 5616 Thief (20 pts, east). 8399 Boots
  <- 5615 Rogue (20 pts, east). 8401 Leggings <- 5615 Rogue (same camp).
  8400 Shoulders + 8402 Helm <- 5623 Assassin (10 pts) / 7805 Scofflaw
  (single 66.16,34.99) / 7883 Andre Firebeard (73.37,47.14) — all three
  spawn only in Tanaris.
- Leatherworking 17722 Pattern: Gloves of the Greatfather <- 7856
  Southsea Freebooter (22 pts, cove pirates), sole dropper.
- Leatherworking 252908 Pattern: Supple Scorpid Boots <- 5471 Dunemaul
  Ogre (10 pts, south-west), sole dropper.

Excluded with reason:
- 15742 + 20253 Pattern: Warbear Harness — sole vendor Meilosh (11557)
  spawns in zones 1448/1452, not Tanaris (Alterac precedent: out-of-zone
  vendor = out).
- 8385 Pattern: Turtle Scale Gloves — vendors Pratt/Jangdor spawn in
  Feralas (1444), and 370 NPCs drop it zone-wide (Elwynn rule: generic).
- All 100+ dropper recipes (Big Voodoo set, Frostweave/Runecloth/
  Brightcloth/Mooncloth/Felcloth/Chimeric/Runic/Chromatic sets, alchemy
  transmutes and potions with 100-600 droppers) — generic world drops.
- 8384 Comfortable Leather Hat (29 droppers, 15 zones) and 217271
  Pattern: Turtle Scale Gloves (32 droppers, 9 zones) — multi-zone
  generics under the Elwynn rule, argued per-case, not shipped.
- 6663 Elixir of Giant Growth (113 droppers), 13489 Transmute Earth to
  Life (110 droppers) — generic despite one in-zone dropper each.
- 286153 Recipe: Plated Armorfish — source object 694054 spawns in
  zone 1430, not Tanaris.
- Quest-reward recipes: quest records carry no reward data — none
  shipped, class-logged in companion-unverified.
- Trainer-taught staples excluded (Polestar's own profession guides).

Professions with NO in-zone source (stated plainly in the guide, Dun
Morogh Blacksmithing precedent): Blacksmithing, Engineering,
Enchanting, First Aid, Fishing.
