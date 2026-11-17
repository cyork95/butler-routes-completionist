# Stranglethorn Vale (Horde) census

Accept-zone key: **1434** (verified by count: 258 quest records carry
`zone=1434` in this data build — the same key and the same count the
Alliance census (`docs/stranglethorn-census.md`) examined). Race masks
in the data: 8589934770 = Horde, 4294967373 = Alliance, null =
neutral (both factions).

Method: every zone-1434 record examined; the Alliance census's 39
banked Horde set-asides reconciled one by one against the Horde-mask
pool; start-item/object scan run over the whole 258-record candidate
pool; pres/exclusives and outside legs resolved from data (npcs.json,
objects.json, items.json, spawnz.json cross-checked).

Pool breakdown: 39 Horde-mask + 35 Alliance-mask + 184 null. The 39
banked set-asides are exactly the 39 Horde-mask zone-1434 records
(verified programmatically — no more, no fewer). Zero Horde-mask
records sit inside the Alliance `stranglethorn` contract (123 quests =
29 Alliance-mask primary + 94 null shared), so the exclusive-contracts
precedent holds with nothing to de-duplicate.

## Band: 30-47

Contracted levels run 34 (581 Hunt for Yenniku) to 47 (3642/3643
Oglethorpe pair); the combat bulk sits 34-46. Contracted minLevels run
30-38 across the bulk (97386 m38 highest), with two sub-30 in-zone
intros IN as in-zone content per the Alliance precedent: 2843 (m20)
and the m1 chain finale 593 (see BORDERLINE (a)). Header band **levels 30-47**. Two records
ride above-band with their gates noted, per the writ/class-chain
precedent (Alliance BORDERLINE (c) contracted L55 7810 and five L60
writs inside a 30-45 band): 5148 (L55, Leatherworking skill gate) and
the 8116-8119 Shaman chain (L60, class + Zandalar rep gates).

No race header for the guide: no contracted quest is locked to a
single Horde race. One class gate: Shaman (8116-8119). Two profession
gates: Engineering (3642/3643), Leatherworking (5148) — routed
when-skill + optional like the Alliance Galvan chain. One dungeon
objective: none. One spawnless kill target: 95776 Var'Taka (no spawn
in npcs.json or spawnz — completes at the giver, 1046-pattern).

Reconciliation of the Alliance census's banked set-asides: all 39 are
IN. None is broken, phantom, repeatable-OUT, event, or above-band-OUT:
593 Filling the Soul Gem (repeatable-flagged — IN as the chain finale,
see BORDERLINE (a)) / 2843 Gnomer-gooooone! / Nimboya chain 581 Hunt
for Yenniku / 582 Headhunting / 584 Bloodscalp Clan Heads / 585
Speaking with Nezzliok / 586 Speaking with Gan'zulah (twin variants,
both Horde, both required by 588) / 588 The Fate of Yenniku / 589 The
Singing Crystals / 591 The Mind's Eye / 592 Saving Yenniku / 596 Bloody
Bone Necklaces / 598 Split Bone Necklace / 629 The Vile Reef (next
95748) / 1261 Marg Speaks (pre 1240 Barrens, ender Nazeer outside —
expedition) / 638 Trollbane (ender Zengu, Arathi — expedition) / 568
The Defense of Grom'gol / 569 same / 570 Mok'thardin's Enchantment /
571 same / 572 same / 573 same / 97453 Weed Whacked / 97386 The Offense
of Grom'gol (pre 569) / 2932 Grim Message (objective in the
Hinterlands — expedition) / 5148 Tribal Leatherworking (pre 2860
Feralas, Leatherworking skill) / Kin'weelay Gurubashi chain 95748 The
Gurubashi Legends of Old (pre 629) / 95770 Locating the Lost City (pre
95748) / 95773 Enemies in the Water (pre 95748, dual starters) / 95775
The Drowned City (pre 95770) / 95776 The Only Good Brinescale... (pre
95770+95773) / 96078 A Tale Spun Around the Fire (pre 95775, ends
Gadrin in Durotar — expedition finale) / Oglethorpe Horde pair 3642
The Pledge of Secrecy (preAny 3635 Undercity / 3637 Barrens;
Engineering) / 3643 Show Your Work (pre 3642; next 3645
Ironforge-keyed extra — expedition note) / 95141 Report to Rog'mar
(ender Krom'rosh in Riverglades — expedition) / Zandalar Shaman chain
8116 Vision of Voodress / 8117 same / 8118 same / 8119 The Unmarred
Vision of Voodress (Shaman + rep-gated).

Item-start enumeration (start-item scan over the whole 258-record
pool): item-started records are 594 (bottle 4098), 620 (sash 3985),
8183 (Heart 19802), 78830 (class Hunter), 79731 (scroll 216880, class
Priest), the five writs (264017/264026/264035/264044/264053), and 8552
(sash 3985) — all null-races and all already contracted in the
Alliance guide. **Zero Horde-mask records carry a start item.**
Repeatable/event scan over the Horde pool: one repeatable (593, ruled
IN below), zero events.

## IN (39)

| ID | Title | Lvl/min | Accept | Notes |
|----|-------|---------|--------|-------|
| 568 | The Defense of Grom'gol | 36/33 | Commander Aggro'gosh 2464 (32.17, 28.9) | 15 Lashtail Raptors 686, ring Grom'gol (30-39, 19-28) |
| 569 | The Defense of Grom'gol | 37/33 | Aggro'gosh; pre 568 | 10 Mosh'Ogg Brutes 1142 + 5 Witch Doctors 1144, east (35-38, 28-32) |
| 570 | Mok'thardin's Enchantment | 38/33 | Far Seer Mok'thardin 2465 (32.12, 29.24) | 8 Shadowmaw Claws 3838 off Panthers 684/1713 (south + northeast clusters) + Pristine Tigress Fang 3839 off Tigress 772 (15%) |
| 571 | Mok'thardin's Enchantment | 41/33 | Mok'thardin; pre 572 | Aged Gorilla Sinew 3862 off Elder Mistvale Gorillas 1557 (5%, south 30-34, 57-68) |
| 572 | Mok'thardin's Enchantment | 41/33 | Mok'thardin; pre 570 | 10 Jungle Stalker Feathers 3863 off Stalkers 687 (west-center 23-34, 36-51) |
| 573 | Mok'thardin's Enchantment | 44/33 | Mok'thardin; pre 571 | 10 Naga Explorers 1907 west coast (23-28, 58-64) + Holy Spring Water 737 off object 759 (28.96, 61.93); chain finale |
| 581 | Hunt for Yenniku | 34/30 | Nimboya 2497 (32.16, 27.72) | 9 Bloodscalp Tusks 3901 off west Bloodscalps (19-34, 8-21) |
| 582 | Headhunting | 37/30 | Nimboya; pre 581 | 20 Shrunken Heads 1532 off Bloodscalp Headhunters 671 (80%, west 20-24, 8-13) |
| 584 | Bloodscalp Clan Heads | 41/30 | Nimboya; pre 582; ends Cauldron 2076 | Gan'zulah's Head 3904 off Gan'zulah 1061 (23.44, 8.12) + Nezzliok's Head 3905 off Nezzliok 1062 (23.52, 9.53) |
| 585 | Speaking with Nezzliok | 40/30 | Cauldron 2076 (32.22, 27.6); pre 584 | 3 trophies off skull objects east: 3906 @2891 (46.13, 32.33), 3907 @2892 (42.21, 36.11), 3908 @2893 (47.65, 39.54) |
| 586 | Speaking with Gan'zulah | 46/30 | Cauldron; pre 584 (twin of 585, both required by 588) | 8 Hunters 669 + 6 Headhunters 781 + 4 Berserkers 783 east (43-48, 38-45) + Broken Armor 3909 off Ana'thek 1059 (44.3, 45) |
| 588 | The Fate of Yenniku | 45/30 | Cauldron; pre 585+586 | no objectives; ends Kin'weelay 2519 (32.27, 27.71) |
| 589 | The Singing Crystals | 45/30 | Kin'weelay; pre 588 | 3 Pulsing Blue Shards 3911 off Ironjaw Basilisks 1551 (80%, 41-44, 45-49) |
| 591 | The Mind's Eye | 46/30 | Kin'weelay; pre 589 | Mind's Eye 3616 off Mai'Zoth 818 (52.93, 27.6) east |
| 592 | Saving Yenniku | 46/30 | Kin'weelay; pre 591; ends Nimboya | Filled Soul Gem 3913 (comes out of 593 below) |
| 593 | Filling the Soul Gem | 46/1 | Yenniku 2530 (39.02, 58.35); pre 592; repeatable-flagged | chain finale, IN — see BORDERLINE (a); Soul Gem 3912 names no source (rides with the accept); complete + turn in at Yenniku |
| 596 | Bloody Bone Necklaces | 37/30 | Kin'weelay | 25 necklaces 3915 off west Bloodscalps (17%) |
| 598 | Split Bone Necklace | 42/30 | Kin'weelay; pre 596 | 25 necklaces 3916 off Ana'thek 1059 + Skullsplitter mobs 667/669/670/672/696/780/781/782/783/784 (10%, east 41-48, 30-45); finale |
| 629 | The Vile Reef | 37/30 | Kin'weelay | Tablet Shard 4094 off Gri'lek objects 179426/58 (24.77, 22.88); npcs.json point only, spawnz carries no entry |
| 638 | Trollbane | 37/32 | Nimboya | talk to Zengu 2703, Arathi (73.8, 33.96) — expedition extra turn-in; 639 (Arathi accept) stays out |
| 1261 | Marg Speaks | 40/30 | Cauldron; pre 1240 (Barrens accept, unrouted) | Jeweled Pendant 5942 off Dustwallow Muckshells/Lord Angler (5%, 1445 only) + turn-in Nazeer 4791, Dustwallow (35.21, 30.66) — expedition; 1262 (Barrens accept) stays out |
| 2843 | Gnomer-gooooone! | 35/20 | Scooty 7853 (27.6, 77.48); pre 2842 (Orgrimmar-routed) | wait on Scooty (kill-typed talk target, count null); when-mini turns in 2842 first |
| 2932 | Grim Message | 42/35 | Nimboya | place the message at the Hinterlands event point (23.41, 58.06, map 1425) — expedition objective leg |
| 3642 | The Pledge of Secrecy | 47/30 | Oglethorpe 7406 (28.36, 76.35); preAny 3635 (Undercity-routed) / 3637 (Barrens accept, unrouted); Engineering | pledge 11282 names no source (bag note, granted with the pre line); when-skill + optional; when-mini turns in 3635 first |
| 3643 | Show Your Work | 47/30 | Oglethorpe; pre 3642; Engineering | 6 Mithril Tubes + Accurate Scope + 2 Advanced Target Dummies, all crafted/sourceless (bag notes); when-skill + optional; 3645 (Ironforge-keyed, no objectives) is an uncontracted extra |
| 5148 | Tribal Leatherworking | 55/40 | Se'Jib 7871 (36.55, 34.09); pre 2860 (Feralas accept, unrouted); Leatherworking | Wild Leather Vest 8211 + Helmet 8214, crafted/sourceless (bag notes); when-skill + optional; excl 5145/5146 noted |
| 8116 | Vision of Voodress | 60/60 | Maywiki 14904 (15.3, 16.02); Shaman; Zandalar rep 3000 | no objectives; talk |
| 8117 | Vision of Voodress | 60/60 | Maywiki; pre 8116; Shaman; rep 9000 | Vision 19606 names no source (bag note) |
| 8118 | Vision of Voodress | 60/60 | Maywiki; pre 8117; Shaman; rep 21000 | Vision 19607 names no source (bag note) |
| 8119 | The Unmarred Vision of Voodress | 60/60 | Maywiki; pre 8118; Shaman; rep 42000 | Vision 19608 names no source (bag note); chain finale |
| 95141 | Report to Rog'mar | 38/36 | Aggro'gosh | talk to Krom'rosh 256418, Riverglades (59.37, 45.6, map 2548) — expedition extra turn-in; npcs.json point only, spawnz carries no entry |
| 95748 | The Gurubashi Legends of Old | 40/30 | Kin'weelay; pre 629 | Third Troll Legend rubbing 2007 off object 52 Fall of Gurubashi (22.95, 12.02) |
| 95770 | Locating the Lost City | 40/30 | Kin'weelay; pre 95748; also starts at Cauldron 2076 | find the Drowned City entrance event (22.38, 27.13, map 1434, from data) |
| 95773 | Enemies in the Water | 37/30 | Aggro'gosh + Nimboya (dual starters); pre 95748; ends Aggro'gosh | 10 Brinescale Tridents 270305 off Skirmishers 262397 (west coast 13-31, 14-34) |
| 95775 | The Drowned City | 40/30 | Kin'weelay; pre 95770 | 4 I'lalai tablets 270308-11, objects 642943-46 with no placed spawn anywhere (bag notes); turn-in Kin'weelay; next 96078 |
| 95776 | The Only Good Brinescale... | 38/30 | Aggro'gosh; pre 95770+95773 | Var'Taka 258924 has no spawn anywhere (bag-note kill — complete at Aggro'gosh, 1046-pattern) |
| 96078 | A Tale Spun Around the Fire | 40/30 | Kin'weelay; pre 95775 | no objectives; ends Master Gadrin 3188, Durotar (55.95, 74.72, map 1411) — expedition finale |
| 97386 | The Offense of Grom'gol | 44/38 | Aggro'gosh; pre 569 | Mosh'Ogg Spellcrafters 710 + Warmongers 709 + Maulers 678 + Shamans 679, Mosh'Ogg camp (46-52, 24-31); counts null in data — work the camp; finale |
| 97453 | Weed Whacked | 38/33 | Gemmil 269166 (32.77, 28.43) + Crank 2498 (27.12, 77.21) dual starters; ends Nerrist 1148 (32.7, 29.23) | 6 Carnivorous Weeds 269175, Grom'gol ring (31-37, 22-33) |

## OUT

Nothing in the Horde pool is OUT: all 39 Horde-mask records are
contracted above. The other 219 pool records are accounted for:

- 123 contracted in the Alliance `stranglethorn` guide (29
  Alliance-mask primary + 94 null shared) — NOT duplicated here by the
  exclusive-contracts precedent. Shared-mask records already in the
  Alliance contract stay out even where takeable by Horde (Ashenvale
  BORDERLINE 7 pattern).
- 96 OUT by the Alliance census's own reasons: repeatable 21 (349,
  619, 1127, 3647, 7838, 8193/8194/8221/8224/8225, 8195/8196/8238/
  8239/8243/8246, 9259, 97065/97066/97067), event 2 (8674, 8716),
  above-band 66 (9272 m49, pirates 1036/4621/83934 m55, Zandalar
  8183/8201/8240 m58, 60 x m60 turn-ins incl. Alliance-mask 8045-8048),
  broken 3 (60870, 96379, 96076), version-duplicate 4 (614
  Alliance-mask + null 615/618/620, superseded by 8551-8554).

Related outside records (ledger notes, not candidates): 1240 The Troll
Witchdoctor (Barrens accept, ends Kin'weelay in-zone) / 1262 Report to
Zor (Barrens accept, follows 1261) / 639 Sigil of Strom (Arathi accept,
follows 638) / 2842 Chief Engineer Scooty (Orgrimmar accept, routed in
orgrimmar-city.guide; turn-in at Scooty) / 2860 Master of the Wild
Leather (Feralas accept, pre of 5148, unrouted) / 3635 Gnome
Engineering (Undercity accept, routed in undercity-city.guide;
turn-in at Oglethorpe) / 3637 Gnome Engineering (Barrens accept, pre
of 3642, unrouted — preAny twin of routed 3635) / 3645 Membership Card
Renewal (Ironforge-keyed, no objectives, ender Oglethorpe — extra
after 3643, uncontracted) / 3640 Pledge of Secrecy (Ironforge) / 3647
Membership Card Renewal (Alliance repeatable, Ironforge-keyed
Booty Bay giver).

## BORDERLINE (all decided, none silent)

(a) 593 Filling the Soul Gem (repeatable-flagged): the flag is real
in the data (`repeatable: true`, `parent: 592`), but the quest is the
Yenniku chain's finale — 592's objective (Filled Soul Gem 3913) only
exists as the product of 593, so OUTing 593 would strand contracted
592. Contracted IN with the flag noted: the route plays 593 once
(accept, fill at Yenniku, turn in); repeat completions are re-farming,
not completionist content. Same class as a chain finale that happens
to be repeatable, not as a battleground/event hand-in (Ashenvale
8266/8296 pattern stays OUT).
(b) 585/586 twin variants: both Horde, both pre 584, both required by
588 (`pre: [585, 586]`). Contracted both, routed in one Skullsplitter
trip — no pick needed.
(c) Expedition chain 638: in-zone accept (Nimboya), outside ender
(Zengu, Arathi 73.8, 33.96), outside follow-up (639, Arathi accept).
Contracted 638 with the turn-in as a documented extra; 639 stays out
by the accept rule. Same shape as Stonetalon 6542/6562.
(d) Expedition chain 1261: outside pre (1240, Barrens accept,
unrouted pack-wide), in-zone accept (Cauldron), outside objective
(Jeweled Pendant, Dustwallow-only droppers) and outside ender (Nazeer,
Dustwallow 35.21, 30.66), outside follow-up (1262, Barrens accept).
Contracted 1261 with the whole outside leg documented in one
expedition; 1262 stays out by the accept rule. The Barrens-spawn
Nazeer point (53.7, 69.8) is noted, not used — the pendant and
Brackenwall both sit in Dustwallow.
(e) Expedition finale 96078: in-zone accept (Kin'weelay), outside ender
(Gadrin, Durotar 55.95, 74.72). Contracted with the turn-in as a
documented extra — Finales IN per the Ashenvale rule.
(f) Oglethorpe pair 3642/3643: in-zone accepts and turn-ins
(Oglethorpe, Booty Bay), outside pres (3635 Undercity-routed, 3637
Barrens-unrouted preAny twins) and an Ironforge-keyed extra follow-up
(3645, no objectives, same giver). Contracted both with when-skill
Engineering + optional gates; a `when onquest 3635` mini turns in the
routed pre first (3637 holders take 3642 on the same terms — noted,
not separately gated). 3645 rides as a noted extra, uncontracted.
(g) 5148 Tribal Leatherworking: in-zone accept/turn-in (Se'Jib),
outside pre (2860, Feralas accept, unrouted pack-wide), crafted
objectives with no source anywhere. Contracted with when-skill
Leatherworking + optional gates and bag notes (Galvan-chain pattern);
excl 5145/5146 are the other-specialization variants. The pre is
named, not routed — the game gates the accept.
(h) Shaman chain 8116-8119: all in-zone (Maywiki, Yojamba Isle),
minLevel 60 with Zandalar rep gates (3000/9000/21000/42000) and
`only Shaman` gates. Contracted with all gates noted (class-quest
precedent); the three Visions objectives name no source anywhere
(bag notes). Above-band by level, contracted by class-chain precedent.
(i) Sourceless-item bag notes (scan-backed, none invented): Soul Gem
3912 (593), pledge 11282 (3642), I'lalai tablets 270308-11 (95775),
Visions 19606-08 (8117-19), crafted 10559/4407/4392 (3643) and
8211/8214 (5148). All have no npc drop, no object drop, and no vendor
anywhere in the data — the guide carries explicit have-in-bags notes.
(j) 95776 Var'Taka: kill target with no spawn in npcs.json or spawnz.
Contracted with the 1046-pattern (complete at the giver Aggro'gosh +
note) — no point invented. 95770's entrance event point (22.38, 27.13)
and 2932's Hinterlands point (23.41, 58.06) come straight from the
objective data.
(k) Dual starters: 95773 (Aggro'gosh + Nimboya, ends Aggro'gosh) and
97453 (Gemmil + Crank, ends Nerrist) route at the ender-side giver
with the twin named — no accept invented.
(l) 629's shard source is npcs.json-only (objects 179426/58 at
24.77, 22.88; spawnz carries no entry) and 95141's ender is
npcs.json-only (Krom'rosh 256418 at Riverglades 59.37, 45.6; spawnz
carries no entry) — both routed with the source named. Stonetalon
6481 precedent.
(m) 2843's objective is kill-typed on its own giver (Scooty, count
null): a wait/talk beat, routed as complete + turn-in at Scooty with
the text quoted. No kill invented.

