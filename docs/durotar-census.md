# Durotar Census

Accept-zone key: **1411** (local QuestieDB data, `--product wowf`). Proof:
272 NPCs and 237 objects spawn on 1411; 148 quest records carry zone=1411,
and every one of them accepts from an NPC/object spawning on 1411. No
side-bucket. (Orgrimmar is key 1454 and is NOT censused here — dual-spawn
NPCs follow the city rule's test: the quest belongs where its accept is
routed, and endgame hand-ins from dual-spawn NPCs go to the future Orgrimmar
census.)

Race-mask key used below: `8589934770` = Horde, `4294967373` = Alliance,
`130` = Orc+Troll, `146` = Orc+Undead+Troll, `162` = Orc+Tauren+Troll,
`2` = Orc, `16` = Undead, `32` = Tauren, `128` = Troll, `null` = open.
Classes: 1 Warrior, 4 Hunter, 8 Rogue, 16 Priest, 64 Shaman, 128 Mage,
256 Warlock. Bit 33 (`8589934592`) is the pack's Horde-faction flag
(Zephras 92598 precedent: gated `only Horde`).

## Band

Lowest contracted minLevel **1** to highest contracted quest level **13**
(1526/1527 Call of Fire, Shaman, min10) = **1-13**. `minnull` treated as
no-minimum (B1 precedent). The lvl-12/13 quests with min4-10 (806, 827-829,
840, 1464-shape 1525-1527) are IN by the zone-finale rule's letter (minLevel
in band); everything with minLevel above 13 is OUT.

## IN ledger (106)

Valley of Trials / Sen'jin / Razor Hill core: 784, 786 (pre 785 is a broken
stub, see BORDERLINE), 788 (pres 787 Orgrimmar + 4641), 789, 790, 791, 792
(classes 1247: all but Warlock — Warlocks have 1485/1499; routed ungated, the
NPC simply doesn't offer it to Warlocks, no wedge), 794 (pre 792+1499), 804
(pre 790), 805 (pre 794), 806 (pre 823), 808, 812, 815, 816, 817, 818, 823,
825 (pre 784), 826, 827 (pre 828), 828 (pre 806), 829 (pre 827, ends Orgrimmar
Neeru — expedition), 830 (item-start: Aged Envelope from Benedict's Chest
3239 on 1411 at 59.26,57.65), 831 (pre 830, ends Orgrimmar Nazgrel —
expedition), 834, 835 (pre 834; both neutral Rezlak), 837, 840 (ends Barrens
Kargal — expedition), 2161, 4402 (pre 788), 4641, 5441, 6394 (pre 5441),
9263 (event objective on 1411), 97279 (ends dual-spawn Kzan), 97281
(item-start: Dull Storm Orb from Dustwind mobs on 1411), 97282 (pre 97281),
96821, 96822, 96825, 96873, 96876 (item-start: Ukor's Lost Pack from
Ukorsbane on 1411), 97223, 97225 (pre 805), 99048, 99049 (pre 99048),
99051 (pre 99049), 99052 (pre 99051), 99123 (escort event), 5843 (item-start:
Valley of Trials Gift Voucher has NO source anywhere — R2 bag note).

Class quests (gated per line): Shaman 1463 (rep=true, see BORDERLINE),
1516, 1517 (pre 1516), 1518 (pre 1517), 1525 (pre 1524 Barrens — soft-pre),
1526 (pre 1525), 1527 (pre 1526, Brazier object-accept), 2983 (races 162,
ends Barrens Kranal — expedition), 98517 (bit33 → only Shaman,Horde per
Zephras precedent; ends 252382); Warrior 1505 (Tarshaw on 1411; ends Barrens
Uzzek — expedition; Mulgore reconciliation note), 2383 Orc (pre 788), 3065
Troll (pre 788); Hunter 3082 Troll (pre 788), 3087 Orc (pre 788), 6062
(races 130), 6069 (races 130), 6083 (pre 6062), 6082 (pre 6083), 6081 (pre
6082, ends Orgrimmar Ormak — expedition), 6067 (races 32 Tauren, ends Mulgore
Yaw — expedition); Rogue 1859 Orc (ends Orgrimmar Therzok — expedition),
3083 Troll (pre 788), 3088 Orc (pre 788); Priest 3085 Troll (pre 788),
5648/5649 Troll (pre chain), 5652/5654 Hex twins (Ur'kyo/Tai'jin), 5660/5662
Touch twins (Undead; end Tirisfal/UC Aelthalyste — expedition); Mage 1883
(Uthel'nay on 1411; Mulgore reconciliation note), 1884 (races 146), 3086
Troll (pre 788), 98576 Orc (pre 788); Warlock 1485, 1499 (pre 1485),
3090 Orc (pre 788), 98575 Troll (pre 788), 1506 (ends Orgrimmar Gan'rul —
expedition).

Profession quests (optional + `when skill` gated, settled handling): 96102,
96604 (pre 96652), 96652 (object-start Lost Journal on 1411, pre 794),
96655, 97899, 97900, 97901, 97902, 97903, 97904, 97905, 97906, 97907, 97908.
Their pres list six other zones' Great Outdoors variants (95998 Elwynn,
96101 Zephras, 96605 Mulgore, 96606 Teldrassil, 96607 Tirisfal, 96608
Dun Morogh) — only Durotar's own 96604 is the operative pre; the rest are
other zones' equivalents, noted not routed (see BORDERLINE).

## OUT

- Above-band (minLevel above 13): 235 (20), 1018 (55), 1944/1945 (26),
  1947 (38), 1953 (40), 1959 (15), 2380 (16), 2861 (46), 2936/2937 (40),
  2985 (20), 5646/5680 (20), 6623 (45), 7068 (42), 7492 (57), 7493 (60),
  8150 (60), 8250/8254 (50), 96989/97200 (40), 1842/1843 (30). 2985, 1944,
  1945, 1953, 1959, 2380, 2985 are class quests above band — OUT all the same.
- Already contracted elsewhere: 1464 Fire Sapta (Barrens), 1521 Call of
  Earth (Barrens — Durotar's chain 1516→1517→1518 turns in cleanly and hands
  off with a note; no wedge).
- Alliance-only set-asides (for the record): 8827, 8860 (seasonal), 94375,
  94468 (Shaman totem variants).
- Seasonal/event: 8828, 8861 (Winter Veil / New Year), 8358 (rep, pre 8312
  Hallow's End chain, kill-credit on a trainer), 8670 (Lunar elder).
- Repeatables: 7664/7665 (mount replacement, min60), 7837 (Additional
  Runecloth, rep).
- Endgame hand-ins (see BORDERLINE): 7833/7834/7835/7836 (lvl60 cloth
  donations, min12-50; flagged for the future Orgrimmar census — Vehena
  dual-spawns 1411/1454).
- Broken/incomplete: 785 (zone=null, no accept, no end — datamined stub; pre
  of 786, see BORDERLINE).

## BORDERLINE

1. 1463 Earth Sapta (rep=true) IN: 51 quests across existing contracts carry
   repeatable=true (incl. class quests and mount exchanges in Elwynn), so the
   flag is not exclusionary in this pack; 1463 accepts only in Durotar and
   would otherwise be guideless. Decided: IN. (1464 excluded ONLY because the
   Barrens already contracts it.)
2. 1521 OUT (already in Barrens): double-contracting one quest in two guides
   breaks the pack's one-quest-one-guide shape; Durotar's 1518 turns in at
   Canaga with nothing pending, so the handoff note leaves no wedge.
3. 786 IN with broken pre 785: 786's accept/end/objectives are fully placed
   on 1411; its pre is a stub that can never complete, so no soft-pre mini is
   possible — the structural warning stands as accepted residue. Decided: IN.
4. 7833-7836 OUT: level-60 endgame donations whose minLevels (12/26/40/50)
   are unlock floors, not level indicators — 47 levels above the band top is
   not a "finale". Vehena dual-spawns in Orgrimmar, so the future all-levels
   Orgrimmar census takes them. Decided: OUT, flagged for Orgrimmar.
5. 1505/1883 IN with Mulgore reconciliation: both genuinely accept on 1411
   (Tarshaw/Uthel'nay); contracted here; the future Mulgore census must
   reference, not duplicate, them.
6. Camping pres: only 96604 operative; the six other-zone variants are
   equivalents for their zones' players, listed in the pres by data design.
   Decided: IN all 12 camping quests (optional+gated); variants noted.
7. 788's pre 787 (Orgrimmar accept, Gornek turn-in) → `when onquest 787`
   mini carrying turnin 787 (documented non-contract, Winterspring
   precedent). 1525's pre 1524 (Barrens-contracted, turn-in at Telf Joolam's
   dual 1411/1413 spawn) → `when onquest 1524` mini carrying turnin 1524
   (documented non-contract).
8. Band 1-13: lowest contracted minLevel 1 → highest contracted quest level
   13 (1526/1527). The 12s ride as finales by minLevel (all min4-10).
9. 792 ungated (classes 1247 = all but Warlock; no exclusion syntax in the
   dialect; the NPC doesn't offer it to Warlocks so the line never wedges).
10. No `[PH]`, no dungeon-objective quests, no same-name-variant disputes
    beyond the routed twins (830/831, 5652/5654, 5660/5662 — both, Harvesting
    precedent).
