# Deadwind Pass census (pack butler-routes-completionist)

Census from local Forever game data (questie-forever quests/npcs/objects/items.json),
built with `--product wowf` + QuestieDB. Accept-zone key **1430** (verified:
the map key carrying Hastings, Calliard, the Dark Riders, Harrison Jones, the
Karazhan door/pew objects and the Deadwind mob set; only 1 quest record keys
1430 in its zone field — the writ below).

Method (settled): a quest belongs to the zone if its accept/start is on 1430.
Chains ending outside are IN; objectives in-zone with accept elsewhere are OUT.
Item-started quests (including rare-drop starts) are IN. The giver-spawn test
was run on every giver: 34 NPCs spawn on 1430 (Spirit Healer, Deadwind
Brute/Mauler/Warlock/Ogre Mage, Restless Shade, Sky Shadow, the Karazhan-crypts
cast — Wailing Spectre, Damned Soul, Unliving Caretaker/Resident, Ley/Mana
Sprites, Maethra Slagheart's ward party, Altruist Wards, Fleuric, Harrison
Jones, Injured/Deceased Adventurers, Mana Elementals, Haunted Anvil, Hastings,
Calliard, Spectral Charger, Mistmantle Prowler, plus Agent Keanna, Dark Rider
and Cat) and 39 objects (Karazhan pews/doors/gates/portcullises, campfires,
bonfires, cauldrons, Charred Bone Fragment, Advanced Swordplay, Recipe: Raw
Plated Armorfish) — **none of them starts any quest in the data** (0 quests
with start.npc/start.object on 1430, verified by full scan and by spot-checks
on Harrison Jones, the Dark Rider, Hastings and Calliard).

Race masks: null neutral IN (EPL precedent). No class, skill, event, pre, excl
or next fields anywhere on the single candidate — no gating applies.

## Band: 60-60

The contract is a single quest at level 60 (see BORDERLINE for why the band
is the quest's level and not its minLevel). Highest and lowest contracted
quest level alike: 60. Written 60-60 because the lint format requires a
min-max range.

## IN - 1 quest

| ID | title | lv/min | giver (accept) | turn-in | notes |
|----|-------|--------|----------------|---------|-------|
| 94355 | Craftsman's Writ: Tuxedo Jacket | 60/1 | item 264155 (sourceless — no drops, no vendors in the data) | Hastings @46.99,75.32 | profession writ; optional, bag-note accept per Arathi writ precedent; races null (Alliance OK) |

## OUT

Nothing. Every OUT class is empty by full scan, not by sampling:
- [PH] placeholders accepting here: 0.
- Horde-only quests accepting here: 0 (the one candidate is races-null).
  Horde set-aside count: **0**.
- Repeatables: 0 (no repeat flag exists on any candidate; the writ class is
  contracted per the Arathi precedent — see BORDERLINE).
- Seasonal/event quests: 0 (event field null on the candidate).
- Broken/incomplete records: 0.
- Accepts outside the zone: not applicable — nothing else accepts here.
- Above-band: 0.
- Objectives in-zone with accept elsewhere: 0 — verified by full scan: no
  quest in the database carries a kill, object, event or talk objective
  targeting any of the 34 NPCs or 39 objects spawning on 1430. (Deadwind is a
  pass-through: the Dark Riders, Harrison Jones and the crypts cast take no
  part in any quest objective in the data.)

## BORDERLINE

1. **Band 60 vs 1-60.** Quest 94355 reads minLevel 1, level 60. The minLevel-1
   is a null-default (no minimum set), not a real floor: the quest's content
   is a level-60 crafted jacket. A "1-60" header band on a one-quest guide
   would mislead players about when to play it. Contracted levelBand: **60**,
   the quest's level, reported with both numbers here. Nothing is OUT on band
   either way.
2. **Sourceless item-start.** Item 264155 has no drops and no vendors anywhere
   in the data, so the accept cannot be sequenced behind a sourcing kill.
   Contracted with an honest bag note ("have the writ in your bags") per the
   Stormwind/Westfall sourceless handling and the Arathi writ precedent
   (94230/94239/94248 ship exactly this way). Expected R2 warning, structural.
3. **Writ repeatability.** Craftsman's Writs smell repeatable, but the data
   carries no repeat flag and the Arathi round already contracts the same
   writ class (94230 et al.). IN per the profession-quest rule; if later data
   shows a repeat cycle, the census gets revisited.
4. **No profession gate.** The writ and jacket items carry no profession
   field and the quest's skill field is null, so no `when skill` gate can be
   honestly pinned (guessing Tailoring from the item name would be brief-side
   invention). Ships `optional` with no skill gate, mirroring the Arathi
   writs, which carry no gates either.
5. **Objects 457088/694054 (Advanced Swordplay, Recipe: Raw Plated Armorfish).**
   Fixed spawns in-zone that look quest-adjacent, but no quest in the data
   starts from or objectives them. Noted here for the companion rounds, not
   contracted.
