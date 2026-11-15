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

_The twin guide. Horde quest lines are already faction-gated inside the Alliance file. Part of the Horde block — built last, after Alliance completion._

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

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

- [x] Census — 95 quests, local-data census (`docs/teldrassil-census.md`)
- [x] Core guide — `teldrassil.guide`
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

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Mulgore — Tauren (Horde) · Horde block — last

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Tirisfal Glades — Undead (Horde) · Horde block — last

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

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

### Stonetalon Mountains — contested (both factions)

_Off Ashenvale. Alliance route first; Horde content handled as the data dictates._

- [x] Census - 80 candidates, 40 Alliance IN / 40 OUT (32 Horde set-aside for the Horde block)
- [x] Core guide - `stonetalon.guide`
- [x] Lint/playtest clean - 0 errors, playtest 4 personas 0 stuck (R1+R2+R5 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 9 rares (no loot in data) + 56 container placements and Barrow Dens caches, 7 recipes (4 vendor + 3 drops), 0 lint errors/warnings

### Duskwood — third zone (Alliance)

_Follows Westfall. Raven Hill country._

- [x] Census - 102 candidates, 93 IN / 9 OUT
- [x] Core guide - `duskwood.guide`
- [x] Lint/playtest clean - 0 errors, playtest 3 personas 0 stuck (R1+R2+R5 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 6 rares (4 above-band with come-back-later notes) + 86-pt container loop and unique/marker steps, 14 recipes (9 vendor + 5 drops), 0 lint errors/warnings

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

### Stranglethorn Vale — follows Duskwood / Redridge

_Booty Bay country._

- [x] Census - 258 candidates, 123 IN / 135 OUT
- [x] Core guide - `stranglethorn.guide`
- [x] Lint/playtest clean - 0 errors, playtest 4 personas + Rogue spot 0 stuck (R1+R2+R5 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 8 rares (6 with sole-drop signatures) + 9 fixed containers, 39 recipes (36 vendor + 3 drops), 0 lint errors/warnings

### Riverglades — Forever-original zone

_Skyborne country._

- [x] Census - 178 candidates, 112 IN / 66 OUT (Horde set-aside)
- [x] Core guide - `riverglades.guide`
- [x] Lint/playtest clean - 0 errors, playtest 3 personas 0 stuck (R1+R2+R5 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 5 rares (5 with sole-drop signatures) + rock-pile container loop, 15 recipes (all vendor), 0 lint errors/warnings

### Thousand Needles — contested (Kalimdor)

- [x] Census - 67 candidates, 34 IN / 33 OUT (27 Horde set-aside)
- [x] Core guide - `thousand-needles.guide`
- [x] Lint/playtest clean - 0 errors, playtest 0 stuck (R1+R2 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Desolace — contested (Kalimdor)

- [x] Census - 89 candidates, 56 IN / 33 OUT (29 Horde set-aside)
- [x] Core guide - `desolace.guide`
- [x] Lint/playtest clean - 0 errors, playtest 0 stuck (R1+R2 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

---

## Set 4 — the next tier (after Set 3, before the Horde block)

### Hillsbrad Foothills — contested

- [x] Census - 60 candidates, 37 IN / 23 OUT (10 Horde set-aside)
- [x] Core guide - `hillsbrad.guide`
- [x] Lint/playtest clean - 0 errors, playtest 0 stuck (R1+R2+R5 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 7 rares + containers, 29 recipes (25 vendor + 4 exclusive drops), 0 lint errors/warnings

### Arathi Highlands — contested

- [x] Census - 117 candidates, 47 IN / 70 OUT (50 Horde set-aside)
- [x] Core guide - `arathi.guide`
- [x] Lint/playtest clean - 0 errors, playtest 0 stuck (R1+R2+R5 accepted only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 9 rares (no loot in data) + containers incl. Illari cache, 23 recipes (15 vendor + 8 drops), 0 lint errors/warnings

### Alterac Mountains — contested

- [x] Census - 164 candidates, 20 IN / 144 OUT (67 Horde set-aside)
- [x] Core guide - `alterac.guide`
- [x] Lint/playtest clean - 0 errors, playtest 0 stuck (R2+R5 writ residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 7 rares (no loot in data, incl. dual-zone Jimmy) + 52 container placements, 26 recipes (22 vendor + 4 drops), 0 lint errors/warnings

### Moonglade — the druid thing (special handling)

_Not a standard zone route: Moonglade is the druid class hub. This guide covers the druid class content centred there — the form quests and class chains — written for druids, not a general completionist route._

- [x] Census
- [x] Core guide - `moonglade.guide`
- [x] Lint/playtest clean - 0 errors, playtest 0 stuck (R1 expedition residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - none in data (0 rares, 1 seasonal event barrel, 8 vendor recipes logged in census; small recipes round later, not this one)

### Dustwallow Marsh — contested (Kalimdor)

- [x] Census
- [x] Core guide - `dustwallow.guide`
- [x] Lint/playtest clean - 0 errors, playtest 0 stuck (R1/R2/R5 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 10 rares + fixed containers; 9 recipes (4 vendor + 5 drops)

### Feralas — contested (Kalimdor)

- [x] Census - 107 candidates, 57 IN / 50 OUT (41 Horde set aside)
- [x] Core guide - `feralas.guide`
- [x] Lint/playtest clean - 0 errors, playtest 3 personas 0 stuck (R1+R2+R5 residue only)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions - 9 rares (7 with sole-drop signatures) + 3 fixed containers, 24 recipes (13 vendor + 11 drops), 0 lint errors/warnings

### Tanaris — contested (Kalimdor)

- [x] Census - 162 candidates, 91 IN / 71 OUT (10 Horde set aside)
- [x] Core guide - `tanaris.guide`
- [x] Lint/playtest clean - 0 errors, playtest 7 personas 0 stuck (R1+R2 residue + 1 R3 warning, all documented)
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

### Blasted Lands — contested (Eastern Kingdoms)

- [x] Census - 33 candidates, 21 IN / 12 OUT (0 Horde set aside)
- [x] Core guide - `blasted-lands.guide`
- [x] Lint/playtest clean - 0 errors, playtest 3 personas 0 stuck (R1 expedition residue, all documented)
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Searing Gorge — contested (Eastern Kingdoms)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Felwood — contested (Kalimdor)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Azshara — contested (Kalimdor)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Un'Goro Crater — contested (Kalimdor)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

---

## Set 6 — everything left (after Set 5, before the Horde block)

### Silverpine Forest — Horde second zone

_Horde heartland — a Horde-faction route, written here in leveling order, ahead of the Horde starting block._

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### The Barrens — Horde second zone

_Horde heartland — a Horde-faction route, written here in leveling order, ahead of the Horde starting block._

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Swamp of Sorrows — contested (Eastern Kingdoms)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### The Hinterlands — contested (Eastern Kingdoms)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Western Plaguelands — contested (Eastern Kingdoms)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Eastern Plaguelands — contested (Eastern Kingdoms)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Burning Steppes — contested (Eastern Kingdoms)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Deadwind Pass — contested (Eastern Kingdoms)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Winterspring — contested (Kalimdor)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Silithus — contested (Kalimdor)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Mount Hyjal — Kalimdor

_Content as the game data dictates._

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Shen'dralas — Forever-original zone

_No public rare data yet — its census leans on game data._

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

---

## Beyond v1.0 — every other open-world zone

_Every open-world zone is now assigned to a set — nothing remains here._

**Out of scope by design:** dungeons/raids (Polestar's own journal covers them). Capital cities are IN scope as smaller guides (see City guides above).
