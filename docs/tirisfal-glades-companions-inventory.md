# Tirisfal Glades companions inventory (pack 0.95.0)

Source: local Forever game data (questie-forever npc/object/item dumps),
zone key 1420, band 1-13, faction Horde. City-key (1458) spawns excluded
per the city rule. Every point below is a data spawn point; nothing is
invented. Core contract = 109 quests (`tirisfal-glades` in
docs/quest-contracts.json); companions carry no accept/turnin lines.

## Rares — scanned, 13 rare-shaped NPCs on 1420

Nine carry the data's rare role; four are rank-4 elites with no rare
role. No candidate is a core-contract quest target and none is a
quest-target lookalike (every shipped rare has its own loot table).

SHIPPED with the rare role (kill entries; signature collect where the
drop is exclusive to that NPC anywhere in the data):

- Lost Soul 1531, lvl 6, 3 pts (44.6,40.51 / 53.18,48.37 / 53.34,45.6).
  No exclusive drop (generic table) — kill entry, no collect.
- Tormented Spirit 1533, lvl 8, 1 pt (45.59,31.62). No exclusive drop.
- Muad 1910, lvl 10, 1 pt (36.49,42.39). No exclusive drop.
- Deeb 1911, lvl 12, 1 pt (63.29,27.48). No exclusive drop.
- Farmer Solliden 1936, lvl 8, 4 pts (34.07,52.11 / 37.09,49.46 /
  38.03,52.21 / 38.04,49.61). Exclusive: 4261 Solliden's Trousers
  (sole NPC dropper) — optional collect.
- Bayne 10356, lvl 10, 1 pt (39.9,42.16). Exclusive: 283462 Bayne's
  Bite (sole NPC dropper) — optional collect.
- Ressan the Needler 10357, lvl 11, 1 pt (42.86,67.57). Exclusive:
  283473 Batwing Bindings (sole NPC dropper) — optional collect.
- Fellicent's Shade 10358, lvl 12, 1 pt (76.96,60.35). Exclusive:
  283471 Fellicent's Bindings (sole NPC dropper) — optional collect.
- Sri'skulk 10359, lvl 13, 1 pt (88.16,51.44). Exclusive: 283480
  Cracked Carapace Hauberk (sole NPC dropper) — optional collect.

SHIPPED rank-4 without the rare role, with the Mulgore-custom-trio
caveat stated (exclusive named loot, no data rare flag):

- Blightsculler 271080, lvl 10, 24 pts, west shore x12-22 z47-62.
  Exclusive: 283460 Decaying Flesh Belt (sole NPC dropper).
- Decrepit Harvester 276061, lvl 8, 24 pts, Brill-west x50-61 z53-61.
  Exclusive narrow recipe: 277470 Schematic: Harvester Override
  Signalcaster (sole NPC dropper) — the collect ships in the RECIPES
  guide; the kill entry rides here with a pointer note.
- The Condemned One 276089, lvl 11, 24 pts, east x64-74 z36-51.
  Exclusive: 286755 Helm Splitter (sole NPC dropper).

EXCLUDED:

- Coldrasp 274300, lvl 12, rank-4, no rare role, NW x14-22 z60-74.
  No exclusive drop (only generic loot plus the zone-flavor custom
  scrolls 211785-87 that drop from nearly everything) and no quest
  linkage — the Durotar lootless-pair outcome, not the Mulgore-trio
  one. Logged, never shipped as fact.

No above-band rares exist (all 13 are lvl 6-13, band is 1-13), so no
come-back-later calls were needed on the rares side.

TAMES: no tame line ships. Bayne (wolf drops), Ressan (bat drops) and
Sri'skulk (spider drops) have drop evidence but the core guide kills
no same-species beast by ID (core kills Duskbats and Night Web
spiders, not Needlers/wolves/this spider), so corroboration fails the
Mulgore bar. All three are logged in docs/companion-unverified.md
with this reasoning. The other ten are undead/humanoid/mechanical or
unknown-nonbeast types and are not tame candidates.

## Treasures — scanned, all fixed-spawn objects on 1420

SHIPPED (all lootless and quest-unused in the data; shipped
Deadwind/Shen'dralas-style with "contents unconfirmed" notes):

- Battered Chest 2843, 7 pts (23.6,58.28 / 24.71,59.78 / 26.11,60.35 /
  31.32,62.16 / 34.22,64.3 / 36.51,62.2 / 37.35,68.01) — one loop.
- Battered Chest 106318, 12 pts (31.63,46.11 / 34.72,40.98 /
  37.93,49.61 / 49.24,33.57 / 49.68,35.68 / 49.79,42.73 / 51,67.4 /
  57.91,32.88 / 58.86,26.91 / 67.08,25.84 / 72.83,25.84 / 77.21,59.79)
  — one loop.
- Perrine's Chest 37098, 1 pt (51.06,67.57) — at the core 370 kill
  site (Captain Perrine @51.14,67.80); note points at the core route.
- Buried Treasure 386675, 1 pt (52.9,54).
- Lost Stash 406736, 1 pt (24.6,59.5).
- Shipwreck Cache 405201, 1 pt (66.7,24.6).
- Supply Locker 412147, 1 pt (81.1,32.1).
- Relic Coffer 404941, 1 pt (52.5,25.8).
- Dark Cleric Salem's Chest 178464, 1 pt (87.06,43.15).
- Mech Arm 459259, 11 pts (52.4,57.7 / 53,55.8 / 53.2,57 / 53.3,57.5 /
  53.7,56.6 / 54.2,57.5 / 54.2,58.7 / 54.5,56.7 / 54.5,58.2 /
  54.8,56.4 / 57.9,56.9) — one loop.

EXCLUDED with reasons:

- Core-contract quest objects (used by routed quests): Wanted poster
  711 (398), Crate of Candles 1586 (431), Gunther-adjacent Lillith's
  Dinner Table 1557 (410), Apothecary Society Primer 405879 (79095),
  Agamand Weapon Racks 105169-72 (1821), Equipment Boxes 164662
  (3902), Marla's Grave 178090 (6395), Dry Branch 671154 (86784
  objective), Glowing Crystal Fragment 694895 (99153), Gloom Weed
  175566 (5481), Doom Weed 175753 (5482), Lumber Pile 554626 (91316),
  Tomb Weed 694732 (99142), Tirisfal Pumpkin 375 (365/407), Bottle
  objects 630871/630885 (95314's 8 elixir bottles — the core complete
  @8.60,59.50 sits on 630871's first point).
- Seasonal/event: all XMas/Winter objects, Hallow's End objects
  (pumpkins G_Pumpkin_*, ghosts, candy, witch hats/brooms, Wickerman,
  bonfires/embers, banners), Nobleman's eggs 113772, Brewfest/
  Midsummer party objects, Box of Incendiaries 176200-204.
- Gathering nodes (never treasures): Silverleaf/Peacebloom/
  Earthroot/Arthas' Tears/Sungrass/Dreamfoil/Mountain Silversage/
  Wilted/Stunted herbs, Copper/Tin/Silver/Gold/Mithril/Truesilver/
  Poor Copper veins.
- Service/scenery: forges, anvils, campfires/cozy fires, chairs,
  mailbox, signposts (1630-66, 2033-38, 146079-81), doors/levers,
  meeting stone, zeppelin, Portal to Orgrimmar, Water Barrel 3658,
  Food Crates 3719/153472/153473 (ambient, no loot/quest evidence).
- Flavor with no loot and no quest (examined, not shipped):
  Gunther's Books 1165, Balnir Snapdragons 102985, Scarlet Watch Post
  19028, Cauldrons 177284/85, Chest of Containment Coffers 105174,
  Cantation of Manifestation 105175, Blood of Heroes 176213,
  Naxxramas Crystal Fragment 656366, Elemental Convergence 616992,
  Relic Vendor object 58611 (vendor-object with no stocked recipes in
  the data; also spawns on 1458).

## Recipes — scanned, 4 ship, all mob-dropped (zero vendor-sold)

Vendor scan: all 331 NPCs spawning on 1420 checked against every
item's vendor list — NO recipe/pattern/plans/schematic/formula sold
by any in-zone vendor. Trainer-taught staples excluded (Polestar's
own profession guides). Quest-reward recipes unverifiable (no reward
data in quest records) — logged as a class, never shipped.

SHIPPED (every goal optional, profession-gated):

- Alchemy: 250366 Recipe: Minor Cleric's Elixir — 4 droppers in 2
  zones; in-zone half is Vile Fin Muckdweller 1545 + Vile Fin
  Attacker 250283 (both lvl 9, core-killed Vile Fin family). Borderline
  call, shipped: 4 droppers is a small named set and the in-zone half
  is family the core route already kills (collect placed on the Vile
  Fin shore @26.81,46.77). Elwynn half (Murloc Forager, Elder
  Finseer) logged here.
- Alchemy: 250988 Recipe: Minor Mender's Potion — 2 droppers in 2
  zones; in-zone dropper Tirisfal Farmer 1934 (lvl 6, 8 pts
  x34-38 z50-52, core quest 364 kills 8 farmers). Shipped (collect
  @36.54,51.80); Teldrassil half (Gnarlpine Mystic) logged here.
- Engineering: 277470 Schematic: Harvester Override Signalcaster —
  SOLE dropper Decrepit Harvester 276061 (in-zone only). Shipped
  (collect at the Harvester grounds @52.03,55.44); kill entry rides
  in the rares guide.
- Engineering: 264207 Schematic: SAF-T Bronze Bomb — SOLE dropper
  Scarlet Scout 4281, but the scout is lvl 29 in the far east
  (x81-87 z28-38), far above band. Shipped with an honest
  come-back-later note (Westfall/Hillsbrad precedent); collect placed
  @83.07,29.34.

EXCLUDED: every classic dropped recipe found on the rare tables
(2553, 2555, 2406/2407/2408, 2598, 6271, 7288, 3609/3610, 4408,
6342/6344/6348, 6716, 4346 — 400-570 droppers each) as generic world
drops per the Elwynn rule; 255007 Golem Isospring (5 droppers) and
255154 Ruined Gyrostabilizer (2 droppers: Westfall Rusty Harvest
Golem + Decrepit Harvester) as Westfall-shared, not zone content.

No-source professions (stated in the guide): Blacksmithing,
Cooking, Enchanting, First Aid, Fishing, Herbalism, Leatherworking,
Mining, Skinning, Tailoring.
