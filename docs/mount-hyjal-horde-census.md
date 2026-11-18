# Mount Hyjal (Horde) census (game data, accept-zone key 2482)

Accept-zone key: **2482** (verified: the simulator map table labels 2482
Mount Hyjal; the Alliance census counted 137 start-based candidates on the
key; the zone-field enumeration in this build holds 142 quest records on
2482 - 16 Horde-mask, 21 Alliance-mask, 105 shared/null. The candidate
definitions differ slightly (start-based vs zone-field); every Horde-mask
record on the key was examined, so nothing Horde hides in the gap).

Race masks: 8589934770 = Horde, 4294967373 = Alliance, null = shared.
Method as established: every Horde-mask 2482 record ruled; the Alliance
census's 13 banked Horde set-asides reconciled one by one; start-item AND
start-object scan run; pres/exclusives resolved from data.

## Band: 54-60

Contracted minLevels run 54 (eleven records) through 57 (92592 Final
Death), with 96830 Farsight Guided minLevel-null riding along per the
B1 precedent (its own level 57 fits the zone). Top contracted quest level
is 60 (92446 Head Scratcher). Derived from the Horde records - the floor
rests on eleven 54s, not one outlier.

No race header beyond faction: all 13 contracted quests are Horde-mask,
none race-locked further. No class gates, no profession gates (CLASS and
SKILL are null on all 13).

## IN (13)

Western post hub - Zet'gan (244511 @13.82,54.75), Kal'tinzan (265788
@13.77,53.06), Ortak Lomgok (244512 @12.93,52.85). Eight of the 13 live
here:

| 91794 Flags of Our Forebears | 59/54 | no pre | 1 Horde Flag (object-source 577731 has NO placed spawn anywhere - the flag rides the in-zone demon crews with the heraldry below) + 3 Scrap of Horde Heraldry off Felguard Sentinels (~43-54,29-46), Doomguards (~49-53,31-39), Mazzogore (5 pts ~50-52,36-42), Bethra'zel (~58,32), Doomguard Xarkul (~58-61,29-35); Jezerelle the Swaying has NO spawn anywhere - named, never routed | accept + turnin Kal'tinzan |
| 92592 Final Death | 59/57 | no pre | 1 Reanimator's Amulet off Scourge Reanimators (8 pts ~22-27,47-58, in-zone west) | Zet'gan to Zet'gan |
| 92609 Feathers in Flight | 57/54 | no pre | 9 Hyjal Owl Feather off Hyjal Owls (western points ~19-32,61-82; the object-source 577746 has NO placed spawn - the owls carry the hunt) | Zet'gan to Zet'gan |
| 95026 Blight No More | 58/54 | no pre (chain head) | 3 Forgotten Soldier + 12 Fleshflay Ravener, both families dense in-zone west (~18-28,46-64) | Zet'gan to Zet'gan. Discharges the Alliance borderline B2: kept out of the main contract as the Horde twin pre, homed here on its own record |
| 92446 Head Scratcher | 60/54 | pre 92609 (in-contract, routed above) | Head Scratcher's Scratchers off Head Scratchers (4 pts ~33-36,71-73) | Zet'gan to Zet'gan |
| 96616 Herbs for the Bruised and Weary | 57/54 | no pre | 12 Hyjal Silphium: SOLE source is object 654624 with NO placed spawn anywhere (no spawnz entry) - sourceless in the data; bag note at accept, no complete (Bear Berries precedent) | Ortak to Ortak |
| 96622 A Rest Without Pain | 57/54 | pre 96616 (in-contract) | no objectives (talk) | Ortak to Ortak |
| 97119 Now We're Cooking | 57/54 | no pre | 6 Savory Stag Sliders: NO source anywhere in the data (no droppers, no vendors, no recipe) - sourceless; bag note at accept, no complete. The Alliance-side 92433 (races-null shared, main-contracted) is untouched - different quest ID, no duplication | Ortak to Ortak |

Elder-grove leg - Curious Crow (257753 @48.26,85.72):

| 94782 The Western Post | 57/54 | pre 95316 (shared, MAIN-contracted - chain note, no mini: the ungated main guide serves 95316 to both factions; the 8996 pattern) | no objectives (talk) | accept Crow, turn in Zet'gan (next 95248, in-contract) |

Summit finale - Thisalee Crow (254915 @68.99,49.99):

| 95248 To the Summit of Eternity | 59/54 | pres 92592+92609+94782+95026 (ALL in-contract, routed above - no minis) | no objectives (talk) | accept Zet'gan, turn in Thisalee. The Horde side of the split chain; Alliance 91688 stays in the main guide untouched |

Far east + Troll Remains chain:

| 96830 Farsight Guided | 57/minnull (rides B1) | no pre | no objectives (talk) | accept Thark Gorax (266802 @79.94,70.69, far east single point), turn in Ortak (west) - a cross-zone walk inside the frame |
| 96998 Tribal Colors | 58/54 | no pre | no objectives; OBJECT-START off Troll Remains 656786 (@61.54,41.47 on 2482 - the pool scan's only object-start) | accept the Remains, turn in Zet'gan (next 96999, in-contract) |
| 96999 Wrap Return | 58/54 | pre 96998 (in-contract) | no objectives (talk) | accept Zet'gan, turn in Tai'tasi (3187) in Durotar (@56.41,73.79 on 1411) - Durotar expedition turn-in |

## OUT (3 of the pool; noted non-contracted)

- 97001 Sawyer's Legacy (57/54), 97006 Notarized Claim (60/54), 97007 Wood Remains (57/54): all three Horde-mask on 2482 but with EMPTY start AND end records (no npc/object/item anywhere) - broken/incomplete, the 93925 class. Logged for the data build; contract if records ever fill in.
- The main guide's documented non-contract soft-pre turn-ins (92009 Winterspring, 93773 Moonglade) belong to the main guide: no contracted Horde chain turns in through them (stated, not duplicated).
- 94832/96077 Belle's Ring: verified both Alliance-only (4294967373) - adjacency only, never Horde pool. The accept-only 96077 stays the main guide's documented record.

## Item-start enumeration

Explicit start-item AND start-object scan over the 16-record Horde pool: exactly ONE object-start (96998 off Troll Remains, IN and routed above); ZERO item-starts. Both sourceless-objective cases (Silphium, Sliders) are objective items, not starter items - bag notes, never invents.

## BORDERLINE (all decided, none silent)

(a) 95026 (named check 2): the Alliance B2 kept it out as a twin pre. Its own record anchors fully on 2482 (accept + turn in Zet'gan, kills in-zone west) with pre [] - a chain head, not a dangling pre. B2 discharged by homing: IN.
(b) Band top on one record: only 92446 reaches quest level 60 (min 54, in band by the minLevel rule). The band floor rests on eleven 54s; the top is honest, not stretched.
(c) 92433 vs 97119 (named check 1, Cooking split): 92433 is races-NULL (shared) and main-contracted; 97119 is Horde-only. Different IDs, zero overlap - each side rides its own contract. No duplication, no conflict.
(d) 94782's pre 95316 served by the ungated main guide: 95316 is races-null shared and main-contracted, so the chain note (not a mini) is the honest shape - a Horde player CAN see it post-ungating. If a future pass re-homes 95316, this note gets a pointer update.
(e) 96999's Durotar turn-in: the accept keeps it a Hyjal quest per the accept rule (B11 precedent - the TN/Redridge tails); the 1411 leg is an R1 expedition by design.
(f) 96830's minnull: own level 57, fits the zone; rides the B1 reading. If the data build ever fills minLevel above band, the census recomputes.
(g) Zero soft-pre minis in this guide: every blocking pre is either in-contract (92609, 96616, 96998, the four summit pres) or main-contracted shared (95316, chain note). First Horde micro-guide with no minis - stated, not missing.
