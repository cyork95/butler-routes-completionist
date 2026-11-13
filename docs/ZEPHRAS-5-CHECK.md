# Zephras Isle — five-quest check vs ForeverDB & co.

Checked 2026-11-13 against PandaBase (player-recorded Forever quest data), ForeverDB (client build 1.60.1.70938, extracted 2026-11-13), 60.tools (client-derived DB), and the community hub list that surfaced the names (hardcorehelper, beta-derived). Tracker reference: `journey.json`, zone `zephras-isle` — 142 quests, lowest ID 92463.

| # | Quest | ID | Zone | Level (req) | Giver | Restrictions | Verdict |
|---|-------|----|------|-------------|-------|--------------|---------|
| 1 | Coming of Age | 92460 | Zephras Isle | 1 (req 1) | Ailee Farheart → turn in to Rorian the Dayseeker | Skyborne only — **both** orders (Alliance & Horde Skyborne); any class | **REAL-MISSING** |
| 2 | Harmony in Balance | 92461 | Zephras Isle | 1 (req 1) | Rorian the Dayseeker | Skyborne only — both orders; any class. Slay 8 Juvenile Vuldren | **REAL-MISSING** |
| 3 | Infestation Investigation | 92462 | Zephras Isle | 2 (req 1) | Elatrell Featherlight | Skyborne only — both orders; any class. Slay 8 Pesky Cirrusflies | **REAL-MISSING** |
| 4 | Hopping Helpers | 94901 | Zephras Isle (hub list only) | 11 (hub list) | none recorded anywhere | Client record exists, but description is literally "[PH] Collect frogs", no objectives, no giver; absent from ForeverDB's Zephras list and from PandaBase | **SCOPED-OUT** |
| 5 | Valanaar Vintages | 94902 | Zephras Isle (hub list only) | 11 (hub list) | none recorded anywhere | Client record exists, but description is literally "[PH] Collect grapes from the vineyard", no objectives, no giver; absent from ForeverDB's Zephras list and from PandaBase | **SCOPED-OUT** |

## Verdicts, one line each

1. **Coming of Age — REAL-MISSING.** The very first Skyborne quest (ID 92460); every Skyborne of either order takes it from Ailee Farheart at the spawn point — it belongs in the tracker and at the head of the guide.
2. **Harmony in Balance — REAL-MISSING.** Rorian's first kill quest (92461); PandaBase even chains it into the class-intro quests (92481–92485, 92532) that the tracker *does* have — the tracker holds the follow-ons but not this.
3. **Infestation Investigation — REAL-MISSING.** Elatrell Featherlight's cirrusfly quest (92462), taken alongside The Cirrusfly Queen (92463) — the tracker has the Queen but not this one.
4. **Hopping Helpers — SCOPED-OUT.** A placeholder record, not a playable quest: "[PH]" text, no objectives, no giver in any database, and ForeverDB's current client extraction for Zephras doesn't list it — there is nothing to accept and no guide step can be written for it.
5. **Valanaar Vintages — SCOPED-OUT.** Same story as its consecutive-ID sibling (94902): placeholder "[PH]" record only; correctly left out until/unless it is implemented with a real giver and objectives.

## Pattern worth knowing

- The three genuine misses are **consecutive IDs 92460–92462, immediately before the tracker's first ID 92463** (The Cirrusfly Queen). The curation didn't skip them by scope — it simply starts three quests late.
- **None of the five is order-specific or class-specific.** The Skyborne two-orders split does not explain any of them: the three real quests are open to Skyborne of both orders and every class (PandaBase: "Skyborne (Alliance), Skyborne (Horde)", "any class").
- The hub list's third "starts somewhere else" quest, Ripped Missive (94490), **is** in the tracker — so item-started quests were in scope; 94901/94902 are excluded by their placeholder nature, not by scope.
- If 92460–92462 are added, the guide's opening becomes: accept 92460 → turnin 92460 → accept 92461 (+ Elemental Unrest) → accept 92462 + 92463 from Elatrell Featherlight.

## Sources

- PandaBase — Coming of Age (#92460): https://pd.zroot.it/forever/quests/92460
- PandaBase — Harmony in Balance (#92461): https://pd.zroot.it/forever/quests/92461
- PandaBase — Infestation Investigation (#92462): https://pd.zroot.it/forever/quests/92462
- ForeverDB — Zephras Isle quest list: https://foreverdb.net/quests/zephras-isle
- ForeverDB — Zephras Isle guide (givers/order): https://foreverdb.net/guide/zephras-isle
- 60.tools — Hopping Helpers (#94901): https://www.60.tools/quests/94901-hopping-helpers
- 60.tools — Valanaar Vintages (#94902): https://www.60.tools/quests/94902-valanaar-vintages
- Hub list that surfaced the five names: https://www.hardcorehelper.com/forever/guides/zephras-isle-leveling-guide
