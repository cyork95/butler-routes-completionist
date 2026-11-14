# Butler Routes — Zone Checklist

_Where every zone stands. Updated 2026-11-14 · Pack v0.6.0 · Repo: `cyork95/butler-routes-completionist` (`master`)_

**The pipeline every zone goes through:**

1. Census — the zone's quest list is pulled and verified
2. Core guide — the all-quests route is written
3. Lint/playtest clean — the compiler and simulated playtest pass
4. Cody pilot — Cody plays the guide live in game
5. Pilot fixes landed — whatever the pilot found is fixed and committed

Companions (Rares & Treasures · Recipes & Patterns) follow the core guide once the Zephras template is proven.

**Build order (Cody, 2026-11-13):** Zephras companions → **Westfall → Loch Modan → Darkshore**, with **Teldrassil alongside**. Horde starts follow.

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

_The twin guide. Horde quest lines are already faction-gated inside the Alliance file._

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
- [x] Core guide — `westfall.guide`
- [x] Lint/playtest clean — 0 errors, playtest 0 stuck
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Dun Morogh / Coldridge Valley — Dwarf & Gnome (Alliance)

_The lead-in for Loch Modan (build order #2)._

- [x] Census — 105 quests, local-data census (`docs/dun-morogh-census.md`)
- [x] Core guide — `dun-morogh.guide`
- [x] Lint/playtest clean — 0 errors, playtest 0 stuck
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Loch Modan — second zone (Alliance) · build order #2

- [x] Census — 41 quests, local-data census (`docs/loch-modan-census.md`)
- [x] Core guide — `loch-modan.guide`
- [x] Lint/playtest clean — 0 errors, playtest 0 stuck
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

### Durotar — Orc & Troll (Horde)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Mulgore — Tauren (Horde)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

### Tirisfal Glades — Undead (Horde)

- [ ] Census
- [ ] Core guide
- [ ] Lint/playtest clean
- [ ] Cody pilot
- [ ] Pilot fixes landed
- [ ] Companions

**v1.0 publishes when every box above is ticked** — then the `v1.0.0` tag push fires the GitHub Actions publish to polestar.guide.

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
- [ ] Duskwood
- [ ] Eastern Plaguelands
- [ ] Hillsbrad Foothills
- [ ] Redridge Mountains
- [ ] Searing Gorge
- [ ] Silverpine Forest
- [ ] Stranglethorn Vale
- [ ] Swamp of Sorrows
- [ ] The Hinterlands
- [ ] Western Plaguelands
- [ ] Wetlands

### Kalimdor

- [ ] Ashenvale
- [ ] Azshara
- [ ] The Barrens
- [ ] Desolace
- [ ] Dustwallow Marsh
- [ ] Felwood
- [ ] Feralas
- [ ] Moonglade
- [ ] Mount Hyjal
- [ ] Silithus
- [ ] Stonetalon Mountains
- [ ] Tanaris
- [ ] Thousand Needles
- [ ] Un'Goro Crater
- [ ] Winterspring

### Forever-new lands

- [ ] Riverglades
- [ ] Shen'dralas

_No public rare data yet for either — their censuses will lean on game data._

**Out of scope by design:** capital cities (no zone route to write) and dungeons/raids (Polestar's own journal covers them).
