# Ashenvale census (pack 0.20.0)

Accept-zone key: **1440** (Kalimdor space: Teldrassil 1438, Darkshore
1439). All 112 quests carrying `zone=1440` were pulled. This is a contested
zone: the census keys on Alliance accepts only (races 4294967373 or null,
plus one Human+Dwarf line). Horde-accept quests are counted and listed as
their own OUT class for the Horde block's census to reconcile against.

Band derivation: in-contract quest levels run 18 (Journey to Stonetalon
Peak 1056) to 32 (Insane Druids 1012, Vile Satyr 1021, Branch of Cenarius
1031, Satyr Slaying 1032); in-contract minLevels run 13–27. Header band
**levels 18–32**. The L31–32 quests are in-band by minLevel (24–26). Two
L47 records (5535/5536, minLevel 45) run above the band and are OUT.

No race header for the guide: no quest is race-locked to a single Alliance
race (78093 covers Human+Dwarf Paladins via one per-line gate). Class gates:
Warrior (78132/78133/78134), Paladin (78089, 78093). No profession quests
(no skill-gated records). No dungeon quests: every Alliance kill objective
resolves to an in-zone spawn (Blackfathom Deeps has no Alliance accept
touching it — its quests accept elsewhere or not at all in this data).

Tower chain: the Darkshore census contracted the Tower chain's ends (981,
1143, both Balthule in Darkshore) and set aside the middle links as
Ashenvale-side. All four accept at Delgren the Purifier in Ashenvale and
are contracted here: 970 (Glowing Soul Gem, pre 967 Darkshore-contracted),
973 (Ilkrud's Tome), 976 (escort Feero Ironhand), 1140 (free the two
Highborne souls), 1167 (turn-in to Balthule in Darkshore — expedition).
The chain reads whole across the two guides.

## BORDERLINE (all decided, none silent)

1. PvP hand-ins (15) OUT as repeatables: 7788/7871/7872/7873 Vanquish the
Invaders tiers, 7863/7864/7865 Sentinel Care Packages, 7886/7887/7888/7921/
8289/8292 Talismans of Merit tiers, 8269 Ribbons of Sacrifice, 8291
Vanquish L60. All turn Warsong marks/talismans earned repeatedly in Warsong
Gulch; the excl structure is tier-exclusion, not variant-exclusion. Same
class as the mount-exchange and cloth turn-in outs.
2. 5535 Spiritual Unrest + 5536 A Land Filled with Hatred (L47/m45,
Loh'atu, dual 1440/1447) OUT above band. Even on the Ashenvale point the
minLevel rule excludes them.
3. 8725 Riversong the Elder (L60/m1, event=7) OUT seasonal/event: a Lunar
Festival elder.
4. Craftsman's Writs (94222/94231/94240/94249, L60/m1, sourceless
item-starts, ends at the Cowardly Peon/Grembly/Murache) IN by the
item-start rule (Redridge 95816/98247 precedent) with bag notes — accepted
here, turn in east/south-east. No repeat or event markers in the data.
5. 78132/78133 Dragonslayer Helm + Shield (L25/m15, Warrior, sourceless
objectives) IN with bag notes + complete at Alonso; 78134 Lance IN with a
Wetlands vendor buy (3180 Dark Iron Entrepreneur) + complete at Alonso.
6. 79090 Repelling Invaders (L60/m18, item-start 211814 dropping from six
in-zone Warsong mobs, end Felore Moonray) IN: optional kill for the mark,
accept, turn in at Felore's Astranaar point (judgment call — both Felore
records are the NPC's own points; the hub chosen).
7. 1017 Mage Summoner (Sarilus Foulborne's Head drops ONLY in the Barrens)
— out-of-zone objective: complete at Sarilus's Barrens point in a dedicated
mini expedition leg, turn in at Velene in Ashenvale.
8. 1134 Pridewings of Stonetalon (Venom Sacs drop ONLY in Stonetalon) —
out-of-zone objective: complete in the Stonetalon expedition leg that
already carries the 1056/1070 turn-ins, turn in at Shindrell in Ashenvale.
9. 78093 Return to Delgren (Human+Dwarf Paladin, object-start Shattered
Orb far east) IN with gate `only Human,Dwarf,Paladin`.
10. Sourceless objectives with honest bag notes (complete at the giver, no
invented collects): 5464/5519 Iron Shaft/Pommel (1026/1027), 5462 Dartol's
Rod (1046, complete at Raene), 5440 Bottle of Disease (1011), 5493 Elune's
Tear (1033), 5494 Stardust x5 (1034), 5424 Ancient Statuette (1007), 5437
Bathran's Hair (1010), 5455 Divined Scroll (1016), 281014 Vine-Wrapped
Scroll (98417), 209872/209873 Helm/Shield (78132/78133), writs (above).
11. 1081 Reception from Tyrande (pre 1082 Update for Sentinel Thenysil,
uncontracted in Stonetalon) — structural note; turn in at Tyrande's
Darnassus point (DA-verified). 78089 Advice From Stormwind (pre 78088 A
Strange Artifact, uncontracted in Darkshore) — structural note; turn in at
Katherine the Pure in Stormwind.
12. 1037 Velinde Starsong (pre 1022 in-contract; end Thyn'tel dual
1438/1457) IN; turn in at Thyn'tel's Darnassus point (DA-verified for
1038's turn-in).

## IN (55)

Tower: 970 (pre 967 Darkshore — structural note; gem @Dark Strand),
973, 976 (escort Feero), 1140 (souls @circles), 1167 (turnin Balthule
Darkshore — expedition). Astranaar hub: 991 → 1023 (gem @Saltspittle) →
1024/1025 → 1026 → 1027 → 1028 (turnin shrine object) → 1055 (accept
shrine) → 1029 → 1030 → 1045 (Bloodtooth @guards + Ran's Skull) → 1046
(Dartol's Rod, bag note). West: 1007 (statuette, bag note) → 1009 (Ring
@Ruuzel); 1008 (Wrathtail x20) → 1134 (sacs Stonetalon — expedition
complete); 1010 (hair, bag note) → 1020 → 1033 (tear, bag note) → 1034
(stardust, bag note) → 1035 (moonstone @Shadethicket Oracle); 1016 (scroll,
bag note) → 1017 (head Barrens — expedition complete); 1021 → 1031 (branch
@Geltharis) → 1032 (horns @Xavian); 1022 (tome object) → 1037 (end
Thyn'tel outside). North/east: 1011 (bottle, bag note; pre 4581) → 1012
(kills Taneel/Uthil/Mavoris); 1054 (Dal's Skull); 1025 (Foulweald kills);
98417 (scroll, bag note; pre none) → 98418 (Xavian kills); 1056 (end
Albagorm Stonetalon — expedition); 1070 (end Kaela Stonetalon —
expedition); 1081 (pre 1082 uncontracted — structural note; end Tyrande
outside); 98027 (pendant object → Maliynn); 95737 (end Caitlin Wetlands —
expedition); 86757 (swords/daggers @Horde mobs SE); 4581 (Kayneth, no
obj); 78089 (Paladin; pre 78088 uncontracted — structural note; end
Katherine SW — expedition); 78093 (Human+Dwarf Paladin, orb object);
78132/78133/78134 (Warrior; bag/bag/buy); 79090 (mark sourcing + Felore).

## OUT (57)

- Horde set-aside (39, for the Horde block's census): 2, 3, 4, 23, 24, 25,
216, 247, 824, 909 (all-Horde-races mask), 1918, 3513, 3514, 6383, 6441,
6442, 6462, 6482, 6503, 6504, 6543, 6544, 6545, 6546, 6547, 6563, 6564,
6565, 6571, 6581, 6621, 6641, 6921, 6922, 8266, 8296, 79098, 94213, 95042,
98251, 98252. Includes the whole Horde Je'neu chain, the Kadrak/Warsong
chain, the Karang/Thistlefur line, the Senani hunt chain, and Horde
Battleground hand-ins.
- Repeatable PvP hand-ins (15): 7788, 7863, 7864, 7865, 7871, 7872, 7873,
7886, 7887, 7888, 7921, 8269, 8289, 8291, 8292.
- Above band (2): 5535, 5536.
- Seasonal/event (1): 8725.
