# Hinterlands companions inventory (pack butler-routes-completionist)

Source: local Forever game data (questie-forever npcs/objects/items/quests.json),
built with `--product wowf` + QuestieDB. Accept-zone key **1425**, core band
**38-51**, Alliance route. The core contract (14 quests) is untouched by this
inventory. Game data wins over community sources throughout.

## RARES - 10 rare-flagged NPCs on 1425, all 10 shipped (9 in-band + 1 CBL)

Rank semantics per the Badlands calibration: rank 4 = Rare, rank 2 = Rare Elite.
Every point below is the data's spawn point verbatim. Signature = the item's
sole dropper anywhere in the data (drops.npc lists only this NPC).

| NPC | lvl | points (map 1425 unless noted) | signature (sole drop) | disposition |
|-----|-----|--------------------------------|------------------------|-------------|
| 8210 Razortalon | 44 | 1: 37.06,45.33 | 283545 Moonchaser's Headdress | SHIP single-goto + collect |
| 8211 Old Cliff Jumper | 42 | 2: 1425 (11.92,53.7) + 1424 (96.9,14.6) | none (wolf meat/paw/mane, all shared) | SHIP 2-pt loop, kill-only |
| 8212 The Reak | 49 | 1: 58.88,43.12 | 284043 Dissolved Link Legguards | SHIP single-goto + collect |
| 8213 Ironback | 51 | 1: 81.48,49.19 | none (turtle meat/scale/shell, all shared) | SHIP single-goto, kill-only |
| 8214 Jalinde Summerdrake | 49 | 1: 30.25,47.95 | 284050 High Elf's Recurve | SHIP single-goto + collect |
| 8215 Grimungous | 50 Rare Elite | 1: 70.19,55.38 | 284064 Cliffbreaker's Pauldrons | SHIP single-goto + collect |
| 8216 Retherokk the Berserker | 48 | 1: 50.54,64.13 | 284061 Berserker's Wraps | SHIP single-goto + collect |
| 8217 Mith'rethis the Enchanter | 52 Rare Elite | 1: 63.86,77.61 | 17050 Chan's Imperial Robes | SHIP single-goto + collect + CBL note |
| 8218 Witherheart the Stalker | 45 | 1: 33.12,70.29 | 284046 Witherheart's Stabber | SHIP single-goto + collect |
| 8219 Zul'arek Hatefowler | 43 | 1: 32.42,56.9 | 284063 Witherbark Hatecleaver | SHIP single-goto + collect |

Notes applied in the guide:
- Retherokk, Witherheart and Zul'arek also drop 9259 Troll Tribal
  Necklace, the objective item of core-contracted 2880/2881 (Troll Necklace
  Bounty) - the steps carry a note pointing at the core guide and never
  accept. Mith'rethis drops it too; his step carries the same note.
- Razortalon, Jalinde, Mith'rethis and Zul'arek drop 8704
  OOX-09/HL Distress Beacon, the starter of core-contracted 485
  (Find OOX-09/HL!) - noted, never accepted in the companion.
- Retherokk, Witherheart, Zul'arek and Mith'rethis drop 9294 Recipe:
  Wildvine Potion - the recipes companion owns that hunt; cross-noted.
- Jalinde Summerdrake is faction=A (Alliance-aligned). She is shipped like
  any other rare: the data flags her rare with loot, and the guide takes no
  position on whether to attack beyond stating the alignment.
- Mith'rethis (52) is 1 level above the band top: shipped with an honest
  come-back-later note (Westfall/Hillsbrad precedent). Nothing is
  far-above-band, so nothing is excluded on level.
- No rare here is a giver, ender or objective of any core-contracted quest,
  so the Dun Morogh exclusion does not fire on any of the 10.
- TAME: no tame lines ship. The data has no tameability flag. Old Cliff
  Jumper (wolf: Red Wolf Meat / Tender Wolf Meat) and Ironback (turtle:
  Turtle Meat) have beast-drop evidence, but the core guide never sends the
  player at wolves or turtles (core kills are sludges, Witherbark trolls,
  Soothsayers, rocs, bears, apes, Skylord) - no corroboration. Razortalon
  has bird-drop evidence (Giant Egg, feathers) and the core has an optional
  roc kill (2659 Razorbeak Skylord), but the family link is unverifiable
  from the data. All three logged in docs/companion-unverified.md.
- Respawn timers are unconfirmed in the data - none stated.

Excluded lookalikes: 221310-221313 (Ysondre, Lethon, Emeriss, Taerar),
level 63 rank-3 Dragons of Nightmare spawning on 4 zones (1425/1431/1440/
1444). Not rare-flagged, world-boss rank, far above band - not companion
content, with reason.

## TREASURES

Generic fixed containers (ONE loop step, said plainly - 51 fixed points):
- 4149 Solid Chest: 10 pts (23.48,58.82 / 25.36,66.86 / 31.61,67.61 /
  32.1,58.75 / 32.19,75.75 / 37.23,72.06 / 40.15,66.24 / 41.24,59.38 /
  47.46,69.05 / 49.26,68.63). Data lists 201 contents (ordinary greens;
  may also hold generic world-drop recipes, which are not zone content).
- 153451 Solid Chest: 20 pts (45.37,39.79 / 50.26,53.3 / 53.11,38.56 /
  57.39,63.42 / 57.47,42.26 / 58.34,67.14 / 58.43,72.84 / 60.87,68.11 /
  60.89,64.53 / 62.07,65.12 / 63.39,73.41 / 63.9,83.58 / 64.26,64.94 /
  65,70.99 / 66.49,44.59 / 67.53,79.92 / 67.64,66.71 / 67.67,77.32 /
  68.25,73.36 / 71.1,48.82). Data lists 157 contents (same ordinary fare).
- 153470 Food Crate: 21 pts (10.69,49.53 / 13.44,43.4 / 13.45,54.02 /
  13.99,41.97 / 14.22,44.18 / 14.42,42.25 / 16.33,47.77 / 23.05,58.86 /
  26.96,48.82 / 31.92,58.18 / 32.57,43.01 / 33.19,47.99 / 45.54,38.72 /
  50.21,52.8 / 53.28,39.43 / 57.26,42.6 / 67.95,66.43 / 68.64,71.77 /
  73.36,52.56 / 77.53,84 / 78.77,67.53). No contents listed in the data;
  shipped as interact-only with that said plainly.

Excluded quest-owned/linked (with reason, verified against quests.json):
- 2556 Cortello's Treasure (1 pt): end-object of 626 Cortello's Riddle,
  contracted in the Swamp core - core-owned, not companion content.
  (677 Call to Arms does NOT reference this object; its objectives kill
  NPCs 2554-2556, a numeric collision across entity types.)
- 144066/144067/144068 Witherbark Cages + 144070 Sharpbeak's Cage: objects
  of 2988 Witherbark Cages / 2994 Saving Sharpbeak, both Hillsbrad-accept
  and uncontracted - out-of-contract quest objects, excluded.
- 144071/144072/144073 Highvale Records/Notes/Report: objects of 2995
  Lines of Communication (zone 1458), uncontracted - excluded.
- 179913 Call to Arms: objective of Horde-only 7861/7862 - excluded.
- 142180 Jintha'Alor Alter: no loot contents; encounter site of
  core-contracted 1446 (Jammal'an the Prophet, turn-in at Atal'ai Exile
  5598) - core-adjacent, excluded.
- 50937 Sack of Rye: gives item 740, objective of 92470 Foul Matriarch
  (custom zone 2521), uncontracted - excluded.
- 2653 Lesser Bloodstone Deposit: gives 4278 Lesser Bloodstone Ore,
  objective of 92102/93567/94533/94535/94679/96558 (zones 1441/2482/
  2548), all uncontracted - excluded.
- 153239 Wildkin Feather (91 pts): gives item 10819, objective item of
  3661 Favored of Elune? (Teldrassil-accept, minLevel 42, uncontracted) -
  quest-item source for an uncontracted quest, excluded.
- 175889 Ancient Egg: gives item 12402, objective of 4787 The Ancient Egg
  (Tanaris-accept 1446, uncontracted) - excluded.
- 179908 Slagtree's Lost Tools: gives item 19033, objective of Horde-only
  7839 Vilebranch Hooligans - excluded.
- 179922 Vessel of Tainted Blood (69 pts): gives item 19071, objective of
  Horde-only 7850 Dark Vessels - excluded.

Logged to docs/companion-unverified.md (present in data, no loot evidence
to build a step from): 181645 Gryphon Egg (22 pts, no contents, no quest
links - NOT the source of 86620's eggs; the data sources those to missing
object 669115), 181643 Featherbeard's Remains, 181649 Featherbeard's
Journal, 442397/442398 Treasure of the Bat (same-spot pair, no contents),
441946 Shrine of the Moon, 445039 Extraplanar Eye, 441140 Humming Box
(4 pts), 441141 Dreampearl (2 pts), 142716 Shadra'Alor Altar, 142698/142700
Witherbark Village + Spell Focus, 142191 Horde Supply Crate (food contents
but no quest linkage; name suggests Horde flavor - not shippable on a
name), 179910 Lard's Picnic Basket (no contents, Horde-vendor
neighborhood), 441252 Book (no contents), 2068 Pupellyverbos Port (42 pts;
gives item 3900, referenced by quests in 6 other zones - the 452 Pyrewood
Ambush "link" is NPC 2068 Lord Mayor Morrison, a numeric collision, not
this object; purpose unknown).

Gathering/profession nodes and furniture are not treasures (excluded by
class, no per-item logging): all veins/deposits (324/1733/1734/1735/2040/
2047/439778), all herbs (1623/2041/2042/2043/2045/2046/141853 Violet Tragan/
142140/142142/142144/176583/439762), campfires/bonfires/braziers/forges/
anvils/mailbox/chairs/stools/MFF decor/fishing objects, 144011 Mailbox.

## RECIPES - 15 shipped (8 vendor buys + 7 drop collects)

Profession tags follow the item-name convention (Recipe:+potion/food/drink
-> Alchemy/Cooking, Pattern: -> Tailoring/Leatherworking, Plans: ->
Blacksmithing, Schematic: -> Engineering, Formula: -> Enchanting); the two
ambiguous Forever-custom names are called out below.

Vendor-sold (buy at the named 1425-spawn vendor; stock class unconfirmed):
- Leatherworking 15735 Pattern: Ironfeather Shoulders - 12958 Gigget
  Zipcoil (AH/neutral, 34.46,38.59), SOLE vendor anywhere in the data.
- Engineering 7742 Schematic: Gnomish Cloaking Device - 6777 Zan
  Shivsproket (AH/neutral, 1.3,56.9), SOLE vendor.
- Leatherworking 8409 Pattern: Nightscape Shoulders - 8160 Nioma
  (Alliance, 13.3,43.37; also sold by 7854 elsewhere).
- Blacksmithing 7995 Plans: Mithril Scale Bracers - 8161 Harggan
  (Alliance, 13.42,44.14; also sold by 8176 elsewhere).
- Engineering 10609 Schematic: Mithril Mechanical Dragonling - 2688 Ruppo
  Zipcoil (AH/neutral, 34.33,37.76, 1425-only), SOLE vendor.
- Cooking 18046 Recipe: Tender Wolf Steak - 4782 Truk Wildbeard
  (Alliance, 14.36,42.31; also sold by 7733/8125/255894).
- Cooking 18160 Recipe: Thistle Tea - 6779 Smudge Thunderwood
  (AH/neutral, 1.4,56.6), SOLE vendor.
- Cooking 21099 Recipe: Smoked Sagefish + 21219 Recipe: Sagefish Delight -
  270780 Qujo (faction null, 77.95,77.83). Both are 24-vendor generic
  cooking stock; shipped per the Barrens/Alterac precedent (vendor content
  is zone content even when widely sold), with that said plainly.

Dropped (collect at the in-zone dropper; each sole dropper is 1425-only):
- Alchemy 9294 Recipe: Wildvine Potion - 27 in-zone droppers (wildkin
  2639-2654, trolls 4465-4467, ogres 7809/7995/7996, keepers 10802, rares
  8216/8217/8218/8219) but only 3 zones in the whole data (1425/1434/
  1417): narrow, not a dozens-of-zones world drop - SHIPPED, riding the
  five spellcaster steps below plus a note on the four rare steps.
- Leatherworking 15760 Pattern: Ironfeather Breastplate - SOLE dropper
  2644 Vilebranch Hideskinner (48, 15 pts) - SHIPPED.
- Enchanting 16214 Formula: Enchant Bracer - Greater Intellect - SOLE
  dropper 2642 Vilebranch Shadowcaster (47, 8 pts) - SHIPPED.
- Alchemy 250992 Recipe: Superior Mender's Potion - SOLE dropper 2640
  Vilebranch Witch Doctor (46, 9 pts) - SHIPPED (profession by the
  Recipe:+potion convention; disclosed, not data-flagged).
- Blacksmithing 251396 Plans: Shining Mithril Pants - SOLE dropper 2653
  Witherbark Sadist (44, 20 pts) - SHIPPED.
- Tailoring 254078 Pattern: Earthenweave Cord - SOLE dropper 4467
  Vilebranch Soothsayer (46, 22 pts) - SHIPPED (profession by the
  weave/cloth convention; disclosed, not data-flagged).
- Engineering 264218 Schematic: EZ-Thro Tru-Trigger - SOLE dropper 2656
  Jade Ooze (47, 24 pts) - SHIPPED.

Excluded (with reason):
- 7613 Pattern: Green Leather Armor - only in-zone vendor is 2698 George
  Candarte (Horde). Alterac precedent: excluded.
- 21099/21219 via 14738 Otho Moji'ko (Horde) - excluded (shipped via
  neutral Qujo above instead).
- Every other 1425-dropping recipe (8387, 10320, 15737, 15757, 7990, 7992,
  3395 and ~150 more): 6-32 zones each, generic multi-zone world drops
  per the Elwynn rule - not zone content. 15760's fellow-drops on 2644
  (3395, 7975, 7989, 7990, 7992, ...) are all in this class.
- 15742 Pattern: Warbear Harness - no in-zone vendor (11557 sells it
  elsewhere) and its 1425 mob drops are a 20-zone generic - excluded.
- Quest-reward recipes: unverifiable (quest records carry no reward data)
  - none shipped, none nameable from data.
- Fishing and First Aid have NO Hinterlands source in the data - stated
  in the guide, not padded (Dun Morogh precedent).
