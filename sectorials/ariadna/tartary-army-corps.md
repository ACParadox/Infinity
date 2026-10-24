---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 305
sectorial_slug: tartary
sectorial_name: Tartary Army Corps
parent_faction: Ariadna
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Tartary Army Corps (TAK) roster, standard loadouts, canonical Fireteam chart, reverse Fireteam index, and the distinct L'Équipe Argent Reinforcement Fireteam chart. Intel Spec-Ops and Ariadna Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# Tartary Army Corps

## Overview and provenance

Repository-native reference for **Tartary Army Corps (TAK)** roster, profiles, points/SWC, AVA, and Fireteam access.

Sources used:

- Army-derived TAK source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `d4329bb596ffea5d568eb2435f74366c305a7630`.
- InfinityDB Fireteam normalization/identity semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **30-unit standard TAK roster** and the complete standard TAK `fireteamChart` in the pinned Army source.
- Soldier of Fortune / generic `merc-*` catalog entries whose source faction list is empty are excluded from the base roster.
- `Intel Spec-Ops` and `Ariadna Team-Ops` are optional game-mode content and are listed separately.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name by itself.
- Parenthetical Army-chart comments are treated as Counts-as / equivalence labels, not as join-scope restrictions.
- Structured `required: true` rows in Veterans, Mobility, and Gunnery Fireteams are preserved as required-choice sets; this file does not reinterpret them as requiring every marked troop type simultaneously.
- Profile restrictions are preserved: only `KONDUKTOR FTO`, `BEASTHUNTER FTO`, and `BARSUK FTO` profiles receive the Fireteam access granted to those named chart entries.
- Linked Reinforcement army ID: **399**, **L'Équipe Argent**. Its Fireteam chart is recorded separately below and is not merged into the main TAK chart.

InfinityDB's current identity summary describes TAK as a veteran Kazak force built around camouflage, ambushes, resilient attack pieces, long-range pressure, and midfield presence.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Tartary Army Corps (TAK) |
| Parent faction | Ariadna |
| Army ID | 305 |
| Army slug | `tartary` |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 30 |
| Optional-mode units | Intel Spec-Ops; Ariadna Team-Ops |
| Reinforcement roster | L'Équipe Argent, Army ID `399` |
| Fireteam limits | Core 1; Haris 1; Duo unlimited |
| Fireteam chart | yes |

## Roster index

| Unit | ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| Col. Yevgueni Voronin | 768 | 1 | LI | Regular | Wildcard; counts as Line Kazak |
| Dog-Warriors | 242 | 3 | WB | Irregular + Impetuous | — |
| Frontoviks | 1136 | 5 | LI | Regular | Line Kazaks; Veterans required-choice; Mobility; counts as Line Kazak / Veteran / Ratnik by row |
| 112, Emergency Service (Motorized) | 1284 | 2 | LI | Regular | Mobility |
| 112, Emergency Service | 255 | 2 | LI | Regular | Veterans |
| Vystrel Mobile Artillery Regiment | 1846 | 2 | REM | Regular | Gunnery required-choice; counts as Gunnery |
| Wardrivers, Mercenary Hackers | 265 | 1 | LI | Regular | — |
| Kazak Spetsnazs | 229 | 4 | MI | Regular | — |
| TankHunters | 231 | 4 | MI | Regular | — |
| Scouts | 238 | 4 | SK | Regular | — |
| Carmen Johns & Bâtard | 1153 | 1 | WB | Irregular + Impetuous | — |
| Beasthunters Free Guild | 1570 | 1 | SK | Irregular | Line Kazaks, FTO profile only |
| Dynamo | 1134 | 5 | LI | Regular + Impetuous | Mobility required-choice |
| Konduktors | 1844 | 2 | LI | Regular | Line Kazaks, FTO profiles only |
| Barsuk, Territorial Defense Reg. | 1845 | 3 | MI | Regular | Wildcard, FTO profiles only; counts as Line Kazaks / Gunnery |
| Streloks | 1126 | 4 | LI | Regular | — |
| Irmandinhos | 240 | 4 | WB | Irregular + Impetuous | — |
| Pavel Aleksei McMannus | 1152 | 1 | SK | Regular | — |
| Antipode Assault Pack | 241 | 2 | WB | Regular + Tactical Awareness | — |
| Kuryer Unit | 1524 | 2 | REM | Regular | Gunnery required-choice; counts as Gunnery |
| Vassily Plushenko | 1150 | 1 | MI | Regular | — |
| Warcors | 50 | 1 | LI | Irregular | — |
| Ratnik | 1127 | 3 | HI | Regular + Tactical Awareness | Mobility required-choice |
| Line Kazaks | 227 | TOTAL | LI | Regular | Line Kazaks |
| Traktor Mul | 257 | 2 | REM | Regular | Gunnery required-choice; counts as Gunnery |
| Kazak Doktor | 243 | 3 | LI | Regular | Line Kazaks; counts as Line Kazak |
| Dozers, Field Engineers | 256 | 2 | LI | Regular | Line Kazaks; Gunnery; counts as Line Kazak / Gunnery |
| Veteran Kazaks | 234 | 5 | HI | Regular | Line Kazaks; Veterans required-choice; counts as Veteran |
| Remontnikbot V-5 Elektronik | 1581 | 1 | REM | Peripheral | — |
| Ioann Bann | 1940 | 1 | WB | Irregular | Mobility |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Intel Spec-Ops | 1915 | Spec-Ops | Line Kazaks Fireteam row, max 1 when Spec-Ops mode is in use |
| Ariadna Team-Ops | 1929 | Team-Ops | No ordinary TAK Fireteam row |

## Unit details

### Col. Yevgueni Voronin

**ID 768 · AVA 1 · LI** — `MOV 10-10 | CC 22 | BS 11 | PH 12 | WIP 14 | ARM 0 | BTS 0 | W 1 | S 4`. Martial Arts L2, Guard, Sixth Sense, Sensor, Counterintelligence, Combat Instinct.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 18 | 0 | Light Shotgun, Flash Pulse, Pistol, AP CCW | Wildcard; counts as Line Kazak |
| 2 | 22 | 0 | As Opt 1; Lieutenant (+1 Command Token) | same |
| 3 | 18 | 0 | T2 Boarding Shotgun, Pistol, AP CCW | same |
| 4 | 22 | 0 | As Opt 3; Lieutenant (+1 Command Token) | same |

### Dog-Warriors

**ID 242 · AVA 3 · WB** — Dogface: `MOV 15-10 | CC 21 | BS 10 | PH 14 | WIP 12 | ARM 1 | BTS 0 | W 3 | S 2`; Dog-Warrior form: `MOV 15-10 | CC 23 | BS 10 | PH 16 | WIP 12 | ARM 3 | BTS 3 | W 3 | S 6`. Courage, Super-Jump, Berserk, Dodge (+2.5), Immunity (ARM), No Cover, Transmutation (1), Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 837 | 21 | 0 | Chain Rifle, Grenades, Smoke Grenades, AP CCW; Irregular + Impetuous | — |

### Frontoviks, Separate Assault Battalion

**ID 1136 · AVA 5 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 11 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. Courage, Mimetism (-3), Warhorse.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | T2 Rifle, Assault Pistol, CCW | Line Kazaks max 1; Veterans max 5; Mobility max 2 |
| 2 | 30 | 1 | AP Spitfire, Assault Pistol, CCW | same |
| 3 | 19 | 1.5 | Heavy Rocket Launcher, Assault Pistol, CCW | same |
| 6 | 26 | 0 | T2 Rifle, Panzerfaust, D-Charges, Assault Pistol, CCW; Engineer, Deactivator | same |
| 7 | 23 | 0 | T2 Rifle, Assault Pistol, CCW; MediKit, Paramedic | same |
| 8 | 28 | 0.5 | AP Sniper Rifle, Assault Pistol, CCW; MSV1 | same |
| 9 | 21 | 0 | T2 Rifle, Assault Pistol, CCW; Lieutenant | same |

Counts as Line Kazak in the Line Kazaks chart, Veteran in the Veterans chart, and Ratnik in the Mobility chart.

### 112, Emergency Service (Motorized)

**ID 1284 · AVA 2 · LI** — `MOV 20-10 | CC 16 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 4`. Doctor, Courage, Mimetism (-3), Limited Cover; MediKit, Motorcycle.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4761 | 19 | 0 | Light Shotgun, Smoke Grenade Launcher, Smoke Grenades, Boarding Pistol, CCW | Mobility max 1 |

### 112, Emergency Service

**ID 255 · AVA 2 · LI** — `MOV 10-10 | CC 16 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Doctor, Courage; MediKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 11 | 0 | **112 FTO**; Light Shotgun, Boarding Pistol, CCW | Veterans max 2 |

### Vystrel Mobile Artillery Regiment

**ID 1846 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 12 | PH 9 | WIP 12 | ARM 2 | BTS 0 | W 2 | S 4`. Remote Presence, Courage, Sapper, BS Attack (SR-1), BS Attack (Shock), ECM: Guided (-6).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0.5 | AP Sniper Rifle, Light Rocket Launcher, PARA CCW | Gunnery required-choice, max 2; counts as Gunnery |
| 2 | 32 | 1.5 | Portable Autocannon, Light Rocket Launcher, PARA CCW; Neurocinetics | same |
| 3 | 26 | 0.5 | AP Sniper Rifle, Light Rocket Launcher, PARA CCW; Neurocinetics | same |

### Wardrivers, Mercenary Hackers

**ID 265 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`. Sixth Sense.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 1 | Boarding Shotgun, Flash Pulse, Cybermine, Pistol, CCW; Hacking Device with UPGRADE: Zero Pain, Hacker | — |
| 2 | 16 | 1 | As Opt 1 plus Disco Baller | — |

### Kazak Spetsnazs

**ID 229 · AVA 4 · MI** — `MOV 10-10 | CC 21 | BS 12 | PH 12 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. Martial Arts L2, BS Attack (Shock), Courage, Marksmanship, Stealth, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 36 | 1.5 | HMG, Silenced Pistol, AP CCW; Camouflage, Surprise Attack (-3), Decoy (1) | — |
| 2 | 32 | 0.5 | AP Sniper Rifle, Silenced Pistol, AP CCW; same camouflage package | — |
| 3 | 27 | 0 | Boarding Shotgun, Grenades, D-Charges, Silenced Pistol, AP CCW; Parachutist, Decoy (1) | — |
| 4 | 27 | 0 | AP Submachine Gun, Grenades, D-Charges, Silenced Pistol, AP CCW; Parachutist, Decoy (1) | — |

### TankHunters

**ID 231 · AVA 4 · MI** — `MOV 10-10 | CC 14 | BS 13 | PH 12 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 2`. Camouflage, Surprise Attack (-3), Courage, Mimetism (-3), Stealth.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 1.5 | AP HMG, D-Charges, AP Mine, Pistol, CCW | — |
| 2 | 36 | 1.5 | Portable Autocannon, D-Charges, AP Mine, Pistol, CCW | — |
| 3 | 28 | 1.5 | Missile Launcher, D-Charges, AP Mine, Pistol, CCW | — |
| 4 | 25 | 0 | AP SMG, Panzerfaust, D-Charges, AP Mine, Pistol, CCW; Chain of Command, Minelayer | — |
| 5 | 24 | 0.5 | AP SMG, Panzerfaust, D-Charges, AP Mine, Pistol, CCW; Forward Deployment (+20), Minelayer | — |
| 6 | 25 | 0 | AP Rifle, Adhesive Launcher Rifle, D-Charges, AP Mine, Pistol, CCW; Minelayer | — |
| 7 | 25 | 0 | As Opt 6; Lieutenant | — |

### Scouts

**ID 238 · AVA 4 · SK** — `MOV 10-10 | CC 15 | BS 12 | PH 13 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. BS Attack (AP), Camouflage, Surprise Attack (-3), Mimetism (-3), Terrain (Total), Stealth, Infiltration.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 27 | 0 | Ohotnik, D-Charges, Shock Mine, Silenced Pistol, CCW | — |
| 2 | 27 | 0 | Ohotnik, D-Charges, PARA Mine, Silenced Pistol, CCW | — |
| 3 | 23 | 0 | T2 Boarding Shotgun, D-Charges, Shock Mine, Silenced Pistol, CCW | — |
| 4 | 25 | 0.5 | T2 Sniper Rifle, Shock Mine, Silenced Pistol, CCW | — |
| 5 | 28 | 0.5 | Ohotnik, D-Charges, E/M Mine, Silenced Pistol, CCW; Minelayer (2) | — |
| 7 | 28 | 0 | Ohotnik, D-Charges, Flash Pulse, Shock Mine, Silenced Pistol, CCW; Forward Observer | — |
| 8 | 27 | 0 | Ohotnik, D-Charges, PARA Mine, Silenced Pistol, CCW; Lieutenant | — |

### Carmen Johns & Bâtard

**ID 1153 · AVA 1 · WB** — Carmen: `MOV 20-10 | CC 22 | BS 11 | PH 13 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 4`. Motorcycle, CC Attack (-6), Booty, Limited Cover, Courage, Dodge (+5), Natural Born Warrior, Impetuous, Mimetism (-3), Dogged. Bâtard: `MOV 15-15 | CC 22 | BS 0 | PH 15 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 5`, Peripheral (Synchronized), Mimetism (-3), Sensor, Dogged.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4264 | 17 | 0 | Carmen with Chain Rifle, Smoke Grenades, Smoke Grenade Launcher, AP Heavy Pistol, DA CCW; includes Bâtard; Irregular + Impetuous | — |

### Beasthunters Free Guild

**ID 1570 · AVA 1 · SK** — `MOV 10-10 | CC 21 | BS 11 | PH 13 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. Mimetism (-3), Stealth, Super-Jump, Terrain (Total), Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 9 | 0 | **BEASTHUNTER FTO**; Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CCW | Line Kazaks max 1 |
| 2 | 15 | 0 | Heavy Flamethrower, Tactical Bow, AP Mine, Pistol, DA CCW; Camouflage, Surprise Attack (-3), Forward Deployment (+20) | — |
| 3 | 15 | 0 | Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CCW; same camouflage package | — |
| 7 | 17 | 0 | Heavy Flamethrower, Panzerfaust, AP Mine, Heavy Pistol, DA CCW; same camouflage package | — |

All Beasthunter profiles are Irregular.

### Dynamo Regiment of Kazak Light Cavalry

**ID 1134 · AVA 5 · LI** — `MOV 20-10 | CC 15 | BS 12 | PH 12 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 4`. Motorcycle, Mine Dispenser (Shock), Dodge (+2.5), Dogged, Courage, Impetuous, Mimetism (-3), Limited Cover.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4179 | 14 | 0 | SMG, Panzerfaust, Smoke Grenade Launcher, Boarding Pistol, CCW | Mobility required-choice, max 2 |
| 4180 | 25 | 1 | AP Spitfire, Smoke Grenade Launcher, Boarding Pistol, CCW | same |
| 4182 | 16 | 0.5 | Boarding Shotgun, Smoke Grenade Launcher, Boarding Pistol, CCW; MediKit, Paramedic | same |

All Dynamo profiles are Regular + Impetuous.

### Konduktors, Transtartaric Railway Troops

**ID 1844 · AVA 2 · LI** — `MOV 10-10 | CC 15 | BS 10 | PH 11 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | **KONDUKTOR FTO**; Chain Rifle, Light Shotgun, Shock Mine, Pistol, CCW | Line Kazaks max 2 |
| 2 | 16 | 0 | **KONDUKTOR FTO**; Shock Marksman Rifle, Pistol, CCW; BS=12 | Line Kazaks max 2 |
| 3 | 12 | 0 | Rifle, Chain-colt, Flammenspeer, Pistol, CCW; Camouflage (1 Use), Infiltration | — |
| 4 | 10 | 0 | **KONDUKTOR FTO**; Rifle, Pistol, CCW; MediKit, Paramedic | Line Kazaks max 2 |

### Barsuk, Territorial Defense Regiment

**ID 1845 · AVA 3 · MI** — `MOV 10-5 | CC 15 | BS 11 | PH 11 | WIP 12 | ARM 3 | BTS 0 | W 1 | S 2`. Immunity (Shock).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 10 | 0 | **BARSUK FTO**; Heavy Flamethrower, Light Shotgun, Pistol, CCW | Wildcard; counts as Line Kazaks / Gunnery |
| 2 | 19 | 0 | **BARSUK FTO**; AP Marksman Rifle, Pistol, CCW; BS Attack (Shock) | same |
| 3 | 12 | 0 | Heavy Flamethrower, Light Shotgun, Pistol, CCW; Forward Deployment (+20) | — |
| 4 | 11 | 0 | Heavy Flamethrower, Light Shotgun, Pistol, CCW; Camouflage (1 Use), Decoy | — |
| 5 | 19 | 0 | AP Marksman Rifle, Pistol, CCW; Camouflage (1 Use), Decoy | — |
| 6 | 12 | 0 | Thunderbolt, Pistol, CCW; Camouflage (1 Use), Decoy | — |

### Streloks, Kazak Reconnaissance Unit

**ID 1126 · AVA 4 · LI** — `MOV 10-10 | CC 16 | BS 11 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Camouflage, Surprise Attack (-3), Forward Deployment (+20), Mimetism (-3), Decoy (1), Stealth.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 24 | 0 | T2 Marksman Rifle, AP Mine, Pistol, CCW; BS=12 | — |
| 3 | 16 | 0 | SMG, Chain-colt, AP Mine, Pistol, CCW | — |
| 5 | 26 | 0 | **STRELOK K-9**; SMG, Chain-colt, AP Mine, Pistol, CCW; Specialist Operative; includes K-9 Antipode | — |
| 6 | 17 | 0.5 | Boarding Shotgun, AP Mine, Pistol, CCW; Minelayer | — |
| 7 | 17 | 0 | Boarding Shotgun, Flash Pulse, AP Mine, Pistol, CCW; Forward Observer | — |

The K-9 Antipode is an included Peripheral (Synchronized): `MOV 15-15 | CC 20 | BS 10 | PH 15 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 5`, with Camouflage, Surprise Attack (-3), Forward Deployment (+20), Dodge (+5), Mimetism (-3), Sensor, Stealth, Climbing Plus.

### Irmandinhos

**ID 240 · AVA 4 · WB** — `MOV 10-10 | CC 21 | BS 10 | PH 14 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Booty, Engineer, Impetuous, No Cover; Deactivator.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 8 | 0 | Chain Rifle, D-Charges, Smoke Grenades, Pistol, AP CCW; Irregular + Impetuous | — |
| 3 | 14 | 0 | Boarding Shotgun, D-Charges, Smoke Grenades, Pistol, AP CCW; Irregular + Impetuous | — |

### Pavel Aleksei McMannus

**ID 1152 · AVA 1 · SK** — `MOV 10-10 | CC 23 | BS 12 | PH 12 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Martial Arts L3, Camouflage, Surprise Attack (-3), Courage, Forward Deployment (+20), Mimetism (-3), Terrain (Total), Specialist Operative, Stealth, Frenzy, Berserk, Immunity (Shock).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 0 | Ohotnik, D-Charges, Shock Mine, Boarding Pistol, AP+T2 CCW | — |

### Antipode Assault Pack

**ID 241 · AVA 2 · WB** — Handler: `MOV 10-10 | CC 14 | BS 11 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`, Tactical Awareness. Each pack includes **3 Antipodes**: `MOV 15-15 | CC 20 | BS 0 | PH 15 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 5`, with Camouflage, Surprise Attack (-3), Dodge (+5), Mimetism (-3), Sensor, Stealth, Super-Jump, Terrain (Jungle), No Cover and Peripheral (Control).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 0 | Handler: Rifle, Smoke Grenade Launcher, Pistol, CCW; includes 3 Antipodes with AP CCW; Regular + Tactical Awareness | — |

### Kuryer Unit

**ID 1524 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 9 | WIP 12 | ARM 2 | BTS 0 | W 1 | S 4`. Baggage, ECM: Guided (-6), Remote Presence, Courage, Minelayer, BS Attack (Guided), Warhorse.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 15 | 1 | Katyusha MRL, Chest Mine, Shock Mine, PARA CCW; BS Attack (-3) | Gunnery required-choice, max 2; counts as Gunnery |
| 2 | 18 | 1 | Uragan MRL, Chest Mine, Shock Mine, PARA CCW; Total Reaction | same |

### Vassily Plushenko

**ID 1150 · AVA 1 · MI** — `MOV 10-10 | CC 17 | BS 13 | PH 12 | WIP 14 | ARM 3 | BTS 0 | W 1 | S 2`. Camouflage, Surprise Attack (-3), Mimetism (-3), Stealth, Dogged, Courage, BS Attack (AP), Decoy (2).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 39 | 0 | T2 Marksman Rifle, Akrylat-Kanone, D-Charges, Heavy Pistol, CCW; Chain of Command | — |
| 2 | 39 | 1 | T2 Sniper Rifle, D-Charges, Heavy Pistol, CCW; Chain of Command | — |
| 3 | 35 | 0 | T2 Marksman Rifle, Akrylat-Kanone, D-Charges, Heavy Pistol, CCW; Lieutenant, Forward Observer | — |
| 4 | 35 | 1 | T2 Sniper Rifle, D-Charges, Heavy Pistol, CCW; Lieutenant, Forward Observer | — |

### Warcors, War Correspondents

**ID 50 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Journalist.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW; 360º Visor; Irregular | — |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW; Sixth Sense; Irregular | — |

### Ratnik

**ID 1127 · AVA 3 · HI** — Full armor: `MOV 10-10 | CC 16 | BS 13 | PH 11 | WIP 13 | ARM 6 | BTS 3 | W 2 | S 5`; Battle Ravaged: `MOV 10-5 | CC 14 | BS 13 | PH 10 | WIP 13 | ARM 4 | BTS 0 | W 2 | S 5`. Tactical Awareness, BS Attack (+1B), Courage, Dogged, Transmutation (1); Deactivator.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4140 | 46 | 1.5 | AP Spitfire, Panzerfaust, Flammenspeer, AP Heavy Pistol, Trench-Hammer, CCW; Regular + Tactical Awareness | Mobility required-choice, max 3 |
| 4141 | 41 | 1.5 | Heavy Rocket Launcher, Heavy Shotgun, AP Heavy Pistol, Trench-Hammer, CCW; Regular + Tactical Awareness | same |

### Line Kazaks

**ID 227 · AVA TOTAL · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 9 | 0 | Rifle, Pistol, CCW | Line Kazaks 1–5 |
| 2 | 20 | 1 | HMG, Pistol, CCW | same |
| 5 | 17 | 1.5 | Missile Launcher, Pistol, CCW | same |
| 6 | 10 | 0 | Rifle, Flash Pulse, Pistol, CCW; Forward Observer | same |
| 7 | 11 | 0 | Rifle, Pistol, CCW; MediKit, Paramedic | same |
| 8 | 9 | 0 | Rifle, Pistol, CCW; Lieutenant | same |
| 10 | 11 | 0 | Rifle, Pistol, CCW; Commlink (+2), Specialist Operative | same |

### Traktor Mul

**ID 257 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 10 | PH 9 | WIP 12 | ARM 2 | BTS 0 | W 1 | S 4`. Baggage, ECM: Guided (-6), Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 5 | 0 | PARA CCW; Deactivator | Gunnery required-choice, max 2; counts as Gunnery |
| 2 | 9 | 1 | Katyusha MRL, PARA CCW; BS Attack (Guided) | same |
| 3 | 14 | 1 | Uragan MRL, PARA CCW; BS Attack (Guided), Total Reaction | same |

### Kazak Doktor

**ID 243 · AVA 3 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Doctor, MediKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 12 | 0 | Rifle, Pistol, CCW | Line Kazaks max 2; counts as Line Kazak |

### Dozers, Field Engineers

**ID 256 · AVA 2 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Courage, Engineer, Deactivator, GizmoKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 13 | 0 | Rifle, D-Charges, Pistol, CCW | Line Kazaks max 1; Gunnery max 1 |
| 3 | 14 | 0 | Rifle, Blitzen, D-Charges, Pistol, CCW | same |
| 4 | 14 | 0 | Rifle, D-Charges, Pistol, CCW; Deployable Cover | same |
| 5 | 15 | 0 | Rifle, D-Charges, Armed Turret (Rifle), Pistol, CCW | same |

Counts as Line Kazak in the Line Kazaks chart and Gunnery in the Gunnery chart.

### Veteran Kazaks

**ID 234 · AVA 5 · HI** — `MOV 15-5 | CC 17 | BS 13 | PH 12 | WIP 14 | ARM 4 | BTS 3 | W 1 | S 2`. Courage, Immunity (Shock), Mimetism (-3), Sixth Sense, No Wound Incapacitation, Warhorse, Combat Instinct, Dodge (+1SD), Immunity (IMM-B), MediKit (PH=15), Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 45 | 1.5 | AP HMG, Heavy Pistol, CCW | Line Kazaks max 2; Veterans required-choice, max 5 |
| 4 | 38 | 0 | T2 Rifle, Light Flamethrower, Heavy Pistol, CCW; MediKit, X-Visor, Paramedic | same |
| 5 | 36 | 0 | T2 Rifle, Light Flamethrower, Flash Pulse, Heavy Pistol, CCW; X-Visor, Forward Observer | same |
| 6 | 36 | 0 | T2 Rifle, Light Flamethrower, Flash Pulse, Heavy Pistol, CCW; X-Visor, Lieutenant, Forward Observer | same |
| 7 | 45 | 1 | AP HMG, Heavy Pistol, CCW; Lieutenant | same |

Counts as Veteran in the Veterans chart.

### Remontnikbot V-5 Elektronik

**ID 1581 · AVA 1 · REM** — `MOV 10-10 | CC 10 | BS 8 | PH 9 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 1`. Courage, Mimetism (-3), Peripheral (Servant).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 2 | 0 | PARA CCW; no Order; attached support Peripheral | — |

### Ioann Bann, Varangian Dog-Warrior

**ID 1940 · AVA 1 · WB** — Dogface: `MOV 15-10 | CC 22 | BS 11 | PH 14 | WIP 13 | ARM 2 | BTS 3 | W 3 | S 2`; Dog-Warrior form: `MOV 15-10 | CC 23 | BS 11 | PH 16 | WIP 13 | ARM 4 | BTS 6 | W 3 | S 6`. Martial Arts L3, BS Attack (-3), Berserk, Dodge (+5), Immunity (ARM), No Cover, Super-Jump, Transmutation (1), Religious Troop, Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 32 | 0 | Chain Rifle, Viral Tactical Bow, Smoke Grenades, AP Heavy Pistol, AP+T2 CCW; Irregular | Mobility max 1 |

## Canonical Fireteam chart

Fireteam limits in the pinned TAK source: **Core 1; Haris 1; Duo unlimited** (`DUO: 256` sentinel).

### Line Kazaks Fireteams

**Types:** Core, Haris

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| LINE KAZAK | 1 | 5 | no | — |
| KAZAK DOKTOR | 0 | 2 | no | Line Kazak |
| VETERAN KAZAK | 0 | 2 | no | — |
| KONDUKTOR FTO | 0 | 2 | no | FTO profiles only |
| FRONTOVIK | 0 | 1 | no | Line Kazak |
| DOZER | 0 | 1 | no | Line Kazak |
| BEASTHUNTER FTO | 0 | 1 | no | FTO profile only |
| INTEL | 0 | 1 | no | Spec-Ops mode only |

### Veterans Fireteams

**Types:** Core, Haris, Duo

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| VETERAN KAZAK | 0 | 5 | yes | Veteran |
| FRONTOVIK | 0 | 5 | yes | Veteran |
| 112 FTO | 0 | 2 | no | — |

The two `required-choice` rows form the Veterans required-choice set; they are not interpreted as requiring both troop types simultaneously.

### Mobility Fireteams

**Types:** Haris, Duo

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| DYNAMO | 0 | 2 | yes | — |
| RATNIK | 0 | 3 | yes | — |
| FRONTOVIK | 0 | 2 | no | Ratnik |
| 112 MOTORIZED | 0 | 1 | no | — |
| IOANN BANN | 0 | 1 | no | — |

The Dynamo and Ratnik rows form the Mobility required-choice set.

### Gunnery Fireteams

**Types:** Haris, Duo

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| TRAKTOR MUL | 0 | 2 | yes | Gunnery |
| TM KURYER | 0 | 2 | yes | Gunnery |
| VYSTREL | 0 | 2 | yes | Gunnery |
| DOZER | 0 | 1 | no | Gunnery |

The three artillery rows form the Gunnery required-choice set.

### Wildcards

| Entry | Max | Counts as / profile restriction |
|---|---:|---|
| BARSUK FTO | 3 | FTO profiles only; Line Kazaks, Gunnery |
| COLONEL VORONIN | 1 | Line Kazaks |

Wildcards use the global Wildcard row of the TAK chart and may join otherwise eligible TAK Fireteams, subject to the chart and profile restrictions above.

## Reverse Fireteam access index

| Unit / profile | Fireteam access | Counts as / restriction |
|---|---|---|
| 112 FTO | Veterans | Max 2 |
| 112 Motorized | Mobility | Max 1 |
| Barsuk FTO | Wildcard | FTO profiles only; Line Kazaks / Gunnery |
| Beasthunter FTO | Line Kazaks | FTO profile only; max 1 |
| Colonel Voronin | Wildcard | Line Kazaks |
| Dozer | Line Kazaks; Gunnery | Max 1 in either; counts as Line Kazak / Gunnery by chart |
| Dynamo | Mobility | Required-choice; max 2 |
| Frontovik | Line Kazaks; Veterans; Mobility | Max 1 / 5 / 2; counts as Line Kazak / Veteran / Ratnik by chart |
| Intel Spec-Ops | Line Kazaks | Optional Spec-Ops mode only; max 1 |
| Ioann Bann | Mobility | Max 1 |
| Kazak Doktor | Line Kazaks | Max 2; counts as Line Kazak |
| Konduktor FTO | Line Kazaks | FTO profiles only; max 2 |
| Kuryer | Gunnery | Required-choice; max 2; Gunnery |
| Line Kazak | Line Kazaks | Native 1–5 row |
| Ratnik | Mobility | Required-choice; max 3 |
| Traktor Mul | Gunnery | Required-choice; max 2; Gunnery |
| Veteran Kazak | Line Kazaks; Veterans | Max 2 / required-choice max 5; Veteran in Veterans chart |
| Vystrel | Gunnery | Required-choice; max 2; Gunnery |

All standard roster units not listed in this reverse index have no Fireteam access in the pinned standard TAK chart.

## Reinforcement Fireteams — L'Équipe Argent

Linked Reinforcement army: **L'Équipe Argent (Army ID 399)**, source revision `7.26246.158`.

These rows are intentionally separate from the standard TAK chart. Reinforcement Fireteam limits in the pinned source are **Core 1; Haris 1; Duo 1**.

### Loup-Garou Reinforcement Fireteams

**Types:** Core, Haris, Duo

| Entry | Min | Max | Counts as / note |
|---|---:|---:|---|
| LOUP-GAROU REINF | 1 | 5 | — |

### Briscards Reinforcement Fireteams

**Types:** Core, Haris, Duo

| Entry | Min | Max | Counts as / note |
|---|---:|---:|---|
| BRISCARD REINF | 1 | 4 | — |

### Reinforcement Wildcards

| Entry | Max | Counts as / profile restriction |
|---|---:|---|
| MOBLOT REINF | 2 | — |
| APACHE REINF. | 2 | Loup-Garou |
| 112 FTO REINF | 1 | — |
| BRIGADIER BRUANT REINF | 1 | Briscards |
| WOLFGANG AMADEUS REINF | 1 | Loup-Garou, Briscards |

Reinforcement Wildcards may join otherwise eligible L'Équipe Argent Reinforcement Fireteams, subject to the Reinforcement chart above.

## Validation notes

- Standard roster count reconciled to **30** ordinary TAK entries after excluding `Intel Spec-Ops`, `Ariadna Team-Ops`, and generic `merc-*` catalog entries with an empty faction list.
- Every standard `fireteamChart` row from Army revision `7.26246.158` is represented, including profile-sensitive FTO joins and all three required-choice sets.
- Fireteam limits are preserved exactly: Core 1, Haris 1, Duo unlimited in TAK.
- The linked Reinforcement army resolves to **L'Équipe Argent (399)** and its three chart groups are preserved separately.
- Main and Reinforcement Wildcards are not merged.
- Package troops (Carmen & Bâtard, Strelok K-9, Antipode Assault Pack) preserve their included Peripheral relationships.
- Source data and Fireteam normalization were rechecked on **2026-10-15** against the pinned Army snapshot and InfinityDB commit listed in the front matter.

## Strategy and listbuilding research

Research synthesis updated **2026-10-16**. This section is strategic guidance rather than rules data; when older commentary conflicts with the canonical N5.3 roster or Fireteam chart above, the pinned Army data wins.

### Source handling

The research pass compared current and recent TAK discussion across long-form video/podcast material, transcript-derived community discussion, faction articles, and player list examples. Direct YouTube caption retrieval was not available for every video, so presenter-specific claims below are only attributed where the surrounding source material exposed enough detail to support them. Video titles alone are not treated as evidence.

The strongest cross-source agreement is that modern TAK is **not simply Camo spam**. It combines a stable defensive backbone with asymmetric midfield pieces and a small number of efficient active attackers. The normal plan is to force the opponent to spend Orders clearing mediocre-looking problems, reveal information and commit an important attacker, then counterattack with a hidden or protected gun.

### Recurring list structure

| Job | Common TAK solutions | What the slot is doing |
|---|---|---|
| Defensive anchor | Vystrel, Kuryer/Traktor, Frontovik, Gunnery Fireteam | Taxes movement and forces the opponent to commit resources before reaching valuable pieces |
| Midfield control | Scout, Strelok, Beasthunter, Barsuk, Konduktor | Camo/Decoy/mine ambiguity, objective presence, short-range punishers |
| Primary active gun | TankHunter AP HMG or Autocannon, Spetsnaz HMG, Veteran Kazak AP HMG, deliberate Ratnik build | Removes the hard target after the defensive shell has exposed it |
| Pressure/trading | Dog-Warrior, Antipode Assault Pack, Carmen & Bâtard, Dynamo, Irmandinho | Smoke, templates, Sensor, mine triggering, fast approach and disposable pressure |
| Command | Voronin, Veteran Kazak LT, TankHunter LT, Vassily, Scout/Line Kazak niche LTs | Determines whether the LT is an economy piece, durable active piece or hidden shell |
| Succession | TankHunter CoC Minelayer; Vassily CoC | Lets an exposed LT play aggressively without buying a completely passive insurance model |
| Support | Dozer, Kazak Doktor, 112, Remontnikbot | Keeps REM/HI packages functional and supplies mission specialists |
| Cheap Fireteam glue | Line Kazak, Barsuk FTO, Konduktor FTO, Beasthunter FTO | Keeps the link inexpensive while adding templates, mines or specialist coverage |

A useful default is **many annoying problems, few premium killers**. TAK does not need every marker to be dangerous enough to kill a heavy infantry model; it needs the opponent to be unsure which markers, mines, templates and AROs deserve Orders now.

### Go-to units

#### Scouts

Scouts are one of the most consistently useful current TAK pieces because they combine true Camouflage, Infiltration, Mimetism, AP shooting and useful mine packages.

- **Minelayer (2), Ohotnik + E/M Mine (28/0.5):** premium board-control profile. Two deployables plus a real Camo gun make a lane or objective cluster expensive to approach.
- **Forward Observer (28):** strong objective specialist that is still a credible shooter.
- **T2 Boarding Shotgun (23):** cheap close-midfield attack profile.
- **Lieutenant (27):** viable hidden-command option when the list wants an LT inside the marker shell, but it spends a high-quality Scout slot on command duty.

Do not judge Scouts only by how many enemy models they personally kill. A Scout that forces Discover, Dodge, mine-clearing and rerouting has already generated value.

#### Streloks

Streloks are the cheaper complementary marker family and are excellent at attacking the **easy target that matters** rather than the opponent's best gun.

- **SMG + Chain-colt (16):** extremely efficient marker/order-tax piece.
- **Minelayer Boarding Shotgun (17/0.5):** cheap additional mine plus a dangerous close-range reveal.
- **Forward Observer (17):** inexpensive specialist in the midfield shell.
- **T2 Marksman Rifle (24):** the version to choose when the marker is expected to make real gunfights.
- **K-9 Specialist (26):** combines a scoring controller with a synchronized Antipode carrying Sensor, Climbing Plus and PH15. Particularly useful when opposing Camo is likely to matter.

The K-9 profile is effectively a specialist plus a dedicated marker-hunting/mobility tool in one slot.

#### TankHunters

TankHunters are one of the strongest recurring TAK recommendations because multiple profiles solve structural list problems.

- **AP HMG (33/1.5):** premier protected active-turn gun. Keep it unrevealed until there is a target worth spending the marker on.
- **Portable Autocannon (36/1.5):** more specialized hard-target ambush with excellent threat value.
- **Missile Launcher (28/1.5):** hidden long-range reactive threat when that is what the table requires.
- **CoC + Minelayer (25):** one of the cleanest succession packages in the faction: Chain of Command, Camo, AP mine and Panzerfaust are all useful even if succession never happens.
- **FD+20 Minelayer (24/0.5):** pushes the mine/marker shell forward without spending Scout points.
- **LT Minelayer (25):** a workable hidden-LT architecture.

The important listbuilding point is that **TAK's CoC tax is unusually productive**. TankHunter CoC is not just a model hiding in the DZ waiting for the LT to die.

#### Vystrel and Gunnery pieces

The post-update defensive shell is one of the most distinctive current TAK tools.

- **Vystrel AP Sniper (23/0.5):** cheap Sapper long-range piece when active Burst matters more than Neurocinetics.
- **Vystrel Neurocinetics AP Sniper (26/0.5):** efficient reactive lane holder.
- **Vystrel Neurocinetics Portable Autocannon (32/1.5):** heavier anti-armor ARO anchor.
- **Kuryer Uragan (18/1):** Total Reaction plus Minelayer and chest/shock mines; useful defensive clutter rather than only an artillery gun.
- **Traktor Mul (5):** very cheap Regular Order plus Baggage/REM utility when the list has room for the S4 base.

The best use is usually **layered defence**, not exposing every expensive gun simultaneously. One visible long-range problem plus hidden markers, mines and short-range templates often costs more Orders than two or three obvious ARO guns that can all be solved by the same attacker.

A practical constraint is physical: S4/S5 bases need hiding places. Heavy artillery saturation can become a deployment problem on dense tournament tables.

#### Veteran Kazaks

Veteran Kazaks are the dependable premium all-rounder rather than mandatory spam.

- **FO (36):** durable WIP14 specialist with X-Visor, T2 rifle, LFT, Mimetism, NWI and strong immunities.
- **LT FO (36):** one of the best generalist command profiles because the LT can actually score and fight.
- **AP HMG (45/1.5):** expensive but reliable active gun.
- **LT AP HMG (45/1):** aggressive command/gun profile; pair with succession insurance if it is expected to fight early.

One Veteran Kazak is easy to justify. Multiple Veterans are a deliberate investment rather than an automatic sectorial requirement.

#### Spetsnaz

The **Camo/Decoy HMG (36/1.5)** remains an excellent independent active attacker: Marksmanship, Mimetism, Surprise Attack and a protected starting state let it attack after the opponent has committed.

The **Parachutist shotgun/AP SMG profiles (27)** provide a different axis: they punish weak backfield troops and order pools without needing to fight the opponent's front-line ARO architecture.

### Fireteam patterns

TAK Fireteams are generally best treated as **supporting architecture**, not as the entire army.

#### Gunnery Haris/Duo

The distinctly current TAK defensive team. Build it to create a lane problem and support network, not to consume half the list in artillery.

Typical logic:

- one Vystrel/Kuryer/Traktor required-choice piece;
- optionally a Dozer for repair, Deactivator/GizmoKit and mission work;
- Barsuk FTO can join as a cheap Wildcard and adds a Heavy Flamethrower/Light Shotgun body.

This team is especially valuable when the rest of the list contains Camo/mines that punish the opponent for taking the alternate route around the gun.

#### Line Kazak Core/Haris

This is the flexible cheap shell.

Useful inserts include:

- up to two Veteran Kazaks;
- one Frontovik;
- Dozer;
- Kazak Doktor;
- Konduktor FTO;
- Beasthunter FTO;
- Barsuk FTO as Wildcard;
- Voronin as Wildcard/counts-as Line Kazak.

The usual strength is **cheap bodies around one or two models that actually need the team**, rather than paying for five premium shooters.

#### Veterans Core/Haris/Duo

Built from Veteran Kazaks and/or Frontoviks, with 112 FTO support. Use this when the list wants a tougher mobile gun/specialist block. It costs enough that the rest of the army should still retain marker and pressure elements; a full premium team plus too many other expensive pieces can erase TAK's asymmetric depth.

#### Mobility Haris/Duo

Current N5.3 Army data allows a Mobility team built around the required-choice set of **Dynamo and/or Ratnik**, with Frontovik, 112 Motorized and Ioann Bann support.

This is an important correction to older October-2025 commentary that said Ratnik Fireteams had been removed. That historical statement is superseded by the current pinned Army chart: **Ratnik is presently a Mobility required-choice and can be in a Mobility Haris or Duo**.

Dynamo is particularly useful here because the current profile has **Mine Dispenser (Shock)** in addition to high movement, Smoke Grenade Launcher, Mimetism and Dogged. Older commentary claiming current Dynamos lost Mine Dispenser is also stale relative to N5.3.

### Lieutenant and Chain-of-Command packages

#### Voronin LT + TankHunter CoC

A safe strategic command package.

Voronin currently brings **WIP14, Lieutenant (+1 Command Token), Counterintelligence, Sensor, Sixth Sense and Wildcard/counts-as Line Kazak**. Current N5.3 data does **not** list Strategos on Voronin; older advice describing him as a Strategos LT should not be carried forward.

The TankHunter CoC Minelayer adds succession while still contributing Camo, an AP mine and a Panzerfaust threat.

Use this package when the LT's job is command economy and support rather than primary attack.

#### Veteran Kazak LT FO + TankHunter CoC

Probably the cleanest aggressive-generalist command package.

The Vet LT can move, score and fight instead of hiding. If it dies, the TankHunter assumes command while having already contributed to the marker/mine shell.

#### Veteran Kazak AP HMG LT + TankHunter CoC

The deliberate combat-LT version. The LT profile saves SWC versus the standard AP HMG and can be the primary gun, but succession insurance becomes more important because the LT is expected to expose itself.

#### Vassily LT / Vassily CoC

Viable but expensive.

The LT/FO version gives Camo, Decoy (2), WIP14 and a T2 gun for 35 points. The CoC versions are 39 points and compete directly with the much cheaper TankHunter CoC Minelayer.

Take Vassily when the list intends to exploit **his whole package**. If the only requirement is succession insurance, TankHunter CoC is usually much easier to fit.

#### Other LTs

- **TankHunter LT Minelayer:** strong shell-game command option.
- **Scout LT:** hidden in the midfield marker game, but consumes a premium infiltrating slot.
- **Line Kazak LT:** cheapest straightforward option when the command model is meant to stay irrelevant.
- **Frontovik LT:** available when the team architecture naturally wants it, but usually less structurally distinctive than the options above.

### Specific combos and sequencing

#### 1. Defensive shell -> enemy commitment -> hidden attacker

A common TAK sequence is:

1. Vystrel/Frontovik/Gunnery piece controls an obvious lane.
2. Scouts, Streloks, Barsuks, Konduktors and mines make alternate routes inefficient.
3. The opponent spends Orders Discovering, Dodging, clearing deployables or moving the real attacker into position.
4. Once that attacker is exposed or isolated, reveal the TankHunter/Spetsnaz or move a Veteran Kazak to remove it.

This is more efficient than revealing the premium Camo gun for a marginal reactive shot on Turn 1.

#### 2. Preserve markers when the ARO is bad

A Camo marker that does not reveal still forces decisions: Discover, Dodge, ignore, reroute, or risk a mine/template. A low-odds rifle ARO that reveals and dies can be much less valuable than retaining uncertainty for another Order.

The reactive question is often **"does revealing now cost the opponent more future Orders than staying a marker?"**

#### 3. Pressure piece first, scoring piece second

Dog-Warriors, Antipodes, Carmen, Dynamos and Irmandinhos can probe dangerous areas before the expensive specialist moves in.

Use them to:

- trigger or locate mines;
- force template/Dodge decisions;
- throw Smoke;
- expose Camo or hidden AROs;
- clear a corner or short-range defender;
- create a safe path for the Scout/Strelok/Veteran that must actually score.

Antipodes are particularly relevant because the pack brings Sensor, speed, Super-Jump and Tactical Awareness. Their value is not limited to CC kills.

#### 4. Dozer + Gunnery package

If the list buys Vystrel/Kuryer/Traktor pieces, a Dozer becomes much more attractive because the Engineer can repair Remote Presence models while also scoring and contributing another tactical tool.

Profile choice changes the defensive texture:

- **Blitzen:** another state/control threat;
- **Deployable Cover:** table-geometry support for valuable pieces;
- **Armed Turret:** additional cheap reactive friction.

#### 5. Strelok K-9 specialist package

The controller handles objectives while the synchronized Antipode provides Sensor, Climbing Plus and PH15 mobility. It is especially useful when the list otherwise lacks an easy way to challenge enemy markers around an objective.

#### 6. Dynamo development package

A Dynamo can spend its speed and Impetuous movement to develop while retaining its Regular Order for later use. Smoke creates safe crossings, while **Mine Dispenser (Shock)** lets the model leave area-control pieces after advancing. The 16-point Paramedic is a particularly fast mission piece; the 25-point AP Spitfire is the profile to consider when the Mobility team needs a gun rather than just development/scoring.

### Lesser-used or underrated tools

#### Konduktor infiltrator — 12 points

Camo (1 Use), Infiltration, Chain-colt and Flammenspeer make this an unusually cheap ambiguous marker. It is not supposed to beat elite troops in repeated gunfights; it is supposed to create a bad short-range decision for a tiny investment.

#### Barsuk Camo/Decoy profiles

The **11-point HFT/shotgun** and **12-point Thunderbolt** profiles are useful because they look like cheap clutter until their specific range/template matters. The **10-point FTO** is also excellent inexpensive Fireteam glue with a Heavy Flamethrower.

#### Antipode Assault Pack

Community discussion pushed back on analyses that omitted Antipodes. Their combination of Tactical Awareness, multiple fast bodies, Sensor, Camo and AP CC creates pressure and objective disruption that raw gun comparisons undervalue.

#### Irmandinho — 8 points

Engineer, Smoke, PH14, AP CCW and D-Charges for very few points. The Irregular/Impetuous order structure means the model should be deployed where its own Order and Impetuous movement are likely to be useful rather than treated as generic pool filler.

#### Traktor Mul — 5 points

A very cheap Regular Order with Baggage and REM utility. Its S4 footprint and the Gunnery opportunity cost are the real constraints, not the profile's price.

#### Dynamo Paramedic — 16 points

A fast specialist with Smoke, Mimetism, Dogged and Mine Dispenser. It can solve mission geometry that a slow Kazak specialist cannot.

### Disputed or build-around choices

| Topic | View A | View B | Practical conclusion |
|---|---|---|---|
| Kuryer/Katyusha | Some TAK analysis is enthusiastic about the artillery package | Other players criticize repeated low-odds raw Speculative Fire | Kuryer can be good for Minelayer/Gunnery/board-control value; do not make unassisted Spec Fire the only attack plan |
| Vassily | Expensive versus cheaper Camo/CoC tools | Experienced players still publish Vassily-centered balanced lists | Viable toolbox, not default tax |
| Antipodes | Sometimes omitted from abbreviated faction reviews | Players argue strongly for their pressure, Sensor and objective value | Treat as a real archetype choice, not a fringe gimmick |
| Ratnik | Expensive S5 build-around | Current N5.3 gives Tactical Awareness, +1B and Mobility FT access | Legitimate Mobility archetype, but not a universal staple |
| Pavel | Strong-looking premium midfield fighter | WIP12 explicitly framed Pavel as "what's not" while other analysis is more positive | The clearest premium profile to scrutinize for opportunity cost |
| Heavy artillery saturation | TAK can stack very efficient S4 defensive pieces | Large-base congestion and shared attack vectors can make them easy to solve | Usually buy enough defence to create layers, not every efficient artillery profile |
| Big Core | Full Kazak/Veteran teams offer stable guns and specialists | TAK's marker pieces are too valuable to squeeze out | Fireteam as backbone is more common than Fireteam as entire game plan |

### Example list archetypes seen in current discussion

WIP12's April-2026 TAK episode published multiple Army codes with list names that illustrate the range of viable construction:

- **"My main list"** — general balanced TAK.
- **"Just two Guys and their tractors"** — artillery/REM-heavy defensive architecture.
- **"Nice mix of things (Vassily)"** — Vassily inside a mixed combined-arms list.
- **"Cavalry Artillery Infantry"** and **V2** — fast pressure plus static guns plus infantry/midfield.
- **"Sensible ratnik list"** and a Ratnik-oriented list — deliberate Ratnik build-around.

The lesson is not that one of these is the canonical TAK list. The recurring skeleton is role-based: **defence + markers + one or two real attackers + pressure + mission coverage**.

### Practical build checklist

For a generic 300-point TAK list, check for the following before optimizing individual profiles:

1. **Command plan:** who is the LT, and does that LT need CoC?
2. **One credible long-range defensive problem:** Vystrel/Gunnery/Frontovik or another deliberate ARO architecture.
3. **Two to four meaningful midfield problems:** Scouts, Streloks, mines, Barsuks, Konduktor, Beasthunter.
4. **At least one protected active gun:** TankHunter, Spetsnaz, Veteran Kazak or a deliberate Ratnik package.
5. **A pressure/trading piece:** Dog-Warrior, Antipodes, Carmen, Dynamo, Irmandinho or Ioann depending on the mission.
6. **Mission specialists that can survive to Turn 2/3:** do not spend every specialist as an early attacker.
7. **Recovery if the expensive package justifies it:** Dozer/Doctor/112 rather than support by habit.
8. **Range diversity:** do not make every important attack depend on one long-range gun or one close-range marker.
9. **Deployment footprint:** count S4/S5 bases and verify the table can hide them.
10. **Turn sequence:** know which cheap piece probes first and which premium piece is being preserved for the decisive attack.

A strong TAK list should usually be able to answer: **what does the opponent have to spend Orders on before they are allowed to attack the model I actually care about?**

### Research sources

- Robert Shepherd, *Infinity N5 Faction Focus: Tartary Army Corps*: https://www.youtube.com/watch?v=eM5cM_Y18vk
- Robert Shepherd written/supporting faction-focus page: https://buymeacoffee.com/robertshepherd/infinity-n5-faction-focus-tartary-army-corps
- WIP12, Episode 203, *Tartary Army Corps with Copper* (April 2026), including example Army codes/list names: https://podfollow.com/wip12-an-infinity-the-game-podcast/episode/61410473e1a9722845a54faaec5feb1e12bcd8b7/view
- O-12 Podcast, *Tartary Army Corps – Kontrolle durch Ungewissheit* (January 2026): https://o12podcast.substack.com/p/tartary-army-corps-kontrolle-durch
- Bureau Aegis TAK discussion following the faction-focus material, including Kuryer, Antipode, Vassily and artillery pushback: https://www.bureau-aegis.org/forum/index.php?topic=17695.60
- Bureau Aegis early-N5 TAK strategy discussion, including marker preservation, Strelok/Scout/TankHunter usage and defensive order-tax concepts: https://www.bureau-aegis.org/forum/index.php?topic=17729.0
- Swiss Miss Gaming, current-N5 TAK tier-list video: https://www.youtube.com/watch?v=YTVcl3haxdg
- DefectiveDice, *Getting Started with TAK*: https://www.youtube.com/watch?v=C8BmvBmu66M

Where these sources discuss older Army versions, profile legality and current equipment are reconciled to the canonical N5.3 data in this file. In particular, current data confirms **Dynamo Mine Dispenser (Shock)**, **Ratnik Mobility Fireteam access**, and a **Voronin profile without Strategos**.

### Transcript-verified review and REM/Mobility deep dive — 2026-10-19

**Read first:** These are *opinions and play patterns*, not changes to the pinned N5.3 unit data above. Sources are full MCP transcripts of three videos and three podcast episodes. Tactical Awareness is **February 2025, before the October roster overhaul**, so its *unit evaluations* are historical, not authoritative for present prices/skills.

#### The clearest cross-source conclusions

- **Plan from a defensive base, then counterattack.** Robert Shepherd and MetaChemistry describe TAK's current strength as Sapper/Neurocinetics REMs + mines/Decoys that consume enemy Orders before TankHunters, Scouts or a mobile piece act. The “why” is information and Order denial, **not** that every TAK gun wins straight-up fights.
- **A bad matchup is high-Mimetism shooting backed by Sensor/MSV.** WIP12 and MetaChemistry stress that a Vystrel can be fearsome against ordinary gunfighters yet fold quickly when an Mimetism (-6) attacker forces poor BS numbers. Retain markers, use short-range templates/Beasthunters, smoke to *avoid* the lane, and play the mission rather than insisting on a sniper duel. A Frontovik MSV1 shooter is a limited active-turn answer, **not** a durable universal ARO solution.
- **Avoid overbuying “efficient” S4 models.** Vystrel, Traktor/Kuryer, Voronin and Dynamo compete for *physical deployment space*, even when the points fit. Their separate tactical jobs can justify several, but plan hiding positions before selecting all of them.
- **TAK's marker shell has a known counter:** MetaChemistry advises opponents to Sensor the important area or *ignore* low-priority markers and complete objectives; wasting an entire pool Discovering Decoys is exactly the TAK player's desired outcome. As TAK, position real mines and important guns where simply ignoring them has consequences.

#### Actual Vehicle / TAG / REM coverage

**No dedicated Vehicle or TAG is listed in the pinned standard TAK roster.** Do not describe Ratnik as a TAG (it is S5 **HI** with Transmutation, Dogged, +1B and Tactical Awareness); Dynamo is S4 motorcycle **LI**. The relevant machines are **Vystrel, Kuryer, Traktor Mul** (all REMs) and **Remontnikbot** (2-point Engineer Peripheral). Other Ariadna/Vanilla discussions are useful for shared REM and Dynamo concepts, **not** proof of TAK TAG/VH access.

| Unit/package | Use it because | Limit / alternative view |
|---|---|---|
| **Vystrel Neurocinetics AP sniper** + **5-point Traktor** Gunnery Duo | 2 STR, Sapper, AP/Shock and team Special Die make a difficult, inexpensive ranged ARO; cheap Baggage REM supplies the link die | MetaChemistry prefers the more frightening **portable autocannon** despite higher cost; WIP12 warns both struggle into Mimetism (-6) and may disappear to one favorable attack |
| **Kuryer Katyusha** (15 pts, 1 SWC) | Shepherd values a cheap Gunnery/minelayer/Baggage unit that can also spend spare Orders on **DA speculative fire** against the midfield without constructing an entire Targeted/Guided engine | Range, Order availability and dice variance matter. Do not expect blind Speculative Fire to replace a reliable main gun; some players dislike spending repeated Orders on low-odds shots |
| **Kuryer Uragan** / **Traktor Uragan** | Total Reaction/long-lane ARO plus artillery utility; Kuryer also contributes Minelayer clutter | Extra SWC and another S4 base; choose an actual firing lane and fallback repair path rather than stacking artillery automatically |
| **Dozer + repair servant** | Repairing damaged Remote Presence guns can force the opponent to clear the same obstacle again; Dozer also brings Engineer objectives | **Disagreement:** Swiss Miss rates Dozer poorly versus 5-point Traktor as Gunnery die-provider or Irmandinho/Frontovik Engineers. The Dozer earns its premium only when recovery and objective access are genuinely used |
| **Dynamo duo: SMG/Panzerfaust (14) + Paramedic (16)** | Cheap 2-model fast objective, smoke and Mine Dispenser package; regular Orders, Dogged and mobility make it a dangerous secondary attack lane | Shepherd strongly recommends this duo; WIP12 warns launched mines near friendly Camo can expose that Camo to enemy template solutions. High bike/S4 count also causes traffic jams |
| **Dynamo AP Spitfire (25)** | Swiss Miss likes an affordable, fast AP gun that can lead a mobile duo; useful when the list needs an aggressive attack piece | WIP12 questions the +9–11 point upgrade over a mine-dispensing utility Dynamo: TAK already has infiltrating shooters and S4 bikes are awkward to maneuver |
| **Ratnik AP Spitfire / HRL (41–46)** | Big gun, +1B, Tactical Awareness; can lead Mobility Haris/Duo with a Frontovik specialist/Engineer. Six active-turn dice from linked AP Spitfire is the attraction | **Strong disagreement:** Swiss Miss and some WIP12 lists favor Ratnik as real brute-force or Haris build-around; Shepherd sees it as a 40+-point vanity/mission-specific tool that competes with Vet Kazaks and often adds less than two cheap Dynamos. It is hackable and drops speed after Transmutation |

**Useful attack sequencing:** Dynamo uses speed to dispense a mine near a defended target → enemy must weigh Dodge against the mine → Kuryer Speculative Fire or a different attack punishes the decision. Shepherd argues this creates a more serious fork than simply firing the Kuryer repeatedly. Verify actual mine placement, Trigger Area and ARO legality on the table; the trick is situational.

#### Other genuine presenter disagreements

| Topic | Pro | Skeptical / why | Working choice |
|---|---|---|---|
| **Spetsnaz HMG spam** | **Tactical Awareness (pre-update):** multiple Marksmanship+Camo Spetsnaz backed by T2 Streloks overwhelm the opponent with independent offensive markers | **WIP12 and Swiss Miss (post-update):** expensive one-wound, non-AP HMG fights compete badly with TankHunter AP HMG, AP Ohotnik Scouts, Vet Kazak and Ratnik | **Parachutist BSG/AP SMG** retains a clearer niche: attack the opponent's rear/order pool along a different axis; main HMG is preference, not automatic |
| **Pavel** | **WIP12 dissenting player:** opponents assume a marker is a Scout, Strelok or mine; Pavel's Berserk/MA/AP T2 can surprise an expensive TAG or LT in CC | **Other WIP12 speakers:** one wound without Dogged/NWI makes this a fragile, costly suicide charge; his shooting/mission/CC flexibility is not necessarily enough | Off-meta ambush/trading pick against worthwhile targets, not baseline midfield specialist |
| **Vassily** | Decoy-rich Lt/CoC shell and potent T2 option; can obscure what the opponent should Discover | Higher points than TankHunter CoC and Scout alternatives; choose only if actively leveraging his gun, disguise and leadership package | Do not pay his premium for CoC alone |
| **WarDriver Disco Ball** | **WIP12/Shepherd:** Eclipse-like visibility denial can solve an MSV gun that normal smoke cannot, allowing mission play | **Swiss Miss:** paying SWC/points for a mediocre hacker brings TAK into a hacking contest it seldom wants | Tech counter for a specific visibility problem, not a standard hacking plan |
| **Dog-Warriors vs Camo-heavy package** | WIP12 advocates durable close pressure and templates to beat bad gunfights, especially high-Mimetism targets | Heavy pressure pieces may consume the Order pool and space that makes multiple Scouts/Streloks effective | Take pressure because it resolves a matchup or scenario route, not simply because dogs are iconic |

#### Sources reviewed at transcript level

1. **Robert Shepherd**, *Infinity N5 Faction Focus: Tartary Army Corps* (30 Oct 2025): https://www.youtube.com/watch?v=eM5cM_Y18vk — defensive triangle, Vystrel/Kuryer/Traktor and direct DA Speculative Fire (~26–32m), Dynamo (~33–39m), Ratnik skepticism (~39–41m).
2. **Swiss Miss Gaming**, *Infinity N5 Tier List: Tartary Army Corps* (4 Dec 2025): https://www.youtube.com/watch?v=YTVcl3haxdg — strong Dynamo/Ratnik opinion, Dozer and WarDriver skepticism, Spetsnaz comparison, REM discussion (~94–102m).
3. **DefectiveDice**, *How to get started with the Tartary Corps in Infinity!* (26 Dec 2025): https://www.youtube.com/watch?v=C8BmvBmu66M — beginner purchase/Action Pack approach; cheap regular Orders and proxying appropriate profiles; **not** treated as evidence of a new competitive consensus.
4. **WIP12 E203**, *Tartary Army Corps with Copper* (15 Apr 2026): https://open.spotify.com/episode/0fLvDDDa2baw7lxt3J4qo9 — actual competing list archetypes; Dynamos (~30–36m), Mimetism problems/Frontovik (~49–55m), Pavel debate (~64–68m), Ratnik (~89–98m).
5. **MetaChemistry E141**, *Faction Takedown – Tartary Army Corps* (4 May 2026): https://open.spotify.com/episode/5Jndc3fD91n84MZ9WZxM4l — deliberately adversarial analysis: Vystrel (~19–23m), Scouts (~30–33m), TankHunters/Spetsnaz (~39–44m), anti-Camo plans (~49–58m).
6. **Tactical Awareness S3 E09**, *ZEROES & HEROES – TAK* (3 Feb 2025): https://open.spotify.com/episode/2VCGfZZhXpth6ahryGhPyw — pre-October-2025 alternative emphasizing max Spetsnaz + T2 Strelok spam (~3–8m) and broad Camo deception. **Old roster details, including a Strategos claim for Voronin, conflict with the N5.3 snapshot above**.

**Confidence boundary:** Transcript claims about preference and practical play are attributed; weapon rules, costs and available Fireteams defer to this file's pinned 2026-09-03 Army snapshot. Full transcripts were read with the connected YouTube/podcast tools; the short clips above are navigation aids, not separate primary material.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Wardriver HD14/1** with Zero Pain is a low-points but relatively **high-SWC** anti-heavy controller/mission specialist. A responsive **KHD hunter** is not part of the usual native TAC network, so avoid trying to beat Interventors/Combined at their own repeater war. **Disagreement in existing TAC analysis:** WIP12/Shepherd value its Disco Baller and tech-side mission utility, while Swiss Miss warns the SWC can crowd strong attack guns. **Decision:** pay for Wardriver only when a TAG/HI-heavy opponent, relevant classified or a real vision-control route creates an Order-saving task that a cheaper Forward Observer cannot do.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

For cross-faction **apex** and **points-value** rankings, the Order types, situational counterexamples and transcript-backed disagreements, see [Cheerleaders and Order Generators — N5.3](../../notes/list-building/cheerleaders-and-order-generators.md). Roster profiles/AVA/Fireteam legality above take precedence.

- **Line Kazaks**: small-base Regular troop with a credible close guard/command-decoy role; check cheapest exact profile before upgrading

**List-building test:** count *transferable* Regular Orders by Combat Group after deployment; include required link members/command enablers, physical DZ footprint, and the unit's actual ARO/mission contribution. Do not treat Irregular, Tactical, Lieutenant or Peripheral activations as interchangeable generic Orders.


## ARO apex/value cross-reference (2026-10-23)

See [ARO units: N5.3 apex/value tiers, hidden-versus-visible and deployment/matchups](../../notes/list-building/aro-units-apex-and-value.md). The **current profile details here** control exact cost/SWC, Training and Fireteam eligibility; do not import another faction's link or specialist upgrades.

- **Tankhunter Camo ML/Panzerfaust/Autocannon** — hidden-information threat and serious anti-armor; Minelayer closes approach, 1W/expensive gun remains fragile
- **Traktor Mul support** — rare Ariadna cheap reload/guided/total-reaction choices; only buy a real Guided program if FO route is viable
- **3pt Warcor Flash** — Irregular very-cheap ARO tax, not a transferable pool Order

**Choose by circumstance:** a hard long gun matters only when the opponent must cross its arc; cheaper mines, Camo markers, templates, Flash, DTWs and hacking force movement or risk without committing an entire attack plan. Budget a second layer and preserved counterattack, check pie-slicing, hidden Order cost, anti-visual bypass and repair routes.

## N5.3 airborne / enemy-DZ profile and value choices (2026-10-23)

**Kazak Spetsnaz Parachutist BSG27/0 or AP SMG27/0** creates a reliable side-edge attack with Decoy(1), Mimetism(-3), Marksmanship and D-Charges: target support/Order generators from an unexpected range band rather than frontally challenging ARO. The **Camo HMG36/1.5 and AP sniper32/0.5** are different non-airborne profiles; no free merger of Camo+HMG and Parachutist. Unlike **Van Zant**, the Spetsnaz uses **ordinary Parachutist and cannot enter directly in enemy DZ**. Preserve a cheap forward specialist and exit Order for scoring.

[Cross-game N5.3 airborne/rear-strike apex-value and landing-risk tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **Use this roster and canonical Fireteam chart for exact legality.**

## Warbands and inexpensive trading roles — N5.3

**Irmandinho Engineer+Chain+Smoke8/0** is the premier utility trader: has a relevant objective/repair function even if no target gets within template range. **Dog-Warrior21/0** uses 15-10/Super-Jump/3W Transmutation/PH Grenade Speculative Fire for **multiple Orders of attack**, not pure sacrificial efficiency. **Carmen+Bâtard17/0** provides bike Smoke+Sensor synchronized counter to enemy Camo. **Ioann Bann32** gives another high-end large-base close-in threat; expensive compared with Irmandinho. Compare **Dynamo** mobility vs tech/midfield mission instead of stuffing every Irregular WB into a single Group 2.

[Cross-game warband/cheap-trader apex and value tiers, targets and command packages](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). Profile-specific sectorial legality/Fireteams above control all selections.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Irmandinho Engineer8** is exceptional cheap Smoke/trading plus occasional forward technical rescue, but usually **cannot safely replace Dozer13 + Remontnik2** staged for STR gun/vehicle recovery. **112 Doctor11**, **Motorized112 19** and **Kazak Doktor12** are cheap WIP13 VITA alternatives; motorized 20-10 MOV covers wider forward zones but risks open crossing. On No-Cube targets Doctor failure is a **35% chance to lose patient**, with no Cube token bailout. [Doctor/Engineer recovery odds and tier guide](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Dog-Warrior21** (15-10, Super-Jump, Berserk, Smoke, 3W in current roster) and **Ioann Bann** are the meaningful *multi-Order close assault* choices; **Irmandinho8** instead gives Smoke and an occasional AP-CC technical trade at minimal cost, but **Irregular/Impetuous** exposure is real. **Spetsnaz CC21/MA2** is still mainly a camouflaged *gunfighter*, not a 29pt Monofilament assassination piece; **TankHunter/Strelok** are ranged/Camo control, not high-CC. Counter incoming enemy CC with mine/camo screen, long-range guns, and templates rather than a Veteran Kazak CC17 duel. [Close-combat apex/value, positioning and counter-CC](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Beasthunter9/15 Panzerfaust/HFT** and **Dozer14 Blitzen** are low-cost deterrents; **Dynamo14 Panzerfaust+Smoke GL** may reach a side-angle with Impetuous/motorcycle risk. **TankHunter33 AP HMG** is repeatable B4 AP gun; **TankHunter36 Portable Autocannon** is AP+EXP B2 **without assuming Vanilla Ariadna's +1B**. **Scout E/M Minelayer28** traps short approach, **Veteran Kazak AP HMG45** adds high survivability. Prioritize contact safety over pure PS math. [Non-hacking armor-killer value rankings and tactical matchups](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## Tactical cross-reference — indirect fire (2026-10-23)

**Kuryer Katyusha15/1** is one of the game's apex **independent Speculative Fire** choices: +3 Range band to 24″, B1 Long Skill, Warhorse/Baggage/Minelayer/Guided. **Traktor Katyusha Guided9/1** wins cheapest conditional payoff if Chasseur/Strelok/Dynamo/other FO already creates Targeted. **Kuryer Uragan18/1** is the Total Reaction defensive variant; **don't** claim its benefits simultaneously with Katyusha. Shepherd favors several safe Kuryer speculative shots over expensive multi-Order Spotlight+Guided setup in many *midfield* situations; WIP12 likes Kuryer flexibility but six saved points on Traktor can fund actual objectives. [Indirect Fire apex/value and media disagreements](../../notes/list-building/indirect-fire-speculative-guided-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Veteran Kazak FO36/0** (Mimetism(-3), W1+NWI, ARM4, Warhorse, Sixth Sense, Immunity IMM-B/Shock, T2 Rifle/HFT) is a sturdy multipurpose terminal carrier; **Paramedic38/0** is separate. **Frontovik Paramedic23/0** Warhorse+Mimetism(-3) is the budget linked holder, **Strelok FO17/0** Camo/Decoy/FD+20 excellent retrieval but not invisibility while carrying. **Strelok K-9 Specialist Operative26/0** + synchronized K-9 Antipode makes two physical threats with *one shared Order*, not two independent orders. **Ratnik HRL41/1.5 / AP Spitfire46/1.5** has full armor W2/ARM6, Transmutation battle-ravaged (still physically active) and TA: high zone VP gun, **not an ordinary Supplies specialist**. **Counter:** exposed Ratnik draws anti-armor/guns; two Streloks plus one Veteran FO can preserve several quadrant options for similar points.

[Cross-game objective holder and zone-domination apex/value tiers, scenario rules, and opposing transcript reviews](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Exact profiles/Fireteams above are authoritative.

## Force multipliers — N5.3 role/value cross-reference (2026-10-23)

**Colonel Voronin LT22/0** has Counterintelligence+Sensor+Guard and +1 Command Token, but **NO Strategos in pinned TAK**; do not transplant Vanilla Ariadna's commander description. **Traktor Mul5/0 Baggage Regular Order** is among game's cheapest reload/Order support, with artillery profiles separately priced. **Kuryer Katyusha15/1** provides Baggage/Warhorse/Minelayer plus a real artillery role. **Strelok/Barsuk/Spetsnaz Decoy** are deception at chosen profile cost, *not real extra ARO bodies*. [Global force-multiplier tiers](../../notes/list-building/force-multipliers-special-abilities-apex-value.md).

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**K-9 Specialist26 with synchronized Sensor Antipode** or a legal **Antipode Assault Pack** gets Sensor to enemy Camo/Hidden markers; the *15-15 movement and scouting route* matters more than the keyword alone. **Voronin WIP14 Sensor** guards a local LT/command area, not the entire midfield. **Wardriver Disco Baller16/1** is scarce **Eclipse** against hostile MSV/Marksmanship; ordinary Smoke/cheap Irmandinho cannot blind MSV2. **Competing TAK judgments:** Antipode Sensor pressure is worth a dedicated approach when multiple markers actually block the mission; simply **ignore a low-value marker** if Discovering it would consume scoring Orders.

[Cross-game anti-tech N5.3 apex/value, mechanics, matchups and checked conflicting transcripts](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## N5.3 peripheral / synchronized / multi-body apex-value update

**Antipode pack26/0** = Handler+3 fast Camouflaged/Sensor/AP melee Control Peripherals, **Regular+Tactical Awareness** from handler; only **one Spearhead** performs target-requiring Attack with controller per Order, other Antipodes can Move; no triple independent CC. **Strelok K-9 Specialist Operative26/0** = STRELOK SMG/Camo/Decoy/FD+20 + synchronized **K-9 Antipode with Sensor/Climbing+**, which can approach separate angles within Controller Coherency; **17/0 FO** has **no dog**. **Dozer/Irmandinho Engineer + 2pt Remontnikbot Servant** remote recovery can position on separate flanks without Engineer walking; one target per Order. **Opposing:** 26pt Antipode pack is stronger high-speed Sensor/CC strike engine, 26pt Strelok+K-9 is stronger **actual specialist plus one dog** carrying mission when alive; `Control` Spearhead ≠ `Synchronized` two full attack targets.

[Cross-game multi-body apex/value and transcript disputes](../../notes/list-building/peripheral-synchronized-multibody-apex-value.md). Current sectorial roster and N5.3 rules decide actual type and access.
