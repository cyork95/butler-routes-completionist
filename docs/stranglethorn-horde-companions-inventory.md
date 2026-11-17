# Stranglethorn Vale (Horde) — companions inventory

Contract: the Horde core `stranglethorn-horde.guide` (39 quests, band
30-47). Accept-zone key 1434. Sources: `npcs.json`, `objects.json`,
`items.json`, `quests.json` from the local Forever data build
(`--product wowf` + QuestieDB). Game data wins everywhere below. Rank
semantics per the Feralas round: rank 4 = Rare, rank 2 = Rare Elite.

## Rares — 8 flagged, all shipped

Every NPC spawn on key 1434 carrying the data's rare flag. All eight
are faction-null (no Falthis-rule exclusion applies — nothing
friendly-to-Horde is flagged rare here) and none is faction-A, so no
Stonetalon-style opposition note is needed either. Levels run 37-45,
all inside the Horde core band (30-47); no above-band rares, nothing
deferred. None of the eight is a giver, ender, or objective of any of
the 39 Horde core quests (objectives arrays scanned; start.item/start
scanned; the eight IDs grepped against the core guide: zero hits) —
all eight are companion content, not core content. Respawn timers are
unconfirmed anywhere in the data; none stated.

- Mosh'Ogg Butcher | npc 723 | level 44 rare (rank 2) | single point
  (49.83, 30.87), Mosh'Ogg mound east | 1680 Headchopper 7%, sole
  dropper | also drops Maury's Key 3930 (30%, an Alliance-contract
  quest item for 613 — not shipped, not a signature) and Green Hills
  pages (Alliance-contract quest items — not shipped) | no quest
  linkage to the Horde 39
- Scale Belly | npc 1552 | level 45 rare | 4 pts north-center (41.79,
  48.36), (42.61, 46.49), (43.44, 45.71), (43.74, 47.5), loop step |
  1604 Chromatic Sword 25% + 4478 Iridescent Scale Leggings 75%, both
  sole droppers | no quest linkage
- Lord Sakrasis | npc 2541 | level 45 rare | 2 pts west (28.33, 62.56),
  (28.85, 62.04), loop step | 5028 Lord Sakrasis' Scepter 50% + 5029
  Talisman of the Naga Lord 50%, both sole droppers; Star Belt 4356
  also drops here at 0.12% but is a 25-dropper generic, not a
  signature — noted, not shipped | no quest linkage
- Gluggle | npc 14487 | level 37 rare | 4 pts north-west (33.92, 22.63),
  (34.71, 21.9), (34.87, 22.71), (35.52, 23.73), loop step | 281750
  Murloc Oracle's Dagger, sole dropper (no rate in the data) | no
  quest linkage
- Roloch | npc 14488 | level 38 rare | single point (37.37, 31.22) |
  generics only, kill note, no collect
- Rippa | npc 14490 | level 44 rare | single point (29.23, 84.89),
  cape tip | generics only (Glistening Frenzy Scale 91.7% is a trade
  good, not a signature), kill note, no collect
- Kurmokk | npc 14491 | level 42 rare | single point (38.11, 61.13) |
  281746 Kurmokk's Pelt, sole dropper (no rate in the data) | no quest
  linkage
- Verifonix | npc 14492 | level 42 rare | 6 pts center-west, loop step:
  (34.89, 56.02), (35.91, 54.46), (36.41, 55.94), (36.52, 57.06),
  (36.55, 55.5), (36.97, 53.82) | 281896 Surveyor's Gloves, sole
  dropper (no rate in the data) | no quest linkage

## Item-start hunts — nothing ships

The Horde core contract carries no item-starts (census scan: zero
Horde-mask `start.item` records on key 1434). Its sourceless objectives
(Soul Gem 3912, pledge 11282, I'lalai tablets 270308-11, Visions
19606-08, crafted 10559/4407/4392/8211/8214) name no mob, object, or
vendor anywhere in the data — the core guide carries explicit
have-in-bags notes, so there is nothing to hunt. Stonetalon 94216
pattern.

## Tame lines — none ships

No tameability flag exists anywhere in the data (same finding as the
Alliance round). No `only Hunter` task ships; all eight rare steps are
kill-or-collect. Logged in `docs/companion-unverified.md`.

## Treasures — fixed containers, Kurzen Supply Crate excluded

Quest-linkage scan (quest objective objects AND item-drops-from-object
against the 39 Horde core quests): object 424002 Kurzen Supply Crate
(49.6, 7.7) drops item 216617 Kurzen Fighter's Uniform, the objective
of core quest 97047 — the core guide already routes its collect there,
so no companion step ships for it (Stonetalon 6284 precedent: pointer
only). The Alliance companions inventory lists this crate as treasure;
its core routes the same uniform from the same crate — flagged in
`docs/companion-unverified.md`, not silently harmonized. Every other
container below has no quest linkage to the Horde 39.

- Generic "Solid Chest": object 2855 (12 fixed pts, north), object 2857
  (15 fixed pts, north + east), object 4149 (24 fixed pts on key 1434,
  south + center). ONE loop step over all 51 fixed points, said plainly
  as generic chests. All faction-null, all openable. (The Alliance
  inventory counts 30 for 4149 and 57 total; the data's 1434 pts array
  holds 24 — the guide loops the 51 placed points. Flagged in
  `docs/companion-unverified.md`, not silently harmonized.)
- Barrel of Sweet Nectar (3706) + Food Crate (3707): identical 24 fixed
  points each, paired placements across the zone (Alterac "matching Food
  Crates" precedent). ONE loop step over the shared 24 points with both
  interacts. (The Alliance inventory counts 45 each; the data's 1434 pts
  arrays hold 24 each — the guide loops the 24 placed points. Flagged in
  `docs/companion-unverified.md`, not silently harmonized.)
- Unique single-point objects, each its own step: 20691 Cozzle's
  Footlocker (43.33, 20.33); 59847 Cuts-N-Bruises Incorporated
  (28.36, 75.33, Booty Bay); 179697 Arena Treasure Chest (30.52, 47.87,
  Gurubashi Arena); 658116 Lost Shipping Crate (38, 3.01, Rebel Camp
  shore); 674124 Traveler's Cache (14.4, 27.2, north-west).
- Every object above exists in `objects.json` with 1434 spawns; no
  faction-locked container exists on key 1434 (no Horde-unusable
  equivalent of Stonetalon's Alliance Chest) — nothing excluded, and
  nothing referenced here is absent from the data.

## RECIPES — 65 shipped (58 vendor + 7 narrow drops)

Vendor scan: every recipe-named item (`Recipe:`/`Pattern:`/`Formula:`/
`Schematic:`/`Plans:`) whose `vendors` list includes an NPC spawning on
key 1434, faction-ruled per vendor (H/AH = buyable by Horde; A-only =
out under the flipped Alterac rule). Every buy ships npc-pinned to the
exact in-zone vendor (EPL lesson: no bare buys). Booty Bay's vendors
are neutral ground in the data (all AH except where noted) — ruled
from the faction field, not from assumption.

Booty Bay (all fac AH except where noted; points from `npcs.json`):
- Cooking, Kelsey Yance (2664, 28.23, 74.34): 6039 Recipe: Giant Clam
  Scorcho, 6369 Recipe: Rockscale Cod, 13940 Recipe: Cooked Glossy
  Mightfish, 13941 Recipe: Filet of Redgill, 13943 Recipe: Hot Smoked
  Bass, 17062 Recipe: Mithril Head Trout, 21099 Recipe: Smoked Sagefish,
  21219 Recipe: Sagefish Delight (same 8 the Alliance ships).
- Alchemy, Glyx Brewright (2848, 28.14, 78.11): 6056 Recipe: Frost
  Protection Potion, 6057 Recipe: Nature Protection Potion (same 2).
- Tailoring, Xizk Goodstitch (2670, 28.71, 76.89): 7087 Pattern: Crimson
  Silk Cloak, 253665 Pattern: Linen Reagent Bag, 253668 Pattern: Woolen
  Reagent Bag (same 3); Enchanting, same vendor: 14630 Pattern:
  Enchanter's Cowl, 217258 same-title twin (both ship with a note, same
  as Alliance).
- Tailoring, Cowardly Crosby (2672, 27, 82.48, cape): 10318 Pattern:
  Admiral's Hat (same 1).
- Tailoring, Narkk (2663, 28.13, 74.42): 10728 Pattern: Black
  Swashbuckler's Shirt (same 1).
- Leatherworking, Rikqiz (2699, 28.49, 76.05): 14635 Pattern:
  Gem-studded Leather Belt, 18239 Pattern: Shadowskin Gloves (same 2).
- Leatherworking, Blixrez Goodstitch (2846, 28.25, 77.54): 5788
  Pattern: Thick Murloc Armor, 5789 Pattern: Murloc Scale Bracers (same
  2; 5788 also drops off Kurzen Commando 938 in-zone at 2.22%, 5789 off
  Bloodsail Raider 1561 in-zone at 1.98% — the vendor is the clean
  in-zone source, so both ship as buys).
- Tailoring, Pix Xizzix (227853, 28.52, 75.86): 228121 Pattern:
  Leather-Reinforced Runecloth Bag (same 1).
- Engineering, Knaz Blunderflame (8679, 51.05, 35.23, east): 10602
  Schematic: Deadly Scope.
- Blacksmithing, Jutak (2843, 27.46, 77.55): 12162 Plans: Hardened Iron
  Shortsword.
- Blacksmithing, Zarena Cromwind (2482, 28.34, 75.46): 12163 Plans:
  Moonsteel Broadsword + 217282 same-title twin (both ship with a note,
  Enchanter's-Cowl-twin precedent).
- Blacksmithing, Vharr (1146, 32.36, 27.95, Grom'gol, fac H): 12164
  Plans: Massive Iron Axe (Jaquilina Dramet 2483, 35.75, 10.66 north,
  fac AH, stocks the same plan — the Grom'gol pin is the routed one).
- Engineering, Mazk Snipeshot (2685, 28.5, 75.12): 13310 Schematic:
  Accurate Scope, 18651 Schematic: Truesilver Transformer.
- Engineering, Gnaz Blunderflame (2687, 50.98, 35.21, east): 13311
  Schematic: Mechanical Dragonling.
- Engineering, Crazk Sparks (2838, 28.36, 76.66): 18648 Schematic:
  Green Firework.

Grom'gol (fac H — the Alliance round's exclusions, now shippable):
- Cooking, Nerrist (1148, 32.7, 29.23): 3682 Recipe: Curiously Tasty
  Omelet (sole in-zone vendor; the Alliance vendors are Stormwind/
  Arathi), 12228 Recipe: Roast Raptor, 12231 Recipe: Jungle Stew
  (Corporal Bluth 734 is A-faction and excluded under the flipped
  Alterac rule; Nerrist stocks both — Tanaris/Vizzklick precedent,
  Horde side).
- Cooking, Uthok (1149, 31.55, 27.95): 16111 Recipe: Spiced Chili Crab
  (sole in-zone vendor).

Yojamba Isle (Rin'wosho the Trader 14921, 15.07, 16, fac AH) — the full
23 stocked here, not just the Alliance round's 12:
- Leatherworking: 19764/19765/19766 Bloodvine 3, 19769/19770/19771
  Primal Batskin 3, 19772/19773 Blood Tiger 2, 19776/19777/19778
  Bloodsoul 3, 19779/19780/19781 Darksoul 3.
- Blacksmithing: 20000 Schematic: Bloodvine Goggles, 20001 Schematic:
  Bloodvine Lens.
- Alchemy: 20011 Recipe: Mageblood Potion, 20012 Recipe: Greater
  Dreamless Sleep, 20013 Recipe: Living Action Potion, 20014 Recipe:
  Major Troll's Blood Potion.
- Enchanting: 20756 Formula: Brilliant Wizard Oil, 20757 Formula:
  Brilliant Mana Oil.
- Cooking: 232610 Formula: Magnificent Trollshine.
- The 11 beyond the Alliance round's 12 share the vendor and the access
  — data wins, so all 23 ship. Flagged in
  `docs/companion-unverified.md`, not silently harmonized.

Dropped (genuinely narrow — sole in-zone dropper families, rates where
the data gives them):
- Cooking 250185 Recipe: Twice-Spiced Raptor Slice <- 855 Young
  Stranglethorn Raptor (lvl 30, 3 pts north-west), sole dropper (same as
  Alliance).
- Tailoring 254018 Pattern: Earthen Silk Gloves <- 701 Bloodscalp
  Mystic (lvl 34, north-west), sole dropper (same as Alliance).
- Tailoring 254022 Pattern: Gilded Handwraps <- 873 Saltscale Oracle
  (lvl 36), sole dropper (same as Alliance).
- Enchanting 11203 Formula: Enchant Gloves - Advanced Mining <-
  Venture Co. Strip Miner 674 (lvl 40, 4%), sole dropper, 1434-only.
- Blacksmithing 251388 Plans: Hard Gold Leggings <- Kurzen Jungle
  Fighter 937 (lvl 32), sole dropper, 1434-only (no rate in the data).
- Blacksmithing 251395 Plans: Shining Mithril Helm <- Naga Explorer
  1907 (lvl 43), sole dropper, 1434-only (no rate in the data).
- Engineering 264210 Schematic: Shafety Sheep <- Venture Co. Miner 1094
  (lvl 34), two-zone family (1434 north + Westfall 1436) — narrow, not
  zone-exclusive, said so (Stonetalon 11151 precedent; flagged in
  `docs/companion-unverified.md`).

Excluded with reason:
- 12228/12231 via Corporal Bluth (A-faction) — excluded; both ship via
  Nerrist above (flipped Alterac rule).
- 15742 Pattern: Warbear Harness — sole vendor Meilosh (11557) spawns
  in zones 1448/1452, not Stranglethorn (same as Alliance).
- 8385 Pattern: Turtle Scale Gloves — vendors 7852/7854 spawn outside
  key 1434, and its droppers are zone-wide generics (Elwynn rule; same
  as Alliance).
- 4356 Pattern: Star Belt (25 droppers incl. in-zone Sakrasis at 0.12%)
  — generic world drop, noted, not shipped (same as Alliance).
- 14509/14510/14511 + 228317 world-boss patterns (lead in-zone dropper
  is Lord Kazzak 12397, level 63 — out of reach for a 30-47 guide,
  Feralas world-boss precedent; same as Alliance).
- Object-chest generics (2406-2409, 2553-2601, 2881-2883, 3393-3396,
  3608-3874, 4292-4301, 4345-4354, 4398+, 5543+ and the whole chest-loop
  class): 0.2-0.7% drops off a dozen-plus world chests each — generic
  under the Elwynn rule, argued per-case, not shipped. Skill-up whites
  (3395 Elixir of Lesser Agility etc.) ride the same rule.
- Quest-reward recipes: quest records carry no reward data — none
  shipped, class-logged in companion-unverified.
- Trainer-taught staples excluded (Polestar's own profession guides).

Professions with NO in-zone Horde source, stated in the guide, not
padded: First Aid, Fishing. (Genuine Horde difference: Blacksmithing
and Engineering DO have in-zone sources here — Jutak/Zarena/Vharr plans
and Knaz/Mazk/Gnaz/Crazk schematics — so neither profession is listed
as sourceless, unlike the Alliance round.)
