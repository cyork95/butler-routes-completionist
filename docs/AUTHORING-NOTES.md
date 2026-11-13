# Authoring notes — Butler Routes, Zephras Isle completionist pilot

**Pack:** `butler-routes` · **Guide:** `butler-routes/zephras-isle` · **Version:** 0.1.0 (pilot)
**Files:** `zephras-isle.guide` (38 steps, 23,712 bytes), `pack.json`, `LICENSE` (CC-BY-4.0 — Polestar's own scaffold default; chosen so other authors can reuse the route with attribution).

Written for Orinis (Skyborne Hunter, gatherer: Mining + Herbalism), but the route is a full-zone
completionist route: every class's and both orders' quests from the tracker list are present,
gated with `only` so they only ever show for a character they belong to.

## Verification (script-checked against the generated file, not the draft data)

| Check | Result |
| --- | --- |
| Quests in the contract list (`journey.json`, zone `zephras-isle`) | 142, all unique IDs |
| `accept` lines | **142 — every contract ID exactly once, no extras, no duplicates** |
| `turnin` lines | **142 — every contract ID exactly once, no extras, no duplicates** |
| Accept/turnin IDs outside the 142 | **none** (see the taming-chain note below) |
| Steps | 38, every step contains at least one goal |
| Turn-in before accept (file order) | none |
| Chain-order spot checks (Scholar, Taming, Elder, Thendal, Falaath, Orchard chains) | all pass |
| Header | `guide`, `title`, `levels`, `zone`, `faction`, `race` all present, plus `category`, `folder`, `keywords`, `coords live`, `version` |
| Keywords used | only ones from the official cheatsheet: goals `accept`, `turnin`, `complete`, `train`, `task`, `level`; directives `only`, `tip`, `note`; modifiers `only <Class[,Faction]>`, `optional`. No invented syntax. |

**Not run:** `forge guide lint` / `polestar playtest` — they need the Polestar toolchain and its
reference data, which are not installed here. Running lint is human step #1 (see Playtest list).

## The taming chain — a correction to the brief

The brief expected the hunter taming chain to sit *outside* the 142. It doesn't: all five quests
are in the tracker list, and ForeverDB's quest pages verify the full chain, in order:

`94007` Taming the Beast (accept Elayaa Easewind, Shen'dar hunter trainer 45.2, 44.3 → hand in to
Quel'ana Quickgale, Valanaar 59.6, 72.6) → `94978` part 1 of 3 (tame a Windsong Crawler; objective
area 51.7, 72.5) → `94979` part 2 of 3 (tame an Ornery Galestrider, Gustberry Lowlands 57.0, 72.1) →
`94013` part 3 of 3 (tame a Vuldren Alpha, Gustberry Lowlands 54.1, 75.1) → `94050` Training the
Beast (Quel'ana Quickgale). The guide uses `complete <id> @x,y live` for the three tames — the only
`complete` lines in the guide, because these are the only objectives with player-recorded
coordinates I could verify. The level-2 hunter quest `92482` The Way of the Hunter (from Rorian the
Dayseeker, like every class's first lesson) is in the class-introduction step.

## Ordering basis

- **Hub flow and giver order:** ForeverDB's Zephras Isle guide (Thendal's 12-step giver sequence,
  Shen'dar, Falaath, Valanaar to level 10; NPC coordinates throughout are ForeverDB's
  "seen in Forever" positions).
- **Levels, faction tags, chain lists:** HardcoreHelper's Zephras Isle guide (110 unique quests by
  hub). Its three named chains are followed exactly: Elemental Unrest → Agitators → Return to
  Rorian / Aetheen of the Gales → Foul Matriarch → The Next Step; The Missing Scholar ×3 →
  Fillion's Mission → Catching Wind → Avenged Tenfold → In Service of Zephras; The High Elder's
  Request → The Turncoat + Al'Aketh Assassins → Unfortunate News → The Cult's True Plans →
  Desperate Times → Prepare for Battle → Making Our Move.
- **Real completion order:** Skyrinis's Dossier biography (78 quest turn-ins, 2026-11-05 – 11-08).
  It fixed several placements: Camping 101 turn-ins spread across the Shen'dar stay (Cooking at
  arrival; First Aid / Fishing / Herbalism after Falaath), The Adventurer and The Great Outdoors
  at Shen'dar arrival, Al'Aketh Assassins completed in the Falaath phase, Unfortunate News turned
  in immediately after The Turncoat.
- **Quest-page verification (ForeverDB):** the five taming quests and the three Missing Scholar
  quests (92727 → 92849 → 92850, givers and objective areas), which also fixes Fillion's Mission
  (99260) after part 3.

**Coverage reconciliation:** the tracker list (142) = HardcoreHelper's 110 − 5 + 37. The 37 are:
23 class quests, the 14 Camping 101 profession quests, The Adventurer, The Great Outdoors, and
More Al'Aketh Ears. The 5 HardcoreHelper quests **not** in the tracker list — Coming of Age,
Harmony in Balance, Infestation Investigation, Hopping Helpers, Valanaar Vintages — are therefore
**not in this guide** (the first three are flagged in a step-1 `note` so a fresh character still
does them). If the tracker list is ever extended, extend the guide to match.

## Design choices

- **ID-only `accept`/`turnin` lines** everywhere else: the compiler fills titles, givers and
  coordinates from its reference data, per the format docs. Player-facing `--` notes carry the
  giver names and coordinates I verified.
- **`coords live` header:** every typed coordinate came from ForeverDB's in-game recordings
  (the client's own map frame); Zephras Isle is a new zone with no Era frame to fall back on.
- **Other classes'/orders' quests are included, gated** (e.g. `accept 92466` inside an
  `only Shaman,Horde` step; per-line `only Mage` etc.). This satisfies the 142-quest contract
  inside an Alliance-headed guide while staying invisible to characters they aren't for.
- **Camping 101 quests are `optional`** (except Herbalism 97968 and Mining 97970 — this route's
  own professions): Skyrinis's biography shows turn-ins for exactly the five professions he had
  trained (Cooking, First Aid, Fishing, Herbalism, Mining), which strongly suggests each is
  offered only once that profession is learned. Tailoring and Enchanting each have two IDs —
  treated as base + specialisation versions.
- **Mining/Herbalism use `train` goals, not `task`:** Shen'dar Village is the first hub *with*
  profession trainers (ForeverDB's Thendal tables list none), so the training step sits at
  Shen'dar arrival, marked `optional` so non-gatherers can skip it. Trainers named in the tip:
  Messana Crestwind (Mining, 44.8, 44.5), Halassa Fernbreeze (Herbalism, 43.0, 43.5).
- **Fernfeather** is an `optional` task in the Windfield Orchard step (spawns 52.6, 81.2 and
  48.0, 85.4, per the brief); **Slydris** is a `note` in step 1 (no recorded spawn points).

## UNVERIFIED — read before playtesting

1. **The seven same-name order pairs are not mapped ID-by-ID to a faction.** Welcome to
   Shen'dar Village (92514 / 93461), To Valanaar (92579 / 92701), In Service of Zephras
   (92860 / 92871), A Grand Adventure (92708 / 92709), What Comes Next (93089 / 93090),
   The Fate of Zephras (93836 / 94369), Confront Lorthuna (92646 / 93835). Both IDs of each pair
   are co-located in one step with a "-- take the one offered" note. Sources agree each pair is
   one Alliance + one Horde version, but no fetched source ties a specific ID to a side.
   **Playtest:** confirm the engine leaves the un-offered version's `accept` harmless; then map
   the IDs (ForeverDB quest pages show level/giver/objective text, which differ for most pairs)
   and split them with per-line `only Alliance` / `only Horde`.
2. **`only Horde` steps inside a `faction Alliance` guide** (Broken Construct chain, Call of
   Earth, Blood for Blood, Call of Fire, plus Horde lines elsewhere). Required by the 142-quest
   contract; lint may warn or refuse them. If lint objects, the fallback is a Horde-headed twin
   guide for the Horde-only quests.
3. **Call of Fire (97243, 97244, 97245, 97257)** — order assumed to be ascending ID; levels,
   giver and chain links unverified (no fetched source covers this chain). Placed late, after
   the Shrine, on the strength of its 97xxx ID block. Call of Earth's order (92466 → 92467 →
   92468) follows HardcoreHelper's objective sequence (Signet of Akir → Earth Sapta → Rough
   Quartz) and matches ascending IDs, but the ID-to-part mapping itself is unverified.
4. **Unfortunate News (92644) accept placement** follows the chain evidence (HardcoreHelper's
   chain list + Skyrinis's turn-in timing) and sits in the High Elder's chain step;
   HardcoreHelper also lists the quest at the Falaath hub, so its exact prerequisite is
   unverified.
5. **Turn-in NPCs not individually verified** (the compiler fills them from data; a wrong guess
   in my `--` notes would be cosmetic, but the goal itself relies on the data): Al'Aketh Thugs
   (92544, note assumes Hanaa Nightwind), Al'Aketh Assassins (98512, turn-in placed in the
   Valanaar chain step), The Adventurer (96638) and The Great Outdoors (96101) givers,
   More Al'Aketh Ears (93459 — placement in the Shadowgale batch is by name only),
   Ripped Missive (94490 — treated as an item-start per HardcoreHelper's "starts somewhere
   else" note), Camping 101 givers/hand-in point (assumed the Shen'dar camp).
6. **Broken Construct chain order** (93735 → 93737 → 93738) follows HardcoreHelper's objective
   order and ascending IDs; the ID-to-part mapping is unverified. Unwelcome Spirits (93736) is
   grouped with that chain although its objective is in Shadowgale Forest.
7. **Level data is beta-era.** HardcoreHelper states its quests are "as they were in the beta".
   The header keeps the specified `levels 1-12` even though the exit/finale quests (What Comes
   Next, The Magical City of Dalaran, The Earthen Ring, Unwelcome Visitors, the Strange Hermit
   set, Mercy Falls on Deaf Ears) are level 13 in that data — they are the zone's completion set
   and belong in the guide.
8. **The Skybreaker Bulwark (94003)** is verified as the Warrior level-10 Defensive Stance quest
   (Seena Skybreaker, Valanaar 59.9, 72.9; objective: Zaal Stormshield at the Shrine of Akir).
   Its `turnin` sits in the post-Shrine Valanaar step; the accept is in the level-10 class step.

## Playtest first, in this order

1. Run `polestar dev` / `forge guide lint` on the pack and fix whatever it flags (expected
   friction: the Horde-gated steps under an Alliance header, and the co-located order pairs).
2. Fresh Skyborne **hunter**, follow the guide from level 1: check the ID-only flow feels right
   (progress is tracked by accept/turn-in only — no kill/collect goals — by design).
3. The order-pair behaviour at Shen'dar arrival (Welcome ×2) — the first pair a player meets.
4. Level 10: the taming chain end-to-end, including the three `complete` coordinates, and the
   Fernfeather task in the Orchard step just before it.
5. Camping 101: confirm the profession-gating theory — that untrained professions' quests are
   simply not offered, so the `optional` lines never block.

## v0.1.1 amendment (2026-11-13, Butler)

The five-quest check (ZEPHRAS-5-CHECK.md) found three of the five were REAL misses: the zone's first three quests — 92460 Coming of Age, 92461 Harmony in Balance, 92462 Infestation Investigation — consecutive IDs immediately before the tracker's previous first quest (92463). They are now tracked steps in the guide (opening flow: 92460 accept/turnin at spawn, 92461 turned in before the class-introduction step it unlocks, 92462 alongside 92463 at Elatrell Featherlight) and restored to the tracker list (142 -> 145). The other two (94901 Hopping Helpers, 94902 Valanaar Vintages) are unimplemented [PH] placeholder records — correctly excluded. Guide re-verified after the patch: 145 accept / 145 turnin, sets exact, no order violations. Guide version 2, pack version 0.1.1.

## v0.1.2 amendment (2026-11-13, Butler)

Pack id renamed `butler-routes` -> `butler-routes-completionist` to match the polestar.guide Studio draft id exactly (the site refuses mismatched pack/route ids). Guide id is now `butler-routes-completionist/zephras-isle`, guide version 3, pack version 0.1.2. The site upload check also confirmed: pack.json valid, route read correctly; its warning that the pack.json `folder` field is ignored for site installs (always PolestarPack_<id>) is expected — the field stays for local builds. All future guides in this pack use the `butler-routes-completionist/` prefix.
