---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 909
sectorial_slug: white-company
sectorial_name: White Company
parent_faction: Non-Aligned Armies (NA2)
rules_baseline: N5.3
army_source_version: "7.26246.159"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-16
coverage: "Complete current White Company main roster, standard profile/loadout digest and AVA, current Fireteam chart and reverse access index, optional Spec-Ops/Team-Ops boundary, linked Reinforcements boundary, and derived tactical indexes."
---

# White Company — N5.3 sectorial reference

## Overview and provenance

Repository-native reference for **White Company** (Army sectorial ID `909`), part of the Non-Aligned Armies (NA2). It is intended to answer roster, profile, AVA, points/SWC, Lieutenant, specialist, hacking/network, deployment and Fireteam questions without reopening Army.

Sources used:

- Corvus Belli Army-derived revision `7.26246.159` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` (`army: N5.3 + ITS18`, 2026-09-03).
- Versioned source: `n5/white-company/7.26246.159.json`, blob `14c4655e63867b9ffb3cc2c12f4ad1323f2ad338`.
- Aggregate source: `n5/white-company/white-company.json`, blob `0ceb4f53f65a64a7da5e77496ce15b1fc3effa4a` at the pinned source commit.
- InfinityDB normalization/semantics: commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers **44 standard White Company roster entries** explicitly assigned to faction `909` by the current Army source.
- `Rumbler Spec-Ops` (ID `1925`) and `NA2 Team-Ops` (ID `1939`) are optional-mode entries and are kept separate from the standard roster.
- Generic Soldiers-of-Fortune / mercenary-catalogue objects with an empty `factions` array are excluded; explicit White Company mercenary/guest entries are retained.
- Linked Reinforcement army ID: **999**. Main and Reinforcement rosters remain separate.
- Army raw Fireteam `DUO: 256` is the source sentinel for effectively unlimited Duo formations, not a literal limit of 256.
- Disabled subordinate forms/peripherals such as Auxbots, Shàngdiào, Bâtard, Anaconda Operator, TurtleMek and Cordelia-as-an-included-form are not counted as independent roster entries.
- `FTO` labels do not independently grant Fireteam access. The current `CLIPPER DRONBOT FTO` profile has no corresponding White Company Fireteam-chart row and is not a Wildcard.
- The current source contains **no top-level relation records** for White Company.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | White Company |
| Parent faction | Non-Aligned Armies (NA2) |
| Army ID | `909` |
| Army slug | `white-company` |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard Main roster entries | 44 |
| Optional-mode entries | Rumbler Spec-Ops; NA2 Team-Ops |
| Reinforcement roster | Army ID `999` |
| Core | up to 1 |
| Haris | up to 1 |
| Duo | unlimited/source `256` sentinel |
| Fireteam families | Fusiliers; K2; White Company; Chaksa Longarms; Varangian Guards; Anaconda |
| Explicit Wildcards | Hǎidào; Hawkwood; Liang Kai; Shona Carano; Emily Handelman; Hannibal; Valkyrie; Laxmee; Señor Massacre |

## Fireteam chart limits and sectorial-level restrictions

| Constraint | Current source value / normalized meaning |
|---|---|
| Core | `1` |
| Haris | `1` |
| Duo | `256` — normalized as unlimited Duos |
| Main/Reinforcement mixing | Main roster and Reinforcement roster `999` remain separate |
| Wildcards | Only the explicit Wildcard rows listed below |
| Profile restrictions | Preserve FTO, Spec-Ops, counts-as comments, `required` flags and source minimums exactly |

The canonical chart below is authoritative. Do not import Fireteam permissions from older White Company charts, PanOceania, Yu Jing, Foreign Company or another NA2 sectorial.

## Unit roster index

| Unit ID | Unit | AVA | Notes |
|---:|---|---:|---|
| 950 | Danavas Hackers | 1 | HD+; Pitcher |
| 18 | Clipper Dronbot | 2 | Guided ML option; FTO-labelled option has no current FT access |
| 1485 | Karhu Special Group | 5 | K2 member; NCO; MSV1 |
| 137 | Zhanshi Yīshēng | 1 | Doctor |
| 36 | Peacemaker Armbots | 2 | Repeater; FD +20; Auxbot options |
| 1500 | Liang Kai | 1 | Explicit Wildcard; CC/assault |
| 35 | Bulleteer Armbots | 2 | Repeater; Mimetism (-6) |
| 5 | ORC Troops | 5 | White Company FT member; LT/HD options |
| 17 | Sierra Dronbot | 2 | Total Reaction |
| 1344 | Laxmee | 1 | HD+; Pitcher; explicit Wildcard |
| 161 | Yáozăo | 2 | Servant peripheral |
| 1751 | Blade-Ops | 1 | TacAware; profiles 1–2 are White Company FTO |
| 1 | Fusiliers | Total | Fusilier FT anchor; LT/HD/FO options |
| 19 | Fugazi Dronbot | 3 | Repeater; Flash Pulse |
| 138 | Mech-Engineer | 1 | Engineer |
| 1310 | Chaksa Longarms | 3 | Native Duo/Haris |
| 38 | Mulebots | 2 | Baggage; EVO/TR options |
| 134 | Guiláng Skirmishers | 2 | Camo/Infiltration; HD/FO/LT options |
| 133 | Gūijiă Squadrons | 1 | TAG; TacAware; LT option |
| 1153 | Carmen Johns & Bâtard | 1 | Irregular/Impetuous biker; smoke |
| 462 | Señor Massacre | 1 | Explicit Wildcard; Eclipse |
| 1556 | John Hawkwood | 1 | Explicit Wildcard `(Fusiliers)`; LT/CoC options |
| 1494 | Jujak Regiment | 4 | White Company FT member; LT/Engineer options |
| 122 | CSU | 2 | Fusilier FT member; specialist option |
| 1750 | Blockers | 1 | Fusilier FT member; Sensor/HD/Pitcher options |
| 16 | Pathfinder Dronbot | 2 | FO/Sensor; TacAware option |
| 1502 | Kunai Solutions Ninjas | 2 | Hidden Deployment; long-range attack/ARO |
| 1246 | Hǎidào Special Support Group | 3 | Explicit Wildcard; KHD/Engineer/CoC/MSV2 options |
| 1484 | Nøkken | 2 | FD +20; Mimetism (-6); HD/KHD/FO options |
| 338 | Kaplan Tactical Services | 5 | K2 and Anaconda FT member; specialists |
| 300 | Anaconda | 2 | TAG; TacAware; native Duo with Kaplan access |
| 50 | Warcor | 1 | Irregular |
| 380 | Scarface & Cordelia | 1 | Combined TAG + Engineer selection |
| 1343 | Valkyrie | 1 | Explicit Wildcard `(ORCs)`; CC |
| 1482 | Wild Bill | 1 | K2 member |
| 126 | Tiger Soldiers | 2 | Combat Jump/Parachutist |
| 1461 | Varangian Guard | 2 | Native Duo; smoke/CC |
| 3 | Nisses | 2 | White Company FT member; MSV2 |
| 1505 | Shona Carano | 1 | Explicit Wildcard `(Varangian)`; CC |
| 1570 | Beasthunters Free Guild | 2 | Profile 1 K2 FTO; profiles 2–3 camo/FD |
| 956 | Cube Jäger | 1 | Airborne Paramedic |
| 1345 | Hannibal | 1 | Explicit Wildcard `(Orcs)`; TacAware/Counterintelligence/Sensor; LT options |
| 1538 | Táowù | 1 | Fusilier FT member; Holomask/Counterintelligence/CoC option |
| 1072 | Emily Handelman | 1 | Explicit Wildcard `(Fusiliers)`; FO/CoC option |

## Current profile/loadout digest

Profile IDs are source option IDs. This is a compact list-building digest; the pinned Army JSON remains authoritative for full stat blocks and weapon traits.

### Danavas Hackers — ID 950, AVA 1
- `2` — **22 / 0.5**: Combi Rifle, Pitcher, Breaker Pistol; Hacking Device Plus with upgraded Oblivion.

### Clipper Dronbot — ID 18, AVA 2
- `1` — **16 / 1.5**: Missile Launcher; Guided.
- `5` — **19 / 1.5**: Missile Launcher; profile name `CLIPPER DRONBOT FTO`, but **no current White Company Fireteam access**.

### Karhu Special Group — ID 1485, AVA 5
All profiles currently have NCO, MSV1, Mimetism (-3) and Climbing Plus.
- `1` — **22 / 0**: MULTI Rifle, Blitzen, AP Mine.
- `2` — **22 / 0**: MULTI Rifle, E/Marat, AP Mine.
- `3` — **34 / 1.5**: Feuerbach, AP Mine.
- `4` — **25 / 0**: MULTI Rifle, Blitzen, D-Charges; Engineer.
- `5` — **24 / 0**: MULTI Rifle, Blitzen, AP Mine; Paramedic.

### Zhanshi Yīshēng — ID 137, AVA 1
- **14 / 0**: Combi Rifle; Doctor, MediKit.

### Peacemaker Armbots — ID 36, AVA 2
Repeater, FD +20, Mimetism (-3); Auxbots are included subordinate forms.
- `1` — **23 / 0**: Heavy Shotgun, Pulzar + Auxbot.
- `3` — **24 / 0.5**: Heavy Shotgun, Pulzar + alternate/minelayer Auxbot package.
- `4` — **23 / 0**: Boarding Shotgun, Pulzar; BS Attack (+1B), no Auxbot.
- `5` — **27 / 0**: Boarding Shotgun, Pulzar; BS Attack (+1B) + Auxbot.

### Liang Kai — ID 1500, AVA 1
- **21 / 0**: Chain Rifle, Light Shotgun, Flash Pulse, EXP CCW; Martial Arts 4, Berserk, FD +10, Mimetism (-3), NWI, Super-Jump. Explicit Wildcard.

### Bulleteer Armbots — ID 35, AVA 2
Repeater, Mimetism (-6).
- `1` — **19 / 0**: Heavy Shotgun (+1B).
- `2` — **22 / 1**: Spitfire.

### ORC Troops — ID 5, AVA 5
- `1` — **28 / 0**: MULTI Rifle.
- `2` — **29 / 0**: MULTI Rifle; TinBot Firewall (-3).
- `3` — **34 / 1.5**: HMG.
- `4` — **26 / 0**: Boarding Shotgun (+1B).
- `6` — **33 / 0.5**: MULTI Rifle; Hacking Device.
- `7` — **28 / 0**: MULTI Rifle; Lieutenant.
- `8` — **34 / 1**: HMG; Lieutenant.
- `10` — **35 / 1.5**: Feuerbach.
- `11` — **27 / 0**: Boarding Shotgun (+1B); TinBot Firewall (-3).

### Sierra Dronbot — ID 17, AVA 2
Total Reaction, 360º Visor.
- `1` — **23 / 1**: HMG.
- `2` — **18 / 0**: Thunderbolt (+1B).

### Laxmee — ID 1344, AVA 1
- **24 / 0.5**: SMG, Pitcher, Cybermine, D-Charges; Hacking Device Plus with Fairy Dust upgrade; Mimetism (-3), Minelayer. Explicit Wildcard.

### Yáozăo — ID 161, AVA 2
- **3 / 0**: Servant peripheral.

### Blade-Ops — ID 1751, AVA 1
All profiles have Tactical Awareness, Mimetism (-3), Stealth and BS Attack (SR-1).
- `1` — **20 / 0**: `BLADE FTO`; Boarding Shotgun, D-Charges, Silenced Pistol.
- `2` — **23 / 0**: `BLADE FTO`; AP SMG, D-Charges, Silenced Pistol; Engineer.
- `3` — **30 / 0**: `BLADE`; AP SMG, E/Mitter, D-Charges; Engineer, FD +20, Decoy.
- `4` — **30 / 0**: `BLADE`; AP SMG, E/Mitter, D-Charges; Engineer, Parachutist, Decoy.
Only profiles **1–2** match the White Company Fireteam row.

### Fusiliers — ID 1, AVA Total
- `1` — **10 / 0**: Combi Rifle.
- `2` — **18 / 1**: HMG.
- `4` — **15 / 1.5**: Missile Launcher.
- `5` — **16 / 1**: MULTI Sniper Rifle.
- `6` — **15 / 0.5**: Combi Rifle; Hacking Device.
- `8` — **12 / 0**: Combi Rifle, Flash Pulse; Forward Observer, Deployable Repeater.
- `9` — **12 / 0**: Combi Rifle; Paramedic.
- `10` — **10 / 0**: Combi Rifle; Lieutenant.

### Fugazi Dronbot — ID 19, AVA 3
- **7 / 0**: Flash Pulse; Repeater, Mimetism (-3).

### Mech-Engineer — ID 138, AVA 1
- `1` — **14 / 0**: Combi Rifle, D-Charges; Engineer.
- `2` — **15 / 0**: same + Deployable Cover.
- `3` — **17 / 0**: Combi Rifle, D-Charges + Armed Turret (Combi Rifle).

### Chaksa Longarms — ID 1310, AVA 3
- `1` — **21 / 0**: Combi Rifle, Pulzar, E/M Grenades.
- `2` — **29 / 1.5**: Portable Autocannon, Pulzar.
- `3` — **24 / 1.5**: Missile Launcher, Pulzar.
- `4` — **25 / 0**: Mk12, Pulzar, AP Mine.

### Mulebots — ID 38, AVA 2
Baggage, Remote Presence.
- `1` — **8 / 0**: Deactivator, Repeater.
- `2` — **14 / 0.5**: EVO Hacking Device.
- `3` — **17 / 0**: Combi Rifle, Repeater; Total Reaction.

### Guiláng Skirmishers — ID 134, AVA 2
Camouflage, Infiltration, Mimetism (-3), MSV1, Stealth.
- `2` — **23 / 0**: Boarding Shotgun, Shock Mine, D-Charges.
- `3` — **28 / 1.5**: MULTI Sniper Rifle, Shock Mine, D-Charges.
- `4` — **31 / 0.5**: Combi Rifle, Shock Mine, D-Charges; Hacking Device.
- `5` — **25 / 0.5**: Boarding Shotgun, Shock Mine, D-Charges; Deployable Repeater, Minelayer.
- `6` — **27 / 0**: Combi Rifle, Flash Pulse, Shock Mine, D-Charges; Forward Observer.
- `7` — **23 / 1**: Boarding Shotgun, Shock Mine, D-Charges; Lieutenant.

### Gūijiă Squadrons — ID 133, AVA 1
TAG with Tactical Awareness, Super-Jump and ECM: Guided.
- `1` — **77 / 1.5**: MULTI HMG, Heavy Flamethrower, DA CCW.
- `2` — **77 / 2**: same; Lieutenant.
Includes disabled Shàngdiào ancillary form; it is not an independent roster entry.

### Carmen Johns & Bâtard — ID 1153, AVA 1
- **17 / 0**: Carmen with Chain Rifle (+1B), Smoke Grenades/Smoke Grenade Launcher, AP Heavy Pistol, DA CCW; Bâtard included as subordinate peripheral. Irregular, Impetuous.

### Señor Massacre — ID 462, AVA 1
Explicit Wildcard.
- `1` — **27 / 0**: Breaker Combi Rifle, Eclipse Grenades, E/M Grenades, Boarding Pistol, Shock/E/M CC weapons.
- `2` — **25 / 0**: Boarding Shotgun (+1B), Eclipse Grenades, E/M Grenades, Boarding Pistol, Shock/E/M CC weapons.

### John Hawkwood — ID 1556, AVA 1
Explicit Wildcard, counts as `(Fusiliers)`.
- `6` — **35 / 1**: K1 Sniper Rifle, Nanopulser, MULTI Pistol, DA CCW.
- `7` — **40 / 0**: Combi Rifle (+1B), Nanopulser, MULTI Pistol, DA CCW; Chain of Command, X-Visor.
- `8` — **35 / 1**: K1 Sniper package; Lieutenant.
- `9` — **39 / 1**: K1 Sniper package; Lieutenant (+1 Order).

### Jujak Regiment — ID 1494, AVA 4
- `1` — **25 / 0**: Combi Rifle, Heavy Flamethrower.
- `2` — **26 / 0**: Breaker Combi Rifle, Heavy Flamethrower.
- `3` — **28 / 0**: Breaker Combi Rifle, Heavy Flamethrower; TinBot Firewall (-3).
- `4` — **29 / 1.5**: Missile Launcher, Light Flamethrower.
- `5` — **31 / 1.5**: Spitfire, Heavy Flamethrower.
- `7` — **27 / 0**: Vulkan Shotgun, Panzerfaust; TinBot Firewall (-3).
- `8` — **29 / 0**: Vulkan Shotgun, Panzerfaust, D-Charges; Engineer.
- `9` — **25 / 0**: Combi Rifle, Heavy Flamethrower; Lieutenant.

### CSU — ID 122, AVA 2
- `1` — **10 / 0**: Breaker Rifle, Nanopulser (+1B), MULTI Pistol.
- `2` — **11 / 0**: Combi Rifle, Nanopulser (+1B), MULTI Pistol.
- `3` — **11 / 0**: Boarding Shotgun, MULTI Pistol, Adhesive Launcher Rifle (+1B).
- `4` — **11 / 0**: Rifle/Light Shotgun, MULTI Pistol; Specialist Operative.
- `5` — **13 / 0**: Breaker Combi Rifle, Nanopulser (+1B), MULTI Pistol; Specialist Operative.

### Blockers — ID 1750, AVA 1
Biometric Visor, X-Visor, Sensor, Discover reroll, BS Attack (+1B).
- `1` — **15 / 0**: Adhesive Launcher Rifle, Pulzar, **Pitcher**, Flash Pulse, MULTI Pistol; Specialist Operative.
- `2` — **19 / 0.5**: Adhesive Launcher Rifle, Pulzar, Flash Pulse, MULTI Pistol; Hacking Device with Firewall upgrade. The current source option does **not** carry the Pitcher shown on profile 1.

### Pathfinder Dronbot — ID 16, AVA 2
Repeater, Forward Observer, Sensor, Triangulated Fire.
- `1` — **14 / 0**: Combi Rifle, Flash Pulse.
- `2` — **17 / 0**: same + Tactical Awareness.

### Kunai Solutions Ninjas — ID 1502, AVA 2
Camouflage, Hidden Deployment, Mimetism (-6), Climbing Plus, Stealth.
- `1` — **28 / 1.5**: MULTI Sniper Rifle.
- `2` — **26 / 0**: Shock Marksman Rifle; AP-oriented BS Attack modifier.
- `3` — **25 / 0.5**: Thunderbolt, PARA Mine; T2-oriented BS Attack modifier.

### Hǎidào Special Support Group — ID 1246, AVA 3
Explicit Wildcard; NWI and Shock Immunity.
- `2` — **24 / 1**: Red Fury.
- `3` — **24 / 0**: Combi Rifle, D-Charges; Chain of Command.
- `4` — **22 / 0**: Boarding Shotgun (+1B), Pitcher, D-Charges; Killer Hacking Device.
- `5` — **25 / 0**: MULTI Rifle, D-Charges; Engineer.
- `6` — **29 / 1.5**: MULTI Sniper Rifle; MSV2.

### Nøkken — ID 1484, AVA 2
FD +20, Mimetism (-6), Terrain Total; Transmutation/Bangbomb chassis.
- `1` — **26 / 1.5**: Spitfire.
- `2` — **27 / 0.5**: Combi Rifle, Light Shotgun; Hacking Device.
- `3` — **25 / 0**: Combi Rifle, Light Shotgun; Killer Hacking Device.
- `4` — **24 / 0.5**: Combi Rifle, Light Shotgun, Shock Mine; Minelayer.
- `5` — **22 / 0**: Boarding Shotgun (+1B), Panzerfaust, Flash Pulse; Forward Observer.
- `6` — **24 / 0**: Boarding Shotgun (+1B), Panzerfaust; MSV1.

### Kaplan Tactical Services — ID 338, AVA 5
Mimetism (-3), BTS6, WIP14; K2 member and Anaconda-Duo member.
- `1` — **21 / 0**: Combi Rifle, Adhesive Launcher Rifle, D-Charges.
- `2` — **20 / 0**: Combi Rifle, Blitzen.
- `3` — **25 / 1.5**: MULTI Sniper Rifle.
- `4` — **20 / 1.5**: Heavy Rocket Launcher, Light Shotgun.
- `5` — **25 / 1**: Spitfire.
- `6` — **25 / 0**: Combi Rifle, Adhesive Launcher Rifle, D-Charges; Engineer.
- `7` — **24 / 0**: Combi Rifle, Blitzen; Doctor.
- `8` — **21 / 0**: Combi Rifle, Blitzen; Specialist Operative.

### Anaconda — ID 300, AVA 2
TAG; Tactical Awareness, Warhorse, ECM: Guided, Escape System.
- `1` — **59 / 1.5**: AP Spitfire, Heavy Flamethrower, AP Thunderbolt, DA CCW.
- `2` — **59 / 1.5**: HMG, Light Shotgun, Panzerfaust, DA CCW.
Anaconda Operator is an included disabled state, not an independent selection.

### Warcor — ID 50, AVA 1
- `1` — **3 / 0**: Flash Pulse; 360º Visor.
- `2` — **3 / 0**: Flash Pulse; Sixth Sense.

### Scarface & Cordelia — ID 380, AVA 1
Combined selection; Scarface has Tactical Awareness and Cordelia is the included Engineer.
- `1` — **80 / 1.5**: Scarface Loadout Alpha + Cordelia.
- `2` — **76 / 1.5**: Scarface Loadout Beta + Cordelia.
- `3` — **76 / 1.5**: Scarface Loadout Gamma + Cordelia.
Scarface/TurtleMek/Cordelia component profiles are disabled constituent forms and are not separate roster entries.

### Valkyrie — ID 1343, AVA 1
Explicit Wildcard, counts as `(ORCs)`.
- `1` — **28 / 0**: Heavy Shotgun, Grenades, Heavy Pistol, EXP CCW.
- `2` — **33 / 0**: MULTI Rifle, Grenades, Heavy Pistol, EXP CCW.

### Wild Bill — ID 1482, AVA 1
K2 member.
- `1` — **22 / 0**: Contender, MULTI Pistol (+1B).
- `2` — **24 / 0**: Rifle, Light Shotgun, MULTI Pistol (+1B); Shock-oriented BS Attack.

### Tiger Soldiers — ID 126, AVA 2
Mimetism (-3), Parachutist, Combat Jump, Super-Jump (Jet Propulsion).
- `2` — **20 / 0**: Boarding Shotgun, D-Charges.
- `4` — **29 / 1.5**: Spitfire.
- `5` — **29 / 0.5**: Combi Rifle, Light Flamethrower; Hacking Device.
- `6` — **26 / 0**: Combi Rifle, Light Flamethrower; Paramedic.

### Varangian Guard — ID 1461, AVA 2
Irregular/Impetuous assault troops; native Duo.
- `3` — **13 / 0**: Boarding Shotgun, Smoke Grenades, Heavy Pistol, AP CCW.
- `4` — **12 / 0**: SMG, Chain Rifle, Smoke Grenades, Heavy Pistol, AP CCW.
- `5` — **13 / 0**: SMG, Chain-colt (+1B), Smoke Grenades, Heavy Pistol, AP CCW.
- `6` — **13 / 0**: SMG, Chain Rifle, Smoke Grenades, Heavy Pistol, Trench-Hammer, AP CCW.

### Nisses — ID 3, AVA 2
MSV2, Mimetism (-3), Terrain Total.
- `2` — **31 / 1.5**: HMG.
- `3` — **29 / 1.5**: MULTI Sniper Rifle.
- `5` — **30 / 0.5**: Combi Rifle, Light Shotgun; Hacking Device.
- `6` — **28 / 0**: Combi Rifle, Light Shotgun; Paramedic.

### Shona Carano — ID 1505, AVA 1
- **22 / 0**: SMG, Nanopulser (+1B), Flash Pulse, AP+EXP CCW; Martial Arts 4, NWI, Super-Jump. Explicit Wildcard, counts as `(Varangian)`.

### Beasthunters Free Guild — ID 1570, AVA 2
- `1` — **9 / 0**: `BEASTHUNTER FTO`; Heavy Flamethrower, Panzerfaust, AP Mine, DA CCW.
- `2` — **15 / 0**: non-FTO; Heavy Flamethrower, Tactical Bow, AP Mine; Camouflage, FD +20.
- `3` — **15 / 0**: non-FTO; Heavy Flamethrower, Panzerfaust, AP Mine; Camouflage, FD +20.
Only profile **1** matches the K2 Fireteam row.

### Cube Jäger — ID 956, AVA 1
Parachutist; MediKit/Paramedic.
- `1` — **15 / 0**: Boarding Shotgun, Pistol, Monofilament CCW.
- `2` — **18 / 0**: SMG, E/Mitter, Pistol, Monofilament CCW.

### Hannibal — ID 1345, AVA 1
Tactical Awareness, Counterintelligence, Sensor, NWI; explicit Wildcard, counts as `(Orcs)`.
- `5` — **24 / 0**: Vulkan Shotgun, Nanopulser, Flash Pulse, Breaker Pistol.
- `6` — **30 / 0**: MULTI Marksman Rifle, Nanopulser, Breaker Pistol.
- `7` — **27 / 0**: profile 5 package + Strategic Deployment.
- `8` — **33 / 0**: profile 6 package + Strategic Deployment.
- `9` — **31 / 0**: profile 5 package; Lieutenant, Strategic Deployment, Strategos L1.
- `10` — **37 / 0.5**: profile 6 package; Lieutenant, Strategic Deployment, Strategos L1.

### Táowù — ID 1538, AVA 1
Holomask, Counterintelligence, Specialist Operative, Natural Born Warrior; Fusilier-family member.
- `1` — **19 / 0**: Light Shotgun, E/Marat, Flash Pulse, Viral Pistol, PARA CCW.
- `2` — **16 / 0**: Contender, Pulzar, Flash Pulse, Viral Pistol, PARA CCW.
- `3` — **21 / 0.5**: profile 2 package; Chain of Command.

### Emily Handelman — ID 1072, AVA 1
Explicit Wildcard, counts as `(Fusiliers)`; Forward Observer, X-Visor, Mimetism (-3), Number 2, Dogged.
- `1` — **22 / 0**: Breaker Combi Rifle, Nanopulser, Flash Pulse, Assault Pistol.
- `2` — **28 / 0**: Combi Rifle, Grenade Launcher, E/M Grenade Launcher, Nanopulser, Flash Pulse, Assault Pistol; Chain of Command.
- `3` — **24 / 0**: same grenade-launcher package without CoC; Flash Pulse (+1B).

## Lieutenant and order-control index

| Unit/profile | Function |
|---|---|
| Fusilier profile 10 | Lieutenant, 10 / 0 |
| ORC profile 7 | Lieutenant, 28 / 0 |
| ORC profile 8 | HMG Lieutenant, 34 / 1 |
| Guiláng profile 7 | Camo/Infiltration Lieutenant, 23 / 1 |
| Gūijiă profile 2 | TAG Lieutenant; Tactical Awareness, 77 / 2 |
| Jujak profile 9 | Lieutenant, 25 / 0 |
| Hawkwood profile 8 | Lieutenant, 35 / 1 |
| Hawkwood profile 9 | Lieutenant +1 Order, 39 / 1 |
| Hannibal profiles 9–10 | Lieutenant + Strategos L1; also Tactical Awareness |
| Karhu | NCO on all current profiles |
| Blade-Ops | Tactical Awareness on all current profiles |
| Gūijiă / Anaconda / Scarface / Hannibal | Tactical Awareness |
| Pathfinder profile 2 | Tactical Awareness |
| Hǎidào profile 3 | Chain of Command |
| Hawkwood profile 7 | Chain of Command |
| Táowù profile 3 | Chain of Command |
| Emily profile 2 | Chain of Command |
| Hannibal / Táowù | Counterintelligence |

## Hacking and network index

### Hackers

- **HD+:** Danavas; Laxmee.
- **Hacking Device:** ORC; Fusilier; Blocker; Guiláng; Nøkken; Tiger Soldier; Nisse.
- **KHD:** Hǎidào; Nøkken.
- **EVO:** Mulebot.
- Optional Rumbler Spec-Ops can take a normal Hacking Device when that mode is enabled.

### Network / projection

- **Pitchers:** Danavas; Laxmee; Blocker profile 1; Hǎidào KHD.
- **Deployable Repeaters:** Fusilier FO; Guiláng profile 5.
- **Repeaters:** Peacemaker; Bulleteer; Fugazi; Pathfinder; Mulebot profiles 1/3.
- **Sensor:** Blocker; Pathfinder; Hannibal.
- **Guided:** Clipper profile 1.
- **EVO support:** Mulebot profile 2.

## Deployment / marker-state index

- **Combat Jump / Parachutist:** Tiger Soldiers; Cube Jäger; Blade-Ops profile 4.
- **Hidden Deployment:** Kunai Solutions Ninjas.
- **Camouflage / Infiltration:** Guiláng; Beasthunter profiles 2–3; Kunai also carries marker/Hidden Deployment tools.
- **Forward Deployment:** Peacemaker +20; Nøkken +20; Beasthunter profiles 2–3 +20; Blade profile 3 +20; Liang Kai +10.
- **Holomask:** Táowù.
- **Fast assault:** Carmen; Guijia; Peacemaker; Bulleteer; Liang Kai; Varangians; airborne Tigers.

## Vision-control and sensor index

- **Smoke:** Carmen Johns; Varangian Guard.
- **Eclipse:** Señor Massacre.
- **MSV2:** Nisse; Hǎidào MULTI Sniper profile.
- **MSV1:** Karhu; Guiláng; Nøkken profile 6.
- **Sensor:** Blocker; Pathfinder; Hannibal.

## Canonical Fireteam definitions

Current chart limit: **1 Core, 1 Haris, unlimited Duos** (`DUO: 256` source sentinel).

### FT-01 — Fusiliers Fireteams

**Types:** Haris, Core  
**Anchor:** Fusilier has source `min: 1`.

| Member | Unit ID | Required | Min | Max | Comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Fusilier | 1 | no | 1 | 5 | — | all |
| ORC | 5 | no | 0 | 2 | — | all |
| CSU | 122 | no | 0 | 2 | — | all |
| Blocker | 1750 | no | 0 | 1 | — | all |
| Táowù | 1538 | no | 0 | 1 | — | all |
| Rumbler Spec-Ops | 1925 | no | 0 | 1 | `Spec-Ops` | optional mode only |

### FT-02 — K2 Fireteams

**Types:** Duo, Haris, Core

The source has unusual raw semantics for the two principal rows: **Kaplan and Karhu are both `required:true` while both have `min:0`**. Preserve those fields exactly rather than inventing an anchor interpretation.

| Member | Unit ID | Required | Min | Max | Comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Kaplan | 338 | **yes** | 0 | 5 | — | all |
| Karhu | 1485 | **yes** | 0 | 2 | — | all |
| Beasthunter | 1570 | no | 0 | 1 | `FTO` | **profile 1 only** |
| Wild Bill | 1482 | no | 0 | 1 | — | all |

### FT-03 — White Company Fireteams

**Types:** Duo, Haris, Core

The source again uses `required:true, min:0` on its two principal rows. Preserve the raw representation.

| Member | Unit ID | Required | Min | Max | Comment | Profile restriction |
|---|---:|---|---:|---:|---|---|
| ORC | 5 | **yes** | 0 | 5 | — | all |
| Jujak | 1494 | **yes** | 0 | 4 | — | all |
| Nisse | 3 | no | 0 | 1 | — | all |
| Blade-Ops | 1751 | no | 0 | 1 | `FTO` | **profiles 1–2 only** |

### FT-04 — Chaksa Longarms Fireteams

**Types:** Duo, Haris

| Member | Unit ID | Required | Min | Max | Profile restriction |
|---|---:|---|---:|---:|---|
| Chaksa Longarm | 1310 | no | 1 | 3 | all |

### FT-05 — Varangian Guards Fireteams

**Type:** Duo

| Member | Unit ID | Required | Min | Max | Profile restriction |
|---|---:|---|---:|---:|---|
| Varangian Guard | 1461 | no | 1 | 2 | all |

### FT-06 — Anaconda Fireteams

**Type:** Duo

| Member | Unit ID | Required | Min | Max | Profile restriction |
|---|---:|---|---:|---:|---|
| Anaconda | 300 | no | 1 | 2 | all |
| Kaplan | 338 | no | 0 | 1 | all |

### Wildcards

| Unit | Unit ID | Counts as / comment | Max | Profile restriction |
|---|---:|---|---:|---|
| Hǎidào | 1246 | — | 3 | all |
| John Hawkwood | 1556 | `(Fusiliers)` | 1 | all |
| Liang Kai | 1500 | — | 1 | all |
| Shona Carano | 1505 | `(Varangian)` | 1 | all |
| Emily Handelman | 1072 | `(Fusiliers)` | 1 | all |
| Hannibal | 1345 | `(Orcs)` | 1 | all |
| Valkyrie | 1343 | `(Orcs)` | 1 | all |
| Laxmee | 1344 | — | 1 | all |
| Señor Massacre | 462 | — | 1 | all |

`Rumbler Spec-Ops` is **not** a global White Company Wildcard; it is an optional-mode member explicitly listed only in Fusiliers Fireteams.

## Unit → Fireteam access index

| Unit | Fireteam | Types | Access | Profile restriction | Notes |
|---|---|---|---|---|---|
| Fusilier | FT-01 | Haris/Core | native anchor | all | 1–5 |
| ORC | FT-01 | Haris/Core | native member | all | 0–2 |
| CSU | FT-01 | Haris/Core | native member | all | 0–2 |
| Blocker | FT-01 | Haris/Core | native member | all | 0–1 |
| Táowù | FT-01 | Haris/Core | native member | all | 0–1 |
| Rumbler Spec-Ops | FT-01 | Haris/Core | optional member | Spec-Ops mode | 0–1 |
| Kaplan | FT-02 | Duo/Haris/Core | K2 row | all | raw required=true, min0, max5 |
| Karhu | FT-02 | Duo/Haris/Core | K2 row | all | raw required=true, min0, max2 |
| Beasthunter | FT-02 | Duo/Haris/Core | FTO member | **profile 1** | 0–1 |
| Wild Bill | FT-02 | Duo/Haris/Core | native member | all | 0–1 |
| ORC | FT-03 | Duo/Haris/Core | White Company row | all | raw required=true, min0, max5 |
| Jujak | FT-03 | Duo/Haris/Core | White Company row | all | raw required=true, min0, max4 |
| Nisse | FT-03 | Duo/Haris/Core | native member | all | 0–1 |
| Blade-Ops | FT-03 | Duo/Haris/Core | FTO member | **profiles 1–2** | 0–1 |
| Chaksa Longarm | FT-04 | Duo/Haris | native anchor | all | 1–3 |
| Varangian Guard | FT-05 | Duo | native anchor | all | 1–2 |
| Anaconda | FT-06 | Duo | native anchor | all | 1–2 |
| Kaplan | FT-06 | Duo | native member | all | 0–1 |
| Hǎidào | Wildcard | permitted teams | Wildcard | all | max 3 |
| Hawkwood | Wildcard | permitted teams | Wildcard, counts as Fusiliers | all | max 1 |
| Liang Kai | Wildcard | permitted teams | Wildcard | all | max 1 |
| Shona Carano | Wildcard | permitted teams | Wildcard, counts as Varangian | all | max 1 |
| Emily Handelman | Wildcard | permitted teams | Wildcard, counts as Fusiliers | all | max 1 |
| Hannibal | Wildcard | permitted teams | Wildcard, counts as Orcs | all | max 1 |
| Valkyrie | Wildcard | permitted teams | Wildcard, counts as Orcs | all | max 1 |
| Laxmee | Wildcard | permitted teams | Wildcard | all | max 1 |
| Señor Massacre | Wildcard | permitted teams | Wildcard | all | max 1 |

If this reverse index ever conflicts with the canonical Fireteam tables above, the canonical tables win.

## Explicit no-access FTO label

`CLIPPER DRONBOT FTO` (Clipper profile 5) is labelled FTO in the source profile name, but the current White Company Fireteam chart contains **no Clipper row** and Clipper is not an explicit Wildcard. Do **not** infer Fireteam access from the profile label alone.

## Optional-mode units

### Rumbler Spec-Ops

**Unit ID:** 1925 · **Mode:** Infinity Spec-Ops · **Normal White Company status:** optional only.  
When Spec-Ops mode is enabled, one Rumbler may join **Fusiliers Fireteams**. It is not a global White Company Wildcard.

Current base options:
- `1` — 28 / 1 HMG.
- `2` — 28 / 1 AP Spitfire.
- `3` — 23 / 0 MULTI Rifle; Specialist Operative/GizmoKit.
- `4` — 26 / 0.5 AP Combi Rifle; Hacking Device.
- `5` — 23 / 0 MULTI Rifle/Flash Pulse; Forward Observer.
- `6` — 23 / 0 AP Combi Rifle; Paramedic.

### NA2 Team-Ops

**Unit ID:** 1939 · **Mode:** Team-Ops · **Normal White Company status:** optional only.  
Contains the NA2 Rumbler-1, Rumbler Heavy and Gort SpecBot Team-Ops profiles. It is not counted as an ordinary matched-play White Company roster entry and is not automatically substituted for Rumbler Spec-Ops in the Fireteam chart.

## Source relations

The current White Company `7.26246.159` source contains **no top-level relation records**. There are therefore no additional main/reinforcement identity constraints encoded at this layer beyond normal unit/character legality.

## Reinforcements boundary

Army links White Company to Reinforcement roster ID **999**. Reinforcement-only profiles, AVA and Fireteam permissions remain outside this Main reference. Do not merge Reinforcement Fireteam permissions into the Main chart above.

## Derived tactical index

This section is analytical and non-authoritative; source profile data and the canonical Fireteam chart above take precedence.

| Block / tag | Strong White Company candidates |
|---|---|
| Group 2 | Fugazi; Warcor; Mulebot EVO/TR; Sierra; Clipper; cheap Fusiliers; Cube Jäger waiting to deploy |
| Long-range attack | Gūijiă; Karhu Feuerbach; ORC HMG/Feuerbach; Nisse HMG; Anaconda; Scarface |
| Mid-range attack | Karhu; ORC/Jujak; Bulleteer; Nøkken; Wild Bill; Hannibal; Kaplan |
| Long-range ARO | Clipper ML; Karhu Feuerbach; Nisse sniper; Hǎidào MSV2 sniper; Chaksa Autocannon/ML; Sierra TR; Fusilier ML/sniper; Jujak ML |
| Mid-range ARO | Chaksa Mk12; Blocker; ORC/Jujak; Wild Bill; Kaplan HRL |
| Close assault | Liang Kai; Shona; Valkyrie; Señor Massacre; Varangians; Carmen; Beasthunters |
| Specialist | Danavas; Karhu Engineer/Paramedic; Yīshēng; ORC HD; Laxmee; Blade Engineer; Fusilier HD/FO/Paramedic; Mech-Engineer; Guiláng HD/FO; Jujak Engineer; Blocker; Pathfinder; Hǎidào KHD/Engineer/CoC; Nøkken HD/KHD/FO; Kaplan Engineer/Doctor/SO; Tiger HD/Paramedic; Nisse HD/Paramedic |
| Cheerleader | Fusilier; Fugazi; Warcor; Mulebot |
| TAG + support | Gūijiă, Anaconda or Scarface + Mech-Engineer/Yáozăo/Karhu Engineer/Hǎidào Engineer |
| REM + support | Bulleteer/Peacemaker/Pathfinder/Sierra/Clipper/Fugazi/Mulebot + Engineers |
| DZ defense | Sierra; Mulebot TR; Clipper; Fusilier ML/sniper; Chaksa; Hǎidào/Nisse sniper |
| Midfield defense | Guiláng; Nøkken; Peacemaker; Beasthunter; Blade profile 3 |
| Midfield specialist | Guiláng FO/HD; Nøkken FO/HD/KHD; Blade Engineer; Peacemaker/Pathfinder support |
| Warband | Varangian Guard; Carmen; Liang Kai; Shona; Valkyrie; Señor Massacre |
| Airborne troops | Tiger Soldiers; Cube Jäger; Blade profile 4 |
| Enemy-DZ attacker | Tigers; Carmen; Liang Kai; Nøkken; Peacemaker; Bulleteer |
| Network projection | Danavas/Laxmee/Blocker Pitchers; Fusilier/Guiláng deployable repeaters; REM repeaters |
| Vision control | Varangian/Carmen smoke; Señor Massacre Eclipse; Nisse/Hǎidào MSV2 exploitation |
| Hacker | Danavas HD+; Laxmee HD+; ORC/Fusilier/Blocker/Guiláng/Nøkken/Tiger/Nisse HD; Mulebot EVO |
| KHD | Hǎidào; Nøkken |
| Tech-counter | Blocker/Pathfinder/Hannibal Sensor; Engineers; Hǎidào/Nøkken KHDs |
| Guided package | Clipper Guided ML + FO/Spotlight network |
| Baggage support | Mulebot |

## Source-normalization and validation notes

- Standard roster count is **44 normal entries + 2 optional-mode entries**.
- Generic `merc-*` catalogue objects with empty `factions` arrays are excluded; explicit faction-`909` guest/mercenary entries are retained.
- Source `DUO: 256` is normalized as effectively unlimited Duos.
- Fusilier, Chaksa Longarm, Varangian and Anaconda anchors use positive source `min` values with `required:false`; those minimums are preserved.
- K2 rows for Kaplan and Karhu use the unusual combination `required:true, min:0`; those raw facts are preserved rather than normalized into a guessed anchor rule.
- White Company rows for ORC and Jujak also use `required:true, min:0`; preserve the source representation.
- Blade-Ops Fireteam access is **profiles 1–2 only** (`BLADE FTO`). Profiles 3–4 do not inherit it.
- Beasthunter K2 access is **profile 1 only** (`BEASTHUNTER FTO`).
- Clipper profile 5 is FTO-labelled but has no current chart row; no Fireteam access is inferred.
- Rumbler Spec-Ops is not a global Wildcard; it is an optional member of Fusiliers Fireteams only.
- The current source has **no relation records**.
- Main and Reinforcement roster `999` remain separate.

## Tactical research — White Company (reviewed 2026-10-23)

**Tactics, not roster authority.** Sources [S1] and [S2] are N5 faction-first reviews; [T1]/[T2] are **actual N5 tournament reports** (some event-specific rules or missions); [P1] is a 2024 N4 podcast and is historical. [G1] is shared PanO/REM analysis; [Y1] covers shared Yu Jing heavy TAGs; [A1] is later opposing Anaconda commentary. The **N5.3 Army 7.26246.159 profiles and canonical Fireteam chart above override all video/podcast list examples**, particularly when October 2025 and later balance changes or sectorial availability differ.

### WhiteCo in one page — specialist combined-arms, not just a shooter Core

| Plan | Why it works | Main trade-off |
|---|---|---|
| **Vision-control sniper package**: Hǎidào MSV2 MULTI sniper (29/1.5) + Hawkwood K1 sniper (35/1), Danavas/Laxmee White Noise, Varangian/Carmen smoke | Present **two distinct FtF solutions**: shoot through smoke with MSV2, or through White Noise using a non-MSV K1 shooter. A backup sniper means losing the first ARO does not collapse the entire game. [S1, T1, T2] | Multiple SWC guns and supporting hackers/smoke cost slots. Hǎidào/Hawkwood Wildcards are **not unrestricted Fireteam anchors**; the base formation's chart still applies. |
| **K2 precision team**: Karhu Feuerbach (34/1.5) + Karhu Engineer (25/0), or Kaplan Engineer/Doctor | Karhu bring **MSV1, Mimetism(-3), NCO, Climbing Plus**; the Feuerbach handles armor and long range, the Engineer provides D-Charges/classified work and durability support; Kaplan has **WIP14** repair/Doctor options and cheap Blitzen/adhesive tools. [S1, P1, T1] | Karhu are fragile one-wound platforms; their **NCO is wasted without an LT-order plan**. K2 needs its actual Kaplan/Karhu source conditions; it is not a general Wildcard team. |
| **White Company mixed HI team**: ORC HMG or Jujak Spitfire + Nisse / Blade FTO + Laxmee/Hǎidào | ORC **ARM4/2W** frontliner, Jujak **templates/engineer**, Nisse **MSV2**, Blade-Ops **Tactical Awareness 20–23/0**, and strong Wildcard hackers/CC give a flexible durable attacker. [S1, S2, T2] | Expensive and Hackable. **Blade FTO only options 1–2**; Nisse is **one native slot**; Laxmee/Fairy Dust may help but is not a reason to expose the whole team to repeaters. |
| **Fusilier / Hawkwood support Core** | 10pt Fusiliers, FO/deployable repeater, Hacker and **Hawkwood (counts as Fusilier)** build an affordable order base around a real K1 sniper and flexible CoC/extra-LT-Order alternatives. The actual Fusilier anchor enables a useful link without five weak gunfighters. [S1, S2, T1] | **At least one actual Fusilier is required**. The 40pt Hawkwood Chain of Command choice and 35pt K1 sniper are different loadouts; the long-range threat cannot simultaneously provide every LT/CoC option. |
| **Assault + screen**: Varangian + Shona Duo, Carmen, Liang Kai, Valkyrie, Señor Massacre | Varangian smoke gains reliable Fireteam dice in a **legal Varangian + Shona Wildcard Duo**; Shona and Liang Kai have high-penetration CC, while **Señor Massacre Eclipse** ignores many MSV answers. [S1, T1, T2] | Best at removing screened/overextended targets, not replacing long-range guns. **A Varangian in a Duo forgoes using its Impetuous Order normally**; do not automatically link it if the free Impetuous smoke is the priority. |
| **Midfield and hacker lattice**: Guiláng/Nøkken/Peacemaker + Laxmee/Danavas/Hǎidào KHD + optional Clipper | Guiláng Camo/Infiltration, Nøkken FD+20/Mimetism(-6), Peacemaker FD+20/Auxbot and Pitchers/Repeaters create **overlapping reveal/template/Spotlight threats**. The **16/1.5 Guided Clipper** converts Targeted into reach on bunkered enemies. [S1, S2, G1] | This is an **option**, not an obligation: unlike top hacking factions, every Guided play costs SWC, repeater/Spotlight Orders, a specialist and a vulnerable REM. WhiteCo can often solve the same target with smoke/K1/Tiger. |
| **TAG + mobile engineer**: Gūijiă / Scarface / Anaconda with Kaplan/Hǎidào/Mech support | TAGs buy an independent active-range problem solver; different profiles trade **durability, bundled engineer, price and legal Duo support**. [S1, S2, G1, Y1, A1] | Hard commit in a roster where the **K2, snipers, mobile specialists and Wildcards** are already very good. Pick the TAG for a mission/table, not because WhiteCo requires one. |

**What to test before submitting a list:** one hard ARO solution, one attacker that can continue after it dies, **two reliable objectives** (one forward-accessible), safe anti-hacker coverage, smoke *or* White Noise when relying on it, a credible route to enemy DZ, and enough Regular Orders. [T1/T2] showcase strong tournament lists with **very little deployed midfield**: fine on the right mission pack, but a liability when central consoles must be pressed early.

### Best units with an explicit why — including the anti-case

- **Hǎidào (24/0 CoC; 22/0 KHD+Pitcher; 25/0 Engineer; 29/1.5 MSV2 sniper):** NWI/Shock Immunity plus **Wildcard AVA3** puts meaningful specialists in otherwise awkward teams. MSV2 sniper exploits smoke; KHD+Pitcher defends/extends the hacker net; CoC protects a forward ORC/Gūijiă/Hawkwood LT. **Counter:** each is a distinct profile: the 29pt sniper does **not** carry CoC/KHD/Engineer, and paying for several Hǎidào eats real points despite their strong individual value. [P1, S1, S2, T1]
- **John Hawkwood:** **35/1 K1 sniper** is the efficient long-range killer; **40/0 CoC+Combi(+1B)** is a more expensive flexible LT safety net; **35/1 LT** and **39/1 LT+1 Order** help a list use Lieutenant Orders. He is a Wildcard that **counts as Fusilier**, so a Fusilier-supported sniper Core can solve heavy armor without expensive ORC guns. **Counter:** a single Hawkwood has a huge target on him; plan the backup sniper/specialist. [S1, P1, T1]
- **Karhu versus Kaplan K2:** **34/1.5 Karhu Feuerbach** supplies anti-TAG reach, MSV1 and Mimetism; **25/0 Karhu Engineer** supplies D-Charges and NCO while keeping a K2 team advancing for classifieds. **25/0 Kaplan Engineer** trades Karhu's stronger shooter package for **WIP14 and BTS6/Mimetism(-3)**; **24/0 Kaplan Doctor** is a good backup in a K2 team with expensive attack pieces. [S1, T1, T2] **Opposing opinions:** [P1/S1] enjoy aggressive Karhu links, while [S2] warns that needing other K2 units to unlock bonuses can make niche choices such as Wild Bill inefficient. Don't turn “K2” into a mandatory 5-man commitment.
- **ORC / Jujak / Nisse / Blade:** **ORC 34/1.5 HMG, 29/0 Firewall(-3), 33/0.5 HD** buys durable mid-long pressure. **Jujak 29/0 Engineer, 27/0 Firewall(-3), 31/1.5 Spitfire** adds templates and tech support. **Nisse 29/1.5 MSV2 sniper or 31/1.5 HMG** suppresses smoke and Mimetism lanes. **Blade FTO 20/0 shotgun or 23/0 Engineer** brings Tactical Awareness and Mimetism in the White Company Fireteam. **Counter:** high exposure to hacking and high price of a full mixed Core; [S1] argues WhiteCo still chooses between **high-modifier Karhu** and **durable HI** rather than obtaining both benefits in a single all-purpose piece.
- **Laxmee vs Danavas:** **Laxmee 24/0.5 HD+ (Fairy Dust upgrade), Pitcher, Mimetism(-3), Cybermine/Minelayer** is a **Wildcard** and helps protect Hackable formations and cover White Noise targets. **Danavas 22/0.5 HD+ with upgraded Oblivion and Pitcher** is a cheaper separate backline hacker, **not a Wildcard**. [S1] says Laxmee is an almost universal high-value toolkit; [S2] also likes the hacker network, but **counter:** 46pts/1SWC for both is too much unless the second HD+ is creating repeaters/control the army will actually use.
- **Guiláng vs Nøkken:** **27/0 Guiláng FO**, **25/0.5 Minelayer/Deployable Repeater**, **31/0.5 HD** get real **Infiltration, Camo, MSV1**. **22/0 Nøkken FO**, **25/0 Nøkken KHD**, **27/0.5 HD** instead bring **FD+20, Mimetism(-6), Bangbomb/Transmutation** and short-range guns; no Guiláng-style Infiltration. [S2] strongly prefers Guiláng for objectives and protection; **counter:** cheaper 22pt Nøkken FO or 25pt KHD pays for itself when its Mimetism and immediate short approach are the actual mission needs. [T1/T2] explicitly warn that 25–31pt midfield specialists can be squeezed out by the beautiful gun/vision tools.
- **Peacemaker / Bulleteer:** **Peacemaker 23/0 FD+20 Heavy Shotgun/Pulzar+Auxbot** creates three simultaneous corner/repeater/template problems; **24/0.5 alternate Minelayer Auxbot package** can establish an extra initial mine screen; **27/0 boarding shotgun(+1B)+Auxbot** buys a more direct assault, while **23/0 boarding-shotgun variant lacks Auxbot**. [S2/G1] value forward denial rather than raw Kills. **22/1 Bulleteer Spitfire Mimetism(-6)** is a compact high-mod assault REM; **19/0 heavy shotgun(+1B)** helps close-range clearance. **Counter:** unlike NCA, **Bulleteer/Peacemaker are not WhiteCo Wildcards or Fireteam members**, so their great gun needs Regular Orders and independent repair/positioning.
- **Smoke/CC choices:** **12–13pt Varangians (AVA2)** offer smoke, Irregular Orders and template/CC trade; **22pt Shona Wildcard** counts as Varangian and increases smoke reliability in legal Duo. **17pt Carmen+Bâtard** is a forward motorcycle attack/smoke package. **21pt Liang Kai Wildcard** is fast Super-Jump/EXP CC, **28–33pt Valkyrie counts as ORC**, **25–27pt Señor Massacre Eclipse** is the MSV-proof approach. [T1/T2] make convincing use of **Shona+Varangian**; [S1] notes unlinked Impetuous smoke can be more order-efficient when you don't need Duo bonuses.
- **Tiger vs Cube Jäger / Blade AD:** **20/0 Tiger Boarding Shotgun**, **26/0 Tiger Paramedic**, **29/0.5 Tiger HD**, Combat Jump/Parachutist, Super-Jump and Mimetism(-3): strong unexpected rear angle and late objective reach. **15/0 Cube Jäger Paramedic** is cheaper but only Parachutist and less gunfighting; **Blade option 4 Parachutist (30/0)** is a solo Engineer with FD/Decoy alternative profile and **cannot link**. **Counter:** too many off-board troops leave midfield under-defended going second. [P1, T1, T2]
- **Hannibal, Táowù, Emily and LT insurance:** **Hannibal LT 31/0 or 37/0.5** offers Strategos L1/TacAware/Counterintelligence but is a more expensive deployment-dependent command platform; **Táowù 21/0.5 CoC** offers Holomask/Counterintelligence as a native Fusilier-family member; **Emily 28/0 CoC/E/M GL** or **Hǎidào 24/0 CoC** are alternate routes. WhiteCo has many legal **CoC options**, unlike several other NA2 sectorials. Choose one when your LT is actually at risk; stacking several wastes points. [S1, S2]
- **Fusilier/CSU/Blocker:** **10/0 Fusilier LT or regular**, **12/0 FO deployable repeater**, **15/0.5 HD** fill economical native Fusilier Core/Haris. **11–13pt CSU Specialist** provides a cheap native specialist; **15/0 Blocker Specialist with Pitcher** adds Sensor/Biometric Visor/repeater projection; **19/0.5 Blocker HD has a Firewall upgrade but does NOT also have the Pitcher of its other profile**. [S2] initially questions Blocker's pure bonuses; **current chart grants native Fusilier-family access, not an unconditional “counts as Fusilier” purity equivalence**, so distinguish membership from all-pure composition. [S1]
- **Chaksa Longarms and Wild Bill:** [S1] dismisses Longarms in many lists as overcosted for the available competition; **29/1.5 portable autocannon**, **24/1.5 ML** and **25/0 Mk12** can nevertheless cover lanes or function as an independent **Duo/Haris** when your Core/Haris choices permit. [S2] thinks **Wild Bill (22–24/0)** needs compatible K2 buddies to benefit from bonuses, which often pushes more self-sufficient guns off the roster. **Neither is a mandatory trap nor a default efficiency pick**; assess a real lane/mission.
- **Irregular/Regular and team-slot budgeting:** 1 Core, 1 Haris, unlimited **legal Duos**, **not two Haris** (the early reaction [S2] mentions the old limit incorrectly). Rumbler optional Spec-Ops cannot be added in standard mode. Preserve the **K2 Kaplan/Karhu and WhiteCo ORC/Jujak raw required=true/min=0** ambiguity rather than inventing an anchor rule; other source minimums apply exactly.

### TAG, REM and Vehicle audit — only what White Company actually fields

| Current WhiteCo unit | Why you might take it | Cost, risk and opposing views |
|---|---|---|
| **Gūijiă TAG (AVA1)**: **77/1.5 MULTI HMG+HFT**; **77/2 LT** | Independent **Tactical Awareness, Super-Jump and strong MULTI HMG** for longer ranged attacks; 77pt chassis does not need a Fireteam. The 2SWC LT variant provides an LT Order but makes your most exposed piece a dangerous LT target. [S1, S2, Y1, G2] | [Y1] regards Gūijiă as *viable but merely average* compared with efficient Yu Jing HI: paying for TAG/CC/Super-Jump without an exceptional FtF modifier. [S2] is more positive about Super-Jump and the specialist **Shàngdiào ancillary**, but WhiteCo already has Karhu/Hawkwood and other ranged guns. Not a native WhiteCo Fireteam member. |
| **Scarface + Cordelia composite TAG (AVA1)**: **76–80/1.5 TOTAL** | Multiple TAG ranged/AP/assault options **plus bundled Engineer Cordelia** in the one legal purchase; [S1] calls the shooting and support excellent and likens its TAG-body value to a discount Gūijiă. [G2] TAG panel agrees Scarface adds a useful NA2 attack style. | **Critical pricing correction:** some videos compare a **roughly 58pt TAG chassis** against **77pt Gūijiă**, overlooking the mandatory **76–80pt Scarface + Cordelia complete selection**. On list cost, the package is **not ~20pt cheaper**; it brings its own Engineer instead. [S2] feels stronger WhiteCo guns reduce its necessity. **No Scarface/Cordelia Fireteam row here**, even if other NA2 factions allow one. |
| **Anaconda TAG (AVA2)**: **59/1.5 AP Spitfire+HFT+AP Thunderbolt** or **59/1.5 HMG+shotgun+Panzerfaust** | **Tactical Awareness, Warhorse, ECM Guided, Escape System/Operator**; **legal Anaconda Duo** can take **another Anaconda or a Kaplan**. **Kaplan Engineer 25/0** is a natural support partner and covers objectives; AP Spitfire/HFT protects near-midfield zones. [S2, A1] | **Contested:** [S1/S2/G2] early reviews call Anaconda suboptimal compared with WhiteCo's better shooters/TAGs; **later [A1] October 2025** argues its N5 AP resilience, Warhorse, improved Operator and linked Engineer can make it a durable anchor. **But [A1] uses StarCo's Armored Haris with Digger; WhiteCo has ONLY Anaconda Duo with Kaplan**. Never import the StarCo Haris bonus into WhiteCo. |
| **Clipper (AVA2)**: **16/1.5 Guided Missile Launcher**; **19/1.5 FTO-labeled ML** | **Actual Guided** Clipper option 1 converts Targeted from Danavas/Laxmee/Hǎidào Pitcher, Guiláng deployable repeater or Fusilier FO. Multiple ways to build the network. [P1, S2] | **WhiteCo has no Clipper Fireteam row**, including option 5 despite the FTO label. Do **not** describe the FTO as “linked Guided” or assume it has Guided; it is different from the 16pt source skill profile. Clipper only wins when target acquisition costs fewer Orders than sending Tiger/K1/Mimetism attackers. |
| **Peacemaker (AVA2)**: **23/0 HSG/Pulzar+Auxbot**, **24/0.5 minelayer Auxbot**, **23/0 no-Auxbot shotgun**, **27/0 shotgun(+1B)+Auxbot** | **FD+20/Mimetism(-3), repeater**, simultaneous template/trigger angles and disposable Auxbot challenge infiltrators; [S2/G1] especially like the minelayer Auxbot for board denial going second. | 0.5SWC option fights with long guns for SWC, and not every Peacemaker profile comes with Auxbot. **No Fireteam access**; the relevant PanO/NCA support options are not automatically available in WhiteCo. |
| **Bulleteer (AVA2)**: **22/1 Spitfire**, **19/0 HSG(+1B)** | **Mimetism(-6) and Repeater** produce fast low-cost attack angles without committing ORC/TAG; Spitfire is especially useful after enemy discover/ARO layer thins. [S2, G1] | **No WhiteCo Fireteam membership**; a solo 1STR chassis can be removed by a template, direct damage or hacked through repeater coverage. In **Neoterra [G1]** other Fireteam/racer support exists—do not import it.
| **Sierra (AVA2)**: **23/1 Total Reaction HMG**, **18/0 TR Thunderbolt(+1B)** | 360º defensive long-lane ARO; **18/0** is the best SWC-neutral choice when sniper/TAG/Clipper consumes the SWC budget. [S2, T1, G1] | **STR1** and no Fireteam access. Pair with repair and stagger threats; two exposed Sierras can simply be killed sequentially.
| **Pathfinder (AVA2)**: **14/0 FO/Sensor/Triangulated Fire**, **17/0 Tactical Awareness** | Objective/anti-Camo work, repeater and **extra Tactical Awareness movement/mission action** for 3 additional points. Valuable when a TAG/sniper roster has too few forward specialists. [T2, G1] | **Not a Wildcard or Fireteam member here**, despite [G1] discussing linked Pathfinder in other PanO sectorials. Cannot replace Guiláng's actual Infiltration/Camo.
| **Fugazi (AVA3)**: **7/0 Flash Pulse Repeater** | Cheap **Regular/Mimetism(-3) Flash Pulse** and distributed repeaters; order base + board defense in one slot. | Fragile; spending all three slots on bots makes the objective force sparse unless the rest of the list scores.
| **Mulebot (AVA2)**: **8/0 Baggage/Repeater**, **14/0.5 EVO**, **17/0 Total Reaction Combi** | Resupply/support, cheap Regular Order; EVO is sensible with **Bulleteer/Peacemaker/Sierra attack plan** or other relevant supportware. [G1] | EVO is optional; buying it with only one eligible solo attack REM is often a bad opportunity cost; **not a WhiteCo linked support bot**.
| **Yáozăo (AVA2) / ancillary Auxbot, Shàngdiào, Bâtard, Anaconda Operator, TurtleMek/Cordelia forms** | **3pt Yáozăo Servant** extends repair/medical reach; constituent/peripheral pieces improve attached unit's capabilities. | **Do not add ancillary/Servant/disabled constituent states as separately purchasable main-roster entries.** They have different activation and Order rules: **Cordelia is an included Engineer in the Scarface composite, not automatically a no-Order Peripheral**. Check the constituent-order rules in Army; don't equate all included models with Fugazi/Servant bots.

**VH check:** Among the **44 current standard WhiteCo entries there is no Vehicle-class (VH) troop**. **Carmen's motorcycle remains an Irregular/Impetuous biker profile**, not VH; **Gūijiă, Scarface, Anaconda are TAGs**, not Vehicles. REMs and their subordinate/peripheral forms are enumerated above. Do not import a different PanO/Yu Jing Vehicle or TAG on the theory that shared-REM videos imply roster access.

### Disagreements and rules traps to preserve

1. **What's WhiteCo's true strength?** [S1] calls N5 a significant improvement because it now has *both* durable HI/TAG and high-mod shooting plus strong CC/hacking. [S2] sees a roster with standout Wildcards and many **competing expensive gun pieces** rather than a singular best list. [T1/T2] prove viable *vision-control combined arms* in event play but also document the problem of **no affordable midfield**. Build to the actual scoring pack.
2. **Gūijiă vs Scarface:** [S1] views Scarface as a cheap near-Gūijiă *chassis*, [S2] prefers the better overall WhiteCo guns and sometimes the Gūijiă; [G2/Y1] see neither as automatic top-tier. **At 76–80 versus 77 complete list points** there is not a ~20-point discount; decide whether you need Cordelia or Super-Jump/standalone Tactical Awareness.
3. **Anaconda is not unanimous rubbish:** [S1/S2/G2] dismiss its raw shootout value, but [A1] describes a viable **Warhorse/AP-immune TAG + Engineer** plan in N5. WhiteCo's **Kaplan Duo**, rather than StarCo's Engineer+Digger Haris, is the only native TAG Fireteam option for it here.
4. **Fusilier five-piece or short links?** [S1] can justify a **Hawkwood/Fusilier Core** because the sniper and supporting specialists share useful advantages; [S2] likes many small Duos/teams for order economy. [T1/T2] use linked snipers/vision control for redundancy but acknowledge midfield-objective deficits. No free assumption that adding Wildcards makes the composition pure.
5. **Guiláng vs Nøkken:** [S2] argues Guiláng Infiltration/Camo beats a Nøkken forward specialist for most objective missions; **Nøkken FO 22/0 or KHD 25/0** is still credible when saving points and Mimetism(-6)/trading matter. Both are priced significantly above cheap order fillers.
6. **Guided Clipper vs direct force:** [P1/S2] consider Danavas/Laxmee/Guiláng+Clipper legitimate; [S2] stresses good Hǎidào/Karhu/K1/Tiger/Peacemaker routes may not need Guided overhead. **FTO Clipper does not link**, and its 19pt profile is not the source's 16pt Guided profile.
7. **Source Fireteam gates:** **K2** Kaplan/Karhu required=true/min=0 source semantics, **White Company** ORC/Jujak ditto; don't guess anchors. **Fusilier at least one** for that family; **Blade FTO options 1/2 only** in White Company; **Beasthunter FTO option 1 only** in K2; **Anaconda Duo only with Anaconda/Kaplan**; other Wildcards join only otherwise-legal teams. **1 Core, 1 Haris**, despite [S2] early speech about two Haris. **Clipper FTO no access**. No other unit gains membership solely from “FTO” in the name.
8. **Avoid tournament-rule contamination:** [T1/T2] involved **Reinforced Command / Stealth Operations and special mission formats**. A player's sample list and unusual strategic choice must be checked against **normal N5.3** Fireteams/LT loss, not imported without the event conditions.

### Best videos, podcasts and transcript provenance

**Sectorial-focused — highest priority**
- **[S1] [Robert Shepherd: Infinity N5 Faction Focus — White Company](https://www.youtube.com/watch?v=y-iuVDPJ-Y4)** (March 2025). **YouTube MCP transcript read**. Strongest comprehensive N5 thesis: resilience/one-wound dilemma, Hawkwood-Fusilier team, Karhu/Kaplan links, 2025 unit value, Gui Jia vs Scarface, hacking and Mimetism.
- **[T1] [Infinity the Dante: Winning* a Tournament with WhiteCo — Arcfinity 2025](https://www.youtube.com/watch?v=hiLOsN7c7zE)** (May 2025). **YouTube MCP transcript read**. Five-round evidence and *why* **Varangian+Shona Duo**, two alternate sniper solutions, White Noise/smoke, specialist coverage and support engineers work; admits its core problem with quick midfield buttons. Check event-specific rules.
- **[T2] [Infinity the Dante: N5 Tournament Report with WhiteCo](https://www.youtube.com/watch?v=8Jp2CJjIlo4)** (April 2025). **YouTube MCP transcript read**. Three-round mission-specific insight on ORC/Valkyrie/Nisse/Laxmee team, K2 Karhu+Kaplan engineer/doctor and Tiger AD objective coverage; describes **few forward midfield specialists**.
- **[S2] [Infinity the Dante: White Company N5 Initial Reaction — RIP ForCo…Unless?](https://www.youtube.com/watch?v=UwgmSkVnrpI)** (January 2025). **YouTube MCP transcript read**. Best strongly contrasting video on TAG value, Nøkken vs Guiláng, Peacemaker/Auxbot mine-layer and why not to force WhiteCo to play every returning Foreign Company unit. Early-edition, not all current details correct.
- **[P1] [WIP12 E160 — White Company](https://open.spotify.com/episode/7zbcLwKEZXivvhDwutJba0)** (2024-06-18). **Podcast MCP 2,102 transcript lines read**. Strongest dedicated historical long-form: WhiteCo identity **~0–15min**, Tiger Soldiers **~30min**, hacking **~35–42**, Peacemaker **~44–49**, Fusiliers **~62**, Karhu/Kaplan **~78–84**, Clipper **~85**, Hawkwood **~93** and Gūijiă **~97–100**. **N4 profile and Fireteam claims are not N5 rules.**
- **[WIP12 E40](https://open.spotify.com/episode/106hZTXyerr2WbCXtSvXun)** and **[E41](https://open.spotify.com/episode/5x7yabWlyBiN1OFXqBqYHs)** (2022). Found in Podcast MCP **but both transcripts unavailable**; N4 historical archives, not used to support claims.

**Shared TAGs/REMs — do not import related sectorial Fireteams**
- **[G2] [Loss of Lieutenant E142: N5 TAG Tier List](https://www.youtube.com/watch?v=dZo_gQWQYSY)**; [Spotify](https://open.spotify.com/episode/1h5CJfZC5zBPxdg66o7xIN) (2025). **YouTube MCP transcript read**: debates **Gūijiă's price for generic BS/CC**, **Scarface's Cordelia bundle**, and **Anaconda's mediocre raw FtF**; global ranking, not WhiteCo-specific mission verdict.
- **[A1] [Loss of Lieutenant E158: Return of the Lost Sectorials Part 2](https://www.youtube.com/watch?v=EoQ3Ma7Hp7k)**; [Spotify](https://open.spotify.com/episode/1pQ6J6OGpzyu8QlxiFoo8D) (Oct 2025). **YouTube MCP transcript read**: later contrary Anaconda appreciation in **StarCo**, with AP immunity, Warhorse and Engineer-based link. **WhiteCo lacks that StarCo Haris**, so transfer only general TAG lessons.
- **[G1] [Robert Shepherd: N5 PanOceania Faction Focus](https://www.youtube.com/watch?v=IqK-RwFt7fw)** and [N5 Neoterra Focus](https://www.youtube.com/watch?v=axa19k7qE1E). **Both YouTube MCP transcripts read**: Peacemaker Auxbots/minelayer, Pathfinder TacAware specialist, TR/remote and relevant supportware. **Neoterra can link units WhiteCo cannot**.
- **[Y1] [Robert Shepherd: N5 Yu Jing Faction Focus](https://www.youtube.com/watch?v=mn4yHSNxsnA)** and [Invincible Army Focus](https://www.youtube.com/watch?v=Lco3q6QmezY). **Both YouTube MCP transcripts read**: generic TAG vs HI value, hacking pressure and some shared Yu Jing troop use. **Other Yu Jing Fireteams are not WhiteCo rules**.
- [2026 White Company community research index](https://forum.corvusbelli.com/threads/n5-recap-white-company-tacticas.43665/) links further material, including a **January 2026 German WhiteCo report**; its full article was not accessible here, so no findings are attributed to unseen text.

**Method:** The transcripts occasionally garble “Gūijiă,” “Hǎidào,” “Karhu,” “Nøkken,” and “WhiteCo,” and older videos can describe profiles no longer available. All actionable prices, FTO eligibility, Wildcards and native Fireteam construction in this section are taken from **this file's pinned N5.3 roster** and checked against the source chart above, not copied blindly from video captions.

## Provenance

Validated against the pinned N5.3 Army-derived source on **2026-10-16**. If future Army revisions change roster entries, AVA, profiles, Fireteam chart semantics, optional modes or Reinforcement linkage, update this file and its `army_source_version`/verification metadata together.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Danavas HD+Oblivion upgrade/Pitcher 22/0.5** and **Laxmee HD+Fairy Dust/Pitcher 24/0.5** are the centerpiece value choice: **White Noise** supplies critical anti-MSV access to PanO/Yu Jing shooters. **Hǎidào KHD+Pitcher 22/0** provides cheap lethal anti-Hacker protection for a current legal mixed HI team; **Nøkken KHD25/0** adds FD+20/Mimetism(-6) scoring, **Guìláng HD31/0.5** Camo/Infiltration network access. **Fusilier HD15/0.5** is the minimalist second HD. **Why:** a single Danavas/Laxmee and Hǎidào gives complementary HD+/KHD coverage; buying *both* HD+ profiles may be redundant unless their specific White Noise/Fairy Dust/weapon support is used. Never import native PanO/NCA TinBot or Fireteam access.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

See the N5.3 [cross-game apex/value rankings and transcript-backed competing assessments](../../notes/list-building/cheerleaders-and-order-generators.md). The current roster and official Fireteam definitions above remain authoritative; unit access/cost may differ from vanilla.

- 7pt Fugazi — fast Flash/Repeater bot; cheap Regular Order plus hacking relay if available.
- 8pt Mulebot — Baggage/reload Regular support, better than paying extra for an idle infantry filler on open DZ tables.
- 3pt Warcor — very useful Irregular Flash ARO/cheap screen, NOT an ordinary transferable Order.

**Selection rule:** Count deployed, transferable Regular Orders per Combat Group, not total models or restricted bonus Orders; choose the lowest-cost protected Regular profile that *also* contributes a relevant Repeater, Baggage, Fireteam, template, ARO or Specialist job. Check Group slots and DZ hiding space before buying a third large-base REM or replacing a needed scoring piece.


## ARO apex/value cross-reference (2026-10-23)

See [Best ARO Units in N5.3 — apex, cost-value, Hidden Deployment, reactive traps, opposed podcast views](../../notes/list-building/aro-units-apex-and-value.md). **Only the legal roster above** establishes options, exact costs/AVA, upgrades and Fireteam permissions in this army.

- **Guilang Camo mine/FO** — protects scoring approaches with uncertainty, forcing Discover or reroute before the core is exposed
- **Ninja hidden/camo** — anti-impersonation or corridor trap if positioned near scoring; may be more valuable unrevealed for own active turn
- **Sierra Thunderbolt TR** — 18pt/0SWC where authorized, all-arc cheap regular ARO and Engineer-restorable lane
- **Fugazi Flashbot** — 7pt Regular cheap Flash/Repeater tax; not substitute for anti-armor hard ARO
- **Warcor 3pt Flash** — token defensive tax/late game stun, Irregular so not a generic Order

**List test:** a strong ARO consumes enemy Orders by forcing Smoke, rerouting, poor range, discoveries or risky trades. A robust list normally prefers *serial, different* defenders—a cheap visible or marker/template screen, a covered second gate, and a preserved attack/scoring unit—rather than two adjacent visible snipers. Plan for opponent pie-slicing, AD, anti-camo, hacking and recovery; evaluate whether extra SWC is better spent on mission attackers.

## Command-unit apex/value cross-reference (2026-10-23)

**Hannibal LT 31/0 or 37/0.5** offers Strategos L1/TacAware/Counterintelligence type command utility without needing another expensive active LT; **Hawkwood LT(+1) 39/1** instead favors a productive ranged attack. **Hǎidào CoC 24/0**, **Táowù CoC 21/0.5**, **Emily Handelman CoC 28/0**, and **Hawkwood CoC 40/0** are distinct succession/utility purchases. Emily's CoC is **real in WhiteCo**, but not on her current **Kestrel** profile.

See [cross-game Lieutenant, CoC and Order-economy tiers](../../notes/list-building/command-units-apex-and-value.md). **Refer to this pinned roster/Fireteam chart for profile legality.**

## Mission specialist choices — N5.3 cross-game evaluation

**Hǎidào Engineer25/KHD22/CoC24** (when present as WhiteCo variants) combine NWI/support with legal-team mission presence; **Hawkwood CoC40** or **Emily CoC28** can provide succession *and* meaningful button/attack, not cheap insurance. **Danavas HD+22** where roster-legal handles White Noise/hacking from behind the attacker. Different roles and legal loadouts cannot be stacked in one model; use a separate quick Specialist when final console is away from the gun team.

See [Mission Specialists / Button Pushers apex and value tiers](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). This roster and its Fireteam chart are the final authority for exact options.

## N5.3 airborne / enemy-DZ profile and value choices (2026-10-23)

**Tiger Soldier BSG20/0, HD29/0.5 and Paramedic26/0** provide true Combat Jump/ordinary Parachutist backline pressure, trading BS13/Mimetism(-3) for landing risk. **Cube Jäger BSG15/0, E/Mitter SMG18/0** is cheaper ordinary edge Parachutist: disruptive late Classified/anti-tech role, not Combat Jump. **Blade-Ops Engineer Parachutist30/0** combines Decoy(2), E/Mitter and Tactical Awareness; **FD+20 Engineer30/0** is another loadout. **Kunai Hidden and Guilang Infiltration** offer on-table alternatives; **Haidao/Táowù/Emily CoC** protect an active LT but are separate choices.

[Cross-game N5.3 airborne/rear-strike apex-value and landing-risk tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **Use this roster and canonical Fireteam chart for exact legality.**

## Warband cheap trading / order economy — N5.3

**Varangian SMG+Chain+Smoke12/0, AVA2** is explicitly **Irregular+Impetuous in White Company**, unlike **O-12/Kosmoflot Regular** versions; assess as **self-funded Smoke/CC23/Dogged** rather than an extra pooled Regular Order. Current native **Varangian Duo** can put two along one lane; this is team movement utility, not guaranteed conversion of their printed Training. **Shona Carano** legal Wildcard counts as Varangian when selected, but is a premium combat character, not free. **Cube Jäger15** is separate late Parachutist scorer; **Hǎidào CoC24/Emily CoC28** are protected command roles.

[Current cross-faction warband apex/value, opponent counters, Lt/CoC packages](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). This faction's own pinned profile and Fireteam rows control legality.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Zhanshi Yīshēng14 WIP13** is the 65%-base budget VITA healer; **Mech-Engineer14 WIP13 + Yáozăo3** is the 17pt **Gūijiă/REM** repair line, rising from 65% to **87.75%** only with a qualifying Remote Presence target and Command Token. **Hǎidào Engineer25** brings NWI and Fireteam utility when a forward HI recovery route is needed. **Scarface & Cordelia** includes a dedicated companion Engineer, but her survival and path still matter. [Recovery support tiers and real success probabilities](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Varangian Guard12/0** buys strong **CC23/Berserk+Smoke/Dogged** *cheap trading*, but **White Company profiles are Irregular+Impetuous**—unlike Regular O-12/Kosmoflot Varangians, so do not assign free pooled Orders. **Kunai25–28 Hidden** is primarily concealed long-range shooter (**MA3 CC21**, not Mono/Infiltration); **Kaplan** and **Hǎidào** are versatile linked gun/specialist/engineering pieces, not premier duelists. Screen **Guijia/Scarface TAGs** with Warbands/Repeaters and deny stealth contact. Roster-legal named melee hero is not an automatic faction import. [N5.3 melee apex/value and counter-CC guide](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Beasthunter9/15 Panzerfaust/HFT**, **Nøkken22 Panzerfaust/FO**, **Kaplan20 Blitzen**, and **Karhu22 Blitzen or E/Marat** are affordable mixed electronic/lethal responses if their legal profile matches the link plan. **Karhu Feuerbach(+1B)** or **Chaksa Longarm Autocannon/ML** gives serious ranged can-opening; **Hawkwood K1 sniper** is an ARM=0 alternate at a meaningful SWC cost. **Cube Jäger15 Monofilament** has higher assassination swing if enemy TAG is accessible via flank. **WhiteCo Varangians12 are Irregular**, not automatic pooled Orders. [Non-hacking anti-armor apex/value, E/M and AP+EXP comparison](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Anaconda59/1.5** (STR3 ARM7 Warhorse TacAware/Transmutation) is very cost-effective **59VP quadrant swing**; only its **Operator alternate state is Specialist Operative**, not an ordinary TAG pickup. **ORC Hacker33/.5** W2 ARM4 is actual durable Specialist where selected; **Hǎidào Engineer25/0** NWI/Shock Immunity provides cheap recovery and box scoring, **KHD22/0** another close carry/hacker option. **Nøkken Hacking Device27/.5** Mimetism(-6)/FD+20 creates concealed approach but cannot carry as a Marker. **Scarface/Cordelia** is a paid pairing: engineer keeps armored zone denial active; don't count them as single 40pt holder. **Counter:** heavy Anaconda loses more objective tempo if opponent bypasses its firing lane; independent Hǎidào plus second cheap scorer can defend two quadrants.

[Cross-game holding and carrier apex/value, scenario rules and transcript disagreements](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Use pinned local roster/Fireteam chart.

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Pathfinder FO/Sensor14/0** and **Blocker Sensor/Biometric** are cheap **Camo/Hidden vs Impersonation** choices with different rules: Sensor sweeps ZoC Camo/Hidden, Biometric improves legal IMP-1 Discover. **Nisse MSV2** or **Hǎidào MSV2 sniper** is the *kill the Mimetism sniper* package; **Señor Massacre Eclipse** passes an enemy visor lane without a gunfight. **Counter:** Varangian ordinary Smoke still loses to hostile MSV; White Company Varangians are **Irregular**, unlike certain other rosters. Multiple MSV AROs invite White Noise/Albedo: preserve a non-visor gun or screened route.

[Full anti-tech N5.3 apex/value, exact mechanics, matchup selection and opposing transcripts](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## N5.3 peripheral / synchronized / multi-body apex-value update

**Peacemaker HSG+Auxbot23/0** and **HSG Minelayer+Auxbot24/.5** supply FD(+20)/native Repeater/Mim(-3)/synchronized HFT fork in midfield; **BSG(+1B)23/0** lacks Auxbot while **BSG+Auxbot27/0** restores the true dual-body attack. **Anaconda TAG59/1.5+Operator**, **Scarface+Cordelia** and similar compound listings are **not Synchronized or Control**: operator deploys only after valid Escape System condition; Cordelia is a separate actual Engineer/Order source as printed. **Engineer + Yáozăo Servant3/0** repairs ARM/STR at a distant position without exposing Controller and without second free Order. **Counter:** Peacemaker is better than solo 27pt ORC guarding a tight interaction square where HFT fork matters, ORC/Anaconda better if enemy dominates with long weapons or hacking disables REM.

[N5.3 Peripheral & Multi-Body apex/value tiers and transcript debates](../../notes/list-building/peripheral-synchronized-multibody-apex-value.md). Pinned source roster/Fireteam restrictions remain authoritative.

## Mission performance — battle-report evidence (2026-11-01)

| Mission(s) | Tested composition / scoring mechanism | Evidence |
|---|---|---|
| **Biotech 4 / custom Mega Turret / firelane control** | Varangian + Shona smoke/CC, Haidao MSV2 Sniper and Hawkwood K1 Sniper under White Noise, Laxmee hacking formed deliberately flexible attack/vision options. | [#010](../../notes/battle-reports/001-010-n5-battle-report-tactical-analysis.md) |
| **Highly Classified** | A second list emphasized real Specialist role diversity rather than copying the sniper/CC list; mission-packet selection drove event results. | [#010](../../notes/battle-reports/001-010-n5-battle-report-tactical-analysis.md), [#032](../../notes/battle-reports/031-040-n5-battle-report-tactical-analysis.md) |
| **Supremacy / zone or Annihilation** | The Haidao/Hawkwood fork and linked support deny long lanes, but movement and actually occupying objectives remain a cost. | [#010](../../notes/battle-reports/001-010-n5-battle-report-tactical-analysis.md) |

**Limits:** #010 is a single five-round recap with **Reinforced Command and custom Mega Turret** rules; #033 is duplicate coverage and must not be double counted. Game-era qualitative evidence, not a win-rate or current Fireteam claim. [Full mission evidence audit](../../notes/battle-reports/cross-report-mission-performance-by-sectorial.md).

## Counterplay — observed N5 battle-report responses (2026-11-02)

| Threat / target | Observed response and limitation | Battle reports |
|---|---|---|
| **Smoke/visor anti-ARO fork** | Varangian Smoke + Haidao MSV2 sniper, White Noise + Hawkwood non-MSV K1 sniper and Laxmee network provide alternate visibility lanes. | [#010](../../notes/battle-reports/001-010-n5-battle-report-tactical-analysis.md) |
| **Failure: exposed Hacker/link** | Combined long Pitcher + Bit/Kiss killed WhiteCo Fusilier Hacker, removed described link Sixth Sense and allowed Charontid to remove Hawkwood. | [#112](../../notes/battle-reports/111-120-n5-battle-report-tactical-analysis.md) |
| **Side-angle assassin** | Shona/Liang Kai/Tiger Soldier are alternate access against front sniper but Daturazi template traded into Hawkwood in a report despite his expensive gun. | [#010](../../notes/battle-reports/001-010-n5-battle-report-tactical-analysis.md) |

**Limit:** #010 uses custom event extras and #033 duplicates it; do not treat full White Company team as currently legal without Fireteam check. Game-era tactical evidence, not current N5.3 profile/Fireteam or faction win-rate claims. [Full cross-report counterplay analysis](../../notes/battle-reports/n5-cross-report-counterplay-tags-hi-hacking-camo-impersonators-fireteams.md).

---

## Must-have / Go-to / Avoid — source-backed recommendations (2026)

Dated source-backed tactical preferences and miniature purchasing priorities; opinions do not override N5.3 roster, profile or Fireteam data above.

**Original audit title:** NA2 mercenary sectorials — Must-have / Go-to / Avoid (N5.3)

**Audit date:** 25 October 2026. **Scope:** Druze Bayram Security, Ikari Company, StarCo Free Company of the Star, Dahshat Company, White Company. This companion to the other faction selection audits in this folder evaluates competitive **standard 300-point N5.3** lists. It does not import Reinforcement, optional Spec-Ops/Team-Ops, or a neighboring faction's Fireteam permissions.

**Authority order:** The five repository-native N5.3 sectorial references linked below are authoritative for available troops, particular profiles, AVA, points/SWC, and Fireteams (Army data 7.26246.159, 3 September 2026, verified 16 October). YouTube/podcast transcripts are evidence for **a speaker's opinion**, not a measured tournament inclusion rate or a guarantee of efficiency. Several sources predate N5.3; their strategic observations must be reconciled with the pinned roster. In particular, N5 fireteam changes invalidate some older linked Guided claims.

**Labels used here:**
- **Must / near-must:** An actual presenter's explicit almost-every-list recommendation, or a defensible near-universal list-building package. Near-must does **not** mean compulsory in every mission or list style.
- **Go-to:** Efficient, consistently defensible use of points, SWC, Order slots and a defined tactical job. The alternatives are often mutually exclusive.
- **Avoid / never take:** An **explicit reviewer rejection**, or a specific profile or construction displaced in its intended role by a better same-roster investment. Mark as **contested/conditional** when any credible niche or dissent exists. Do not invent categorical bans when only an older negative opinion is available.
- **Evidence:** **Direct** = explicit recommendation/rejection in a transcript; **Corroborated** = source rationale plus previously transcript-audited repository guide; **Contested** = meaningful opposing speaker's interpretation; **Edition-limited** = interpretation of pre-current Army data.

### Quick comparison

| Sectorial | Most defensible must / near-must | Reliable go-to choices | Strongest sourced avoid | Absolute never-take? |
|---|---|---|---|---|
| **Druze** | Druze **KHD + Pitcher** (direct repeated default) | Brawler HRL, Hunzakut FO, Valerya, Yuan Yuan, Digger, Scarface or Bulleteers | **Anaconda as default TAG** vs Scarface/Triphammer; ordinary Druze HMG value | No: Anaconda has a scenario/total-cost niche |
| **Ikari** | No single compulsory unit; **cheap Keisotsu regular-order base** and **Wú Míng AP HMG** are most convincing defaults | Motorized Yojimbo, Yuan Yuan/Desperado, Tankō, Armand, Druze KHD, Karakuri/Pathfinder | **Security Chief Arslan** as value pick (explicit rejection) | No |
| **StarCo** | **Al Hawwa' KHD**, **Irmandinho** (direct auto-take claims); **Knauf FTO + Uhahu** as a standout package | Brawler/Digger PMC, Bandit Minelayer, Hellcat Paramedic, Mobile Brigada LT, Riot Grrls/Avicenna | **Alguacil premium guns**; **unsupported TAG investment** (Anaconda itself contested) | No |
| **Dahshat** | **Mimetism(-3) Libertos** (direct strong 9-point profile default) | Hunzakut, McMurrough, Zúyŏng + Rui Shi, Valerya, Zhēnchá, Maghariba | Redundant **Al Fasid HMG** or ordinary **Ghulam HMG as main attack** | No |
| **White Company** | No proven single must; **Hǎidào's multi-profile Wildcard role** is a near-default toolbox | Hawkwood K1, Karhu/Kaplan, Laxmee, Varangian/Shona, Guiláng, Tiger, Peacemaker/Sierra | **Fusilier SWC guns as premium shooters**; niche Longarms/Wild Bill | No |

### 5. White Company

**Current reference:** [White Company N5.3](white-company.md). **Direct sources:** [W1: Robert Shepherd, Infinity N5 Faction Focus White Company](https://www.youtube.com/watch?v=y-iuVDPJ-Y4) (March 2025, full transcript reviewed); [W2: Infinity the Dante, Winning* a Tournament with WhiteCo](https://www.youtube.com/watch?v=hiLOsN7c7zE) (May 2025, tournament report transcript reviewed); [W3: Infinity the Dante, White Company N5 Initial Reaction](https://www.youtube.com/watch?v=UwgmSkVnrpI) (Jan 2025, full transcript previously reviewed); [W4: WIP12 E160, White Company](https://open.spotify.com/episode/7zbcLwKEZXivvhDwutJba0) (June 2024/N4, transcript retrieved; historical only). [Current White Company tactical review](white-company.md#tactical-research--white-company-reviewed-2026-10-23) records anti-cases and tournament limitations.

#### Must / near-must

- **No sourced universally compulsory individual unit.** White Company can meaningfully choose between K2 guns, Hawkwood/Fusilier defensive Core, ORC/Jujak heavy teams, direct TAGs, and Tiger/midfield-led mission plans. The sources endorse **packages**, not identical lists.
- **Hǎidào is the strongest near-default flexible family — Corroborated [W1,W2,W3].** Available as **24/0 Chain of Command**, **22/0 KHD+Pitcher**, **25/0 Engineer**, **29/1.5 MSV2 sniper** with NWI, Wildcard and strong team fit. **Do not pretend one Hǎidào profile simultaneously has all four jobs.** Whether any Hǎidào makes the final 15 depends on the chosen mission/link archetype.

#### Go-to

| Unit/profile | Why it is good | When to skip | Evidence |
|---|---|---|---|
| **John Hawkwood K1 sniper 35/1** | High-efficiency anti-armor shooting in Fusilier-supported pure Core; named primary recommendation | Heavy points/SWC lane commitment, LT/CoC choices are different profiles | W1 Direct |
| **Karhu Feuerbach 34/1.5 + Engineer 25/0 / Kaplan Doctor 24/0** | K2 firepower with MSV1/Mimetism, NCO/D-Charges or WIP14 Doctor healing | Overinvesting in 4–5 expensive K2 bodies crowds out midfield specialists | W1,W2,W3 |
| **Laxmee HD+ 24/0.5** | White Noise, Pitcher, improved Fairy Dust, useful Wildcard | Second Danavas/HD+ hacker rarely needed absent a genuine network plan | W1,W3 |
| **Varangian 12–13 / Shona Carano 22** | Smoke and cheap CC trades; can force favorable snipers/approach lines | Linking a Varangian may forgo its Irregular Impetuous move; some armies prefer solo smoke | W2 Direct tournament evidence |
| **Guiláng FO 27 / Nøkken FO 22 or KHD 25** | Real Camo Infiltration/late objective vs cheaper FD+20 Mimetism(-6) approach | Current 15-slot and point pressure; select by mission | W1,W3 |
| **Tiger Soldier AD 20–29 / Liang Kai 21** | Surprise flank/objective angle or efficient Super-Jump/EXP CC | Unnecessary to buy multiple flank pieces for defensive missions | W1,W2 |
| **Peacemaker Auxbot 23–27 / Bulleteer Spitfire 22/1** | Forward repeater and template forks, or fast Mimetism(-6) attack | Both are independent, not WhiteCo Fireteam members | W1,W3 |
| **Sierra TR Thunderbolt 18/0 / Pathfinder TacAware 17** | Economical reactive lane, or mobile FO/Sensor + activation | Fragile; not linkable here | W2,W3 |
| **ORC/Jujak, Gūijiă or Scarface+Cordelia** | Durable alternative to K2, TAG AP direct strike, or supported gun platform | Different points/SWC and hacker exposure; complete Scarface composite costs 76–80 | W1,W3 |

#### Avoid / never-take candidates

- **Fusilier SWC guns as the principal expensive damage dealer — Direct tactical warning [W1].** Shepherd recommends taking cheap Fusilier LT, FO, Hacker/decoy as a viable Hawkwood-Fusilier Core, **not** buying ordinary Fusilier HMG/ML upgrades to do premium gunfighting. *Fusilier as a cheap support backbone is excellent*, not an avoid.
- **Chaksa Longarms as a default main gun — Direct negative preference [W1,W3], conditional.** More compelling competing K2, Hawkwood, Nisse or ORC long-range tools often make their 24–29pt SWC shooting unattractive; their own legal independent Duo/Haris and specialized guns still fill particular lanes.
- **Wild Bill as general-purpose K2 attachment — Conditional [W3].** Costs additional K2 teammates to exploit bonuses, often crowding out a superior independent problem-solver. **Exception:** deliberately built legal K2 team leveraging his precise short-range gunfight.
- **Anaconda as unsupported raw-duel TAG — Contested [W1,W3 vs later StarCo analysis].** Early WhiteCo discussion dislikes BS13 damage output versus K2, Scarface or Gūijiă; current AP resistance/Warhorse and **legal Anaconda + Kaplan Duo** can make a sensible repair/holding alternative. **StarCo's Brawler+Digger Armored Haris does not transfer to WhiteCo.**
- **Hawkwood CoC option as automatic substitute for the 35/1 K1 sniper — Direct preference [W1], conditional.** The speaker strongly prefers the K1 profile; however a 40/0 CoC Hawkwood is defensible if LT insurance is actually required. This criticizes spending pattern, not the CoC skill or troop.

### Cross-sectorial ranking principles / edition checks

1. **A “must” is a reported list-building default, not tournament telemetry.** Most explicit Druze/StarCo/Dahshat endorsements are a named player's preferences; there is no verified representative inclusion-rate database here.
2. **Do not call every TAG “never take.”** Druze Anaconda has strongly negative direct testimony, whereas **StarCo Anaconda gets a persuasive later rehabilitation in a supported Haris**, and WhiteCo uses a different Kaplan Duo. It is the *same chassis with different team architecture*. The Triphammer's 0-SWC entry can also be right even if it loses raw shootout comparisons.
3. **Do not conflate FTO label and permission:** Druze Guided Clipper differs from Fireteam FTO direct ML; Ikari Guided Clipper similarly does not link; WhiteCo Clipper FTO has no Fireteam row at all; StarCo Stempler FTO likewise has no current StarCo chart row. Always use the exact current Fireteam chart and profile option.
4. **Irregular versus Regular economy is decisive:** Irregular smoke/assault excels individually in Ikari, StarCo and Dahshat, but 15 slots and too few pooled Orders can make even a roster of efficient units dysfunctional. The **Regular** cheap Keisotsu, Fusiliers, Fugazi/Fanous/Transductor and specialist options have systemic value.
5. **Mission scoring and delivery beat theoretical damage:** Druze/Dahshat Hunzakut, Ikari Karakuri/Pathfinder, StarCo Al Hawwa'/Hellcat and WhiteCo Guiláng/Tiger change whether a gun-heavy list can reach a console on time.
6. **No illegal legacy data:** Current N5.3 Army references override early N5/N4 transcripts: old StarCo Alguacil LT SWC tax, old N4 Dahshat Zúyŏng LT, imported Karakuri Fireteams, early linked-Guided Clipper assumptions and other-faction TAG/REM permissions are not reliable.

### Source coverage and limitations

- **Direct full/partial transcripts checked in the immediate research:** Druze N5 Dante, WIP12 Druze E75; StarCo N5 Dante, Loss of Lieutenant E158 StarCo section; WIP12 Ikari E191 sections, Dahshat E165 Libertos sections; WhiteCo N5 Robert Shepherd and tournament report. Remaining linked recordings were **already transcript reviewed in the corresponding existing GitHub tactical files**; do not portray every transcript as newly reviewed in this commit.
- **N4-era sources:** Druze WIP12 E75 (2022), Dahshat WIP12 E165/E166 (2024), WhiteCo WIP12 E160 (2024), Ikari IGL E163 (2024). Their exact points, team bonuses, and equipment are not current evidence. The N5.3 sectorial files take priority for such facts.
- **Dahshat N5 coverage is comparatively thin:** one substantive current N5 battle report plus cross-faction unit reviews; especially avoid inventing consensus “never take” choices. **WhiteCo tournament footage** demonstrates actual successful packages but some event formats/rules and mission requirements differ from standard play.
- **Contrary opinions intentionally retained:** Ikari Daiyōkai/Al Fasid vs cheap Wú Míng; Druze Scarface vs cheaper direct solutions; StarCo Anaconda before/after later podcast; Dahshat Maghariba vs discount swarm; WhiteCo Guiláng vs Nøkken and K2 vs heavier support.

### Whole-unit purchasing audit — can I omit an entire miniature? (2026-10-30)

This section is intentionally **sectorial-specific**: buying the same Anaconda sculpt for *Druze* versus *StarCo* gives materially different Fireteam/support access. **Skip by default** = low purchasing priority in mainstream 300pt builds, **not** a proven prohibition on every list.

| Sectorial | Entire model/unit to defer | Why / decisive exception |
|---|---|---|
| **Druze Bayram Security — Anaconda** | **Skip by default — strong single-source-pair negative** | [D1] presenters favor **Scarface + Cordelia** as the efficient TAG/repair purchase. Anaconda remains valid as a **59pt standalone/Mechanized Duo** role that Scarface's full package cannot duplicate. Do not transfer this verdict to StarCo. |
| **Ikari — Security Chief Arslan (35pt)** | **Skip by default for normal attack/LT plans** | [I1] Copper directly rates his cost inefficient against **Keisotsu/Brawler LT** and **Wú Míng AP HMG** covering those jobs. Buy if specifically leveraging **MSV1, Warhorse, NWI or command/team role**. Not a dismissal of Druze Shock Teams. |
| **StarCo — Anaconda / Triphammer** | **Defer blind standalone TAG purchases; no entire-unit hard skip** | [S1] condemns both; later [S2] argues for Anaconda's **Brawler Engineer + Digger Armored Haris**, while Triphammer buys **0 SWC**. Purchasing one for a supported role can be rational. |
| **Dahshat** | **No source-backed whole-model avoid** | Al Fasid and Ghulam **generic guns** duplicate other attacks, but retain real support/defensive profiles and there is too little current direct evidence to blacklist units. |
| **White Company — Chaksa Longarms** | **Defer as first main gun; low confidence** | [W1,W3] prefer K2, Nisse and ORC for the usual ranged role, but Longarms' legal Duo/Haris and unusual weaponry still create distinct angles. Anaconda can use a Kaplan Duo, unlike Druze/StarCo constructions. |

**Important:** The ordinary Druze HMG, Alguacil SWC, Fusilier SWC, Clockmaker-without-repair-target and Hawkwood CoC criticisms are **profile/usage warnings**, not full model skips. See [all-armies buying shortlist](../../notes/factions/model-purchase-avoid-summary-2026.md).

### Worst-value, rare-use and proxy-first mercenary miniature purchases (2026-10-30)

**Scope and evidence.** This is a **miniature-buying audit**, not a re-ranking of every profile. It covers each current NA2 army separately: [Druze Bayram Security](../non-aligned-armies/druze.md), [Ikari Company](ikari-company.md), [StarCo](../non-aligned-armies/starco-free-company-of-the-star.md), [Dahshat Company](dahshat-company.md), and [White Company](white-company.md). References are the **pinned N5.3, September 2026 Army 7.26246.159 rosters and Fireteam charts**. **Direct negative** means the speaker actually criticized that use in the earlier [transcript-backed source register](#source-coverage-and-limitations). **Proxy first**, **conditional whole-model deferral**, and **extra-copy defer** are *reasoned buying suggestions*, not claims the media said those literal words. **Rare** means unusual in reviewed all-comers constructions, *not a measured tournament inclusion rate*. When the existing podcast reviews predate current Army, the **current printed profiles** govern. No all-profile universally unplayable unit is established.

**Four distinctions matter:** a **weak gun profile** can belong to a very good unit; a **conditional whole-model deferral** is not a zero-win-rate label; a **rare specialized peripheral/character** can deserve a proxy even when genuinely excellent; and **AVA / alternate weapon sculpts** alone never create a shopping need. Also **one bought model can be reused across different legal sectorials**, not fielded twice simultaneously. No current complete inventory of the five mercenary armies was found at the expected inventory paths; the cross-army proxy examples below **do not assume ownership** of NA2-exclusive models.

#### 5. White Company — low-priority Longarms/Wild Bill and redundant K2/hero sculpts

| Unit / profile / purchase | Criticism, role competition and valid exception | Buying verdict |
|---|---|---|
| **Chaksa Longarm gun family21–29** as default main gun | **Direct lower-priority preference — [Shepherd WhiteCo](https://www.youtube.com/watch?v=y-iuVDPJ-Y4) and [Dante initial reaction](https://www.youtube.com/watch?v=UwgmSkVnrpI)**: **Karhu Feuerbach34/1.5**, **John Hawkwood K1 sniper35/1**, **Nisse/ORC** or K2 heavy teams more often justify the main long-ranged slot. **Longarm portable autocannon29/1.5, missile24/1.5, Mk12/AP mine25/0** have different AP/ARO jobs and **legal own Duo/Haris**; not all profiles worthless. | **Defer dedicated Longarm model/box by default, proxy 1–2 compatible S2 gun figures first**, then buy if specialized Chaksa link, autocannon or missile role wins. Do not buy three merely to reach AVA3. |
| **Wild Bill22–24** as a general list addition | **Conditional negative [Dante N5 reaction](https://www.youtube.com/watch?v=UwgmSkVnrpI):** a Wild Bill boost tied to **K2 team architecture** needs legal teammates, while his own short-range shooting does not replace **Karhu, Kaplan, Hawkwood or a mission specialist**. Real **MULTI Pistol(+1B)**, and 0-SWC gun profile can still help a planned midrange link. | **Skip dedicated Wild Bill unless specifically building a legal K2 package; proxy first**. A weak generic pick is not a proof of zero useful current loadouts. |
| **Fusilier HMG18/1, ML15/1.5, MULTI Sniper16/1** as a premium gun | **Direct [Shepherd WhiteCo](https://www.youtube.com/watch?v=y-iuVDPJ-Y4)** prefers **Fusilier LT10, FO12, Hacker15/.5 and cheap link bodies** supporting stronger **Hawkwood/Karhu/Kaplan** attackers. This doesn't make the cheap Fusilier line bad. | **Avoid purchasing optional heavy weapon Fusilier sculpt as a *main* gun**; proxy weapon/loadout for a legal special team. **Buy/use basic rifle/specialist figures**, not premium guns by default. |
| **Hawkwood CoC40 versus K1 Sniper35/1** | **Direct Shepherd preference** for **K1 sniper** when the army needs a long-range anti-armor attack; **CoC** command insurance can be right with vulnerable LT and has **0SWC, X-Visor, Combi(+1B)**. **Hawkwood is AVA1**, so the alternatives do not coexist in a list. | **Buy only one Hawkwood miniature if frequently using him; proxy the alternate weapon/card**, don't buy CoC and sniper sculpts for what is normally one on-table unit. |
| **Anaconda59/1.5 as unsupported generic TAG** | **Contested**: earlier sources favor **Gūijiă77 MULTI HMG, Scarface composite76–80, or efficient K2 gun teams** for damage and recovery. **White Company explicitly has a legal Anaconda+Kaplan Duo**, which differs from StarCo Armored Haris or Druze Mechanized access; **Warhorse/AP Immunity/Escape Operator** are legitimate. | **Proxy S7 Anaconda with Operator representation first**, buy if the **Kaplan repair/support Duo** is a repeated plan. **Don't call the *same TAG* universally bad across three different sectorials.** |
| **Second Gūijiă, alternate full Scarface or Anaconda / all TAG variants** | **Gūijiă77/1.5 and Scarface+Cordelia76–80/1.5** offer different TAG attack and ancillary bodies; **Gūijiă is AVA1** and a distinct **Shàngdiào ancillary** must be physically represented. For Scarface there are **Scarface, Cordelia, TurtleMek** pieces. Most WhiteCo 300pt armies won't need multiple simultaneous large purchases. | **Proxy-test one full TAG/support package**, buy the recurring primary TAG. **No second Gūijiă standard list**; don't acquire alternate TAG weapon sculpts just for a single character/profile. |
| **Second/third Karhu, Kaplan, ORC/Jujak and Hǎidào gun/team collection without an actual K2/HI architecture** | **Strong units, extra-quantity inference:** **Karhu Feuerbach34**, **Karhu Engineer25**, **Kaplan Doctor24**, **Hǎidào CoC24 / KHD22 / Engineer25 / MSV2 sniper29**, and **ORC/Jujak** provide legitimate efficient pieces. But a full Karhu + Kaplan + ORC/Jujak + Hǎidào wardrobe is more variety than one list can deploy. **One Hǎidào cannot provide CoC, KHD, Engineer and MSV2 sniper simultaneously.** | **Buy core selected K2/HI team and first useful Hǎidào**, **proxy alternate gun and excess copy** until different profiles need separate simultaneous physical models. **Do not downgrade all Hǎidào/Karhu** because some sculpts overlap. |
| **Second HD+ Danavas22/.5 in addition to Laxmee24/.5** without a two-network plan | **Laxmee** adds **Fairy Dust upgrade, Mimetism, Wildcard, Pitcher**, **Danavas** has ordinary **HD+ Pitcher/Oblivion** and may be better at a particular standalone network role. Two paid HD+ nodes can be redundant if FO/hacking already works and SWC is tight. | **Proxy second dedicated hacker first**; buy both only if they bring a distinct effective firewall/network zone. Neither is a source-backed weak whole unit. |
| **Peacemaker+Auxbot, Bulleteer, Sierra/Pathfinder and several other REM models all together** | **Source-backed favorable individual roles:** **Peacemaker23–27** forward repeater/template, **Bulleteer22/1** Mimetism(-6) attacker, **Sierra18** TR gun, **Pathfinder17 TA** objective network, **Fugazi** cheap regular repeater. **Peacemaker selected profiles have Auxbot, some do not**; **WhiteCo none of these are automatically linkable**. | **Proxy *extra* chassis, alternate Peacemaker weapon and Auxbot partner** before buying whole remote catalogue. Buy separate physical REMs when actually present together; an Auxbot is its own body. |
| **Specialist characters/mission attackers: Carmen+Bâtard17, Blade-Op Parachutist30, Kunai sniper, Valkyrie, Tiger AD and Guiláng vs Nøkken** | **Low-confidence conditional buying, not “never take”:** **Carmen+Bâtard** need 2 bodies and Irregular assault route, **Blade-Op FTO20 or Engineer23** are linked but **30pt FD/Parachutist** options are not; **Tiger** scores behind lines, **Guiláng FO27** and **Nøkken FO22** target different midfield zones, **Kunai** hidden precision snipes. Buying every one is unnecessary and may be impossible to activate in a 15-order list. | **Proxy the *second* specialty character or alternate AD/HD gun**, buy whichever has an actual mission/terrain advantage. **Carmen requires Bâtard body; Blade-Op FTO does not import the 30pt Parachutist**. |
| **Clipper Guided / FTO name, or excess missile/guided kit** | **Hard legal trap:** **White Company Clipper FTO has no Fireteam chart access**, even if a generic FTO card exists. Guided requires actual **Targeted**/Spotlight from **Laxmee/Danavas + Repeater** or FO route. A missile chassis without a legal link or target plan is just SWC/points committed to a speculative use. | **Proxy a suitable Clipper REM**, do not buy solely for a nonexistent linked Guided team. **Keep cheap Pathfinder/FO/Repeater support** because it supports many other actual tactics. |

**WhiteCo priority:** chosen **Hawkwood K1 sniper or Karhu Feuerbach**, inexpensive **Fusilier** bodies, **one Hǎidào** with the *chosen* CoC/KHD/Engineer/sniper role, **Kaplan Doctor/Engineer or Laxmee** if link/network warrants, and a distinct midfield specialist. **Strongest whole-model defers** are **Chaksa Longarms as first gun** and **Wild Bill without K2 team**, plus **unsupported Anaconda**. None is a proven no-play unit.

#### 6. Cross-mercenary — reuse, proxy rules and multi-body purchase traps

**Inventory note:** no separately verified, complete Druze/Ikari/StarCo/Dahshat/WhiteCo miniature inventories were found. The project *does* contain physical inventories for [Shindenbutai](../../inventory/shindenbutai.md), [Caledonia](../../inventory/caledonia.md), [Kestrel](../../inventory/kestrel.md), [Military Orders](../../inventory/military-orders.md) and [Steel Phalanx](../../inventory/steel-phalanx.md). **Cross-collection re-use is a candidate, not an assumption that the same sculpt is unoccupied in a simultaneous list.** In particular, two Yáoxiè Rui Shi/Lù Duān physical chassis, PanO Dronbot/Mulebot pools and both Yojimbo forms are documented in Shinden; Caledonia Cateran(s) and shared Warcor can be available where current roster allows. Check [inventory rows](../../inventory/shindenbutai.md) before ordering equivalents for an NA2 list.

| Physical category and example models | Recommended test/reuse | Do not overbuy or misrepresent |
|---|---|---|
| **Shared NA2 infantry characters** — Arslan, Valerya, Druze, Brawler, Digger, Aïda, Saito, Wild Bill, Hawkwood, Knauf, Uhahu, Parvati etc. | Use an appropriate, distinctly identified **same-size Corvus Belli infantry proxy** in each legal sectorial; prioritize characters actually in the intended list. One sculpt can represent **non-simultaneous** options across armies, or another legal unit if accepted. | **Do not import faction access.** Druze Arslan differs from Ikari Arslan value; StarCo Knauf cannot be WhiteCo Hawkwood by changing cards without an allowed physical proxy; one model can't be two deployed characters at once. |
| **Alguacil/Fusilier/Keisotsu/Ghulam/Druze/Brawler weapon variants and FTO** | Use existing generic or same-troop properly sized mini to test LT/FO/KHD/Doctor/Engineer/HMG/ML choices; clearly declare the selected loadout. | Buy **extra specific weapon sculptures** when they are actually **different legal simultaneous troopers**, not because a variant appears in Army. FTO status and link membership must be checked by exact sectorial. |
| **TAGs and supporting model counts** — Anaconda S7, Scarface+Cordelia+Turtlemek, Triphammer+Turtlemek, Maghariba S8+Jandab, Gūijiă+Shàngdiào | Borrow a *correct silhouette/base TAG* and **all separately deployed ancillary/Engineer figures** in the actual selected package. A Tag-equivalent S7 base does not automatically stand for an **S8 Maghariba**. Anaconda **Operator** appears on escape; plan an S2 model/representation then. | Scarface composite is **not just a Scarface TAG purchase**; regular physical count includes **Cordelia** and **TurtleMek**. Ancillaries aren't independent Regular Order generators. Buy large sculpts after real mission tests, not for one-time novelty. |
| **Peripherals/Servants** — Fiddler+Jackbot(s), Carmen+Bâtard, Peacemaker+Auxbot, Yáozăo/Nasmat/Zondbot, Yojimbo Koalas, Synchronized companions | Proxy **each fielded partner** with a separate, correctly based body; **equipment markers** (mine, Koala etc.) have their own marker requirements but don't make extra troopers. | Some options do **not** include companions (e.g. Fiddler FTO vs independent Jackbot; specific Peacemaker without Auxbot). Don't buy all option-specific peripherals without selecting their legal profiles. |
| **Shared JSA/Chinese/PanO REM chassis** — Yáoxiè Rui Shi/Lù Duān, Dronbot Pathfinder/Clipper/Sierra/Fugazi, Yáopú/Pangguling/Mulebot, Rafiq/Fanous, Traktor Mul | Reuse documented **2 Yáoxiè chassis**, **4 PanO Dronbots** and **2 PanO Mulebots** as **compatible-sized** temporary replacements, provided current event proxy permissions. **Traktor Mul S4** and **Maghariba S8** must be represented by their own size, not any spare S3 Dronbot. | Buy only chassis that actually **co-deploy in an NA2 list**, or are needed for correct base/size/appearance. The inventory's two Rui Shi/Lù Duān models are **two physical total**, not two of each. |
| **Smoke/Irregular warbands and airborne attackers** — Yuan Yuan, Bashi Bazouk, Hunzakut, Desperado, Libertos, Kum, Irmandinho, McMurrough, Motorized Bounty Hunter, Yojimbo | Proxy a rarely used cheap trader/AD with a **distinct correct-size** infantry/motorcycle/warband in the intended legal roster. The [Shinden inventory](../../inventory/shindenbutai.md) confirms foot+mounted Yojimbo; **motorcycle S4** differs from ordinary S2 smoke infantry. | Don't buy up to AVA automatically. **Hunzakut FO** and **Irmandinho Engineer** are Irregular; too many Irregular trades can starve the main gun of pooled Regular activations. |
| **Medium-heavy specialized silhouettes** — Al Fasid S5, Daiyōkai S5, Karakuri S2, Wú Míng S2, Riot Grrl S2, and vehicle/motorbike models | Use **correct silhouette/base** first and choose models with clearly different identities. **S5** is not an ordinary S2 stand-in; a TAG/Vehicle cannot be represented as common infantry at organized play without organizer permission. | Don't buy an S5 heavyweight simply because you already own a generic S2 HI; verify actual match and legal current unit. |
| **No actual rules on “linked Guided” unless exact profile supports both** | Druze/Ikari Clipper FTO direct ML is **not Guided**, while the Guided profile is **unlinked**; WhiteCo Clipper FTO has **no Fireteam access**; StarCo Stempler FTO likewise not linkable. Test individual **correct unit/profile/network** combinations in Army before purchase. | Do not buy REM artillery boxes for a nonexistent *FTO Guided* bonus. A Guided missile requires actual Targeted source, not merely an expensive KHD with a Pitcher. |
| **Legacy N4/early N5/Spec-Ops/Team-Ops minis** | Reuse sculpts as current legal proxies where sizes and organizer acceptance fit; edition-old fireteam boxes aren't automatically useful whole bundles. | **Do not buy optional-mode-only troops solely for standard play**. A saved N4 TAG/Fireteam roster isn't an N5.3 shopping list. |

**Combined “do not bother buying first” shortlist (not all-profile play bans):** **Druze** Anaconda without a real 59pt plan, HMG-only Druze and full Fiddler multi-bot kit; **Ikari** Arslan and unsupported Al Fasid/S5 or multiple TAGs; **StarCo** solo Anaconda/Triphammer without the relevant Armored plan, expensive optional Alguacil SWC guns, second Engineer/sniper collection; **Dahshat** Al Fasid as redundant gun, optional Ghulam HMG/ML, unproven extra guided/Maghariba TAG and excess Irregular duplicates; **WhiteCo** Chaksa Longarm box and Wild Bill before a specific team, Fusilier heavy weapon sculpts, nonplanned Anaconda and alternate Hawkwood/HD+ kits. **All** deserve re-evaluation if the exact mission, missing collection capability or verified legal Fireteam calls for them.

**Proxy policy/physical limit:** Always declare which legal Army profile each figure represents before playing. Keep its **proper base, silhouette, visibility geometry, different body for each simultaneous trooper, and actual peripheral/Ancillary count**; check current ITS and event organizer proxy policy before organized play. Proxies never change Army availability, AVA, SWC, Fireteam chart, model's real equipment, or independent Order generation.
