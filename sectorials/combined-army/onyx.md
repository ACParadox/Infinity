---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 604
sectorial_slug: onyx
sectorial_name: Onyx Contact Force
parent_faction: Combined Army
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Onyx Contact Force roster, standard loadouts, canonical Fireteam chart, and reverse Fireteam index. Nexus-7 Spec-Ops and Combined Army Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# Onyx Contact Force

## Overview and provenance

Repository-native reference for **Onyx Contact Force** roster, profiles, points/SWC, AVA, and Fireteam access.

Sources used:

- Army-derived Onyx source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- Source blob: `aaf63e8d4e0cb3bd1db9e004239dc511362b720f`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **35-unit standard Onyx roster** and the complete Onyx `fireteamChart` in the pinned Army source.
- `Nexus-7 Spec-Ops` and `Combined Army Team-Ops` are optional game-mode content and are listed separately.
- Generic Soldier of Fortune / mercenary-catalog records with `factions: []` are excluded. The sectorial-native Cube Jäger record with Onyx in its faction list is included.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name by itself.
- Structured `required: true` rows in **Onyx Fireteams** are preserved as one required-choice set across Suryats, Kurgats, Umbra Samaritans, and Umbra Legates; they are not interpreted as requiring all four unit types simultaneously.
- Structured `required: true` rows in **Exrah Fireteam** are likewise preserved as a required-choice set between Base Operators and Void Operators.
- The chart uses generic `UMBRA LEGATE` rows rather than an FTO-qualified row, so the Fireteam chart itself does not restrict Umbra Legate access only to loadouts whose display name says FTO.
- Nexus and Kerr-Nau Wildcard access is limited to the source's `(Unidron)` context. Nourkias Wildcard access is limited to Umbra Samaritan, Umbra Legate, and Xeodron contexts.
- The Wildcard chart also contains a source placeholder named `--` with comment `Spec-Ops`, max 1. It is retained as an optional-mode hook rather than assigned to a standard roster unit by inference.
- Sphinx includes a Scindron ancillary Remote. Overdron, Caskuda, and Xeodron include a Staldron ancillary Remote. Bit includes one of the KISS! peripheral variants according to loadout.
- Fraacta has Jump Form and Survival Form profile groups; these are transformation states of one logical unit.
- The source relation pairs standard Ko Dali with Reinforcement Ko Dali; the Reinforcement counterpart remains outside this standard roster.
- Linked Reinforcement army ID: **699**. Reinforcement Fireteams are not merged into the main chart here.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Onyx Contact Force |
| Parent faction | Combined Army |
| Army ID | 604 |
| Rules baseline | N5.3 |
| Standard roster | 35 logical units |
| Reinforcement army | 699 |
| Fireteam chart | yes |

## Fireteam chart limits

| Constraint | Value / wording |
|---|---|
| Core | 1 |
| Haris | 2 |
| Duo | Unlimited (`256` source sentinel) |
| Main/Reinforcement mixing | Reinforcement roster kept separate |
| Required-choice semantics | Onyx: Suryat/Kurgat/Umbra Samaritan/Umbra Legate; Exrah: Base/Void |

## Roster index

| Unit ID | Unit | AVA | Type | Classification | Regularity | Fireteam access |
|---:|---|---:|---|---|---|---|
| 524 | Sphinx | 1 | TAG | Mechanized | Regular + Tactical Awareness | — |
| 516 | Shasvastii Noctifers | 2 | LI | Headquarters | Regular | — |
| 510 | T-Drones | 1 | REM | Support | Regular | — |
| 741 | E-Drones | 1 | REM | Support | Regular | — |
| 495 | Umbra Legates | 3 | MI | Elite | Regular + Tactical Awareness | Unidron Core/Haris; Onyx Core/Haris/Duo required-choice |
| 1516 | Special Operative Ko Dali | 1 | MI | Character | Regular | — |
| 785 | Overdron Batroids | 2 | TAG | Mechanized | Regular + Tactical Awareness | Overdron Duo, 1–2 |
| 1763 | WCD Vector Operators | 1 | MI | Elite | Regular | Exrah Duo/Haris max 1 |
| 508 | M-Drones | 2 | REM | Support | Regular | — |
| 509 | Q-Drones | 1 | REM | Support | Regular | — |
| 526 | Slave Drones | 2 | REM | Support | Peripheral | — |
| 783 | Nexus Operatives | 3 | MI | Spec. Trained | Regular | Wildcard max 3, Unidron context only |
| 527 | Ímetron | 2 | LI | Support | Regular | — |
| 992 | Nexus-7 Operative Kerr-Nau | 1 | MI | Character | Regular | Wildcard max 1, Unidron context only |
| 517 | Kurgat Regiment of Assault Engineers | 2 | MI | Spec. Trained | Regular | Onyx Core/Haris/Duo required-choice max 2 |
| 956 | Cube Jäger | 1 | LI | Mercenary | Irregular | — |
| 532 | Ikadron Batroids | 2 | REM | Support | Regular | — |
| 1873 | Glyph Warcors | 1 | LI | Support | Irregular | — |
| 494 | Fraacta Drop Unit | 3 | MI | Spec. Trained | Regular | — |
| 530 | Suryat Assault Heavy Infantry | 3 | HI | Veteran | Regular | Onyx Core/Haris/Duo required-choice max 3 |
| 1298 | Greif Operators | 1 | SK | Spec. Trained | Regular | — |
| 496 | Maakrep Trackers | 2 | MI | Spec. Trained | Regular | Onyx Core/Haris/Duo max 1 |
| 1624 | Caskuda | 1 | TAG | Mechanized | Regular + Tactical Awareness | — |
| 493 | Unidron Batroids | Total | REM | Line | Regular | Unidron Core/Haris, 1–5 |
| 497 | Rodoks | 5 | MI | Spec. Trained | Regular | Rodok Duo/Haris, 1–3 |
| 765 | Umbra Samaritans | 3 | LI | Elite | Regular | Onyx required-choice max 3; Xeodron max 2 |
| 1513 | Nourkias | 1 | LI | Character | Regular | Wildcard max 1 in Umbra Samaritan/Umbra Legate/Xeodron contexts |
| 502 | Malignos | 2 | SK | Veteran | Regular | — |
| 1764 | WCD Void Operators | 2 | MI | Spec. Trained | Regular | Exrah Duo/Haris required-choice max 2 |
| 1766 | EXOs, Exrah Executive Officers | 1 | MI | Spec. Trained | Regular | — |
| 1765 | WCD Base Operators | 2 | MI | Spec. Trained | Regular | Exrah Duo/Haris required-choice max 2 |
| 507 | Med-Tech Obsidon Medchanoid | 1 | LI | Support | Regular | — |
| 784 | Xeodron Batroids | 4 | TAG | Mechanized | Regular + Tactical Awareness | Xeodron Duo/Haris, 1–3 |
| 965 | Bit & KISS! | 1 | LI/REM | Character | Regular + Peripheral | — |
| 511 | R-Drones | 1 | REM | Support | Regular | — |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Nexus-7 Spec-Ops | 1918 | Spec-Ops | Optional-mode record; source chart exposes a generic max-1 `Spec-Ops` Wildcard placeholder rather than naming this unit directly |
| Combined Army Team-Ops | 1932 | Team-Ops | Optional-mode record; not treated as an ordinary matched-play roster entry |

## Unit details

### Sphinx

**ID 524 · AVA 1 · TAG · Mechanized** — `MOV 15-15 | CC 20 | BS 14 | PH 15 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`. Remote Presence, Camouflage, Hidden Deployment, Mimetism (-6), Surprise Attack (-3), Climbing Plus, Courage, Tactical Awareness, Terrain (Total), BS Attack (SR-1), ECM: Guided (-6), Dodge (PH=11), GizmoKit (PH=13).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 93 | 2 | Spitfire, Heavy Flamethrower (+1B), DA CCW (PS 5); includes Scindron ancillary Remote | — |

### Shasvastii Noctifers

**ID 516 · AVA 2 · LI · Headquarters** — `MOV 10-10 | CC 15 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Shasvastii, Camouflage, Hidden Deployment, Mimetism (-6), Surprise Attack (-3), Stealth, Dogged, Courage; X-Visor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 29 | 1 | Spitfire, Breaker Pistol, CCW | — |
| 3 | 30 | 1.5 | Missile Launcher, Assault Pistol, CCW | — |
| 6 | 31 | 1.5 | Spitfire, Breaker Pistol, CCW; Forward Deployment (+10) | — |

### T-Drones

**ID 510 · AVA 1 · REM · Support** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CCW (-3); BS Attack (Guided) | — |

### E-Drones

**ID 741 · AVA 1 · REM · Support** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage, Terrain (Total); EVO Hacking Device, Hacker.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 17 | 0.5 | Combi Rifle, PARA CCW (-3) | — |

### Umbra Legates

**ID 495 · AVA 3 · MI · Elite** — `MOV 15-5 | CC 22 | BS 13 | PH 12 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Martial Arts L3, Mimetism (-3), NWI, Courage, Stealth, Immunity (Shock), Tactical Awareness, Dodge (+2.5).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 36 | 0 | Vulkan Shotgun (+1B), Zapper, Flash Pulse, Pistol, DA CCW (PS 5); Forward Deployment (+20) | Unidron; Onyx required-choice |
| 2 | 41 | 1.5 | Spitfire, Zapper, Flash Pulse, Pistol, DA CCW (PS 5); Forward Deployment (+20) | same |
| 3 | 33 | 0 | **UMBRA LEGATE FTO**; K1 Combi Rifle, Zapper, Flash Pulse, Pistol, DA CCW (PS 5) | same |
| 4 | 37 | 1.5 | **UMBRA LEGATE FTO**; Spitfire, Zapper, Flash Pulse, Pistol, DA CCW (PS 5) | same |
| 5 | 38 | 0 | **UMBRA LEGATE FTO**; K1 Combi Rifle, Zapper, D-Charges, Flash Pulse, Pistol, DA CCW; Chain of Command | same |
| 6 | 38 | 0.5 | **UMBRA LEGATE FTO**; K1 Combi Rifle, Zapper, D-Charges, Flash Pulse, Pitcher, Pistol, DA CCW; Hacking Device Plus, Hacker | same |
| 7 | 42 | 0.5 | Vulkan Shotgun (+1B), Zapper, Flash Pulse, Pistol, DA CCW; Hacking Device Plus, Deployable Repeater, Hacker, Forward Deployment (+20) | same |
| 8 | 33 | 0 | **UMBRA LEGATE FTO**; K1 Combi Rifle, Zapper, Flash Pulse, Pistol, DA CCW; Lieutenant | same |
| 9 | 37 | 1.5 | **UMBRA LEGATE FTO**; Spitfire, Zapper, Flash Pulse, Pistol, DA CCW; Lieutenant | same |
| 10 | 36 | 0 | Vulkan Shotgun (+1B), Zapper, Flash Pulse, Pistol, DA CCW; Lieutenant, Forward Deployment (+20) | same |

The chart rows say `UMBRA LEGATE` rather than `UMBRA LEGATE FTO`; therefore this reference does not infer an FTO-only restriction.

### Special Operative Ko Dali

**ID 1516 · AVA 1 · MI · Character** — `MOV 15-5 | CC 19 | BS 14 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Martial Arts L3, MSV2, Courage, Dodge (+5), Immunity (ARM), Protheion, Stealth, Specialist Operative.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 37 | 0 | MULTI Rifle, Pulzar, D-Charges, Assault Pistol (+1B), AP CCW; Parachutist, Combat Jump, Super-Jump (Jet Propulsion) | — |
| 2 | 34 | 0 | MULTI Rifle, Pulzar, D-Charges, Assault Pistol (+1B), AP CCW; Forward Deployment (+20), Mimetism (-3) | — |

### Overdron Batroids

**ID 785 · AVA 2 · TAG · Mechanized** — `MOV 15-5 | CC 16 | BS 13 | PH 13 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`. Remote Presence, Courage, Tactical Awareness, BS Attack (SR-1), Dodge (PH=11); Albedo (-6), TinBot: ECM Guided (-6), TinBot: Firewall (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 62 | 1.5 | Hyper-Rapid Magnetic Cannon, Boarding Pistol, AP CCW (PS 6); includes Staldron | Overdron Duo, 1–2 |
| 2 | 59 | 1.5 | Plasma Sniper Rifle (+1B), Boarding Pistol, AP CCW (PS 6); includes Staldron | same |
| 3 | 51 | 1.5 | Heavy Rocket Launcher (+1B), SMG, Boarding Pistol, AP CCW (PS 6); includes Staldron | same |

### WCD Vector Operators

**ID 1763 · AVA 1 · MI · Elite** — `MOV 15-5 | CC 14 | BS 12 | PH 11 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 2`. MSV2, Courage, Mimetism (-3), Terrain (Total), Exrah, Super-Jump (Jet Propulsion), Dodge (+2.5).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Heavy Shotgun, D-Charges, Shock Mine, Pistol, CCW | Exrah max 1 |
| 2 | 24 | 0.5 | MULTI Marksman Rifle, Pistol, CCW | same |
| 3 | 26 | 1.5 | Spitfire, Pistol, CCW | same |
| 4 | 29 | 1.5 | Plasma Sniper Rifle, Pistol, CCW | same |

### M-Drones

**ID 508 · AVA 2 · REM · Support** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Triangulated Fire, Courage, Forward Observer, Terrain (Total), Sensor; Deactivator, Repeater.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 15 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3) | — |
| 3 | 18 | 0 | Same; Tactical Awareness | — |

### Q-Drones

**ID 509 · AVA 1 · REM · Support** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage, Mimetism (-3), Total Reaction; 360º Visor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 25 | 1 | HMG, PARA CCW (-3) | — |
| 2 | 24 | 1 | Plasma Rifle, PARA CCW (-3) | — |
| 3 | 20 | 0.5 | Thunderbolt (+1B), PARA CCW (-3) | — |

### Slave Drones

**ID 526 · AVA 2 · REM · Support** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Peripheral (Servant), Courage, Mimetism (-3); no Order of its own.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | PARA CCW (-3) | — |

### Nexus Operatives

**ID 783 · AVA 3 · MI · Spec. Trained** — `MOV 10-10 | CC 17 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 6 | W 1 | S 2`. Courage, Dodge (+3), NCO, Number 2, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | AP SMG, E/Mitter, D-Charges, Breaker Pistol, CCW; Chain of Command | Wildcard max 3, Unidron context |
| 2 | 24 | 0.5 | Same weapons; Hacking Device (Oblivion +1B), Hacker | same |
| 3 | 27 | 0.5 | Combi Rifle (+1SD), Zapper, D-Charges, E/M Mine, Breaker Pistol, CCW; Hacking Device (Carbonite +1B), Hacker | same |
| 5 | 23 | 0 | AP SMG, E/Mitter, D-Charges, Breaker Pistol, CCW; Engineer, Deactivator, GizmoKit | same |
| 6 | 29 | 1 | Spitfire, Zapper, Breaker Pistol, CCW; Nanoscreen, No Cover | same |
| 7 | 22 | 0 | MULTI Rifle, Zapper, D-Charges, Breaker Pistol, CCW; Specialist Operative | same |
| 8 | 19 | 0 | MULTI Rifle, Zapper, D-Charges, Breaker Pistol, CCW; Lieutenant, Specialist Operative | same |
| 9 | 27 | 0.5 | Combi Rifle (+1SD), Zapper, D-Charges, E/M Mine, Breaker Pistol, CCW; Lieutenant, Hacking Device (Carbonite +1B), Hacker | same |

### Ímetron

**ID 527 · AVA 2 · LI · Support** — immobile deployment unit: `CC — | BS — | PH — | WIP — | ARM 0 | BTS 3 | W 1 | S 2`. Warhorse, Religious Troop; must deploy by Combat Jump during the Deployment Phase.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 6 | 0 | No weapons; Combat Jump (PH=12) | — |

### Nexus-7 Operative Kerr-Nau

**ID 992 · AVA 1 · MI · Character** — `MOV 10-10 | CC 16 | BS 12 | PH 11 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. Courage, Dodge (+3), Immunity (ARM), NCO; X-Visor, Killer Hacking Device with White Noise upgrade.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 30 | 0 | Plasma Rifle, D-Charges, Pitcher, Breaker Pistol, CCW; Hacker | Wildcard max 1, Unidron context |
| 2 | 35 | 0 | Plasma Rifle, Pitcher, D-Charges, Boarding Pistol, CCW; Nanoscreen, No Cover, Hacker | same |

### Kurgat Regiment of Assault Engineers

**ID 517 · AVA 2 · MI · Spec. Trained** — `MOV 10-10 | CC 18 | BS 12 | PH 12 | WIP 13 | ARM 2 | BTS 6 | W 1 | S 2`. Engineer, Warhorse, Religious Troop; Deactivator, GizmoKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 30 | 1 | Portable Autocannon, D-Charges, Heavy Pistol, CCW | Onyx required-choice max 2 |
| 2 | 19 | 0 | Boarding Shotgun, D-Charges, Drop Bears, Heavy Pistol, CCW | same |
| 3 | 22 | 0 | Boarding Shotgun, D-Charges, AP Mine, Armed Turret (Marksman Rifle), Heavy Pistol, CCW | same |
| 4 | 19 | 0 | Boarding Shotgun, D-Charges, Panzerfaust, Heavy Pistol, CCW | same |
| 5 | 25 | 0 | Combi Rifle (AP source modifier), E/Mitter, D-Charges, AP Mine, Heavy Pistol, CCW; BS Attack (SR-1) | same |

### Cube Jäger

**ID 956 · AVA 1 · LI · Mercenary** — `MOV 10-10 | CC 16 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Parachutist, Immunity (Shock), Stealth; MediKit. Irregular.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 15 | 0 | Boarding Shotgun, Pistol, Monofilament CCW; Paramedic | — |
| 2 | 18 | 0 | SMG, E/Mitter, Pistol, Monofilament CCW; Paramedic | — |

### Ikadron Batroids

**ID 532 · AVA 2 · REM · Support** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 2`. Remote Presence, Courage, Discover (+3), Dodge (+2.5), Dogged; Baggage, Repeater.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 11 | 0 | Light Flamethrower (+1B), Pistol, PARA CCW (-3) | — |

### Glyph Warcors, Ur Hegemony Journalists

**ID 1873 · AVA 1 · LI · Support** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Dodge (+3), Journalist. Irregular.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 4 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor | — |
| 2 | 4 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); Sixth Sense | — |

### Fraacta Drop Unit

**ID 494 · AVA 3 · MI · Spec. Trained** — Jump Form: `MOV 10-10 | CC 15 | BS 12 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 2 | S 2`; Survival Form: same CC/BS/WIP/S, `PH 10 | ARM 2 | BTS 6 | W 2`. Courage, Parachutist, Combat Jump, Super-Jump (Jet Propulsion), Transmutation.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1759 | 19 | 0 | Boarding Shotgun, Adhesive Launcher Rifle, D-Charges, Pistol, CCW | — |
| 1760 | 27 | 1.5 | Spitfire, Nanopulser, Pistol, CCW | — |
| 1761 | 25 | 0.5 | Combi Rifle, Nanopulser, D-Charges, Pistol, CCW; Hacking Device, Hacker | — |

### Suryat Assault Heavy Infantry

**ID 530 · AVA 3 · HI · Veteran** — `MOV 10-10 | CC 17 | BS 13 | PH 13 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 2`. Warhorse, Religious Troop, Immunity (AP), Terrain (Jungle).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 34 | 0 | Vulkan Shotgun, MULTI Pistol, CCW (PS 7) | Onyx required-choice max 3 |
| 3 | 36 | 0 | MULTI Rifle, Light Flamethrower, MULTI Pistol, CCW (PS 7) | same |
| 4 | 36 | 1.5 | Heavy Rocket Launcher, MULTI Pistol (+1B), CCW (PS 7); MSV1, TinBot: Firewall (-3) | same |
| 6 | 43 | 1.5 | HMG, MULTI Pistol, CCW (PS 7); Tactical Awareness | same |
| 7 | 44 | 1.5 | HMG, MULTI Pistol, CCW (PS 7); Tactical Awareness, TinBot: Firewall (-3) | same |
| 9 | 45 | 1.5 | HMG, MULTI Pistol, CCW (PS 7); Lieutenant (+1 Order), TinBot: Firewall (-3) | same |

### Greif Operators

**ID 1298 · AVA 1 · SK · Spec. Trained** — `MOV 10-10 | CC 17 | BS 11 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Courage, Stealth; MSV1.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Combi Rifle, D-Charges, Breaker Pistol (+1B), CCW, Viral Mine; Forward Deployment (+20), Mimetism (-6) | — |
| 2 | 25 | 0 | Shock Marksman Rifle, D-Charges, Breaker Pistol (+1B), CCW; Forward Deployment (+20), Mimetism (-6) | — |
| 3 | 21 | 0.5 | Breaker Combi Rifle, D-Charges, Silenced Pistol (+1B), CCW; Surprise Attack (-3), Impersonation (IMP-2) | — |

### Maakrep Trackers Unit

**ID 496 · AVA 2 · MI · Spec. Trained** — `MOV 10-10 | CC 15 | BS 12 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Courage, Sixth Sense, Combat Instinct, Regeneration (PH=14); MSV2.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 29 | 1.5 | HMG, Breaker Pistol, CCW | Onyx max 1 |
| 3 | 19 | 0 | Boarding Shotgun, Grenades, Breaker Pistol, CCW | same |
| 4 | 27 | 1.5 | MULTI Sniper Rifle, Breaker Pistol, CCW | same |

### Caskuda WCD Armored Jump Operator

**ID 1624 · AVA 1 · TAG · Mechanized** — `MOV 15-10 | CC 18 | BS 14 | PH 16 | WIP 12 | ARM 7 | BTS 6 | W 3 | S 7`. Remote Presence, Courage, Tactical Awareness, Combat Jump (PH=14 / Explosion), BS Attack (SR-2, +1B), Dodge (PH=12), GizmoKit (PH=12), ECM: Guided (-6).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 64 | 1 | MULTI Rifle, Chain Rifle, E/M CCW (PS 4); includes Staldron | — |

### Unidron Batroids

**ID 493 · AVA Total · REM · Line** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 12 | ARM 1 | BTS 6 | W 1 | S 2`. Remote Presence, Courage, Dogged, Discover (+3), Dodge (+2.5).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Plasma Carbine, Pistol, PARA CCW (-3) | Unidron Core/Haris, 1–5 |
| 2 | 14 | 0 | K1 Combi Rifle, Pistol, PARA CCW (-3) | same |
| 3 | 15 | 0.5 | K1 Combi Rifle, Pistol, PARA CCW (-3); TinBot: Firewall (-3) | same |
| 4 | 24 | 1.5 | Plasma Sniper Rifle, Pistol, PARA CCW (-3) | same |
| 5 | 20 | 1.5 | Missile Launcher, Light Shotgun, Pistol, PARA CCW (-3) | same |
| 6 | 18 | 1 | Spitfire, Pistol, PARA CCW (-3) | same |
| 7 | 15 | 0 | Plasma Carbine, Flash Pulse, Pistol, PARA CCW (-3); Forward Observer | same |
| 8 | 16 | 0 | Plasma Carbine, Pistol, PARA CCW (-3); Commlink (+1), Specialist Operative | same |

### Rodok, Morat Armed Imposition Detachment

**ID 497 · AVA 5 · MI · Spec. Trained** — `MOV 10-10 | CC 17 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 6 | W 1 | S 2`. Mimetism (-3), Terrain (Jungle), Religious Troop, Warhorse, Combat Instinct, Super-Jump (+7.5).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4 | 29 | 1.5 | Missile Launcher, Light Shotgun, Heavy Pistol, CCW | Rodok Duo/Haris, 1–3 |
| 5 | 23 | 0 | Thunderbolt (+1B), Heavy Pistol, CCW | same |
| 6 | 24 | 0 | AP SMG, E/Mitter, Heavy Pistol, CCW; Strategic Deployment | same |
| 7 | 24 | 0 | Boarding Shotgun, Heavy Pistol, CCW; Hacking Device (Trinity), Hacker | same |
| 8 | 21 | 0 | Boarding Shotgun, Heavy Pistol, CCW; MediKit, Paramedic | same |
| 11 | 29 | 1.5 | Spitfire, Heavy Pistol, CCW; X-Visor | same |

### Umbra Samaritans

**ID 765 · AVA 3 · LI · Elite** — `MOV 15-5 | CC 24 | BS 12 | PH 12 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. Martial Arts L4, Protheion, Super-Jump, NWI, Courage, Immunity (Shock), Stealth, NCO. The structured source carries Dodge modifiers of both +5 and +3; both are preserved as source data rather than collapsed.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 6 | 37 | 0 | Plasma Rifle, Pulzar, Flash Pulse, Pistol, Vorpal CCW, DA CCW (PS 6) | Onyx required-choice max 3; Xeodron max 2 |
| 7 | 43 | 0.5 | Same; Hacking Device + Killer Hacking Device, Hacker | same |
| 8 | 35 | 0 | Same; Lieutenant | same |

### Umbra Samaritan Nourkias, Kai'l Rank

**ID 1513 · AVA 1 · LI · Character** — `MOV 15-5 | CC 25 | BS 12 | PH 12 | WIP 15 | ARM 2 | BTS 3 | W 1 | S 2`. Martial Arts L4, Protheion, Super-Jump, NWI, Courage, Stealth, Immunity (ARM), NCO; Hacking Device with Total Control (PS=3) and Trinity (PS=5) upgrades.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 48 | 1 | K1 Combi Rifle, Flash Pulse (PS 5 source modifier), Pistol, Vorpal CCW, E/M CCW (PS 6); Hacker | Wildcard max 1: Umbra Samaritan/Umbra Legate/Xeodron contexts |
| 5 | 46 | 1 | Same; Lieutenant, Hacker | same |

### Malignos

**ID 502 · AVA 2 · SK · Veteran** — `MOV 15-5 | CC 15 | BS 12 | PH 12 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Shasvastii, Camouflage, Hidden Deployment, Mimetism (-6), Surprise Attack (-3), Infiltration, Terrain (Total), Regeneration, Stealth.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 31 | 0.5 | SMG, Viral Mine, Silenced Pistol, CCW; Minelayer | — |
| 3 | 30 | 0 | Boarding Shotgun, Pulzar (+1B), Viral Mine, Silenced Pistol, CCW | — |
| 4 | 33 | 1.5 | MULTI Sniper Rifle, Pulzar, Silenced Pistol, CCW | — |
| 5 | 34 | 0.5 | SMG, D-Charges, Shock Mine, Silenced Pistol, CCW; Hacking Device, Hacker | — |
| 6 | 30 | 0 | SMG, Flash Pulse, D-Charges, Shock Mine, Silenced Pistol, CCW; Forward Observer | — |
| 8 | 32 | 0 | SMG, D-Charges, Shock Mine, Silenced Pistol, CCW; Killer Hacking Device, Dazer, Hacker | — |

### WCD Void Operators

**ID 1764 · AVA 2 · MI · Spec. Trained** — `MOV 15-5 | CC 17 | BS 12 | PH 11 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 2`. Courage, Dodge (+2.5), NCO, Terrain (Zero-G), Exrah, Super-Jump (Jet Propulsion); X-Visor, 360º Visor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Heavy Shotgun, E/M Grenades, Pistol, CCW | Exrah required-choice max 2 |
| 2 | 26 | 1 | Red Fury, Pistol, CCW | same |
| 3 | 26 | 0 | Combi Rifle, Light Rocket Launcher, Pistol, CCW | same |
| 4 | 20 | 0 | SMG, Cybermine, Pistol, CCW; Killer Hacking Device, Hacker | same |

### EXOs, Exrah Executive Officers

**ID 1766 · AVA 1 · MI · Spec. Trained** — `MOV 15-5 | CC 14 | BS 12 | PH 11 | WIP 14 | ARM 3 | BTS 3 | W 1 | S 2`. Courage, Dodge (+2.5), Exrah, Super-Jump (Jet Propulsion); No Cube.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0.5 | Plasma Carbine, Pistol, PARA CCW (-6); Chain of Command | — |
| 2 | 22 | 0.5 | MULTI Rifle, Nanopulser, Pistol, PARA CCW (-6); Chain of Command | — |
| 3 | 19 | 0 | Plasma Carbine, Assault Pistol, PARA CCW (-6); X-Visor, Specialist Operative | — |
| 4 | 22 | 0 | MULTI Rifle, Nanopulser, Assault Pistol, PARA CCW (-6); X-Visor, Specialist Operative | — |

### WCD Base Operators

**ID 1765 · AVA 2 · MI · Spec. Trained** — `MOV 15-5 | CC 14 | BS 11 | PH 11 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. Courage, Dodge (+2.5), Exrah, Super-Jump (Jet Propulsion).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 17 | 0 | Combi Rifle, Light Shotgun, Pistol, CCW | Exrah required-choice max 2 |
| 2 | 19 | 0 | MULTI Rifle (+1B), Pistol, CCW | same |
| 3 | 20 | 0 | Mk12, Pistol, CCW | same |
| 4 | 18 | 0.5 | Heavy Shotgun, Pistol, CCW; Hacking Device, Hacker | same |
| 5 | 17 | 0 | Heavy Shotgun, D-Charges, Pistol, CCW; Engineer, GizmoKit | same |

### Med-Tech Obsidon Medchanoid

**ID 507 · AVA 1 · LI · Support** — `MOV 15-10 | CC 16 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 3`. Engineer, Doctor; Deactivator, GizmoKit, MediKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | Combi Rifle, Zapper, D-Charges, Pistol, CCW | — |
| 3 | 22 | 0 | Same; Deployable Cover | — |
| 4 | 24 | 0 | Combi Rifle, Zapper, D-Charges, Armed Turret (Combi Rifle), Pistol, CCW | — |
| 5 | 25 | 0 | Combi Rifle, Zapper, D-Charges, Armed Turret (Marksman Rifle), Pistol, CCW | — |

### Xeodron Batroids

**ID 784 · AVA 4 · TAG · Mechanized** — `MOV 15-5 | CC 17 | BS 13 | PH 13 | WIP 13 | ARM 5 | BTS 6 | W 3 | S 6`. Remote Presence, Courage, Tactical Awareness, Super-Jump, BS Attack (SR-1), Dodge (PH=12); ECM: Guided (-6).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 49 | 0.5 | K1 Marksman Rifle, Blitzen, Heavy Pistol, Shock CCW (PS 7); includes Staldron | Xeodron Duo/Haris, 1–3 |
| 2 | 49 | 0.5 | MULTI Marksman Rifle, Blitzen, Heavy Pistol, Shock CCW (PS 7); includes Staldron | same |
| 3 | 50 | 1 | Red Fury, Blitzen, Heavy Pistol, Shock CCW (PS 7); includes Staldron | same |

### Bit & KISS!

**ID 965 · AVA 1 · Character**. Bit: `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 6 | W 1 | S 2`, Minelayer. KISS!: `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`, REM Peripheral (Synchronized), Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 25 | 0.5 | Bit: SMG, Pitcher, Pistol, CCW; Deployable Repeater; Hacking Device (Trinity), Hacker; includes KISS! (Repeater) | — |
| 3 | 24 | 0.5 | Bit: SMG, Pitcher, Pistol, CCW; Deployable Repeater; Killer Hacking Device (Oblivion), Hacker; includes KISS! | — |

KISS! source variants carry Adhesive Launcher Rifle and either Pitcher (+1B) plus Deployable Repeater or a Repeater configuration, with PARA CCW (-3), as selected by Bit's parent loadout.

### R-Drones

**ID 511 · AVA 1 · REM · Support** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage, Mimetism (-3); Repeater.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) | — |

## Optional-mode profiles

### Nexus-7 Spec-Ops

**ID 1918 · optional Spec-Ops mode.** Initial and enhanced Nexus-7 profile groups plus Voldron 401 SpecBot options are preserved in the Army source. This is not counted in the 35-unit standard roster.

### Combined Army Team-Ops

**ID 1932 · optional Team-Ops mode.** Contains Nexus-7A Spec-Ops, Nexus-7 Heavy Spec-Ops, and Voldron 401 SpecBots. This is not counted in the 35-unit standard roster.

## Canonical Fireteam definitions

Chart-wide limits: **Core 1, Haris 2, Duo unlimited (`256`)**.

### FT-01 — Unidrons Fireteams

**Types:** Haris, Core

| Member | Unit ID | Required | Min | Max | Counts as / note | FTO restriction |
|---|---:|---|---:|---:|---|---|
| UNIDRON | 493 | no | 1 | 5 | — | — |
| UMBRA LEGATE | 495 | no | 0 | 3 | — | none in chart |

### FT-02 — Onyx Fireteams

**Types:** Duo, Haris, Core

| Member | Unit ID | Required-choice | Min | Max | Note | FTO restriction |
|---|---:|---|---:|---:|---|---|
| SURYAT | 530 | yes | 0 | 3 | Onyx required-choice set | — |
| KURGAT | 517 | yes | 0 | 2 | Onyx required-choice set | — |
| UMBRA SAMARITAN | 765 | yes | 0 | 3 | Onyx required-choice set | — |
| UMBRA LEGATE | 495 | yes | 0 | 3 | Onyx required-choice set | none in chart |
| MAAKREP TRACKER | 496 | no | 0 | 1 | — | — |

The four `required: true` rows are treated as a **required-choice set**: a legal Onyx team needs the source-required anchor from this set, but the data is not interpreted as forcing all four unit types into the same team.

### FT-03 — Exrah Fireteam

**Types:** Duo, Haris

| Member | Unit ID | Required-choice | Min | Max | Note |
|---|---:|---|---:|---:|---|
| BASE OPERATORS | 1765 | yes | 0 | 2 | Exrah required-choice set |
| VOID OPERATOR | 1764 | yes | 0 | 2 | Exrah required-choice set |
| VECTOR | 1763 | no | 0 | 1 | — |

The Base/Void `required: true` rows are treated as a required-choice set rather than both being simultaneously mandatory.

### FT-04 — Rodoks Fireteams

**Types:** Duo, Haris

| Member | Unit ID | Required | Min | Max | Note |
|---|---:|---|---:|---:|---|
| RODOK | 497 | no | 1 | 3 | — |

### FT-05 — Xeodrons Fireteams

**Types:** Duo, Haris

| Member | Unit ID | Required | Min | Max | Counts as / note |
|---|---:|---|---:|---:|---|
| XEODRON | 784 | no | 1 | 3 | — |
| UMBRA SAMARITAN | 765 | no | 0 | 2 | source comment `(Xeodron)` |

### FT-06 — Overdrons Fireteams

**Types:** Duo

| Member | Unit ID | Required | Min | Max | Note |
|---|---:|---|---:|---:|---|
| OVERDRON | 785 | no | 1 | 2 | — |

### Wildcards

| Entry | Unit ID | Max | Context / restriction |
|---|---:|---:|---|
| NEXUS | 783 | 3 | Unidron context only; source `(Unidron)` |
| KERR-NAU | 992 | 1 | Unidron context only; source `(Unidron)` |
| NOURKIAS | 1513 | 1 | Umbra Samaritan, Umbra Legate, and Xeodron contexts only |
| `--` | — | 1 | `Spec-Ops` optional-mode placeholder exactly as exposed by source chart |

## Reverse Fireteam index

| Unit | Fireteam access |
|---|---|
| Unidron Batroids | Unidron Core/Haris, 1–5 |
| Umbra Legates | Unidron Core/Haris max 3; Onyx Core/Haris/Duo required-choice max 3; chart does not impose FTO-only restriction |
| Suryats | Onyx Core/Haris/Duo required-choice max 3 |
| Kurgats | Onyx Core/Haris/Duo required-choice max 2 |
| Umbra Samaritans | Onyx Core/Haris/Duo required-choice max 3; Xeodron Duo/Haris max 2 |
| Maakrep Trackers | Onyx Core/Haris/Duo max 1 |
| WCD Base Operators | Exrah Duo/Haris required-choice max 2 |
| WCD Void Operators | Exrah Duo/Haris required-choice max 2 |
| WCD Vector Operators | Exrah Duo/Haris max 1 |
| Rodoks | Rodok Duo/Haris, 1–3 |
| Xeodron Batroids | Xeodron Duo/Haris, 1–3 |
| Overdron Batroids | Overdron Duo, 1–2 |
| Nexus Operatives | Wildcard max 3; Unidron context only |
| Kerr-Nau | Wildcard max 1; Unidron context only |
| Nourkias | Wildcard max 1; Umbra Samaritan/Umbra Legate/Xeodron contexts only |
| Optional Spec-Ops placeholder | Wildcard max 1 only when the relevant optional mode is in use |

## Reinforcement linkage

The pinned Onyx Army data links Reinforcement roster **699**. The source also contains an exclusivity relation between standard Ko Dali (`1516`) and Reinforcement Ko Dali (`1616`). Reinforcement roster entries and Reinforcement-specific Fireteams are deliberately kept separate from the standard Onyx chart.

## Source pinning

- Army source version: `7.26246.158`
- Army data changed on: `2026-09-03`
- Army backup commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`
- Army source blob: `aaf63e8d4e0cb3bd1db9e004239dc511362b720f`
- InfinityDB commit: `4e2662be3f43387fbae42b3790a711b3e98570c4`
- Rules baseline: N5.3 + N5 FAQ v0.1
- Verified/generated: `2026-10-15`

## Validation notes

- Standard roster count: **35 logical units**, excluding Nexus-7 Spec-Ops and Combined Army Team-Ops optional modes and excluding generic mercenary-catalog records with `factions: []`.
- The Onyx-specific Cube Jäger record is included because its faction list explicitly contains Onyx (`604`).
- Canonical Fireteam limits are Core 1, Haris 2, and unlimited Duo (`256` source sentinel).
- Canonical Fireteam families are Unidrons, Onyx, Exrah, Rodoks, Xeodrons, and Overdrons, plus the Wildcard table.
- Onyx Suryat/Kurgat/Umbra Samaritan/Umbra Legate rows are a required-choice set; they are not all simultaneously mandatory.
- Exrah Base/Void rows are a required-choice set; they are not both treated as simultaneously mandatory for every team.
- Umbra Legate Fireteam rows are generic in the chart; no FTO-only limitation is inferred from profile display names.
- Nexus and Kerr-Nau Wildcard access is Unidron-only. Nourkias Wildcard access is limited to Umbra Samaritan, Umbra Legate, and Xeodron contexts.
- The chart's anonymous `--` / `Spec-Ops` Wildcard row is preserved as an optional-mode placeholder instead of being silently mapped to a named standard unit.
- Sphinx/Scindron, Overdron/Staldron, Caskuda/Staldron, Xeodron/Staldron, and Bit/KISS! are represented as parent/peripheral or ancillary relationships, not additional logical roster entries.
- Fraacta Jump Form and Survival Form are profile groups of one logical unit.
- Reinforcement roster 699 is linked but not mixed into the standard roster or Fireteam chart.

## TAG tactical cross-reference (2026-10-23)

**Overdron** is the standout value choice: **51-point HRL+1B**, **59-point Plasma sniper+1B**, or **62-point HRMC**, with TacAware, Albedo and Firewall utility. **Xeodron (49–50)** is a cheap short/mid-ranged TacAware body with K1/Marksmanship-style options and specific legal Duo/Haris access. **Sphinx (93)** is apex flanking/Hidden Deployment but poor AP-efficiency into heavy armor; **Caskuda (64)** is a Combat Jump backline tool. Do not import link allowances between chassis; check the canonical chart.

Across all factions, compare **apex power** separately from **points value**, counterplay and mission fit: [N5.3 TAG guide](../../notes/list-building/tags.md). The current unit profiles and canonical Fireteam chart above take precedence over tactical opinions.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Kerr-Nau KHD + White Noise 30/0** is a rare **0-SWC anti-Hacker + anti-MSV hybrid**, with X-Visor Pitcher, Plasma weapon and NCO: use when the team can *use* both cyber access and fighting. **Bit+KISS! HD+Trinity 25/0.5 or KHD+Oblivion 24/0.5** adds a perimeter/Repeater companion and an actual choice of target class. **Nexus HD + Oblivion(+1B) 24/0.5 / Carbonite(+1B) 27/0.5** supplies cheaper linked anti-heavy control; **Umbra Legate HD+ 38–42/0.5** has White Noise but costs more than a basic cyber backbone. **Malignos KHD32/0** is for Camo scoring. **Why:** KHD/White Noise Kerr-Nau solves an MSV lane and kills hostile hackers; it is not a full HD against HI without Bit/Nexus support.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

Cross-faction [apex and cost-value Order-generator rankings](../../notes/list-building/cheerleaders-and-order-generators.md), circumstance guide and transcript disagreements. **This file remains authoritative for profiles, AVA, Training and Fireteam legality.**

- 6pt Ímetron — best absolute Regular Order/point; mandatory Combat Jump and no weapons restrict defence.
- 7pt R-Drone — cheap transferable Order, Repeater and Flash ARO; uses S3 space and AVA.
- 11pt Ikadron — Regular Baggage/Repeater with 2 light-flamethrower shots; guards lanes better than a bare beacon.
- Unidron — more expensive than a Flash REM but adds plasma and a Fireteam body; pay for that specific work.
- Warcor — Irregular Flash Pulse ARO distraction, NOT a passive transferable Regular Order.

**When to pick:** Prefer transferable, safe Regular Orders when the Combat Group needs fuel; choose the higher-priced option only when its smoke, template, weapon, repeater, Fireteam function or scoring ability has a real job. Do not count Irregular/Impetuous/Tactical/Lieutenant Orders or Peripheral bodies as interchangeable Regular pool Orders; account for DZ footprint and link/enabler package costs.
