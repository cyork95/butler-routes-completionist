# Arathi Highlands (Horde) companions inventory

Scope: accept-zone key **1417**, Horde core band **30-40**, faction **Horde**.
Built from the local data dumps (`upstream-polestar/data/forever/*.json`:
`npcs.json`, `objects.json`, `items.json`, `quests.json`) — game data wins
over the Alliance inventory (`docs/arathi-companions-inventory.md`) wherever
they differ; every delta is flagged inline.

The Horde core contract is 29 quests (`docs/arathi-horde-census.md`):
677/678 kill Witherbark Axe Thrower 2554, Headhunter 2556, Witch Doctor 2555
and Boulderfist Brute 2566, Magus 2567; 639-646 run the sigil chain through
Trollbane's Tomb 2703; 94212 is the sourceless writ; 92707 has no start record.

## Rares — shipped (10)

Rare basis in this build: `rank` 2/4 **plus** a `roles: ["rare"]` flag.
All ten below carry the flag; levels from the data; all points are key-1417
spawns. Loot in this build is a flat generic-green table by dropper-count —
**none of the ten has a sole-dropper signature item**, so the rares guide
ships kills with no `collect` goals (same loot semantics as the Alliance
finding, verified in this build by reverse-indexing every item drop record).

| Rare | NPC ID | Lvl | Spawns (1417) | Treatment |
|---|---|---|---|---|
| Darbel Montrose | 2598 | 39 | 14 pts, ogre mound west [25-30, 60-66] | loop, in-band |
| Singer | 2600 | 34 | 1 pt [32.31, 30.99] | single goto, in-band |
| Foulbelly | 2601 | 42 | 4 pts, ogre grounds SW [18-21, 66-69] | loop, ABOVE band — come-back-later note |
| Ruul Onestone | 2602 | 39 | 1 pt [17.96, 68.56] | single goto, in-band |
| Kovork | 2603 | 36 | 3 pts, mid-zone [30-33, 43-46] | loop, in-band |
| Molok the Crusher | 2604 | 39 | 3 pts, ogre mound south [53-55, 79-82] | loop, in-band |
| Zalas Witherbark | 2605 | 40 | 10 pts, Witherbark village east [61-70, 72-82] | loop, in-band (top edge) |
| Nimar the Slayer | 2606 | 37 | 15 pts, east basin [60-74, 61-75] | loop, in-band |
| Geomancer Flintdagger | 2609 | 40 | 1 pt [82.8, 32.23] | single goto, in-band |
| Prince Nazjak | 2779 | 41 | 24 pts, naga shore NE [19-24, 82-90] | loop, ABOVE band — come-back-later note |

No core overlap: none of the ten is a target of any Horde-contracted quest.
Faction: all ten are faction-null (hostile to both) — engageable by Horde.
None drops a Horde-core quest starter (the core's only item-start, 94212, is
sourceless; 92707 has no start record) — see "Item-start hunts" below.

## Rares — excluded (with reasons)

- Witherbark Axe Thrower 2554 / Headhunter 2556 / Boulderfist Brute 2566:
  **no rare flag in this build** (rank None, no rare role) AND kill targets of
  core-contracted 677/678 — not companion content (Dun Morogh precedent).
  DELTA vs the Alliance inventory, which shipped these three as its rare loop:
  the flag basis does not hold in this build.
- "Falthis": the 2574 record in this build is **Drywhisker Digger** (lvl 36-37,
  faction null, no rare flag) — "Falthis" exists nowhere in the data. Not a
  rare; excluded as unflagged.
- "Barash": the 2549 record is **Garr Salthoof** (lvl 41-43) spawning **only
  on key 1434 (Stranglethorn)** — not in Arathi at all in this build.
- Lo'Grosh 2453: spawns keyed **1416 (Alterac)** [47.52,32.31],[52.09,46.94],
  none on 1417 — not Arathi content in this build; not duplicated here.
  (Whether the Alterac guides cover it is Butler's call.)
- Flamescale Drake 2472: loot confirmed but **zero spawn points anywhere** in
  the data — no writable step; logged to `docs/companion-unverified.md`.
- Bliztik 2481: spawns on **key 1431 (Duskwood)** — Duskwood content, not here.
- Nimboya 2497: spawns on **key 1434 (Stranglethorn)** — STV content, not here.
- NPCs 2576 / 211016 (the Alliance doc's "Forsaken Assassin / Courier"):
  **records absent from this build's npc table** — not in data.
- Tamra Stormpike 14275 (lvl 28, rank 2, rare role, faction 'A', 3 pts on
  1417): Alliance-faction — excluded for Horde (Falthis rule).
- Needletooth 217836 (lvl 35, rank 4, **no rare role**, 24 pts on 1417,
  custom wolf model): quest-lookalike ruling stands — excluded, with reason.

## Tameables

**No tame lines ship.** None of the ten rares has drop evidence of a
tameable-beast kind (flat generic loot, no exclusive pet/beast drops) and
there is no core-guide beast-family corroboration (the core kills
troll/ogre humanoids, not beasts). Tameability has no data flag — the open
question is logged to `docs/companion-unverified.md`, never guessed.

## Item-start hunts

**None ship, and why:** the Horde census found exactly one Horde-mask
item-start (94212, writ item 264012 — **sourceless**, no placed dropper
anywhere: the core carries it as a bag note) and 92707 has no start record
at all. There is no writable in-zone hunt for either (Baron Aquanis shape).
Stated in the rares guide so the absence is deliberate, not an omission.

## Treasures — shipped

| Object | ID | Points (1417) | Treatment |
|---|---|---|---|
| Solid Chest | 2855 | 9 pts (west + east clusters) | one loop step |
| Solid Chest | 2857 | 18 pts (NE coast + Stromgarde clusters) | one loop step (distinct object and distinct points from 2855) |
| Solid Chest | 153451 | 1 pt [88, 22.7] | single goto + note |
| Barrel of Melon Juice 3659 + Food Crate 3695 | — | 2 shared pts, Hammerfall [8.7,47.6],[10.2,50.5] | small loop step |
| Barrel of Sweet Nectar 3706 + Food Crate 3707 | — | 24 shared pts, zone-wide | one loop step |
| Horde Chest | 105578 | 3 pts, Hammerfall [60.11,55.91],[60.18,58.71],[62.72,56.43] | loop step |
| Illari's Loot Cache | 418855 | 1 pt [94.15, 69.28] | single goto + note: end-object of the nameless, objective-less STV record 79242 (uncontracted, broken) — contents unconfirmed. DELTA vs Alliance ("no quest refs"): the ref exists but is not Arathi content. |
| Trelane's Chest 2716 + Lockbox 2718 | — | 1 pt each [18.17,69.15],[18.03,67.87] (Stromgarde west) | one loop over the pair + note: unreferenced in this build (their neighbour Footlocker 2717 is quest-owned out-of-zone, not here) — contents unconfirmed |

All shipped treasure objects are lootable world objects with no quest link
to either Arathi contract; contents unconfirmed in data — said plainly.

## Treasures — excluded (with reasons)

All IDs below verified against this build's quest table (several Alliance-doc
IDs proved stale — e.g. its "Satchel of the Dabbler 142978" is a Campfire
here, its "Sealed Barrel 142076" does not exist, and its Trelane/linked
quest IDs reference nothing on these objects).

- Alliance Chest 4096 (3 pts) / 105579 (4 pts) / 105581 (4 pts): Alliance-only
  (Witherbark + Stromgarde Alliance camps) — a Horde player cannot use them.
- Cache of Explosives 2704: destroy-objective of Alliance 633 (Wetlands).
- Shards of Myzrael 2705: furniture of Alliance 647 + Alliance 98071.
- Shards of Myzrael 138492: end-object of shared 635/642 (main guide) and
  Badlands 656 — main/other-guide content, not Horde-Arathi.
- Iridescent Shards 2701: furniture of shared 642/651 (main guide) + Swamp
  legs — not Horde-Arathi content.
- Stones of Binding 2690/2691/2702 + Spell Focus 103660 + Book 2695: 2690
  and 103660 unreferenced; 2691 (East Binding) ends Hinterlands-Horde 7841;
  2695 (Book) ends Ironforge-Alliance 637/683; 2702 (Inner Binding) is
  shared-Myzrael furniture (651/652 main guide + Swamp legs) — none is
  Horde-Arathi content.
- Trollbane's Tomb 2703: turn-in/accept object of Horde-core 645/646.
- Keystone 2688: start-object of the Myzrael chain (Horde 688, shared 652,
  Alliance 653) — core/main-guide furniture.
- Charging Stone 2711 / Calcified Elven Gem 2712 / Wanted Board 2713:
  furniture of the Alliance Arathi chain (657-661, 684/685) — Alliance
  content.
- Spirit of Silverpine Charts 2708 + Log 2710: furniture of Alliance 690/697.
- Messenger Bag 406918 + Hastily Rolled-Up Satchel 424006: furniture of the
  uncontracted 1417 chain 79976 (null-mask, starts at the Bag, ends at the
  Satchel; its pre-link 79975 is the main guide's intentional non-contract
  turn-in) — someone else's quest furniture, not treasure. Census
  consideration for Butler, not this round.
- Scrolls 423897: start-object of uncontracted Undercity record 79949 —
  someone else's quest furniture, not treasure.
- Trelane's Footlocker 2717: referenced by out-of-zone quests (zone-232
  records 6642-46, Searing Gorge 7848, Silverpine 8578) — not Arathi content.
  (Its neighbours 2716/2718 are unreferenced and ship above.)
- Ebenezer Rustlocke's Corpse 2652: furniture of Alliance 631/632 plus
  zone-2652 (Shen'dralas) records — not Horde-Arathi content.
- Waterlogged Letter 2656: furniture of Hinterlands-Alliance 2877.
- Bottle 2687: furniture of STV-Alliance 97420.
- Syndicate Footlocker 423466: record is **empty in this build** (no name,
  no spawns) — examined, not shippable. DELTA vs Alliance (placed furniture
  of 96784): no quest in this build references it either.
- Yellow aura column 2870: furniture of Feralas-Alliance 2869/2870/2871.
- Floating Sparkles 2722: furniture of Stormwind-Alliance 332.
- Seasonal/event objects (Hallow's End pumpkins 180405-07, ghosts 180411-12,
  candy/skulls/bats 180425-27/180471-72, apples 180523): all carry 1417
  spawns but are excluded by the seasonal rule — nothing seasonal ships.
- Gathering nodes (herbs/veins), fishing schools, signposts/plaques,
  campfires/bonfires, furniture (chairs, tables, anvils, forges, looms),
  cannons, and display objects (Cauldron 103772, Grave 424267, Smoked Meat
  Rack 142979, Jintha'Alor Alter 142180, Runed Pedestal 2715, Ancient Egg
  175889, memorials 181062-67, Bolt Charged Bramble 103662, nameless 103773):
  scenery or profession nodes — never companion content.

## Recipes — shipped (16: 9 vendor + 7 drop)

Item records carry no profession field — professions assigned by the pack's
settled item-name convention (Recipe = Cooking, Pattern = cloth/leather wear,
Formula = Enchanting, Plans = Blacksmithing, Manual = Alchemy/First Aid by
name, Schematic = Engineering), stated per item below.

Vendor-sold (in-zone Horde vendors; buy lines pin the vendor by NPC ID):

| Item | Profession | Vendor (1417 point) |
|---|---|---|
| 3682 Recipe: Curiously Tasty Omelet | Cooking | Keena 2821 @74.09,32.73 (Hammerfall) |
| 12228 Recipe: Roast Raptor | Cooking | Keena 2821 @74.09,32.73 |
| 5973 Pattern: Barbaric Leggings | Leatherworking | Keena 2821 @74.09,32.73 (also on Alliance Hammon — Horde buys here) |
| 11163 Formula: Enchant Bracer - Lesser Deflection | Enchanting | Keena 2821 @74.09,32.73 |
| 7089 Pattern: Azure Silk Cloak | Tailoring | Jun'ha 6574 @72.69,36.45 (Hammerfall) |
| 253665 Pattern: Linen Reagent Bag | Tailoring | Jun'ha 6574 @72.69,36.45 |
| 253668 Pattern: Woolen Reagent Bag | Tailoring | Jun'ha 6574 @72.69,36.45 |
| 7613 Pattern: Green Leather Armor | Tailoring | George Candarte 2698 @28.1,11.8 (Stromgarde) |
| 13287 Pattern: Raptor Hide Harness | Leatherworking | Tunkk 2819 @74.84,34.59 (Hammerfall; SOLE vendor anywhere in data) |

Narrow drops (dropper spawns on 1417; each dropper family tight/in-zone):

| Item | Profession | Dropper (1417 spawn) |
|---|---|---|
| 249487 Formula: Twisted Nether Wand | Enchanting | Boulderfist Magus 2567 (9 pts, ogre mound) |
| 251335 Plans: Sterling Silver Boots | Blacksmithing | Syndicate Watchman 2261 (1 pt [19,20] — in-zone but lvl 20: below-band note) |
| 251386 Plans: Hard Gold Boots | Blacksmithing | Syndicate Highwayman 2586 (23 pts) + Smuggler 267065 (24 pts, Stromgarde surrounds) |
| 251393 Plans: Shining Mithril Pauldrons | Blacksmithing | Daggerspine Sorceress 2596 (8 pts, naga shore) |
| 254014 Pattern: Earthen Silk Slippers | Tailoring | Witherbark Troll 2552 (5 pts) |
| 255723 Manual: Greater Healing Potion | Alchemy | Syndicate Mercenary 2589 (14 pts) |
| 264212 Schematic: EZ-Thro Bronze Mortar | Engineering | Boulderfist Shaman 2570 (12 pts) |

No-source notes for the guide: **First Aid** (Refuge Deneb Walker is
Alliance-only — Horde has no in-zone source) and **Fishing** (none in-zone).
Blacksmithing HAS in-zone sources (3 narrow plans above) — no no-source note.

## Recipes — excluded (with reasons)

- Alliance-vendor-only (6): 10858 Plans: Solid Iron Maul (Jannos Ironwill);
  5973/12228 dupes on Hammon Karwn (Horde buys both from Keena); 6056 Recipe:
  Frost Protection Potion (Drovnar Strongbrew); 4609 Recipe: Barbecued
  Buzzard Wing (Narj Deepslice); 13288 Pattern: Raptor Hide Belt (Androd
  Fadran — SOLE vendor anywhere: genuine Horde gap, stated in the guide);
  16112/16113 Manuals: Heavy/Mageweave Bandage (Deneb Walker — Horde has no
  First Aid source in-zone).
- 5789 Pattern: Murloc Scale Bracers: **no in-zone dropper in this build**
  (Blackwater Deckhand 2636 spawns only on 1434; Bloodsail Raider on 1434;
  vendors 2846/4897 are out-of-zone) — DELTA vs the Alliance inventory, which
  recorded a 1417 Deckhand source. Not zone content here.
- ~750 recipe items dropping across dozens of zones: generic world drops, not
  zone content (Elwynn rule) — unlisted individually.
- Quest-reward recipes: unverifiable (no reward data in quest records) —
  never shipped (Zephras finding).
- Trainer-taught staples: out of scope per the pack rule.
