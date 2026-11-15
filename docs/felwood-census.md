# Felwood census (game data, accept-zone key 1448)

Source: local Forever game data (questie-forever quest/NPC/object/item
dumps, built with `--product wowf` + QuestieDB). Zones table: 1448 =
Felwood (Kalimdor, between Ashenvale 1440 and Winterspring 1452 in the
area table). A quest belongs to Felwood if its accept/start is in 1448:
start-NPC spawn zones, start-object spawn zones, or start-item dropper
spawn zones checked per quest; `zone` field used as a cross-check only.
Race mask 4294967373 = Alliance (established on contracted
Badlands/Blasted Lands quests); 8589934770 = Horde; null = neutral
(taken by the Alliance route). Class bitmask is the standard ChrClasses
mask (2 = Paladin, 4 = Hunter, 256 = Warlock — matches the contracted
SG warlock and hunter quests). Objective types in this zone's data are
only item/kill/object/event.

Band **45-55**: accessible minLevels run m10 (968, a low-level
item-start, free entry), m43 (6131, Timbermaw entry, free entry), a
heavy m45 block (9: Timbermaw/Winterfall/Gorn/Gregory lines), a heavy
m48 block (10: Emerald Sanctuary + Shadow Hold core), m49 (9: Eridan
chains + Arko chain), m50 (9: warlock chains + Meilosh), m52 (3:
Winterfall turn-ins + Salfa), m53 (5249, the Winterspring breadcrumb),
m1 (6 writs + 1 Lunar elder, optional, excluded from band logic per
the Arathi/Hillsbrad precedent), and null (86577, 91952 — both lvl 55;
null-min quests are contracted elsewhere in the pack: Darnassus 98096,
Redridge 93555, Wetlands 98072/98208, STV x5, Riverglades 94961 — so
no floor stated means IN at the band top, objectives in-zone). Quest
own-levels run 18-60; the lvl-60 records (8481/8484, min 45) are IN per
the band rule. Break above m53: next minLevels are m60 (7 class quests,
OUT). Below-band entry is free: 968 (m10) and 6131 (m43) accept
in-zone at their minLevel.

**IN 59 / OUT 70** (38 repeatable, 21 Horde set-aside, 7 above-band,
4 accepts-elsewhere).

## IN — 59

| ID | Title | Lvl/min | Giver / start | Disposition |
|----|-------|---------|---------------|-------------|
| 939 | Flute of Xavaric | 54/49 | item 11668 Flute <- Felwood droppers | item-start IN; 11674 Jadefire Felbind x5 off Jadefire satyrs, south run (~32,67); ender Eridan (51.35,81.51); next 4441 |
| 968 | The Powers Below | 18/10 | item 5352 Book <- Felwood + Darkshore droppers | item-start IN (low-level entry, free); Darkshore census did not contract it (qzone 1455), so Felwood owns it; ender Gerrig is Ironforge (expedition turn-in) |
| 4005 | Aquementas | 54/47 | 9116 Eridan Bluewind (51.35,81.51) | obj 11522 Silver Totem drops off 9453 in TANARIS (expedition complete); ender J.D. Collie is Un'Goro (double-expedition leg); pre 4084; next 3961 Un'Goro (noted, out of scope) |
| 4084 | Silver Heart | 54/47 | Eridan | 11172 Silvery Claws x11 (Felwood bears/wolves) + 11173 Irontree Heart (Irontree Vale mobs, in-zone); pre 3942 Linken's Memory accepts in Un'Goro (structural warning); next 4005 |
| 4101 | Cleansing Felwood | 55/48 | 9528 Arathandris Silversky (54.15,86.83) | 11503 Blood Amber x15 off Warpwood mobs, east (~54-59,15-22); next 5882 |
| 4261 | Ancient Spirit | 56/49 | 9598 Arei (49.57,29.6) | escort event @49.42,14.54; ender Kayneth Stillwind is Ashenvale (expedition turn-in); pre 4442 |
| 4421 | The Corruption of the Jadefire | 54/49 | Eridan | Felsworn x11 + Shadowstalker x9 + Rogue x9 + Xavathras (south Jadefire Run); next 4906 |
| 4441 | Felbound Ancients | 54/49 | Eridan | Vial of Blessed Water x1 comes from object 138498 Temple of the Moon Fountain, which spawns ONLY in Teldrassil (25.4,64.7) and Darnassus — expedition fetch; pre 939; next 4442 |
| 4442 | Purified! | 54/49 | Eridan | no objectives, completes on spot; pre 4441; next 4261 |
| 4906 | Further Corruption | 54/49 | Eridan | Hellcaller x8 + Betrayer x8 + Trickster x8 + Xavaric (north Jadefire clusters ~39-46,13-22); pre 4421 |
| 5083 | Winterfall Firewater | 56/52 | item 12771 Empty Firewater Flask <- Felwood + Winterspring droppers | item-start IN (see BORDERLINE 1); ender Donova Snowden is Winterspring (expedition turn-in); next 5084 Winterspring (noted, out of scope) |
| 5085 | Mystery Goo | 56/52 | object 176091 Deadwood Cauldron (60.2,5.84) | object-start IN; ender Donova is Winterspring (expedition turn-in); pre 5084 Falling to Corruption accepts in Winterspring (structural warning); next 5086 Winterspring (noted) |
| 5155 | Forces of Jaedenar | 51/48 | 10922 Greta Mosshoof (51.21,82.11) | Hound x4 + Guardian x4 + Adept x6 + Cultist x6, Shadow Hold (~34-39,57-62); next 5157 |
| 5156 | Verifying the Corruption | 54/48 | 10921 Taronn Redfeather (50.89,81.62) | Entropic Beast x2 + Entropic Horror x2 + crater event @41.03,41.96 (Shatter Scar Vale) |
| 5157 | Collection of the Corrupt Water | 52/48 | Greta | Corrupt Moonwell Water x1 from object 176184 Corrupt Jaedenar Moonwell (35.17,59.79); next 5158 |
| 5158 | Seeking Spiritual Aid | 52/48 | Greta | no objectives; ender Islen Waterseer is the Barrens (expedition turn-in); next 5159 Cleansed Water accepts in the Barrens (noted, out of scope) |
| 5165 | Dousing the Flames of Protection | 55/48 | Greta | 3 braziers in Shadow Hold (36.27,56.3 / 37.68,52.69 / 36.73,53.27); pre 5159 accepts in the Barrens (structural warning); next 5242 |
| 5202 | A Strange Red Key | 55/49 | item 13140 Blood Red Key <- Felwood + Darkshore droppers | item-start IN; ender Captured Arko'narin (36.21,55.47); next 5203 |
| 5203 | Rescue From Jaedenar | 55/49 | Arko'narin | escort event @35.45,59.06; ender Jessir Moonbow (51.35,82.01); next 5204 |
| 5204 | Retribution of the Light | 57/49 | Jessir | kill Rakaiah (38.3,50.51); ender Remains of Trey Lightforge (38.5,50.41); next 5385 |
| 5242 | A Final Blow | 58/48 | Greta | Moora (38.81,46.87) + Salia + 13207 Shadow Lord Fel'dan's Head (Fel'dan 38.82,46.78, Jaedenar summit); pre 5165 |
| 5249 | To Winterspring! | 56/53 | 10924 Ivy Leafrunner (50.96,81.58) | no objectives; ender Wynd Nightchaser is Winterspring (expedition turn-in); excl 5250 Starfall is the Teldrassil-accepting variant (see BORDERLINE 2); next 5244 Winterspring (noted) |
| 5385 | The Remains of Trey Lightforge | 57/49 | Remains of Trey Lightforge | no objectives; ender Jessir; pre 5204 |
| 5882 | Salve via Hunting | 55/48 | Arathandris | one-time feeder (rep undefined) into the repeatable 4103; 11515 Corrupted Soul Shard x6 (source verified in guide phase); next 4103 repeatable (noted, out of scope) |
| 5883 | Salve via Mining | 55/48 | Arathandris, Mining | one-time feeder; optional + when-skill gated per settled handling; 11513 Tainted Vitriol x4; next 4104 repeatable (noted) |
| 5884 | Salve via Gathering | 55/48 | Arathandris, Herbalism | one-time feeder; optional + gated; 11514 Fel Creep x4; next 4105 repeatable (noted) |
| 5885 | Salve via Skinning | 55/48 | Arathandris, Skinning | one-time feeder; optional + gated; 11512 Patch of Tainted Skin x5; next 4106 repeatable (noted) |
| 5886 | Salve via Disenchanting | 55/48 | Arathandris, Enchanting | one-time feeder; optional + gated; 11174 Lesser Nether Essence x1; next 4107 repeatable (noted) |
| 6031 | Runecloth | 55/50 | 11557 Meilosh, Felwood spawn (65.69,2.81) | dual-spawns Winterspring; Felwood spawn contracts it here (Winterspring census must set aside — noted below); Runecloth x30 bag note |
| 6032 | Sacred Cloth | 55/50 | Meilosh, Tailoring | optional + gated; dual-spawn note as 6031; Mooncloth x2 crafted bag note |
| 6131 | Timbermaw Ally | 48/43 | 11554 Grazle (50.93,85.01) | Deadwood south village kills x7 (twin with 8460 — counts differ x7 vs x6, both routed with a note) |
| 6221 | Deadwood of the North | 55/45 | Grazle | Deadwood north village kills x5 (twin with 8461 — x5 vs x6, both routed with a note) |
| 6241 | Winterfall Activity | 56/52 | 11556 Salfa, Felwood spawn (68.3,6.1) | dual-spawns Winterspring, contracted here (set-aside note as 6031); kills are Winterspring-only mobs (7439/7440/7438 spawn 1452 only) — expedition farm; twin handling vs 8464 differs by counts (see BORDERLINE 3) |
| 7601 | What Niby Commands | 50/50 | 14469 Niby the Almighty (41.38,44.85), Warlock | only-Warlock; no objectives; ender Impsy (41.36,45.02); next 7602 |
| 7602 | Flawless Fel Essence | 55/50 | 14470 Impsy, Warlock | only-Warlock; 3 essences: Jaedenar 18622 (in-zone) + Azshara 18624 (expedition) + Dark Portal 18623 = Blasted Lands (expedition, dropper verified in guide phase); next 7603 |
| 7603 | Kroshius' Infernal Core | 55/50 | Impsy, Warlock | only-Warlock; kill Kroshius (spawn verified in guide phase) + core; ender Niby |
| 8420 | Hot and Itchy | 52/50 | Impsy, Warlock | only-Warlock; excl 8419 An Imp's Request is the Stormwind-accepting variant (contracted in stormwind-city — chain-consistent Felwood leg contracted here, see BORDERLINE 4); Felcloth x1; pre none; next 8421 |
| 8421 | The Wrong Stuff | 52/50 | Impsy, Warlock | only-Warlock; 20613 Rotting Wood x10 + 20614 Bloodvenom Essence x4 (sources verified in guide phase); pre 8420 (in-contract) + 8419 Stormwind (noted alternative) |
| 8422 | Trolls of a Feather | 52/50 | Impsy, Warlock | only-Warlock; voodoo feathers 20606/20607/20608 x2 each (sources verified in guide phase); pre 8421 |
| 8460 | Timbermaw Ally | 48/45 | Grazle | twin with 6131 (x6 vs x7); next 8462; both routed with a note |
| 8461 | Deadwood of the North | 55/45 | 15395 Nafien, Felwood spawn (64.77,8.13) | twin with 6221 (x6 vs x5); dual-spawn note as 6031; next 8465 |
| 8462 | Speak to Nafien | 55/45 | Grazle | ender Nafien (Felwood point); pre 8460 |
| 8464 | Winterfall Activity | 58/45 | Salfa | Winterfall kills x8 (twin with 6241 — x8 vs x6, both routed with a note); kills are Winterspring-only — expedition farm; dual-spawn note as 6031 |
| 8465 | Speak to Salfa | 55/45 | Nafien | ender Salfa (Felwood point); pre 8461; dual-spawn note as 6031 |
| 8470 | Deadwood Ritual Totem | 55/45 | item 20741 <- Felwood droppers | item-start IN; ender Kernda (65.5,3.52) |
| 8471 | Winterfall Ritual Totem | 56/50 | item 20742 <- Felwood + Winterspring droppers | item-start IN (Felwood source exists; Winterspring census must set aside — noted below); ender Kernda |
| 8481 | The Root of All Evil | 60/45 | 11555 Gorn One Eye (65.18,2.68) | 21145 Essence of Xandivious — Xandivious spawns ONLY in Winterspring (69.8,38.2): expedition kill; next 8484 |
| 8484 | The Brokering of Peace | 60/45 | Gorn One Eye | Alliance leg; ender King Magni Bronzebeard is Ironforge (expedition turn-in); pre 8481 |
| 86577 | A Sampling of Putrescence | 55/null | 10920 Kelek Skykeeper (51.14,81.75) | null-min IN per precedent (10 contracted null-min quests pack-wide); organs off Felwood bears/wolves (droppers in 1448) |
| 86611 | Stag Lord's Bauble | 55/48 | object 661778 Statue of Malorne (42.03,47.36) | object-start IN; ender Golhine the Hooded (61.93,24.54); Horde twin 86612 set aside |
| 8723 | Nightwind the Elder | 60/1 | 15603 Elder Nightwind | Lunar elder, seasonal event flag — optional + seasonal note per the SG/TN precedent |
| 81790 | Materials of Significance | 53/45 | 221636 Gregory (44.6,52) | Forever-custom Paladin quest (class mask 2 = Paladin — the standard ChrClasses bitmask, cross-checked against contracted Warlock-256 and Hunter-4 quests); only-Paladin; 220166 Fiery Infernal Core drops in-zone, but 220167 (Grave Mound object 441222 has NO spawns), 220168 (vendor 9499 MISSING from NPC data) and 220169 (no source in data at all) are sourceless — R2 residue with bag notes |
| 91952 | The Source of the Corruption | 55/null | Greta | null-min IN per precedent; no objectives; ender Ketharas (73.34,81.88) is Mount Hyjal zone 2482 (expedition turn-in) |
| 94259 | Craftsman's Writ: Nature Protection Potion | 60/1 | Greta, Alchemy | R5 writ: optional + when-skill gated + bag note (crafted potion turn-in); sourceless item-start per the TN/SG writ precedent |
| 94271 | Craftsman's Writ: Ornate Mithril Shoulders | 60/1 | Taronn, Blacksmithing | R5 writ, same handling |
| 94283 | Craftsman's Writ: Goblin Land Mine | 60/1 | Jessir, Engineering | R5 writ, same handling |
| 94295 | Craftsman's Writ: Wild Leather Helmet | 60/1 | Ivy, Leatherworking | R5 writ, same handling |
| 94307 | Craftsman's Writ: Shadoweave Robe | 60/1 | Eridan, Tailoring | R5 writ, same handling |
| 94308 | Craftsman's Writ: Enchanted Mageweave Pouch | 60/1 | Impsy, Enchanting | R5
...[truncated 6154 chars]