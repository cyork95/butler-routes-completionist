# Authoring notes — Butler Routes, Elwynn Forest completionist

**Pack:** `butler-routes-completionist` · **Guide:** `butler-routes-completionist/elwynn-forest`
**Files:** `elwynn-forest.guide` (39 steps, 25,627 bytes). `pack.json` and the Zephras pilot files
were not touched — the pack-id change (`butler-routes` → `butler-routes-completionist`, to match
the polestar.guide Studio draft) is applied here in the guide header and these notes only; Butler
is updating `pack.json` and the Zephras guide centrally.

Written for the whole roster that passes through Elwynn: Skyrinis (Skyborne Druid on his
completionist Journey), Orinis (Skyborne Hunter) and human alts starting in Northshire. No
profession-training tasks and no pet notes (those were Zephras/Orinis specifics); class quests for
other classes are present, gated with `only`, so they never show for a character they are not for.
There is deliberately no `race` header — this route serves Humans and Skyborne alike.

## Verification (script-checked against the generated file, not the draft data)

| Check | Result |
| --- | --- |
| Quests in the contract list (`journey.json`, zone `elwynn-forest`) | 83, all unique IDs |
| `accept` lines | **83 — every contract ID exactly once, no extras, no duplicates** |
| `turnin` lines | **83 — every contract ID exactly once, no extras, no duplicates** |
| Accept/turnin IDs outside the 83 | **none** |
| Steps | 39, every step contains at least one goal |
| Turn-in before accept (file order) | none |
| Header | `guide` (with the corrected pack prefix), `title`, `levels 1-10`, `zone`, `faction` all present, plus `category`, `folder`, `keywords`, `coords live`, `version` — matching the pilot's conventions |
| Keywords used | only ones from the official cheatsheet: goals `accept`, `turnin`, `task`, `level`; directives `only`, `tip`, `note`; modifiers `only <Class>`, `optional`, `direct`. No invented syntax. |
| Chain-order spot checks (Milly, Billy, lovers, lake, Azora, Thomas, taming, Collector chains) | all pass |

The first verification run caught two missing quests — the mount exchanges (7677, 7678) were
described in the header comment but had no step. They now sit in their own Eastvale step, and the
re-run passes clean.

**Not run:** `forge guide lint` / `polestar playtest` — they need the Polestar toolchain and its
reference data, which are not installed here. Running lint is human step #1 (see Playtest list).
This is stated plainly: the guide is script-verified against the contract and the cheatsheet, and
nothing more.

## Ordering basis

- **Hub flow, levels, givers, hand-ins:** ForeverDB's Elwynn Forest quest guide (83 quests with
  pickup/objective/hand-in steps; its data is Classic CMaNGOS until a player sees the quest in
  Forever) and ForeverDB's Northshire Valley walkthrough (giver-by-giver order for levels 1–10,
  with coordinates recorded in Forever: Willem 48.2, 43.0 · McBride 48.9, 41.6 · Eagan 48.9, 40.2 ·
  Milly 50.7, 39.3 · Falkhaan 45.6, 47.8 · Dughan 42.1, 65.9 · Remy 42.2, 67.2 · William 43.3, 65.8 ·
  Sam 44.9, 63.3 · Josephine Carson 41.2, 66.2 · Josetta 43.3, 65.7).
- **Chains:** HardcoreHelper's Elwynn guide — its three long chains are followed exactly:
  the Northshire web (A Threat Within → Kobold Camp Cleanup / Eagan Peltskinner / Brotherhood of
  Thieves → Wolves Across the Border / Investigate Echo Ridge / Bounty on Garrick Padfoot →
  Milly Osworth / Skirmish at Echo Ridge → Milly's Harvest / Report to Goldshire → Grape Manifest);
  the marshal's east chain (A Fishy Peril → Further Concerns → Find the Lost Guards → Discover
  Rolf's Fate → Report to Thomas → Deliver Thomas' Report → Cloth and Leather Armor); and the
  Crystal Lake chain in ascending ID order (A Net Disaster → Slimy Menace → A Man About a Murloc →
  An Enticing Offer → Baited for Success, which also matches ForeverDB's objectives).
- **Class quests:** wowhandbook's class-quest tables (Hunter: Josephine Carson, Goldshire —
  Rockhide Boar → Gray Forest Wolf → Young Forest Bear, then Training the Beast to Isaac Chan,
  Goldshire; Priest: Divine Grace from Priestess Josetta, Goldshire, to High Priestess Laurena in
  Stormwind) and a Forever hunter-pet guide for the target order.
- **Applejack pair:** Polestar's own 0.3.2 changelog (the still comes after Homer Stonefield sells
  the apples; the quest never shows in the log; keep the Thunder Applejack for Sergeant De Vries),
  wowforever.ninja's Applejack Still page (collect 4 Shiny Red Apples; giver unknown there), the
  Forever atlas (An Apple Treat starts with Sergeant De Vries at Westbrook), and a map listing
  that puts the still at 24.5, 58.2.

**Coverage reconciliation:** the tracker list (83) and ForeverDB's zone list (83) share 71 quests
by name. ForeverDB's page carries 12 the tracker omits — the Paxton book chain (Book Inventory,
Nibbled-On Book, Rascally Rodents, Mining Consultant, The Big Picture, Follow That Kobold!,
Shhh! We're Hunting Kobolds, Book Return, Rare Books), A Scribbled Letter, Croaky's Head and
Elmpaw's Head — and the tracker carries 12 ForeverDB's zone page omits: the two mount exchanges,
Camping 101: Alchemy / Enchanting / Herbalism, the Applejack pair, Divine Grace and the four
hunter taming quests. The guide flags the unlisted abbey/Goldshire book quests in `note` lines
(steps 1 and 8) and Elmpaw's Head in the bears note, so a completionist still does them.

## Design choices

- **ID-only `accept`/`turnin` lines**, as in the pilot: the compiler fills titles, givers and
  coordinates from its reference data. Player-facing `--` notes carry the giver names and the
  ForeverDB coordinates I verified. No `kill`/`collect`/`complete` goals anywhere — progress is
  tracked by accept/turn-in only, and objective-heavy areas (both mines, the Fargodeep run) are
  steps whose goals are the hand-ins the run produces, with the work described in the `tip`.
- **`coords live` header**, matching the pilot: every typed coordinate came from ForeverDB's
  in-game recordings (or, for the still, a map listing of the live game).
- **Class quests gated per line** (`accept 94774 only Priest`) where a single quest sits inside a
  general step, and **whole-step** (`only Hunter` + `level 10`) for the taming chain — both
  patterns copied from the pilot.
- **Camping 101 quests are `optional`** (all twelve), following the pilot: each is offered once
  the matching profession shows proficiency. Their accepts are batched at Sam's camp; hand-ins
  are placed where ForeverDB puts the trainers (Goldshire batch step; Fishing → Lee Brown at the
  lake; Tailoring → Eldrin at Eastvale; Engineering and Mining → Stormwind).
- **Profession-flavoured quests are `optional`**: Rough Wolf Pelts (pelts come from skinning
  wolves) and An Enchanting Lesson (it works by disenchanting effigies). If either is offered to
  everyone, the `optional` flag is harmless; if it is profession-gated, non-specialists are never
  blocked. Same treatment for Welcome! (only a fresh human holds the voucher) and the two level-60
  mount exchanges.
- **Applejack Still is a `direct` turn-in** (the cheatsheet's Distracting-Jarven pattern): the
  quest never enters the log, so the step carries an `optional` accept for contract completeness
  and a `turnin … direct` at the still itself. The apples are primed two dozen steps earlier by an
  `optional` task at the Stonefield Farm (Homer Stonefield sells them) — the sequencing Polestar's
  own guide settled on after its first version sent players to the still empty-handed.
- **Named rares:** one short `note` in the Eastvale hand-ins step covers the zone's bear rares
  (Matriarch Bristlefur; Elmpaw, level 12 elite, south of Eastvale) and a `note` under the
  Westbrook step covers Hogger's level and his hand-in.

## UNVERIFIED — read before playtesting

1. **Delicate Instruments ID mapping.** 91723 and 91724 share a name. I assigned 91723 to the
   Jasperlode Geomancers version and 91724 to the Stone Cairn Lake Rogue Wizards version, by
   ascending ID and by ForeverDB's listing order. The sources also disagree on details:
   ForeverDB says level 8 / 8 geomancers and level 10 / 8 wizards; HardcoreHelper says both are
   level 10, with 8 geomancers and 6 wizards. The mapping is the single most likely thing in this
   guide to be wrong; check Hamish Bergwort's two offers against the IDs on first playtest.
2. **Taming-chain ID-to-tame mapping.** The chain itself is verified (Josephine Carson, Goldshire,
   41.2, 66.2; three tames in the order Rockhide Boar → Gray Forest Wolf → Young Forest Bear;
   Training the Beast to Isaac Chan, Goldshire). ForeverDB's walkthrough lists the four quests in
   the order 94792, 94863, 94864, 94793, and the guide follows that order — but no fetched source
   ties each ID to a specific tame individually.
3. **Divine Grace's ID.** The tracker says 94774; one quest-guide site's completion check uses
   94773, and several same-name "Divine Grace" records exist (the spell is new in Forever for
   Human priests). Class, level (10), giver (Priestess Josetta) and hand-in (High Priestess
   Laurena, Stormwind Cathedral) are verified; the exact ID in the tracker may be a sibling
   record.
4. **The Applejack dependency.** That the still is a direct hand-in wanting 4 Shiny Red Apples,
   that Homer Stonefield sells the apples, and that the Thunder Applejack goes to Sergeant De
   Vries at Westbrook are each attested (Polestar changelog; wowforever.ninja; Forever atlas).
   What is not attested: whether An Apple Treat (91738) must be accepted before the still will
   produce the applejack, and the still's exact spot (24.5, 58.2 comes from one map listing).
   The guide sequences still → De Vries accept → De Vries hand-in inside one step; if the game
   wants the quest first, the fix is a five-minute reorder of that step.
5. **Camping 101 loose ends.** Pickups from Sam Sarsaparilla are verified for nine of the twelve
   on ForeverDB's zone page, and for Enchanting (97917) and Herbalism (97921) in its walkthrough;
   Alchemy's (97915) pickup is assumed to be Sam like the rest. Hand-ins: Herbalism goes to
   Herbalist Pomeroy (ForeverDB walkthrough) — his location is not verified, and the turn-in sits
   in the Stormwind step on the Classic-data assumption that he is the city's herbalist; the
   Alchemy and Enchanting hand-in NPCs are not named in any fetched source, so their `--` notes
   deliberately say "the trainer the quest names" and rely on the compiler's data.
6. **Cloth and Leather Armor (59) gating.** Placed after Deliver Thomas' Report, following
   HardcoreHelper's chain list. If it is in fact ungated, nothing breaks — the accept simply
   happens later than it could. Its hand-in (Sara Timberlain) is why the route makes a final
   Eastvale pass after the last Goldshire reports.
7. **Shipment to Stormwind (61) prerequisite.** Classic wants Kobold Candles handed in first;
   ForeverDB's walkthrough takes both quests together, suggesting Forever dropped the link. The
   guide accepts 61 in the Goldshire pass after 60's hand-in, which works under either rule.
8. **The Collector (123) → Manhunt (147).** The guide assumes the item-started schedule quest
   precedes Manhunt and accepts 147 in the same Goldshire pass that hands the schedule in. If
   the Schedule's drop (Riverpaw gnolls around Stone Cairn Lake) is slow, that lake step — whose
   only accept is the item quest — is where the route will wait. ForeverDB's own route takes
   Manhunt without the schedule quest, so the link may not exist; the order is harmless either
   way.
9. **Give Gerard a Drink (16).** Giver and hand-in are Gerard Tiller per ForeverDB (Classic
   CMaNGOS data); no fetched source pins his exact spot, so the guide keeps him "in the valley"
   and groups the quest with the vineyard step. Accept and hand-in are the same NPC, so the
   placement risk is a short walk, nothing more.
10. **Welcome! (5805).** Hand-in to Merissa Stilwell per ForeverDB; her abbey spot is not
    independently verified. Both lines are `optional`, so a missing voucher or a moved NPC never
    blocks the route.
11. **Mount exchanges (7677, 7678).** Katie Hunter at the Eastvale stables is Classic geography
    (the camp's stables and horse breeder); ForeverDB's zone page does not list these level-60
    quests at all. They are in the guide for contract completeness, marked `optional`.
12. **Helene Peltskinner's exact spot.** Grouped with Sam's camp (she is listed among the
    Goldshire-area givers, and she is also the Skinning Camping hand-in). If she stands elsewhere
    around Goldshire, two `--` notes are cosmetically wrong and nothing else.
13. **Levels are beta-era in the sources.** HardcoreHelper states its quests are "as they were in
    the beta". The header keeps the specified `levels 1-10` even though Wanted: "Hogger" is
    level 11 and the horse exchanges are level 60 — both are the zone's completion set and belong
    in the guide, flagged where they sit.

## Playtest first, in this order

1. Run `polestar dev` / `forge guide lint` on the pack and fix whatever it flags (expected
   friction: the `direct` Applejack turn-in paired with an `optional` accept, and the item-started
   `accept 123`).
2. Fresh **human**, follow the guide from level 1: check the ID-only flow through Northshire
   (the McBride/Willem/Eagan batching) and the farms web — the lovers and Billy chains interleave
   four NPCs across two farms, and any mis-ordered accept shows up there first.
3. Level 10, **hunter**: the taming chain end-to-end — confirm the ID order (94792 → 94863 →
   94864 → 94793) against Josephine Carson's actual offers.
4. Level 10, **priest**: confirm Divine Grace's ID at Priestess Josetta (94774 vs 94773).
5. The Tower of Azora: confirm which Delicate Instruments ID is the Jasperlode list.
6. The Applejack Still: buy the apples at Stonefield, work the still before speaking to De Vries,
   and confirm the direct hand-in ticks the goal and the applejack satisfies An Apple Treat.
7. Camping 101: confirm the proficiency gating — that untrained professions' quests are simply
   not offered, so the `optional` lines never block — and pin down the Alchemy/Enchanting
   hand-ins and Herbalist Pomeroy's location.
