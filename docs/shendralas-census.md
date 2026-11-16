# Shen'dralas Census

Accept-zone key: **2652** (local QuestieDB data, `--product wowf`). Proof:
every Shen'dralas-named NPC/object spawn lives on 2652 (Shen'dralas Protector,
Shen'dralar Pylons, all quest givers below), and all 32 zone-2652 quest records
accept from NPCs/objects spawning on 2652. No side-bucket: unlike Silithus's
1414 split, nothing Shen'dralas keys elsewhere. Shen'dralas is the contained
zone inside Maraudon (the Desolace census already treats 2652 as
inside-Maraudon: "delivery-into-dungeon").

Race-mask key used below: `4294967373` = Alliance
(Human/Dwarf/Night Elf/Gnome), `8589934770` = Horde, `null` = open.

## Band

Lowest contracted minLevel **30** (93035/93037/93041/93072/93125/93129/93188)
to highest contracted quest level **49** (93404 Rot and Regret) = **30-49**.
`minnull` treated as no-minimum (B1 precedent). 93404 (49/minnull) is IN by the
zone-finale rule's letter (its min is unrecorded, its chain is in-band).

## IN ledger (28)

| ID | Title | Lvl/Min | Accept | Turn-in | Notes |
|----|-------|---------|--------|---------|-------|
| 92914 | Strange Pylons | 43/- | Shen'dralar Pylons 577959/577960 | Mordent Evenshade 253471 | object accept; event objective @47.6,76.66 |
| 96010 | Fragments of the Pylons | 41/- | Mordent Evenshade | Mordent Evenshade | item objs 255656/255657, sources unmapped (R2) |
| 96018 | Powering the Pylons | 43/- | Mordent Evenshade | Mordent Evenshade | pre 96010 |
| 93016 | A Brief History Lesson | 43/- | Mordent Evenshade | Mordent Evenshade | pre 96018 |
| 93394 | Meeting the Magister | 43/- | Mordent Evenshade | Magister Kirandis 254656 | pre 93016 |
| 93341 | Forlorn Gardens | 43/- | Mithera 254578 | Mithera | pre 93394; pedestal event @70.32,79.69 |
| 93362 | What They've Done to My Peonies | 43/- | Mithera | Mithera | pre 93341; kills 254566/254567/254572, all 2652 |
| 93594 | Word of the Woods | 43/- | Mithera | Woodwyrd 254674 | pre 93341 |
| 93404 | Rot and Regret | 49/- | Woodwyrd | Woodwyrd | pre 93594; kill Woodwyrd + Vial 258296 (source obj 612179 unmapped, R2) |
| 93601 | Passing the Blame | 45/- | Woodwyrd | Kog'thug 253527 | pre 93404, delivery |
| 93604 | Agamaggan's Blood | 45/- | Kog'thug | Kog'thug | pre 93601; blood 260237 via kill-credit npc 255669, no spawns (R2) |
| 93606 | Not on Squealing Terms | 45/- | Kog'thug | Quolga 255678 | pre 93604; Bouquet 260244 sourceless (R2) |
| 93450 | Phantasmal Problems | 42/- | Vindael 254717 | Vindael | pre 93394; Blade 258735 sourceless (R2) |
| 93546 | Spectral Iron Ore | 42/- | Vindael | Vindael | pre 93450; ore 259226 x10, source objs unmapped (R2) |
| 96060 | Tempered Expectations | 42/- | Vindael | Vindael | pre 93546 |
| 99257 | A Heart of Crystal | 43/- | Historian Biraxas 255486 | Biraxas | pre 93394; heart 286647 drops from 252711 (2652) |
| 99258 | Mana Mania | 43/- | Biraxas | Biraxas | pre 99257; kill 276401 (2652) |
| 93035 | Ravaging Ravagers | 38/30 | Nerlokh 253177 | Nerlokh | pre 93034 (Desolace, soft-pre) |
| 93037 | Outing Outcasts | 40/30 | Nerlokh | Nerlokh | pre 93034 (Desolace, soft-pre) |
| 93041 | Facing the Truth | 38/30 | Nerlokh | Uthek 5397 (Desolace expedition) | pre 93035+93037; feeds Desolace 93044 |
| 93125 | Going Home | 43/30 | Rokren 254040 | Nerlokh | no pre |
| 93072 | Long-Term Solutions | 43/30 | Hagiak 253851 | Hagiak | pre 93066 (Desolace, soft-pre); kills 254283/254284 (2652) + 8x 11559 (Desolace 1443 expedition) |
| 93129 | Threat of Starvation | 43/30 | Hagiak | Hagiak | pre 93066 (Desolace, soft-pre) |
| 93188 | Return to Orgrul | 43/30 | Hagiak | Orgrul 253136 (2652 spawn) | pre 93072+93129; feeds Desolace 93196 |
| 93568 | Partially Digested Collar | 45/- | item 259461 (Prowler 255207, 2652) | Liranne 255385 | item-start, sourcing in-zone |
| 93574 | Corpsefeeder's Carapace | 45/- | item 259893 (Corpsefeeder 253394 rare elite, 2652) | Kog'thug | item-start, sourcing in-zone |
| 93609 | Forlorn Necklace | 45/- | item 260247 (no drops anywhere, bag) | Mithera | sourceless item-start (R2 bag note) |
| 93644 | Tattered Journal | 45/- | item 260347 (Magram Necromancer 253272, 2652; also 11559 Desolace) | Mordent Evenshade | item-start, narrow drop, sourcing in-zone |

## OUT (4) — Horde-gated pre chain

93058 Saving Our Own, 93062 Bone Burying (both pre 93045), 93122 Checking
Things Out (pre 93058+93062), 93128 Khan Jehn (pre 93122). Pre 93045 Test Your
Theory is Horde-only (races 8589934770), uncontracted anywhere (absent from the
Desolace census, correctly excluded there as Horde-only). An Alliance player can
never complete 93045, so Nerlokh will never offer 93058/93062 and the four are
uncompletable on the Alliance route — the same class of exclusion as a
Horde-only quest. Their accepts are race-open on 2652, so the Horde block
should review this chain (93045 + these four) for its own census. If
pre-enforcement proves softer than the data suggests, Butler may rule them back
in. 93128's twin 93196 (Khan Jehn, pre 93188) IS reachable and stays in
Desolace's contract — no twin conflict.

## Cross-zone bookkeeping

Already contracted in Desolace (accepts from dual-spawn Orgrul/Nerlokh/Uthek,
zone 1443, NOT this contract): 92844, 92846, 92847, 92873, 92893, 92894, 93066,
93196. Their 2652 legs (93066 ends at Hagiak, 93188 feeds 93196) are handled by
soft-pre on our side. Our 93041 feeds Desolace 93044 (pre 93041, contracted).
Pres living in Desolace: 93034 (pre of 93035/93037), 93066 (pre of
93072/93129), 92841-chain (pre of Desolace's chain, not ours). No Horde-only
quest accepts on 2652 (all 32 records are null or Alliance); Horde set-aside
count is 0 as quests, with the 4-gated chain noted above for Horde review.

## Unused objects (companion-round material, not core)

Centaur Supplies 602101 (9 fixed points SW) and Evenshade's Journal 613713
(next to Mordent) are referenced by NO quest objective — not core content.

## BORDERLINE

1. 93058/93062/93122/93128 — see OUT section; excluded as a block rather than
   contracted with unfillable soft-pres because an accept that can never fire
   would wedge the route. Decided: OUT.
2. Band floor 30 vs content level 38+: six min30 quests, two min35 (both OUT),
   twenty minnull. Per the derivation rule (lowest contracted minLevel to
   highest quest level) the band is 30-49. Decided: 30-49.
3. 93404's kill-Woodwyrd objective (giver is the target, count null) — routed
   as a complete at his point; the Vial rides an R2 note. No invention.
4. No race header: all 28 contracted quests are races=null (open). No class or
   profession quests in the set (all classes=null).
