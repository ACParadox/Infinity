---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 601
sectorial_slug: combined-army
sectorial_name: Vanilla Combined Army
parent_faction: Combined Army
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Complete standard Vanilla Combined Army roster, standard loadouts/profile states, canonical vanilla Fireteam chart, reverse Fireteam index, optional-mode hooks, and linked Reinforcement army. Generic Soldier of Fortune catalog entries are excluded."
---

# Vanilla Combined Army

## Overview and provenance

Repository-native reference for **Vanilla Combined Army** (`army_id: 601`). This file uses the sectorial-reference schema even though Combined Army is the parent vanilla faction rather than a sectorial.

Sources used:

- Army-derived Combined Army source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`, path `n5/combined-army/7.26246.158.json`.
- Army source blob `b93bf73c1e3a09f81ea883e9440b6915865eb3e6`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- The ordinary matched-play roster contains **52 standard logical units** in Army roster order.
- `Nexus-7 Spec-Ops`, `Treitak Spec-Ops`, and `Combined Army Team-Ops` are optional-mode records, not ordinary matched-play roster entries.
- Generic Soldier of Fortune / mercenary-catalog entries with `factions: []` are excluded. Faction-listed Armand, Krakot Renegades, Libertos, and Aïda Swanson are standard vanilla Combined Army entries and are included.
- Vanilla Combined Army has a source-defined Fireteam chart: **no Core, maximum 1 Haris, maximum 2 Duos**.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name by itself.
- Rindak joins the Morat Fireteam only through **RINDAK FTO option 1**.
- Umbra Legate Wildcard access is explicitly marked `FTO` by the chart and therefore uses only the FTO-labelled vanilla profiles: options **3, 4, 5, 6, and 9**.
- Aïda Swanson has an FTO-labelled profile but no vanilla Combined Army Fireteam-chart row; that label alone does not grant Fireteam access.
- The source includes a `--` / `Spec-Ops` placeholder in Combined Army and Overdron Fireteams. It is retained as an optional-mode hook and is not assigned to a particular optional record by inference.
- Fraacta-like transformation logic is not present in this vanilla roster, but several included logical units have alternate states: Armand has active/inactive Symbiont Armor states; Seed-Soldiers have Seed-Embryo/developed states; Sartroids have connected/autonomous states.
- Sphinx includes a Scindron ancillary Remote. Caskuda, Avatar, and Overdron include Staldron ancillary Remotes. Bit includes one KISS! peripheral variant according to loadout. These are parent/peripheral relationships, not extra roster units.
- The pinned source links standard Ko Dali and Sheskiin to their Reinforcement counterparts. Reinforcement army **699** is kept separate from the standard roster and Fireteam chart.

## Sectorial summary

| Field | Value |
|---|---|
| Faction | Vanilla Combined Army |
| Parent faction | Combined Army |
| Army ID | 601 |
| Rules baseline | N5.3 |
| Standard roster units | 52 |
| Optional-mode records | 3 |
| Linked Reinforcement army | 699 |
| Main Fireteam chart | yes |

## Fireteam chart limits and faction-level restrictions

| Constraint | Value / wording |
|---|---|
| Core | `0`: none |
| Haris | `1`: maximum 1 |
| Duo | `2`: maximum 2 |
| Main/Reinforcement mixing | Reinforcement roster/chart kept separate |
| Rindak restriction | `RINDAK FTO` only; vanilla option 1 |
| Umbra Legate Wildcard restriction | `FTO` only; vanilla options 3, 4, 5, 6, 9 |
| FTO labels generally | An FTO label does not grant access unless the Fireteam chart says so |
| Spec-Ops placeholder | Source `--` row, max 1; retained as an optional-mode hook without inferred identity |

## Roster index

| Unit | ID | AVA | Type | Order / state | Vanilla Fireteam access |
|---|---:|---:|---|---|---|
| The Shrouded | 501 | 2 | SK | Regular | — |
| Rasyat Diplomatic Division | 519 | 1 | MI | Regular | — |
| Rindak Emergency Brigade | 1575 | 1 | HI | Regular | Morat Duo/Haris max 1, FTO opt 1 only |
| Shasvastii Noctifers | 516 | 1 | LI | Regular | — |
| WCD Vector Operators | 1763 | 1 | MI | Regular | Combined Army Duo/Haris max 1 |
| M-Drones | 508 | 2 | REM | Regular; one profile + Tactical Awareness | — |
| T-Drones | 510 | 1 | REM | Regular | — |
| Glyph Warcors | 1873 | 1 | LI | Irregular | — |
| The Anathematics | 523 | 1 | HI | Regular | — |
| Umbra Legates | 495 | 1 | MI | Regular + Tactical Awareness | Wildcard max 1, FTO opts only |
| Ímetron | 527 | 2 | LI | Regular | — |
| Sphinx | 524 | 1 | TAG | Regular + Tactical Awareness | — |
| Caskuda | 1624 | 1 | TAG | Regular + Tactical Awareness | — |
| Yaogat Strike Infantry | 518 | 3 | MI | Regular | Morat Duo/Haris max 3 |
| Speculo Killers | 503 | 1 | SK | Regular | — |
| Unidron Batroids | 493 | Total | REM | Regular | Combined Army Duo/Haris max 3 |
| Med-Tech Obsidon Medchanoid | 507 | 1 | LI | Regular | — |
| Slave Drones | 526 | 2 | REM | Peripheral; no own Order | — |
| E-Drones | 741 | 2 | REM | Regular | — |
| Ikadron Batroids | 532 | 2 | REM | Regular | — |
| Victor Messer | 1299 | 1 | LI | Regular | Wildcard max 1 |
| Morat Vanguard Infantry | 492 | 4 | LI | Regular | Morat Duo/Haris max 3 |
| Avatar | 500 | 1 | TAG | Regular + Tactical Awareness | — |
| Special Operative Ko Dali | 1516 | 1 | MI | Regular | — |
| Dāturazi Witch-Soldiers | 504 | 4 | WB | Regular + Impetuous | — |
| Sartroids: Ranters | 1885 | 1 | REM | Peripheral (Cyberplug); no own Order | — |
| Armand ‘Le Muet’ | 680 | 1 | MI/LI | Regular; Transmutation | — |
| Greif Operators | 1298 | 1 | SK | Regular | — |
| Krakot Renegades | 756 | 2 | LI | Regular + Impetuous | — |
| Caliban | 528 | 2 | LI | Regular | — |
| R-Drones | 511 | 1 | REM | Regular | — |
| Sartroids: Puzzlers | 1886 | 1 | REM | Peripheral (Cyberplug); no own Order | — |
| Malignos | 502 | 2 | SK | Regular | — |
| The Hungries: Gakis | 505 | Total | WB | Irregular + Impetuous | — |
| The Hungries: Pretas | 506 | Total | WB | Irregular + Impetuous | — |
| Libertos Freedom Fighters | 1275 | 1 | LI | Irregular | — |
| WCD Base Operators | 1765 | 2 | MI | Regular | Combined Army Duo/Haris max 2 |
| WCD Void Operators | 1764 | 2 | MI | Regular | Combined Army Duo/Haris max 2 |
| The Charontids | 498 | 1 | HI | Regular | — |
| Rodok | 497 | 3 | MI | Regular | Morat Duo/Haris max 3 |
| Achilles | 1863 | 1 | HI | Regular | — |
| Mentor | 1292 | 1 | LI | Regular | — |
| Dartok Cybercombat Team | 1572 | 1 | LI | Regular | Morat Duo/Haris max 1 |
| Nourkias | 1513 | 1 | LI | Regular | Combined Army Duo/Haris max 1; Overdron Duo max 1 |
| Shasvastii Seed-Soldiers | 512 | 2 | LI | Regular; transformation state | — |
| Aïda Swanson | 1160 | 1 | LI | Regular | —; FTO label alone grants none |
| Bit & KISS! | 965 | 1 | LI + REM peripheral | Regular | — |
| Overdron Batroids | 785 | 1 | TAG | Regular + Tactical Awareness | Overdron Duo: exactly 1 Overdron base member |
| EXOs, Exrah Executive Officers | 1766 | 1 | MI | Regular | Combined Army Duo/Haris max 1 |
| Q-Drones | 509 | 1 | REM | Regular | — |
| Cadmus-Naish Agent Sheskiin | 533 | 1 | LI | Regular | — |
| Nexus Operatives | 783 | 2 | MI | Regular | Combined Army Duo/Haris max 2; Overdron Duo max 1 |

### Optional-mode records

| Unit | ID | Mode | Ordinary roster? | Fireteam relevance |
|---|---:|---|---|---|
| Nexus-7 Spec-Ops | 1918 | Spec-Ops | No | Source has a generic `--` / `Spec-Ops` hook; identity not inferred |
| Treitak Spec-Ops | 1919 | Spec-Ops | No | Source has a generic `--` / `Spec-Ops` hook; identity not inferred |
| Combined Army Team-Ops | 1932 | Team-Ops | No | No specific ordinary-row identity inferred from the `--` placeholder |

## Unit details

### The Shrouded

**ID 501 · AVA 2 · SK** — `MOV 10-10 | CC 14 | BS 12 | PH 12 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Shasvastii, Surprise Attack (-3), Camouflage, Mimetism (-3), Infiltration, Terrain (Total), Regeneration, Stealth.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 20 | 0 | Boarding Shotgun, Shock Mine, Pistol, CCW | — |
| 3 | 24 | 1.5 | MULTI Sniper Rifle, Pistol, CCW | — |
| 4 | 28 | 0.5 | Combi Rifle, Shock Mine, Pistol, CCW; Hacking Device, Hacker | — |
| 5 | 24 | 0 | Combi Rifle, Flash Pulse, Shock Mine, Pistol, CCW; Forward Observer | — |
| 6 | 24 | 0.5 | Combi Rifle, Shock Mine, Pistol, CCW; Minelayer | — |
| 7 | 21 | 0.5 | Boarding Shotgun, Pistol, CCW; Dazer, Minelayer | — |
| 9 | 26 | 0 | Combi Rifle, Shock Mine, Pistol, CCW; Killer Hacking Device, Hacker | — |

### Rasyat Diplomatic Division

**ID 519 · AVA 1 · MI** — `MOV 10-10 | CC 21 | BS 12 | PH 13 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. Martial Arts L2, Natural Born Warrior, Parachutist (Deployment Zone), Combat Jump, Stealth, Warhorse, Religious Troop, Dodge (+2.5), Super-Jump (Jet Propulsion).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 25 | 0 | Boarding Shotgun, D-Charges, Eclipse Grenades, Heavy Pistol, DA CCW (PS 5) | — |
| 3 | 34 | 1.5 | Spitfire, D-Charges, Eclipse Grenades, Heavy Pistol, DA CCW (PS 5) | — |
| 4 | 31 | 0 | Combi Rifle, E/M Carbine, D-Charges, Eclipse Grenades, Heavy Pistol, DA CCW (PS 5) | — |

### Rindak Emergency Brigade

**ID 1575 · AVA 1 · HI** — `MOV 15-5 | CC 16 | BS 12 | PH 13 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Hackable, structure profile; MediKit (+1B), Sensor, No Wound Incapacitation, Climbing Plus, Religious Troop, Warhorse and source Dodge modifiers.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 0 | **RINDAK FTO**; SMG, Adhesive Launcher Rifle, Flash Pulse (+1B), Heavy Pistol, PARA CCW; Paramedic | Morat max 1; exact FTO profile |
| 2 | 32 | 0 | Vulkan Shotgun, E/Mitter, Heavy Pistol, PARA CCW; Paramedic, Forward Deployment (+20) | — |
| 3 | 33 | 0 | MULTI Rifle (+1B), Blitzen, Heavy Pistol, PARA CCW; Paramedic, Forward Deployment (+20) | — |
| 4 | 26 | 0 | SMG, Adhesive Launcher Rifle, Flash Pulse (+1B), Heavy Pistol, PARA CCW; Paramedic, Forward Deployment (+20) | — |
| 5 | 32 | 0.5 | Vulkan Shotgun, Blitzen (+1B), Shock Mine, Heavy Pistol, PARA CCW; Paramedic, Forward Deployment (+20), Minelayer | — |

### Shasvastii Noctifers

**ID 516 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. X-Visor; Shasvastii, Surprise Attack (-3), Camouflage, Hidden Deployment, Mimetism (-6), Stealth, Dogged, Courage.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 2 | 29 | 1 | Spitfire, Breaker Pistol, CCW |
| 3 | 30 | 1.5 | Missile Launcher, Assault Pistol, CCW |
| 6 | 31 | 1.5 | Spitfire, Breaker Pistol, CCW; Forward Deployment (+10) |

### WCD Vector Operators

**ID 1763 · AVA 1 · MI** — `MOV 15-5 | CC 14 | BS 12 | PH 11 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 2`. MSV2, Courage, Dodge (+2.5), Exrah, Mimetism (-3), Terrain (Total), Super-Jump (Jet Propulsion).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Heavy Shotgun, D-Charges, Shock Mine, Pistol, CCW | Combined Army max 1 |
| 2 | 24 | 0.5 | MULTI Marksman Rifle, Pistol, CCW | same |
| 3 | 26 | 1.5 | Spitfire, Pistol, CCW | same |
| 4 | 29 | 1.5 | Plasma Sniper Rifle, Pistol, CCW | same |

### M-Drones

**ID 508 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Deactivator, Repeater; Remote Presence, Triangulated Fire, Courage, Forward Observer, Terrain (Total), Sensor.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 15 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3) |
| 3 | 18 | 0 | Same; Tactical Awareness |

### T-Drones

**ID 510 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CCW (-3); BS Attack (Guided) |

### Glyph Warcors, Ur Hegemony Journalists

**ID 1873 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular; Journalist and Dodge (+3).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 4 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor |
| 2 | 4 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); Sixth Sense |

### The Anathematics

**ID 523 · AVA 1 · HI** — `MOV 15-5 | CC 19 | BS 13 | PH 13 | WIP 16 | ARM 5 | BTS 6 | W 2 | S 6`. Surprise Attack (-3), Camouflage, Mnemonica, Mimetism (-6), Stealth, No Wound Incapacitation, Courage, Dodge (+5).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 3 | 73 | 0.5 | Plasma Rifle, Sepsitor, Pulzar (+1B), AP Heavy Pistol, Monofilament CCW (-3); Hidden Deployment |
| 4 | 72 | 0.5 | Plasma Rifle, Pulzar, AP Heavy Pistol, Monofilament CCW (-3); Hacking Device with Trinity (+1B), Hacker, Hidden Deployment |
| 5 | 75 | 0 | Lieutenant (+1 Command Token); loadout as opt 3 |
| 6 | 70 | 0.5 | Lieutenant; Hacking Device with Trinity (+1B), loadout as opt 4 |
| 7 | 74 | 0.5 | Lieutenant (+1 Command Token); Hacking Device with Trinity (+1B), loadout as opt 4 |

### Umbra Legates

**ID 495 · AVA 1 · MI** — `MOV 15-5 | CC 22 | BS 13 | PH 12 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Regular + Tactical Awareness; Courage, Dodge (+2.5), Mimetism (-3), No Wound Incapacitation, Stealth, Immunity (Shock), Martial Arts L3.

| Opt | Pts | SWC | Label / loadout | Wildcard? |
|---:|---:|---:|---|---|
| 1 | 36 | 0 | UMBRA LEGATE; Vulkan Shotgun (+1B), Zapper, Flash Pulse, Pistol, DA CCW (PS 5); Forward Deployment (+20) | no |
| 2 | 41 | 1.5 | UMBRA LEGATE; Spitfire, Zapper, Flash Pulse, Pistol, DA CCW; Forward Deployment (+20) | no |
| 3 | 33 | 0 | **UMBRA LEGATE FTO**; K1 Combi Rifle, Zapper, Flash Pulse, Pistol, DA CCW | yes |
| 4 | 37 | 1.5 | **UMBRA LEGATE FTO**; Spitfire, Zapper, Flash Pulse, Pistol, DA CCW | yes |
| 5 | 38 | 0 | **UMBRA LEGATE FTO**; K1 Combi Rifle, Zapper, D-Charges, Flash Pulse, Pistol, DA CCW; Chain of Command | yes |
| 6 | 38 | 0.5 | **UMBRA LEGATE FTO**; K1 Combi Rifle, Zapper, D-Charges, Flash Pulse, Pitcher, Pistol, DA CCW; Hacking Device Plus, Hacker | yes |
| 7 | 42 | 0.5 | UMBRA LEGATE; Vulkan Shotgun (+1B), Zapper, Flash Pulse, Pistol, DA CCW; Hacking Device Plus, Deployable Repeater, Hacker, Forward Deployment (+20) | no |
| 9 | 37 | 1.5 | **UMBRA LEGATE FTO** Lieutenant; Spitfire, Zapper, Flash Pulse, Pistol, DA CCW | yes |

### Ímetron

**ID 527 · AVA 2** — `MOV — | CC — | BS — | PH — | WIP — | ARM 0 | BTS 3 | W 1 | S 2`. Must deploy by Combat Jump during the Deployment Phase. Warhorse, Combat Jump (PH=12), Religious Troop.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 6 | 0 | No weapons; contributes a Regular Order |

### Sphinx

**ID 524 · AVA 1 · TAG** — `MOV 15-15 | CC 20 | BS 14 | PH 15 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`. ECM: Guided (-6), Mimetism (-6), Camouflage, Hidden Deployment, Courage, Tactical Awareness, Climbing Plus, Remote Presence and source TAG skills.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 93 | 2 | Spitfire, Heavy Flamethrower (+1B), DA CCW (PS 5); includes Scindron ancillary Remote; Regular + Tactical Awareness |

### Caskuda

**ID 1624 · AVA 1 · TAG** — `MOV 15-10 | CC 18 | BS 14 | PH 16 | WIP 12 | ARM 7 | BTS 6 | W 3 | S 7`. ECM: Guided (-6), Remote Presence, Courage, Combat Jump, Tactical Awareness, source BS Attack and landing/explosion modifiers.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 64 | 1 | MULTI Rifle, Chain Rifle, E/M CCW (PS 4); includes Staldron ancillary Remote; Regular + Tactical Awareness |

### Yaogat Strike Infantry

**ID 518 · AVA 3 · MI** — `MOV 10-10 | CC 16 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. MSV2, Number 2, Religious Troop, Warhorse.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 0 | Combi Rifle, Panzerfaust, Heavy Pistol, CCW | Morat max 3 |
| 2 | 21 | 0 | Boarding Shotgun, Panzerfaust, Heavy Pistol, CCW | same |
| 3 | 32 | 1.5 | MULTI Sniper Rifle (+1B), Heavy Pistol, CCW | same |
| 5 | 29 | 1.5 | Spitfire, Heavy Pistol, CCW | same |
| 6 | 29 | 0.5 | Combi Rifle, Panzerfaust, Heavy Pistol, CCW; Hacking Device, Hacker | same |

### Speculo Killers

**ID 503 · AVA 1 · SK** — `MOV 10-10 | CC 22 | BS 12 | PH 12 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Shasvastii, Martial Arts L3, Impersonation, Surprise Attack (-3), Courage, Dodge (+2.5), Regeneration, Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 29 | 1 | Combi Rifle, Nanopulser, Smoke Grenades, Silenced Pistol, Monofilament CCW |
| 2 | 26 | 1 | Boarding Shotgun, Nanopulser, Smoke Grenades, Silenced Pistol, Monofilament CCW |

### Unidron Batroids

**ID 493 · AVA Total · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 12 | ARM 1 | BTS 6 | W 1 | S 2`. Remote Presence, Courage, Dogged, Discover (+3), Dodge (+2.5).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Plasma Carbine, Pistol, PARA CCW (-3) | Combined Army max 3 |
| 2 | 14 | 0 | K1 Combi Rifle, Pistol, PARA CCW (-3) | same |
| 3 | 15 | 0.5 | K1 Combi Rifle, Pistol, PARA CCW (-3); TinBot: Firewall (-3) | same |
| 4 | 24 | 1.5 | Plasma Sniper Rifle, Pistol, PARA CCW (-3) | same |
| 5 | 20 | 1.5 | Missile Launcher, Light Shotgun, Pistol, PARA CCW (-3) | same |
| 6 | 18 | 1 | Spitfire, Pistol, PARA CCW (-3) | same |
| 7 | 15 | 0 | Plasma Carbine, Flash Pulse, Pistol, PARA CCW (-3); Forward Observer | same |
| 8 | 16 | 0 | Plasma Carbine, Pistol, PARA CCW (-3); Commlink, Specialist Operative | same |

### Med-Tech Obsidon Medchanoid

**ID 507 · AVA 1 · LI** — `MOV 15-10 | CC 16 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 3`. Deactivator, GizmoKit, MediKit; Engineer, Doctor.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 21 | 0 | Combi Rifle, Zapper, D-Charges, Pistol, CCW |
| 3 | 22 | 0 | Same; Deployable Cover |
| 4 | 24 | 0 | Base weapons + Armed Turret (Combi Rifle) |
| 5 | 25 | 0 | Base weapons + Armed Turret (Marksman Rifle) |
| 6 | 24 | 0 | Base weapons + Cyberplug |

### Slave Drones

**ID 526 · AVA 2 · REM** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Peripheral (Servant), Courage, Mimetism (-3); no Order of its own.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 3 | 0 | PARA CCW (-3) |

### E-Drones

**ID 741 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. EVO Hacking Device, Remote Presence, Courage, Hacker, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 17 | 0.5 | Combi Rifle, PARA CCW (-3) |

### Ikadron Batroids

**ID 532 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 2`. Baggage, Repeater; Remote Presence, Courage, Discover (+3), Dodge (+2.5), Dogged.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 11 | 0 | Light Flamethrower (+1B), Pistol, PARA CCW (-3) |

### Victor Messer

**ID 1299 · AVA 1 · LI** — `MOV 10-10 | CC 14 | BS 12 | PH 10 | WIP 14 | ARM 0 | BTS 3 | W 2 | S 2`. Nanoscreen; Hacking Device Plus with source upgrades, Shasvastii, Stealth, No Cover, Technorganic and source GizmoKit/MediKit modifiers.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 31 | 0.5 | MULTI Rifle, Nanopulser (+1B), Cybermine, D-Charges, Breaker Pistol (PS 6), CCW; Deployable Repeater, TinBot: ECM Guided (-9), Hacker | Wildcard max 1 |
| 2 | 30 | 0.5 | Vulkan Shotgun, E/Mitter, Cybermine, D-Charges, Silenced Pistol (PS 6), CCW; Deployable Repeater, Hacker, Minelayer | same |

### Morat Vanguard Infantry

**ID 492 · AVA 4 · LI** — `MOV 10-10 | CC 15 | BS 11 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Religious Troop, Warhorse.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Heavy Pistol, CCW | Morat max 3 |
| 2 | 23 | 1 | HMG, Heavy Pistol, CCW; BS Attack (-3) | same |
| 4 | 17 | 1 | K1 Sniper Rifle, Heavy Pistol, CCW | same |
| 5 | 19 | 1.5 | Missile Launcher, Heavy Pistol, CCW | same |
| 7 | 15 | 0 | Combi Rifle, Flash Pulse, Heavy Pistol, CCW; Forward Observer | same |
| 8 | 16 | 0 | Combi Rifle, Heavy Pistol, CCW; MediKit, Paramedic | same |
| 9 | 14 | 1 | Lieutenant; Combi Rifle, Heavy Pistol, CCW | same |
| 11 | 16 | 0 | Combi Rifle, Heavy Pistol, CCW; Commlink, Specialist Operative | same |

### Avatar

**ID 500 · AVA 1 · TAG** — `MOV 15-10 | CC 19 | BS 15 | PH 16 | WIP 17 | ARM 9 | BTS 9 | W 3 | S 7`. ECM: Guided (-6), Mimetism (-6), Strategos L2, Mnemonica, Tactical Awareness and source TAG defensive modifiers.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 122 | 3 | MULTI HMG, Sepsitor Plus, DA CCW (PS 4); Lieutenant (+1 Command Token); includes Staldron; Regular + Tactical Awareness |

### Special Operative Ko Dali

**ID 1516 · AVA 1 · MI** — `MOV 15-5 | CC 19 | BS 14 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. MSV2, Martial Arts L3, Courage, Dodge (+5), Immunity (ARM), Protheion, Stealth, Specialist Operative.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 37 | 0 | MULTI Rifle, Pulzar, D-Charges, Assault Pistol (+1B), AP CCW; Parachutist, Combat Jump, Super-Jump (Jet Propulsion) |
| 2 | 34 | 0 | MULTI Rifle, D-Charges, Pulzar, Assault Pistol (+1B), AP CCW; Forward Deployment (+20), Mimetism (-3) |

### Dāturazi Witch-Soldiers

**ID 504 · AVA 4 · WB** — `MOV 10-10 | CC 23 | BS 11 | PH 14 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Regular + Impetuous; Martial Arts L4, Berserk, Dodge (+2.5), Mimetism (-3), Religious Troop, No Cover, Warhorse.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 4 | 14 | 0 | Chain Rifle (+1B), Grenades, Smoke Grenades, Heavy Pistol, DA CCW (PS 4) |
| 5 | 15 | 0 | Boarding Shotgun, Smoke Grenades, Heavy Pistol, DA CCW |
| 6 | 18 | 0.5 | Combi Rifle, Smoke Grenade Launcher, Heavy Pistol, DA CCW |

### Sartroids: Ranters

**ID 1885 · AVA 1 · REM** — Peripheral (Cyberplug); no Order of its own. Army exposes two profile states rather than two roster units.

| State | MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Connected | 15-10 | 16 | 13 | 12 | 12 | 3 | 6 | 1 | 5 |
| Autonomous | 15-10 | 12 | 11 | 11 | 11 | 3 | 6 | 1 | 5 |

Connected state includes ECM: Hacker (-3); both states retain the source Peripheral/Courage package, with the connected state carrying the stronger deployment/mobility modifiers.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 18 | 0 | Mk12, Boarding Pistol, PARA CCW (-3) |
| 2 | 19 | 1 | Spitfire, Boarding Pistol, PARA CCW (-3) |
| 3 | 12 | 0 | SMG, Thunderbolt, Boarding Pistol, PARA CCW (-3) |

### Armand ‘Le Muet’

**ID 680 · AVA 1** — one logical character with active/inactive Symbiont Armor states.

| State | Type | MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Active | MI | 10-10 | 21 | 13 | 12 | 13 | 2 | 3 | 2 | 2 |
| Inactive | LI | 10-10 | 21 | 13 | 12 | 13 | 0 | 0 | 2 | 2 |

Active state: BS Attack (Shock), Forward Deployment (+10), Natural Born Warrior, Mimetism (-6), Stealth, Transmutation. Inactive state retains BS Attack (Shock), Natural Born Warrior and Stealth.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 2338 | 33 | 1.5 | MULTI Sniper Rifle, Nanopulser, Shock Mine, Breaker Pistol (+1B), Viral CCW (PS 7); Minelayer |
| 2339 | 34 | 1.5 | MULTI Sniper Rifle, Nanopulser, Breaker Pistol (+1B), Viral CCW (PS 7); MSV1 |

### Greif Operators

**ID 1298 · AVA 1 · SK** — `MOV 10-10 | CC 17 | BS 11 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. MSV1, Courage, Stealth.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 23 | 0 | Combi Rifle, D-Charges, Breaker Pistol (+1B), CCW, Viral Mine; Forward Deployment (+20), Mimetism (-6) |
| 2 | 25 | 0 | Shock Marksman Rifle, Breaker Pistol (+1B), CCW, D-Charges; Forward Deployment (+20), Mimetism (-6) |
| 3 | 21 | 0.5 | Breaker Combi Rifle, D-Charges, Silenced Pistol (+1B), CCW; Surprise Attack (-3), Impersonation (IMP-2) |

### Krakot Renegades

**ID 756 · AVA 2 · LI** — `MOV 15-5 | CC 23 | BS 11 | PH 13 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. Regular + Impetuous; Berserk, Forward Deployment (+10), Warhorse, MetaChemistry (ReRoll), Super-Jump, Religious Troop, No Cover, Dodge (+5).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 14 | 0 | Chain Rifle, Chest Mine, Grenades, Heavy Pistol, DA CCW (PS 6); BS Attack (+1B) |
| 2 | 16 | 0 | Boarding Shotgun, Chest Mine, Heavy Pistol, AP CCW (PS 6) |
| 4 | 17 | 0 | SMG (+1B), Chest Mine, Heavy Pistol, DA CCW |
| 5 | 24 | 1 | Red Fury, Chest Mine, Heavy Pistol, AP CCW |

### Caliban

**ID 528 · AVA 2 · LI** — `MOV 10-10 | CC 23 | BS 12 | PH 13 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Shasvastii, Surprise Attack (-3), Forward Deployment (+20), Dodge (+5), Mimetism (-3), Protheion, Stealth, Martial Arts L3, Courage, Camouflage, Immunity (Shock).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 24 | 0 | Boarding Shotgun, D-Charges, Pistol, CCW (PS 5) |
| 5 | 26 | 0 | Vulkan Shotgun, Flash Pulse (+1B), D-Charges, Pistol, CCW; Forward Observer |
| 7 | 26 | 0 | SMG, Pulzar, Grenades, D-Charges, Pistol, CCW; Specialist Operative |
| 8 | 36 | 1.5 | Spitfire, D-Charges, Pistol, CCW; MSV1 |

### R-Drones

**ID 511 · AVA 1 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Remote Presence, Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) |

### Sartroids: Puzzlers

**ID 1886 · AVA 1 · REM** — Peripheral (Cyberplug); no Order of its own. Army exposes connected/autonomous states.

| State | MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Connected | 20-5 | 15 | 12 | 10 | 12 | 3 | 6 | 1 | 5 |
| Autonomous | 15-10 | 12 | 10 | 9 | 11 | 3 | 6 | 1 | 5 |

Both states carry the source Peripheral/Courage package; the connected state carries the stronger deployment/infiltration modifiers.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 13 | 0 | Deployable Repeater, Adhesive Launcher Rifle, E/Marat, Stun Pistol (+1B), PARA CCW (-6); Camouflage (1 Use) |
| 2 | 12 | 0 | Deployable Repeater, Akrylat-Kanone, E/Marat, Stun Pistol (+1B), PARA CCW (-6); Hidden Deployment |

### Malignos

**ID 502 · AVA 2 · SK** — `MOV 15-5 | CC 15 | BS 12 | PH 12 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Shasvastii, Surprise Attack (-3), Camouflage, Hidden Deployment, Mimetism (-6), Infiltration, Terrain (Total), Regeneration, Stealth.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 2 | 31 | 0.5 | SMG, Monofilament Mine, Silenced Pistol, CCW; Minelayer |
| 3 | 30 | 0 | Boarding Shotgun, Pulzar (+1B), Viral Mine, Silenced Pistol, CCW |
| 4 | 33 | 1.5 | MULTI Sniper Rifle, Pulzar, Silenced Pistol, CCW |
| 5 | 34 | 0.5 | SMG, D-Charges, Shock Mine, Silenced Pistol, CCW; Hacking Device, Hacker |
| 6 | 30 | 0 | SMG, Flash Pulse, D-Charges, Shock Mine, Silenced Pistol, CCW; Forward Observer |
| 8 | 32 | 0 | SMG, D-Charges, Shock Mine, Silenced Pistol, CCW; Killer Hacking Device, Dazer, Hacker |

### The Hungries: Gakis

**ID 505 · AVA Total · WB** — `MOV 15-15 | CC 20 | BS 9 | PH 14 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular + Impetuous; Berserk, Dodge (+2.5), Explode, Climbing Plus, No Cover.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 4 | 0 | AP CCW |

### The Hungries: Pretas

**ID 506 · AVA Total · WB** — `MOV 15-15 | CC 20 | BS 9 | PH 14 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular + Impetuous; Courage, Dodge (+2.5), Dogged, Climbing Plus, No Cover.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 7 | 0 | Chain Rifle, AP CCW |

### Libertos Freedom Fighters

**ID 1275 · AVA 1 · LI** — `MOV 10-10 | CC 16 | BS 11 | PH 11 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular; Camouflage (1 Use), Courage, Forward Deployment (+20), source Dodge modifiers, Terrain (Aquatic), Dogged, Frenzy.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 8 | 0 | SMG, Chain-colt, Pistol, CCW |
| 4 | 8 | 1 | Light Shotgun, Shock Mine, Pistol, CCW; Minelayer |

### WCD Base Operators

**ID 1765 · AVA 2 · MI** — `MOV 15-5 | CC 14 | BS 11 | PH 11 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. Courage, Dodge (+2.5), Exrah, Super-Jump (Jet Propulsion).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 17 | 0 | Combi Rifle, Light Shotgun, Pistol, CCW | Combined Army max 2 |
| 2 | 19 | 0 | MULTI Rifle (+1B), Pistol, CCW | same |
| 3 | 20 | 0 | Mk12, Pistol, CCW | same |
| 4 | 18 | 0.5 | Heavy Shotgun, Pistol, CCW; Hacking Device, Hacker | same |
| 5 | 17 | 0 | Heavy Shotgun, D-Charges, Pistol, CCW; GizmoKit, Engineer | same |

### WCD Void Operators

**ID 1764 · AVA 2 · MI** — `MOV 15-5 | CC 17 | BS 12 | PH 11 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 2`. X-Visor, 360º Visor, Courage, Dodge (+2.5), NCO, Terrain (Zero-G), Exrah, Super-Jump (Jet Propulsion).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Heavy Shotgun, E/M Grenades, Pistol, CCW | Combined Army max 2 |
| 2 | 26 | 1 | Red Fury, Pistol, CCW | same |
| 3 | 26 | 0 | Combi Rifle, Light Rocket Launcher, Pistol, CCW | same |
| 4 | 20 | 0 | SMG, Cybermine, Pistol, CCW; Killer Hacking Device, Hacker | same |

### The Charontids

**ID 498 · AVA 1 · HI** — `MOV 15-5 | CC 17 | BS 14 | PH 13 | WIP 16 | ARM 5 | BTS 6 | W 2 | S 5`. ECM: Hacker (-3), X-Visor, Courage, Mnemonica, No Wound Incapacitation, Dodge (+2.5).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 67 | 0 | Plasma Rifle, Pulzar (+1B), AP Heavy Pistol, Shock CCW (PS 7); MSV3 |
| 2 | 70 | 1.5 | AP HMG, Pulzar (+1B), AP Heavy Pistol, Shock CCW; MSV3 |
| 4 | 69 | 0.5 | Plasma Rifle, Sepsitor Plus, Pulzar (+1B), AP Heavy Pistol, Shock CCW; Hacking Device Plus, Hacker |
| 5 | 67 | 0 | Lieutenant; Plasma Rifle profile with MSV3 |
| 6 | 70 | 1 | Lieutenant; AP HMG profile with MSV3 |
| 9 | 71 | 0.5 | Lieutenant (+1 Order); Hacking Device Plus; Plasma Rifle, Sepsitor Plus, Pulzar (+1B), AP Heavy Pistol, Shock CCW; Hacker |

### Rodok, Morat Armed Imposition Detachment

**ID 497 · AVA 3 · MI** — `MOV 10-10 | CC 17 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 6 | W 1 | S 2`. Mimetism (-3), Terrain (Jungle), Religious Troop, Warhorse, Combat Instinct, Super-Jump.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4 | 29 | 1.5 | Missile Launcher, Light Shotgun, Heavy Pistol, CCW | Morat max 3 |
| 5 | 23 | 0 | Thunderbolt (+1B), Heavy Pistol, CCW | same |
| 6 | 24 | 0 | AP SMG, E/Mitter, Heavy Pistol, CCW; Strategic Deployment | same |
| 7 | 24 | 0 | Boarding Shotgun, Heavy Pistol, CCW; Hacking Device with Trinity upgrade, Hacker | same |
| 8 | 21 | 0 | Boarding Shotgun, Heavy Pistol, CCW; MediKit, Paramedic | same |
| 11 | 29 | 1.5 | Spitfire, Heavy Pistol, CCW; X-Visor | same |

### Achilles

**ID 1863 · AVA 1 · HI** — `MOV 15-10 | CC 24 | BS 15 | PH 15 | WIP 15 | ARM 3 | BTS 6 | W 3 | S 2`. Nanoscreen; Martial Arts L4, BS Attack (SR-1), Courage, Forward Deployment (+10), Dodge (+5), Mimetism (-3), Stealth, No Cover, Frenzy.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 62 | 2 | AP Spitfire, Pulzar, Pistol, EXP CCW (PS 5) |
| 2 | 63 | 1 | Plasma Rifle, Pulzar, Pistol, EXP CCW; X-Visor |

### Mentor

**ID 1292 · AVA 1 · LI** — `MOV 10-10 | CC 16 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 6 | W 1 | S 2`. Shasvastii, Surprise Attack (-3), Camouflage, Mimetism (-3), Stealth, Decoy, Counterintelligence.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 20 | 0 | Vulkan Shotgun, Breaker Pistol, CCW |
| 2 | 24 | 0 | Shock Marksman Rifle, Breaker Pistol, CCW |
| 3 | 25 | 0.5 | Vulkan Shotgun, Breaker Pistol, CCW; Hacking Device, Hacker |

### Dartok Cybercombat Team

**ID 1572 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 11 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Religious Troop, Warhorse, Dogged; Hacking Device with source Trinity upgrade.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 23 | 0.5 | Combi Rifle, Pitcher, Cybermine, Heavy Pistol, CCW; Hacker, Firewall (-3) | Morat max 1 |

### Umbra Samaritan Nourkias, Kai'l Rank

**ID 1513 · AVA 1 · LI** — `MOV 15-5 | CC 25 | BS 12 | PH 12 | WIP 15 | ARM 2 | BTS 3 | W 1 | S 2`. Hacking Device with source Total Control/Trinity upgrades; Martial Arts L4, Courage, Dodge modifiers, Protheion, Stealth, Super-Jump, No Wound Incapacitation, Immunity (ARM), NCO.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 3 | 48 | 1 | K1 Combi Rifle, Flash Pulse (PS 5), Pistol, Vorpal CCW, E/M CCW (PS 6); Hacker | Combined Army max 1; Overdron max 1 |
| 6 | 46 | 1 | Lieutenant; same weapon/hacking package | same |

### Shasvastii Seed-Soldiers

**ID 512 · AVA 2 · LI** — one logical unit with Seed-Embryo and developed states.

| State | MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Seed-Embryo | — | 10 | 1 | 11 | — | 2 | 3 | 1 | 0 |
| Developed | 10-10 | 16 | 11 | 11 | 13 | 0 | 3 | 1 | 2 |

Seed-Embryo carries the source Shasvastii/Camouflage/Forward Deployment/Mimetism/Transmutation package and can use only its Seed-state permitted weapons; developed state is the same roster entry after transformation.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 15 | 0 | Boarding Shotgun, Panzerfaust, Chest Mine, Boarding Pistol, PARA CCW |
| 2 | 16 | 0 | Combi Rifle, Panzerfaust, Chest Mine, Pistol, PARA CCW |
| 3 | 17 | 0 | Combi Rifle, Panzerfaust, Chest Mine, Flash Pulse, Pistol, PARA CCW; Forward Observer |
| 4 | 18 | 0 | Combi Rifle, Panzerfaust, Chest Mine, Pistol, PARA CCW; MediKit, Paramedic |

### Aïda Swanson, Submondo Smuggler

**ID 1160 · AVA 1 · LI** — `MOV 10-10 | CC 19 | BS 12 | PH 11 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Martial Arts L2, Courage, Booty, Forward Deployment (+10), Mimetism (-3), Shasvastii, Stealth.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 0.5 | SMG (+1B), Viral Mine, Viral Pistol, Shock CCW (PS 7); Minelayer, Decoy | — |
| 2 | 21 | 0 | **AÏDA SWANSON FTO**; SMG, Viral Mine, Viral Pistol, Shock CCW (PS 7); Minelayer | —; no vanilla chart row |

### Bit & KISS!

**ID 965 · AVA 1** — Bit is `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 6 | W 1 | S 2`; KISS! is a synchronized REM peripheral `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`.

| Opt | Pts | SWC | Bit loadout / included peripheral |
|---:|---:|---:|---|
| 1 | 25 | 0.5 | SMG, Pitcher, Pistol, CCW; Deployable Repeater, Hacking Device with Trinity, Hacker; includes KISS! (Repeater) variant |
| 2 | 22 | 0.5 | Same personal weapons; Killer Hacking Device with Oblivion, Deployable Repeater, Hacker; includes standard KISS! variant |

Peripheral source profiles: standard KISS! carries Adhesive Launcher Rifle, Pitcher and PARA CCW (-3) with Deployable Repeater; the Repeater-labelled variant carries Adhesive Launcher Rifle and PARA CCW (-3). They are disabled child profiles, not separate roster entries.

### Overdron Batroids

**ID 785 · AVA 1 · TAG** — `MOV 15-5 | CC 16 | BS 13 | PH 13 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`. Albedo (-6), TinBot: ECM Guided (-6), TinBot: Firewall (-3), Courage, Tactical Awareness, Remote Presence and source TAG modifiers.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 62 | 1.5 | HRMC, Boarding Pistol, AP CCW (PS 6); includes Staldron | Overdron Duo: min/max 1 |
| 2 | 59 | 1.5 | Plasma Sniper Rifle (+1B), Boarding Pistol, AP CCW; includes Staldron | same |
| 3 | 51 | 1.5 | Heavy Rocket Launcher (+1B), SMG, Boarding Pistol, AP CCW; includes Staldron | same |

### EXOs, Exrah Executive Officers

**ID 1766 · AVA 1 · MI** — `MOV 15-5 | CC 14 | BS 12 | PH 11 | WIP 14 | ARM 3 | BTS 3 | W 1 | S 2`. Courage, Dodge (+2.5), Exrah, Super-Jump (Jet Propulsion).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 3 | 19 | 0 | Plasma Carbine, Assault Pistol, PARA CCW (-6); X-Visor, Specialist Operative | Combined Army max 1 |
| 4 | 22 | 0 | MULTI Rifle, Nanopulser, Assault Pistol, PARA CCW (-6); X-Visor, Specialist Operative | same |

### Q-Drones

**ID 509 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. 360º Visor, Remote Presence, Courage, Mimetism (-3), Total Reaction.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 25 | 1 | HMG, PARA CCW (-3) |
| 2 | 24 | 1 | Plasma Rifle, PARA CCW (-3) |
| 3 | 20 | 0.5 | Thunderbolt (+1B), PARA CCW (-3) |

### Cadmus-Naish Agent Sheskiin

**ID 533 · AVA 1 · LI** — `MOV 15-10 | CC 24 | BS 15 | PH 15 | WIP 13 | ARM 1 | BTS 3 | W 2 | S 2`. Nanoscreen; Shasvastii, Martial Arts L4, Courage, Dodge (+5), Protheion, BS Attack (SR-2), Stealth, No Cover.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 48 | 0 | MULTI Rifle, Pulzar, D-Charges, AP Heavy Pistol, DA CCW (PS 4) |
| 2 | 50 | 1 | Red Fury, Pulzar, D-Charges, AP Heavy Pistol, DA CCW (PS 4) |
| 3 | 48 | 0 | Lieutenant; MULTI Rifle loadout |
| 4 | 50 | 0.5 | Lieutenant; Red Fury loadout |

### Nexus Operatives

**ID 783 · AVA 2 · MI** — `MOV 10-10 | CC 17 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 6 | W 1 | S 2`. Courage, Dodge (+3), NCO, Number 2, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | AP SMG, E/Mitter, D-Charges, Breaker Pistol, CCW; Chain of Command | Combined Army max 2; source `(Unidron)`; Overdron max 1 |
| 2 | 24 | 0.5 | Same base weapons; Hacking Device with Oblivion (+1B), Hacker | same |
| 3 | 27 | 0.5 | Combi Rifle (+1SD), Zapper, D-Charges, E/M Mine, Breaker Pistol, CCW; Hacking Device with Carbonite (+1B), Hacker | same |
| 5 | 23 | 0 | AP SMG, E/Mitter, D-Charges, Breaker Pistol, CCW; Deactivator, GizmoKit, Engineer | same |
| 6 | 29 | 1 | Spitfire, Zapper, Breaker Pistol, CCW; Nanoscreen, No Cover | same |
| 7 | 22 | 0 | MULTI Rifle, Zapper, D-Charges, Breaker Pistol, CCW; Specialist Operative | same |
| 9 | 27 | 0.5 | Lieutenant; Combi Rifle (+1SD), Zapper, D-Charges, E/M Mine, Breaker Pistol, CCW; Hacking Device with Carbonite (+1B), Hacker | same |

## Canonical Fireteams

This section is authoritative for standard vanilla Combined Army Fireteam legality. The reverse index below is derivative.

### FT-01 — Combined Army Fireteams

**Types:** Duo, Haris  
**Chart context:** Main Vanilla Combined Army

| Member | Unit ID | Required | Min | Max | Counts as / source note | FTO restriction | Allowed loadout IDs |
|---|---:|---|---:|---:|---|---|---|
| UNIDRON | 493 | no | 0 | 3 | — | — | all |
| BASE OPERATORS | 1765 | no | 0 | 2 | — | — | all |
| VOID OPERATOR | 1764 | no | 0 | 2 | — | — | all |
| NEXUS | 783 | no | 0 | 2 | `(Unidron)` | — | all |
| VECTOR | 1763 | no | 0 | 1 | — | — | all |
| EXO | 1766 | no | 0 | 1 | — | — | all |
| NOURKIAS | 1513 | no | 0 | 1 | — | — | all |
| `--` | — | no | 0 | 1 | `Spec-Ops` | optional-mode hook | not inferred |

### FT-02 — MORAT Fireteam

**Types:** Duo, Haris  
**Chart context:** Main Vanilla Combined Army

| Member | Unit ID | Required | Min | Max | Counts as / note | FTO restriction | Allowed loadout IDs |
|---|---:|---|---:|---:|---|---|---|
| MORAT VANGUARD | 492 | no | 0 | 3 | — | — | all |
| YAOGAT | 518 | no | 0 | 3 | — | — | all |
| RODOK | 497 | no | 0 | 3 | — | — | all |
| DARTOK | 1572 | no | 0 | 1 | — | — | all |
| RINDAK FTO | 1575 | no | 0 | 1 | — | **FTO** | option 1 only |

### FT-03 — Overdron Fireteams

**Type:** Duo  
**Chart context:** Main Vanilla Combined Army

| Member | Unit ID | Required | Min | Max | Counts as / note | FTO restriction | Allowed loadout IDs |
|---|---:|---|---:|---:|---|---|---|
| OVERDRON | 785 | no | 1 | 1 | At least one Overdron due source minimum | — | all |
| NOURKIAS | 1513 | no | 0 | 1 | — | — | all |
| NEXUS | 783 | no | 0 | 1 | — | — | all |
| `--` | — | no | 0 | 1 | `Spec-Ops` | optional-mode hook | not inferred |

### Wildcards

| Unit | Unit ID | Max | Counts as / source note | FTO/profile restriction |
|---|---:|---:|---|---|
| UMBRA LEGATE | 495 | 1 | source comment `FTO` | options 3, 4, 5, 6, 9 only |
| VICTOR MESSER | 1299 | 1 | unrestricted Wildcard row | all vanilla options |

## Reverse Fireteam index

| Unit | Effective vanilla Fireteam access |
|---|---|
| Unidron Batroids | FT-01 Combined Army Duo/Haris, max 3 |
| WCD Base Operators | FT-01 Combined Army Duo/Haris, max 2 |
| WCD Void Operators | FT-01 Combined Army Duo/Haris, max 2 |
| Nexus Operatives | FT-01 Combined Army Duo/Haris max 2, source `(Unidron)`; FT-03 Overdron Duo max 1 |
| WCD Vector Operators | FT-01 Combined Army Duo/Haris max 1 |
| EXOs | FT-01 Combined Army Duo/Haris max 1 |
| Nourkias | FT-01 Combined Army Duo/Haris max 1; FT-03 Overdron Duo max 1 |
| Morat Vanguard Infantry | FT-02 Morat Duo/Haris max 3 |
| Yaogat Strike Infantry | FT-02 Morat Duo/Haris max 3 |
| Rodok | FT-02 Morat Duo/Haris max 3 |
| Dartok Cybercombat Team | FT-02 Morat Duo/Haris max 1 |
| Rindak FTO | FT-02 Morat Duo/Haris max 1; option 1 only |
| Overdron Batroids | FT-03 Overdron Duo; exactly one Overdron base member |
| Umbra Legate FTO | Wildcard max 1; options 3, 4, 5, 6, 9 only |
| Victor Messer | Wildcard max 1; all vanilla options |
| Optional Spec-Ops hook | FT-01 max 1 and FT-03 max 1 when the applicable optional mode is in use; source does not identify the `--` row beyond `Spec-Ops` |

## Reinforcement linkage

The pinned Combined Army source links Reinforcement army **699**. The standard source also records one-to-one relations between standard Ko Dali / Sheskiin and their Reinforcement counterparts. This reference deliberately keeps Reinforcement roster entries and Reinforcement-specific Fireteams separate from the standard Vanilla Combined Army roster and chart.

## Source pinning

- Army source version: `7.26246.158`
- Army data changed on: `2026-09-03`
- Army backup commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`
- Army source blob: `b93bf73c1e3a09f81ea883e9440b6915865eb3e6`
- InfinityDB commit: `4e2662be3f43387fbae42b3790a711b3e98570c4`
- Rules baseline: N5.3 + N5 FAQ v0.1
- Verified/generated: `2026-10-15`

## Validation notes

- Standard roster count: **52 logical units**, excluding the three optional-mode records and generic catalog entries with `factions: []`.
- Faction-listed Armand, Krakot Renegades, Libertos and Aïda Swanson are included; later generic `merc-*` catalog duplicates with no faction assignment are not.
- Canonical Fireteam limits are Core 0, Haris 1, Duo 2.
- Vanilla Combined Army Fireteams are source-defined and are not inferred from sectorial Fireteam charts.
- Rindak's Morat Fireteam row is specifically `RINDAK FTO`; only vanilla option 1 qualifies.
- Umbra Legate is a Wildcard only through FTO-labelled vanilla options 3, 4, 5, 6 and 9.
- Aïda Swanson FTO does not receive vanilla Fireteam access because she has no row in the vanilla chart.
- The source `--` / `Spec-Ops` row is preserved without guessing which optional-mode record it represents.
- Seed-Soldier states, Armand states and Sartroid connected/autonomous states are represented as profile states rather than extra roster units.
- Ancillary/peripheral profiles (Scindron, Staldron, KISS!) are represented through their parent unit and do not inflate the standard roster count.
- The source marks Sartroid Ranters/Puzzlers as Peripheral (Cyberplug); this file does not invent an additional top-level controller relation that is not encoded in the snapshot.
- Reinforcement army 699 is linked but not merged into the standard roster or canonical Fireteam chart.

## Expanded Vanilla Combined tactical guide (2026-10-23)

The [Vanilla Combined Army N5.3 tactical/list-building guide](../../notes/factions/vanilla-combined-army.md) compares middleweight packages with Avatar/Anathematic/Charontid, Vector+Unidron/Nexus, Overdron TAG builds and hidden threats. **Charontid MSV3 guns and HD+/Sepsitor options are distinct loadouts.** Vanilla has **Duo/Haris, no standard Core** and current TAG options **Avatar, Overdron, Sphinx, Caskuda** only.

## Command-unit apex/value cross-reference (2026-10-23)

**Avatar LT 122/3** has the game's extreme Strategos L2/Mnemonica/TacAware command ceiling but is vulnerable to cheap-Order attrition; **Mnemonica transfers LT after entering Null, not Isolation**. **Anathematic 70–74 LT** favors strong hacking with Mnemonica, and **Charontid 67 MSV3 LT or 71 HD+ LT(+1)** has **different legal loadouts**. **Nexus CoC 23/0** is a top multifunctional successor for eligible Unidron/Overdron teams. Don't count Avatar's Strategic Orders and NCO twice.

See [cross-game Lieutenant, CoC and Order-economy tiers](../../notes/list-building/command-units-apex-and-value.md). **Current pinned profiles and Fireteam chart above govern legality.**

## N5.3 mission specialists — apex/value decisions (2026-10-23)

**Malignos FO30/KHD32** reaches hidden enemy-side objective, **Shrouded FO24** is better cheap exposed midfield value, and **Caliban FO26** adds CC/Protheion in legal roster. **M-Drone FO/Sensor15 or TacAware18**, **Med-Tech21 Doctor+Engineer** and **Nexus CoC23/Engineer23/Hacker24** cover distinct mission categories. **Nexus option roles are mutually exclusive**; no Mnemonica on ordinary button-pushers simply from Combined affiliation.

[Cross-game Mission Specialists / Button Pushers tiers](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). The current faction profile and Fireteam reference above controls legality.

## Airborne and enemy-DZ attack choices — N5.3 (2026-10-23)

**Rasyat BSG25/0 or Spitfire34/1.5** is exceptionally efficient **Parachutist(DZ)** plus Eclipse/Warhorse/CC, while **Speculo BSG26/1** threatens catastrophic Monofilament/Impersonation trades but can be killed by prepared mines/templates; **Greif IMP-2 21/.5** is lower-ceiling deception. **Caskuda64/1** has Combat Jump **(PH14 according to pinned Onyx)**, thus **70% basic/85% +3 Controlled Jump**; failed N5.3 jump retreats to **own DZ edge as Model**, not scatter. **Sheskiin LT48–50** is ground-based attack LT, not aerial, and **Caliban CoC is NOT listed in Vanilla CA profile options**—do not import SEF's CoC.

See [current cross-game apex/value, landing odds and expected-trade tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **This roster and Fireteam chart control exact loadout/availability.**

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn gunfighter choice (N5.3):** **Avatar LT122/3** has extreme BS15/Mimetism(-6)/ARM9 command+shooting ceiling but weak *point-value* when support Orders collapse; **Overdron HRMC62/1.5** is the economic **Albedo vs enemy MSV** and AP heavy-gun answer; **Sheskiin MULTI Rifle48/0 or Red Fury50/1** handles short/midrange kill chains and CC/Protheion. **Vector Spitfire26/1.5** solves an MSV2 + Mimetism/smoke lane at a fraction of Avatar points; needs an actual favorable route. **Podcast dissent:** LoL #142 considers Avatar poor value; Robert Shepherd's 2026 analysis emphasizes more affordable supporting guns, without denying Avatar's head-to-head ceiling. [Cross-game tiers and transcripts](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## Warbands and cheap high-upside trading — N5.3

**Dāturazi Chain(+1B)+Smoke14/0** is a **Regular+Impetuous, MA4/Warhorse** smoke engine and anti-CC trader; value rises with Yaogat/other actual legal MSV2 gun. **Gaki4/0** is Explode/AP CC only; **Preta7/0** has Chain Rifle+Dogged. Cheap melee cannot guaranteed-hit a 3W TAG: plan movement/CC and count AROs. **Rasyat25** is a different *Eclipse enemy-DZ* attacker, not a 14pt Dāturazi profile. Combined TAG/REM don't inherit universal Morat Warhorse immunity. **Caliban CoC Shas-only** should not be imported as Vanilla backup.

[Current cross-game warband apex/value, target counters and LT/CoC tiers](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). Pinned profile choices and canonical Fireteam chart in this roster remain authoritative.

## TAG tactical cross-reference (2026-10-23)

**Avatar** offers the highest standalone command/kill ceiling (Strategos L2, Mnemonica, Mimetism -6, Sepsitor) but costs **122/3 SWC**; keep a scoring spine and protect anti-hacking lanes. **Sphinx (93)** favors Hidden Deployment/climbing/flame flank attacks rather than armor duels. **Overdron HRMC (62)** is a far cheaper long-range pressure platform, and **Caskuda (64)** buys a disruptive Combat Jump vector at the cost of off-table first-turn presence. Prefer the latter two when redundant attackers/specialists are more valuable.

Across all factions, compare **apex power** separately from **points value**, counterplay and mission fit: [N5.3 TAG guide](../../notes/list-building/tags.md). The current unit profiles and canonical Fireteam chart above take precedence over tactical opinions.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Apex single Hacker:** **Anathematics HD + Trinity(+1B) 72/0.5 WIP16** has Hidden Deployment, Mimetism(-6), ARM5/NWI and Mnemonica: a terrifying cyber ambush but expensive as an *Order/points-efficient* network piece. **Charontid HD+ 69/0.5 WIP16** adds White Noise/Sepsitor/Plasma, but **not native Trinity**; buy for combat/command/vision control. **Bit+KISS! HD+Trinity 25/0.5** versus **KHD+Oblivion 22/0.5** compresses attack/control with peripheral-based projection; **Dartok 23/0.5** supplies an inexpensive Pitcher+Trinity alternative. **Malignos KHD 32/0** and **Shrouded KHD 26/0** score under Camo and counter enemy Hackers. An expensive WIP16 champion cannot replace cheap Repeaters or reliable mission specialists.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

Cross-faction [apex and cost-value Order-generator rankings](../../notes/list-building/cheerleaders-and-order-generators.md), circumstance guide and transcript disagreements. **This file remains authoritative for profiles, AVA, Training and Fireteam legality.**

- 6pt Ímetron — best absolute Regular Order/point; mandatory Combat Jump and no weapons restrict defence.
- 7pt R-Drone — cheap transferable Order, Repeater and Flash ARO; uses S3 space and AVA.
- 11pt Ikadron — Regular Baggage/Repeater with 2 light-flamethrower shots; guards lanes better than a bare beacon.
- Dāturazi — Regular smoke/CC/Impetuous pressure where legal; not merely passive cheap Order filler.
- Unidron — more expensive than a Flash REM but adds plasma and a Fireteam body; pay for that specific work.

**When to pick:** Prefer transferable, safe Regular Orders when the Combat Group needs fuel; choose the higher-priced option only when its smoke, template, weapon, repeater, Fireteam function or scoring ability has a real job. Do not count Irregular/Impetuous/Tactical/Lieutenant Orders or Peripheral bodies as interchangeable Regular pool Orders; account for DZ footprint and link/enabler package costs.


## ARO apex/value cross-reference (2026-10-23)

The [N5.3 cross-faction ARO apex/value and matchup study](../../notes/list-building/aro-units-apex-and-value.md) compares hidden missile traps, Neurocinetics/TR, cheap templates/mines, DZ guards and conflicting creator opinions. Consult the **roster and Fireteam chart above** for legally available profiles, SWC, Training and AVA.

- **Noctifer ML** — 30pt hidden launcher, decisive attack from an apparently empty lane; remains vulnerable after revealing and supplies no normal Order while Hidden
- **Q-Drone TR Thunderbolt** — 20pt/0.5SWC and Mimetism(-3), useful reactive presence with Engineer support; won't solo elite active guns
- **R-Drone Flash** — 7pt regular + Repeater and reactive stun threat; value is Order+network+minor tax, not a durable lane
- **Warcor Flash** — 3pt Irregular ARO tax/late-game Stun attempt, not a Regular Order
- **Ikadron Baggage/Flamethrower** — cheap multi-purpose DZ corner guard and Repeater; contributes more than pure filler without being a long gun

**Practical deployment:** put cheap disposable/Flash/DTW or mine pressure on the approach; retain a separate unseen or recoverable threat for the decisive square; avoid exposing a premium active attacker and check opponent Smoke, MSV, hacking, AD and pie-slicing. No automatic order from an off-table Hidden model; Irregular ARO units do not supply generic Regular Orders.
