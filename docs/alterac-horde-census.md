# Alterac Mountains (Horde) census

Accept-zone key: **1416** (verified by count: 164 quest records carry
`zone=1416` in this data build — the same key and the same count the
Alliance census (`docs/alterac-census.md`) examined; Alterac Valley is
the separate battleground map 1459 and out of scope). Race masks in the
data: 8589934770 = Horde, 4294967373 = Alliance, null = neutral (both
factions), 34 = Orc+Tauren (the Shaman-eligible Horde races — caught by
inspection, not by mask read), 4294967296 = non-playable/docs-only
(Child of Nature 94912 + Welcome to Azeroth 94947, neither Horde).

Method: every zone-1416 record examined against the pack's inclusion
rules; the Alliance census's 67 banked Horde set-asides reconciled one
by one against the Horde-mask pool plus the races-34 record; the
battleground screen applied as a class (repeatable or not, per the
brief); start-item/object scan run over the whole 164-record candidate
pool; pres/exclusives and outside legs resolved from data (`npcs.json`,
`objects.json`, `items.json`, `quests.json`, `spawnz.json`
cross-checked).

Pool breakdown: 66 Horde-mask + 1 races-34 (79365) + 74 Alliance-mask +
21 null + 2 docs-only. The 67 banked set-asides are exactly the 66
Horde-mask zone-1416 records plus 79365 (verified programmatically — no
more, no fewer). Zero Horde-mask/34 records sit inside the Alliance
`alterac` contract (20 quests), so the exclusive-contracts precedent
holds with one directional check (565/555 twin, BORDERLINE (h)).

## Band: 20-45

Contracted levels run 20 (2480 Hinott's Assistance) to 45 (2934/2935
venom pair). Contracted minLevels run 13 (1066/1067 Innocent Blood pair)
through 40 (2934/2935/2938 venom trio), with sub-30-min intros IN as
in-zone content per precedent. Header band **levels 20-45**. Above-band
but contracted with honest notes: 2938 (L55/m40 — zone finale whose
minLevel is in band, per the band rule) and the Shaman chain 8411-8413
(L50-52/m50, class-gated per the STV 8116-8119 precedent; every reagent
bag-noted — none names a 1416 source). Above-band OUT: the m51
Alterac-Valley/Frostwolf set (BG screen below) plus 7181/7381
(repeatable + BG).

No race header for the guide: no contracted quest is locked to a single
Horde race. Class gates: Rogue (2480 — class 8, Ravenholdt/Junkboxes mask), Shaman (79365, 8411/8412/8413).
One profession gate: Cooking 185 (7321, optional + when-skill). No other
skill gates in the Horde pool. One dungeon turn-in: none — every
contracted turn-in sits in the open world or a capital (capital legs
are expeditions, city rule as always). No contracted objective sits
inside an instance.

Reconciliation of the Alliance census's banked set-asides: all 67
accounted for — 50 IN, 17 OUT (14 battleground-screen + 1 seasonal + 1
broken + 1 accept-outside — each ruled below). (An earlier draft of this
census routed the Desolace clan quests 1367/1368/93225/94872/94873/92812
and 93045 here; their records carry zone 1443 with Desolace-only
givers, so they are not 1416 candidates at all and stay homed in
desolace-horde — see BORDERLINE (a). They were never in the 67.)

Item-start enumeration (start-item scan over the whole 164-record
pool): item-started Horde-mask records: NONE. The Horde contract's
poster quests (549/566/567) are OBJECT-starts (WANTED boards
1763/556670 + Dangerous board 2008/556669, all placed on 1416) — routed
at the boards. Pool-wide item-starts are the Alliance writs + 6681 +
79362/79363/96137 (all Alliance-contracted or below-band). **Zero
Horde-mask item-starts — asserted only after the scan.** Repeatable
scan over the Horde pool: 7181/7381 (Korrak pair, BG — OUT),
6983 (Winter Veil — OUT seasonal). Events: 6983 only (seasonal).
`[PH]`: none. Broken: 1051 (Vorrel spawnless everywhere — OUT).

## IN (50)

Tarren Mill hub (dual-map NPCs spawn on 1416 AND 1424; every accept
below is routed at the 1416 point — the operational accept test passes
in-zone; the 1424 twin is never used):

Elixir chain (Apothecary Lydon 2216 @60.1,80.7):
| 496 Elixir of Suffering | 22/19 | no pre | 10 Gray Bear Tongues (2351/2354/2356, 1416) + Creeper Ichor (2349/2350, 1416) |
| 499 Elixir of Suffering | 22/19 | pre 496 | deliver to Umpi 2230 (in-zone) |
| 501 Elixir of Pain | 24/21 | no pre | 10 Mountain Lion Blood (2384/2406/2407, 1416, 15%) |
| 502 Elixir of Pain | 24/21 | pre 501 | feed Stanley 2274 (in-zone) |
| 509 Elixir of Agony | 28/24 | no pre | 6 Mudsnout Blossoms — object 1723 spawns ONLY on 1424 (Hillsbrad) → Hillsbrad expedition objective |
| 513 Elixir of Agony | 30/24 | pre 509 | Composite to Faranell 2055, Undercity (48.82,69.28) — capital expedition; next 515 accepts in Undercity (uncontracted, noted) |
| 517 Elixir of Agony | 30/24 | pre 515 (Undercity-accept, uncontracted — 5148 precedent: game-gated accept + note) | Keg of Shindigger Stout — object 1727 on 1417 (Arathi Dun Garok) + 1424 (Hillsbrad Dun Garok side) → expedition objective (Hillsbrad side, shared with the Dun Garok leg) |
| 524 Elixir of Agony | 30/24 | pre 517 | Rug object 1728 (61.7,80.3, in-zone) — no travel needed |

Gol'dir chain (Krusk 2229; Gol'dir 2316 @59.96,43.74):
| 506 Blackmoore's Legacy | 36/29 | pre 503 | Gol'dir→Krusk, no objectives |
| 507 Lord Aliden Perenolde | 42/29 | pre 506 | Perenolde 2423 (1416 Durnholde) + Elysa 2317 turn-in |
| 508 Taretha's Gift | 40/29 | pre 507 | Taretha's pendant → Krusk; chain finale |

Battle of Hillsbrad chain (Darthalia 2215 @61.1,82.1):
| 527 Battle of Hillsbrad | 24/19 | no pre | farmers/farmhands/Ray on the 1416 border farms (24-27, 95-99); Farmer Getz 2403 spawns ONLY on 1424 → noted Hillsbrad touch (one kill, not a leg) |
| 528 Battle of Hillsbrad | 25/19 | pre 527 | 15 Peasants — 2267 spawns ONLY on 1424 (Southshore) → Hillsbrad expedition leg |
| 529 Battle of Hillsbrad | 26/19 | pre 528 | Verringtan + Apprentices + Shipment object 1736 — ALL 1424-only → Hillsbrad expedition leg (Southshore/town cluster) |
| 532 Battle of Hillsbrad | 26/19 | pre 529 | Burnside + Councilmen + Proclamation 1761 + Registry object 1759 — ALL 1424-only → Hillsbrad expedition leg (town cluster) |
| 539 Battle of Hillsbrad | 28/19 | pre 532 | Bonds + Miners, 1424-only → Hillsbrad expedition leg |
| 541 Battle of Hillsbrad | 30/19 | pre 539 | Dun Garok (1417 + 1424; Hillsbrad side 68-72, 75-80 chosen, shared with the sword leg) → Hillsbrad expedition leg |
| 550 Battle of Hillsbrad | 32/19 | pre 541 | no objectives; end Varimathras, Undercity — capital expedition turn-in |
| 546 Souvenirs of Death | 25/20 | pre 527 | 30 Skulls off Hillsbrad humans; 2266 Hillsbrad Farmer carries them on 1416 (no rate in the data — family farm, honest note) |

Syndicate/Durnholde (Krusk 2229 @62.2,82.5; posters in-zone):
| 498 The Rescue | 22/17 | no pre | cages 1721/1722 spawn ONLY on 1424 (Durnholde east) → Hillsbrad expedition objective; pre of 533 via its preAny |
| 533 Infiltration | 34/29 | preAny 498 | Missive off Footpad/Thief (1416 Durnholde camp, 33%) |
| 535 Valik | 34/29 | parent 533 (no formal pre — unconditional accept + link note, STV-13542 pattern) | Southshore Stout: Drunken Footpad 97% on 1416 (vendors unlisted for 1416) → Valik in-zone |
| 549 WANTED: Syndicate Personnel | 22/17 | OBJECT-START posters in-zone; no pre | Rogues + Watchmen 1424-only (Syndicate camp 65-67, 45-48) → Hillsbrad expedition leg; pre of 566 |
| 566 WANTED: Baron Vardus | 40/35 | preAny 549 | Baron Vardus 2306 on 1416 (5 pts, 100% head) — fully in-zone |
| 567 Dangerous! | 28/19 | OBJECT-START board in-zone; no pre | 4 named town kills, ALL 1424-only → Hillsbrad expedition leg |

Crown chain (Melisara 2278 @61.5,82.5):
| 518 The Crown of Will | 39/34 | pre 495 (Silverpine-accept, uncontracted — outside pre noted; the 495 twin 8410-style city rule does not apply, this one is simply elsewhere) | 10 Crushridge Maulers (in-zone) |
| 519 The Crown of Will | 41/34 | pre 518 | Targ 2420 + Muckrake 2421 + Glommus 2422 heads (100%, 1 pt each, in-zone) |
| 520 The Crown of Will | 43/34 | pre 519 | Mug'thol 2257 head + Crown (100%, in-zone) |
| 521 The Crown of Will | 43/34 | pre 520 | no objectives; end Sharlindra, Undercity (text says Undercity over its Silverpine spawn) — capital expedition turn-in |

Dalaran + Perenolde (Magus 2410 @60.3,82.8; Thaivand 2429 @62.9,81.4):
| 544 Prison Break In | 33/30 | no pre | 4 Bloodstone turn-ins (Kegan/Ricter/Alina/Dermot, 100%, 1 pt each, in-zone) |
| 545 Dalaran Patrols | 35/30 | pre 544; Hillsbrad lead-in 93680 (Key to the City, Hillsbrad-accept, hillsbrad-horde-contracted — named, not routed) | 6 Summoners + 12 Slaves (Dalaran camp 10-22, 73-84, in-zone); next 92434 is hillsbrad-horde-contracted (chain link noted, not duplicated) |
| 552 Helcular's Revenge | 33/29 | no pre | Helcular's Rod off Yetis (1416, 6%) → Thaivand |
| 553 Helcular's Revenge | 33/29 | pre 552 (completed — plain accept + note, STV-5148 pattern) | charge at Flames 1768/1769/1770 (in-zone) |
| 556 Stone Tokens | 33/30 | no pre | 10 Worn Stone Tokens (Dalaran guards, 1416, 47-48%) → Bel'varil 2437 |
| 557 Bracers of Binding | 33/30 | pre 556 | 4 Bracers off Elemental Slaves (1416, 80%) |

Stone + Hammer + Vorrel-adjacent singles:
| 1361 Regthar Deathgate | 32/30 | no pre; starters Krusk (1416) + Nazgrel/Belgrom (Orgrimmar-only — noted, not used) | no objectives; end Regthar 3389, Barrens (45.34,28.41) — Barrens expedition turn-in; pre of uncontracted 1362 (Desolace guide turns it in at Felgur — chain link noted) |
| 547 Humbert's Sword | 30/26 | no pre | sword off Dun Garok mobs (8%, Arathi+Hillsbrad) → Hillsbrad-side Dun Garok expedition leg; Humbert ends in-zone |
| 676 The Hammer May Fall | 32/30 | no pre | Boulderfist Ogres/Enforcers (Arathi-only) + end Drum Fel 2771, Arathi (74.24,33.92) — Arathi expedition (objectives + turn-in) |
| `when onquest 1065` soft-pre mini at Lydon (turn in 1065, accept 1066) — the pre ends in-zone at the follow-up's giver (Kadrak pattern) |
| `when onquest 2479` soft-pre mini at Hinott (turn in 2479, accept 2480) — same pattern; 2479 accepts in Orgrimmar (3401), ends in-zone |
| 7321 Soothing Turtle Bisque | 31/28 | skill 185 (Cooking); excl 555 (Alliance Hillsbrad twin, unroutable) | Turtle Meat (Snapjaw 2408/ Benj 14223, 1416) + Soothing Spices (Jeffcoat vendor, npc-pinned) → Jeffcoat; optional + when skill Cooking 1 (Galvan pattern); excl noted, never fires for Horde |
| 79365 With Wind Beneath Your Wings | 40/30 | races 34 (Orc+Tauren) + class 64 (Shaman); no pre | no objectives; Bath'rah → Rau Cliffrunner 4722, Thousand Needles (46.14,51.71) — TN expedition turn-in; `only Shaman` composing with the race restriction (engine form argued in BORDERLINE (j)) |
| 8411 Mastering the Elements | 50/50 | Shaman; excl 8410 (Mulgore twin, thunder-bluff-contracted — noted, never fires here) | Elemental Air/Earth/Fire/Water — NONE names a 1416 source (verified scan) → bag notes; Bath'rah→Bath'rah |
| 8412 Spirit Totem | 52/50 | Shaman; pre 8410/8411 (8411 satisfies) | Spider Eyes + Thick Claws — no 1416 source → bag notes |
| 8413 Da Voodoo | 52/50 | Shaman; pre 8412 | 6 voodoo feathers — no 1416 source (custom mobs, unplaced) → bag notes; chain finale |

Venom trio (Lydon 2216 @60.1,80.7):
| 2934 Undamaged Venom Sac | 45/40 | pre 2933 (Hinterlands, starter-unknown — outside pre noted) | Sac off Witherbark Broodguard 2686 (Hinterlands-only, 10%) → Hinterlands expedition objective |
| 2935 Consult Master Gadrin | 45/40 | pre 2934 | no objectives; end Gadrin 3188, Durotar (55.95,74.72) — Durotar expedition turn-in |
| 2938 Venom to the Undercity | 55/40 | pre 2937 (Durotar-accept, uncontracted — 2936/2937 Durotar pair noted for a future Durotar round; 5148 precedent: game-gated accept + note) | no objectives; end Faranell, Undercity — capital expedition turn-in; zone-finale above-band-by-level, minLevel in-band — IN per the band rule |

Gelkis/Magram befriendings (Maurin? No — Alterac-side: the befriendings accept in-zone for Horde):
| 503 Gol'dir | 36/29 | pre 533 (in-contract; 533 itself opens via its 498 preAny — see Rescue row) | Rusted Iron Key off Jailor Borhuin 2431 (100%, in-zone) + event at Gol'dir's hold (from data @60.6,43.8) → Gol'dir 2316 turn-in, in-zone |

Innocent Blood pair (Lydon 2216 @60.1,80.7):
| 1066 Blood of Innocents | 23/13 | pre 1065 (Mulgore-accept, outside — soft-pre mini below) | Vials of Innocent Blood off Syndicate Shadow Mages (1424-only, 80%) → Hillsbrad expedition objective; sub-band intro IN |
| 1067 Return to Thunder Bluff | 23/13 | pre 1066 | no objectives; end Zamah, Thunder Bluff (22.81,20.89) — TB expedition turn-in |
| `when onquest 1065` soft-pre mini at Lydon (turn in 1065, accept 1066) — the pre ends in-zone at the follow-up's giver |

Hinott (Hinott 2391 @60.3,80.9):
| 2480 Hinott's Assistance | 20/20 | pre 2479 (Orgrimmar-accept, outside); class 8 (Rogue) | event objective in Hillsbrad (map 1424 @61.57,19.21) → Hillsbrad expedition objective; `only Rogue`; `when onquest 2479` soft-pre mini at Hinott (turn in + accept) |

## OUT (17)

- Battleground screen (14): 7082, 7101, 7124 (m51 AV objectives, Corporal Teeka); 7142 (m51, objective defeats Vanndar INSIDE Alterac Valley map 1459); 7222 (m51, no start data, pre of 7142 — BG chain link); 8272 (m51, pre 7142 — BG chain link); 7181 + 7381 (Korrak pair, repeatable + BG); 7161/7163/7164/7165/7166/7167 (Frostwolf rank chain, m51, Frostwolf rep-gated 729 — BG content, repeatable or not). All zone 1416/area 2597 but battleground content — OUT by class per the brief.
- Seasonal (1): 6983 You're a Mean One (event=2 Winter Veil, pre 6963 Orgrimmar) — OUT.
- Broken/unplaceable (1): 1051 Vorrel's Revenge — starter Vorrel Sengutz 3981 has NO spawn in npcs.json or spawnz (the turn-in Monika + the ring dropper Nancy ARE placed, but the accept is not) — OUT by the 7221 rule. If the giver is ever placed, Nancy's in-zone ring + Monika's turn-in resolve it; revisit with source.
- Accept-outside (1): 96984 Heart of Disruption — starter Image of Archmage Modera 269127 spawns ONLY on 1421 (Silverpine). Zone field 1416 loses to the operational accept test per the Redridge/Ironforge precedent and the Alliance BORDERLINE 5 (which moots the 92458 twin question the same way). Silverpine inherits it with the full chain (92432 Hillsbrad → 96984 → 97287 hillsbrad-horde, all Hillsbrad-contracted around it).
- Above-band: none beyond the BG/REP set (m44+ non-BG Horde records do not exist in the pool — verified by the level scan; 7028/7044-style L50+ non-BG quests are all null-mask here).
- Below-band: none (lowest contracted minLevel 13 rides as a sub-band intro per precedent; no Horde record is cut for low level).

## BORDERLINE (all decided, none silent)

(a) The Desolace-clan brief-vs-data conflict (named checks 1 and 3):
records 1367, 1368, 93225, 94872, 94873, 92812, 93045 (and shared
1369/1370) carry zone 1443 with Desolace-only givers (Maurin, Warug,
Uthek, Molkar — 1443-only spawns; 93045's ender Nerlokh is 2652-only).
They are not 1416 candidates at all, and all seven Horde records are
already contracted in desolace-horde (order 58). The operational accept
test (Redridge/Ironforge precedent, Alliance BORDERLINE 5) decides
over the zone field — and over the brief, per the game-data-wins rule:
OUT of this contract as accept-outside, homed where their accepts
live. The data also settles the clan-choice shape the brief asked
about: 1367/1368 carry no mutual exclusion (excl [] both ways), and
the Gelkis pick (94873) is the chain-consistent one there because
94872's next needs Alliance-only 93226. The Horde route reaches shared
1369/1370 through desolace-horde's pres (the ungated main guide serves
them to both factions). If a future data build moves these givers onto
1416, this contract re-opens them.
(b) 96984 accept-outside: same operational test as (a), same outcome.
The Modera image (269127) spawns only on 1421; the quest's zone field
(1416) loses. Silverpine inherits it with the full chain (92432
Hillsbrad → 96984 → 97287 hillsbrad-horde — both neighbors contracted
around it, verified above). The 92458 twin question is moot the same
way the Alliance census mooted it. OUT, documented.
(c) 1051 broken: Vorrel Sengutz 3981 has no spawn in npcs.json or
spawnz (checked both); Monika (turn-in) and Nancy (ring dropper, 100%,
in-zone) ARE placed. Same class as Alliance-broken 7221 (no placed
accept). OUT. Revisit only with a placed giver; the ring farm stays
valid.
(d) 8411-8413 above-band IN: m50/L50-52 inside a 20-45 band. Contracted
anyway per the STV 8116-8119 class-chain precedent: all accepts and
turn-ins in-zone at Bath'rah, no other gates, twin pre satisfiable
in-contract (8412's 8410-or-8411 needs 8411, held). The cost is honest
bag notes for all six reagents — the verified scan found no 1416
source for any of them (nearest are Desolace 1442/1443 elementals and
unplaced custom voodoo mobs). If the pack ever rules class chains
band-capped, these three drop as a unit.
(e) 2938 L55/m40 IN: zone-finale whose level exceeds the band with
minLevel in band — the band rule's explicit case (Alliance 96770
L46/m39 precedent). Its pre (2937, Durotar-accept, uncontracted) is
named, not routed; the UC turn-in rides the capital leg. The
2936/2937 Durotar pair is noted for a future Durotar round, which will
cite this contract the way Shen'dralas cites 93045's home.
(f) 79365 gating (named check 2): `only Orc,Tauren,Shaman` per line —
the engine's comma-joined multi-gate form (barrens 6365 `only
Orc,Troll`; ashenvale 78093 `only Human,Dwarf,Paladin`). races=34 is
exactly Orc+Tauren; class 64 is Shaman; the composition is verified by
lint in the guide round (the compiler is the check the brief asks
for). No further mask-miss catches: the full pool scan found races=34
exactly once (79365) and races=4294967296 twice (94912/94947, both
docs-only, uncontracted) — reported per the brief's scepticism rule.
(g) Hillsbrad-leg honesty: 528/529/532/539/541/549/567/498/546-touch/
1066/2480 all resolve objectives on 1424 (dual-map NPCs notwithstanding
— the OBJECTIVES' maps decide, per the accept/objective split in the
Alliance 92457-92459 ruling). Each leg names its 1424 points from the
dumps; nothing is routed on assumed adjacency. Dun Garok uses the
Hillsbrad-side points (shared with the 547 sword leg and the 517 keg);
Arathi-side points are noted, not used — except 676, which is a pure
Arathi leg (Boulderfist + Drum Fel both 1417).
(h) 546's skulls (None% rate on the 1416 dropper 2266): farmed, not
bag-noted — the dropper IS placed in-zone, so the honest form is a
family farm with the rate unknown, stated. If the playtest shows zero
credit across the family, it degrades to a bag note with no route harm.
(i) 535's parent link: parent=533 with no formal pre — routed as an
unconditional accept with the link noted (game-gated). If the game
proves it requires 533 completion, the note already sends the player
there first.
(j) 7321 vs 555: excl [555] named and dismissed — 555 is Alliance-mask
(Hillsbrad 1424), unroutable for Horde, so the exclusion never fires.
Skill gate (Cooking 185) + when-skill + optional per the Galvan
pattern; the twin question the brief raised is moot by mask.
