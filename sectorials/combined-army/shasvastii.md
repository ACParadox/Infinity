---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 603
sectorial_slug: shasvastii
sectorial_name: Shasvastii Expeditionary Force
parent_faction: Combined Army
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Shasvastii Expeditionary Force roster, standard loadouts, canonical Fireteam chart, and reverse Fireteam index. Shasvastii Corax Spec-Ops and Shasvastii Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# Shasvastii Expeditionary Force

## Overview and provenance

Repository-native reference for **Shasvastii Expeditionary Force** roster, profiles, points/SWC, AVA, and Fireteam access.

Sources used:

- Army-derived Shasvastii source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- Source blob: `3876e25145c7efba4ba35546765977fafc0b19da`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **30-unit standard Shasvastii roster** and the complete Shasvastii `fireteamChart` in the pinned Army source.
- `Shasvastii Corax Spec-Ops` and `Shasvastii Team-Ops` are optional game-mode content and are listed separately.
- Soldier of Fortune / generic mercenary-catalog entries whose source faction list is empty are excluded from the base roster.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name by itself.
- The Army JSON currently labels the Shock family `Shaveshii Shock Fireteams` and uses related `(Shavesii)` / `(Shaveshii)` comments. This reference normalizes that obvious source spelling inconsistency to **Shasvastii Shock** while preserving its structural meaning.
- Structured `required: true` rows for Jayth Cutthroats and Gwailos in Shasvastii Shock are preserved as a required-choice set; they are not interpreted as requiring both unit types simultaneously.
- FTO/profile restrictions are preserved: T-Drone access to Nox uses the FTO profile only; M-Drone access to Shasvastii Shock uses the FTO profile only; Aïda Swanson joins Nox only through her FTO profile; Agent Dukash Wildcard access uses the FTO profile; the Jayth Shock row is specifically `JAYTH CUTTHROATS FTO`.
- Corax Hasht's Wildcard context is limited by the source to Nox and Shasvastii Shock; Victor Messer's is limited to Shasvastii Shock; Aïda's is limited to Nox.
- Seed-Soldier and Cadmus Seed profiles are transformation states of their corresponding roster entries, not separate units.
- The Sphinx includes its Scindron ancillary Remote; Jayth Pit Patrol includes a synchronized Taigha.
- Linked Reinforcement army ID: **699**. Reinforcement Fireteams are not merged into the main chart here.

## Sectorial summary

| Field | Value |
|---|---|
| Army ID | 603 |
| Parent faction | Combined Army |
| Standard roster | 30 logical units |
| Reinforcement army | 699 |
| Core limit | 1 |
| Haris limit | 1 |
| Duo limit | Unlimited (`256` source sentinel) |

## Roster index

| Unit | ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| Jayth Cutthroats | 1294 | 4 | LI | Regular | Shasvastii Shock Duo/Haris, FTO profiles only, required-choice max 3 |
| Speculo Killers | 503 | 2 | SK | Regular | — |
| Med-Tech Obsidon Medchanoid | 507 | 1 | LI | Regular | — |
| T-Drones | 510 | 1 | REM | Regular | Nox Core/Haris max 1, FTO profile only |
| Shasvastii Haiduks | 514 | 3 | LI | Regular | Haiduk Duo/Haris, 1–3 |
| The Shrouded | 501 | 4 | SK | Regular | — |
| Q-Drones | 509 | 2 | REM | Regular | — |
| Slave Drones | 526 | 2 | REM | Peripheral | — |
| Ikadron Batroids | 532 | 2 | REM | Regular | — |
| Victor Messer | 1299 | 1 | LI | Regular | Wildcard, Shasvastii Shock context only |
| Taigha Creatures | 1296 | 8 | WB | Irregular + Impetuous | — |
| Cadmus-Naish Agent Sheskiin | 533 | 1 | LI | Regular | Wildcard max 1 |
| Shasvastii Gwailos | 520 | 1 | HI | Regular | Shasvastii Shock Duo/Haris, required-choice max 1 |
| Aïda Swanson | 1160 | 1 | LI | Regular | Wildcard max 1, Nox context, FTO profile only |
| Agent Dukash | 1514 | 1 | LI | Regular | Wildcard max 1, FTO profile only |
| Malignos | 502 | 3 | SK | Regular | — |
| Shasvastii Noctifers | 516 | 3 | LI | Regular | — |
| M-Drones | 508 | 2 | REM | Regular | Shasvastii Shock Duo/Haris max 2, FTO profile only |
| Glyph Warcors | 1873 | 1 | LI | Irregular | — |
| Shasvastii Cadmus | 513 | 4 | LI | Regular | — |
| Mentor | 1292 | 3 | LI | Regular | — |
| Shasvastii Seed-Soldiers | 512 | 4 | LI | Regular | — |
| E-Drones | 741 | 1 | REM | Regular | — |
| Caliban | 528 | 4 | LI | Regular | — |
| Tensho Experts | 1302 | 1 | LI | Regular | Nox Core/Haris max 1 |
| Shasvastii Nox Troops | 1290 | Total | LI | Regular | Nox Core/Haris, 1–5 |
| Oktavia Grímsdóttir | 1501 | 1 | LI | Regular | Nox Core/Haris max 1 |
| Shasvastii Corax Hasht | 537 | 1 | LI | Regular | Wildcard max 1, Nox/Shasvastii Shock contexts |
| R-Drones | 511 | 2 | REM | Regular | — |
| Sphinx | 524 | 2 | TAG | Regular + Tactical Awareness | — |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Shasvastii Corax Spec-Ops | 1920 | Spec-Ops | Nox Fireteam row, max 1 when Spec-Ops mode is in use |
| Shasvastii Team-Ops | 1934 | Team-Ops | No ordinary Shasvastii Fireteam-chart row |

## Unit details

### Jayth Cutthroats, Shasvastii Independent Assault Group

**ID 1294 · AVA 4 · LI** — `MOV 10-10 | CC 23 | BS 12 | PH 13 | WIP 13 | ARM 0 | BTS 6 | W 1 | S 2`. Shasvastii, Martial Arts L3, Mimetism (-6), Berserk, Dodge (+5), Combat Instinct, Stealth, Courage, Immunity (Shock), MSV1.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | **JAYTH CUTTHROATS FTO**; Chain Rifle (+1B), E/M Grenades, E/M Mine, Disco Baller, Heavy Pistol, DA CCW (PS 5) | Shasvastii Shock required-choice max 3 |
| 2 | 24 | 0 | **JAYTH CUTTHROATS FTO**; SMG, Chain Rifle, E/M Grenades, Heavy Pistol, DA CCW (PS 5) | same |
| 3 | 34 | 1 | **JAYTH CUTTHROATS FTO**; Red Fury, E/M Grenades, Heavy Pistol, DA CCW (PS 5) | same |
| 4 | 26 | 0 | **JAYTH CUTTHROATS FTO**; SMG, Chain Rifle, AP Mine, Disco Baller, Heavy Pistol, DA CCW (PS 5); Specialist Operative | same |
| 6 | 30 | 0 | **Pit Patrol**; SMG, Chain Rifle, E/M Grenades, Heavy Pistol, DA CCW (PS 5); includes 1 synchronized Taigha | —; chart row is specifically FTO |

### Speculo Killers

**ID 503 · AVA 2 · SK** — `MOV 10-10 | CC 22 | BS 12 | PH 12 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Shasvastii, Martial Arts L3, Impersonation, Surprise Attack (-3), Courage, Dodge (+2.5), Regeneration, Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 29 | 1 | Combi Rifle, Nanopulser, Smoke Grenades, Silenced Pistol, Monofilament CCW | — |
| 2 | 26 | 1 | Boarding Shotgun, Nanopulser, Smoke Grenades, Silenced Pistol, Monofilament CCW | — |
| 3 | 31 | 1.5 | Combi Rifle, Nanopulser, Shock Mine, Smoke Grenades, Silenced Pistol, Monofilament CCW; Minelayer | — |

### Med-Tech Obsidon Medchanoid

**ID 507 · AVA 1 · LI** — `MOV 15-10 | CC 16 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 3`. Engineer, Doctor, Deactivator, GizmoKit, MediKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | Combi Rifle, Zapper, D-Charges, Pistol, CCW | — |
| 3 | 22 | 0 | Same; Deployable Cover | — |
| 4 | 24 | 0 | Combi Rifle, Zapper, D-Charges, Armed Turret (Combi Rifle), Pistol, CCW | — |
| 5 | 25 | 0 | Combi Rifle, Zapper, D-Charges, Armed Turret (Marksman Rifle), Pistol, CCW | — |

### T-Drones

**ID 510 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CCW (-3); BS Attack (Guided) | — |
| 2 | 15 | 1.5 | **T-DRONE FTO**; Missile Launcher, Flash Pulse, PARA CCW (-3) | Nox max 1; FTO only |

### Shasvastii Light Support Unit Haiduks

**ID 514 · AVA 3 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Shasvastii, BS Attack (Shock), Sapper, MSV2.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 21 | 0.5 | AP Marksman Rifle, Pistol, CCW; X-Visor | Haiduk Duo/Haris, 1–3 |
| 3 | 23 | 1.5 | MULTI Sniper Rifle, Pistol, CCW | same |

### The Shrouded, Shasvastii Pioneer Corps

**ID 501 · AVA 4 · SK** — `MOV 10-10 | CC 14 | BS 12 | PH 12 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Shasvastii, Surprise Attack (-3), Camouflage, Mimetism (-3), Infiltration, Terrain (Total), Regeneration, Stealth.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 20 | 0 | Boarding Shotgun, Shock Mine, Pistol, CCW | — |
| 3 | 24 | 1.5 | MULTI Sniper Rifle, Pistol, CCW | — |
| 4 | 28 | 0.5 | Combi Rifle, Shock Mine, Pistol, CCW; Hacking Device, Hacker | — |
| 5 | 24 | 0 | Combi Rifle, Flash Pulse, Shock Mine, Pistol, CCW; Forward Observer | — |
| 6 | 24 | 0.5 | Combi Rifle, Shock Mine, Pistol, CCW; Minelayer | — |
| 8 | 21 | 0 | Boarding Shotgun, Pistol, CCW; Dazer, Minelayer | — |
| 9 | 26 | 0 | Combi Rifle, Shock Mine, Pistol, CCW; Killer Hacking Device, Hacker | — |

### Q-Drones

**ID 509 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage, Mimetism (-3), Total Reaction, 360º Visor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 25 | 1 | HMG, PARA CCW (-3) | — |
| 2 | 24 | 1 | Plasma Rifle, PARA CCW (-3) | — |
| 3 | 20 | 0.5 | Thunderbolt (+1B), PARA CCW (-3) | — |

### Slave Drones

**ID 526 · AVA 2 · REM** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Peripheral (Servant), Courage, Mimetism (-3); no Order of its own.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | PARA CCW (-3) | — |

### Ikadron Batroids

**ID 532 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 2`. Baggage, Repeater, Remote Presence, Courage, Discover (+3), Dodge (+2.5), Dogged.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 11 | 0 | Light Flamethrower (+1B), Pistol, PARA CCW (-3) | — |

### Victor Messer, Autonomous Agent of Chaos

**ID 1299 · AVA 1 · LI** — `MOV 10-10 | CC 14 | BS 12 | PH 10 | WIP 14 | ARM 0 | BTS 3 | W 2 | S 2`. Shasvastii, Stealth, No Cover, Technorganic, Nanoscreen, Hacking Device Plus with Trinity (PS 5) and Zero Pain upgrades.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 31 | 0.5 | MULTI Rifle, Nanopulser (+1B), Cybermine, D-Charges, Breaker Pistol (PS 6), CCW; Deployable Repeater, TinBot: ECM Guided (-9), Hacker | Wildcard max 1; Shasvastii Shock only |
| 2 | 30 | 0.5 | Vulkan Shotgun, E/Mitter, Cybermine, D-Charges, Silenced Pistol (PS 6), CCW; Deployable Repeater, Minelayer (2), Hacker | same |

### Taigha Creatures

**ID 1296 · AVA 8 · WB** — `MOV 15-10 | CC 21 | BS 9 | PH 13 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 1`. Berserk, Dodge (+3/+5 source modifiers), Sixth Sense, Courage, No Cover, Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 6 | 0 | Viral CCW (PS 7); Irregular + Impetuous | — |

### Cadmus-Naish Agent Sheskiin

**ID 533 · AVA 1 · LI** — `MOV 15-10 | CC 24 | BS 15 | PH 15 | WIP 13 | ARM 1 | BTS 3 | W 2 | S 2`. Nanoscreen, Shasvastii, Martial Arts L4, Courage, Dodge (+5), Protheion, BS Attack (SR-2), Stealth, No Cover.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 48 | 0 | MULTI Rifle, Pulzar, D-Charges, AP Heavy Pistol, DA CCW (PS 4) | Wildcard max 1 |
| 2 | 50 | 1 | Red Fury, Pulzar, D-Charges, AP Heavy Pistol, DA CCW (PS 4) | same |
| 3 | 48 | 0 | Opt 1; Lieutenant | same |
| 4 | 50 | 0.5 | Opt 2; Lieutenant | same |

### Shasvastii Armed Imposition Detachment Gwailos

**ID 520 · AVA 1 · HI** — `MOV 10-10 | CC 14 | BS 13 | PH 12 | WIP 13 | ARM 3 | BTS 9 | W 2 | S 2`. Nanoscreen, Albedo (-6), Shasvastii, Stealth, Combat Instinct, No Cover.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 44 | 1.5 | HMG, Breaker Pistol, CCW, E/M Carbine (+1B) | Shasvastii Shock required-choice max 1 |
| 3 | 39 | 1.5 | Heavy Rocket Launcher, Breaker Pistol, CCW, E/M Carbine (+1B); MSV2 | same |
| 4 | 44 | 1.5 | Opt 1; Lieutenant | same |
| 5 | 39 | 1.5 | Opt 3; Lieutenant | same |

### Aïda Swanson, Submondo Smuggler

**ID 1160 · AVA 1 · LI** — `MOV 10-10 | CC 19 | BS 12 | PH 11 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Martial Arts L2, Courage, Booty, Forward Deployment (+10), Mimetism (-3), Shasvastii, Stealth.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 0.5 | SMG (+1B), Viral Mine, Viral Pistol, Shock CCW (PS 7); Minelayer, Decoy (2) | — |
| 2 | 21 | 0 | **AÏDA SWANSON FTO**; SMG, Viral Mine, Viral Pistol, Shock CCW (PS 7); Minelayer | Wildcard max 1; Nox only, FTO only |

### Agent Dukash, Vashar Special Corps

**ID 1514 · AVA 1 · LI** — `MOV 10-10 | CC 21 | BS 13 | PH 12 | WIP 14 | ARM 2 | BTS 3 | W 2 | S 2`. Martial Arts L1, Courage, Dodge modifiers, Specialist Operative, Stealth, Mimetism (-3), Shasvastii, Immunity (ARM).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 39 | 0 | **AGENT DUKASH FTO**; MULTI Marksman Rifle, Nanopulser, D-Charges, Viral Pistol, Viral CCW (PS 7) | Wildcard max 1; FTO only |
| 2 | 40 | 0 | MULTI Rifle, Nanopulser, Viral Pistol, Viral CCW (PS 7), D-Charges; Parachutist (Deployment Zone) | — |

### Malignos, Shasvastii Deep Incursion Corps

**ID 502 · AVA 3 · SK** — `MOV 15-5 | CC 15 | BS 12 | PH 12 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Shasvastii, Surprise Attack (-3), Camouflage, Hidden Deployment, Mimetism (-6), Infiltration, Terrain (Total), Regeneration, Stealth.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 31 | 0.5 | SMG, Monofilament Mine, Silenced Pistol, CCW; Minelayer | — |
| 3 | 30 | 0 | Boarding Shotgun, Pulzar (+1B), Viral Mine, Silenced Pistol, CCW | — |
| 4 | 33 | 1.5 | MULTI Sniper Rifle, Pulzar, Silenced Pistol, CCW | — |
| 5 | 34 | 0.5 | SMG, D-Charges, Shock Mine, Silenced Pistol, CCW; Hacking Device, Hacker | — |
| 6 | 30 | 0 | SMG, Flash Pulse, D-Charges, Shock Mine, Silenced Pistol, CCW; Forward Observer | — |
| 8 | 32 | 0 | SMG, D-Charges, Shock Mine, Silenced Pistol, CCW; Killer Hacking Device, Dazer, Hacker | — |

### Shasvastii Tactical Dominance Special Wing Noctifers

**ID 516 · AVA 3 · LI** — `MOV 10-10 | CC 15 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Shasvastii, Surprise Attack (-3), Camouflage, Hidden Deployment, Mimetism (-6), Stealth, Dogged, Courage, X-Visor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 29 | 1 | Spitfire, Breaker Pistol, CCW | — |
| 3 | 30 | 1.5 | Missile Launcher, Assault Pistol, CCW | — |
| 6 | 31 | 1.5 | Spitfire, Breaker Pistol, CCW; Forward Deployment (+10) | — |

### M-Drones

**ID 508 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Deactivator, Repeater, Remote Presence, Triangulated Fire, Courage, Forward Observer, Terrain (Total), Sensor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 15 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3) | — |
| 2 | 23 | 0 | **M-DRONE FTO**; Combi Rifle, Flash Pulse, PARA CCW (-3); Nanoscreen, Tactical Awareness, No Cover | Shasvastii Shock max 2; FTO only |
| 3 | 18 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3); Tactical Awareness | — |

### Glyph Warcors, Ur Hegemony Journalists

**ID 1873 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Dodge (+3), Journalist; Irregular.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 4 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor | — |
| 2 | 4 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); Sixth Sense | — |

### Shasvastii Airborne Infiltration Group Cadmus

**ID 513 · AVA 4 · LI** — Cadmus is represented by a Seed form and a Developed Shape. The source notes that MOV, CC, BS, and PH can vary depending on Morpho-Scan, and that the Seed-Cadmus profile can use only its Chest Mines and PARA CCW.

**CADMUS-SEED:** `MOV — | CC 10 | BS 1 | PH 12 | WIP — | ARM 2 | BTS 3 | W 1 | S 0`. Shasvastii, Combat Jump, Decoy (1), Surprise Attack (-3), Transmutation (Hatching); Chest Mine and PARA CCW (-6).

**Developed Shape:** `MOV 10-10 | CC 15 | BS 11 | PH 12 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. Shasvastii, Morpho-Scan, Stealth, Surprise Attack (-3), BS Attack (+1B).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1826 | 22 | 0 | Combi Rifle, Pulzar, Pistol, DA CCW (PS 6) | — |
| 1827 | 19 | 0 | Boarding Shotgun, Pulzar, Pistol, DA CCW (PS 6) | — |
| 1829 | 22 | 0 | Boarding Shotgun, Pulzar, Pistol, DA CCW (PS 6); Killer Hacking Device, Hacker | — |

### Shasvastii Tactical Monitoring Company Mentor

**ID 1292 · AVA 3 · LI** — `MOV 10-10 | CC 16 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 6 | W 1 | S 2`. Shasvastii, Surprise Attack (-3), Camouflage, Mimetism (-3), Stealth, Decoy (1), Counterintelligence.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 20 | 0 | Vulkan Shotgun, Breaker Pistol, CCW | — |
| 2 | 24 | 0 | Shock Marksman Rifle, Breaker Pistol, CCW | — |
| 3 | 25 | 0.5 | Vulkan Shotgun, Breaker Pistol, CCW; Hacking Device, Hacker | — |
| 6 | 20 | 0 | Vulkan Shotgun, Breaker Pistol, CCW; Lieutenant | — |
| 7 | 24 | 0 | Shock Marksman Rifle, Breaker Pistol, CCW; Lieutenant | — |

### Shasvastii Seed-Soldiers

**ID 512 · AVA 4 · LI** — Seed-Soldiers are represented by a Seed-Embryo form and Developed Shape. The source notes that the Seed-Embryo profile can use only its Chest Mine and PARA CCW.

**SEED-EMBRYO:** `MOV — | CC 10 | BS 1 | PH 11 | WIP — | ARM 2 | BTS 3 | W 1 | S 0`. Shasvastii, Surprise Attack (-3), Camouflage (1 Use), Forward Deployment (+20), Mimetism (-3), Transmutation (Hatching); Chest Mine and PARA CCW.

**Developed Shape:** `MOV 10-10 | CC 16 | BS 11 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`. Surprise Attack (-3), Shasvastii.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 15 | 0 | Boarding Shotgun, Panzerfaust, Chest Mine, Boarding Pistol, PARA CCW | — |
| 2 | 16 | 0 | Combi Rifle, Panzerfaust, Chest Mine, Pistol, PARA CCW | — |
| 3 | 17 | 0 | Combi Rifle, Panzerfaust, Flash Pulse, Chest Mine, Pistol, PARA CCW; Forward Observer | — |
| 4 | 18 | 0 | Combi Rifle, Panzerfaust, Chest Mine, Pistol, PARA CCW; MediKit, Paramedic | — |

### E-Drones

**ID 741 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. EVO Hacking Device, Remote Presence, Courage, Hacker, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 17 | 0.5 | Combi Rifle, PARA CCW (-3) | — |

### Shasvastii Sabotage and Destruction Unit Caliban

**ID 528 · AVA 4 · LI** — `MOV 10-10 | CC 23 | BS 12 | PH 13 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Shasvastii, Surprise Attack (-3), Forward Deployment (+20), Dodge (+5), Mimetism (-3), Protheion, Stealth, Martial Arts L3, Courage, Camouflage, Immunity (Shock).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 0 | Boarding Shotgun, D-Charges, Pistol, CCW (PS 5) | — |
| 3 | 29 | 0 | SMG, Pulzar, D-Charges, Pistol, CCW (PS 5); Chain of Command | — |
| 4 | 28 | 0 | SMG, Pulzar, D-Charges, Pistol, CCW (PS 5); Deactivator, GizmoKit, Engineer | — |
| 5 | 26 | 0 | Vulkan Shotgun, Flash Pulse (+1B), D-Charges, Pistol, CCW (PS 5); Forward Observer | — |
| 7 | 26 | 0 | SMG, Pulzar, Grenades, D-Charges, Pistol, CCW (PS 5); Specialist Operative | — |
| 8 | 36 | 1.5 | Spitfire, D-Charges, Pistol, CCW (PS 5); MSV1 | — |

### Tensho Experts

**ID 1302 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 11 | PH 11 | WIP 14 | ARM 0 | BTS 3 | W 1 | S 2`. Shasvastii, Immunity (Shock), Specialist Operative, Regeneration, Stealth, Warhorse.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 3 | 14 | 0 | Boarding Shotgun, Pistol, CCW, Nanopulser | Nox max 1; source `(Nox)` |
| 4 | 16 | 0 | SMG, Pistol, CCW; Journalist | same |
| 5 | 16 | 0 | SMG, E/Mitter, Disco Baller, Pistol, CCW | same |

### Shasvastii Nox Troops

**ID 1290 · AVA Total (`255`) · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Shasvastii, Immunity (Shock), Stealth.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Zapper, Pistol, CCW | Nox 1–5 |
| 2 | 21 | 1 | HMG, Pistol, CCW | same |
| 3 | 15 | 1 | Combi Rifle, Grenade Launcher, Pistol, CCW | same |
| 4 | 19 | 1 | MULTI Sniper Rifle, Pistol, CCW | same |
| 6 | 14 | 0.5 | SMG, Zapper, Pistol, CCW; Hacking Device, Hacker | same |
| 7 | 15 | 0 | Combi Rifle, Zapper, Flash Pulse, Pistol, CCW; Forward Observer | same |
| 8 | 16 | 0 | Combi Rifle, Zapper, Pistol, CCW; MediKit, Paramedic | same |
| 10 | 14 | 0 | Combi Rifle, Zapper, Pistol, CCW; Lieutenant | same |
| 11 | 21 | 1 | MULTI Sniper Rifle, Pistol, CCW; BS Attack (Guided) | same |
| 13 | 16 | 0 | Combi Rifle, Zapper, Pistol, CCW; Commlink (+1), Specialist Operative | same |

### Oktavia Grímsdóttir, Icebreaker's Harpooner

**ID 1501 · AVA 1 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. Albedo (-3), BS Attack (+1B), Courage, Combat Instinct, Dogged.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 30 | 1.5 | Missile Launcher, Contender, Heavy Pistol, CCW | Nox max 1; source `(Nox)` |
| 2 | 26 | 1.5 | Heavy Rocket Launcher, Contender, Heavy Pistol, CCW; Sixth Sense | same |

### Shasvastii Corax Hasht

**ID 537 · AVA 1 · LI** — `MOV 10-10 | CC 19 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Nanoscreen, Shasvastii, Immunity (Shock), Stealth, Specialist Operative, No Wound Incapacitation, Combat Instinct, No Cover.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 1 | Red Fury, Breaker Pistol, CCW; Strategic Deployment | Wildcard max 1; Nox/Shasvastii Shock only |
| 2 | 29 | 0.5 | AP SMG, E/Mitter, AP Mine, Breaker Pistol, CCW; Strategic Deployment, Minelayer | same |
| 3 | 30 | 1 | Red Fury, Breaker Pistol, CCW | same |
| 4 | 33 | 1 | AP Spitfire, Breaker Pistol, CCW | same |

### R-Drones

**ID 511 · AVA 2 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Remote Presence, Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) | — |

### Shasvastii Special Armoured Corp Sphinx

**ID 524 · AVA 2 · TAG** — `MOV 15-15 | CC 20 | BS 14 | PH 15 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`. ECM: Guided (-6), BS Attack (SR-1), Surprise Attack (-3), Camouflage, Courage, Hidden Deployment, Mimetism (-6), Tactical Awareness, Terrain (Total), Climbing Plus, Remote Presence; includes a Scindron ancillary Remote.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 93 | 2 | Spitfire, Heavy Flamethrower (+1B), DA CCW (PS 5); includes Scindron | — |

**SCINDRON ancillary:** `MOV 15-10 | CC — | BS — | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Courage, Dodge (+3), Mimetism (-3), Specialist Operative, Terrain (Total), Peripheral (Ancillary); no independent Order.

## Canonical Fireteam chart

Fireteam limits in the pinned source: **Core 1; Haris 1; Duo unlimited** (`DUO: 256` sentinel).

### Nox Fireteams

**Types:** Haris, Core

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| NOX | 1 | 5 | no | — |
| TENSHO | 0 | 1 | no | Nox |
| T-DRONE | 0 | 1 | no | FTO profile only; Nox context |
| OKTAVIA | 0 | 1 | no | Nox |
| CORAX | 0 | 1 | no | Spec-Ops mode only |

### Shasvastii Shock Fireteams

The source labels this family `Shaveshii Shock Fireteams`; spelling is normalized here without changing its structure.

**Types:** Duo, Haris

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| JAYTH CUTTHROATS FTO | 0 | 3 | yes | Shasvastii Shock; FTO profiles only |
| GWAILO | 0 | 1 | yes | Shasvastii Shock |
| M-DRONE | 0 | 2 | no | FTO profile only |

The Jayth and Gwailo `required-choice` rows form a required-choice set from the Army chart; they are not interpreted here as requiring both unit types simultaneously.

### Haiduks Fireteams

**Types:** Duo, Haris

| Entry | Min | Max | Required-choice | Note |
|---|---:|---:|---|---|
| HAIDUK | 1 | 3 | no | — |

### Wildcards

| Entry | Max | Counts as / profile restriction |
|---|---:|---|
| SHESKIIN | 1 | Unrestricted Wildcard |
| CORAX HASHT | 1 | Nox and Shasvastii Shock contexts only |
| VICTOR MESSER | 1 | Shasvastii Shock context only |
| AÏDA SWANSON | 1 | FTO profile only; Nox context only |
| AGENT DUKASH FTO | 1 | FTO profile only |

## Reverse Fireteam index

| Unit | Fireteam access |
|---|---|
| Nox Troops | Nox Core/Haris, 1–5 |
| Tensho Experts | Nox Core/Haris max 1; source `(Nox)` |
| T-Drone FTO | Nox Core/Haris max 1; Opt 2 only |
| Oktavia Grímsdóttir | Nox Core/Haris max 1; source `(Nox)` |
| Corax Spec-Ops | Nox Core/Haris max 1 in Spec-Ops mode |
| Jayth Cutthroats FTO | Shasvastii Shock Duo/Haris required-choice max 3; Opts 1–4 only |
| Gwailos | Shasvastii Shock Duo/Haris required-choice max 1 |
| M-Drone FTO | Shasvastii Shock Duo/Haris max 2; Opt 2 only |
| Haiduks | Haiduk Duo/Haris, 1–3 |
| Sheskiin | Wildcard max 1 |
| Corax Hasht | Wildcard max 1; Nox and Shasvastii Shock contexts only |
| Victor Messer | Wildcard max 1; Shasvastii Shock context only |
| Aïda Swanson FTO | Wildcard max 1; Nox context only; Opt 2 only |
| Agent Dukash FTO | Wildcard max 1; Opt 1 only |

## Reinforcement linkage

The pinned Shasvastii Army data links Reinforcement roster **699**. This reference deliberately keeps Reinforcement roster entries and Reinforcement-specific Fireteams separate from the standard Shasvastii chart.

## Source pinning

- Army source version: `7.26246.158`
- Army data changed on: `2026-09-03`
- Army backup commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`
- Army source blob: `3876e25145c7efba4ba35546765977fafc0b19da`
- InfinityDB commit: `4e2662be3f43387fbae42b3790a711b3e98570c4`
- Rules baseline: N5.3 + N5 FAQ v0.1
- Verified/generated: `2026-10-15`

## Validation notes

- Standard roster count: **30 logical units**, excluding Shasvastii Corax Spec-Ops and Shasvastii Team-Ops optional modes and excluding generic mercenary-catalog entries with `factions: []`.
- Canonical Fireteam limits are Core 1, Haris 1, and unlimited Duo (`256` source sentinel).
- The source's `Shaveshii` / `Shavesii` spelling inconsistency is normalized to `Shasvastii` in prose while preserving the chart's family/context relationships.
- Jayth Cutthroats and Gwailos are a Shasvastii Shock required-choice set; the source does not mean every `required: true` row must be present simultaneously.
- Nox T-Drone access is FTO-only; Shasvastii Shock M-Drone access is FTO-only; Aïda's Nox Wildcard access is FTO-only; Agent Dukash Wildcard access is FTO-only.
- Jayth Pit Patrol is not granted Shock Fireteam access because the chart row specifically names `JAYTH CUTTHROATS FTO`.
- Seed-Soldier Seed-Embryo and Cadmus-Seed are transformation states rather than additional roster units.
- Sphinx/Scindron and Jayth Pit Patrol/Taigha are represented as parent/peripheral relationships rather than additional roster entries.
- Reinforcement roster 699 is linked but not mixed into the standard roster or Fireteam chart.

## Expanded Shasvastii tactical guide (2026-10-23)

Read the [Shasvastii Expeditionary Force tactical guide](../../notes/factions/shasvastii-expeditionary-force.md) for marker-state tempo, Speculo/Noctifer/Caliban choices, tournament face-up/face-down lists, Sphinx and Q/R-Drone coverage, plus Gwailo skepticism and tournament counterexamples. **Gwailo MSV2 is specific to the HRL option**, not its HMG; the current Shock chart retains eligible **M-Drone FTO** entries.

## Command-unit apex/value cross-reference (2026-10-23)

**Mentor LT** provides deceptive protected command; **Sheskiin LT** trades safety for active killing and benefits from separate CoC. **Caliban CoC 29/0** offers actual camouflaged forward specialist/assault utility, but keep it alive to take over rather than sacrificing it first. **Sphinx** is an expensive standalone stealth TAG, not an automatic LT; **Shasvastii/Embryo mechanics** don't make the rest of the roster immune to Loss of Lieutenant.

See [cross-game Lieutenant, CoC and Order-economy tiers](../../notes/list-building/command-units-apex-and-value.md). **Current pinned profiles and Fireteam chart above govern legality.**

## N5.3 mission specialists — apex/value decisions (2026-10-23)

**Caliban FO26, Engineer28, CoC29** is an exceptional Camo/FD+20 objective threat (different options), while **Shrouded FO24 and Malignos FO30/KHD32** trade lower cost for deeper Hidden Deployment. **M-Drone FO15/TA18** handles Sensor/Repeater and **Med-Tech21** supplies Doctor+Engineer with Slave service range, not servant-owned button activations. Preserve protected Caliban if it is the only CoC.

[Cross-game Mission Specialists / Button Pushers tiers](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). The current faction profile and Fireteam reference above controls legality.

## Airborne and enemy-DZ attack choices — N5.3 (2026-10-23)

**Speculo BSG26/1 or Minelayer31/1.5** is the best direct Impersonation assault/Turn-0 defense tax with Monofilament, but fragile single-W and failed kill may be negative trade. **Shas Cadmus BSG19/0 or KHD22/0** is a lower-cost Combat Jump/decoy attack; actual landing and state interaction must use pinned N5.3 rules. **Sphinx93/2** is the extreme **Hidden fast TAG** attacker, not Parachutist; **Caliban FD+20** and Shrouded/Malignos Camo pressure increase safe approach options. **Sheskiin LT48–50 on-table** can breach with Protheion; **Caliban CoC29** is separate hidden succession and should survive.

See [current cross-game apex/value, landing odds and expected-trade tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **This roster and Fireteam chart control exact loadout/availability.**

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **Sheskiin MULTI Rifle48/0** is the effective BS15 mobile close/midrange gun without SWC expense; **Red Fury50/1** trades SWC for better ranged Burst. **Sphinx Spitfire93/2** is a separate **TAG** category: Hidden/Mimetism(-6)/Climbing creates an oppressive first shot, but a non-AP Spitfire against top ARM is weak points value. **Speculo** changes defender positioning and can reveal the real attack route; avoid spending the whole turn on an unsuitable assassination when Sheskiin can exploit the opening. [Non-TAG/TAG apex and value rankings](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## TAG tactical cross-reference (2026-10-23)

**Sphinx (93)** is the premium Hidden Deployment, Camouflage, Mimetism(-6), Climbing Plus flanker: expose only after you identify a decisive attack route. Its Spitfire has no AP and 93 points weakens the secondary assault/scoring base, so the **2025 TAG podcast is strongly divided** on its overall value. The current profile supersedes older comments.

Across all factions, compare **apex power** separately from **points value**, counterplay and mission fit: [N5.3 TAG guide](../../notes/list-building/tags.md). The current unit profiles and canonical Fireteam chart above take precedence over tactical opinions.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Malignos KHD 32/0** gives **Hidden/Camo, Mimetism and Dazer** alongside Trinity for late scoring and cyber ambush; **Shrouded KHD 26/0 vs HD 28/0.5** is the cheaper Camo specialist choice. **Nox HD 14/0.5** is budget Carbonite/Oblivion/Spotlight, **Mentor HD 25/0.5** a more expensive command/defense piece, and **Cadmus AD KHD 22/0** reaches unexpected rear objectives. **Victor Messer 30–31/0.5** brings Deployable Repeater/Cybermine and defensive equipment. **Why:** Shasvastii's Hidden Deployment and midfield positioning are the main advantages; don't replace mission Camo with an expensive network shell when few good Repeaters exist. Note standard **KHD does not disable ordinary TAGs**.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

Cross-faction [apex and cost-value Order-generator rankings](../../notes/list-building/cheerleaders-and-order-generators.md), circumstance guide and transcript disagreements. **This file remains authoritative for profiles, AVA, Training and Fireteam legality.**

- 7pt R-Drone — cheap transferable Order, Repeater and Flash ARO; uses S3 space and AVA.
- 11pt Ikadron — Regular Baggage/Repeater with 2 light-flamethrower shots; guards lanes better than a bare beacon.
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

## N5.3 midfield area denial / speed bumps (tactical synthesis)

**Cheap layered markers:** **Shrouded Dazer Minelayer 21/0** blocks an approach via movement geometry; **Shrouded Shock Minelayer 24/.5** adds lethal corner denial. Regeneration/Camo density makes either harder to clear permanently. **Speculo 31/1.5 Shock Minelayer** imposes Impersonation plus a prepaid mine but cannot place its initial mine in an existing enemy's trigger area. **Counterpoint:** Dazer is low value where lanes bypass it; **Malignos** Hidden is dearer and should have a specific specialist/attack role rather than replace every Shrouded.

[Cross-game apex/value, matchups, and video/podcast disagreements](../../notes/list-building/midfield-area-denial-and-speed-bumps-apex-value.md). Qualitative tactics; the unit profile tables above remain authoritative.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Med-Tech Obsidon21 + Slave Drone3** provides cheap dual repair/revival: keep Drone behind **Sphinx TAG fallback** and one behind **Sheskiin** or other key VITA lane. A 70% base WIP14 Doctor attempt can kill the patient on failure; keep a legal Cube token reroll if relevant. Do not send the doctor itself through Shasvastii's aggressive marker ambush route unnecessarily. [Doctor/Engineer apex/value, odds and media disagreement](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## N5.3 DZ defense / anti-alpha-strike tactical choices

**Ikadron 11/0 Light Flamethrower(+1B)** is a Regular close-corner guard with **Baggage, Repeater, Dogged and Discover(+3)**, protecting more valuable Orders. **Q-Drone Thunderbolt TR+360º 20/.5** covers rear/roof approaches and can be repaired. **Noctifer hidden ML30/1.5** is a different *second gate* that may punish commitment but loses normal Order contribution while Hidden; **Victor Messer 30/.5 Minelayer(2) Cybermines** is sophisticated but dear for mere cheerleader protection. **Counterpoint (Shepherd N4 concepts):** Q-Drone+Noctifer placement forces two problems, but an impersonator/corner bypass may skip the expensive long sightline altogether. Use cheap templates/mines at the actual extraction square.

[Whole-game DZ-defender apex/value tiers and media disagreements](../../notes/list-building/dz-defenders-alpha-strike-and-impersonation-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Speculo BSG26/1** combines Impersonation, Monofilament, MA3 and regenerating one-Wound threat against TAGs/HI, but pays SWC; **Caliban BSG24/0** is Camo/FD+20 MA3 **Protheion on VITA**, better when nearby unarmored targets allow growth and scoring. **Sheskiin48/0 or 50/1** is a **BS15 + MA4/CC24/DA** two-Wound repeat attacker, not a cheap disposable assassin; Protheion does not grow from enemy STR. Enemy Biometric/Guard/mines defeat careless Impersonation arrival. [CC assassin apex/value, Guard, anti-CC and evidence](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## N5.3 network projection — Pitchers, Repeaters, TinBots and disposable delivery

**R-Drone7/0 Flash/native Repeater**, **Ikadron11/0 native Repeater/LFT/Baggage**, **M-Drone FO/Sensor/Repeater** establish low-cost network for protected hackers, while **Victor Messer Cybermine/Deployable Repeater Minelayer(2)30/.5** can pre-place remote nodes on the *actual chosen Minelayer profile* (the 31/.5 ECM-Guided TinBot option is separate). Hidden/forward Shasvastii units instead deny different approaches; do **not** claim that owning Mines alone means a free deployed Repeater. **Counter:** cyber network without worthwhile Hackable targets is weaker than Shrouded mine/Noctifer ARO and physical screens, and enemy KHDs can retaliate via exposed nodes.

[Whole-game network projection: apex/value, current profiles, and opposing transcript views](../../notes/list-building/network-projection-repeaters-pitchers-apex-value.md).

## Tactical cross-reference — toolbox units (2026-10-23)

**Caliban FO26/0, Engineer28/0 or CoC29/0** compress Camo/FD+20/Protheion/MA3/CC23 with a **profile-specific** objective, repair or command job. **MSV1 Spitfire36/1.5 is a DIFFERENT combat-only loadout.** 2026 tournament evidence supports multiple independent Caliban plus a conventional ranged gun, while one 1W Caliban left exposed remains vulnerable. **Sheskiin** is better direct combat but not a hacker/scoring specialist. [Cross-game toolbox tiers](../../notes/list-building/jack-of-all-trades-toolbox-units-apex-value.md).

## N5.3 rare abilities & unusual combinations — tactical synthesis

**Caliban Camo+FD(+20)+MA3+Protheion BSG24/0** is the rare *shoot/ambush first, then CC-feed* piece; if you need another useful job choose **Engineer28/0, CoC29/0, FO26/0**. Feeding heals or gains up to **+2 VITA** from **legal CC wounds on VITA targets**, not STR or shooting. **Sheskiin MULTI Rifle48/0, Red Fury50/1** combines BS15, 15-10 MOV, Nanoscreen, 2W and Protheion for an apex snowball but wants a safe exit and several useful combats. **Gwailos HRL+MSV2+Albedo(-6)39/1.5** uniquely attacks visors and camo with Nanoscreen; **44/1.5 HMG lacks HRL profile's MSV2**, don't merge. **Real debate:** TA early-N5 lists skip Caliban for easier Shrouded/Speculo; MetaChemistry 2026 event winner used multiple Calibans and fed a victim to reach VITA3; a specific success, not universal autopick.

[Cross-faction rare abilities apex/value, mechanics, and MCP source debates](../../notes/list-building/rare-capabilities-and-unique-combinations-apex-value.md). Current roster/Fireteam profile tables above are authoritative.

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Seed Soldier15/0 Panzerfaust+Chest Mine**, **Tensho16 E/Mitter**, and **Malignos31 Monofilament Minelayer** provide ordinary, electronic and hidden path denial. **Speculo26/1** is the true Impersonation+Monofilament execution specialist; **Noctifer ML30/1.5** threatens a hard TAG ARO unexpectedly; **Gwailos E/M Carbine(+1B)** is a higher-cost repeatable specialist. Engineer/Reset may undo E/M; marker delivery only works if the enemy has not screened its actual TAG base. [Cross-game anti-armor apex/value, E/M and AP+EXP guide](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## Tactical cross-reference — indirect fire (2026-10-23)

**T-Drone Guided16/1.5** complements **Victor Messer/FO/Shrouded/M-Drone** rather than replaces a Noctifer/Gwailo/Sheskiin direct threat. **Nox Grenade Launcher15/1** offers cheap independent B1 Speculative while **Nox MULTI Sniper Guided21/1** is another role-specific profile; do not treat either as the T-Drone's off-board missile chassis. Expensive Spec/Guided plans compete with Shasvastii's independently useful Camo, Protheion and mission pressure. [Whole-game guide](../../notes/list-building/indirect-fire-speculative-guided-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Shasvastii-specific rule:** in official **Domination**, **Shasvastii Embryo as well as Normal** counts its points in quadrant; don't generalize to Supplies or equipment tokens. **Caliban FO26/0** Camo/FD+20/Protheion is sturdy *once it feeds VITA*, but starts ARM1 W1; **Shrouded/Malignos FO** are better ambush/pickup than carrying openly, because box forces non-Marker. **Sphinx93/2** 3STR/Hidden/Mimetism(-6) can shift 93 zone points only when *actually represented*, and is not an ordinary eligible carrier; use it to defend a protected specialist. **MetaChemistry 2026 event winner:** multiple Calibans and surviving camo/embryo bodies won quadrants by careful mission timing; counter is Sensor+mines and crossing the other zone instead of spending 6 Orders hunting one marker.

[Cross-game zone-holder and carrier apex/value, mission rules, and opposing transcripts](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Current local roster/FT chart is authoritative.

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**M-Drone FO/Sensor/Triangulated Fire** detects **enemy Camouflage/Hidden** within ZoC at far lower investment than a specialized sniper; **Shrouded/Malignos/Caliban Camo** protect your own approach but **are not detectors** just by being markers. **Charontid MSV3 is not ordinary Shasvastii roster access**: use legal **Shrouded/Noctifer ambush, Caliban flanks, Nox MSV2, or Aswang Albedo** profiles where present. **Counter:** Sensor cannot mass-reveal IMP-1 and does not automatically detect an opposing Speculo; mines/DTW/guard screening cover the impersonator problem. Do not treat the opponent's Camo shell and your own Hidden deployment as the same ability.

[Non-hacking & tech-specific counter-selection, N5.3 anti-tech apex/value and opposing MCP transcripts](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## Force multipliers — N5.3 role/value cross-reference (2026-10-23)

**Camo/Decoy LT and mines** make enemy sensor/discover priorities uncertain, but **Decoy replicas do not provide Orders, independent AROs or extra Mines**. **Ikadron Baggage** supports Pitcher/Deployable stock and orders but needs real ZoC/reload access. **EVO14/.5** is not mandatory just to support a Q-Drone or Guide missiles; choose when its *printed supportware* improves active gun/ARO or airborne arrival enough to beat buying another actual specialist. [Force multiplier roles](../../notes/list-building/force-multipliers-special-abilities-apex-value.md).

## N5.3 peripheral / synchronized / multi-body apex-value update

**Shasvastii multi-body advantage** concentrates on **Sphinx + Scindron Ancillary** and **Doctor/Engineer+Servants**, not Next Wave-style autonomous Cyberplugs or Nomad Pupniks. **Sphinx93/2** 3STR/Hidden/Mimetism(-6)/Climbing+ with included **Scindron Specialist Operative**: ancillary **not on board at deployment**, Sphinx must **Place Deployable** to release it. Does not give 2 Regular Orders or a free Hidden-Specialist on another side of table. **Shasvastii Embryo** is a *state/model scoring exception* in Domination, **not** a Peripheral or extra attacking body. **Opponent view:** keep Sphinx hidden and preserve special scoring protection, but deploying Scindron late has a real Order cost and can alter Fireteam/Hidden-based plans; cheap Caliban/Speculo are independent attackers with independent Orders, often more flexible.

[Whole-game N5.3 Peripheral & Multi-Body Apex/Value guide](../../notes/list-building/peripheral-synchronized-multibody-apex-value.md). Exact current roster, dependency and Fireteam chart above override commentary.

## Battle-report effectiveness and combinations (qualitative, 2026-11-01)

**Observed successful role split:** **Shrouded + Malignos hidden specialists/mines + Speculo Killers/Calibans** make a multi-marker shell that taxes Discover Orders and holds objectives away from the opponent's elite attack. #159's winning Shasvastii report consciously scored *around* an Achilles/Pandora hero link; #196 shows saturation/Decoy coverage. [#159](../../notes/battle-reports/151-160-n5-battle-report-tactical-analysis.md) · [#196](../../notes/battle-reports/191-200-n5-battle-report-tactical-analysis.md).

**Overinvestment trap:** In #231 **Sphinx** reportedly killed about four targets but spent ~9–10 Orders, leaving a Torchlight **Moonraker/Jamie** attack able to hit Med-Tech/EVO/order support while winning distant Battleground bands 10–0. #189 similarly shows **Sphinx/Sheskiin** gun strength failing to complete collector deliveries while a single TR HMG guarded both circles. [#231](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md) · [#189](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md).

**Recommendation:** Preserve a **second non-Sphinx mission route**, screen the rear against Parachutists and be willing to use Hidden Deployment solely for deterrence/zone points. These are mission-dependent losses, not proof the TAG is generally weak.

[Cross-report synthesis and evidence cautions](../../notes/battle-reports/cross-report-unit-effectiveness-and-combinations.md).

## Mission performance — battle-report evidence (2026-11-01)

| Mission(s) | Tested composition / scoring mechanism | Evidence |
|---|---|---|
| **Provisioning / Area of Interest** | Shrouded/Malignos hidden specialists, Caliban, Speculo and Decoy mines create multiple early/late objective paths while enemy spends Discover Orders. | [#159](../../notes/battle-reports/151-160-n5-battle-report-tactical-analysis.md), [#187](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md), [#196](../../notes/battle-reports/191-200-n5-battle-report-tactical-analysis.md) |
| **Data Harvest / collector warning** | Sphinx/Sheskiin firepower failed to complete collection/delivery while Tohaa controlled the scored corridor. | [#189](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md) |
| **Battleground / distant band warning** | Sphinx killed approximately four for nine–ten Orders but Torchlight Jamie/Moonraker entered the backfield and won 10–0. | [#231](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md) |

**Limits:** Tackle rear-edge defense and delivery Orders before an expensive Sphinx alpha. Game-era qualitative evidence, not a win-rate or current Fireteam claim. [Full mission evidence audit](../../notes/battle-reports/cross-report-mission-performance-by-sectorial.md).

## Counterplay — observed N5 battle-report responses (2026-11-02)

| Threat / target | Observed response and limitation | Battle reports |
|---|---|---|
| **Vs TAG/vehicle or airborne** | Sāchā E/M grenade genuinely disabled Next Wave Skyhound on a critical; Shrouded/Malignos hacker, Q-Drone/M-Drone Sensor can threaten flyers, but anti-flyer overinvestment lost Provisioning. | [#187](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md) |
| **Camo/Impersonator pressure** | Speculo + Shrouded/Malignos/Dazer saturation used opponent Discover and Camo-avoidance Orders, held Area of Interest zones against Next Wave. | [#159](../../notes/battle-reports/151-160-n5-battle-report-tactical-analysis.md), [#196](../../notes/battle-reports/191-200-n5-battle-report-tactical-analysis.md) |
| **How opponents beat Shas Camo** | Hassassin McMurrough smoke + cheap Daylami mine clearance + Muyib/Yara/Leila D-Charges crossed Malignos/Shrouded screen in Double Bind; WinterFor Peacemaker mines/turrets repelled late Speculo room breach. | [#232](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md), [#182](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md) |
| **TAG overcommit risk** | Sphinx spent nine–ten Orders for about four kills while Jamie/Moonraker removed fragile Med-Tech/EVO backline and scored Battleground 10–0. | [#231](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md) |

**Limit:** Do not infer that a Sensor automatically removes Impersonation; #187 E/M critical was a single high-variance event. These are historical qualitative interactions, not present N5.3 unit, Fireteam, or win-rate claims. [Full cross-report counterplay analysis](../../notes/battle-reports/n5-cross-report-counterplay-tags-hi-hacking-camo-impersonators-fireteams.md).

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

### 3. Shasvastii Expeditionary Force

**Sources:** [Robert Shepherd, *SEF faction focus*](https://www.youtube.com/watch?v=mtqHMuHmjjo) (full transcript rechecked; older analysis); [Tactical Awareness S3E12 Shasvastii](https://open.spotify.com/episode/0oGd3tdSkCtTp2Yi99sRc5) (full podcast transcript rechecked); [MetaChemistry E139 — 2026 Battle by the Beach winner Brian/Nazeen](https://open.spotify.com/episode/6FErkreAsQoUKosH4WkdPW) (full podcast transcript rechecked; actual 2026 tournament evidence); [existing SEF guide](../../notes/factions/shasvastii-expeditionary-force.md); [N5.3 roster](shasvastii.md).

**No defensible universal individual “must-have.”** The **2026 winner** describes at least two genuinely different solutions: a **face-down** build (2 Speculo, 3 Caliban, Shrouded, order bots, solo late-game Jayth) and a **face-up** mission/gun build (Sheskiin + Nox/Tensho specialists, Gwailo + Victor). Calling Speculo, Sheskiin, Gwailo or Noctifer mandatory across **both** would erase this direct evidence.

**Go-to**
- **Speculo Killer** — Impersonation/Mines makes opponent defend deployment and priority pieces; doubles exaggerate the threat, but cost Orders/specialists.
- **Caliban specialist / Engineer / MSV Spitfire and Shrouded FO/Minelayer/Dazer** — advanced Camo, objective scoring, Protheion or persistent area denial; Caliban stronger attacker, Shrouded cheaper workhorse.
- **Noctifer ML or Spitfire** — Hidden Deployment threatens ARO **or** opens a hidden attack route. Missile is not automatic; threatened shot can be prevented, while Spitfire offers a more proactive gun.
- **Sheskiin gunfighter** — rapid all-round assault, Protheion durability if kills are accessible; strong *when the mission wants face-up tempo*, not universal.
- **Mentor LT Counterintelligence/Decoy; Taigha; Ikadron / R-Drone / Q-Drone** — command shelter, rapid cheap trade and cheap defence. Irregular Taigha cannot simply replace Regular pooled activations.
- **Gwailo HRL MSV2 (39/1.5) + Victor Messer in eligible Shock arrangement** — late-2026 precedent for lane denial and objective-focused teamwork. **Important:** the **44pt Gwailo HMG does not have MSV2** in the current roster.
- **Jayth with disco balls, Dukash, Malignos** — mission-specific visibility bypass, flank attack and premium hidden specialist.

**Avoid / profile-qualified**
- **Cadmus KHD 22/0 instead of Boarding Shotgun 19/0 for a plain backline kill-drop** — **Direct:** Shepherd says not to buy the KHD for that specific job, which the cheaper BSG is designed for. **Not an absolute:** the extra 3 points add a Specialist/KHD for missions that need one.
- **Historical Cadmus Red Fury rejection is *not actionable***: the speaker also says not to buy the Red Fury, but **that profile is not present in the pinned 2026 roster**. Likewise an old, expensive hackable/armoured Sheskiin discussed on video is not a current listed loadout; don't import old “never take” claims.
- **Not “never take”: Gwailo, Jayth, Sphinx, Noctifer ML.** Shepherd was skeptical of some costs; Brian's 2026 event use strongly contradicts treating Gwailo/Jayth as traps. Sphinx 93pt/2SWC is a matchup and specialist/opportunity-cost question, not a proven bad unit.

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

#### 3. Shasvastii Expeditionary Force — expensive stealth duplicates and 2026 evidence corrections

| Unit, profile or quantity | Why it can be weak, rare or tempting to overbuy | Buying verdict / contradictory evidence |
|---|---|---|
| **Cadmus KHD22 for a simple rear-entry BSG kill** | **Direct [Shepherd SEF](https://www.youtube.com/watch?v=mtqHMuHmjjo):** the **19pt BSG** performs the simple lethal drop more cheaply. KHD buys a distinct specialist/hacker mission; old Cadmus Red Fury negative is **irrelevant because that profile is absent in pinned N5.3**. | **Avoid *KHD for a pure kill-drop*, not the whole Cadmus unit**. **Proxy the extra 3pt variant** using one Cadmus miniature until hacking/scoring requires it. |
| **Sphinx as the default frontal anti-TAG solution** | **Contested:** stealth/Climbing Plus/Mimetism(-6) excels into **soft Orders, flanks and late scoring**, while cost and limited AP make long direct armor duels unreliable. Earlier Sphinx champions favour patient strikes/retreat; N5 critics cite 93pt opportunity cost. | **Proxy first before expensive TAG purchase**, *unless* practising a dedicated Sphinx list. Multiple TAGs (**SEF AVA2**) are a skew to test rather than an obligation. |
| **Gwailo written off as too costly / blind extra Gwailo purchase** | **Conflict must survive:** old reviewers criticize Gwailo's investment, but [MetaChemistry 2026 tournament winner](https://open.spotify.com/episode/6FErkreAsQoUKosH4WkdPW) actually fielded **Gwailo + Victor** in a face-up style. Current **Gwailo HRL has MSV2, HMG does not**; this is a profile and mission distinction. | **Not a verified bad unit**. **If trying a Gwailo-centered list, buy/proxy one** (AVA1); do not buy an HMG sculpt based on nonexistent HMG MSV2 synergy. |
| **Jayth as an automatic cheap filler, or surplus full Jayth link** | **Contested:** fragile short-range/close positioning can make an expensive assault team awkward; **2026 winning Shasvastii list used a solo Jayth in late-game work**. Only **FTO Jayth** are eligible for the listed Shasvastii Shock team. | **Proxy-test first**, particularly extra Jayth beyond the one specific assault/mission role. **Do not label whole Jayth “worst” after actual winning-list use.** |
| **Second Speculo Killer / fourth Caliban / additional Shrouded or Malignos without a specific marker plan** | **Direct tournament counterexample to blanket avoidance:** the **2026 winner fielded TWO Speculos and THREE Calibans** in a “face-down” plan. But not *every* mission/list needs that many high-quality hidden/infiltrating attackers; Caliban, Shrouded and Malignos do different price/mission/assault jobs. | **Proxy the extra models for the specific double-impersonator or many-camo list**, instead of buying AVA2/4/3 merely to fill options. **The first Caliban/Shrouded/Speculo remains strongly defensible**. |
| **Haiduk, third Noctifer or expensive specialty sniper as a routine additional ARO gun** | **Inference:** **Haiduk** provides a legal distinct Duo/Haris and dedicated sniper/fire lane; **Noctifer ML** adds Hidden ARO surprise, **Q-Drone** recoverable defense. Several may become inactive while objective runners run out of Orders. A legal Haiduk team can be a deliberate strategy. | **Proxy extra snipers / third Noctifer**, not the first useful **Noctifer ML**. **Unrated as universally poor**, since the defensive roles and team permissions differ. |
| **Seed-Soldier / Nox multiple gun sculpts solely for inexpensive Orders** | **Inference:** **Nox + Tensho** can be a legitimate face-up specialist team, while Seed-Soldiers have transformation/hidden placement quirks; basic infantry bodies are often cheaper and more versatile than another elite gun. The current roster has no reason to buy all sculpts for each loadout. | **Proxy an alternate Nox/Seed Soldier profile** and buy only actual **simultaneous** link/scorer counts. **Represent the selected profile's state and footprint correctly**. |
| **Agent Dukash, Corax Hasht, Oktavia or Aïda bought simply for every one-off named slot** | **Lower-confidence unranked:** specialist fireteam and unique weapon/delivery roles are genuine; none is singled out as a definitive worst whole model by the media above. **Aïda FTO, Dukash FTO** and other character team rights are option/row-specific. | **Proxy-test each named character with a distinct compatible model** until a particular legal FTO and mission use occurs repeatedly. Do not invent a universal “never take” rating. |
| **Extra Guided T-Drone, EVO E-Drone or M-Drone FTO acquired merely to link/launch missiles** | **Conditional:** **T-Drone FTO** can join a Nox team, **M-Drone FTO** a Shock team, but only the correct option and chart row. E-Drone EVO needs actual Supportware target; Guided needs Targeted. | **Avoid imaginary/unsupported variants**, and **proxy existing correct-size REM chassis** before buying multiple alternatives. This is not a ban on cheap Q-/R-/M-Drone support. |
| **Taigha saturation up to AVA8 without Regular-order and mission plan** | **Inference:** extremely dangerous cheap rush/trade pieces, but **Irregular/Impetuous** and 15-slot costs are meaningful. Tourney success with stealth/hidden pieces doesn't imply buying every available Taigha. | **Proxy fifth–eighth models first**, not the first few that actually protect the marker screen. State exact legal model count and availability. |

**Sources:** [Shepherd SEF](https://www.youtube.com/watch?v=mtqHMuHmjjo), [Tactical Awareness Shasvastii](https://open.spotify.com/episode/0oGd3tdSkCtTp2Yi99sRc5), [MetaChemistry E139 / 2026 winner](https://open.spotify.com/episode/6FErkreAsQoUKosH4WkdPW), [Shasvastii guide](../../notes/factions/shasvastii-expeditionary-force.md). **For shopping**, the riskiest assumption is *“everything unique and hidden must be owned at full AVA.”* The evidence shows deliberately different **face-down** and **face-up** lists, and directly prevents “Gwailo/Jayth bad” generalizations.

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
