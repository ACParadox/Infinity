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

## Expanded Onyx tactical guide (2026-10-23)

The [Onyx N5.3 tactical/list-building guide](../../notes/factions/onyx-contact-force.md) preserves Overdron HRMC/Plasma disagreements, 51-point HRL alternative, robotic attrition, Xeodron/Nourkias and Caskuda insertion. **Nexus/Kerr-Nau Wildcards are Unidron-context only**, while Nourkias has specifically delimited eligible team contexts. The pinned current chart above remains definitive.

## Command-unit apex/value cross-reference (2026-10-23)

**Nexus CoC 23/0** is top value because it supplies **NCO, Number 2, Mimetism(-3), BS13 and E/Mitter** while replacing a useful Unidron link member; its Onyx Wildcard access is **Unidron-only**. A Nexus LT 19/0 can be safe/cheap, while **EXO CoC 19/0.5** and **Umbra Legate FTO CoC 38/0** are distinct backup roles. **Nourkias LT or fighting Legate** increases exposure; keep successor apart from the assault. Neither Xeodron nor Overdron receives Warhorse or Mnemonica simply from Combined Army affiliation.

See [cross-game Lieutenant, CoC and Order-economy tiers](../../notes/list-building/command-units-apex-and-value.md). **Current pinned profiles and Fireteam chart above govern legality.**

## N5.3 mission specialists — apex/value decisions (2026-10-23)

**Nexus CoC23, Engineer23, Hacker24–27** offers Mimetism(-3), NCO, real specialist and **Unidron-only Onyx Wildcard** team movement; they are distinct variants. **M-Drone FO15/TA18** is reliable Sensor/Repeater objective access; **Kerr-Nau KHD30** adds Plasma/Pitcher/White Noise to linked scoring. **Med-Tech21 Doctor+Engineer** supports high-price Xeodron/Overdron and the healing Classifieds. No unrestricted Nexus Xeodron link.

[Cross-game Mission Specialists / Button Pushers tiers](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). The current faction profile and Fireteam reference above controls legality.

## Airborne and enemy-DZ attack choices — N5.3 (2026-10-23)

**Caskuda TAG64/1** is a high-ceiling **Combat Jump(PH14, Explosion)** + TA threat; **70% native success/85% with actual friendly Controlled Jump(+3)** before ARO/attack odds. Failure places it at own DZ table edge and loses the intended backline run, not random dispersion. **M-Drone Sensor/Repeater** and Nexus hacker can exploit target disruption without paying TAG arrival risk. **Greif IMP-2** gives cheap Turn-0 attack/deployment tax where permitted. Keep **Nexus CoC23** safe as distinct succession/linked utility; Onyx Nexus Wildcard is Unidron-context, not universal Xeodron team.

See [current cross-game apex/value, landing odds and expected-trade tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **This roster and Fireteam chart control exact loadout/availability.**

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **Overdron HRMC62/1.5** is the economical **TAG** AP heavy-volume attack with Albedo against MSV defenders; **plasma sniper59/1.5** instead pressures other saves and can be worse in direct active HMG-range FtF. **Caskuda64/1** is a separate **TAG** delivering an explosive rear entry, but landing risk and loss of Cover on entry undermine consistent long-range shooting. An **EXO** or **Unidron** support gun can clean soft targets rather than committing the big armored body into every bad exchange. [Separate TAG and non-TAG combat rankings](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## Warbands and cheap high-upside trading — N5.3

**Onyx** lacks the broad **Dāturazi Regular-Smoke/cheap-Hungries** suite in Vanilla/MAF: use **roster-legal Ikadron/Unidron cheap templates and REM screens** to tax enemy close assault, **D-/M-Drone** sensor/tech where actually permitted, and linked **Nexus/Kerr-Nau** hacking/White Noise against fragile midfields. **Greif IMP-2** can impose early order/deployment tax but is not a 5pt warband. **Nexus CoC23** is a succession/scoring profile, **not** disposable anti-TAG melee. No imaginary 4pt Gaki imported from Morat.

[Current cross-game warband apex/value, target counters and LT/CoC tiers](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). Pinned profile choices and canonical Fireteam chart in this roster remain authoritative.

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


## ARO apex/value cross-reference (2026-10-23)

The [N5.3 cross-faction ARO apex/value and matchup study](../../notes/list-building/aro-units-apex-and-value.md) compares hidden missile traps, Neurocinetics/TR, cheap templates/mines, DZ guards and conflicting creator opinions. Consult the **roster and Fireteam chart above** for legally available profiles, SWC, Training and AVA.

- **Noctifer ML** — 30pt hidden launcher, decisive attack from an apparently empty lane; remains vulnerable after revealing and supplies no normal Order while Hidden
- **Q-Drone TR Thunderbolt** — 20pt/0.5SWC and Mimetism(-3), useful reactive presence with Engineer support; won't solo elite active guns
- **R-Drone Flash** — 7pt regular + Repeater and reactive stun threat; value is Order+network+minor tax, not a durable lane
- **Warcor Flash** — 3pt Irregular ARO tax/late-game Stun attempt, not a Regular Order
- **Ikadron Baggage/Flamethrower** — cheap multi-purpose DZ corner guard and Repeater; contributes more than pure filler without being a long gun

**Practical deployment:** put cheap disposable/Flash/DTW or mine pressure on the approach; retain a separate unseen or recoverable threat for the decisive square; avoid exposing a premium active attacker and check opponent Smoke, MSV, hacking, AD and pie-slicing. No automatic order from an off-table Hidden model; Irregular ARO units do not supply generic Regular Orders.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Med-Tech Obsidon21 + Slave Drone3** is an efficient dual hub for **Overdron/Caskuda TAGs**, REMs and VITA assault elements. **Kurgat Engineer** buys a separate forward combat/repair role when a legal Fireteam is advancing; the 21pt hub usually provides more pure recovery per point. **Remote Presence** lets a single successful repair cancel either Unconscious level if the Servant can safely reach the disabled machine. [Doctor/Engineer apex/value, odds and media disagreement](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Onyx** normally makes best melee contact after **gun/Repeater/template** troops remove a route, not by paying for MA5 Hidden assassins unavailable in this roster. **Sphinx** has strong defensive Camo/Climbing/DA CCW but is a **93pt TAG** bought for stealthy gunfire, not a 29pt Monofilament CC killer. **Rindak/Kurgat/Cube Jäger** or other legal short-range pieces should attack in their proper role, not be mistaken for universal dedicated MA4 duellists. [Dedicated CC assassin apex/value, delivery and counter-CC](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## N5.3 network projection — Pitchers, Repeaters, TinBots and disposable delivery

**Bit & KISS! HD+Trinity/Pitcher+Deployable Repeater25/.5 with native-Repeater KISS** offers an excellent package of pitched, placed and *mobile* nodes; **Onyx KHD/Oblivion24/.5** has a different KISS variant. **Umbra Legate FTO HD+/Pitcher38/.5** extends White Noise/cyber pressure through a source-legal team; **Kerr-Nau Pitcher30/0** brings plasma/hacking combat as expensive projector. **R-Drone7/0**, **Ikadron11/0** and **M-Drone FO/Sensor/Repeater** are efficient physical native carriers. **Counter:** a 25pt Bit package can be crippled by one clean KHD/DTW opportunity; a 7pt R-Drone + independent hacker may be enough where expensive multi-weapon team loses initiative.

[Whole-game network projection: apex/value, current profiles, and opposing transcript views](../../notes/list-building/network-projection-repeaters-pitchers-apex-value.md).

## N5.3 rare abilities & unusual combinations — tactical synthesis

**Ko Dali37/0 Combat Jump+MSV2+Protheion+Specialist**, or **34/0 FD(+20)+Mimetism(-3)**, uniquely lands behind a camouflaged backline and can exploit a VITA victim; **Combat Jump and FD are mutually exclusive profiles**. **Umbra Samaritan37/0 Plasma + MA4 + Super-Jump + NWI + Protheion**, or **Nourkias48/1** cyber/MA4/Protheion is an elite late-game CC snowball; do not pay for a 37pt Samaritan solely to feed one fragile enemy. **Overdron HRL51/1.5** (or gun59–62/1.5) with Albedo(-6) counters high-cost enemy MSV long AROs but **does not possess an MSV**; comparison with MSV+Albedo Bào/Satrah is a different archetype. **Opposing Irregular Order #56 (Oct 2026):** one host values Umbra multi-Wound feeding, another doubts expensive Samaritan/Xeodron skews and thinks Ko Dali's BS14/MSV2 shooting is her real purchase.

[Cross-faction rare abilities apex/value, mechanics, and MCP source debates](../../notes/list-building/rare-capabilities-and-unique-combinations-apex-value.md). Current roster/Fireteam profile tables above are authoritative.

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Unidron14 K1 Combi**, **Cube Jäger15 Mono/18 E/Mitter+Mono**, **Nexus23 E/Mitter** are different cheap can-openers: gun, flank assassin or electronic state. **Kurgat30/1 Portable Autocannon** is repeatable AP+EXP lethality, **Umbra Legate33 K1 Combi** is high-cost durable attack, **Xeodron K1 Marksman49** is TAG pricing separately. One E/M hit does not guarantee a permanent kill; use the Engineer-route/turn analysis. [Cross-game anti-armor apex/value, E/M and AP+EXP guide](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## Tactical cross-reference — indirect fire (2026-10-23)

**Onyx:** **T-Drone Guided16/1.5** can exploit Umbra/Nexus/Victor/Bit and R-/M-Drone/Unidron networks when those hackers and repeaters are already in the list. An **Overdron Albedo/Tactical Awareness** gun often removes a key MSV ARO more directly; **ECM: Guided on the TAG does not make the Overdron a Guided shooter**. Prioritize direct K1/plasma fire, super-jump objective access and specialist coverage over missile-only setup. [Global Guided vs Spec guide](../../notes/list-building/indirect-fire-speculative-guided-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Xeodron49/.5** (3STR/ARM5/BTS6, Tactical Awareness, Super-Jump, legal Xeodron Fireteam) is an exceptional **medium-cost TAG zone swing**, more affordable than 93pt Sphinx; **49/.5 K1 vs MULTI** are separate loadouts. **Sphinx93/2** gives exceptional stealth apex, but must reveal to count VP and needs non-hackable support plan. **Unidron FO15/0** or **Specialist/Commlink16/0**, Dogged/Remote Presence/Plasma is economical objective entry support; **Dogged does not guarantee end-round non-Null scoring**. **Ikadron11/0 Baggage/Repeater/LFT** guards close approaches and is huge only in *Baggage-bonus scenarios*. **Opposing Irregular Order #56:** linked Xeodron skew can dominate contested space, but consuming almost half a list can cost too many independent specialists/Orders; protect fallback.

[Cross-game zone-holder and carrier apex/value, mission rules, and opposing transcripts](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Current local roster/FT chart is authoritative.
