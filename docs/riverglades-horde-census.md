# Riverglades (Horde) census (pack 0.105.0 base; Horde block)

Accept-zone key: **2548** (area 16591, parent 1415 Eastern Kingdoms).
Forever-original zone, no Classic counterpart. **178** quest records carry
zone=2548 (IDs 93786-96126, Forever-custom 93-96k space) — verified by
counting quests.json; same key the Alliance census used.

Method: every zone-2548 quest examined against the pack's inclusion rules;
the Alliance census's 66 banked Horde set-asides reconciled one by one
against the dumps; start-item/object scan run over all 66 Horde-mask
candidates; pres/exclusives resolved from data.

One ID correction against the round brief: the brief named Tan'jani quests
95151/95155, but those IDs do not exist in quests.json. The actual Horde
Tan'jani records are **95951** "Fetch 'n' Fletch and **95955** "Stick 'Em"
(Horde mask, Tan'jani giver/ender, chain-linked). The 66 below use the
data's IDs.

Race masks in the data carry faction: 8589934770 = Horde, 4294967373 =
Alliance, null = both (neutral). Classes, skill, event and repeatable are
null on all 178 records, so the mask is the only faction signal.
Exclusive-contracts precedent (Ashenvale round: zero quest overlap between
the Alliance and Horde contracts) applies: neutral quests already
contracted in the Alliance `riverglades` guide are NOT duplicated here.

## Band: 35-45

Lowest contracted minLevel is 35 (93786 A Message in Blood, the chain
opener); bulk min is 36; top min is 40 (94968 Eye of Mugg, 95033 On the
Other Side — the same two records the Alliance census names as the Horde
top-out). Levels run 36-46: the two 46s (94768 Bring Me His Head min 38,
95433 Death to the Executioner min 36) are IN per the minLevel rule, same
as the Alliance census's over-band finales. No L60 writ proves Horde-side:
all five writs (94262/94274/94286/94298/94310) are null-mask neutrals
already contracted in the Alliance guide, so no writ-class exception is
needed here.

## IN (66 — the full Horde 66, nothing ruled OUT)

### Krom'rosh command hub

| ID | Title | Lvl/min | Accept | Notes |
|----|-------|---------|--------|-------|
| 93786 | A Message in Blood | 36/35 | Krom'rosh 256418 (59.37, 45.6) | 12 Meadowsbrook Farmhands, all in-zone (east fields cluster) |
| 93787 | Food for the Taking | 36/36 | Krom'rosh | 6 Feed Satchels (262640) name no dropper and no vendor anywhere — R2 bag note |
| 93788 | Borrowed Blades | 38/36 | Kreza Darkthorn 256657 (59.92, 45.97) | 10 Woodworker's Axes off Turner's Mill Lumberjacks, in-zone |
| 93971 | Farholde Scouting Report | 45/36 | — (empty starter) | No giver in data; ender Krom'rosh. Contracted: accept at Krom'rosh with an honest note (R2 bag-note handling — an empty starter is a data fact, not a reason to drop) |
| 93976 | The Goblin Trader | 36/36 | Kreza Darkthorn | ends Friz Frazzlespark (port); next 95288 is neutral, main-guide contracted — handoff noted |
| 94480 | A Gift From Our Enemies | 36/36 | Krom'rosh | ends Gorg 256655 (58.65, 44.57); pre 93787 |
| 94481 | A Serving of Strength | 38/36 | Gorg | 8 Rog'mar Trainees, in-zone (south-east flats) |
| 94483 | Show Them How It's Done | 39/36 | Krom'rosh | 8 Farholde Priests + 12 Farholde Scouts, in-zone; pre 93786+93787; feeds the Tran'gul chain (94672+94680) |
| 94744 | The Wayward Warrior | 43/38 | Krom'rosh | ends Da'grosh 258570 (33.47, 37.93); pre 95428 |
| 94745 | Carving a Path | 44/38 | Da'grosh | Fanatics/Corrupters/Champions, in-zone west Twilight camp (Horde mirror of 94889; faction split decides, no excl in data) |
| 94748 | Break Their Chains | 44/38 | Da'grosh | 5 Rog'mar Scouts, in-zone west; pre 94744 |
| 94768 | Bring Me His Head | 46/38 | Da'grosh | Kilgar's Head off Overlord Kilgar (elite) — required chain kill with an elite note (Alliance mirror 94890 is a normal step); pre 94745+94748 |
| 94962 | Bloodmaster's Ring | 42/36 | Jezap Jinglesprocket 257062 (65.58, 21.45) | Ring line link 3 of 8 (by ID, never merged); pre 94739 |
| 94964 | Bloodmaster's Ring | 43/36 | Jezap Jinglesprocket | Ring line link 4 of 8; pre 94962 |
| 94965 | Bloodmaster's Ring | 44/36 | Jezap Jinglesprocket | Ring line link 7 of 8; pre 94737 |
| 94968 | Eye of Mugg | 45/40 | Krom'rosh | Eye of Mugg: only dropper Overlord Mugg has no spawn anywhere — 1046-pattern (complete at Krom'rosh + bag note), never an invented point; pre 95278 |
| 94972 | Tome of Twilight | 44/39 | Tran'gul 256710 (59.51, 43.96) | Tome of Twilight: only dropper Nar'gurk has no spawn anywhere — 1046-pattern (complete at Tran'gul + bag note); pre 95278 |
| 94973 | Krol'dok Moulding | 41/38 | — (empty starter) | No giver, no objectives; ender Kreza. Contracted: accept at Kreza with an honest note; feeds 94974 |
| 94974 | Key Ingredients | 41/38 | Kreza Darkthorn | 4 Thick Leather (Lhara sells off-zone; skinners' mobs are off-zone) + 12 Iron Bars (no dropper/vendor — smelted); Blacksmithing gate said honestly (STV-k precedent), bag notes |
| 94975 | A Token of Vengeance | 42/38 | Da'grosh | 15 Cultist Ears: all six droppers (Grunt, Warlock, Outrider, Lieutenant, Zarmok, Zalfan) have no spawn anywhere — 1046-pattern (complete at Da'grosh + bag note); pre 94768 |
| 95033 | On the Other Side | 41/40 | Tan'jani 263190 (58.13, 45.32) | ends Witch Doctor Uzer'i (map 1444 [74.42, 43.36]) — a documented expedition turn-in via `zone map 1444`, the same expedition map the main guide already uses for its Tanaris leg |
| 95062 | Frazzlespark's Crate | 36/36 | Friz Frazzlespark 255897 (77.1, 52.9) | Horde mirror of 95059 (faction split decides); ends Krom'rosh |
| 95063 | Bloodmaster's Ring | 45/36 | Jezap Jinglesprocket | Ring line link 8 of 8; ends Clugfist 255829 (64.25, 15.72); pre 94965 |
| 95278 | It Is Time, Brother... | 45/38 | Da'grosh | ends Krom'rosh; pre 94768; feeds 94968+94972 |
| 95428 | Clugfist's Decree | 41/36 | Clugfist | ends Krom'rosh; pre 95424+95425; feeds 94744 and (via 95424/95425) the Jezap ring line |

### Tran'gul Twilight chain

| ID | Title | Lvl/min | Accept | Notes |
|----|-------|---------|--------|-------|
| 94672 | Encroaching Twilight | 41/36 | Tran'gul | Raiders/Shadowmancers/Neophytes, in-zone west camp; pre 94483 |
| 94680 | Twilight Missives | 41/36 | Tran'gul | 3 Twilight Missives off Shadowmancers, in-zone; pre 94483 |
| 94727 | Digging for Answers | 40/36 | Tran'gul | ends Clubtoe 260931 (49.95, 46.99); pre 94672+94680 |
| 95417 | The Purple Ones | 40/36 | Clubtoe | ends Twilight Brute 261208 (49.18, 46.74); pre 94727 |
| 95418 | Spread the Word | 40/36 | Clubtoe | ends Tran'gul; pre 95427; feeds 95420 |
| 95420 | Land of Giants | 40/36 | Tran'gul | ends Clugfist; pre 95418; feeds 95424+95425 |
| 95424 | Might Makes Right | 41/36 | Clugfist | 7 Twilight Maulers + 7 Firecallers, in-zone north-east; pre 95420 |
| 95425 | Unworthy Champion | 42/36 | Clugfist | Skullbasher off Klunk (in-zone, not elite); pre 95420 |
| 95427 | Twilight No More! | 41/36 | Clubtoe | Chogg's + Zac's Heads off Chogg'Zac (elite) — optional + tip (Alliance mirror 95562 marks the same); pre 95601+95602 |
| 95431 | Rumblings of Discontent | 41/38 | Da'grosh | ends Crag'rog 260993 (27.66, 36.54); pre 94744 |
| 95432 | Rise Up! | 43/36 | Crag'rog | pre 95431 |
| 95433 | Death to the Executioner | 46/36 | Crag'rog | Executioner's Mace off Executioner Morg (elite) — required chain kill with an elite note; ends Clugfist; pre 95432 |
| 95601 | The Purple Ones | 40/36 | Twilight Brute | 5 Empowered Brutes + 10 Ritualists, in-zone (Horde mirror of 95643; faction split decides); pre 95417 |
| 95602 | Sickening Lights | 40/36 | Clubtoe | pre 94727; feeds 95427 |

### Neza Bloodsnout gnoll chain

| ID | Title | Lvl/min | Accept | Notes |
|----|-------|---------|--------|-------|
| 94532 | Gnoll Infestation | 38/36 | Neza Bloodsnout 258031 (60.46, 47.86) | Mystics/Trappers/Brutes, in-zone north (Horde twin of 94678 — no excl flags in the data either way; chain-consistency picks the Horde twin: ours chains from 96109 while 94678 stands alone); pre 96109 |
| 94533 | Snargl's Snout | 40/36 | Neza Bloodsnout | Snargl's Snout off Snargl (elite) — required step with an elite note (Alliance mirror 94679 is a normal step); dual-map Redridge/Riverglades, guide uses the 2548 points; pre 96109 |
| 94535 | Bristle Hills Bandits | 38/36 | Kreza Darkthorn | 40 Stolen Ore off the same north gnolls — fills with 94532; pre 96109 |
| 96103 | A Feast for Buzzards | 38/36 | Picked Carcass 263316 (61.64, 58.81) | ends Neza Bloodsnout; feeds 96104 |
| 96104 | Song of the Strider | 39/36 | Neza Bloodsnout | Intact Tallstrider Beak off Roving Tallstriders, in-zone; pre 96103 |
| 96105 | King of the Wild Plains | 41/36 | Neza Bloodsnout | Ombassa's Hide off Ombassa (elite) — optional + tip (Alliance mirror 95986 marks the same); pre 96104 |
| 96107 | Feathers for Fletching | 40/36 | Neza Bloodsnout | 6 Plains Buzzard Feathers, in-zone; feeds 96108 |
| 96108 | Poison Tips | 40/36 | Neza Bloodsnout | 4 Glade Viper Venom, in-zone; pre 96107 |
| 96109 | A Hunter's Quiver | 40/36 | Neza Bloodsnout | 6 Prized Lion Hides off Patriarchs/Huntresses, in-zone; pre 96108; feeds 94532+94533+94535 |

### Na'zok / Tan'jani / misc Horde

| ID | Title | Lvl/min | Accept | Notes |
|----|-------|---------|--------|-------|
| 95162 | Paletusk Harvesting | 41/38 | Na'zok 256728 (70.73, 28.09) | 10 Chunk of Boar Meat: no 2548 dropper (all droppers on classic maps) — bag note + complete at Na'zok |
| 95163 | Drive Them Back | 40/38 | Na'zok | 10 Young Paletusk, in-zone east; no pre (stands with 95162) |
| 95951 | Fetch 'n' Fletch | 38/36 | Tan'jani 263190 (58.13, 45.32) | 20 Makeshift Stickin' Spears: no dropper/vendor anywhere — bag note + complete at Tan'jani; feeds 95955 |
| 95955 | Stick 'Em | 39/36 | Tan'jani | 10 Freshwater Crocolisks, in-zone; pre 95951 |
| 95181 | Twilight Scouting Report | 42/36 | — (empty starter AND ender) | No giver, no ender, no objectives. Contracted as an accept-only record with an honest note (94963-pattern) — an empty starter/ender is a data fact to document, not a reason to drop |
| 95183 | Step One: Rock | 41/38 | Gorgegut 259988 (69.64, 25.92) + Hamur 263440 (67.24, 21.75) | dual start, single ender (Hamur); 10 Good Rocks name no dropper/vendor — bag note; feeds 96026 |
| 96026 | Step Two: More Rock | 41/38 | Hamur | 10 Heavy Weightstones: no dropper (crafted) — Blacksmithing gate said honestly (STV-k precedent) + bag note; pre 95183 |
| 95882 | WANTED: Scoutmaster Vargas | 43/38 | — (object-start) | WANTED poster 707249 at (59.6, 46.99); Scoutmaster's Eye off Scoutmaster Vargas (elite) — optional + tip; ends Neza Bloodsnout |
| 95936 | Hail the Dragonslayer | 43/36 | — (empty starter) | No giver in data; ender Krom'rosh — accept at Krom'rosh with an honest note (95935-pattern). Head of Scaldaron off Scaldaron (rare elite) — optional + tip (Alliance mirror 95935 marks the same) |
| 95992 | WANTED: Ghostmaw | 42/38 | — (object-start) | WANTED poster 645164 at (59.46, 47.02); Ghostmaw's Fang off Ghostmaw (elite) — optional + tip (Alliance mirror 95991 marks the same); ends Tan'jani |
| 94733 | Our Ogre Friend | 41/36 | Jezap Jinglesprocket | ends Gobam 257058 (67, 17.18); pre 94964; ring-line bridge (links 4→5) |
| 94734 | A Boar's Delight | 41/36 | Gobam | 8 Sweetberries + 12 Riverweed: neither names any dropper/vendor anywhere — bag notes + complete at Gobam; pre 94733 |
| 94737 | A Treat for a Friend | 41/36 | Gobam | ends Jezap Jinglesprocket; pre 94734; feeds 94965 |
| 94739 | Bloodmaster's Ring | 42/36 | Jezap Jinglesprocket | Ring line link 2 of 8; pre 94670; full ring order: 94668 → 94669 Pay to Play → 94670 → 94739 → 94962 → 94964 → 94733 → 94734 → 94737 → 94965 → 95063 |
| 94556 | Jom-jom's Escape | 42/36 | Jom-jom 258048 (73.37, 24.74) | ends Clugfist; standalone (no pre/next links in data) |
| 94668 | Bloodmaster's Ring | 41/36 | Clugfist | Ring line link 1 of 8; ends Jezap; pre 95424+95425; feeds 94669 |
| 94669 | Pay to Play | 41/36 | Jezap Jinglesprocket | Ring-line bridge (titled, not a "Bloodmaster's Ring" line — counted with the 8); pre 94668 |
| 94670 | Bloodmaster's Ring | 41/36 | Jezap Jinglesprocket | Ring line link with 94739 (pre 94669, next 94739) |

"Bloodmaster's Ring" names eight records by ID (94962, 94964, 94965, 95063,
94739, 94668, 94670 — seven titled lines — plus the titled bridge 94669
Pay to Play): disambiguated strictly by ID above and routed as one
eleven-link chain; never merged, never dropped for sharing a name.

Item/object-start scan over all 66: exactly the two object-starts above
(95882, 95992); zero item-starts — "no others" is claimed only after this
scan. No objective-object refs anywhere in the 66, so no phantom objects
on the Horde side (the Alliance census's ~17 phantom refs are Alliance-side).

Spawn audit: every giver, ender and kill target referenced by the 66
spawns on map 2548 except Uzer'i (map 1444, the documented expedition).
No spawnless NPC is referenced directly; the spawnless records are
*sources*: Overlord Mugg (94968), Nar'gurk (94972), and the six Cultist
Ear mobs (94975) get NO invented coordinates — 1046-pattern completes at
the giver with bag notes. Tunk is not referenced by any Horde record.

## OUT

Of the Horde 66: none. Every record routes (above-band: none; broken:
none; repeatable/seasonal/placeholder: none; excl: none in data).

Not duplicated here (Ashenvale exclusive-contracts precedent — already
contracted in the Alliance `riverglades` guide): the 29 null-mask
neutrals (94262, 94274, 94286, 94298, 94310, 94961, 94963, 95118, 95119,
95120, 95121, 95122, 95123, 95124, 95165, 95254, 95260, 95261, 95267,
95288, 95293, 95294, 95295, 95296, 95792, 95934, 95982, 96063, 96067).

Alliance-only zone-2548 quests (set aside for the record): the 83
races-4294967373 records (the Alliance census's IN 112 minus the 29
neutral above).

Candidates examined: 178 zone-2548 records. IN (Horde contract) 66, OUT 0,
not-duplicated neutral 29, Alliance-only 83.

## BORDERLINE (carried honest versions)

Summarised inline in the tables above; the load-bearing calls: empty
starters 93971/94973 accept at their ender with a note; 95181's empty
starter AND ender contracts accept-only; spawnless-sourced 94968/94972/
94975 complete at the giver with bag notes; sourceless-item 93787/94734/
95162/95951/95183 and crafted-gate 94974/96026 carry bag notes and honest
profession gates; expedition 95033 rides `zone map 1444`; the 8-line Ring
disambiguation is by ID; twins 94532/94533 chain-consistency over the
Alliance mirrors (no excl flags in the data either way).

## Faction-ungating ruling (zone-specific judgment call)

The Alliance census recorded null classes/skill/event/repeatable across
the zone — verified true for all 178 — but faction does NOT come from a
null field: the records' `races` mask is the faction data (8589934770 =
Horde, 4294967373 = Alliance, null = both), and the split on this key is
83/66/29 by that mask. Ruling: the 83 Alliance-mask quests are NOT
acceptable by Horde players, so dropping the `faction Alliance` header
alone would strand Horde players on dead steps. The ungate therefore gates
every Alliance-mask quest line `only Alliance` (composing with existing
gates; soft-pre `when onquest` minis and any travel lines by the same
rule) and drops the header. Verified by the dead-line check from both
factions and the travel-line search (see the ungating report); the
Alliance contract's accepts/turn-ins are unchanged.
