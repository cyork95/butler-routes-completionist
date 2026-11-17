# Duskwood (Horde) companions inventory (pack 0.107.0)

Every entry shipped in the two Duskwood Horde companion guides, one line each:
name, NPC/item id, source type, coordinates or vendor, and the data source
verified against. All coordinates are the client's own (live) map frame on
map 1431 (Duskwood). Game data is questie-forever npcs.json, objects.json
and items.json; quest linkage checked against the full quest table and the
5-quest Horde core contract (`duskwood-horde.guide`). The data carries an
explicit `rare` role flag; 6 Duskwood NPCs hold it. Band note: the Horde
core band is 37–42 — ALL six flagged rares sit BELOW it (levels 23–34).
They ship with an honest below-band note each (trivial at Horde levels,
swept opportunistically), the mirror of the Alliance round's above-band
come-back-later notes. Data wins over the Alliance inventory wherever they
differ (two overturns logged below).

## duskwood-horde-rares.guide — 6 rares + world containers + sights

- Lord Malathrom | npc503 | level 31 rare, fac None | BELOW BAND — shipped with honest below-band note | loop over 7 points (20.31, 28.83) … (25.92, 30.9), north-west | signatures: Spiked Collar (item1187) + Cloak of Rot (item4462), both sole drops (npc503 only); no quest takes either | source: npcs.json + items.json + quests.json
- Fenros | npc507 | level 32 rare, fac None | BELOW BAND | loop over 8 points (60.68, 40.7) … (63.88, 51.77), east | signatures: Ravenwood Bow (item4474) + Tribal Worg Helm (item6204), both sole drops (npc507 only); no quest takes either | source: npcs.json + items.json + quests.json
- Lupos | npc521 | level 23 rare, fac None | BELOW BAND | loop over 16 points (19.99, 26.39) … (70.63, 26.64), the western road and Raven Hill woods | signatures: Hide of Lupos (item3018) + Nightbane Staff (item3227), both sole drops (npc521 only); no quest takes either | source: npcs.json + items.json + quests.json
- Nefaru | npc534 | level 34 rare, fac None | BELOW BAND | loop over 3 points (61.85, 81.38), (63.48, 83.67), (74.33, 77.9), far south | signatures: Beastwalker Robe (item4476) + Nefarious Buckler (item4477), both sole drops (npc534 only); no quest takes either | source: npcs.json + items.json + quests.json
- Naraxis | npc574 | level 27 rare, fac None | BELOW BAND | single point (86.36, 47.57), far east | signatures: Husk of Naraxis (item4448) + Naraxis' Fang (item4449), both sole drops (npc574 only); no quest takes either | source: npcs.json + items.json + quests.json
- Commander Felstrom | npc771 | level 32 rare, fac None | BELOW BAND | loop over 10 points (13.18, 36.19) … (18.55, 35.73), west | signatures: Trouncing Boots (item4464) + Bonefist Gauntlets (item4465), both sole drops (npc771 only); no quest takes either | source: npcs.json + items.json + quests.json
- Fixed world containers | obj2850 (Solid Chest, 20 pts) + obj2852 (Solid Chest, 24 pts) + obj3659/obj3695 (Barrel of Melon Juice + Food Crate, 24 pts each) | one loop step, 68 unique points (raw 92, dedupe 68), ordinary low-level goods | source: objects.json — OVERTURN: the Alliance inventory (pack 0.40.0) counted 86 unique points (obj2852 as 32 pts); the data in front of me shows obj2852 with 24 pts and 68 unique overall. Data wins.
- Unique containers, quest-unused in the data | obj411348 Dusty Coffer (26.0, 31.0), north-west | obj410779 Offering Box (81.2, 71.8), far south-east | obj321/obj706187 Tear of Tilloa (78.35, 35.95), east — two object ids, one sight | each its own step | source: objects.json + quests.json (no structural quest ref to any of them)
- Markers (flavor, no loot confirmed — one sightsee step each) | obj37 Eliza's Tombstone (28.9, 30.5) | obj410034 Carved Stone (49.4, 34.0) | obj22706 Faustin's Alchemy Set (87.48, 35.19), beside the Horde hub | obj612088 Field Guide (78.3, 45.3) | obj673515 Memory of Valor (21.1, 55.6) | obj177280 Moonwell (49.2, 33.29) | source: objects.json

Argued exclusions:
- Classic rares WITHOUT the data flag (Mor'Ladim npc522 L35, Stitches npc412 L35, Stalvan Mistmantle npc315 L32, Eliza npc314 L31, Morbent Fel npc1200 L32; all roles=undefined): the flag is the rule, standing ruling carried, not re-litigated. Data wins over community memory.
- Faction ruling: all 6 shipped rares are fac None — no Falthis exclusion fires, and no Stonetalon-rule Alliance-held-ground note is needed (none sits in faction-flavoured territory).
- Alliance-quest furniture excluded — a Horde player cannot accept the quests these objects serve, so pointing at them serves nothing: obj21052 Defias Strongbox (Alliance 1244 objective-item site), obj119/obj167 Abercrombie's Crate (Alliance 134 objective item1349), obj441114 Mysterious Box (Alliance Missions-chain objective site). Quest-owned per the Alliance round's determination; excluded here by the faction rule.
- Quest-owned generics (same list as the Alliance round — not companion content for either faction): Nightmare Moss (obj439557), Cold Iron Deposit (obj439558), Unhatched Green Dragon Egg (obj441119), Ogre Magi Trunk (obj441113), Battered Trunk (obj642320, writ 94223 start), Spellbook (obj409735, core 81747 start), Mound of Dirt (obj59/19030), Weather Grave (obj61), Eliza's Grave Dirt (obj51708).
- Flavor/furniture surveyed but not shipped (no container or loot in the data): signposts, chairs, campfires, anvils, forges, mailbox, books, pumpkins/decor, doors, herbs, veins, leyline, portals.
- No Horde-contract quest has any of the 6 shipped rares as giver, ender, or kill objective (all 5 checked: 1372/1383/1388/1391 NPC starts, 94241 sourceless item start). No pointer steps needed — the Wanted-Poster case does not arise (the writ item 264041 is sourceless; there is nothing to hunt, documented, no step).
- Tame lines: none shipped. Lupos shows wolf evidence (Lean Wolf Flank item1015 among 14 droppers) and Naraxis spider evidence (Spinnerets, Gooey Legs), but the Horde core guide (5-contract) carries no tame corroboration — no Hunter chain, no beast-family kill line. Same bar as the Alliance round (see docs/companion-unverified.md "Duskwood tame lines and lookalikes"); Horde outcome identical. Logged there, not shipped as fact.

## duskwood-horde-recipes.guide — 4 vendor-sold + 5 in-zone drops

Vendor-sold (all vendors neutral/AH — every goal npc-pinned; profession from the item-name convention, no profession flag exists in the data):
- Recipe: Holy Protection Potion | item6053 | buy from Kzixx, npc3134 [AH], (81.82, 19.77) north-east | Alchemy (protection potion) | source: items.json vendors
- Recipe: Shadow Oil | item6068 | buy from Bliztik, npc2481 [AH], (18.04, 54.36) west | Alchemy (oil) | source: items.json vendors
- Schematic: Goblin Jumper Cables | item7561 | buy from Kzixx [AH] (also Horde-sold elsewhere; the in-zone source is the shipped one) | Engineering (schematic) | source: items.json vendors
- Recipe: Elixir of Coalesced Regret | item210709 | buy from Kzixx [AH] | Alchemy (elixir) | source: items.json vendors

Drops (in-zone droppers, killable by Horde; sole-zone ones plain, multi-zone ones noted honestly):
- Plans: Sterling Silver Leggings | item251336 | collect from the Skeletal Warrior, npc48 (L21, sole-zone dropper, sole map 1431) — SOLE ZONE | Blacksmithing (plans + metal basis) | source: items.json drops + npcs.json spawns
- Manual: Clever Poultice | item255724 | collect from the Defias Enchanter, npc910 (L26, sole-zone dropper, sole map 1431) — SOLE ZONE | First Aid (manual basis) | source: items.json drops + npcs.json spawns
- Recipe: Minor Cleric's Elixir | item250366 | collect from the Murloc Forager, npc46 (L9, (58.6, 9.8), (62.2, 11.1), (71.1, 12.6)) — 3 zones [1429, 1431, 1420], noted honestly | Alchemy (elixir) | source: items.json drops + npcs.json spawns
- Pattern: Robes of Arcana | item5773 | collect from the Defias Enchanter, npc910 (L26, points above) — 3 droppers / 4 zones [1431, 1439, 1413, 1441], noted honestly | Tailoring (pattern basis) | source: items.json drops + npcs.json spawns
- Pattern: Invoker's Cord | item215369 | collect from the Skeletal Fiend, npc531 (L24, sole-zone dropper, sole map 1431) — SOLE ZONE | Tailoring (pattern basis) | source: items.json drops + npcs.json spawns — OVERTURN: the Alliance inventory (pack 0.40.0) counted 4 zones [1454, 1438, 1457, 1431]; the data in front of me shows the sole dropper npc531 spawning only on 1431. Data wins.

Every other Duskwood-dropping recipe drops in 5+ map-zones (generic world drops, Elwynn rule) — none shipped. Quest-reward recipes are unverifiable from quest records — none shipped. Professions with NO Horde Duskwood source: Leatherworking, Cooking, Fishing, Enchanting, and Tailoring-by-vendor (Tailoring ships on drops only) — stated in the guide, not padded (Dun Morogh Blacksmithing precedent).

Argued exclusions:
- Alliance-faction-vendor exclusives (Alterac rule, flipped for Horde — the brief's named case): Pattern: Greater Adept's Robe (item6275, Sheri Zipstitch [A]), Pattern: Dark Silk Shirt (item6401, Sheri [A]), Pattern: Bright Yellow Shirt (item14627, Danielle Zipstitch [A] — SOLE ZONE but Alliance-only), Pattern: Linen Reagent Bag (item253665) + Pattern: Woolen Reagent Bag (item253668) (Lohgan Eva / Danielle / Sheri, all fac A). Five recipes a Horde player cannot buy in-zone — excluded with reason, not shipped as Horde buys.
- Quartermaster Falinar (npc222684, fac AH, 2 spawns on 1431) sells no recipes in the data — surveyed, nothing to ship.
- No other recipe in the data lists any of the 17 1431-spawning vendors (full items.json vendor sweep: exactly the 9 Alliance-round recipes; 4 neutral + 5 Alliance-only).
