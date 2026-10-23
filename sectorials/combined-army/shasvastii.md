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

## TAG tactical cross-reference (2026-10-23)

**Sphinx (93)** is the premium Hidden Deployment, Camouflage, Mimetism(-6), Climbing Plus flanker: expose only after you identify a decisive attack route. Its Spitfire has no AP and 93 points weakens the secondary assault/scoring base, so the **2025 TAG podcast is strongly divided** on its overall value. The current profile supersedes older comments.

Across all factions, compare **apex power** separately from **points value**, counterplay and mission fit: [N5.3 TAG guide](../../notes/list-building/tags.md). The current unit profiles and canonical Fireteam chart above take precedence over tactical opinions.
