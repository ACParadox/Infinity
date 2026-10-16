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
