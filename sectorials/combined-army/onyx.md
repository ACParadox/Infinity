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

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**M-Drone FO/Sensor/Triangulated Fire** is the cheap **Camo/Hidden ZoC** answer, while **Ko Dali MSV2 + FD(+20)34/0 or Combat Jump37/0** actively hunts Mimetism from unexpected lanes. **Overdron Albedo(-6) 51–62pt** is a **conditional anti-enemy-MSV/Marksmanship** TAG rather than universal Mimetism; **Kerr-Nau KHD with White Noise30/0** supplies a rare direct anti-visor screen without claiming every KHD has that program. **Counter:** Onyx does not inherit Morat Dāturazi or generic Vanilla Camo tools; if no enemy visors, prefer independent M-Drone/Sensor/mission pressure instead of paying for conditional Albedo.

[Non-hacking & tech-specific counter-selection, N5.3 anti-tech apex/value and opposing MCP transcripts](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## N5.3 peripheral / synchronized / multi-body apex-value update

**Bit+KISS! HD+Trinity25/.5** = true synchronized **Hacker+native-Repeater KISS** physical attack/network fork; **24/.5 KHD+Oblivion** in Onyx carries **different KISS loadout**, not the same Repeater. Bit can hide as 1W/ARM0 controller while KISS projects adhesive/Pitcher angle subject to Coherency; KISS is **not an extra pooled Order**. **Xeodron49–50/.5–1 and Overdron/Sphinx included Stal-/Scindron Ancillary** can only create on-board second body after Place Deployable and may leave active Fireteam on doing so; do not award free start/Order. **Contrary approach:** Bit/KISS is safer 25pt dual-target harassing piece on hacking-focused Onyx, while 49pt Xeodron with separate 7pt R-Drone is far better for independent Orders and moving a larger VP zone swing. Avoid conflating standard Ancillary with Cyberplug autonomy.

[Whole-game N5.3 Peripheral & Multi-Body Apex/Value guide](../../notes/list-building/peripheral-synchronized-multibody-apex-value.md). Exact current roster, dependency and Fireteam chart above override commentary.

## Battle-report effectiveness and combinations (qualitative, 2026-11-01)

**Observed productive toolkit:** #212 deployed a **Xeodron K1 / MULTI Marksman Duo** with **Rodok Paramedic, Umbra Legate, Kurnau KHD/White Noise and Med-Tech/E-Drone**. The TAGs fixed defenders while **Kurnau and cheap support completed Classifieds**; a disposable EVO REM deliberately absorbed a mine so a mission actor could proceed. Onyx won **Countermeasures 6–0** even though the Xeodrons alone were not the source of all points. [#212](../../notes/battle-reports/211-220-n5-battle-report-tactical-analysis.md).

**Mission-dependent contrast:** #237's vanilla Ariadna attacker chose **Wallace** into an atypical **multiple-Umbra** Onyx list to preserve anti-materiel/CC access; a large quantity of Cybermask/Hacking alone is not proof of safe objective control. [#237](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md).

**Build rule:** Prefer **TAG Duo / Umbra gun-and-hacking pressure plus cheap, distinct WIP/Doctor/Engineer/Specialist routes**. Preserve ability to spend Orders on Countermeasures actions; no 6–0 result establishes faction-wide win probability.

[Cross-report synthesis and evidence cautions](../../notes/battle-reports/cross-report-unit-effectiveness-and-combinations.md).

## Mission performance — battle-report evidence (2026-11-01)

| Mission(s) | Tested composition / scoring mechanism | Evidence |
|---|---|---|
| **Countermeasures** | Xeodron K1/MULTI Duo plus Rodok/Kurnau/Doctor Worm/E-Drone opened Classified routes; 6–0 vs Invincible Army. | [#212](../../notes/battle-reports/211-220-n5-battle-report-tactical-analysis.md) |
| **Evacuation / Classifieds** | Umbra Samaritan/Legate plus hacker/Pitcher and independent mission workers retained several task types as Haqq broke Fireteam to carry civilians. | [#141](../../notes/battle-reports/141-150-n5-battle-report-tactical-analysis.md) |
| **Area of Interest matchup caution** | Unusual multiple-Umbra/Cybermask build was bypassed by vanilla Ariadna's Wallace/zone plan; that opponent was not a normal Onyx roster. | [#237](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md) |

**Limits:** The Xeodron Duo's zone pressure is useful because Kurnau/cheap REMs still perform the exact Classifieds, not because the TAGs score everything. Game-era qualitative evidence, not a win-rate or current Fireteam claim. [Full mission evidence audit](../../notes/battle-reports/cross-report-mission-performance-by-sectorial.md).

## Counterplay — observed N5 battle-report responses (2026-11-02)

| Threat / target | Observed response and limitation | Battle reports |
|---|---|---|
| **Against TAG/HI and mine field** | Xeodron K1/MULTI Duo drew defender attention while Kurnau White Noise/KHD and E-Drone sacrificed itself to clear a mine for a Countermeasures Classified (6–0). | [#212](../../notes/battle-reports/211-220-n5-battle-report-tactical-analysis.md) |
| **Against defensive team** | Umbra Samaritan/Legate forward hacking, Suryat TinBot/launcher and cheap Ikadron support create multiple angles while surviving specialists perform Evacuation/Classified. | [#141](../../notes/battle-reports/141-150-n5-battle-report-tactical-analysis.md) |
| **Opposing infiltration/CC risk** | Atypical five-Umbra/Cybermask roster let vanilla Ariadna Wallace and cheap zone pieces score around its plasma tech. Anti-hacker group should not omit a real scorer. | [#237](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md) |

**Limit:** Distinguish Onyx-specific profiles from vanilla Combined; #237 opponent roster is atypical and round context limited. These are historical qualitative interactions, not present N5.3 unit, Fireteam, or win-rate claims. [Full cross-report counterplay analysis](../../notes/battle-reports/n5-cross-report-counterplay-tags-hi-hacking-camo-impersonators-fireteams.md).

---

## Must-have / Go-to / Avoid — source-backed recommendations (2026)

Dated source-backed tactical preferences and miniature purchasing priorities; opinions do not override N5.3 roster, profile or Fireteam data above.

**Original audit title:** Combined Army — must-have, go-to and avoid audit (N5.3, 2026-10-23)

**Scope:** Vanilla Combined Army, Morat Aggression Forces (MAF), Shasvastii Expeditionary Force (SEF), Onyx Contact Force (OCF), Next Wave. The user-defined categories are deliberately demanding: **must-have** = an almost-every-list personal default reported by a speaker or genuinely indispensable faction engine; **go-to** = broadly good when assigned a sensible role; **never take / avoid** = profile-level displacement or explicit speaker rejection, **not** proof of mathematical domination. An empty hard-veto category is more accurate than inventing one.

**Factual authority:** the five [current repository sectorial reference files]() (all `status: current`, N5.3, Army `7.26246.158`, changed 2026-09-03), then [rules](../../rules/README.md). These establish **legality, costs and loadouts**, while videos/podcasts establish **opinions and observed results**. Earlier N4/2025 advice cannot override the current roster. [Official N5.3/ITS18 changes](https://infinityuniverse.com/en/news/infinity-rules-update-5-3) include updated Team-Ops/Spec-Ops and Sāchā availability. Normal-list recommendations do **not** silently assume optional Team-Ops.

**Evidence key:** **Direct** = attributable preference or rejection from a full transcript checked for this audit; **Corroborated** = source discussion + existing reviewed guide; **Contested** = sourced counter-opinion exists; **Edition-limited** = pre-N5.3 material must be interpreted using current reference. “Near-must” is still **not a mandatory unit**.

### Quick comparison

| Army | Strongest near-default evidence | Go-to engines | Credible profile-level avoid | Absolute unit veto? |
|---|---|---|---|---|
| **Vanilla** | Dāturazi Smoke; Bit & KISS **KISS Pitcher** option; Libertos Mine layer (all speaker-personal, not all mandatory) | Vector + Unidrons, Legate HD+, Sheskiin, elite Aspects | Umbra Legate LT, non-LT Charontid if LT version fits, wrong Bit & KISS for network projection | No |
| **Morats** | Dāturazi or **alternative** Smoke engine; no uncontested individual compulsory purchase | Sogarat LT/NCO, Yaogat MSV2, Dartok FTO, Oznat/Hungries | Yaogat Combi/Panzerfaust or BSG/Panzerfaust as default shooters; unbalanced double-Krakot team | No |
| **Shasvastii** | **None universal**: 2026 winner reports distinct sneak and face-up lists | Speculo, Caliban, Shrouded, Noctifer, Sheskiin, Mentor, Gwailo/Victor | Cadmus KHD over basic BSG **for a pure assassination/drop role** | No |
| **Onyx** | No uncontested must: 2026 hosts **disagree on Unidron quantity** | Nexus + Unidrons, Bit & KISS, Overdron, Xeodron/Nourkias, Noctifer | Void Operators as default generic team fillers; generic Suryat gun package when it crowds out Onyx tools | No |
| **Next Wave** | **Pandora** (Shepherd says every list); **Gearhead + Puzzler** near-core in disruption builds | Blackheart, Stinger, Harbinger specialists, Wraith FTO, Skyhound/Ironside | Harbinger HMG/ML, Wraith Hidden MULTI Marksman, naked Gearhead Engineer over useful alternatives | No |

### 4. Onyx Contact Force

**Sources:** [Irregular Order #56, *Onyx Contact Force Review*, 17 Oct 2026](https://open.spotify.com/episode/7b2QJ494pgPp6NY6WQ9QWF) (**full podcast transcript rechecked**; particularly ~85–120min Nexus/Unidrons, ~125–160min Morat/Exrah, ~165–210min TAGs and hidden pieces); [Robert Shepherd, *Onyx faction focus*](https://www.youtube.com/watch?v=U238na0BXfs) (full YouTube transcript rechecked; older); [Tactical Awareness S3E14 Onyx](https://www.youtube.com/watch?v=u_e7wxbn1Zk); [existing Onyx guide](../../notes/factions/onyx-contact-force.md); [N5.3 roster](onyx.md).

**No uncontested must-have.** In the **Oct 2026 Irregular Order review (~105–110min)** one host takes substantial **Unidron** infrastructure; the other openly says he generally *does not*. That means “must take Unidron Core” is a **playstyle judgment**, not faction consensus.

**Go-to**
- **Nexus LT/CoC/Engineer/Hacker + Unidron Plasma/K1/FO/Missile** — inexpensive resilient link infrastructure, real specialists, gun and Engineer recovery; cheap linked Unidrons repeatedly repairing via Remote Presence can consume enemy turns. **Contested** on quantity and emphasis.
- **Bit & KISS + other legal Repeaters** — threatens enemy hackers before TAG movement; compatible with cheap engineer and Umbra support. Distinguish its current Onyx options rather than importing Vanilla loadout wording.
- **Overdron (HRL 51 / Plasma Sniper 59 / HRMC 62, each 1.5 SWC)** — Albedo (-6) ranged MSV-counter gun, Remote Presence repair; a realistic turn-one ARO remover. HRL is the cheaper legitimate alternative, not simply “HRMC versus Plasma.”
- **Xeodron + Nourkias legal Duo/Haris contexts** — mobile Super-Jump gun + close-range/anti-armour combat or hacking; one of the sectorial's signature non-standstill attack packages.
- **Umbra Legate / Samaritan, Noctifer, Q-Drone, Ko Dali/Fraacta** — choose second-wave mobility, Hidden ARO, repeater/total-reaction defence, or off-axis strikes based on opponent and table. **Samaritan** can be outshone by Nourkias *on general utility*, but is not literally useless.

**Avoid / speaker-personal rather than categorical**
- **Void Operator as generic FTO filler instead of cheaper Base Operator or an actual premium Vector gun** — **Direct:** in *Irregular Order* (~146–148min), a host says he has **never picked Void over Base**; extra utility often fails to justify the premium in his lists. Another host points out its rocket/KHD utility. **Contested**, not a strict never.
- **Generic Suryat or Kurgat/Morat gun package without a special role** — 2026 hosts (~128min, ~157min) consider some imported Morats less efficient **in the Onyx ecosystem** than Nexus/Unidron/TAG/Ironwork choices. **Rodok**, especially a mobile Engineer, remains a defensible exception.
- **Kerr-Nau as an automatic inclusion** — 2026 reviewers compare its price/stat growth against newer Nexus; older Shepherd notes Kerr-Nau's KHD/plasma/Fireteam role. **No defensible unit ban.**
- **Not “never take”: Sphinx/Caskuda, Xeodron, ordinary Samaritan or Overdron.** All have real role/tradeoff discussions and speakers disagree over whether their specialist cost is warranted.

### Confidence rules and conclusion

1. **Strict “never take” labels attach to exact current loadouts**, not to entire units. Use *speaker strongly avoids* rather than declaring a mathematical theorem from one opinion.
2. **Every faction has successful alternative list architectures.** At most a handful of troop choices are speaker-verified near-defaults; in Onyx and Shasvastii, **no individual unit has sufficiently strong all-build consensus**.
3. **Preserve opposing speakers.** Especially: Morat **Sogarat vs Kornak**, Shasvastii **Gwailo and Jayth skepticism vs 2026 winner**, Onyx **Unidron density**, Next Wave **Drakios**, Vanilla **Avatar effectiveness vs list cost**.
4. The roster is **N5.3, September 2026**, but most opinions are earlier; they are tactical heuristics, **not independently updated tournament win-rate data**. The Oct 2026 Onyx review and 2026 SEF tournament testimony receive more weight than older recordings where they conflict.

### Whole-unit purchasing audit — can I skip the miniature? (2026-10-30)

**Whole-unit** here means *every currently legal profile of that named troop in the specified army*, not one disliked loadout. **Defer** is a collection-building recommendation, not a competitive ban; evaluate the same miniature again when playing a different sectorial. **Hard whole-unit avoids: none established by these recordings.**

| Army | Entire model/unit to defer buying? | Why; what would change the answer |
|---|---|---|
| **Vanilla Combined** | **No source-supported whole-unit skip** | The Umbra Legate **LT** and non-LT Charontid criticisms leave useful alternative profiles; Bit & KISS's wrong network loadout does not disqualify its Pitcher configuration. Avatar is *strong but optional*, not bad. |
| **Morat** | **No** | Cheap Yaogat Panzerfaust profiles are disliked, but the MSV2 Spitfire/sniper are positively recommended. Suryat, Kornak and TAGs still have distinct uses. |
| **Shasvastii** | **No** | Cadmus KHD criticism applies to a backline-kill role; the BSG and KHD specialist jobs differ. 2026 results directly contradict blanket Gwailo/Jayth skips. |
| **Onyx** | **Defer Void Operator unless deliberately using its rocket/KHD utility — low confidence** | An [Irregular Order #56](https://open.spotify.com/episode/7b2QJ494pgPp6NY6WQ9QWF) host never preferred it over Base Operator; another defends its unique tools. A *personal* buying deferral, **not** all-profile dominance. |
| **Next Wave** | **No** | Harbinger heavy guns, Wraith hidden MMR, plain Gearhead Engineer and Bit & KISS as a *Pitcher substitute* are the poor choices. Other profiles/uses remain legitimate, so do **not** skip those entire model families. |

**Purchase rule:** consider skipping a full unit only when its *best* viable profile also loses its expected role in your chosen army. A bad SWC weapon or wrong Fireteam configuration does **not** justify avoiding an entire kit. See the [cross-faction buying shortlist](../../notes/factions/model-purchase-avoid-summary-2026.md).

### Worst-value, circumstantial and proxy-first miniature purchases by army (2026-10-30)

**Question:** For **Vanilla Combined Army, Morat Aggression Forces, Shasvastii Expeditionary Force, Onyx Contact Force and Next Wave**, which are the **weakest everyday picks**, most specialized rarely *needed* purchases, or **good units better represented by a proxy before buying an extra miniature**? An **AVA maximum is not a shopping target**. “Rare/circumstantial” below is a *qualitative estimate of how often a particular job arises in the reviewed list plans*, **not a measured tournament pick rate**. The current [N5.3 roster files]() (Army data 3 September 2026) take priority over earlier recordings for exact variants, base/silhouette, unit access and Fireteams.

**Decision labels:** **Defer/skip as a default dedicated miniature** = an explicit reviewer's negative judgment on that *usual role*, with exceptions explained. **Proxy first** = a specialized yet legitimate **inferred purchase priority**, *not* an invented direct quotation. **Avoid profile, NOT unit** = the named loadout/Fireteam plan is poor but other choices are strong. **Proxy the extra** = first copy or alternative sculpt may be a normal good purchase, but redundant physical duplicates need demonstrated simultaneous use. **Contested** = dated contrary opinions, successful tournament use or a distinct current-profile benefit make a universal “worst” label dishonest. **No verified complete-unit all-profile hard ban exists** in the present evidence.

#### 4. Onyx Contact Force — the clearest specialist full-model deferral

| Model or profile | Evidence and competing role | Purchase / proxy verdict |
|---|---|---|
| **WCD Void Operator as an automatic Exrah team body instead of Base Operator** | **Direct — [Irregular Order #56, October 2026](https://open.spotify.com/episode/7b2QJ494pgPp6NY6WQ9QWF):** one host has **never personally chosen Void over Base** for the generic role; another defends the **rocket/KHD** utility. Void and Base **both** have **current Exrah team required-choice** permissions, not identical rules. | **Defer full-model Void purchase by default / proxy first** unless **specific KHD/rocket / Exrah composition** is central. **Explicitly contested, not all-profile dominated**. |
| **Generic Suryat/Kurgat or imported Morat gun package without a unique job** | **Direct speaker-comparative skepticism in Onyx October 2026** versus **Nexus/Unidron/Overdron/Xeodron** ecosystem; **Suryat** can offer hard resilience/Fireteam structure, and **Kurgat** legitimate Engineering/repair. **Rodok Engineer/mobile gun** was specifically treated more favourably. | **Proxy-test specialized Suryat/Kurgat/extra Morat shooter**, not a no-Suryat/no-Engineer rule. If a selected **Onyx Fireteam requires Suryat or Kurgat**, account for that legal anchor. |
| **Kerr-Nau when a regular Nexus already covers hacker/command roles** | **Direct nuanced 2026 review:** hosts question extra cost/role overlap against newer Nexus, while **Kerr-Nau KHD/plasma/Unidron Wildcard** retains a unique upgrade. **Nexus** provides flexible LT/CoC/Engineer and link. | **Proxy first**; buy for an actual **KHD/plasma/special Unidron team** rather than treating Kerr-Nau as universal near-must. Not a verified entire-character dud. |
| **Ordinary Umbra Samaritan when Nourkias already does the same attack** | **Cross-source comparative, partly older:** Nourkias may be superior for general anti-TAG/hacking/CC, but regular Samaritan's price/Fireteam eligibility and specialized CC delivery can differ. **Onyx allows Samaritan on Onyx and Xeodron teams** where legitimate. | **Proxy the *extra* regular Samaritan**, particularly if already using Nourkias. **No categorical unit ban**; buy for a distinct permitted formation or to allocate attack threats. |
| **Full five-Unidron collection just because an Onyx Core exists** | **Strong direct disagreement — Irregular Order #56 (~105–110min):** one host likes a high-Unidron **Nexus Engineer/FO/missile repair** shell, the other generally avoids massing them. A full Core uses money/models and list cost that could go to a TAG/skirmisher. | **Buy enough for the legal team you actually use; proxy extra Unidrons**. **Never label first cheap linked Unidron or Nexus bad**. A 5-Unidron style is legitimate but *not mandatory*. |
| **Second Xeodron / Overdron / another heavy TAG on top of the first ranged hammer** | **Inference:** **Xeodron + Nourkias** and **Overdron HRMC/Plasma/HRL** are differentiated legal attack cores; Overdron Albedo answers enemy MSV, Xeodron Super-Jump and teams maneuver, while more TAGs can deplete repair/scoring Orders. Overdron can form a **real Duo**; **Sphinx and Caskuda** compete for very different skew roles. | **Proxy extra TAG** before buying **two Overdrons (AVA2), multiple Xeodrons (AVA4)** or a second large chassis. **Do not skip the first Overdron or Xeodron because of an optional skew concern.** |
| **Caskuda or Sphinx as a general straightforward linebreaker** | **Contested:** Combat Jump TAG needs clear landing/anti-hacking plan; Sphinx expensive stealth Spitfire wants soft backlines, not hard frontal AROs. [Onyx review](https://open.spotify.com/episode/7b2QJ494pgPp6NY6WQ9QWF) discusses both viable specialised threats, while older TAG reviews object to consistency/cost. | **Proxy-test unusual TAG first**, buy once the distinct infiltration/drop plan survives multiple game tables. **Not a universal worst verdict**. |
| **Cube Jäger vs a Fraacta/Ko Dali extra backline purchase; another Greif** | **Inference from roles:** the cheap **Cube Jäger is Irregular** and aims at a limited specialist objective, while **Fraacta** and **Ko Dali** add different attack/landing tools. **Greif** provides different impersonation/deception value and can't be treated as Speculo. | **Proxy the *second* flank/surprise attacker** until missions show why both are needed; not enough direct evidence to label these troops bad. |
| **Maakrep, EXO, extra Vector or second expensive premium sightline gun** | **Unrated / inferred:** **Maakrep** anti-Mimetism, **Vector** MSV2 long-range, **EXO** Exrah utility and Overdron all have meaningful different team roles. The generic extra gun may duplicate lanes and spend SWC unproductively. | **Proxy the uncommon specialist/gun before buying a dedicated sculpt**. The source does **not** justify a “Maakrep/EXO never take” claim. |
| **Bit & KISS, Med-Tech + Slave Drones, T-/E-/Q-/M-Drone bought without their corresponding network/repair** | **Good tools, invalid *shopping assumption*:** KISS requires its physical partner, Med-Tech/Slave have controller/servant interactions, and EVO/Guided need Supportware/Targeted. Q/M cheap utility remains. | **Proxy extra support REMs**, buy enough genuine **Repeater/Engineer** infrastructure when the TAG/repeater list actually uses it. **No extra Regular Orders from peripherals**. |

**Direct sources:** [Irregular Order #56 2026](https://open.spotify.com/episode/7b2QJ494pgPp6NY6WQ9QWF), [Shepherd Onyx](https://www.youtube.com/watch?v=U238na0BXfs), [Tactical Awareness Onyx](https://www.youtube.com/watch?v=u_e7wxbn1Zk), [Onyx guide](../../notes/factions/onyx-contact-force.md). **High-confidence first-choice model roles to preserve:** one useful **Nexus**, a small or purpose-built **Unidron** package, **Bit & KISS** where legal, a chosen **Overdron/Xeodron** if building armour, and selected **Noctifer/Malignos** scoring/deception. The strongest **full-model** deferral is **Void Operator for a generic filler role**, not the whole Exrah roster.

#### Cross-Combined Army — even useful models often make better first proxies

**Physical collection unknown:** No authoritative Combined Army collection counts were found at the expected paths **\`inventory/combined-army.md\`, \`inventory/morat.md\`, \`inventory/shasvastii.md\`, \`inventory/onyx.md\`, \`inventory/next-wave.md\`**. The guide does **not** assume you own or lack particular minis. Actual collection and list needs should override any inferred purchase quantity.

| Potential purchase | Proxy-first / shared-model recommendation | When to buy, and what must match |
|---|---|---|
| **Alternative weapon/role sculpt of the same troop** — Yaogat, Charontid, Unidron, Nexus, Rodok, Sogarat, Caliban, Shrouded, Noctifer, Gwailo, Overdron, Harbinger, Wraith-1, Stinger | Use a distinct **correct-silhouette/base model** to represent the selected *N5.3 profile*, with the actual rifle/ML/MSV/HD+/LT/FTO effects declared. For example, **a Yaogat Sniper and Spitfire are mutually exclusive equipment**, and **Charontid HD+/Sepsitor is not MSV3 by default**. | A separate sculpt is needed when **two physically distinct loadouts appear in one list**, repeated use or tournament proxy/paint requirements justify it. A single mini is often enough for every non-simultaneous profile of an AVA1 character. |
| **Named heroes / specialty operators** — Kornak, Victor Messer, Kerr-Nau, Ko Dali, Sheskiin, Nourkias, Pandora, Drakios, Patroclus, Achilles, Ruby Monday | Before buying all collectible personalities, test a **distinct correctly sized existing Corvus Belli figure** for the *one* legal name/role in a list. Don't reuse one physical mini for two characters *on the same table*. | Buy as the hero becomes a recurring component. **Some are excellent and near-auto** (e.g. Pandora in Shepherd's Next Wave lists); proxy-first does *not* mean “bad.” |
| **Shared Combined Army R-/M-/T-/Q-/E-Drones and Unidrons** | Test optional **Guided/EVO/anti-Camo or extra ARO** use with unused **matching-footprint REMs**, but do not assume different REM families share the same silhouette or model count. **Unidron is a trooper**, not a proxy for every drone chassis by default. | Buy more after real *simultaneous* REM count exceeds your physical pool; example: **Q-Drone + T-Drone** plus a separate linkable Unidron if needed. No false Core memberships. |
| **TAG substitutes** — Avatar, Sphinx, Caskuda, Overdron, Xeodron, Raicho, Bultrak, Juggernaut | Borrow/test an **appropriately based and silhouetted TAG** before spending heavily; do not confuse **weapon chassis differences, hidden/deployment states or faction legality**. One physical TAG can stand in as a different TAG only if its size and event rules permit. | When that exact large attack plan recurs or multiple TAGs are fielded **simultaneously**. A stock S2 infantry figure is not a safe proxy for a large TAG; **Vanilla does not automatically gain sectorial TAGs**. |
| **Next Wave Skyhound (VH) or other unusual non-TAG chassis** | Use a matching **Vehicle-sized model**; a Skyhound is neither a Juggernaut TAG nor a regular infantry hacker. Test no-Cover/vertical table dependence before buying a unique vehicle. | Purchase for a recurring altitude/attack/specialist plan; model the physical footprint and current movement/LoF geometry accurately. |
| **Extra Speculo/Fiday-like infiltrators, Greif, Shasvastii Caliban/Shrouded/Malignos and hidden troops** | Use spare **distinct camouflaged infantry sculpts** with suitable silhouette/base. **A Greif Operator is not a Speculo Killer and has different rules**; disguise/markers change information, not legal unit access. | Buy duplicate impostors/skirmishers when your actual **two-Speculo or three-Caliban** list repeatedly puts them all on-table together; an unmatched model is fine for a practice game only by agreement. |
| **Bit + KISS, Med-Tech + Slave Drones, Gearhead + Sartroid Puzzlers/Ranters** | **Represent each controller AND every actually fielded peripheral/servant body**. Do not count Puzzlers, KISS or Slave Drones as extra Regular Orders. The correct Cyberplug/Connected configuration must be chosen. **KISS Pitcher versus KISS Repeater varies by army/profile**; the plastic model itself cannot override a roster. | Buy a complete unit/partner set when it becomes a recurring list component. You can't represent a two-model team with one physical base and claim both independently. |
| **Taigha, Gaki, Preta, Dāturazi, Krakot and other warband quantities** | **Proxy additional compatible silhouettes** to try a large-screen build before buying to AVA. In Morats, **Oznat + Hungries** requires separate individual bodies and exact current Fireteam permission; unlinked Irregular warbands do not create pooled Regular Orders. | Buy when *simultaneous* legal body counts exceed the existing pool and the intended list's Regular Order economy still works. |
| **Unrated one-off specialists** — Zabuk, Tyrok, Maakrep, Cube Jäger, Ruby Monday, Kurgat second Engineer, Shasvastii Aïda/Dukash, Drakios | When a full transcript does not single out a unit negatively, do not invent a “never buy.” **Proxy a named legal variant** and track **which mission, matchup, Fireteam or deployment actually improves** before making an expensive character purchase. | Buy for a repeated *specific* role, not because a unit exists in the N5.3 index. Cross-faction model reuse is about physical proxying, not magically sharing AVA or access. |
| **Optional-mode Spec-Ops / Team-Ops models** | Most ordinary matches do **not** use these modes. **Do not buy a dedicated optional-mode sculpt just to complete a sectorial catalog**. | Buy only when your league/scenario expressly allows the relevant optional mode. N5.3 changed some optional-mode availability: older list entries may be obsolete. |

**Model proxy legality:** disclose all substitutions to opponents; verify the actual **Silhouette, base diameter, physical model count and selected roster's present legal Fireteam row**. Check the *current* ITS season and event organizer policy before competitive play rather than asserting an older season's proxy permission. A model cannot be a larger/smaller trooper by assumption; an appropriate TAG, REM, Vehicle or peripheral should be physically representable at the required footprint. **No proxy changes actual availability, Army classification or weapon/program option.**

**Bottom-line purchasing order:** **Most explicitly criticized everyday roles:** Vanilla **Umbra Legate Spitfire LT/non-LT Charontid gun default**, Morat **Yaogat Combi/BSG Panzerfaust and poor double-Krakot link**, Shasvastii **Cadmus KHD for BSG-only assassination**, Onyx **Void Operator as generic Base alternative**, Next Wave **Harbinger HMG/ML, hidden Wraith MMR, plain Gearhead Engineer**. **Most worthwhile *whole-model* defer/proxy tests:** **Avatar/Sphinx/Caskuda** and other large TAG or Skyhound plans, **Morat alternative TAGs**, extra **Shasvastii Speculo/Caliban/Sphinx**, **Onyx Void or second premium TAG**, **Next Wave Juggernaut/Drakios/Skyhound**, unusual named characters and extra FTO/weapon-option sculpts. Retain the detailed contrary tournament/podcast evidence before deciding that a unit is really weak.
