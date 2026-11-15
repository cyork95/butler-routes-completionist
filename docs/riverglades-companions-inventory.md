# Riverglades companions inventory (game data, accept-zone key 2548)

Source: local Forever game data (questie-forever NPC/object/item dumps).
Riverglades is a Forever-original zone: every NPC, object and vendor below
exists only in this data (high IDs, questie-forever source), and the census
data is the only authority. Rank semantics calibrated in earlier rounds:
rank 4 = Rare, rank 2 = Rare Elite. (Note: all 7 flagged Riverglades NPCs
carry rank 2/4 but EMPTY roles arrays — the sweep keys on rank, verified
against the Tanaris/Stranglethorn/Badlands lists where rank and roles
agree.) Loot "sole dropper" means the item's drops.npc lists only this NPC
and no object source. Rates shown where the data gives a number; null rates
do not disqualify a sole drop (Feralas/Tanaris calibration). Tameability has
NO data flag anywhere: a tame line ships only on drop evidence PLUS
core-guide corroboration, else it is logged in docs/companion-unverified.md.

## RARES — 7 flagged (4 Rare + 3 Rare Elite), 5 shipped, 2 excluded

| NPC | Lvl | Rank | Point(s) | Sole-drop signature | Guide step |
|-----|-----|------|----------|---------------------|------------|
| 256892 Kargra the Blind | 46 | 4 | 7 pts, west-center (26-30, 41-49) | 281666 Robes of the Blind Cultist | loop + collect + band-edge note |
| 257034 Mad Marrius | 41 | 2 | 10 pts, center (44-47, 53-57) | 281657 Corrupted Riverglades Pendant | loop + collect |
| 258032 Twilight Forgemaster | 46 | 2 | 33 pts (24 + 9 more), west (27-42, 43-57) | 281665 Twilight Forgehammer | loop + collect + band-edge note |
| 259801 Mosh'gra | 41 | 4 | 21 pts, east-center Rog'mar (58-67, 30-48) | 281676 Rog'mar Trainee Shoulderpads | loop + collect + Horde-aligned note |
| 263141 Scaldaron | 43 | 2 | 14 pts, far west coast (29-33, 68-74) | 271612 Head of Scaldaron (contracted 95935) + 271613 Head of Scaldaron (Horde twin 95936) + 281650 Dragonscale Buckler | loop + collects + core-guide note |

Notes:
- No core-contracted quest references any shipped rare structurally
  (start/end/objectives/sourceItem scanned over the 112-contract quests).
- Above-band handling (band 36-45, Westfall/Hillsbrad/Duskwood precedents —
  excluded, or shipped with an honest note when the data argues for it):
  Kargra (+1) and Twilight Forgemaster (+1 elite) SHIP with a plain
  band-edge note — one level over is reachable at band top, and both carry
  sole-drop signatures; a come-back-later demand for +1 would be dishonest,
  and hiding them would hide real content. (Hillsbrad drew its cutoff hard
  at +1 and excluded Lady Zephris; the data here argues the other way, so
  this call is argued, not silent.) Gul'gash (npc259758, lvl 49 Rare Elite,
  263 spawn points sprawling the whole eastern half, sole drop 281648
  Gul'gash's Greathammer its only loot) is EXCLUDED — a +4 elite is group
  content no note can make soloable (Badlands Anathemus pattern), and a
  263-point loop is not a usable sweep step; logged here with the reason.
- Faction calls (mirrored-hub zone, hub-by-hub check): Mosh'gra is fac=H
  (Horde-aligned Rog'mar patrol, hostile to Alliance characters) — killable,
  ships with that note. Reginald Holmsby (npc256410, lvl 38 Rare, 8 pts at
  the southern farm, faction=A = Alliance-aligned, sole drop 281661
  Well-Worn Pitchfork, no quest takes him or it) is EXCLUDED — friendly to
  the guide's faction, so an Alliance character can neither kill him nor
  loot him; a kill step would be a broken step. Logged here, not shipped.
- Tameability: no tame lines ship. Shared-drop evidence is scrolls, Waylaid
  Crates, a Pristine Hide (Scaldaron) and a Skypierce Javelin — no
  meat/fang-family evidence for any shipped rare, and the core guide carries
  zero `only Hunter` lines, so the corroboration half is unmet regardless.
  Logged in docs/companion-unverified.md. (Scaldaron reads dragon by name,
  quest title and Dragonscale Buckler — not a tameable family in any case.)
- Scaldaron twin-head note: 271612 feeds CONTRACTED quest 95935 Hail the
  Dragonslayer (the note points at the core guide — the companion never
  accepts or turns in); 271613 feeds 95936, the same-title Horde twin
  (races 8589934770, ender in Horde hands) — named so Alliance players know
  the second head is not theirs.
- Respawn timers: unconfirmed anywhere in the data; none stated.

## TREASURES

- "Rock Pile" 649094: 5 fixed pts in the east-center (65.2,25 / 66.4,25.5 /
  67.1,29 / 68.4,29.2 / 74.8,39.6). ONE loop step, said plainly as a fixed
  container. Loot is 271892 Good Rock + 271893 Bad Rock; no quest takes
  either. The zone's only lootable fixed container.
- Excluded with reason (core owns them, Dun Morogh precedent): 625582
  "Fuzzle's Treasure" (contracted 94963 Biting the Hand end-object — note:
  94963 is the documented no-turn-in record, but the object is still core
  content), 629761 "Painted Hide" (contracted 95260 Terrors From the Deep
  start-object). No step duplicates a core interaction.
- The other 21 objects are not treasure: 3 mailboxes, 5 WANTED/Wanted
  posters, 9 name plaques/memorials/book/letter (Brienne Stormhart, Sir
  Howard Armstrong, Roderick the Unbroken, Rosalind Ashwood, Alden
  Amberhall, Fern Crimsonleaf, Lady Isolde Brightlance, Knights of the
  Brotherhood, A Wartorn Land and The Brotherhood, Letter from Dragha),
  616992 Elemental Convergence (12 pts, no loot and no quest link —
  event/decor, not a container), 621813 Loose Soil and 630863 Guild Vault
  (single pts, no loot in the data). No chests, footlockers, clams or caches
  exist in the zone data — the Rock Pile loop is the whole treasure yield,
  stated plainly in the guide rather than padded.

## RECIPES — 15 shipped, all vendor-sold (no mob-dropped recipe has an
in-zone dropper anywhere in the data)

East hub = Powderfuse Port (neutral, fac AH vendors); south hub = Turner
farm country (Alliance, fac A vendors). Hub-by-hub faction check done:
- Cooking, Fimbo Greasemitz (79.02,54.2, port): 21099 Recipe: Smoked
  Sagefish, 21219 Recipe: Sagefish Delight (also sold by Miranda Turner
  (62.51,82.01, south, fac A) — both in-zone sources ship-named per the
  Feralas/Pratt precedent; 22 vendors elsewhere each).
- Cooking, Gritta Chumwater (11 pts around (77-80,52-54), port): 6330
  Recipe: Bristle Whisker Catfish, 6368 Recipe: Rainbow Fin Albacore.
- Cooking, Grizzek (8 pts around (74-77,51-54), port): 16767 Recipe:
  Undermine Clam Chowder.
- Cooking, Innkeeper Zizplink (78.77,53.98, port): 18046 Recipe: Tender
  Wolf Steak.
- Tailoring, Stitch Pinwizzle (6 pts around (77-79,51-53), port): 7088
  Pattern: Crimson Silk Robe, 21358 Pattern: Soul Pouch, 253665 Pattern:
  Linen Reagent Bag, 253668 Pattern: Woolen Reagent Bag (Tanaris sells the
  same four — Stitch is the in-zone source here; the Linen/Woolen bags have
  33 vendors elsewhere and still ship per the Vizzklick precedent).
- Engineering, Kor'gar (8 pts around (77-79,51-54), port): 16046
  Schematic: Masterwork Target Dummy, 16047 Schematic: Thorium Tube.
- Engineering, Fizzix Boomshot (9 pts around (77-80,51-55), port): 18650
  Schematic: EZ-Thro Dynamite II.
- Blacksmithing, Martha Wellsworth (9 pts around (63-65,82-86), south,
  fac A): 251460 Plans: Mithril Warhammer, 274977 Recipe: Plain Ol'
  Paletusk — Martha is the ONLY vendor anywhere for both (nVendorsOut 0).
- No limited-stock flag exists in the data; no recipe is marked limited.
  Each vendor step notes that stock class is unconfirmed.

Excluded with reason:
- 5483 Recipe: Scorpid Surprise — sole vendor 261313 Naluk (8 pts around
  (53-59,45-47)) is Horde-faction (fac H): the zone's Horde-hub vendor.
  Excluded per the Alterac precedent (an Alliance guide does not route a
  Horde-only vendor), logged here.
- Quest-reward recipes: quest records carry no reward data — none shipped,
  class-logged in companion-unverified.
- Trainer-taught staples excluded (Polestar's own profession guides).

Professions with NO Riverglades source (stated plainly in the guide, Dun
Morogh Blacksmithing precedent): Alchemy, Enchanting, First Aid, Fishing,
Leatherworking.
