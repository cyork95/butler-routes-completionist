# Ashenvale (Horde) companions inventory (pack 0.102.0)

Every entry shipped in the two Ashenvale (Horde) companion guides, one line each:
name, NPC/item id, source type, coordinates or vendor, and the data source
verified against. All coordinates are the client's own (live) map frame on map
1440 (Ashenvale). Game data is questie-forever npcs.json, items.json and
objects.json; quest linkage checked against the full quest table and the
35-quest Horde core contract (`ashenvale-horde.guide`, band 19-30, contract
`ashenvale-horde`). The data carries an explicit `rare` role flag; 13 Ashenvale
NPCs hold the flag (the same 13 the Alliance inventory found). Band cutoff: the
Horde core band is 19-30; level 30 is the top and is IN, anything above is OUT
unless the item-start hunt rule or the come-back-later precedent applies (argued
per rare below).

Vendor faction rule (flipped for Horde, Alterac precedent): recipes sold ONLY by
Alliance-faction vendors are excluded; Horde and neutral vendors are IN. Of the
9 vendor recipes on map 1440, 7 are sold only by Alliance-faction vendors
(Ulthaan 3960, Lardan 3958, Harklan Moongrove 3956, Harlown Darkweave 6731,
Dalria 3954) and are OUT; 2 are sold by Horde vendor Wik'Tar 12962 and are IN.

## ashenvale-horde-rares.guide — 11 rares + 4 item-start hunts + fixed containers

- Akkrilus | npc3773 | level 26 rare | single point (25.62, 63.54), southwest | no exclusive loot (Shredder Manual pages only, 5 zones); pure kill | source: npcs.json + items.json drops
- Terrowulf Packlord | npc3792 | level 32 rare (two above band — ships with an honest come-back-later note) | single point (49.77, 39.61), east of center | Ruffled Chaplet (item5753, Ashenvale-exclusive) + Wolfpack Medallion (item5754, Ashenvale-exclusive) as optional collects | source: npcs.json + items.json drops
- Lady Vespia | npc10559 | level 22 rare | loop over 2 northwest-shore points (9.87, 14.34), (13.63, 24.73) | Frostbitten Staff (item284704, Ashenvale-exclusive) as optional collect; Ring of Zoram (item5445) drops here and on Darkshore (2 zones, no collect — noted) | source: npcs.json + items.json drops
- Rorgish Jowl | npc10639 | level 25 rare | single point (35.82, 36.61), north | Den Guardian's Crusher (item284700, Ashenvale-exclusive) as optional collect | source: npcs.json + items.json drops
- Oakpaw | npc10640 | level 27 rare | single point (56.01, 62.75), southeast of center | no exclusive loot (Shredder Manual pages only, 5 zones); pure kill; tame question logged unverified (no beast loot drops, so no drop evidence) | source: npcs.json + items.json drops
- Branch Snapper | npc10641 | level 25 rare | single point (46.51, 44.27), center | no exclusive loot of its own (Pagan Mantle, 8 zones); pure kill; tame question logged unverified (no beast loot, no turtle-family kills in the core guide) | source: npcs.json + items.json drops
- Eck'alom | npc10642 | level 27 rare | single point (52.76, 70.05), southeast | Broken/Damaged/Fractured/Crushed Elemental Bracers (items 5446/5447/5448/5451, Ashenvale-exclusive, shared with Tideress) are questItems for the Alliance quest Elemental Bracers (q1016, races 4294967373) with no Horde use — no collects shipped, pure kill with an honest note | source: npcs.json + items.json drops + quests.json
- Mugglefin | npc10643 | level 23 rare | single point (19.38, 42.73), west | no exclusive loot (murloc loot, 7+ zones); pure kill; murlocs are not a tameable family — logged unverified | source: npcs.json + items.json drops
- Mist Howler | npc10644 | level 22 rare | loop over 2 northwest points (20.93, 36.92), (26.8, 18.35) | Wolf Whistle (item284666, Ashenvale-exclusive) as optional collect; tame question logged unverified (drops Lean Wolf Flank but the core guide kills no wolves — no corroboration) | source: npcs.json + items.json drops
- Prince Raze | npc10647 | level 32 rare (two above band — ships with an honest come-back-later note) | loop over 2 far-east points (78.08, 46.35), (81.56, 48.51) | Arcane Charged Robes (item284697, Ashenvale-exclusive) as optional collect; Satyr Horns (item5481) as optional collect with a note pointing at the core guide (feeds contracted q6441) | source: npcs.json + items.json drops
- Ursol'lok | npc12037 | level 31 rare (one above band — ships with an honest come-back-later note) | single point (83.37, 48.51), far-east edge | Ursol'lok's Paws (item284573, Ashenvale-exclusive) as optional collect; only-Hunter tame task ships (drops Big Bear Meat + Bear Gall Bladder and the core guide's q98251 kills Ashenvale Bears — drop evidence plus core-guide corroboration, the Mulgore Mazzranache pattern) | source: npcs.json + items.json drops
- Sharptalon's hunt | npc12676 (NOT rare-flagged — ships by the item-start hunt rule) | level 31 beast, faction A (hostile to Horde, killable; the core guide kills it) | single point (74.98, 70.06) | kill + Sharptalon's Claw (item16305, 100% drop, Ashenvale-exclusive) as optional collect + note pointing at the core guide (starts contracted q2; the accept/turnin live there) | source: npcs.json + items.json drops
- Ursangous's hunt | npc12678 (NOT rare-flagged — ships by the item-start hunt rule) | level 25 beast, faction A | single point (39.76, 65.21) | kill + Ursangous's Paw (item16303, 100% drop, Ashenvale-exclusive) as optional collect + note pointing at the core guide (starts contracted q23); NO tame line although the drop/corroboration pattern holds (bear meat + core q98251 kills bears) — the core contract needs the kill for q23, so taming instead would wedge the core route | source: npcs.json + items.json drops
- Shadumbra's hunt | npc12677 (NOT rare-flagged — ships by the item-start hunt rule) | level 28 beast, faction A | single point (57.5, 56.05) | kill + Shadumbra's Head (item16304, 100% drop, Ashenvale-exclusive) as optional collect + note pointing at the core guide (starts contracted q24); no tame line (core needs the kill) | source: npcs.json + items.json drops
- Tideress's hunt | npc12759 (NOT rare-flagged — ships by the item-start hunt rule) | level 27 | single point (46, 70), Mystral Lake | kill + Befouled Water Globe (item16408, 100% drop, Ashenvale-exclusive) as optional collect + note pointing at the core guide (starts contracted q1918); Intact Elemental Bracer (item12220) noted as Alliance-quest fodder (q1016), no collect | source: npcs.json + items.json drops
- Fixed world containers | obj2849 (Battered Chest, 4 pts) + obj2850/obj2852 (Solid Chest, 12 + 7 pts) + obj3659/obj3695 (Barrel of Melon Juice + Food Crate, 24 shared pts) + obj3662/obj3705 (Food Crate + Barrel of Milk, 1 shared pt) + obj3689/obj3702 (Weapon Crate + Armor Crate, 4 shared pts) + obj19021 (Rusty Chest, 24 pts) + obj19022 (Worn Chest, 1 pt) + obj178144 (Troll Chest, 14 pts — core q6462 collects charms here, so the loop carries a core-pointer note; the companion never accepts) + obj179487/obj179489 (Waterlogged Footlocker, 11 + 1 pts) + obj441128 (Vibrating Crate, 3 pts) | one loop step over all fixed points, said plainly; all ordinary low-level goods, no unique treasure confirmed | source: objects.json
- Warsong Oil crates | obj178195 (Warsong Oil, 7 pts: (66.45, 56.85), (66.85, 57.14), (67.03, 56.69), (78.18, 44.75), (78.38, 45.07), (79.47, 50.74), (80.5, 51.24)) | own loop step with a note pointing at the core guide (core q6571 collects oil here) | source: objects.json
- Plant Bundle | obj17282 (14 pts) | own loop step; fixed pickable with no quest reference anywhere in the data — contents unconfirmed, said plainly | source: objects.json + quests.json
- Bottle of Disease | obj18036 (2 pts: (75.27, 71.8), (75.29, 72.22)) | own loop step; fixed pickable with no quest reference anywhere in the data — contents unconfirmed, said plainly | source: objects.json + quests.json
- Kurothel's Knapsack | obj673431 (4 pts: (80.6, 49), (81.1, 50.6), (81.3, 50.3), (81.7, 49.2)) | own loop step; fixed container with no quest reference anywhere in the data — contents unconfirmed, said plainly | source: objects.json + quests.json
- No contract quest has object-type objectives naming any shipped container (the Horde contract's objectives are item/event/kill typed — verified by scan). No shipped rare is a giver, ender, or objective of any Horde contract quest (all 35 checked against the shipped ids; the hunt droppers' linkage is item-start only and owned by the core guide's accept/turnin).

Argued exclusions:
- Apothecary Falthis (npc3735, lvl 22 rare, 3 northern points): Horde-faction NPC (faction H), hence friendly to Horde players and unkillable by them — NOT shipped in the Horde guide (the Alliance guide covers him for their side). This is the faction-asymmetry case the Horde block exists to catch.
- Varo'then's Ghost (npc6118, lvl 48, 1 pt (97.9, 47.9) far east): sixteen levels above the band with nothing exclusive to come back for (widest loot is 14-zone Ichor of Undeath) — excluded (Arathi precedent).
- Baron Aquanis (npc12876, lvl 28): has NO spawns anywhere in the data — no goto can be written; excluded with this reason (the core guide covers his Strange Water Globe via bag note; the accept/turnin live there).
- Aean Swiftriver (npc5797): spawns in the Barrens (1413), not Ashenvale — out of zone, excluded (the core guide covers the Runed Scroll via its Barrens expedition).
- Foulweald Totem Mound (obj178206) + Murgut's Totem Basket (obj178227): single-purpose core-quest furniture for contracted q6621 — excluded with a core-pointer note (nothing to collect).
- Naga Brazier (obj178247) + trap copy (obj178248): single-purpose core-quest furniture for contracted q6641 — excluded with a core-pointer note.
- Gurda's Shredder (obj178146): the core q6504 giver's furniture — excluded with a note.
- Ruul Snowhoof Cage (obj178147): the core q6482 escort furniture — excluded with a core-pointer note.
- Sapphire of Aku'Mai mouths (obj178184/178185/178186): the core q6563 sapphire sources — excluded with a core-pointer note.
- Fathom Stone (obj177964): has NO spawns in the data — nothing to ship (the core guide covers the Fathom Core via bag note).
- Tome of Mel'Thandris (obj19027): objective of Alliance quest q1022 (The Howling Vale) — Alliance content, excluded.
- Circle of Imprisonment (obj19901/obj20352): objectives of Alliance quest q1140 (Tower of Althalaxx chain) — Alliance content, excluded.
- Herbs, veins, and gathering nodes (Mageroyal through Gromsblood, Copper through Truesilver, Dreamroot, Fool's Gold): gathering nodes, never companion treasure content — not shipped, stated not padded.
- Lore/scenery/furniture uniques with no container behavior evidenced (books, monuments, portals, anvils, mailboxes, campfires, braziers, moonwells, shrines, soulgems, Chalice of Elune, Dream-Touched Dragon Egg, Azsharan Prophecy, Gleaming Crescent Pendant, Wooden Figurine/Archaeologist's Cart/Unlit Torch cluster, Spear of Mannoroth, Shattered Orb, Carved Stone, Dark Ritual Stone, Bough of Shadows, Leyline, Field Guide, Elemental Convergence, Elune's Tear, Giant Clams, Dor'Danil Pillar, Legacy of the Aspects): not shipped — the pack's treasure scope is fixed containers plus evidenced pickables (Alliance parity).
- Tame lines: exactly one shipped (Ursol'lok — see above). All others logged in docs/companion-unverified.md with the failing half of the test named (Oakpaw, Mist Howler, Terrowulf Packlord, Branch Snapper, Mugglefin, Sharptalon, and the hunt-trio moot cases).

## ashenvale-horde-recipes.guide — 2 vendor-sold + 10 narrow mob drops

Vendor-sold (profession from the item-name convention: Pattern = Leatherworking unless cloth-named, Plans = Blacksmithing, Formula = Enchanting, Recipe food/fish = Cooking, Recipe potion/elixir = Alchemy — no profession flag exists in the data):
- Recipe: Rockscale Cod | item6369 | buy from Wik'Tar, npc12962, Fish Merchant & Supplies (11.71, 34.1), west coast | Cooking | source: items.json vendors
- Recipe: Mithril Head Trout | item17062 | buy from Wik'Tar, npc12962 | Cooking | source: items.json vendors

Drops (sole dropper, or the dropper's spawns are in-zone and the drop is narrow):
- Formula: Enchant Bracer - Minor Healing Power | item249475 | collect from the Dark Strand Cultist, npc3725 (level 18, 7 far-north points) — the SOLE dropper anywhere | Enchanting (name basis: Formula) | source: items.json drops
- Recipe: Bear Brisket | item250182 | collect from the Ashenvale Bear, npc3809 (level 21, 24 points across the zone) — the SOLE dropper anywhere; the bear also spawns in the Barrens (dual 1413/1440), noted honestly | Cooking | source: items.json drops
- Pattern: Hillman's Leather Boots | item252804 | collect from the Shadowhorn Stag, npc3817 (level 22, 69 points across the zone) — the SOLE dropper anywhere | Leatherworking | source: items.json drops
- Recipe: Cleric's Elixir | item250368 | collect from the Xavian Hellcaller, npc3757 (level 29, 6 eastern points) — the SOLE dropper anywhere; Uncloven Satyr Hoof also drops here (Alliance-quest item, q1842 — noted, no collect) | Alchemy (content basis: elixir) | source: items.json drops
- Plans: Sterling Silver Gauntlet | item251337 | collect from the Wrathtail Myrmidon, npc3711 (level 20, 14 northwest-shore points) — the SOLE dropper anywhere; the myrmidon also spawns on Darkshore (dual 1439/1440), noted honestly | Blacksmithing | source: items.json drops
- Recipe: Elixir of Strength | item250385 | collect from the Shadethicket Oracle, npc3931 (level 30, band top, 1 point (66.66, 82.17) southeast) — the SOLE dropper anywhere | Alchemy (content basis: elixir) | source: items.json drops
- Plans: Bronze Dory | item251455 | collect from the Dark Strand Enforcer, npc3727 (level 20, 1 point (31.62, 30.68) far north) — the SOLE dropper anywhere | Blacksmithing | source: items.json drops
- Plans: Iron Fists | item251456 | collect from the Bleakheart Hellcaller, npc3771 (level 26, 8 eastern points) — the SOLE dropper anywhere | Blacksmithing | source: items.json drops
- Pattern: Tooled Leather Belt | item252858 | collect from the Highborne Apparition, npc6116 (level 45, 2 far-east-edge points (98.6, 45.8), (99.1, 46.2)) — the SOLE dropper anywhere; far out-of-band, ships with an honest come-back-later note (Westfall Shafety Sheep precedent) | Leatherworking | source: items.json drops
- Plans: Blessed Plate Pauldrons | item251438 | collect from the Highborne Lichling, npc6117 (level 46, 2 far-east-edge points (98.2, 47), (99.1, 46.2)) — the SOLE dropper anywhere; far out-of-band, ships with an honest come-back-later note | Blacksmithing | source: items.json drops

Every other Ashenvale-dropping recipe drops in 3+ zones (generic world drops, Elwynn rule) — none shipped. Quest-reward recipes are unverifiable from quest records (no rewards field) — none shipped. Professions with NO Ashenvale (Horde) source: Tailoring, First Aid, Engineering, Fishing, Leatherworking beyond the three listed patterns, Enchanting beyond the one listed formula — stated in the guide, not padded (Dun Morogh Blacksmithing precedent).

Argued exclusions:
- The 7 Alliance-vendor recipes (Big Bear Steak 3734, Lean Venison 5489, Barbaric Leggings 5973, Shadow Protection Potion 6054, Herbalist's Gloves 7361, Enchant Cloak - Minor Agility 11039, Enchant Bracer - Lesser Strength 11101): sold ONLY by Alliance-faction vendors (Ulthaan, Lardan, Harklan Moongrove, Harlown Darkweave, Dalria) — excluded by the flipped faction rule, with this reason.
- The Baron/Lorgus helm plans and patterns (items 251350-251354, 252456, 252814-252817): dozens of listed droppers but EVERY one is spawnless in the data (no spawning NPC drops them anywhere) and no vendor sells them — effectively unobtainable; logged in docs/companion-unverified.md, not shipped.
- Samophlange Manual Cover/Page and Formula: Enchant Gloves - Herbalism: per the Alliance inventory's ruling (quest items / multi-zone world drop) — logged in docs/companion-unverified.md, not shipped.
