# Butler Routes — Zone Checklist

_Where every zone stands. Updated 2026-11-14 · Pack v0.8.0 · Repo: `cyork95/butler-routes-completionist` (`master`)_

**Pack principle (Cody, 2026-11-13): this is a COMPLETIONIST pack, not a leveling guide.** Every guide covers every quest in its zone — including the ones a leveling route would skip as XP-inefficient. The build order follows the sequence a player levels through the content, but that only decides which zone gets written next; inside a zone, efficiency shapes the route's order, never its quest selection.

**The pipeline every zone goes through:**

1. Census — the zone's quest list is pulled and verified
2. Core guide — the all-quests route is written
3. Lint/playtest clean — the compiler and simulated playtest pass
4. Cody pilot — Cody plays the guide live in game
5. Pilot fixes landed — whatever the pilot found is fixed and committed

Companions (Rares & Treasures · Recipes & Patterns) follow the core guide once the Zephras template is proven.

**Build order (Cody, 2026-11-13):** Zephras companions → **Westfall → Loch Modan → Darkshore**, with **Teldrassil alongside** → then **Alliance completion** (companions for every Alliance zone, plus all pilots and pilot fixes) → then the **Alliance city guides** (Stormwind → Ironforge → Darnassus — smaller guides, city quests) → then **Set 2** (Redridge Mountains → Ashenvale → Stonetalon Mountains → Duskwood) → then **Set 3** (Wetlands → Stranglethorn Vale → Riverglades → Thousand Needles → Desolace) → then **Set 4** (Hillsbrad Foothills → Arathi Highlands → Alterac Mountains → Moonglade → Dustwallow Marsh → Feralas → Tanaris) → then **Set 5** (Badlands → Blasted Lands → Searing Gorge → Felwood → Azshara → Un'Goro Crater) → then **Set 6** (everything left) → **the Horde block, last**: the Horde starting zones (Durotar, Mulgore, Tirisfal, Zephras twin) **plus all the Horde guides** — the Horde side of every shared and contested zone, and the Horde city guides (Orgrimmar → Thunder Bluff → Undercity) — so the pack ends with both factions holding a completionist path through the whole world.

---

## v1.0 scope — starting zones, both factions

### Zephras Isle — Skyborne (Alliance)

- [x] Census — 145 quests, tracker-verified
- [x] Core guide — `zephras-isle.guide`
- [x] Lint/playtest clean — 0 errors, playtest 0 stuck
- [ ] Cody pilot — Orinis, week of Nov 16
- [ ] Pilot fixes landed
- [x] Companion: Rares & Treasures — built, lint clean (0 errors / 0 warnings)
- [x] Companion: Recipes & Patterns — built, lint clean (0 errors / 0 warnings)

### Zephras Isle — Skyborne (Horde)

_Case B (audit-and-close round, pack 0.96.0): no separate twin - the shared `zephras-isle.guide` serves both factions. Census in `docs/zephras-isle-horde-census.md`: 121 Horde-applicable quests all routed with correct faction gates; only the `faction Alliance` header blocked Horde. Fixed by dropping the header (nil = either) in the core + both companions and gating 97973/98286 `only Alliance`._

- [x] Census - 121 Horde-applicable of 145 (24 Alliance-only set aside), `docs/zephras-isle-horde-census.md`
- [x] Core guide - shared `zephras-isle.guide` (Case B: header fix, no separate file)
- [x] Lint/playtest clean - 0 new errors; Horde personas (incl. Shaman) play 0 stuck
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - shared rares + recipes (headers fixed; all vendors neutral AH)

### Elwynn Forest — Human (Alliance)

- [x] Census — 83 quests, tracker-verified
- [x] Core guide — `elwynn-forest.guide`
- [x] Lint/playtest clean — 0 errors
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions — 24 rares + fixed containers, 4 vendor recipes, lint 0/0 (pilot pending)

### Westfall — follow-on zone (Alliance) · build order #1

- [x] Census — 43 quests, tracker-verified
- [x] Core guide — `westfall.guide`
- [x] Lint/playtest clean — 0 errors
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions — 14 rares + fixed containers, 10 recipes, lint 0/0 (pilot pending)

### Dun Morogh / Coldridge Valley — Dwarf & Gnome (Alliance)

_The lead-in for Loch Modan (build order #2)._

- [x] Census — 105 quests, local-data census (`docs/dun-morogh-census.md`)
- [x] Core guide — `dun-morogh.guide`
- [x] Lint/playtest clean — 0 errors, playtest 0 stuck
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions — 11 rares + fixed containers, 3 recipes, lint 0/0 (pilot pending)

### Loch Modan — second zone (Alliance) · build order #2

- [x] Census — 41 quests, local-data census (`docs/loch-modan-census.md`)
- [x] Core guide — `loch-modan.guide`
- [x] Lint/playtest clean — 0 errors, playtest 0 stuck
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions — 10 rares + figurine + fixed chests, 10 recipes, lint 0/0 (pilot pending)

### Teldrassil — Night Elf (Alliance) · alongside

- [x] Census — 96 quests, local-data census (`docs/teldrassil-census.md` + 934 addendum)
- [x] Core guide — `teldrassil.guide` (96 accepts / 96 turn-ins)
- [x] Micro-fix: quest 934 "Crown of the Earth" added to contract + route (was in no contract; accept-tested to Teldrassil, Darnassus fill expedition)
- [x] Lint/playtest clean — 0 errors, playtest 0 stuck
- [ ] Cody pilot — Ferinis is playing the zone now
- [ ] Pilot fixes landed
- [x] Companions

### Darkshore — second zone (Alliance) · build order #3

- [x] Census — 74 quests, local-data census (`docs/darkshore-census.md`)
- [x] Core guide — `darkshore.guide`
- [x] Lint/playtest clean — 0 errors, playtest 0 stuck
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions

### Durotar — Orc & Troll (Horde) · Horde block — last

- [x] Census
- [x] Core guide
- [x] Lint/playtest clean (106 quests, lint 0 errors; playtest: Horde personas, 0 stuck / 0 failed beyond R1/R2 residue)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (6 rares + Battered Chest loop + 5 rune objects; 4 recipes: 2 vendor Cooking, 2 narrow-drop Alchemy)

### Mulgore — Tauren (Horde) · Horde block — last

- [x] Census (74 quests, 2026-11-17 item-start addendum: 781 + 98424)
- [x] Core guide (74 quests)
- [x] Lint/playtest clean (72 quests, lint 0 errors; playtest: Horde personas, 0 stuck / 0 failed beyond R1 residue)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (9 rares, 13 recipes; Thunder Bluff city stock excluded)
### Tirisfal Glades — Undead (Horde) · Horde block — last

- [x] Census (109 quests, accept key 1420; Undercity city-rule set-asides)
- [x] Core guide (109 quests)
- [x] Lint/playtest clean (109 quests, lint 0 errors; playtest: Horde personas, 0 stuck / 0 failed beyond R1/R2 residue)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (12 rares, 10 treasures, 4 recipes)

**Publish rule (Cody, 2026-11-13): v1.0.0 waits for ALL of it** — every zone on this checklist, both factions and Set 2 included, done at first pass: core + companions written and lint-clean. Then the `v1.0.0` tag push fires the GitHub Actions publish to polestar.guide. Pilots and pilot-fix rounds continue after publish as v1.x updates. The build order follows zone progression; per the pack principle above, that orders the writing, never the content.

## Final QA — the pre-publish gate (Cody, 2026-11-15)

_Everything built is not the same as everything verified together. Before the v1.0.0 tag, the whole pack gets one full QA pass — the per-round checks are local; this pass is where cross-cutting failures would hide._

- [ ] Pack-as-shipped lint — the whole pack linted exactly as the publish workflow will zip it (not isolated per-zone copies): no duplicate IDs, header collisions, or folder mistakes
- [ ] Dangling-chain audit — every accepted out-of-contract pre-quest warning from every round (the 512/514 class) resolved or documented as genuinely unresolvable; no silent danglers in a completionist pack
- [ ] Journey playtests — simulated characters following the guides in leveling order across zone boundaries: band continuity, hearth points, and `next` links checked at the handoffs, not just inside zones
- [ ] Full goto re-audit — the mechanical goto audit re-run over ALL guides against a fresh data build, catching spawn drift from any Forever patch since each zone was written
- [ ] Public-text review — every guide read for leftover working notes, placeholder text, and references to Cody's characters or play; the pack ships to strangers
- [ ] Install rehearsal — the publish zip built locally the way the workflow builds it, installed into a clean AddOns folder, and every guide confirmed to load and open in Polestar
- [ ] In-game spot pilots — at least a sample of never-piloted mid-level zones run in game before strangers trust them
- [ ] QA fix round(s) landed — anything the pass finds is fixed on master and re-verified before the tag

---

## City guides — smaller guides (after the Alliance companion rounds)

_Cities are in scope as SMALLER guides (Cody, 2026-11-14): a census + core route for the quests that accept inside the city — the content the city rule has been setting aside since the Teldrassil round. Companions only where a city's data actually warrants one. The Horde cities (Orgrimmar → Thunder Bluff → Undercity) are part of the Horde block, last._

### Stormwind — Alliance capital

- [x] Census
- [x] Core guide
- [x] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (recipes built — 34 vendor recipes; no city rares, so no rares companion)

### Ironforge — Alliance capital

- [x] Census - 345 candidates, 188 IN / 157 OUT
- [x] Core guide - `ironforge.guide`
- [x] Lint/playtest clean - 0 errors, playtest 7 personas 0 stuck
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (recipes built — 46 vendor recipes; no city rares, so no rares companion)

### Darnassus — Alliance capital

_The 19 city-accept quests the Teldrassil census set aside land here._

- [x] Census - 132 candidates, 70 IN / 62 OUT
- [x] Core guide - `darnassus.guide`
- [x] Lint/playtest clean - 0 errors, playtest 14 persona-plays 0 stuck (R1 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (recipes built — 30 vendor recipes; no city rares, so no rares companion)

---

## Set 2 — the third zones (after the Alliance companion rounds, before the Horde block)

### Redridge Mountains — third zone (Alliance)

_Follows Westfall and Loch Modan._

- [x] Census - 46 candidates, 44 IN / 2 OUT
- [x] Core guide - `redridge.guide`
- [x] Lint/playtest clean - 0 errors, playtest 5 personas 0 stuck (R1+R2 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 8 rares (no loot in data) + containers incl. Lucius lockbox, 325 recipes (321 vendor + 4 exclusive drops), 0 lint errors/warnings

### Ashenvale — third zone (Alliance)

_Follows Darkshore._

- [x] Census - 112 candidates, 55 Alliance IN / 57 OUT (39 Horde set-aside for the Horde block)
- [x] Core guide - `ashenvale.guide`
- [x] Lint/playtest clean - 0 errors, playtest 9 personas 0 stuck (R1+R2+R5 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 12 rares (no loot in data) + 121 container placements, 19 recipes (9 vendor + 10 drops), 0 lint errors/warnings
- [x] Faction ungating (Option A, 2026-11-17)

### Stonetalon Mountains — contested (both factions)

_Off Ashenvale. Alliance route first; Horde content handled as the data dictates._

- [x] Census - 80 candidates, 40 Alliance IN / 40 OUT (32 Horde set-aside for the Horde block)
- [x] Core guide - `stonetalon.guide`
- [x] Lint/playtest clean - 0 errors, playtest 4 personas 0 stuck (R1+R2+R5 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 9 rares (no loot in data) + 56 container placements and Barrow Dens caches, 7 recipes (4 vendor + 3 drops), 0 lint errors/warnings
- [x] Faction ungating (Option A, 2026-11-17)

### Duskwood — third zone (Alliance)

_Follows Westfall. Raven Hill country._

- [x] Census - 102 candidates, 93 IN / 9 OUT
- [x] Core guide - `duskwood.guide`
- [x] Lint/playtest clean - 0 errors, playtest 3 personas 0 stuck (R1+R2+R5 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 6 rares (4 above-band with come-back-later notes) + 86-pt container loop and unique/marker steps, 14 recipes (9 vendor + 5 drops), 0 lint errors/warnings
- [x] Faction ungating (Option A, 2026-11-17) - 175 Alliance-only lines gated, header dropped, 0 dead lines

---

## Set 3 — the next tier (after Set 2, before the Horde block)

### Wetlands — follows Loch Modan (Alliance)

_Menethil Harbor. Sorinis is questing here now._

- [x] Census - 90 candidates, 87 IN / 3 OUT
- [x] Core guide - `wetlands.guide`
- [x] Lint/playtest clean - 0 errors, playtest 4 personas 0 stuck (R1+R2+R5 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 8 rares (7 in-band + 1 one-over with note) + 4 generic loops and 5 uniques, 16 recipes (12 vendor + 4 drops), 0 lint errors/warnings
- [x] Faction ungating (Option A, 2026-11-17) - 218 lines + 2 mask-pure steps step-gated to Alliance (11 double-only class lines carried by step gates), header dropped, 0 dead lines both factions

### Stranglethorn Vale — follows Duskwood / Redridge

_Booty Bay country._

- [x] Census - 258 candidates, 123 IN / 135 OUT
- [x] Core guide - `stranglethorn.guide`
- [x] Lint/playtest clean - 0 errors, playtest 4 personas + Rogue spot 0 stuck (R1+R2+R5 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 8 rares (6 with sole-drop signatures) + 9 fixed containers, 39 recipes (36 vendor + 3 drops), 0 lint errors/warnings
- [x] Faction ungating (Option A, 2026-11-17) - 83 Alliance-only lines gated, header dropped, 0 dead lines

### Riverglades — Forever-original zone

_Skyborne country._

- [x] Census - 178 candidates, 112 IN / 66 OUT (Horde set-aside)
- [x] Core guide - `riverglades.guide`
- [x] Lint/playtest clean - 0 errors, playtest 4 personas (Alliance + Horde) 0 stuck (R1+R2+R5 residue only)
- [x] Faction ungating (Option A, 2026-11-17) - 222 Alliance-only lines gated, header dropped, 0 dead lines both factions (races masks are the faction data; see the Horde census ruling)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 5 rares (5 with sole-drop signatures) + rock-pile container loop, 15 recipes (all vendor), 0 lint errors/warnings

### Thousand Needles — contested (Kalimdor)

- [x] Census - 67 candidates, 34 IN / 33 OUT (27 Horde set-aside)
- [x] Core guide - `thousand-needles.guide`
- [x] Lint/playtest clean - 0 errors, playtest 0 stuck (R1+R2 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 7 rares (all with sole-drop signatures, come-back notes for the 2 above-band), 18-pt Solid Chest loop, 9 recipes (4 vendor + 5 exclusive/narrow drops)
- [x] Faction ungating (Option A, 2026-11-17)

### Desolace — contested (Kalimdor)

- [x] Census - 89 candidates, 56 IN / 33 OUT (29 Horde set-aside)
- [x] Core guide - `desolace.guide`
- [x] Lint/playtest clean - 0 errors, playtest 0 stuck (R1+R2 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 5 rares (4 sole-drop signatures + kill-note Hissperak; Cursed Centaur excluded above-band), 31-pt treasure (25 chest + 6 battered), 21 recipes (18 vendor + 3 exclusive drops)
- [x] Faction ungating (Option A, 2026-11-18) - 36 Alliance-only lines gated (5 added this round, incl. Paladin,Alliance composition), header dropped, 0 dead lines both factions

---

## Set 4 — the next tier (after Set 3, before the Horde block)

### Hillsbrad Foothills — contested

- [x] Census - 60 candidates, 37 IN / 23 OUT (10 Horde set-aside)
- [x] Core guide - `hillsbrad.guide`
- [x] Lint/playtest clean - 0 errors, playtest 4 personas (Alliance + Horde) 0 stuck (R1+R2+R5 residue only)
- [x] Faction ungating (Option A, 2026-11-18) - 93 Alliance-only lines gated (39 added this round), header dropped, 0 dead lines both factions
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 7 rares + containers, 29 recipes (25 vendor + 4 exclusive drops), 0 lint errors/warnings

### Arathi Highlands — contested

- [x] Census - 117 candidates, 47 IN / 70 OUT (50 Horde set-aside)
- [x] Core guide - `arathi.guide`
- [x] Lint/playtest clean - 0 errors, playtest 0 stuck (R1+R2+R5 accepted only)
- [x] Faction ungating (Option A, 2026-11-18)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 9 rares (no loot in data) + containers incl. Illari cache, 23 recipes (15 vendor + 8 drops), 0 lint errors/warnings

### Alterac Mountains — contested

- [x] Census - 164 candidates, 20 IN / 144 OUT (67 Horde set-aside)
- [x] Core guide - `alterac.guide`
- [x] Lint/playtest clean - 0 errors, playtest 0 stuck (R2+R5 writ residue only)
- [x] Faction ungating (Option A, 2026-11-17)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 7 rares (no loot in data, incl. dual-zone Jimmy) + 52 container placements, 26 recipes (22 vendor + 4 drops), 0 lint errors/warnings

### Moonglade — the druid thing (special handling)

_Not a standard zone route: Moonglade is the druid class hub. This guide covers the druid class content centred there — the form quests and class chains — written for druids, not a general completionist route._

- [x] Census
- [x] Core guide - `moonglade.guide`
- [x] Lint/playtest clean - 0 errors, playtest 0 stuck (R1 expedition residue only)
- [x] Faction ungating (Option A, 2026-11-17)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - recipes shipped (8 vendor buys in `moonglade-recipes.guide`); rares/treasures none in data (0 rares, 1 seasonal event barrel)

### Dustwallow Marsh — contested (Kalimdor)

- [x] Census
- [x] Core guide - `dustwallow.guide`
- [x] Faction ungating (Option A, 2026-11-17) - 51 Alliance-only lines gated (incl. `only Paladin,Alliance` composition), header dropped, 0 dead lines both factions
- [x] Lint/playtest clean - 0 errors, playtest 0 stuck (R1/R2/R5 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 10 rares + fixed containers; 9 recipes (4 vendor + 5 drops)

### Feralas — contested (Kalimdor)

- [x] Census - 107 candidates, 57 IN / 50 OUT (41 Horde set aside)
- [x] Core guide - `feralas.guide`
- [x] Lint/playtest clean - 0 errors, playtest 3 personas 0 stuck (R1+R2+R5 residue only)
- [x] Faction ungating (Option A, 2026-11-17)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 9 rares (7 with sole-drop signatures) + 3 fixed containers, 24 recipes (13 vendor + 11 drops), 0 lint errors/warnings

### Tanaris — contested (Kalimdor)

- [x] Census - 162 candidates, 91 IN / 71 OUT (10 Horde set aside)
- [x] Core guide - `tanaris.guide`
- [x] Lint/playtest clean - 0 errors, playtest 7 personas 0 stuck (R1+R2 residue + 1 R3 warning, all documented)
- [x] Faction ungating (Option A, 2026-11-17)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 10 rares (6 with sole-drop signatures) + 6 fixed containers, 25 recipes (16 vendor + 9 drops), 0 lint errors/warnings

---

## Set 5 — the next tier (after Set 4, before the Horde block)

### Badlands — contested (Eastern Kingdoms)

- [x] Census - 77 candidates, 35 IN / 42 OUT (35 Horde set aside)
- [x] Core guide - `badlands.guide`
- [x] Lint/playtest clean - 0 errors, playtest 3 personas 0 stuck (R1/R2/R5 residue, all documented)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 6 rares (3 with sole-drop signatures) + 10 fixed containers, 8 recipes (2 vendor + 6 drops), 0 lint errors/warnings
- [x] Faction ungating (Option A, 2026-11-17) - 32 Alliance-only lines + 4 soft-pre minis gated, header dropped, 0 dead lines both factions

### Blasted Lands — contested (Eastern Kingdoms)

- [x] Census - 33 candidates, 21 IN / 12 OUT (0 Horde set aside)
- [x] Core guide - `blasted-lands.guide`
- [x] Lint/playtest clean - 0 errors, playtest 3 personas 0 stuck (R1 expedition residue, all documented)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 5 rares (3 sole-drop signatures + come-back notes for above-band), 8-pt Solid Chest loop, 2 recipes (1 vendor + 1 exclusive drop)

### Searing Gorge — contested (Eastern Kingdoms)

- [x] Census - 88 candidates, 39 IN / 49 OUT (19 Horde set aside)
- [x] Core guide - `searing-gorge.guide`
- [x] Lint/playtest clean - 0 errors, 36 warnings (all dispositioned), playtest 0 stuck (R1+R2+R5 residue only)
- [x] Faction ungating (Option A, 2026-11-17)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 9 rares (4 sole-drop signatures, 4 kill-note, Quartermaster come-back + bank note), 32-pt treasure (15 chest + 17 footlocker), 9 recipes (all exclusive drops)

### Felwood — contested (Kalimdor)

- [x] Census
- [x] Core guide (59 quests, band 45-55)
- [x] Lint/playtest clean (0 errors; 45 accepted warnings; playtest 0 stuck, residue R1x47/R2x36/R5x33)
- [x] Faction ungating (Option A, 2026-11-17)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 7 rares (2 sole-drop signatures, 5 kill-note), 19-pt treasure (13 troll + 3 battered + 2 solid + worn + Arko chest), 9 recipes (8 exclusive drops + Meilosh vendor-or-drop)

### Azshara — contested (Kalimdor)

- [x] Census — 95 examined, 52-contract Alliance route
- [x] Core guide — `azshara.guide`
- [x] Lint/playtest clean — 0 errors, 30 accepted warnings; playtest 0 stuck (R1+R5 expedition residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions — 8 rares (1 sole-drop signature Joonho’s Mercy, 7 kill-note, incl. Varo’then core pointer; Feardred loops 3 pts), 46-pt treasure (13 + 12 solid chests + 21 mossy footlockers), 21 recipes (17 exclusive drops + 4 neutral-vendor)
- [x] Faction ungating (Option A, 2026-11-17) - 54 Alliance-only lines + 1 soft-pre mini gated (step split for the shared 8236 mini), header dropped, 0 dead lines both factions

### Un'Goro Crater — contested (Kalimdor)

- [x] Census
- [x] Core guide
- [x] Lint/playtest clean (42/42, 0 errors)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions — 3 rares (no signature loot; rank-2 Gruff/Mosh excluded per rank rule), no confirmed treasure (rares-only), 10 recipes (LW 9 + Cooking 1)
- [x] Faction ungating (Option A, 2026-11-17) — 7 Alliance-only lines + 1 soft-pre mini step-gated, header dropped, 0 dead lines both factions

---

## Set 6 — everything left (after Set 5, before the Horde block)

### Silverpine Forest — Horde second zone

_Horde heartland — a Horde-faction route, written here in leveling order, ahead of the Horde starting block._

- [x] Census (67-contract, band 10-20)
- [x] Core guide (67 accepts, 66 turn-ins + documented 78261)
- [x] Lint/playtest clean (0 errors; R1/R2/R3 residue only)
- [x] Alliance addendum — 5 quests (the Alliance-only accepts incl. the Modera trio)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (7 rares + treasures; 17 vendor buys + Rot Hide drop)
- [x] Faction ungating (Option A, 2026-11-17)

### The Barrens — Horde second zone

_Horde heartland — a Horde-faction route, written here in leveling order, ahead of the Horde starting block._

- [x] Census (157 IN, 141 OUT)
- [x] Core guide (157 accepts, 157 turn-ins)
- [x] Lint/playtest clean (0 errors; R1/R2/R5 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (32 rares + treasures; 70 recipes)
- [x] Faction ungating (Option A, 2026-11-17)

### Swamp of Sorrows — contested (Eastern Kingdoms)

- [x] Census (19 IN, 33 OUT)
- [x] Core guide (19 accepts, 19 turn-ins)
- [x] Lint/playtest clean (0 errors; R1/R2/R5 residue only)
- [x] Faction ungating (Option A, 2026-11-17)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (5 rares + treasures; 2 vendor buys + 5 mob drops)

### The Hinterlands — contested (Eastern Kingdoms)

- [x] Census (14 IN, 76 OUT)
- [x] Core guide (14 accepts, 14 turn-ins)
- [x] Lint/playtest clean (0 errors; 7 XP-noise + 1 structural pre-quest warning)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (10 rares, 1 generic-containers loop; 15 recipes: 8 vendor, 7 drop)
- [x] Faction ungating (Option A, 2026-11-17) - 25 Alliance-only quest lines + 7 Alliance-attributed kill lines gated, header dropped, 0 dead lines both factions

### Western Plaguelands — contested (Eastern Kingdoms)

- [x] Census (65 quests, band 50-58)
- [x] Core guide (65 accepts / 62 turn-ins + 3 documented accept-only records)
- [x] Lint/playtest clean (0 errors; XP-noise + structural + sourceless warnings argued)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (10 rares + 35-pt container sweep; 16 drop recipes, 0 vendors in-zone)
- [x] Faction ungating (Option A, 2026-11-17) - 36 Alliance-only quest lines + 7 Alliance-attributed kill lines + 1 soft-pre mini gated, header dropped, 0 dead lines both factions

### Eastern Plaguelands — contested (Eastern Kingdoms)

- [x] Census (76 quests, band 50-60)
- [x] Core guide (76 accepts / 76 turn-ins)
- [x] Lint/playtest clean (0 errors; XP-noise + structural + door-face warnings argued)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (11 rares + 7 fixed-container loops + 7 singles; 21 recipes: 19 vendor, 2 drop)
- [x] Faction ungating (Option A, 2026-11-17) - 74 lines for 29 Alliance quests gated, 0 minis, 0 travel, header dropped, 0 dead lines both factions

### Burning Steppes — contested (Eastern Kingdoms)

- [x] Census (59 quests, band 48-60)
- [x] Core guide (59 accepts / 59 turn-ins)
- [x] Lint/playtest clean (0 errors; XP-noise + structural + sourceless-craft warnings argued)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (11 rares + 4 fixed-container loops + 2 singles; 10 recipes: 1 vendor, 9 drop)
- [x] Faction ungating (Option A, 2026-11-17)

### Deadwind Pass — contested (Eastern Kingdoms)

- [x] Census (1 quest, band 60-60)
- [x] Core guide (1 accept / 1 turn-in)
- [x] Lint/playtest clean (0 errors, 0 warnings; R2 + R5 sourceless-writ residue argued)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (no rares in data; 3 treasure singles; 2 recipes, both sole-source drops)

### Winterspring — contested (Kalimdor)

- [x] Census (48 quests, band 47-60)
- [x] Core guide (48 accepts / 48 turn-ins)
- [x] Lint/playtest clean (0 errors, 59 warnings in 4 argued classes; R1 + R5 residue, 0 stuck)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (7 rares, 1 chest loop; 23 recipes: 13 vendor + 10 zone-exclusive drops)

### Silithus — contested (Kalimdor)

- [x] Census (52 quests, band 54-60)
- [x] Core guide (52 accepts / 52 turn-ins)
- [x] Lint/playtest clean (0 errors, 41 warnings in 3 argued classes; R1 + R2 + R5 residue, 0 stuck)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (4 rares, 3 unique treasures; 52 recipes: 50 vendor + 2 zone-narrow drops)

### Mount Hyjal — Kalimdor

_Content as the game data dictates._

- [x] Census (123 quests, band 54-60, accept key 2482)
- [x] Core guide (123 accepts / 121 turn-ins + 2 non-contract soft-pre turn-ins 93773/92009; 95793 rides both turn-in lines)
- [x] Lint/playtest clean (0 errors, 35 warnings in 3 argued classes; R1 + R5 residue, 0 stuck)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (8 rares, 0 treasures in data; 80 recipes: 78 vendor + 2 zone-narrow drops)

### Shen'dralas — Forever-original zone

_No public rare data yet — its census leans on game data._

- [x] Census (28 quests, band 30-49, accept key 2652)
- [x] Core guide
- [x] Lint/playtest clean (lint 0 errors; playtest residue R1x2 + R5x1 only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (0 rares in data, treasures-only rares guide: 1 loop + 1 single; 1 recipe: Blacksmithing drop)
- [x] Faction ungating (Option A, 2026-11-17) - 0 Alliance-only lines (all-shared contract) + 0 minis, header dropped, 0 dead lines both factions

## The Horde block — Horde sides, Horde cities, and addenda

_Per Cody's build order, the Horde block runs last: the Horde starting zones (tracked in their own sections above — Durotar, Mulgore, Tirisfal Glades, the Zephras Isle twin) plus ALL the Horde guides below. Every Horde guide is its own file and its own contract (the Silverpine precedent: `silverpine.guide` for the Horde route, `silverpine-alliance.guide` for the other faction's piece) — never merged into the Alliance file. Each Horde census reconciles against the set-aside IDs its zone's Alliance census banked. The Horde heartland zones written Horde-first (Silverpine Forest, The Barrens) are tracked in their own sections above. **Blasted Lands has NO Horde side** — its census proved zero Horde quests in the data, double-evidenced — so it has no section here._

### Orgrimmar — Horde capital

_City guide per the Alliance city pattern: a census + compact core for the quests that accept inside the city. Companions only where the data warrants._

- [x] Census (173 quests, span 1-60)
- [x] Core guide
- [x] Lint/playtest clean (0 errors; R1/R2/R5 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (recipes built - 119 vendor recipes; no city rares, so no rares companion)

### Thunder Bluff — Horde capital

_City guide per the Alliance city pattern: a census + compact core for the quests that accept inside the city. Companions only where the data warrants._

- [x] Census — 155 candidates, 78 IN (Mulgore 150 reconciled)
- [x] Core guide — `thunder-bluff-city.guide`
- [x] Lint/playtest clean — 0 errors, playtest residue R1/R5 only
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (recipes built - 28 vendor recipes; no city rares, so no rares companion)

### Undercity — Horde capital

_City guide per the Alliance city pattern: a census + compact core for the quests that accept inside the city. Companions only where the data warrants._

- [x] Census — 108 quests, city key 1458
- [x] Core guide — `undercity-city.guide`
- [x] Lint/playtest clean — 0 errors, residue R1/R2 only
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (recipes built - 33 vendor recipes; no city rares, so no rares companion)

### Ashenvale — Horde

- [x] Census - 39 banked set-asides reconciled (35 IN; 8266/8296 repeatable OUT, 79098/95042 broken OUT, 3/4 phantom), docs/ashenvale-horde-census.md
- [x] Core guide - ashenvale-horde.guide (35 quests, band 19-30)
- [x] Lint/playtest clean - lint 0 errors, 20 warnings all argued; playtest 3 Horde personas, 0 stuck, residue R1/R2/R5 only
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (rares: 11 rares + 4 item-start hunts + fixed containers; recipes: 2 vendor + 10 narrow mob drops; both 0 errors / 0 warnings)

### Stonetalon Mountains — Horde

- [x] Census - 32 banked set-asides reconciled (23 IN; 6568/6602 above-band, 97446 mount/broken, 6x zone-1413 already in Barrens contract), docs/stonetalon-horde-census.md
- [x] Core guide - stonetalon-horde.guide (23 quests, band 12-30)
- [x] Lint/playtest clean - lint 0 errors; playtest 2 Horde personas, 0 stuck, residue R1/R2/R5 only
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (rares: 9 rares + fixed containers; recipes: 3 vendor + 4 narrow mob drops; both 0 errors / 0 warnings)

### Duskwood — Horde

- [x] Census - 100 zone-field records + 1 spawn-pull; 5 Horde IN (1372-1391 chain + 94241 writ), 92 already contracted (not duplicated), 4 OUT, docs/duskwood-horde-census.md
- [x] Core guide - duskwood-horde.guide (5 quests, band 37-42 + L60 writ special)
- [x] Lint/playtest clean - 0 errors; playtest Horde personas, 0 stuck, residue R1/R2/R5 only
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions (rares: 6 below-band rares + 68-pt container loop + 3 uniques + 6 markers; recipes: 4 neutral-vendor + 5 in-zone drops; both 0 errors / 0 warnings)

### Stranglethorn Vale — Horde

- [x] Census - 258 zone-1434 records (39 Horde / 35 Alliance / 184 null by races mask); 39 Horde IN, 0 OUT, 123 Alliance-contracted not duplicated, docs/stranglethorn-horde-census.md
- [x] Core guide - stranglethorn-horde.guide (39 quests, band 30-47; 5148 + 8116-8119 above-band with gates noted)
- [x] Lint/playtest clean - 0 errors; honest playtest Horde personas (Orc Warrior/Shaman), residue R1/R5 only (expedition legs + bag-note objectives)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 8 rares + 51-pt container loop + 5 uniques; 65 recipes (58 vendor + 7 narrow drops); both guides 0 errors / 0 warnings

### Riverglades — Horde

- [x] Census - 178 zone-2548 records (83 Alliance / 66 Horde / 29 neutral by races mask); 66 Horde IN, 0 OUT, 29 neutral not duplicated, docs/riverglades-horde-census.md
- [x] Core guide - riverglades-horde.guide (66 quests, band 35-45, map-1444 expedition)
- [x] Lint/playtest clean - 0 errors; playtest Horde personas (Orc Warrior/Shaman/Hunter), 0 stuck, residue R1/R5 only (bag-note items + expedition leg)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 5 rares (all sole-drop signatures, Reginald as killable opposition) + Rock Pile loop, 13 vendor recipes (12 port + Naluk), 0 lint errors/warnings

### Thousand Needles — Horde

- [x] Census - 26 Horde IN at band 20-32, 27/27 set-asides reconciled, docs/thousand-needles-horde-census.md
- [x] Core guide - thousand-needles-horde.guide (26 quests, Freewind Post + expedition legs)
- [x] Lint/playtest clean - 0 errors; honest playtest Horde personas, 0 stuck, residue R1/R2 only
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 7 rares (4 in-band + 3 come-back notes, all sole-drop signatures) + 2 item-start hunts + 18-pt chest loop + crate note, 9 recipes (4 vendor + 5 drops), 0 lint errors/warnings

### Desolace — Horde

- [x] Census - 89 zone-1443 records (29 Horde / 15 Alliance / 45 null by races mask); 25 Horde IN, 4 OUT, docs/desolace-horde-census.md
- [x] Core guide - desolace-horde.guide (25 quests, band 31-45; 93045 + 4 expeditions)
- [x] Lint/playtest clean - 0 errors; honest playtest Horde personas, residue R1 only (4 expedition legs)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 6 rares + 1480 hunt, 25 Solid + 6 Battered + 10 footlocker pts + 3 unique objects, 38 recipes (32 vendor + 6 drops), 0 lint errors/warnings

### Hillsbrad Foothills — Horde

- [x] Census - 60 zone-1424 records (44 Alliance / 10 Horde / 4 neutral + 2 race-masked); 10 Horde IN, 0 OUT, docs/hillsbrad-horde-census.md
- [x] Core guide - hillsbrad-horde.guide (10 quests, band 19-32, 5 dedicated soft-pre minis)
- [x] Lint/playtest clean - 0 errors; playtest Horde personas (Orc/Scourge/Paladin), 0 stuck, residue R5 only (bag-note key + spawnless-target turn-ins)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 7 rares (all sole-drop signatures, 2 as killable opposition) + Fixed Chests loop + Shindigger Kegs, 20 recipes (14 vendor + 6 narrow drops), 0 lint errors/warnings

### Arathi Highlands — Horde

- [x] Census - 29 IN (50/50 set-asides reconciled), band 30-40 + L60 writ special
- [x] Core guide - `arathi-horde.guide`
- [x] Lint/playtest clean - 0 errors, playtest 0 stuck (R1+R2+R5 accepted only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 10 rares (8 in-band + Foulbelly/Nazjak come-back-later) + Fixed Chests loop + 11 uniques, 16 recipes (9 vendor + 7 narrow drops), 0 lint errors/warnings

### Alterac Mountains — Horde

- [x] Census - 67 pool records, 50 IN / 17 OUT (67/67 banked set-asides reconciled), band 20-45, docs/alterac-horde-census.md
- [x] Core guide - `alterac-horde.guide` (50 quests, band 20-45, 2 soft-pre minis + expedition legs)
- [x] Lint/playtest clean - 0 errors; playtest Horde personas incl. Orc/Tauren Shaman, 0 stuck (R1 expedition + R5 bag-note residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 8 rares, 73-pt container loop + 2 unique objects, 20 vendor + 4 drop recipes, 0 lint errors/warnings

### Dustwallow Marsh — Horde

- [x] Census - 69 zone-1445 records (27 Alliance / 15 Horde / 24 neutral + 1 Human-only); 5 Horde IN, 10 OUT above-band, docs/dustwallow-horde-census.md
- [x] Core guide - dustwallow-horde.guide (5 quests, band 30-45, 1 dedicated soft-pre mini + Barrens expedition turn-in)
- [x] Lint/playtest clean - 0 errors; playtest Horde personas (Orc/Shaman/Hunter), 0 stuck, residue R1 only (Barrens expedition leg)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 12 rares (all sole-drop signatures, 2 as killable opposition) + Fixed Chests loop (91 pts) + Gizmorium Crate, 14 recipes (9 vendor + 5 narrow drops), 0 lint errors/warnings

### Feralas — Horde

- [x] Census - 41 Horde-mask pool records (41/41 banked set-asides reconciled: 39 IN / 2 OUT above-band), band 38-50, docs/feralas-horde-census.md
- [x] Core guide - `feralas-horde.guide` (39 quests, band 38-50, Camp Mojache hub + capital/out-zone expedition legs)
- [x] Lint/playtest clean - 0 errors, 43 warnings in accepted classes; playtest Horde personas 0 stuck (R1 expedition + R2 sourceless residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Tanaris — Horde

- [x] Census - 10 Horde-mask pool records (10/10 banked set-asides reconciled), 7 IN / 3 OUT, band 38-50, docs/tanaris-horde-census.md
- [x] Core guide - `tanaris-horde.guide` (7 quests, band 38-50, 1 soft-pre mini + 3 capital expeditions)
- [x] Lint/playtest clean - 0 errors; playtest Horde personas, 0 stuck (R1 expedition + R2/R5 sourceless residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Badlands — Horde

- [x] Census (reconcile against 35 set-asides banked by the Alliance census) - 77 zone-1418 records (35 Horde / 29 neutral / 13 Alliance by races mask); 13 Horde IN (band 30-40), 22 OUT argued, docs/badlands-horde-census.md
- [x] Core guide - badlands-horde.guide (13 quests, band 30-40, Kargath hub + 3 expedition legs)
- [x] Lint/playtest clean - 0 errors; playtest Horde personas in band, 0 stuck; residue R1 expedition leg only (Orgrimmar continent change)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Searing Gorge — Horde

- [x] Census - 88 records on key 1427 (81 placed + 7 sourceless), zero in-band Horde-only accepts; Kargath 18 homed to Badlands (Horde) (8 IN / 10 OUT above-band); 8998 ruled OUT (Bodley accept, min58, endgame) — docs/searing-gorge-horde-census.md
- [ ] Core guide (no micro-contract: section closed by census)
- [x] Lint/playtest clean - main-guide ungating verified (0 errors; warned IDs identical to baseline; both-faction playtest 0 stuck, dead-line 0 violations)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Felwood — Horde

- [x] Census - 13 Horde-mask pool records (banked 21 reconciled: 13 in-zone + 7 Darkshore-zone + 1 Ashenvale-zone, contracted), band 45-48, docs/felwood-horde-census.md
- [x] Core guide - `felwood-horde.guide` (8 quests, band 45-48, profession-gated salve chain)
- [x] Lint/playtest clean - 0 errors; playtest Horde personas, 0 stuck (R1 expedition + R5 bag-note residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Azshara — Horde

- [x] Census (reconcile against 30 set-asides banked by the Alliance census) - 82 zone-1447 records (23 Horde / 19 Alliance / 40 null by races mask) + 13 off-key ledger IDs = 95 with the Alliance ledger, none missing; 22 Horde IN (band 44–50), 8 OUT argued, docs/azshara-horde-census.md
- [x] Core guide - azshara-horde.guide (22 quests, band 44–50, west hub + east camp + 4 expedition legs)
- [x] Lint/playtest clean - 0 errors; playtest Horde personas in band, 0 stuck; residue R1 expedition legs only
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Un'Goro Crater — Horde

- [x] Census (3 IN at band 47-53; Larion chain 4145/4147/4148; 4146/94399/98093 OUT argued; 8-vs-5 reconciled to the census's named 5)
- [x] Core guide — `ungoro-horde.guide`
- [x] Lint/playtest clean (3/3 + intentional non-contract 4146 mini turnin, 0 errors, 1 accepted R2 warning)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Swamp of Sorrows — Horde

- [x] Census - 17 Horde-mask pool records (17/17 banked set-asides reconciled: 12 IN / 5 OUT), band 30-38, docs/swamp-of-sorrows-horde-census.md
- [x] Core guide - `swamp-of-sorrows-horde.guide` (12 quests, band 30-38, 1 soft-pre mini + 2 capital expeditions)
- [x] Lint/playtest clean - 0 errors; playtest Horde personas, 0 stuck (R1 expedition + R5 bag-note residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### The Hinterlands — Horde

- [x] Census (reconcile against 25 set-asides banked by the Alliance census — the Revantusk block) - 38 zone-1425 records (23 Horde / 8 Alliance / 7 null by races mask) + city-rule sweep, no beyond-25 Horde; 25 Horde IN (band 38–46), 0 banked OUT, docs/the-hinterlands-horde-census.md
- [x] Core guide - the-hinterlands-horde.guide (25 quests, band 38–46, Revantusk hub + 4 expedition legs)
- [x] Lint/playtest clean - 0 errors; playtest Horde personas in band, 0 stuck; residue R1 expedition legs only
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Wetlands — Horde

- [x] Census (1 IN: 95682 Open the Maw by in-zone giver geography, band 24-31; 97171 OUT hollow + above-band; item-start scan clean)
- [x] Core guide — `wetlands-horde.guide` (single-quest micro-guide at the Deathstalker Agent)
- [x] Lint/playtest clean (1/1, 0 errors, 2 accepted warnings: structural pre in arathi-horde + unplaced dispatch objective)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Moonglade — Horde (Druid)

- [x] Census - 18 Horde-mask pool records (18/18 banked set-asides reconciled), span 10-20, docs/moonglade-horde-census.md
- [x] Core guide - `moonglade-horde.guide` (18 quests, span 10-20, Tauren/Skyborne-gated lines)
- [x] Lint/playtest clean - 0 errors (XP-model noise only); playtest Horde druid personas + non-druid, 0 stuck, 0 residue
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Western Plaguelands — Horde

- [x] Census (20 banked Horde set-asides reconciled + 6 rule-excluded crafting records; 19 Horde IN (band 54–58), 1 broken + 6 rule-excluded OUT, docs/western-plaguelands-horde-census.md)
- [x] Core guide - western-plaguelands-horde.guide (19 quests, band 54–58, Bulwark hub + 2 expedition legs)
- [x] Lint/playtest clean - 0 errors; playtest Horde personas in band, 0 stuck; residue R1 expedition legs only
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Eastern Plaguelands — Horde

- [x] Census (9 Horde IN, band 50-60; rogue block homed in undercity-city, 15/15 set-asides reconciled)
- [x] Core guide - `eastern-plaguelands-horde.guide` (9 accepts / 9 turn-ins, 8 soft-pre minis)
- [x] Lint/playtest clean (0 errors, 11 warnings in accepted classes; 4 Horde personas 0 fails)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Burning Steppes — Horde

- [x] Census (3 Horde IN: 4121/3822/8998, band 48-58; 3/3 banked set-asides reconciled; Krom'Grul + Bodley accept-geography rulings)
- [x] Core guide - `burning-steppes-horde.guide` (3 accepts / 3 turn-ins + 2 documented non-contract soft-pre turn-ins 3821/4122; Grark/Bodley/Sha'ni camps + Badlands/Orgrimmar expeditions)
- [x] Lint/playtest clean (0 errors, 3 warnings in accepted classes; Orc Warrior + Orc Shaman 0 stuck, R1 Orgrimmar-leg residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Deadwind Pass — Horde

- [ ] Census (set-asides counted when the zone's Alliance census runs)
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Winterspring — Horde

- [ ] Census (set-asides counted when the zone's Alliance census runs)
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Silithus — Horde

- [ ] Census (set-asides counted when the zone's Alliance census runs)
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Mount Hyjal — Horde

- [ ] Census (set-asides counted when the zone's Alliance census runs)
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Shen'dralas — Horde

- [x] Census (4 banked Horde-gated set-asides reconciled + full-pool 2652 sweep, no others; 4 IN (band 30–35), 0 OUT, docs/shendralas-horde-census.md)
- [x] Core guide - shendralas-horde.guide (4 quests, band 30–35, Nerlokh chain + Desolace expedition leg)
- [x] Lint/playtest clean - 0 errors; playtest Horde personas in band, chain fires end-to-end (0 stuck; residue R1 expedition leg only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### The Barrens — Alliance addendum

_The mirror of the Silverpine Alliance addendum: the Alliance quests the Barrens' Horde census set aside._

- [ ] Census (reconcile against 17 set-asides banked by the Barrens census)
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

---

## Beyond v1.0 — every other open-world zone

_Every open-world zone is now assigned to a set — nothing remains here._

**Out of scope by design:** dungeons/raids (Polestar's own journal covers them). Capital cities are IN scope as smaller guides (see City guides above).
