# Butler Routes — Zone Checklist

_Where every zone stands. Updated 2026-11-13 · Pack v0.2.0 · Repo: `cyork95/butler-routes-completionist` (`master`)_

**Pack principle (Cody, 2026-11-13): this is a COMPLETIONIST pack, not a leveling guide.** Every guide covers every quest in its zone — including the ones a leveling route would skip as XP-inefficient. The build order follows the sequence a player levels through the content, but that only decides which zone gets written next; inside a zone, efficiency shapes the route's order, never its quest selection.

**The pipeline every zone goes through:**

1. Census — the zone's quest list is pulled and verified
2. Core guide — the all-quests route is written
3. Lint/playtest clean — the compiler and simulated playtest pass
4. Cody pilot — Cody plays the guide live in game
5. Pilot fixes landed — whatever the pilot found is fixed and committed

Companions (Rares & Treasures · Recipes & Patterns) follow the core guide once the Zephras template is proven.

**Build order (Cody, 2026-11-13):** Zephras companions → **Westfall → Loch Modan → Darkshore**, with **Teldrassil alongside** → then **Alliance completion** (companions for every Alliance zone, plus all pilots and pilot fixes) → then **Set 2** (Redridge Mountains → Ashenvale → Stonetalon Mountains → Duskwood) → then **Set 3** (Wetlands → Stranglethorn Vale → Riverglades → Thousand Needles → Desolace) → **Horde last** (Durotar, Mulgore, Tirisfal, Zephras twin).

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
- [ ] Companions — after the Zephras template

### Westfall — follow-on zone (Alliance) · build order #1

- [x] Census — 43 quests, tracker-verified
- [ ] Core guide — the next core build
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Dun Morogh / Coldridge Valley — Dwarf & Gnome (Alliance)

_The lead-in for Loch Modan (build order #2)._

- [ ] Census — needs a ForeverDB pull
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

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

- [ ] Census — follows Teldrassil
- [ ] Core guide
- [ ] Lint/playtest clean
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

## Beyond v1.0 — every other open-world zone

_Not started. Same pipeline applies when we get there._

### Eastern Kingdoms

- [ ] Alterac Mountains
- [ ] Arathi Highlands
- [ ] Badlands
- [ ] Blasted Lands
- [ ] Burning Steppes
- [ ] Deadwind Pass
- [ ] Eastern Plaguelands
- [ ] Hillsbrad Foothills
- [ ] Searing Gorge
- [ ] Silverpine Forest
- [ ] Swamp of Sorrows
- [ ] The Hinterlands
- [ ] Western Plaguelands

### Kalimdor

- [ ] Azshara
- [ ] The Barrens
- [ ] Dustwallow Marsh
- [ ] Felwood
- [ ] Feralas
- [ ] Moonglade
- [ ] Mount Hyjal
- [ ] Silithus
- [ ] Tanaris
- [ ] Un'Goro Crater
- [ ] Winterspring

### Forever-new lands

- [ ] Shen'dralas

_No public rare data yet for either — their censuses will lean on game data._

**Out of scope by design:** capital cities (no zone route to write) and dungeons/raids (Polestar's own journal covers them).
