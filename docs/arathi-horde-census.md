# Arathi Highlands (Horde) census

Accept-zone key: **1417** (verified by count: 117 quest records carry
`zone=1417` in this data build — the same key and the same count the
Alliance census (`docs/arathi-census.md`) examined). Race masks in
the data: 8589934770 = Horde, 4294967373 = Alliance, null = neutral
(shared). Faction picture: **50 Horde-mask / 42 Alliance-mask / 25
null** (22 neutral + 3 class-8-gated null: the 96784-96786 Rogue chain,
shared per the Duskwood ruling, contracted in the main guide).

Method: every zone-1417 record examined against the pack's inclusion
rules; the Alliance census's 50 banked Horde set-asides reconciled one
by one against the Horde-mask pool; start-item scan run over the whole
117-record candidate pool; pres/exclusives and outside legs resolved
from data (`npcs.json`, `objects.json`, `items.json`, `quests.json`
cross-checked); giver spawn maps verified for every IN quest (all
spawn on 1417 — no city-rule cases).

## Band: 30-40 (+ writ special)

Contracted minLevels: seven m29 legs (655, 672, 674, 675, 701, 702,
847), an m30 bulk (671, 677, 678, 679, 680, 688, 92707, 97539, 92519),
m32 x7 (the 639-646 sigil chain), m35 x2 (673, 6622), m36 (95143),
one m24 low leg (95663, see BORDERLINE (a)), m40 profession
(5146, skill-gated). Quest levels run 31-42 in the core, 45 (6622),
55 (5146), 60 (94212 writ). Header band **levels 30-40**; the L60
writ 94212 rides as the writ special (min 1, excluded from band logic
per the Hillsbrad precedent the Alliance census cites). Above-band OUT
by minLevel: 7846/7847 (m46). Low-edge legs (m29 x7, m24 x1) are IN:
below-band-edge is not an OUT rule, and the Alliance census contracted
its own m24-m28 low outliers.

No race header for the guide: no contracted quest is locked to a single
Horde race. Class gates: none in the Horde pool (the class-gated
records on this key are the Alliance-mask Shaman chain
79358/96016/96135/96264 and the null-mask Rogue chain 96784-96786 —
both main-guide business, neither duplicated here). Profession-gated:
5146 (Leatherworking) and 6622 (First Aid) ride `optional` + `when
skill` per the pack rule.

Reconciliation of the Alliance census's banked set-asides: **29 IN, 21
OUT** (7846/7847 above-band; 16 Arathi Basin bracket records + 3
Defiler's care packages, repeatables per the Alliance screen — each
ruled below). The 50 banked IDs match the 50 Horde-mask zone-1417
records exactly (verified programmatically — no more, no fewer), so
this enumeration found no Horde quests beyond the bank.

Item-start enumeration (start-item scan over the whole 117-record
pool): Horde-mask item-starts are **exactly one**: 94212 (Craftsman's
Writ: Elixir of Wisdom, item 264012). 92707 has NO start record at
all (no NPC, object, or item) — sourceless, not item-started; it rides
with an honest R2 bag-note (Shen'dralas precedent). Null-mask writs
belong to the main guide (contracted there). Alliance-mask item-starts
are that guide's business.

## IN (29)

Hammerfall hub (Gor'mul 2792 @72.64,33.93; Tor'gan 2706 @74.72,36.29;
Drum Fel 2771 @74.24,33.92; Korin Fel 2772 @74.04,33.07; Doctor
Gregory Victor 12920 @73.41,36.89; Zaruk 2787 @74.54,35.64):

- 655 Hammerfall | 34/29 | no pre | Gor'mul->Tor'gan courier opener, no objectives
- 671 Foul Magics | 33/30 | no pre | 10 Bloodstone Amulet 4495 off the Boulderfist family (Tor'gan->Tor'gan)
- 672 Raising Spirits | 34/29 | pre 655 | 10 Highland Raptor Eye 4512 (Tor'gan->Tor'gan)
- 673 Foul Magics | 40/35 | pre 671 | Befouled Bloodstone Orb 4510 (Tor'gan->Tor'gan)
- 674 Raising Spirits | 34/29 | pre 672 | courier to Gor'mul, no objectives
- 675 Raising Spirits | 34/29 | pre 674 | Gor'mul->Tor'gan courier, no objectives
- 701 Guile of the Raptor | 37/29 | pre 675 | 12 Raptor Heart 4513 (Tor'gan->Tor'gan)
- 702 Guile of the Raptor | 37/29 | pre 701 | courier to Gor'mul, no objectives
- 847 Guile of the Raptor | 37/29 | pre 702 | Gor'mul->Tor'gan courier, no objectives
- 677 Call to Arms | 32/30 | pre 676 (Alterac accept, unrouted — pre-note) | 10 Witherbark Axe Thrower 2554 + 10 Headhunter 2556 + 8 Witch Doctor 2555 (Witherbark village east 59-67, 67-82; Drum Fel->Drum Fel)
- 678 Call to Arms | 38/30 | pre 677 | 10 Boulderfist Brute 2566 + 4 Magus 2567 (ogre mound south-center 49-54, 72-80)
- 679 Call to Arms | 40/30 | pre 678 | 7 Boulderfist Shaman 2570 + 3 Lord 2571 (ogre grounds far south-west 17-20, 64-69)
- 680 The Real Threat | 40/30 | pre 678 | Or'Kalar's Head 4551 (Korin Fel->Korin Fel; Or'Kalar placed from data at guide time)
- 95143 Finding Tan'jani | 38/36 | no pre | Tor'gan sends to Tan'jani — ends outside the zone (expedition turn-in, placed from data)
- 97539 Silky Sutures | 36/30 | no pre | 12 Surgical Spidersilk 278225 (Victor->Victor)
- 92519 Ward Restocking | 36/30 | pre 97539 | Packaged Tonics 278462 (Victor->Victor)
- 95663 Dragonmaw Rumors | 31/24 | no pre | Zaruk->Deathstalker Agent 13155 (Wetlands 1437 — expedition turn-in; next 95682 Open the Maw continues there) — low-edge leg, see BORDERLINE (a)
- 92707 The Giant in the Den | 33/30 | NO START RECORD — R2 bag-note, see BORDERLINE (b) | Goliath's Wristguards 253711 (placed from data) -> Drum Fel
- 94212 Craftsman's Writ: Elixir of Wisdom | 60/1 | ITEM-START 264012, no pre | writ + Elixir of Wisdom 3383 -> Muggol Breezebeard 257296 (in-zone, 1417) — optional, writ special
- 5146 Elemental Leatherworking | 55/40 | no pre; excl 5145/5148 (sister specializations, accept elsewhere — not candidates; player picks one) | 2 Heart of Fire 7077 + 2 Globe of Water 7079 + 2 Core of Earth 7075 + ... -> Brumn Winterhoof 7869 @28.27,45.09 — optional + when-skill (profession rule)
- 6622 Triage | 45/35 | pre 6623 (Durotar accept, unrouted — verified NOT in the Durotar contract; pre-note) | 15 Patients Saved event @ Dustwallow 67.79,49.06 (Theramore hospital — expedition complete) -> Victor — optional + when-skill (First Aid)

Sigil chain, Hammerfall east (Zengu 2703 @73.8,33.96; Tor'gan; Trollbane's Tomb object 2703 @28.86,59.62):

- 639 Sigil of Strom | 37/32 | pre 638 (Stranglethorn accept, CONTRACTED in stranglethorn-horde — pre-note; chain reads whole) | Sigil of Strom 4440 -> Zengu
- 640 The Broken Sigil | 40/32 | pre 639 | 11 Sigil Fragment 4450 -> Tor'gan
- 641 Sigil of Thoradin | 40/32 | pre 640 | courier to Zengu, no objectives
- 643 Sigil of Arathor | 41/32 | pre 641 | Sigil of Arathor 4458 -> Zengu
- 644 Sigil of Trollbane | 42/32 | pre 643 | Sigil of Trollbane 4466 -> Zengu
- 645 Trol'kalar | 42/32 | pre 644 | Zengu->TROLLBANE'S TOMB (object turn-in at the Tomb, west) — NOT accept-only; the turn-in is the object interact
- 646 Trol'kalar | 42/32 | pre 645 | take at the Tomb -> Zengu (chain finale)

Myzrael twin (Keystone object 2688 @36.08,58.09):

- 688 Myzrael's Allies | 40/30 | pre 652 (shared Myzrael chain, main guide — pre-note) | take at the Keystone -> Zaruk @74.54,35.64. Horde twin of Alliance-contracted 653 (clean faction-twin shape, Hillsbrad 555/7321 precedent); shared links NOT duplicated.

## OUT (21)

- 7846 Recover the Key! | 51/46 | pre 7845 (Hinterlands accept) | above-band (min 46)
- 7847 Return to Primal Torntusk | 51/46 | pre 7846 | above-band (min 46)
- 8120 The Battle for Arathi Basin! | 55/50 | AB bracket record (excl 7 incl. Alliance 8105/8166-8168) | repeatable battleground — OUT per the Alliance screen
- 8121 Take Four Bases | 60/60 | AB bracket | repeatable — OUT
- 8122 Take Five Bases | 60/60 | pre 8121 | AB bracket | repeatable — OUT
- 8123 Cut Arathor Supply Lines | 55/50 | AB bracket | repeatable — OUT
- 8124 More Resource Crates | 55/50 | AB bracket | repeatable — OUT
- 8160/8161/8162 Cut Arathor Supply Lines | 45/40, 35/30, 25/20 | AB brackets | repeatables — OUT
- 8163/8164/8165 More Resource Crates | 45/40, 35/30, 25/20 | AB brackets | repeatables — OUT
- 8169/8170/8171 The Battle for Arathi Basin! | 45/40, 35/30, 25/20 | AB brackets (excl each other + 8120) | repeatables — OUT
- 8299 Cut Arathor Supply Lines | 60/60 | AB bracket | repeatable — OUT
- 8300 More Resource Crates | 60/60 | AB bracket | repeatable — OUT
- 8263/8264/8265 Defiler's Basic/Standard/Advanced Care Package | 34/25, 44/35, 60/45 | bracketed mount-exchange-style repeats (excl each other) | repeatables — OUT

Set-aside accounting (not contracted here, listed for the record):
42 Alliance-mask records = 23 contracted in the Alliance guide
(632, 647, 653, 657, 658, 660, 661, 681, 682, 684, 685, 691,
693-697, 79358, 92872, 95315, 96016, 96135, 96264 — includes the
Alliance Shaman chain; the 96784-96786 Rogue chain is null-mask
shared) + 19 ruled OUT by the Alliance census as repeatable
battleground/care-package records (8080, 8081, 8105, 8114, 8115,
8154-8159, 8166-8168, 8260-8262, 8297, 8298).
25 null-mask records = 24 contracted in the Alliance guide + 636
Legends of the Earth (OUT broken: no start, no end, no objectives —
the Alliance census's documented broken record, confirmed in data).

## BORDERLINE

(a) 95663 Dragonmaw Rumors (min 24 in a 30-40 band): IN. The accept
test passes (Zaruk spawns 1417), the chain runs somewhere real
(95682 accepts at the Deathstalker Agent in the Wetlands), and the
Alliance census contracted its own m24-m28 low outliers — below-band-
edge is not an OUT rule. Routed as an early Hammerfall leg with the
Wetlands expedition turn-in.

(b) 92707 The Giant in the Den (no start record): IN. Real quest
(lvl 33, min 30, item objective + Drum Fel turn-in both in data);
sourceless accepts ride the R2 bag-note pattern (Shen'dralas
precedent), never an invented source.

(c) 677 Call to Arms (pre 676 accepts in Alterac, zone 1416): IN.
Accept test passes (Drum Fel, 1417); the pre is simply outside this
contract. Pre-note + normal accept (Thousand Needles 1147 precedent);
structural pre warning expected and accepted.

(d) 6622 Triage (pre 6623 accepts in Durotar, zone 1411): IN.
Verified 6623 is NOT in the Durotar contract (106 IDs checked), so no
cross-guide discharge is available. Pre-note + normal accept; the
Dustwallow event complete rides an expedition leg. Structural pre
warning expected and accepted.

(e) 645/646 Trol'kalar same-name pair + 671/673, 672/674/675, 677/678/
679 same-name multiples: all sequential chain links (each pre points
at the previous link; 645's next IS 646), NOT mutually exclusive
variants — every link routes. 645's turn-in is the Tomb object
interact, 646's accept is the Tomb: no accept-only record, no
invented turn-in.

(f) 5146 excl 5145/5148 (specialization exclusives): IN optional.
The counterparts are not zone-1417 candidates (accept elsewhere), so
there is no in-contract variant to pick between; the player picks one
specialization and the route stays optional + skill-gated.

(g) 636 Legends of the Earth: OUT broken. Null-mask, so it cannot
ride the Horde contract on faction grounds anyway; and it has no
start, no end, and no objectives — nothing to route (Alliance census
agrees). If data ever grows it a giver, it belongs in the MAIN guide
(shared), never here — no silent contracting.
