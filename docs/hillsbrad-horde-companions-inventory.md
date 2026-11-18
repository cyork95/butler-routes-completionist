# Hillsbrad Foothills (Horde) — companions inventory

Contract: the Horde core `hillsbrad-horde.guide` (10 quests, band 19–32
— the band is committed in docs/hillsbrad-horde-census.md and is reused
here, not re-derived). Zone key 1424. Sources: `npcs.json`,
`objects.json`, `items.json`, `quests.json` from the local Forever game
data build. Game data wins throughout. Rank semantics calibrated in
earlier rounds: rank 4 = Rare, rank 2 = Rare Elite. (All 11 flagged
Hillsbrad NPCs carry explicit `role: rare` flags — the sweep keys on
roles, verified against the Alliance inventory built from the same
dumps.) Loot "sole dropper" means the item's drops.npc lists only this
NPC and no object source; no vendor sells any signature below.
Tameability has NO data flag anywhere: a tame line ships only on drop
evidence PLUS core-guide corroboration, else it is logged in
docs/companion-unverified.md.

## RARES — 11 flagged on key 1424, 7 shipped, 4 excluded

Faction calls mirror the Alliance round, flipped (hub-by-hub from the
data): Dalaran Spellscribe (npc1920, lvl 21 Rare, faction A) and Tamra
Stormpike (npc14275, lvl 28 Rare, faction A) are Alliance-aligned —
killable opposition for Horde players, so both SHIP with that note
(Stonetalon rule: hostile faction-A rares ship as killable opposition
with an honest note). No flagged rare is Horde-aligned, so the Falthis
rule excludes nothing here. Above-band handling (band 19–32): Narillasanz
(npc2447, lvl 44), Old Cliff Jumper (npc8211, lvl 42), Araga (npc14222,
lvl 35) and Lady Zephris (npc14277, lvl 33) are EXCLUDED — all four sit
above the band with no in-band claim (same call as the Alliance round,
so the two factions agree on all four).

- Dalaran Spellscribe | npc 1920 | level 21 rare, faction A | 1 pt far
  west [8.9, 23.8] | 4436 Jewel-encrusted Sash + 4437 Channeler's Staff
  (sole each) | kill + collects, no loop (single point) + killable-
  opposition note |
- Tamra Stormpike | npc 14275 | level 28 rare, faction A | 3 pts SE
  [70.68, 78.05], [72.31, 82.34], [73.25, 81.09] | 282710 Dun Garok Rifle
  (sole) | loop + collect + killable-opposition note |
- Scargil | npc 14276 | level 30 rare, neutral | 1 pt [29.08, 73.56] |
  282716 Imbued Scaled Cuffs (sole) | kill + collect, no loop |
- Ro'Bark | npc 14278 | level 28 rare, neutral | 1 pt [65.72, 60.15] |
  282721 Gnash Shaman's Staff (sole) | kill + collect, no loop |
- Creepthess | npc 14279 | level 24 rare, neutral | 1 pt [38.6, 58.37] |
  282720 Spider Swarm (sole) | kill + collect, no loop |
- Big Samras | npc 14280 | level 27 rare, neutral | 1 pt [86.03, 39.93] |
  282717 Durable Bearhide Pauldrons (sole) | kill + collect, no loop |
- Jimmy the Bleeder | npc 14281 | level 23 rare, neutral | 1 pt
  [60.1, 9.1] | 282713 Bloodstained Pants (sole) | kill + collect, no
  loop |

Shared drops on the shipped seven are ordinary greens (plus scrolls and
cloth on some) — no tameable-family evidence beyond the meat/venom/silk
(claw on Samras) noted under TAME below, and the core guide carries no
corroboration either way.

Notes:
- No core-contracted quest references any shipped rare structurally:
  the 10-contract quests were scanned (start/end/kill-objective/sourceItem
  — including 8409's Keg start-object and 96986's spawnless kill) — zero
  hits. (Dun Morogh rule satisfied; the Atrexis case is documented below,
  not routed.)
- Quest-target lookalikes are not rares: Atrexis (96986's ender) has no
  spawn entries, no moves entry, no rank and no roles anywhere in the
  data — the Baron Aquanis exclusion, in writing: no point is invented
  for him, and no companion step covers him. (His quest rides the core
  guide's honest no-complete handling.)
- Tameability: Creepthess drops Crisp Spider Meat, Large Venom Sac and
  Spider's Silk; Big Samras drops Big Bear Meat and Sharp Claw — real
  beast-family evidence — but the Horde core guide carries no `only
  Hunter` lines and no references to either mob, so per the Duskwood
  precedent the bar does not lower for a small core: no tame lines ship.
  Logged with the evidence in docs/companion-unverified.md.
- Respawn timers: unconfirmed anywhere in the data; none stated.

## ITEM-START HUNTS — nothing ships

- The census found exactly ONE in-zone object-start (8409's Keg 180570
  at [51.37, 58.98]) and zero item-starts, verified by scan (start.npc/
  start.item/start.object over all Horde 1424 records plus the cross-key
  sweep). The core routes the Keg itself (8409 accept at the object,
  note at source, no wedge). No hunt ships — stated plainly, not padded.
- The sweep found 549/566/567 WANTED-board object-starts touching 1424
  ([62.63, 20.75] Tarren Mill post / [62.56, 19.66] square), but all
  three are zone-field 1416 with Horde masks — the Alterac pool, and the
  alterac-horde contract already lists 549/550/566/567. Flagged for that
  round, not contracted here.

## TREASURES — fixed containers loop + one flagged addition

One `Fixed Chests` loop step rides all of these (loop needs ≥2 gotos;
(Rares with single points get no loop — same rule as the core guides'
  companions):
- 2039 Hidden Strongbox (7 pts), 2850/2852/2855 Solid Chest (4/6/8
  pts), 3659 Barrel of Melon Juice (33 pts), 3694/3695/153470 Food Crate
  (5/33/6 pts), 3705 Barrel of Milk (5 pts), 3715/4096/105579/111095
  Alliance Chest (7/4/10/5 pts), 105570 Alliance Strongbox (4 pts),
  103815 Ambermill Strongbox (1 pt), 179486/179488 Battered Footlocker
  (10/8 pts), 181302 Camp Crate (2 pts), 181620 Unopened Crate (1 pt).
  Every one verified: fac None (no faction lock anywhere in the data),
  no quest start/objective link in any quest record. The Alliance-named
  chests/strongbox ship because the data carries no Alliance lock — the
  Alliance guide ships the same objects; both factions sweep the same
  boxes and the point sets match exactly (no contradiction).
- 1727 Keg of Shindigger Stout (5 pts, loot the keg itself): SHIPS as a
  flagged Horde-side addition — a beverage vessel, the same class as the
  shipped Milk barrel (fixed multi-point placement + own loot + no
  faction/quest lock), which the Alliance inventory omits without a
  stated reason. Data wins; the delta is flagged here, not harmonized.

Excluded with reasons (logged, not papered over):
- 180570 Keg (8409's start-object on 1424): Hillsbrad Horde core owns
  it — Dun Morogh rule, no step duplicates a core interaction.
- 1763 WANTED + 2008 Dangerous!: Alterac-contracted quest furniture
  (549/566 + 567, all in the alterac-horde contract) — excluded, the
  owning round named. 707245 WANTED board: no 1424 spawn — not in-zone.
- 1738/1739/1740 Syndicate Documents: Alterac quest furniture (510/
  511 Alliance + 532 Horde, all zone 1416) — excluded, named.
- 1721/1722 locked ball and chain: Alterac quest furniture (498, Horde,
  zone 1416) — excluded, named.
- 1768/1769/1770 Flames of Azel/Veraz/Uzel: Alterac quest furniture
  (553, Horde, zone 1416) — excluded, named.
- 1759 Hillsbrad Town Registry + 1736 Shipment of Iron: single-point
  non-vessel furniture with self-loot and no quest link — not openable
  containers by kind; excluded, named.
- 1723 Mudsnout Blossom: flower (flora class, same as the gathering
  nodes) — excluded.
- 1728 Dusty Rug / 1729 Tainted Keg / 1730 smoke / 180575 Keg: single-
  point decor scenes with no loot (or no quest link) — excluded.
- 1720 Stanley's Dish / 1761 Proclamation / 1767 Helcular's Grave:
  no-loot decor (Grave named — Helcular-adjacent, no quest link) —
  excluded.
- Mailboxes, anvils, forges, campfires, signposts (1771-2061 series),
  mining veins, herbs, Elemental Convergence 616992, Loose Soil 621813,
  Guild Vault 630863, Black Smoke 965, Test 2558: travel/work furniture,
  gathering nodes, event/decor — class exclusions, same as the Alliance
  round.
- 2714 Alterac Granite (6 pts, 114-entry generic world loot table, no
  signature loot, no quest link, no faction): evaluated and excluded —
  a rock by kind, not an openable vessel; its table is world clutter,
  not a container signature. The Alliance inventory agrees by omission;
  the agreement is logged here (both rounds see the same records).
- 179487 Waterlogged Footlocker: no 1424 spawn — not in-zone.

## RECIPES — 14 vendor-sold + 6 narrow drops

Recipe scan: every recipe/pattern/plans/schematic/formula item against
every 1424 mob drop table, plus every vendor with a 1424 spawn against
its full stock. Zero in-zone mob drops for most; vendor coverage below.

Vendor-sold, Horde-buyable on 1424 (npc-pinned in the guide):
- Christoph Jeffcoat 2393 (fac H, Tarren Mill [62.29, 19.04]): 5788
  Thick Murloc Armor, 6054 Shadow Protection Potion.
- Mallen Swain 2394 (fac H, [61.9, 20.98]): 6274 Blue Overalls, 6401
  Dark Silk Shirt, 253665 Linen Reagent Bag, 253668 Woolen Reagent Bag.
- Derak Nightfall 2397 (fac H, [63.09, 19.41]): 6330 Bristle Whisker
  Catfish, 21099 Smoked Sagefish, 21219 Sagefish Delight.
- George Candarte 2698 (fac H, [92.02, 38.23]): 7613 Green Leather
  Armor.
- Zixil 3537 (fac AH neutral, [55.38, 34.71]): 5772 Red Woolen Bag,
  6377 Enchant Boots, 7362 Earthen Leather Shoulders, 7561 Goblin
  Jumper Cables, 210709 Elixir of Coalesced Regret.
- Zan Shivsproket 6777 (fac AH, [84.1, 18.4]): 7742 Cloaking Device.
- Smudge Thunderwood 6779 (fac AH, [84.2, 18.1]): 18160 Thistle Tea.
- Checked with no recipe stock in the data: Innkeeper Shay, Kayren
  Soothallow, Kris Legace, Ott, Jason Lemieux, Mirvyna Jinglepocket
  (food/mushroom stock only), Horde Warbringer (empty) — not shipped.
- No limited-stock flag exists in the data; no recipe is marked
  limited. Each vendor step notes that stock class is unconfirmed.

Narrow drops (no vendor anywhere in the data; named mob or tight
in-zone family):
- 249881 Root Tea ← Torn Fin Oracle 2376 (sole dropper, in-zone).
- 251335 Sterling Silver Boots ← Syndicate Watchman 2261 (sole).
- 251391 Hard Gold Pauldrons ← Crushridge Ogre 2252 (sole; lvl 34,
  +2 over band — come-back-later note).
- 284870 Unsanctified Grenade ← Crushridge Warmonger 2287 (sole;
  lvl 39, +7 — come-back-later note).
- 11152 Enchant Gloves - Fishing ← Torn Fin family (Muckdweller 2374,
  Coastrunner 2375, Oracle 2376, Tidehunter 2377, all lvl 28-31
  in-zone) + Scargil 14276 (lvl 30, shares their ground): 5 droppers,
  ALL 1424-only, one camp — a tight in-zone family per the Thousand
  Needles precedent. FLAGGED: the Alliance inventory omits it (its 4
  exclusives are all sole-droppers); the data shows no vendor anywhere
  and a single-camp family, so it ships here with the delta stated.
- Excluded: 5775 Black Silk Pack (3 droppers across 3 zones, single
  in-zone source the lvl-37 Shadowy Assassin — scattered, not a tight
  family; the Alliance agrees by omission, reason logged here);
  4301 Barbaric Belt (32 droppers — generic world drop, not narrow).
- Fished/quest/etc. sources: none others found; the scan covered all
  recipe-named items.

Excluded (Alliance-only vendors, rule stated per recipe — the faction
rule, flipped for Horde; the Duskwood pattern):
- 4355 Icy Cloak (Micha Yance A; only Horde vendor Ghok'kah off-zone).
- 6055 Fire Protection (Nandar Branson A; only Horde vendor Jeeda
  off-zone).
- 18046 Tender Wolf Steak (Truk Wildbeard A; Horde vendors Fizzgrimble/
  Dirge/Zizplink all off-zone).
- 11163 Enchant Bracer Deflection (Micha Yance A; only Horde vendor
  Keena off-zone).
- 8409 Nightscape Shoulders (Nioma A; only Horde vendor Jangdor
  off-zone).
- 7995 Mithril Scale Bracers (Harggan A; only Horde vendor Gharash
  off-zone).
- 6369 Rockscale Cod (Lindea Rabinne A; only Horde vendor Mara Jumash
  off-zone).
- 17062 Mithril Head Trout (Lindea Rabinne / Merr Goodwin A; Horde
  vendors off-zone).
- Quest-reward recipes: quest records carry no reward data — never
  shipped, class-logged in companion-unverified.md.
- Trainer-taught staples excluded (Polestar's own profession guides).
- No-source professions stated plainly in the guide, not padded: First
  Aid, Fishing, Blacksmithing (Martha-analog gaps: every in-zone
  source is Alliance-only as listed above).

Cross-check against the Alliance inventory: same 7 shipped rares with
the same points, drops and band calls; same fixed-container set plus
the flagged Shindigger addition; 14 of its 25 vendor recipes ship (the
8 excluded are all Alliance-vendor-locked, each logged); its 4 narrow
drops ship plus the flagged 11152 addition; no tame lines on either
side for the same reason (evidence without corroboration); Atrexis and
the WANTED boards excluded on both sides with the owning round named.
Where the two inventories differ (Shindigger Kegs, 11152), this
document states the data reason — never silently harmonized.
