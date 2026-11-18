# Hinterlands (Horde) companions inventory

Scope: accept-zone key **1425**, Horde core band **38–46**, faction
**Horde**. Built from the local data dumps (`upstream-polestar/data/forever/*.json`:
`npcs.json`, `objects.json`, `items.json`, `quests.json`) — game data wins
over the Alliance inventory (`docs/hinterlands-companions-inventory.md`)
wherever they differ; every delta is flagged inline AND logged in
`docs/companion-unverified.md`, never silently harmonized.

The Horde core contract is 25 quests (`docs/the-hinterlands-horde-census.md`):
OOX honey chain (77/81), Fel'zerul return (1444), Rin'ji chain
(2742/2782), Venom Bottles (2933), the Revantusk core (7815-7816,
7828-7830, 7839-7844), the Torntusk chain (7845-7847, 7849-7850), the
wanted posters (7861/7862) and Ti'ik (98203). No Horde-contracted quest
is item-started, so there is no writable in-zone item-start hunt —
stated, not padded.

## Rares — 10 rank-flagged on 1425, all 10 shipped

Rank semantics per the Badlands calibration: rank 4 = Rare, rank 2 =
Rare Elite. Every point below is the data's spawn point verbatim.
Signature = the item's sole dropper anywhere in the data (drops.npc
lists this NPC only). Verified in THIS build — same ten as Alliance,
same signatures.

| NPC | lvl | points (map 1425 unless noted) | signature (sole drop) | disposition |
|-----|-----|--------------------------------|------------------------|-------------|
| 8210 Razortalon | 44 | 1: 37.06,45.33 | 283545 Moonchaser's Headdress | SHIP single-goto + collect |
| 8211 Old Cliff Jumper | 42 | 2: 1425 (11.92,53.7) + 1424 (96.9,14.6) | none (wolf meat/paw/mane, all shared) | SHIP 2-pt cross-zone loop, kill-only |
| 8212 The Reak | 49 | 1: 58.88,43.12 | 284043 Dissolved Link Legguards | SHIP single-goto + collect + CBL note |
| 8213 Ironback | 51 | 1: 81.48,49.19 | none (turtle meat/scale/shell, all shared) | SHIP single-goto, kill-only + CBL note |
| 8214 Jalinde Summerdrake | 49 | 1: 30.25,47.95 | 284050 High Elf's Recurve | SHIP single-goto + collect + CBL note; faction=A alignment note (shipped like any other rare) |
| 8215 Grimungous | 50 Rare Elite | 1: 70.19,55.38 | 284064 Cliffbreaker's Pauldrons | SHIP single-goto + collect + CBL note |
| 8216 Retherokk the Berserker | 48 | 1: 50.54,64.13 | 284061 Berserker's Wraps | SHIP single-goto + collect + CBL note |
| 8217 Mith'rethis the Enchanter | 52 Rare Elite | 1: 63.86,77.61 | 17050 Chan's Imperial Robes | SHIP single-goto + collect + CBL note |
| 8218 Witherheart the Stalker | 45 | 1: 33.12,70.29 | 284046 Witherheart's Stabber | SHIP single-goto + collect |
| 8219 Zul'arek Hatefowler | 43 | 1: 32.42,56.9 | 284063 Witherbark Hatecleaver | SHIP single-goto + collect |

Notes applied in the guide:
- Retherokk, Witherheart and Zul'arek drop 9259 Troll Tribal Necklace,
  the objective item of Horde-core 7842 (Another Message to the
  Wildhammer) — the steps carry a pointer at the core guide and never
  accept. Mith'rethis drops it too; his step carries the same note.
  (Alliance pointed at 2880/2881; the Horde mirror is 7842.)
- Razortalon, Jalinde, Mith'rethis and Zul'arek drop 8704
  OOX-09/HL Distress Beacon, the starter of 485 (Find OOX-09/HL!,
  contracted in the main guide) — noted, never accepted in the
  companion. (Horde-side: Gammerita 7977, the core 7816 lure target,
  also drops it — same note class.)
- Retherokk, Witherheart, Zul'arek, Mith'rethis, the Jintha'Alor
  keepers/trolls below AND the four narrow-drop steps' mobs all drop
  9294 Recipe: Wildvine Potion (27 in-zone droppers, 3 zones total:
  1417/1425/1434 — narrow, not a dozens-of-zones world drop, same call
  as Alliance): the recipes guide owns that hunt (kill + signature
  collect on each narrow-drop step); the four rare steps carry the
  pointer note instead of their own hunt.
- Jalinde Summerdrake is faction=A (Alliance-aligned). She is shipped
  like any other rare: the data flags her rare with loot, and the guide
  takes no position on whether to attack beyond stating the alignment.
- Six rares (8212/8213/8214/8215/8216/8217, L48–52) sit above the
  38–46 band: shipped with honest come-back-later notes (same six as
  Alliance, whose 38–51 band still left Mith'rethis noted). Nothing is
  far-above-band, so nothing is excluded on level.
- 8215/8217 are rank 2 (Rare Elite) — shipped per the Badlands
  calibration (rank 2 = Rare Elite), same as Alliance.
- No rare here is a giver, ender or kill objective of any
  Horde-contracted quest, so the Dun Morogh exclusion fires on none of
  the 10.
- TAME: no tame lines ship. The data has no tameability flag. Old Cliff
  Jumper (wolf: Red Wolf Meat / Tender Wolf Meat) and Ironback (turtle:
  Turtle Meat) have beast-drop evidence, but the core guide never sends
  the player at wolves or turtles (core kills are snapjaws, stalkers,
  howlers, owlbeasts, skylords, Highvale humanoids, Vilebranch trolls,
  oozes, Ti'ik) — no corroboration. Razortalon has bird-drop evidence
  (Giant Egg, feathers) and the core has an optional roc kill (2659
  Razorbeak Skylord via 7830), but the family link is unverifiable from
  the data. All three logged in docs/companion-unverified.md.
- Respawn timers are unconfirmed in the data - none stated.

Excluded lookalikes (with reason, verified in this build): 221310-221313
(Ysondre, Lethon, Emeriss, Taerar), level 63 rank-3 Dragons of Nightmare
spawning on 4 zones (1425/1431/1440/1446). Not rare-flagged, world-boss
rank, far above band - not companion content, with reason. (Also present
as 14887-14890 same-name rank-1 singles on 1425 - unflagged lookalikes,
not rares.)

## Jintha'Alor named spawns — ruled one by one (named check)

The troll city terraces hold named spawns tied to core-contracted
NON-item-start quests. Standing rule: a named NPC whose only
significance is a core-contracted NON-item-start quest is NOT companion
content, and quest-target lookalikes are not rares without their own
rank flag and loot. Outcome:

- 7995 Vile Priestess Hexx (L51, rank 1, NO rare role, 1 pt 59.47,78.26):
  kill objective of core 7861 — OUT (core quest target, not a rare).
- 2643 Berserker / 2645 Shadow Hunter / 2646 Blood Drinker / 2647 Soul
  Eater (rank 1, 15/19/24/15 pts, terraces): kill objectives of core
  7862 — OUT. 2648 Aman'zasi Guard (rank 1, 24 pts): kill objective of
  core 7861 — OUT.
- 2644 Vilebranch Hideskinner (rank 1, 15 pts, NO quest refs at all):
  regular mob, no flag, no signature — OUT (lookalike without rare
  data, not companion content).
- 10802 Hitah'ya the Keeper (L51, rank 1, NO rare role, 1 pt
  57.32,86.64): drops 19064 Shackle Key, the objective item of core
  7846 (plus 9294/9259/8704 among generics) — a core-item feeder like
  Dessecus, rank-1 and unflagged — OUT (not companion content).

None of the eight carries a rank flag or rare role; none drops an item
starting a Horde quest. The terraces contribute zero companion steps —
stated, not silent.

## Treasures — 3 generic loops, same set as Alliance

One loop step per object over ALL data-confirmed points, said plainly
(51 fixed points total):

- 4149 Solid Chest: 10 pts (23.48,58.82 / 25.36,66.86 / 31.61,67.61 /
  32.1,58.75 / 32.19,75.75 / 37.23,72.06 / 40.15,66.24 / 41.24,59.38 /
  47.46,69.05 / 49.26,68.63). Usual chest fare, nothing unique.
- 153451 Solid Chest: 20 pts (45.37,39.79 / 50.26,53.3 / 53.11,38.56 /
  57.39,63.42 / 57.47,42.26 / 58.34,67.14 / 58.43,72.84 / 60.87,68.11 /
  60.89,64.53 / 62.07,65.12 / 63.39,73.41 / 63.9,83.58 / 64.26,64.94 /
  65,70.99 / 66.49,44.59 / 67.53,79.92 / 67.64,66.71 / 67.67,77.32 /
  68.25,73.36 / 71.1,48.82). Usual chest fare, nothing unique.
- 153470 Food Crate: 21 pts (10.69,49.53 / 13.44,43.4 / 13.45,54.02 /
  13.99,41.97 / 14.22,44.18 / 14.42,42.25 / 16.33,47.77 / 23.05,58.86 /
  26.96,48.82 / 31.92,58.18 / 32.57,43.01 / 33.19,47.99 / 45.54,38.72 /
  50.21,52.8 / 53.28,39.43 / 57.26,42.6 / 67.95,66.43 / 68.64,71.77 /
  73.36,52.56 / 77.53,84 / 78.77,67.53). No contents listed in the
  data; shipped interact-only with that said plainly.

Excluded quest-owned/linked (with reason, verified against quests.json
in this build):

- 2556 Cortello's Treasure (1 pt): end-object of 626 Cortello's Riddle,
  contracted in the Swamp core - core-owned, not companion content.
- 142702-142714 Venom Bottles (14 pts, two west-den clusters):
  start-objects of Horde-core 2933 - core furniture, not treasure.
- 142127 Rin'ji's Secret: start-object of Horde-core 2782 - core
  furniture (the 142036 Rin'ji's Cage beside it has no quest refs and
  no contents - logged, not shipped).
- 179908 Slagtree's Lost Tools (5 pts): objective-item source of
  Horde-core 7839 - core furniture.
- 179910 Lard's Picnic Basket: sits on core 7840's ground
  (Kidnapper/table point) but has NO quest refs and no contents in the
  data - logged to companion-unverified, not shipped, with the
  Lard-name note (same placement as Alliance).
- 179912 Aerie Peak Town Center: event-location object - scenery.
- 179913 Call to Arms!: start-object of Horde-core 7861/7862 - core
  furniture.
- 179914 Pile of Bones / 179915 Pile of Skulls: objective sources of
  Horde-core 7849 - core furniture.
- 179922 Vessel of Tainted Blood (24 pts): objective source of
  Horde-core 7850 - core furniture.
- 179914/179915/179922 are Horde-core ground; the Alliance doc excluded
  179922 already and logged the rest elsewhere - same outcome here.
- 142180 Jintha'Alor Alter: encounter site of core-contracted 1446
  (Jammal'an the Prophet, turn-in at Atal'ai Exile 5598) -
  core-adjacent, excluded.
- 144066/144067/144068 Witherbark Cages + 144070 Sharpbeak's Cage:
  objects of 2988 Witherbark Cages / 2994 Saving Sharpbeak
  (Hillsbrad-accept, uncontracted) - out-of-zone quest objects.
- 144071/144072/144073 Highvale Records/Notes/Report: objects of 2995
  Lines of Communication (zone 1458), uncontracted - excluded.
- 153239 Wildkin Feather (24 pts): gives item 10819, objective of 3661
  (Teldrassil-accept, uncontracted) - quest-item source for an
  uncontracted quest, excluded.
- 175889 Ancient Egg: gives item 12402, objective of 4787 The Ancient
  Egg (Tanaris-accept 1441, uncontracted) - excluded.
- 2558 Test (1 pt): objective of 92867 (out-of-zone record) - test
  object, excluded.
- 181073 Fragrant Cauldron: start/end object of 9029 A Bubbling
  Cauldron (seasonal event) - seasonal quest furniture, excluded.
- Dwarven Fire 22223/61037/61038/61039 + 181301/181302/181305 Camp +
  181345 Flame of the Hinterlands + 181605 Ribbon Pole + 16606/16781
  Midsummer pair: seasonal Midsummer objects - excluded by the seasonal
  rule, nothing shipped.
- 177224 Troll Drum Sound Object: sound object, no loot, no quest refs
  - scenery, excluded by class.
- 50937 Sack of Rye / 2653 Lesser Bloodstone Deposit / 2068
  Pupellyverbos Port / 441140 Humming Box / 441141 Dreampearl /
  441252 Book / 442397+442398 Treasure of the Bat / 441946 Shrine of
  the Moon / 445042 Extraplanar Eye / 142716 Shadra'Alor Altar /
  142698/142700 Witherbark Village + Spell Focus / 142191 Horde Supply
  Crate / 181645 Gryphon Egg / 181643 Featherbeard's Remains / 181649
  Featherbeard's Journal / 142036 Rin'ji's Cage / 18047-18062 nameless
  cluster (16 singles, Witherbark village ground, no refs): logged to
  docs/companion-unverified.md (present, no loot evidence to build a
  step from), not shipped. 142191 gives food items plus 8684
  (Horde-core 77's objective) but no quest references the crate itself
  - name and contents alone do not make it shippable; the core guide
  farms 8684 off the Venom Bottle objects.

Gathering/profession nodes and furniture are not treasures (excluded by
class, no per-item logging): all veins/deposits, all herbs (Liferoot,
Fadeleaf, Khadgar's Whisker, Stranglekelp, Goldthorn, Violet Tragan,
Purple Lotus, Sungrass, Ghost Mushroom, Golden Sansam, Star Lotus),
campfires/bonfires/braziers/forges/anvils/chairs/stools/MFF decor,
fishing objects, Smoked Meat Racks, 144011 Mailbox.

## RECIPES — shipped (7 vendor buys + 7 drop collects)

Profession tags follow the item-name convention (Recipe:+potion/drink ->
Alchemy/Cooking, Pattern: -> Tailoring/Leatherworking, Plans: ->
Blacksmithing, Schematic: -> Engineering, Formula: -> Enchanting); the
two ambiguous Forever-custom names are called out below.

Vendor-sold (buy at the named 1425-spawn vendor; stock class unconfirmed):

- Leatherworking 7613 Pattern: Green Leather Armor - 2698 George
  Candarte (Horde, in-zone @7.9,73.3; also sold by 2679 Wenna
  Silkbeard, Alliance, Wetlands 1437). HEADLINE DELTA, both directions:
  the Alliance inventory excluded this as Horde-only (Alterac
  precedent) - for the Horde round George is a live in-zone source and
  it SHIPS here. Logged, not harmonized.
- Engineering 7742 Schematic: Gnomish Cloaking Device - 6777 Zan
  Shivsproket (AH/neutral, @1.3,56.9), SOLE vendor anywhere. Same as
  Alliance - no delta.
- Engineering 10609 Schematic: Mithril Mechanical Dragonling - 2688
  Ruppo Zipcoil (AH/neutral, @34.33,37.76, 1425-only), SOLE vendor.
  Same as Alliance - no delta.
- Leatherworking 15735 Pattern: Ironfeather Shoulders - 12958 Gigget
  Zipcoil (AH/neutral, @34.46,38.59), SOLE vendor. Same as Alliance -
  no delta.
- Enchanting 18160 Recipe: Thistle Tea - 6779 Smudge Thunderwood
  (AH/neutral, @1.4,56.6), SOLE vendor. Same as Alliance (their
  profession tag: Enchanting by the tea/consumable convention -
  kept, disclosed). No delta.
- Cooking 21099 Recipe: Smoked Sagefish + 21219 Recipe: Sagefish
  Delight - 14738 Otho Moji'ko (HORDE, Revantusk @79.38,79.08) and
  270780 Qujo (neutral, Revantusk @77.95,77.83). Both are 24-vendor
  generic cooking stock; shipped via the Revantusk pair per the
  Barrens/Alterac vendor precedent, with that said plainly. HEADLINE
  DELTA: the Horde round buys its sagefish recipes at its own hub
  instead of only Qujo - same items, Horde-pinned lines.
- Cooking 16110? not in-zone Horde... see excluded (Truk is
  Alliance-faction; no Horde in-zone vendor) - genuine Horde gap,
  stated in the guide.

Dropped (collect at the in-zone dropper; each sole 1425-only dropper):

- Leatherworking 15760 Pattern: Ironfeather Breastplate - SOLE dropper
  2644 Vilebranch Hideskinner (15 pts, terraces) - SHIPPED.
- Enchanting 16214 Formula: Enchant Bracer - Greater Intellect - SOLE
  dropper 2642 Vilebranch Shadowcaster (8 pts) - SHIPPED.
- Alchemy 250992 Recipe: Superior Mender's Potion - SOLE dropper 2640
  Vilebranch Witch Doctor (9 pts) - SHIPPED (profession by the
  Recipe:+potion convention; disclosed, not data-flagged).
- Blacksmithing 251396 Plans: Shining Mithril Pants - SOLE dropper 2653
  Witherbark Sadist (20 pts) - SHIPPED.
- Tailoring 254078 Pattern: Earthenweave Cord - SOLE dropper 4467
  Vilebranch Soothsayer (22 pts) - SHIPPED (profession by the
  weave/cloth convention; disclosed, not data-flagged).
- Engineering 264218 Schematic: EZ-Thro Tru-Trigger - SOLE dropper 2656
  Jade Ooze (24 pts) - SHIPPED.
- Alchemy 9294 Recipe: Wildvine Potion - 27 in-zone droppers (3 zones
  total: 1417/1425/1434 - narrow, not a dozens-of-zones world drop, same
  call as Alliance): SHIPPED riding a collect on each of the six
  narrow-drop steps above (2644/2642/2640/2653/4467 all drop it) plus
  a note on the four rare steps that drop it (8216/8217/8218/8219).

Excluded (with reason):

- Wildhammer (Alliance)-only in-zone (3, each with the off-zone Horde
  vendor named): 8409 Pattern: Nightscape Shoulders (Nioma A in-zone;
  Horde buys from 7854 Jangdor Swiftstrider, Un'Goro 1444);
  7995 Plans: Mithril Scale Bracers (Harggan A in-zone; Horde buys
  from 8176 Gharash, Swamp 1435); 18046 Recipe: Tender Wolf Steak
  (Truk Wildbeard A in-zone; Horde buys from neutral 7733/8125,
  Tanaris 1446, or 255894, zone 2548). Genuine in-zone Horde gaps -
  each stated in the guide.
- 7613 via 2679 Wenna Silkbeard (Alliance, Wetlands) - not needed;
  George covers the Horde in-zone.
- Every other 1425-dropping recipe (~150 items: 3395, 7975, 7989,
  7990, 7992, 10315, 15731, 15737, 15745 and the rest): multi-zone
  generic world drops per the Elwynn rule - not zone content.
- Quest-reward recipes: unverifiable (quest records carry no reward
  data) - none shipped, none nameable from data.
- Trainer-taught staples: out of scope per the pack rule.
- Fishing and First Aid have NO Hinterlands Horde source in the data -
  stated in the guide, not padded.
