# Azshara (Horde) companions inventory (pack 0.148.0)

Every entry shipped in the two Azshara (Horde) companion guides, one line
each: name, NPC/item id, source type, coordinates or vendor, and the data
source verified against. All coordinates are the client's own (live) map
frame on map 1447 (Azshara). Game data is questie-forever npcs.json,
objects.json and items.json; quest linkage checked quest by quest against
the full quest table and the 22-quest Horde core contract
(`azshara-horde.guide`, band 44-50). The data carries rank flags plus an
explicit `roles: ["rare"]` flag; all eight shipped rares hold both
(rank 4 + rare role), all with faction null (no Falthis-style Horde
exclusion anywhere).

This inventory mirrors `docs/azshara-companions-inventory.md` with the
vendor-faction rule flipped. Where the set is genuinely identical the
inventory says so — every rare point and every dropper link below was
re-verified from the data, not copied. Deltas are flagged in
`docs/companion-unverified.md`, never silently harmonized.

## azshara-horde-rares.guide — 8 rares + 3 fixed containers

- Varo'then's Ghost | npc6118 | level 48 rare | single point (13.23, 74.2), far west | no sole drop in the data (drops Ichor of Undeath 7972 as 1 of 120 world droppers) | kill + note pointing at the ungated main guide, which contracts shared quest 8256 (The Ichor of Undeath) — the Horde core does not route it | source: npcs.json + items.json + quests.json + quest-contracts.json
- Magister Hawkhelm | npc6647 | level 52 rare | single point (58.46, 30.89), center | no sole drop in the data (9295 Invisibility Potion is a 560-dropper world drop) | kill + note | source: npcs.json + items.json + quests.json
- Antilos | npc6648 | level 50 rare | single point (16.6, 54.1), west | no sole drop in the data | kill + note | source: npcs.json + items.json + quests.json
- Lady Sesspira | npc6649 | level 51 rare | single point (35.39, 55.69), center | no sole drop in the data (the rank-4 one is the rare; 239942 same-name regular is the quest-target lookalike, stays out per Dun Morogh) | kill + note | source: npcs.json + items.json + quests.json
- General Fangferror | npc6650 | level 51 rare | single point (41.31, 53.96), center | signature: Joonho's Mercy (item17054), sole dropper in the data; starts nothing, objective of nothing | kill + optional signature collect | source: npcs.json + items.json + quests.json
- Gatekeeper Rageroar | npc6651 | level 50 rare | single point (38.27, 32.08), center | no sole drop in the data | kill + note | source: npcs.json + items.json + quests.json
- Master Feardred | npc6652 | level 52 rare | 3 points (61.35, 24.92), (61.55, 24.25), (66.3, 16.72), north-east | no sole drop in the data | loop over all 3 | source: npcs.json + items.json + quests.json
- The Evalcharr | npc8660 | level 48 rare | single point (17.87, 65.6), west | no sole drop in the data | kill + note | source: npcs.json + items.json + quests.json
- Solid Chest | obj153451 | 13 fixed points, western arc | generic loop, said plainly | no loot table confirmed | source: objects.json
- Solid Chest | obj153453 | 12 fixed points, scattered | generic loop, said plainly (second same-name object, own step) | no loot table confirmed | source: objects.json
- Mossy Footlocker | obj179497 | 21 fixed points, scattered | generic loop, said plainly | no loot table confirmed | source: objects.json

Argued exclusions:
- Rank-2 anomalies (same as Alliance): Monnos the Elder npc6646 L54 and Scalebeard npc13896 L52 carry roles ["rare"] but are rank 2 (elites), not rank-4 rares — quest-target lookalikes stay out per Dun Morogh.
- Mammoth Shark (npc12125): rank 1, roles null, faction null, drops table null, zero sole-drop items anywhere in the data. It is the placed objective dropper of the broken record 91611 (OUT in the Horde census) — a quest-target lookalike with no rare flag and no signature loot, so NOT companion content per the standing exclusion.
- Unflagged but named (no rank flag, none shipped — same list as Alliance): Thundering Invader, Avalanchion, Scalebeard 244188, Elder Bramblesnap, Furze, Korsa. Above-band and unflagged (world-boss tier): Azuregos, Spirit of Azuregos, Maws.
- Quest-owned objects stay out: Azsharite formations, Kim'jael's Equipment, Saria's Knapsack, Hydraxis' Coffer (core content), the Ravencrest tablets/runes, tide pools, campfires and furniture (no loot). The Betrayed starter object 151286 (core 3506) is quest furniture, not treasure.
- Mining/herb nodes are gathering, fishing pools are not fixed treasure — never shipped.
- No Horde contract quest names any shipped rare as giver, ender, or kill objective (all 22 checked; every hit list empty). Fangferror's signature starts nothing and is no quest's objective.
- Item-start hunts: none. Quest 91607 (Pay Dirt!) has no start record in the data; the Horde core homes its accept at the ender Izvi Gildfizz (Ironforge precedent, documented there) and its objective (Humongous Crystal) drops from non-rare Cliff Walkers — no rare-dropped starter exists, so no hunt ships.
- Tame lines: none. The data has no tameability flag on any Azshara rare and the Horde core guide carries zero Hunter lines and no reference to any flagged rare. Logged in docs/companion-unverified.md instead of shipped as fact.

## azshara-horde-recipes.guide — 4 vendor-sold + 17 in-zone drops

Vendor-sold (both vendors neutral AH-faction, 1447-only spawns — Horde can buy; identical to Alliance, re-verified):
- Schematic: Deepdive Helmet | item10607 | buy from Jubie Gadgetspring, npc8678 [AH], (45.28, 90.95) | vendor-exclusive, zero droppers | Engineering | source: items.json vendors
- Pattern: Chimeric Gloves | item15729 | buy from Blimo Gadgetspring, npc12957 [AH], (45.21, 90.85) | vendor-exclusive, zero droppers | Leatherworking | source: items.json vendors
- Pattern: Blue Dragonscale Breastplate | item15751 | buy from Blimo [AH] | vendor-exclusive, zero droppers | Leatherworking | source: items.json vendors
- Pattern: Honed Blue Dragonscale Breastplate | item227898 | buy from Blimo [AH] | vendor-exclusive, zero droppers | Leatherworking | source: items.json vendors

Drops (in-zone droppers; every one a SOLE dropper in the data with zero object drops — all re-verified this round):
- Pattern: Ghostweave Belt | item14473 | Tailoring | collect from the Lingering Highborne, npc7864 (L48, 6 pts) — sole dropper | source: items.json drops
- Pattern: Ghostweave Cord | item254074 | Tailoring | collect from the Haldarr Trickster, npc6126 (L45, 4 pts) — sole dropper | source: items.json drops
- Pattern: Wicked Leather Bracers | item15728 | Leatherworking | collect from the Legashi Rogue, npc6201 (L51, 16 pts) — sole dropper | source: items.json drops
- Pattern: Stormshroud Armor | item15753 | Leatherworking | collect from the Arkkoran Oracle, npc6138 (L54, 20 pts) — sole dropper | source: items.json drops
- Pattern: Blue Dragonscale Shoulders | item15763 | Leatherworking | collect from the Cliff Breaker, npc6146 (L54, 24 pts) — sole dropper | source: items.json drops
- Pattern: Stormshroud Shoulders | item15764 | Leatherworking | collect from the Son of Arkkoroc, npc6144 (L54, 8 pts) — sole dropper | source: items.json drops
- Pattern: Honed Blue Dragonscale Shoulders | item227899 | Leatherworking | collect from the Cliff Breaker, npc6146 — sole dropper | source: items.json drops
- Pattern: Blue Suede Belt | item252886 | Leatherworking | collect from the Spitelash Battlemaster, npc7885 (L53, 18 pts) — sole dropper | source: items.json drops
- Pattern: Supple Scorpid Belt | item252929 | Leatherworking | collect from the Blood Elf Surveyor, npc6198 (L51, 11 pts) — sole dropper | source: items.json drops
- Pattern: Charged Scorpid Vest | item252932 | Leatherworking | collect from the Spitelash Siren, npc6195 (L50, 24 pts) — sole dropper | source: items.json drops
- Formula: Enchant Gloves - Greater Agility | item16219 | Enchanting | collect from the Legashi Rogue, npc6201 — sole dropper | source: items.json drops
- Formula: Enchant Gloves - Advanced Skinning | item249516 | Enchanting | collect from the Spitelash Myrmidon, npc6196 (L50, 24 pts) — sole dropper | source: items.json drops
- Recipe: Clam Linguine | item250189 | Cooking | collect from the Spitelash Enchantress, npc7886 (L54, 11 pts) — sole dropper | source: items.json drops
- Legashi Firewater Recipe | item235645 | profession tag absent in the data (ungated step with disclosure, Alliance precedent) | collect from the Legashi family (Satyr 6200, Rogue 6201, Hellcaller 6202, Soulstealer 236867, Hellraiser 236874, Blackguard 236876 — all 1447) — narrow named family; 244129 (Legashi Rogue, no spawns anywhere — phantom record, disclosed) | source: items.json drops + npcs.json
- Recipe: Superior Spellblasting Potion | item250980 | Alchemy | collect from the Spitelash Screamer, npc6193 (L47, 23 pts) — sole dropper | source: items.json drops
- Plans: Imperial Plate Gauntlets | item251441 | Blacksmithing | collect from the Blood Elf Reclaimer, npc6199 (L52, 18 pts) — sole dropper (the sole Blacksmithing source in-zone) | source: items.json drops
- Schematic: Spellpower Goggles Xtreme Plus | item16045 | Engineering | collect from the Spitelash Siren, npc6195 — sole dropper | source: items.json drops

Argued exclusions:
- Valormok vendors sell NO recipes: Kurll (npc3621 [H]) stocks weapons/goods (Falchion line + threads) and Gruul Darkblade (npc10361 [H]) stocks plain weapons — verified full stocks, zero recipe items. The Horde hub therefore adds no vendor source; both factions buy from the same two neutral vendors. Zero vendor deltas vs Alliance.
- The Alliance vendor Brinna Valanaar (npc14301 [A]) stocks only ammo and bows (verified full stock) — no Alliance-only recipe gap to log.
- Duke Hydraxis (npc13278 [AH]) sells a single non-recipe item (Enchanted Sigil: Flowing Waters, item228979) — not recipe content.
- Every other Azshara-dropping recipe is a generic multi-zone world drop (Elwynn rule — including the full Varo'then-table set at 400-650 droppers, and 9295 at 560 droppers despite Hawkhelm dropping it). Near-misses 13491 (Felwood second dropper), 14477 (EPL second dropper), 251438 and 252858 (dual-zone single-droppers, Felwood precedent) stay out. Quest-reward recipes are unverifiable — never shipped. Trainer-taught staples excluded.
- Professions with NO Azshara Horde source: First Aid and Fishing — stated in the guide, not padded (identical to Alliance).
