# Zephras Isle Horde census (audit-and-close round, pack 0.95.0 → 0.96.0)

Method: local game data only (`upstream-polestar/data/forever`, built `--product wowf` + QuestieDB).
Accept key **2521** (Zephras Isle). No city key exists on the island. Band **1–12**
(guide header; all 145 contracted quests sit in it; every non-contract find below
is above band or broken). Race/class matrix: `races.json` — Skyborne plays both
sides: Alliance Skyborne WARRIOR/HUNTER/ROGUE/MAGE/DRUID, Horde Skyborne
WARRIOR/HUNTER/ROGUE/SHAMAN/DRUID. Faction-bit rule used below, grounded the same
way: bit33 (0x200000000) = Horde (quest 787 Durotar/ORG), bit32 (0x100000000) =
Alliance (quest 1076/167 Stormwind), both = shared, empty = unrestricted.

## Accepts on key 2521: 149 records = 145 contracted + 4 non-contract

Item-start scan over the 145: exactly one item-started quest, **94490 Ripped
Missive** (start item 265476, drops from Commander Haalien 253622, lvl 10, on
2521). Routed with the pack's bag-note pattern ("starts from a missive found on
the cultists"); shared content, both factions. No other contract quest has a
start item.

The 4 non-contract quests on 2521, all correctly OUT:
- 93161 Ancient Hilt (lvl 16, start object 676059) — above band.
- 96996 / 97205 (lvl/min 40, races bit32+33 shared, start=end npc 265756) —
  riding-training records, above band.
- 97029 Eluvi'ana (no level, no races, no classes, start=end npc 259012) —
  broken/incomplete record.

## Reconciliation vs the 145-contract and `zephras-isle.guide`

- (a) Contracted and correctly gated for Horde: **121** — the 28 Horde-mask
  quests (92484, 92598, 92466, 92467, 92468, 92514, 92595, 92700, 93735, 93736,
  93737, 93738, 93746, 94411, 97972, 98284, 92579, 92871, 93740, 92646, 92708,
  93090, 93836, 95349, 97243, 97244, 97245, 97257) every one carrying its
  `only Horde` (plus class where the data gates one), and the 93 shared-data
  quests routed ungated (both factions takeable per the data). Includes the
  shared 92880→92881 chain (92642/92645 → 92880 → 92881 → 92643, all
  empty-races, ungated, self-contained — no Horde wedge).
- (b) Contracted but under-gated: **5**. 97973 (Alliance Tailoring) and 98286
  (Alliance Enchanting) are Alliance-data, `optional`, with NO faction gate —
  a Horde player would be offered a dead line. Fixed this round
  (`optional only Alliance`). 92481 / 93791 / 93797 (Alliance Mage chain) carry
  `only Mage` only — but Horde Skyborne cannot be Mage (`races.json`), so no
  Horde persona can ever match those lines. Left as-is, argued here instead of
  gated (see BORDERLINE).
- (c) Missing from the contract: **none**. Every Horde-takeable accept on 2521
  is contracted.
- (d) Correctly absent: the **24 Alliance-only** contract quests (92481, 92597,
  92596, 92699, 92727, 92849, 92850, 93461, 94413, 97973, 98286, 92840, 99260,
  92701, 92834, 92860, 92709, 93089, 93835, 94369, 94946, 92741, 93791, 93797),
  each `only Alliance`-gated so Horde skips them, plus the 4 non-contract
  records above.

## The header finding (why this is Case B, not Case A)

Per-line gating is complete (after the 2 fixes), but the file header reads
`faction Alliance`. Engine semantics (`ARCHITECTURE.md`: `faction = ...
nil (either)`; `GUIDE_FORMAT.md`: "Skyborne plays on both sides: a guide's
`faction` or an `only` faction picks the side"; `Guides.GuideMatches` filters
the guide list by faction, race, class): a Horde Skyborne player on their own
faction filter is never shown this guide — all 31 `only Horde` lines and every
Horde-gated step are unreachable. Checklist note ("lines already faction-gated
inside") is true but insufficient. The route itself does NOT diverge (same hubs,
same chains; order twins co-located by design), so no separate Horde file
(Case C) — the fix is the header, in place (Case B).

Fix applied: `faction Alliance` header line removed from `zephras-isle.guide`
(nil = either faction; `moonglade-recipes.guide` ships the same shape and lints
clean). Per-line `only` gates now pick sides exactly as the format describes.
No travel lines in the file (island start); all notes are order-neutral
("your order"); `train` lines are rank-only and resolve nearest own-faction at
runtime. `race Skyborne` header retained (both factions' race).

## Companions audit

- `zephras-isle-rares.guide`: content is faction-neutral (8 rares carry no
  faction flags; tame lines are `only Hunter`; notes point at the shared core
  route). Same header block — fixed the same way (`faction Alliance` removed).
- `zephras-isle-recipes.guide`: all 6 vendors verified faction AH in the data
  (257006 Nyalah Brightfire, 251905 Zerril Softbreeze, 251991 Taleen
  Shimmerthread, 257020 Nasalanna Windsinger, 252380 Othesia Evengale, 257004
  Eaysaa Brightgust — neutral, serve both factions). Same header block — fixed
  the same way. No vendor sells faction-exclusive stock per the data.
- No separate Horde companions: content is identical for both sides.

## Machine-checkability

No new contract entry: a second entry would double-count the same file in the
totals. Horde coverage regresses on (1) the unchanged 145/145 contract check —
the Horde lines live in the same file — and (2) the honest playtest, which plays
each race that can reach the guide: after the header fix that includes Horde
Skyborne personas (verified in this round's playtest).

## BORDERLINE

- Mage lines (92481/93791/93797, `only Mage` without `only Alliance`): left
  ungated-by-faction because Horde Skyborne+Mage is not a pair that exists in
  the game (`races.json`). If Forever ever opens Mage to Horde Skyborne, these
  three need `only Alliance` added.
- 92880/92881 (empty races, ungated): kept shared — the data marks them
  unrestricted and their whole chain (92642/92645/92643) is shared. The
  Valennia-name flavor does not change the data's faction bits.
- 93161: has a real end NPC (259012) but level 16 — above band either way.
- 97029: no level/races/classes — broken record, not a hidden quest.
- No Horde Paladin/Priest/Warlock content exists in the data for this zone
  (no such class bits on any 2521 quest) — matches `races.json` (Horde Skyborne
  plays none of those), so no gap.
