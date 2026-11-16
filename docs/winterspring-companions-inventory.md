# Winterspring companions inventory (pack butler-routes-completionist)

Source: local Forever game data (questie-forever npcs/objects/items/quests.json),
built with `--product wowf` + QuestieDB. Accept-zone key **1452**, core band
**47-60**, Alliance route. The core contract (48 quests) is untouched by this
inventory. Game data wins over community sources throughout.

## RARES - 7 rare-flagged NPCs on 1452 (rank 4 = Rare, rank 2 = Rare Elite),
all 7 shipped

No rare is a kill objective of any contract quest, and no rare drops a
contract quest-start item (the only contract item-start is 12842, the
Crudely-written Log, sole-dropped by non-rare High Chief Winterfall), so the
Dun Morogh exclusion does not fire. Signature = the item's SOLE dropper
anywhere in the data. Every point below is the data's spawn point verbatim.

| NPC | lvl | points (map 1452) | signature (sole drop) | disposition |
|-----|-----|-------------------|-----------------------|-------------|
| 10196 General Colbatann | 57, rank 2 | 3: 54.20,50.29 / 55.34,49.81 / 59.67,49.52 | none (all loot generic, 400+ droppers each) | SHIP 3-pt loop, kill-only |
| 10197 Mezzir the Howler | 55, rank 4 | 1: 45.03,37.37 | none (Wicked Claw is a 263-dropper generic) | SHIP single-goto, kill-only; wolf tame question logged |
| 10198 Kashoch the Reaver | 60, rank 2 | 1: 63.36,70.19 | none (all loot generic) | SHIP single-goto, kill-only (in-band top) |
| 10199 Grizzle Snowpaw | 59, rank 4 | 1: 66.90,35.60 | 284268 Furbolg Shaman's Girdle (sole, rate null) | SHIP single-goto + collect; furbolg (humanoid), no tame |
| 10200 Rak'shiri | 57, rank 4 | 1: 51.13,10.81 | none (Purification Potion is a 523-dropper generic) | SHIP single-goto, kill-only; cat tame question logged |
| 10201 Lady Hederine | 61, rank 2 | 1: 65.03,80.28 | none (all loot generic) | SHIP single-goto with come-back-later note (1 above band) |
| 10202 Azurous | 59, rank 4 | 1: 66.74,53.81 | 284261 Magically Fortified Legguards (sole, rate null) | SHIP single-goto + collect; draconic, no tame |

Tame-line basis: the data has no tameability flag. Mezzir (wolf) and Rak'shiri
(cat) are the only beast-shaped rares, but no contract quest kills wolves or
cats (contract kills: Winterfall furbolgs, Frostmaul, sprites, High Chief,
Lorax), so the required core-guide corroboration is absent - both tame
questions go to docs/companion-unverified.md, never guessed. The other five
show no beast evidence at all (humanoid/draconic names, generic humanoid
loot) and ship kill-only with no log entry.

No quest-target lookalikes carry the rare flag on 1452.

## TREASURES - fixed-spawn container objects on 1452

SHIPPED: Solid Chests - O153454 (12 pts: 29.27,46.90 / 30.50,35.71 /
33.09,36.69 / 39.66,43.13 / 41.51,42.52 / 46.02,35.97 / 53.02,40.48 /
55.84,44.69 / 66.36,35.89 / 66.64,37.06 / 67.63,35.28 / 68.08,36.70) plus
O153453 (1 pt: 71.30,81.90). One object name, fixed placements: ONE loop step
over all 13 points, said plainly in the guide.

EXCLUDED, each with reason:
- Mining veins (Small Thorium, Gold, Mithril, Truesilver, Rich Thorium) and
  herb nodes (Dreamfoil, Mountain Silversage, Icecap, Black Lotus): profession
  gathering nodes, never companion treasures (all rounds).
- Campfires / bonfires / benches / stoves / forges / anvils / mailboxes /
  skullpiles / necropolis / banners / ribbons / pumpkins / candy buckets /
  fire-traps / undead-fire auras / circles: decor, event dressing (Winter Veil,
  Midsummer, Hallow's End) or ambience with no container loot.
- Flight-point marker doodads (177131-177155 "Everlook", "Moonglade",
  "Felwood", "Kel'Theril", "Starfall Village", "Frostsaber Rock",
  "Mount Hyjal"): map markers, not containers.
- Core/soft-pre quest objects (no companion significance of their own):
  Frostmaul Shards (core 969), Moontouched Feather (soft-pre 978), Jaron's
  Wagon / Damaged Crate / Jaron's Supplies (core 4861-4864), Highborne Relic
  Fragments (core 5245), Runes of Mazthoril (core 4842 discovery), Elune
  altar/gem/light/aura/fire set (core 4901 discovery), Malyfous's Catalogue
  (core 5162), Water Elemental Rift (core 5163 mob-spawn area), Drop-Off
  Point / High Chief Cave-Mouth focus (core 5121/5123 area), Izzy's Holdings
  (core 92008 crate area), O463214 Book (starts Stormwind-contracted Ka-Boom
  84399 - a quest start, not loot), flavor books (457095 Elements for
  Dummies, 457098 Finding Your Inner Feline - readable lore, no loot), Stone
  of Shy-Rotam (103819/177684 - lore stone, no quest link and no container
  loot anywhere in the data).

## RECIPES - 23 shipped (13 vendor-sold, 10 zone-exclusive drops)

Vendor key: fac AH reads as both-factions neutral in this data (Evie, Qia,
Xizzer, Himmik all serve Alliance characters in Everlook). No stock-class
field exists in the data, so nothing is marked limited (Felwood Woolies
precedent: unconfirmed). Every buy line carries an npc pin to its in-zone
vendor.

| item | profession | source | disposition |
|------|------------|--------|-------------|
| 13480 Recipe: Major Healing Potion | Alchemy | Evie Whirlbrew 11188 @60.75,37.78 | SHIP buy npc 11188 |
| 14526 Pattern: Mooncloth | Tailoring | Evie Whirlbrew 11188 AND Qia 11189 @61.2,37.21 (both stock it) | SHIP buy at each vendor, cross-noted |
| 14468 Pattern: Runecloth Bag | Tailoring | Qia 11189 | SHIP buy npc 11189 |
| 14481 Pattern: Runecloth Gloves | Tailoring | Qia 11189 | SHIP buy npc 11189 |
| 15740 Pattern: Frostsaber Boots | Tailoring | Qia 11189 | SHIP buy npc 11189 |
| 16221 Formula: Enchant Chest - Major Health | Enchanting | Qia 11189 | SHIP buy npc 11189 |
| 16046 Schematic: Masterwork Target Dummy | Engineering | Xizzer Fizzbolt 11185 @60.8,38.6 (also sold by Kor'gar in Riverglades - in-zone source still counts) | SHIP buy npc 11185 |
| 16047 Schematic: Thorium Tube | Engineering | Xizzer Fizzbolt 11185 | SHIP buy npc 11185 |
| 16050 Schematic: Delicate Arcanite Converter | Engineering | Xizzer Fizzbolt 11185 | SHIP buy npc 11185 |
| 18652 Schematic: Gyrofreeze Ice Reflector | Engineering | Xizzer Fizzbolt 11185 | SHIP buy npc 11185 |
| 18656 Schematic: Powerful Seaforium Charge | Engineering | Xizzer Fizzbolt 11185 | SHIP buy npc 11185 |
| 16110 Recipe: Monster Omelet | Cooking | Himmik 11187 @61.33,39.16 (also sold by Malygen Felwood-A and Bale Darkshore-H - neutral recipe, in-zone source counts) | SHIP buy npc 11187 |
| 13495 Recipe: Greater Frost Protection Potion | Alchemy | SOLE dropper 7428 Frostmaul Giant @58.06,68.7 | SHIP collect at the giant |
| 13497 Recipe: Greater Arcane Protection Potion | Alchemy | SOLE dropper 7437 Cobalt Mageweaver @53.94,54.53 | SHIP collect at the mageweaver |
| 14493 Pattern: Robe of Winter Night | Tailoring | SOLE dropper 7437 Cobalt Mageweaver @53.94,54.53 | SHIP collect at the mageweaver |
| 16054 Schematic: Arcanite Dragonling | Engineering | SOLE dropper 7437 Cobalt Mageweaver @53.94,54.53 | SHIP collect at the mageweaver |
| 15747 Pattern: Frostsaber Leggings | Leatherworking | SOLE dropper 7440 Winterfall Den Watcher @30.34,36.33 (a core 5082 kill mob - the recipe, not the mob, is the content) | SHIP collect with the Den Watchers |
| 252890 Pattern: Blue Suede Hat | Leatherworking | SOLE dropper 7440 Winterfall Den Watcher @30.34,36.33 | SHIP collect with the Den Watchers |
| 15761 Pattern: Frostsaber Gloves | Leatherworking | SOLE dropper 7441 Winterfall Totemic @29.71,37 | SHIP collect with the Totemics |
| 15779 Pattern: Frostsaber Tunic | Leatherworking | SOLE dropper 7438 Winterfall Ursa @65.11,37.18 | SHIP collect with the Ursas |
| 16223 Formula: Enchant Weapon - Icy Chill | Enchanting | SOLE dropper 7524 Anguished Highborne @50.31,42.72 | SHIP collect with the Highborne |
| 250178 Recipe: Bear Bruscitti | Cooking | SOLE dropper 7446 Rabid Shardtooth @56.39,71.41 | SHIP collect with the Shardtooths |

Professions with NO in-zone source (Dun Morogh precedent - said plainly in the
guide, not padded): Blacksmithing, First Aid, Fishing.

EXCLUDED:
- Meilosh's 14 recipes (13484 Transmute Earth to Water, 15742/20253 Warbear
  Harness, 15754/20254 Warbear Woolies, 19202/19204 Heavy Timbermaw,
  19215/19218/19326/19327 Timbermaw patterns, 19445 Agility, 22392 2H
  Agility, 228982 Law of Nature): Meilosh (11557) is Felwood-contracted -
  his Timbermaw Hold home is the Felwood side (1448 [65.69,2.81]); his 1452
  point is the border-cave side of the same hold. No double-coverage: his
  stock belongs to the Felwood recipes companion (which currently carries
  only Woolies - the other 13 are flagged there as backfill, not here).
- Generic world drops (Elwynn rule): every other recipe with an in-zone
  dropper above drops from dozens to hundreds of mobs zone-wide (Mithril
  plans, Big Voodoo, Red Mageweave, Thorium/Radiant sets, Transmutes,
  Stoneshield, Frostweave/Runecloth/Brightcloth, Felcloth pieces) - not zone
  content, never shipped.
- Quest-reward recipes: UNVERIFIABLE - quest records carry no reward data.
  Plausible-but-unverifiable: the Lorax smithing chain (5124/5126/5127) may
  reward smithing recipes; not shipped, not asserted. Logged here and in
  docs/companion-unverified.md.
