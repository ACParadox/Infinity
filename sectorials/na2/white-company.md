---
schema_version: 1
reference_type: sectorial
status: partial
sectorial_id: 909
sectorial_slug: white-company
sectorial_name: White Company
parent_faction: Non-Aligned Armies (NA2)
rules_baseline: N5.3
army_source_version: "7.26246.159"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-16
coverage: "Complete current White Company main roster, standard profile/loadout digest and AVA, current Fireteam chart and reverse access index, optional Spec-Ops/Team-Ops boundary, linked Reinforcements boundary, and source-normalization/validation notes."
---

# White Company — N5.3 sectorial reference

## November 2026 Army profile update

**Precedence:** These corrections supersede conflicting archived profile rows. The original source pin is retained for unchanged fields; Fireteam charts and roster indexes have not been fully reconciled, so this reference is partial.

Source: [SITREP 5.7.4](https://www.infinitytheclassifieds.com/sitrep), November 25, 2026; Army backup `e2a8532270a039796db45bd07b1d111dc7bc8311`, revision `7.26329.480`.




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

**November 2026 correction:** Only the FD (+20) Engineer and Parachutist Engineer gain Surprise Attack (-3); FTO profiles unchanged.

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

## N5.3 costed Fireteam compositions and field evidence

**Status:** These are **standard-mode** costed example teams built from the pinned Army `7.26246.159` loadouts and the authoritative chart above; **not** additional permissions. `#` is the reference profile ID where exposed (a **sole profile** means this reference does not expose a separate numeric ID); each entry shows **pts/SWC** and the total column adds only that team. **Best** identifies a recommended build, not a performance guarantee. `FT L1–L5` is determined by the largest shared same-Unit or explicit Fireteam `counts as` equivalence group, not merely the number of models (see [N5 Fireteam Bonuses](https://infinitythewiki.com/Fireteam_Bonuses)). Reports support the named combination and tactical job; chosen current loadout IDs are **N5.3 reconstructions**, not copies of unverified historical Army exports.

| Pick | Legal chart family / type (bodies) | FT level | Exact profiles (pts/SWC) | Team pts / SWC | Use / evidence / restrictions |
|---|---|---|---|---:|---|
| **Best — Shona/Varangian Smoke-CC Duo** | Varangian Guards · Duo 2 | **L2** | Varangian #4 SMG/Chain Rifle/Smoke **12/0** · Shona Carano sole profile **22/0** | **34 / 0** | Shona Wildcard counts as Varangian. Repeated in [#010](../../notes/battle-reports/001-010-n5-battle-report-tactical-analysis.md) and [#032](../../notes/battle-reports/031-040-n5-battle-report-tactical-analysis.md) shells. Varangian is Irregular. |
| **Best — Karhu/Kaplan attack-recovery Duo** | K2 · Duo 2 | **L1** | Karhu #3 Feuerbach/NCO **34/1.5** · Kaplan #7 Doctor **24/0** | **58 / 1.5** | Both source-choice families present. Despite K2 name, Karhu and Kaplan are **not** the same unit/equivalence: Level 1. |
| Anaconda/Kaplan repair Duo | Anaconda · Duo 2 | **L1** | Anaconda #2 HMG **59/1.5** · Kaplan #6 Engineer **25/0** | **84 / 1.5** | Anaconda anchor mandatory, Kaplan is native optional member; distinct units mean Level 1. |
| **Best — K2 two-Karhu specialist Haris** | K2 · Haris 3 | **L2** | Karhu #3 Feuerbach/NCO **34/1.5** · Karhu #4 Engineer/NCO **25/0** · Kaplan #7 Doctor **24/0** | **83 / 1.5** | At most two Karhu in K2 Fireteam; with a Kaplan this is a legal three-body **Level 2**, not Level 3. |
| Reported double-Hǎidào K2 Haris | K2 · Haris 3 | **L2** | Hǎidào #6 MSV2 MULTI Sniper **29/1.5** · Hǎidào #4 Killer Hacker **22/0** · Karhu #4 Engineer **25/0** | **76 / 1.5** | Three-unit combination in [#010 List A](../../notes/battle-reports/001-010-n5-battle-report-tactical-analysis.md); Karhu is required source-choice member; two Hǎidào give Level 2. |
| Mixed White Company breach Haris | White Company · Haris 3 | **L1** | ORC #3 HMG **34/1.5** · Jujak #8 Engineer **29/0** · Nisse #5 Hacker **30/0.5** | **93 / 2** | Native ORC/Jujak anchor present, Nisse max one. Three different units give Level 1: no +1SD. |
| Triple Chaksa defensive Haris | Chaksa Longarms · Haris 3 | **L3** | Chaksa Longarm #2 Portable Autocannon **29/1.5** · Chaksa Longarm #1 E/M Grenades **21/0** · Chaksa Longarm #4 Mk12 **25/0** | **75 / 1.5** | All three Longarms contribute to Level 3; their family only permits Duo/Haris, not Core. |
| **Best — Mission-class K2 four-body Core** | K2 · Core 4 | **L2** | Hǎidào #6 MSV2 MULTI Sniper **29/1.5** · Hǎidào #4 Killer Hacker **22/0** · Kaplan #7 Doctor **24/0** · Beasthunter #1 FTO HFT/Panzerfaust **9/0** | **84 / 1.5** | Reported [#010 List B](../../notes/battle-reports/001-010-n5-battle-report-tactical-analysis.md) four-body K2 structure. Beasthunter must be **#1 FTO**. Level only 2 (two Hǎidào), not 4. |
| Four-body Fusilier command Core | Fusiliers · Core 4 | **L4** | Fusilier #10 Lieutenant **10/0** · Fusilier #6 Hacker **15/0.5** · Hawkwood #6 K1 Sniper **35/1** · Emily #2 CoC/E/M Grenade Launcher **28/0** | **88 / 1.5** | Hawkwood and Emily count as Fusiliers; four members all count for Level 4. |
| Reported ORC/Valkyrie Core | White Company · Core 4 | **L2** | ORC #8 HMG Lieutenant **34/1** · Valkyrie #1 Heavy Shotgun **28/0** · Nisse #3 MSV2 MULTI Sniper **29/1.5** · Laxmee sole profile HD+/Pitcher **24/0.5** | **115 / 3** | Four-unit composition in [#032](../../notes/battle-reports/031-040-n5-battle-report-tactical-analysis.md); Valkyrie counts as ORC, others do not: **Level 2**. |
| **Best — Five-body mixed K2 Core** | K2 · Core 5 | **L3** | Kaplan #4 Heavy Rocket Launcher **20/1.5** · Kaplan #7 Doctor **24/0** · Kaplan #6 Engineer **25/0** · Karhu #3 Feuerbach/NCO **34/1.5** · Karhu #5 Paramedic/NCO **24/0** | **127 / 3** | Legal mix of three Kaplan and maximum two Karhu; five models **only Level 3**. Strong role diversity, but expensive. |
| Five-Kaplan pure K2 Core | K2 · Core 5 | **L5** | Kaplan #4 Heavy Rocket Launcher **20/1.5** · Kaplan #7 Doctor **24/0** · Kaplan #6 Engineer **25/0** · Kaplan #8 Specialist Operative **21/0** · Kaplan #1 Adhesive Launcher **21/0** | **111 / 1.5** | Five natural Kaplan are Level 5; higher bonus than a three-Kaplan/two-Karhu mix but less premium ranged offense. |
| Five-body ORC-equivalent Core | White Company · Core 5 | **L5** | ORC #3 HMG **34/1.5** · ORC #2 TinBot MULTI Rifle **29/0** · ORC #6 Hacking Device **33/0.5** · Hannibal #5 Vulkan Shotgun **24/0** · Valkyrie #1 Heavy Shotgun **28/0** | **148 / 2** | Hannibal and Valkyrie are explicit `counts as ORC` Wildcards; all five attain Level 5, with substantial points investment. |
| Reported long-range mixed Fusilier Core | Fusiliers · Core 5 | **L2** | Hǎidào #6 MSV2 MULTI Sniper **29/1.5** · Hawkwood #6 K1 Sniper **35/1** · Fusilier #1 Combi Rifle **10/0** · Laxmee sole profile HD+/Pitcher **24/0.5** · Señor Massacre #2 Eclipse/BSG **25/0** | **123 / 3** | Five named bodies in [#010 List A](../../notes/battle-reports/001-010-n5-battle-report-tactical-analysis.md). Only Hawkwood+Fusilier count as Fusiliers: **Level 2**, despite five bodies; expensive sniper/control fork. |
| **Best — Hawkwood/Emily five-body Fusilier Core** | Fusiliers · Core 5 | **L5** | Hawkwood #6 K1 Sniper **35/1** · Emily #2 Chain of Command/E/M GL **28/0** · Fusilier #6 Hacker **15/0.5** · Fusilier #10 Lieutenant **10/0** · Fusilier #8 Forward Observer **12/0** | **100 / 1.5** | Based on [#112 Unmasking](../../notes/battle-reports/111-120-n5-battle-report-tactical-analysis.md), replacing its historically reported 'Lt Decoy' with **current #8 FO** rather than inventing an extra standard Lieutenant. All five count as Fusiliers => Level 5. |

**Restrictions / comparative levels:** one **Core** and one **Haris**, but unlimited Duo slots. K2's `required:true, min:0` Kaplan/Karhu source-choice rows are preserved rather than converted into a fabricated one-of-each obligation. K2 has **max two Karhu**; a mixed K2 Core of five is not automatically Level 5. White Company ORC/Jujak `required:true,min:0` flags likewise remain a source-choice set. Native Fusilier Haris/Core requires a real Fusilier; Hǎidào is a Wildcard (**max three per team**, normal AVA three across all teams). Only Beasthunter **#1 FTO** and Blade-Ops **#1/#2 FTO** are valid in their listed families. **Clipper #5 FTO has no White Company Fireteam access**. Historical #010, #032 and #112 report memberships are not assumed to certify all 2026 profiles or simultaneous SWC budgets.


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

## Provenance

Validated against the pinned N5.3 Army-derived source on **2026-10-16**. If future Army revisions change roster entries, AVA, profiles, Fireteam chart semantics, optional modes or Reinforcement linkage, update this file and its `army_source_version`/verification metadata together.

**Tactical and purchasing analysis:** [White Company tactical guide](../../notes/factions/white-company.md). Profile costs, AVA, Fireteams, source provenance and validation remain authoritative here.
