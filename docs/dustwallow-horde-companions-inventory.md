# Dustwallow Marsh (Horde) — companions inventory

Contract: the Horde core `dustwallow-horde.guide` (5 quests, band 30–45
— the band is committed in docs/dustwallow-horde-census.md and is reused
here, not re-derived). Zone key 1445. Sources: `npcs.json`,
`objects.json`, `items.json`, `quests.json` from the local Forever game
data build. Game data wins throughout. Rank semantics calibrated in
earlier rounds: rank 4 = Rare, rank 2 = Rare Elite. (All 12 flagged
Dustwallow NPCs carry explicit `role: rare` flags — the sweep keys on
role, verified against the Alliance inventory built from the same
dumps.) Loot "sole dropper" means the item's drops.npc lists only this
NPC and no object source; no vendor sells any signature below.
Tameability has NO data flag anywhere: a tame line ships only on drop
evidence PLUS core-guide corroboration, else it is logged in
docs/companion-unverified.md.

## RARES — 12 flagged on key 1445, all 12 shipped (10 in-band + 2 below-band with notes)

No Horde-aligned flagged rare exists, so the Falthis rule excludes
nothing; the two Alliance-excluded faction-A rares are killable
opposition for Horde players, so both ship with that note (Stonetalon
rule) — and both sit below the band, so both also carry a below-band
mirror note (Duskwood Horde precedent: below-band sources ship with the
mirror note). Above-band: none — the highest-flagged rare is exactly 45
(Brimgore, ships).

- Brimgore | npc 4339 | level 45 rare | 1 pt (42.12, 75.94), far south |
  285063 Black Brood Battleguards (sole) | kill + collect, no loop |
- Darkmist Widow | npc 4380 | level 40 rare | 1 pt (31.15, 20.4), west |
  285102 Darkmist Dirk (sole) | kill + collect, no loop — the shared
  5884 Unpopped Darkmist Eye is the core 1206 objective's drop, so the
  hunt rides the core guide; the note points at the core, never a step |
- Burgle Eye | npc 14230 | level 38 rare | 1 pt (59.04, 9.37),
  north-east shore | 285095 Twitching Eye (sole; no quest takes it) |
  kill + collect, no loop |
- Drogoth the Roamer | npc 14231 | level 37 rare | 1 pt (39.5, 18.92),
  west | 285089 Swamp Roamer's Band (sole; no quest takes it) | kill +
  collect, no loop |
- Dart | npc 14232 | level 38 rare | 1 pt (47.27, 18.38), west | 285100
  Serrated Raptor Teeth + 285283 Serrated Axes (both sole; no quest
  takes either) | kill + collects, no loop |
- Ripscale | npc 14233 | level 39 rare | 4-pt loop (37.8, 50.29),
  (42.35, 55), (44.08, 50.17), (49.06, 57.33), south-east | no sole
  drops — ordinary greens get a note, not a goal | kill + loop, no
  collect |
- Hayoc | npc 14234 | level 41 rare | 1 pt (52.02, 62.87), south |
  285103 Marsh Serpent's Scales (sole; no quest takes it) | kill +
  collect, no loop |
- The Rot | npc 14235 | level 43 rare | 1 pt (52.9, 57.4), south |
  285101 Rot-Fused Greaves (sole; no quest takes it) | kill + collect,
  no loop |
- Lord Angler | npc 14236 | level 44 rare | 1 pt (57.83, 61.62),
  south-east | 285094 Ravaged Fishing Pole (sole; a fishing pole,
  flavor) | kill + collect, no loop |
- Oozeworm | npc 14237 | level 42 rare | 3-pt loop (34.95, 70.86),
  (36.03, 63.07), (39.12, 63.05), far south | no sole drops — ordinary
  greens get a note | kill + loop, no collect |
- Malgin Barleybrew | npc 5848 | level 25 rare, faction A | 1 pt
  (27.2, 58.61) | 286541 Bael'dun Tankard (sole; his other drops are
  generic vendor drinks) | kill + collect, no loop + two notes:
  killable opposition for Horde (faction A) AND below the band (mirror
  note) |
- Captain Gerogg Hammertoe | npc 5851 | level 27 rare, faction A | 1 pt
  (27.1, 57.7) | 285344 Guard Captain's Barrier (sole) | kill +
  collect, no loop + same two notes |

Notes:
- No core-contracted quest references any shipped rare structurally:
  the 5-contract quests were scanned (start/end/kill-objective) — zero
  hits. (Dun Morogh rule satisfied; the Loose Dirt and Badge starters
  are documented below, not here.)
- Quest-target lookalikes are not rares without their own flag: none of
  the above is one (all 12 carry the flag; the Onyxia furniture below
  carries none of it — it is excluded as chain furniture, not as a
  lookalike).
- Tameability: the Widow drops Thick Spider's Silk 4337, Dripping Spider
  Mandible 4585, Large Fang 5637 and White Spider Meat 12205 — real
  beast-family evidence — but npc records carry no tameability flag and
  the Horde core guide (5-contract) carries no `only Hunter` lines and
  no references to any rare. No tame lines ship (Duskwood precedent).
  Logged with the evidence in docs/companion-unverified.md.
- Respawn timers: unconfirmed anywhere in the data; none stated.

## ITEM-START HUNTS — nothing ships

- The census found exactly ONE in-zone object-start pair (1238/1239's
  Loose Dirt mound 20985 at [55.44, 25.92]) and zero item-starts,
  verified by scan (start.npc/start.item/start.object over all 15 Horde
  records plus the cross-key sweep). The core routes both accepts at the
  mound. No hunt ships — stated plainly, not padded.
- The sweep found no Horde item-starts dropping on 1445 in any zone
  ("no others" is claimed only after this scan).

## TREASURES — fixed containers loop + unique objects

One `Fixed Chests` loop step rides all of these (loop needs ≥2 gotos;
all points below verified against the dumps; fac None throughout — no
faction lock on any container):
- 2857 Solid Chest (12 pts) + 4149 Solid Chest (19 pts) + 3715 Alliance
  Chest + 3714 Alliance Strongbox (3 shared pts) + 111095 Alliance Chest
  (1 pt) + 153470 Food Crate (8 pts) + 3707 Food Crate (14 pts) + 3702
  Armor Crate (8 pts) + 3689 Weapon Crate (8 pts) + 3695 Food Crate (5
  pts) + 3706 Barrel of Sweet Nectar (7 pts) + 20925 Captain's
  Footlocker (1 pt) + 174728 Damaged Crate (1 pt) + 20727 Gizmorium
  Shipping Crate (1 pt [54.07, 56.49]; loot 5862 Seaforium Booster) —
  ordinary low-level goods; no unique treasure confirmed beyond the
  uniques below. Gizmorium is a Horde-side addition (fixed single-point
  container with loot, no quest link, no faction lock — same class as
  the shipped Damaged Crate; the Alliance inventory omits it): flagged,
  not harmonized.
- Unique objects, each its own step/note: 3646 General Twinbraid's
  Strongbox (26.3, 58.5; loot 5038 Tear of the Moons); 19904/19905/
  19906 Mok'Morokk's Snuff/Grog/Strongbox (44.53, 66.04 / 38.66, 65.57
  / 36.64, 69.57; loots 5834/5835/5836; NO quest link anywhere in the
  data — flavor, not furniture); 2871 Seaworn Altar (59.36, 9.63) +
  2872 Enchanted Sea Kelp (59.35, 9.6), east coast; 21128 Orc Spy Report
  (68.18, 48.63), Theramore (noted, no loot in the data — no step).

Excluded with reasons (logged, not papered over):
- 20985 Loose Dirt mound: core-owned (1238/1239's start-object; the
  Alliance 1219 twin uses the same mound) — Dun Morogh rule, no step
  duplicates a core interaction.
- 20359 Egg of Onyxia (6 pts) + 177928 Onyxia's Gate (1 pt) + 175321
  Unforged / 175322 Forged Seal of Ascension (1 pt each, Emberstrife
  ground): the excluded above-band Onyxia chain's furniture — the pack
  does not route that chain, so per the round rule these get an
  inventory ruling, not a step. (1172 The Brood of Onyxia is the
  Barrens-zone Horde link; 6602 is the Stonetalon-OUT link.)
- 21042 Theramore Guard Badge: quest-start furniture (1252 Alliance +
  1269 Horde, both zone 1413) — not contracted here; 1273's soft-pre
  mini names the in-zone point.
- 20992 Black Shield: quest-start furniture (1251 Horde + 1253
  Alliance, both zone 1413).
- 2555 Musty Scroll: quest-start furniture (626 Cortello's Riddle,
  zone 1413, neutral).
- 423900 Waterlogged Book: quest-start furniture (79952 RwlRwlRwlRwl!,
  zone 1458, neutral).
- 186426 Wanted Poster: flavor marker, no loot and no quest link in
  the data — surveyed, not shipped.
- 4096/105579 Alliance Chest + 105570 Alliance Strongbox + 179486/
  179488 Battered Footlocker + 181302 Camp Crate + 181620 Unopened
  Crate + 103815 Ambermill Strongbox: NO 1445 spawn anywhere in the
  data (their points live on 1416/1417/1421/1424/1437/1442) — the
  Alliance guide routes them anyway; flagged as the round's
  cross-zone delta, not shipped here and never harmonized.
- Gathering nodes (veins, herbs, Stranglekelp), campfires, chairs,
  anvils, forges, signs, portals, runes, mana rift, event decor
  (pumpkins/skulls/candy buckets/ghosts), meeting stone, cannons, ship
  wreckage, fishing schools (Oily Blackmouth/Firefin schools +
  Floating Wreckage are schools, not treasure), wreckage, string
  lights/poles, manual-labour furniture, stoves, tables, braziers,
  bookcases, barrels/cups/jugs/plates (unlisted decor), shield stands,
  weapon racks, stables, troughs, portcullis, lighthouse beam, rune
  circle, Dwarven fire, cannonballs, archives clutter: class
  exclusions (gathering/travel/work/event furniture, same as the
  Alliance round).

## RECIPES — 9 vendor + 5 narrow drops

Vendor-sold, Horde-buyable on 1445 (npc-pinned in the guide):
- Ogg'marr 4879 (fac H, Butcher, Brackenwall [36.7, 30.97]): 12228
  Roast Raptor, 12232 Carrion Surprise, 12239 Dragonbreath Chili, 20075
  Heavy Crocolisk Stew (all Cooking).
- Ghok'kah 6567 (fac H, Tailoring Supplies, Brackenwall [35.15,
  30.83]): 4355 Icy Cloak, 253665 Linen Reagent Bag, 253668 Woolen
  Reagent Bag (all Tailoring basis).
- Balai Lok'Wein 13476 (fac H, Potions/Scrolls/Reagents, Brackenwall
  [36.49, 31.76]): 16112 Heavy Silk Bandage, 16113 Mageweave Bandage
  (First Aid manuals), plus 16084 Expert First Aid book (First Aid is
  covered in-zone).
- Krak, Zulrg, Zanara, Nat Pagle (fac H/AH on 1445): checked, no
  recipe stock — not shipped.
- No limited-stock flag exists in the data; no recipe is marked
  limited. Each vendor step notes that stock class is unconfirmed.

Narrow drops (no vendor anywhere in the data; sole in-zone dropper
unless noted — the Duskwood mirror of the Elwynn rule):
- 251459 Mithril Shortsword ← Mirefin Coastrunner 4362 (L36, 14
  in-zone pts) — sole dropper, 1445-only. Blacksmithing.
- 254020 Earthen Silk Cuffs ← Mirefin Murloc 4359 (L35, 24+3 in-zone
  pts) — sole dropper, 1445-only. Tailoring.
- 249511 Enchant 2H Weapon-Lesser Agility ← Firemane Scout 4329 (L41,
  24+28 in-zone pts; also drops in the Barrens — dual-zone noted
  honestly). Enchanting.
- 250184 Raptor Rouladen ← Bloodfen Lashtail 4357 (L40, 15 in-zone
  pts; also drops in the Barrens — dual-zone noted honestly). Cooking.
- 254684 Stormcloth Headband ← Firemane Flamecaller 4334 (L43, 24+12
  in-zone pts) — sole dropper, 1445-only. Tailoring.
- Excluded narrow candidates with reasons: 5775 Black Silk Pack (3
  droppers across 3 zones; single in-zone source is the lvl-37
  Shadowy Assassin — scattered, not a tight in-zone family; the
  Alliance agrees by omission); 5786/5787 (vendored, plus 2-zone) —
  not shipped; 250989 Lesser Mender's Potion (2 droppers, Stormscale
  1439/1448 + Preserver 1413/1445 — scattered, not tight; Alliance
  agrees by omission); 12706/12714/12718 Runic set (1445-only sole
  droppers BUT levels 59-62 — out-of-band/out-of-reach, Feralas
  precedent: logged, never shipped).

Excluded Alliance-only vendors (documented per recipe — the faction
rule, flipped for Horde):
- 5789 Murloc Scale Bracers (Helenia Olden A; other vendor Blixrez AH
  1434 — off-zone, no H/AH in-zone source).
- 12233 Mystery Stew (Helenia Olden A; other vendor Super-Seller AH
  1443 — off-zone).
- Quest-reward recipes: class unverifiable (quest records carry no
  reward data) — never shipped, logged in companion-unverified.md.
- Trainer-taught staples excluded (Polestar's own profession guides).
- No-source professions stated plainly in the guide, not padded:
  Fishing, Engineering, Alchemy. (First Aid: Balai's book + manuals;
  Cooking/Tailoring/Enchanting/Blacksmithing: covered above.)

Cross-check against the Alliance inventory: same 10 in-band rares with
the same points, drops and band calls, plus the two below-band
opposition additions (Malgin/Gerogg) flagged with reasons; same fixed
containers verified point-for-point EXCEPT 7 objects the Alliance guide
routes that have no 1445 spawn anywhere (4096/105579 Alliance Chest,
105570 Alliance Strongbox, 179486/179488 Battered Footlocker, 181302
Camp Crate, 181620 Unopened Crate — flagged as their cross-zone routing,
never copied) plus the Gizmorium addition flagged; same 5 narrow drops
verified sole-and-in-zone (251459/254020/249511/250184/254684); vendor
lists differ by faction exactly as the data dictates (9 Horde vendor
recipes + First Aid book vs their 4 Alliance ones). Total shipped here:
9 vendor + 5 narrow = 14. Theirs: 4 + 5 = 9. Genuine faction
differences stated, never harmonized.
