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

- [ ] Census — needs a ForeverDB pull
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [x] Companions — 11 rares + fixed containers, 3 recipes, lint 0/0 (pilot pending)

### Loch Modan — second zone (Alliance) · build order #2

- [ ] Census — needs a ForeverDB pull
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Teldrassil — Night Elf (Alliance) · alongside

- [ ] Census — Ferinis is playing the zone now; curation follows
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Darkshore — second zone (Alliance) · build order #3

- [x] Census — 74 quests, local-data census (`docs/darkshore-census.md`)
- [x] Core guide — `darkshore.guide`
- [x] Lint/playtest clean — 0 errors, playtest 0 stuck
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

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

---

## City guides — smaller guides (after the Alliance companion rounds)

_Cities are in scope as SMALLER guides (Cody, 2026-11-14): a census + core route for the quests that accept inside the city — the content the city rule has been setting aside since the Teldrassil round. Companions only where a city's data actually warrants one. The Horde cities (Orgrimmar → Thunder Bluff → Undercity) are part of the Horde block, last._

### Stormwind — Alliance capital

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions (only where the data warrants)

### Ironforge — Alliance capital

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions (only where the data warrants)

### Darnassus — Alliance capital

_The 19 city-accept quests the Teldrassil census set aside land here._

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions (only where the data warrants)

---

## Set 2 — the third zones (after the Alliance companion rounds, before the Horde block)

### Redridge Mountains — third zone (Alliance)

_Follows Westfall and Loch Modan._

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Ashenvale — third zone (Alliance)

_Follows Darkshore._

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Stonetalon Mountains — contested (both factions)

_Off Ashenvale. Alliance route first; Horde content handled as the data dictates._

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Duskwood — third zone (Alliance)

_Follows Westfall. Raven Hill country._

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

---

## Set 3 — the next tier (after Set 2, before the Horde block)

### Wetlands — follows Loch Modan (Alliance)

_Menethil Harbor. Sorinis is questing here now._

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Stranglethorn Vale — follows Duskwood / Redridge

_Booty Bay country._

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Riverglades — Forever-original zone

_Skyborne country._

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Thousand Needles — contested (Kalimdor)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Desolace — contested (Kalimdor)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

---

## Set 4 — the next tier (after Set 3, before the Horde block)

### Hillsbrad Foothills — contested

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Arathi Highlands — contested

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Alterac Mountains — contested

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Moonglade — the druid thing (special handling)

_Not a standard zone route: Moonglade is the druid class hub. This guide covers the druid class content centred there — the form quests and class chains — written for druids, not a general completionist route._

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Dustwallow Marsh — contested (Kalimdor)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Feralas — contested (Kalimdor)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Tanaris — contested (Kalimdor)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

---

## Set 5 — the next tier (after Set 4, before the Horde block)

### Badlands — contested (Eastern Kingdoms)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Blasted Lands — contested (Eastern Kingdoms)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
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
