# Searing Gorge census (game data, accept-zone key 1427)

Source: local Forever game data (questie-forever quest/NPC/object/item
dumps, built with `--product wowf` + QuestieDB). Zones table: 1427 =
Searing Gorge (areaId 51). A quest belongs to Searing Gorge if its
accept/start is in 1427: start-NPC spawn zones, start-object spawn zones,
or start-item dropper spawn zones checked per quest; `zone` field used as
a cross-check only. Race mask 4294967373 = Alliance-accessible (it is the
mask on contracted Badlands/Blasted Lands quests); 8589934770 = Horde;
null = neutral (taken by the Alliance route). Objective types in this
zone's data are only item/kill/object/event.

Band **40-52**: accessible minLevels run m1 (5 writs + 1 Lunar elder,
optional, excluded from band logic per the Arathi/Hillsbrad precedent),
then a heavy m40 block (12), m43 (4), a heavy m45 block (13), m46 (2);
quest levels run 45-55 with the top own-levels (52: 3372/3463/3566)
carried by in-band minLevels. Break above m46: next minLevels are m50
(4264, contracted — a zone finale with an in-band minLevel per the band
rule), m55 (attunement twins + 7761, OUT), m58 (Bodley chain, OUT).
Below-band entry is free: the m40 chains (Suntara, Prayer, Kalaran,
Trinkets, Elemental LW) accept in-zone at their minLevel.

**IN 39 / OUT 49** (19 Horde set-aside, 25 above-band, 4 repeatable,
1 accepts-elsewhere).

## IN — 39

| ID | Title | Lvl/min | Giver / start | Disposition |
|----|-------|---------|---------------|-------------|
| 3181 | The Horn of the Beast | 48/40 | item 10000 Margol's Horn <- 5833 Margol the Rager, SG-only (73.52,82.31) | item-start IN; ender Pebblebitty is Loch Modan (expedition turn-in); next 3182 lives in Loch Modan (home guide) |
| 3367 | Suntara Stones | 48/40 | 8284 Dorius Stonetender (63.92,60.99) | escort event @74.47,19.44; next 3368 |
| 3368 | Suntara Stones | 48/40 | object 175704 Singed Letter (74.45,19.29) | object-start; ender Thorius is Ironforge (expedition turn-in); next 3371 Ironforge (out of scope, noted) |
| 3372 | Release Them | 52/40 | 8417 Dying Archaeologist (41.14,25.56) | accept-only in data (no end; 10442 artifact sourceless) — contracted with honest note; pre 3371 Ironforge is out-of-contract (structural warning); next 3566 |
| 3377 | Prayer to Elune | 50/40 | 8436 Zamael Lunthistle (29.57,26.29) | kill-the-giver objective; next 3378 |
| 3378 | Prayer to Elune | 50/40 | Zamael (29.57,26.29) | prayer drops off in-zone Twilight cultists; ender Astarii is Teldrassil/Darnassus (expedition turn-in) |
| 3379 | Shadoweaver | 50/46 | 8439 Nilith Lokrav (40.99,74.95), Tailoring | profession-gated; next 3385 |
| 3385 | The Undermarket | 50/46 | Nilith Lokrav, Tailoring | Kovic + Clunk kills, satchel off Kovic; next 3402 |
| 3402 | The Undermarket | 50/43 | Nilith Lokrav, Tailoring | ender Vizzklick is Tanaris (expedition turn-in) |
| 3441 | Divine Retribution | 48/40 | 8479 Kalaran Windblade (39.06,38.99) | kill-the-giver; next 3442 |
| 3442 | The Flawless Flame | 48/40 | Kalaran Windblade | hearts/flame off elementals, oil off golems/elementals (all in-zone) |
| 3443 | Forging the Shaft | 48/40 | Kalaran Windblade | 8x Thorium Plated Dagger drops off in-zone Dark Iron mobs per data (normal collect, not R5) |
| 3452 | The Flame's Casing | 50/40 | Kalaran Windblade | Symbol off in-zone Twilight cultists |
| 3453 | The Torch of Retribution | 50/40 | Kalaran Windblade | kill-the-giver; next 3454 |
| 3454 | The Torch of Retribution | 50/40 | Kalaran Windblade | accept-only in data (no end) — contracted with honest note; next 3462 |
| 3462 | Squire Maltrake | 50/40 | Kalaran -> 8509 Squire Maltrake (39.17,39) | next 3463 |
| 3463 | Set Them Ablaze! | 52/40 | Squire Maltrake | 4 braziers, all in-zone; next 3481 |
| 3481 | Trinkets... | 50/40 | object 149502 Hoard (38.85,38.99) | object-start, accept-only (no end; next 4022 Burning Steppes, out of scope) — contracted with honest note |
| 3566 | Rise, Obsidion! | 52/45 | 8417 Dying Archaeologist | heads off Lathoric + Obsidion (both in-zone); ender Thorius is Ironforge (expedition turn-in) |
| 4264 | A Crumpled Up Note | 58/50 | item 11446 <- 78 droppers incl. in-zone Anvilrage pack | item-start IN (SG is a genuine source); pre 4242 Burning Steppes out-of-contract (structural warning); ender Windsor has no spawn in data (note-only turn-in); next 4282 noted |
| 4449 | Caught! | 45/43 | object 173265 Wooden Outhouse (65.59,62.17) | object-start, accept-only (no end) — contracted with honest note; next 4450 |
| 4450 | Ledger from Tanaris | 46/43 | outhouse (65.59,62.17) | 20 shafts off in-zone Glassweb Spiders; ledger/package sourceless (chain note); flameberge off 9916 Jarquia, Swamp of Sorrows (expedition); ender Goodsteel is Tanaris (expedition turn-in) |
| 4451 | The Key to Freedom | 47/43 | item 11818 <- 6 in-zone Dark Iron droppers | item-start, accept-only (no end) — contracted with honest note |
| 5144 | Elemental Leatherworking | 55/40 | 7868 Sarah Tanner (63.56,75.97), LW225 | profession-gated; the SG variant — 5141 accepts Feralas, 5143 accepts TN/Feralas (see BORDERLINE) |
| 7701 | WANTED: Overseer Maltorius | 50/45 | board 179827 (37.65,26.47) | head off Maltorius (40.77,35.89); ender Longstriker in-zone |
| 7704 | Look at the Size of It! | 50/45 | item 18950 (sourceless) | item-start with bag note (Stormwind/Westfall handling); ender Sootsmoker in-zone |
| 7722 | What the Flux? | 50/45 | 14624 Burninate (38.8,28.51) | plans 18922 sourceless in data (Slag Pit note, R2); feeds the repeatable turn-ins (OUT) — the one-time pickup is IN |
| 7723 | Curse These Fat Fingers | 49/45 | 14627 Heavyhands (38.58,27.81) | 20 Heavy War Golems in-zone |
| 7724 | Fiery Menace! | 49/45 | Heavyhands | 20 Greater Lava Spiders in-zone |
| 7727 | Incendosaurs? Whateverosaur | 49/45 | Heavyhands | 20 Incendosaurs in-zone |
| 7728 | STOLEN: Smithing Tuyere... | 48/45 | board 179827 | tuyere off Steamsmith + spyglass off Lookout (both in-zone); ender Scrange in-zone |
| 7729 | JOB OPPORTUNITY: Culling... | 48/45 | board 179827 | 15 Taskmasters + 15 Slavers in-zone; ender Scrange in-zone |
| 81900 | The Burning Beast | 54/45 | object 441061 Weathered Etching (14.54,35.8) | object-start; ender Lynnore is Blasted Lands (expedition turn-in; chain continues in BL core 81917) |
| 8651 | Ironband the Elder | 60/m1 | 15567 Elder Ironband (21.46,78.97) | Lunar elder (EVENT=7): optional + seasonal note per TN precedent (see BORDERLINE) |
| 94263 | Craftsman's Writ: Fire Protection Potion | 60/m1 | item-start (sourceless writ) | bag note + when-skill Alchemy + optional (R5); ender Durganon in-zone |
| 94275 | Craftsman's Writ: Solid Sharpening Stone | 60/m1 | item-start (sourceless writ) | R5 Blacksmithing; ender Burninate in-zone |
| 94287 | Craftsman's Writ: Fire Goggles | 60/m1 | item-start (sourceless writ) | R5 Engineering; ender Durganon in-zone |
| 94299 | Craftsman's Writ: Nightscape Shoulders | 60/m1 | item-start (sourceless writ) | R5 Leatherworking; ender Sootsmoker in-zone |
| 94311 | Craftsman's Writ: Red Mageweave Pants | 60/m1 | item-start (sourceless writ) | R5 Tailoring; ender Longstriker in-zone |

No-turn-in records (5, Ironforge/Redridge precedent): 3372, 3454, 3481, 4449, 4451.

## OUT - Horde set-aside (19)

Badlands-accepting Kargath side (race 8589934770, qzone 1418, none in
the Badlands Alliance contract — excluded there too): 782, 793 (Gorn),
2202, 2203, 2258 (Jarkal reagent chain), 2338, 2339, 2340 (Jarkal
gem chain), 3821, 3906, 3907 (Thunderheart/Disharmony), 4061, 4062
(Rise of the Machines), 4081, 4082 (KILL ON SIGHT boards), 4134
(Lost Thunderbrew), 4768 (Darkstone Tablet), 7201 (Last Element).
Plus 8998 Back to the Beginning (Horde Mokvar variant of the Bodley
finale). The Horde block reconciles against this list.

## OUT - above-band (25)

Attunement twins 7487/7848 (min 55, Lothos Riftwaker) and 7761
Blackhand's Command (min 55, Quartermaster has an SG point at
43.3,99.2 but the quest is endgame) — iconic, but the band rule is
explicit. Bodley endgame chain 8961-8997 (min 58, 22 quests: 8961,
8962-8965 Components variants, 8966-8969 Left Piece variants,
8970, 8985-8988 More Components variants, 8989-8992 Right Piece
variants, 8994, 8995, 8996, 8997 Alliance finale) — a future endgame
round takes them, not this one.

## OUT - repeatable (4)

7736/7737/8241/8242 Restoring Fiery Flux Supplies + Gaining Acceptance
(`repeatable:true` + Thorium Brotherhood minRep in the data). The
one-time pickup 7722 that feeds them IS contracted.

## OUT - accepts elsewhere (1)

81955 A Mind of Metal (qzone 1458; Owen Thadd/Garion Wendell accepts
outside SG). Noted as a chain-link, not contracted.

## BORDERLINE

1. **Band 40-52 vs 43-52.** The brief expects mid-to-late 40s, but the
   data's minLevel cluster starts at 40 with 12 quests (Suntara, Prayer,
   Kalaran, Trinkets, Elemental LW). The band rule draws the TOP line;
   below-band entry is free. 40-52 keeps the cluster whole; 43-52 would
   orphan nothing (no quest is excluded by the low end either way) but
   would misstate where the zone starts. Picked 40-52.
2. **8651 Lunar elder IN.** The brief lists seasonal/event as OUT, but
   the Thousand Needles round contracted Lunar elders 8682/8724 as
   optional + seasonal note, lint-clean and verified. Consistency with
   the shipped pack beats the brief's generic rule; the note carries
   the seasonal caveat honestly. Butler rules on appeal.
3. **5144 vs 5141/5143.** Mutually exclusive LW variants (excl lists
   all three). 5141 starts in Feralas (1447), 5143 in TN/Feralas
   (1441/1444); 5144 starts with Sarah Tanner in SG. Chain-consistent
   SG variant contracted (94824/94817 + 7383/934 precedents); the other
   two stay out with their home zones named.
4. **4264 + 3181 item-starts with qzone elsewhere.** 4264's qzone is
   242 and 3181's is 1432, but their start items drop in SG (78
   Anvilrage droppers; Margol the Rager SG-only). The item-start rule
   keys on the source, not qzone — both IN, sequenced with sourcing
   notes so the route never wedges.
5. **8997/8998 variants.** The Alliance/Horde Bodley-finale pair would
   resolve to 8997 — except both sit at min 58, above the band, so the
   pair drops out together (8997 above-band, 8998 Horde set-aside).
6. **7722 feeds repeatables but is itself one-time.** Contracted: it is
   a normal pickup quest (pre for the rep cycle, not rep-flagged).
   The guide notes the plans have no placed source in the data.
7. **3372's pre (3371 Dwarven Justice, Ironforge) and 4264's pre
   (4242 Abandoned Hope, Burning Steppes) sit outside the contract.**
   Both accepts stay in the guide (their own accepts are in-zone);
   lint's structural pre-quest warnings are accepted with the chains
   named. Same for 3368 -> 3371 and 3481 -> 4022 links noted as
   out-of-scope pointers, and 4264 -> 4282.
