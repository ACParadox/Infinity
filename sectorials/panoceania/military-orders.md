---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 103
sectorial_slug: military-orders
sectorial_name: Military Orders
parent_faction: PanOceania
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Military Orders roster, standard loadouts, canonical Fireteam chart, and reverse Fireteam index. Confessor Spec-Ops and Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# Military Orders

## Overview and provenance

Repository-native reference for **Military Orders** roster, profiles, points/SWC, AVA, and Fireteam access.

Sources used:

- Army-derived Military Orders source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **36-unit standard Military Orders roster** and the complete Military Orders `fireteamChart` in the pinned Army source.
- Soldier of Fortune entries with empty faction lists are excluded from the base roster.
- `Confessor Spec-Ops` and `Confessor Team-Ops` are optional game-mode content and are listed separately.
- Fireteam legality comes from the canonical chart in this file, not from an `FTO` loadout name by itself. The Clipper Dronbot is the important Military Orders example: it has an FTO-labelled option but no Military Orders Fireteam-chart row.
- Parenthetical Army-chart comments such as `(Crosier)`, `(Order Sergeant)`, and `(Knight Hospitaller)` are **Counts-as / equivalence labels**, not restrictions on which Fireteam a Wildcard may join.
- Counts-as comments attached to a native member row are row-specific unless the same equivalence is separately present in another row.
- Knights of Santiago profiles with Combat Jump explicitly **cannot be part of a Fireteam**.
- Only one Joan of Arc may be selected across Joan v1 and Joan v2.
- Linked Reinforcement section: **Code: Capital** (`army_id: 199`). No Reinforcement Fireteam rows are merged into the main chart here.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Military Orders |
| Parent faction | PanOceania |
| Army ID | 103 |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 36 |
| Optional-mode units | Confessor Spec-Ops; Confessor Team-Ops |
| Reinforcement roster | Code: Capital (`199`) |
| Fireteam chart | yes |

## Roster index

| Unit | ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| Military Order Curators | 1587 | 1 | LI | Regular | Military Orders; Order Sergeants |
| PanOceanian Black Friars | 771 | 2 | MI | Regular | Military Orders; Order Sergeants |
| Bulleteer Armbots | 35 | 2 | REM | Regular | Order Sergeants; Velox |
| Tikbalang of Montesa | 33 | 1 | TAG | Regular | — |
| Infirmarers of Saint Lazarus | 1487 | 3 | MI | Regular | Military Orders; Order Sergeants; Velox |
| Order Sergeants | 24 | 4 | LI | Regular | Military Orders and Order Sergeants, FTO profiles only |
| Trinitarian Tertiaries | 1527 | 3 | SK | Regular | — |
| Coadjutor Crosiers | 1560 | T | LI | Regular | Military Orders required-choice |
| Warcors | 50 | 1 | LI | Irregular | — |
| Sierra Dronbots | 17 | 2 | REM | Regular | — |
| Joan of Arc | 20 | 1 | HI | Regular | Crusade; counts as Knight Hospitaller |
| Knights of Santiago | 27 | 3 | HI | Regular | Military Orders / Order Sergeants / Crusade, FTO profiles only |
| Raveneye Officers | 1588 | 1 | LI | Regular | — |
| Knights of Montesa | 28 | 1 | HI | Regular | Wildcard, FTO profile only |
| Pathfinder Dronbots | 16 | 2 | REM | Regular | — |
| Mulebots | 38 | 2 | REM | Regular | — |
| Knights of the Holy Sepulchre | 29 | 2 | HI | Regular | — |
| Joan of Arc v2 | 42 | 1 | HI | Regular | Crusade; Velox |
| Gabriele De Fersen | 40 | 1 | HI | Regular | Wildcard; counts as Knight Hospitaller |
| Knights Hospitaller | 6 | 5 | HI | Regular | Crusade, FTO profiles only |
| Clipper Dronbot | 18 | 1 | REM | Regular | —; FTO-labelled option has no MO chart row |
| Palbots | 37 | 2 | REM | Peripheral | — |
| Crusader Brethren | 43 | 3 | MI | Regular | — |
| Peacemaker Armbots | 36 | 2 | REM | Regular | — |
| Motorized Knights of Montesa | 1209 | 2 | HI | Regular | Velox required-choice |
| Seraphs | 34 | 2 | TAG | Regular | — |
| Indigo Brother Konstantinos | 47 | 1 | LI | Regular | Wildcard, FTO profile only; counts as Crosier / Order Sergeant |
| Knight Hospitaller Kyle Hawkins | 1586 | 1 | HI | Regular | Wildcard; counts as Knight Hospitaller |
| Padre-Inquisidor Mendoza | 1562 | 1 | HI | Regular | Wildcard, FTO profile only |
| Teutonic Knights | 30 | 3 | HI | Regular | Military Orders required-choice |
| Knight of Justice | 1489 | 2 | HI | Regular | Wildcard; counts as Knight Hospitaller |
| Team Crux Father-Knights | 1815 | 1 | HI | Regular | Wildcard, FTO profiles only |
| Knight Commander | 1561 | 1 | MI | Regular | Military Orders; counts as Crosier in that row |
| Fugazi Dronbot | 19 | 1 | REM | Regular | — |
| Tech-Bees | 935 | 1 | LI | Regular | — |
| Dart, Optimate Huntress | 1130 | 1 | SK | Regular | — |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Confessor Spec-Ops | 1913 | Spec-Ops | Military Orders and Order Sergeants rows, max 1 when Spec-Ops mode is in use |
| Confessor Team-Ops | 1927 | Team-Ops | No ordinary Military Orders Fireteam row |

## Unit details

### Military Order Curators

**ID 1587 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`. Engineer, Immunity (Shock), Religious Troop, Deactivator.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 17 | 0 | Combi Rifle, D-Charges, AP Mine, Pistol, CCW; GizmoKit | Military Orders max 1; Order Sergeants max 1 |
| 2 | 18 | 0 | As 1 + Deployable Cover | same |
| 3 | 20 | 0 | Combi Rifle, D-Charges, AP Mine, Armed Turret (Marksman Rifle), Pistol, CCW; GizmoKit | same |

In the Order Sergeants Fireteam row, Curator counts as **Order Sergeant**. That equivalence is not present in the general Military Orders row.

### PanOceanian Black Friars

**ID 771 · AVA 2 · MI** — `MOV 10-10 | CC 19 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. MSV2, Albedo (-6), Combat Instinct, Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 24 | 0 | Thunderbolt (+1B), Nanopulser, Pistol, CCW | Military Orders max 2; Order Sergeants max 1 |
| 3 | 27 | 0 | MULTI Rifle, Nanopulser, Drop Bears, Pistol, CCW; Biometric Visor; Discover (+3) | same |
| 4 | 22 | 1.5 | Heavy Rocket Launcher, Nanopulser, MULTI Pistol (+1B), CCW | same |

### Bulleteer Armbots

**ID 35 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Repeater, Remote Presence, Courage, Mimetism (-6).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Heavy Shotgun, PARA CCW (-3) | Order Sergeants max 1; Velox max 2 |
| 2 | 22 | 1 | Spitfire, PARA CCW (-3) | same |

### Tikbalang of Montesa

**ID 33 · AVA 1 · TAG** — `MOV 15-10 | CC 17 | BS 15 | PH 15 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`. ECM: Guided (-6), Remote Presence, Mimetism (-3), Climbing Plus, Tactical Awareness, NCO, BS Attack (SR-1), Courage, Terrain (Jungle), GizmoKit (PH=13).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 3 | 68 | 1.5 | **TIKBALANG OF MONTESA**; HMG, Heavy Flamethrower, DA CCW; Crabbot | — |

### Infirmarers of Saint Lazarus

**ID 1487 · AVA 3 · MI** — `MOV 15-5 | CC 21 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Martial Arts L1, Doctor, Dodge (+2.5), Stealth, Religious Troop, Terrain (Total), MediKit.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 20 | 0 | Combi Rifle, Boarding Pistol, Shock CCW | Military Orders max 1; Order Sergeants max 1; Velox max 1 |
| 2 | 17 | 0 | Boarding Shotgun, Boarding Pistol, Shock CCW | same |

In the Order Sergeants row, Infirmarer counts as **Order Sergeant**. It has no such equivalence in the Military Orders or Velox rows.

### Order Sergeants

**ID 24 · AVA 4 · LI** — `MOV 10-10 | CC 18 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 13 | 0 | **ORDER SERGEANT FTO**; Combi Rifle, Nanopulser, Pistol, CCW | Military Orders max 3; Order Sergeants min 1/max 3 |
| 3 | 15 | 1.5 | **ORDER SERGEANT FTO**; Heavy Rocket Launcher, Assault Pistol, CCW | same |
| 5 | 18 | 0.5 | **ORDER SERGEANT FTO**; Combi Rifle, Nanopulser, Pitcher, Pistol, CCW; Hacking Device, Hacker | same |
| 14 | 17 | 0 | **ESCORT SERGEANT**; Combi Rifle, Nanopulser, Pistol, CCW; AUXBOT | — |
| 15 | 22 | 1.5 | **ESCORT SERGEANT**; Heavy Rocket Launcher, Assault Pistol, CCW; Neurocinetics; AUXBOT | — |
| 16 | 22 | 0.5 | **ESCORT SERGEANT**; Combi Rifle, Nanopulser, Pistol, CCW; Hacking Device, Hacker; AUXBOT | — |

The FTO profiles count as **Crosier** when used in the Military Orders Fireteam row.

### Trinitarian Tertiaries

**ID 1527 · AVA 3 · SK** — `MOV 10-10 | CC 18 | BS 12 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Camouflage, Mimetism (-6), Infiltration, Surprise Attack (-3), Stealth, Religious Troop, Deactivator.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 25 | 1.5 | MULTI Sniper Rifle, Pistol, CCW | — |
| 2 | 24 | 0 | Boarding Shotgun, D-Charges, Shock Mine, Pistol, CCW; Killer Hacking Device, Hacker | — |
| 3 | 22 | 0 | Boarding Shotgun, D-Charges, Flash Pulse, Shock Mine, Pistol, CCW; Forward Observer | — |
| 4 | 23 | 1 | As 3; Minelayer | — |
| 5 | 23 | 0 | SMG (+1SD), Flash Pulse, D-Charges, Shock Mine, Pistol, CCW; Forward Observer | — |
| 6 | 23 | 1 | Boarding Shotgun, Flash Pulse, D-Charges, Pistol, CCW; Deployable Repeater; Minelayer, Forward Observer | — |

### Coadjutor Crosiers

**ID 1560 · AVA Total · LI** — `MOV 10-10 | CC 15 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 11 | 0 | Combi Rifle, Pistol, CCW | Military Orders required-choice, max 5 |
| 2 | 12 | 0 | Combi Rifle, Blitzen, Pistol, CCW | same |
| 3 | 19 | 1 | MULTI Sniper Rifle, E/M Mine, Pistol, CCW; Minelayer | same |
| 4 | 18 | 1 | Spitfire, Pistol, CCW; X Visor | same |
| 5 | 13 | 0 | Combi Rifle, Pistol, CCW; MediKit, Paramedic | same |
| 6 | 24 | 1 | HMG, Pistol, CCW; MSV2 | same |
| 7 | 13 | 0 | Combi Rifle, Pistol, CCW; Commlink (+1), Specialist Operative | same |

### Warcors

**ID 50 · AVA 1 · LI · Irregular** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Journalist.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor | — |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); Sixth Sense | — |

### Sierra Dronbots

**ID 17 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage, Total Reaction, 360º Visor.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 1 | HMG, PARA CCW (-3) | — |
| 2 | 18 | 0 | Thunderbolt (+1B), PARA CCW (-3) | — |

### Joan of Arc

**ID 20 · AVA 1 · HI** — `MOV 10-10 | CC 23 | BS 15 | PH 15 | WIP 15 | ARM 5 | BTS 6 | W 2 | S 2`. Martial Arts L3, Inspiring Leadership, Frenzy, Stealth, NWI, Religious Troop, Tactical Awareness, Number 2, BS Attack (SR-1), X Visor.

All profiles: MULTI Rifle, Pulzar (+1B), Pistol, EXP CCW.

| Opt | Pts | SWC | Differences | FT |
|---:|---:|---:|---|---|
| 1 | 47 | 0 | Chain of Command; Non-Specialist | Crusade max 1; counts as Knight Hospitaller |
| 2 | 53 | 0 | Chain of Command; Non-Specialist; Strategic Deployment | same |
| 3 | 47 | +1 | Lieutenant | same |
| 4 | 51 | +1 | Lieutenant (+1 Command Token) | same |
| 5 | 53 | +1 | Lieutenant; Strategic Deployment | same |

Only one Joan of Arc may be selected across IDs 20 and 42.

### Knights of Santiago

**ID 27 · AVA 3 · HI** — `MOV 15-5 | CC 23 | BS 14 | PH 13 | WIP 13 | ARM 4 | BTS 3 | W 2 | S 2`. Martial Arts L1, Frenzy, Dodge (+2.5), Specialist Operative, Stealth, Religious Troop, Terrain (Zero-G), 360º Visor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 1.5 | **KNIGHT OF SANTIAGO FTO**; Spitfire, E/M Grenades, D-Charges, Boarding Pistol, DA CCW | MO max 2; Order Sergeants max 1; Crusade max 2 |
| 2 | 31 | 0 | **KNIGHT OF SANTIAGO FTO**; MULTI Rifle, D-Charges, Boarding Pistol, DA CCW; KHD, TinBot: Firewall (-3), Hacker | same |
| 3 | 38 | 0 | Boarding Shotgun (+1B), Flash Pulse, D-Charges, Shock Mine, Boarding Pistol, DA CCW; Combat Jump, Super-Jump (Jet Propulsion), KHD, Hacker | **cannot join Fireteams** |
| 4 | 36 | 0 | Boarding Shotgun (+1B), Flash Pulse, D-Charges, Shock Mine, Boarding Pistol, DA CCW; Combat Jump, Super-Jump (Jet Propulsion) | **cannot join Fireteams** |
| 5 | 33 | 0 | **KNIGHT OF SANTIAGO FTO**; Lieutenant; Spitfire, E/M Grenades, D-Charges, Boarding Pistol, DA CCW | MO / Order Sergeants / Crusade as above |
| 6 | 31 | 0 | **KNIGHT OF SANTIAGO FTO**; Lieutenant; MULTI Rifle, D-Charges, Boarding Pistol, DA CCW; KHD, TinBot: Firewall (-3), Hacker | same |

Army source note: **Options with Combat Jump cannot be part of a Fireteam.**

### Raveneye Officers

**ID 1588 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Minelayer, Forward Observer, Immunity (Shock), Deactivator.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 12 | 0 | SMG, E/Marat, Flash Pulse, E/M Mine, Pistol, CCW | — |
| 2 | 12 | 0 | SMG, E/Marat, Flash Pulse, Cybermine, Pistol, CCW | — |

### Knights of Montesa

**ID 28 · AVA 1 · HI** — `MOV 10-10 | CC 23 | BS 13 | PH 13 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 2`. Martial Arts L2, Limited Cover, Mimetism (-3), Religious Troop, Impetuous, Terrain (Aquatic/Jungle), BS Attack (SR-1).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 32 | 1.5 | Red Fury, Boarding Pistol, DA CCW; Forward Deployment (+20) | — |
| 3 | 26 | 0 | Boarding Shotgun, Boarding Pistol, DA CCW; MediKit, Paramedic; Forward Deployment (+20) | — |
| 5 | 20 | 0 | **KNIGHTS OF MONTESA FTO**; Boarding Shotgun, Blitzen, Boarding Pistol, DA CCW; MediKit, Paramedic | Wildcard max 1 |
| 6 | 35 | 1.5 | Spitfire, Drop Bears, Boarding Pistol, DA CCW; Forward Deployment (+20) | — |

### Pathfinder Dronbots

**ID 16 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Repeater, Deactivator, Triangulated Fire, Forward Observer, Sensor, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3) | — |
| 2 | 17 | 0 | As 1; Tactical Awareness | — |

### Mulebots

**ID 38 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 4`. Baggage, Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | Deactivator, Repeater, PARA CCW (-3) | — |
| 2 | 14 | 0.5 | EVO Hacking Device, Hacker, PARA CCW (-3) | — |
| 3 | 17 | 0 | Repeater, Combi Rifle, PARA CCW (-3); Total Reaction | — |

### Knights of the Holy Sepulchre

**ID 29 · AVA 2 · HI** — `MOV 15-5 | CC 22 | BS 14 | PH 13 | WIP 13 | ARM 5 | BTS 9 | W 2 | S 5`. Holoprojector, Surprise Attack (-3), Natural Born Warrior, Stealth, Religious Troop, Warhorse, BS Attack (SR-1).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 53 | 0 | MULTI Marksman Rifle (+1B), Heavy Pistol, Shock CCW; Deployable Repeater | — |
| 4 | 53 | 1 | AP HMG, Heavy Pistol, Shock CCW; NCO | — |

### Joan of Arc v2 (Mobility Armor)

**ID 42 · AVA 1 · HI** — `MOV 15-5 | CC 23 | BS 15 | PH 14 | WIP 15 | ARM 3 | BTS 6 | W 2 | S 2`. Martial Arts L3, Inspiring Leadership, Frenzy, NWI, Stealth, Religious Troop, Tactical Awareness, Number 2, Terrain (Total), X Visor.

All profiles: AP Spitfire, Pulzar (+1B), Pistol, EXP CCW.

| Opt | Pts | SWC | Differences | FT |
|---:|---:|---:|---|---|
| 2 | 45 | 1.5 | Chain of Command; Non-Specialist | Crusade max 1; counts as Knight Hospitaller; Velox required-choice max 1 |
| 3 | 51 | 1.5 | Chain of Command; Non-Specialist; Strategic Deployment | same |
| 4 | 45 | 1 | Lieutenant | same |
| 5 | 49 | 1 | Lieutenant (+1 Command Token) | same |
| 6 | 51 | 1 | Lieutenant; Strategic Deployment | same |

Only one Joan of Arc may be selected across IDs 20 and 42.

### Father-Officer Gabriele De Fersen

**ID 40 · AVA 1 · HI** — `MOV 15-5 | CC 22 | BS 14 | PH 14 | WIP 14 | ARM 4 | BTS 6 | W 2 | S 2`. Martial Arts L3, Dodge (+2.5), Stealth, Religious Troop, Hacking Device with Trinity (+1SD), Hacker.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 42 | 0.5 | MULTI Rifle, Light Flamethrower, Flash Pulse, Pistol, AP+Shock CCW | Wildcard max 1; counts as Knight Hospitaller |
| 2 | 46 | 1.5 | Spitfire, Flash Pulse, Pistol, AP+Shock CCW | same |
| 3 | 42 | 0.5 | As 1; Lieutenant | same |
| 4 | 46 | 1.5 | As 2; Lieutenant | same |

### Knights Hospitaller

**ID 6 · AVA 5 · HI** — `MOV 10-10 | CC 22 | BS 14 | PH 14 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 2`. Martial Arts L2, Frenzy, Stealth, Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 27 | 0 | **KNIGHT HOSPITALLER FTO**; MULTI Rifle, Pistol, DA CCW; TinBot: Firewall (-3) | Crusade min 1/max 5 |
| 3 | 32 | 1.5 | **KNIGHT HOSPITALLER FTO**; HMG, Pistol, DA CCW | same |
| 4 | 26 | 0 | **KNIGHT HOSPITALLER FTO**; Boarding Shotgun, E/Mitter, Pistol, DA CCW | same |
| 7 | 30 | 0 | **KNIGHT HOSPITALLER FTO**; MULTI Rifle, Pistol, DA CCW; MediKit, Doctor | same |
| 8 | 27 | 0 | **KNIGHT HOSPITALLER FTO**; Lieutenant; MULTI Rifle, Pistol, DA CCW; TinBot: Firewall (-3) | same |
| 9 | 32 | 0 | Boarding Shotgun, Contender, D-Charges, Pistol, DA CCW; Forward Deployment (+20) | — |
| 10 | 32 | 1 | **KNIGHT HOSPITALLER FTO**; Lieutenant; HMG, Pistol, DA CCW | Crusade min 1/max 5 |

### Clipper Dronbot

**ID 18 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CCW (-3); BS Attack (Guided) | — |
| 5 | 19 | 1.5 | **CLIPPER DRONBOT FTO**; Missile Launcher (+1B), PARA CCW (-3) | **—; no Military Orders chart row** |

The FTO label on option 5 does not itself grant Military Orders Fireteam access.

### Palbots

**ID 37 · AVA 2 · REM · Peripheral** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Peripheral (Servant), Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | PARA CCW (-3) | — |

### Crusader Brethren

**ID 43 · AVA 3 · MI** — `MOV 10-10 | CC 21 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Martial Arts L2, Parachutist, Combat Jump, Super-Jump (Jet Propulsion), Combat Instinct, Religious Troop, Terrain (Zero-G).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 3 | 23 | 0 | Boarding Shotgun, D-Charges, Disco Baller, Pistol, E/M CCW | — |
| 4 | 28 | 0 | MULTI Rifle, Light Flamethrower (+1B), Pistol, E/M CCW | — |
| 5 | 31 | 1.5 | Spitfire, Pistol, E/M CCW | — |
| 6 | 23 | 0 | Boarding Shotgun, Flash Pulse, D-Charges, Pistol, E/M CCW; Forward Observer | — |

### Peacemaker Armbots

**ID 36 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Repeater, Remote Presence, Courage, Forward Deployment (+20), Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Heavy Shotgun, Pulzar, PARA CCW (-3); AUXBOT_3 | — |
| 3 | 24 | 0.5 | Heavy Shotgun, Pulzar, PARA CCW (-3); AUXBOT_3B | — |
| 4 | 23 | 0 | Boarding Shotgun, Pulzar, PARA CCW (-3); BS Attack (+1B); no Auxbot | — |
| 5 | 27 | 0 | As 4; AUXBOT_3 | — |

AUXBOT_3 carries Heavy Flamethrower, Shock Mine, PARA CCW (-3); AUXBOT_3B adds Minelayer.

### Motorized Knights of Montesa

**ID 1209 · AVA 2 · HI** — `MOV 20-15 | CC 23 | BS 13 | PH 13 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 4`. Motorcycle, Martial Arts L2, Limited Cover, Dodge (+2.5), Immunity (Shock), Mimetism (-3), Religious Troop, Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | Boarding Shotgun, Boarding Pistol, DA CCW | Velox required-choice max 2 |
| 2 | 26 | 0 | MULTI Rifle, Boarding Pistol, DA CCW | same |
| 3 | 29 | 1 | Red Fury, Boarding Pistol, DA CCW | same |
| 4 | 23 | 0 | Boarding Shotgun, Boarding Pistol, DA CCW; MediKit, Paramedic | same |

### Seraphs

**ID 34 · AVA 2 · TAG** — `MOV 15-10 | CC 23 | BS 15 | PH 16 | WIP 13 | ARM 7 | BTS 6 | W 3 | S 7`. ECM: Guided (-6), Martial Arts L1, BS Attack (SR-1), Remote Presence, Tactical Awareness, NCO, Religious Troop, Super-Jump, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 72 | 1.5 | AP Spitfire, Pulzar, EXP CCW; AUXBOT_2; Crabbot | — |
| 2 | 74 | 1.5 | MULTI HMG, Pulzar (+1B), EXP CCW; Crabbot | — |

### Indigo Brother Konstantinos

**ID 47 · AVA 1 · LI** — `MOV 10-10 | CC 18 | BS 12 | PH 12 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. MSV1, Mimetism (-3), Specialist Operative, Sensor, Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | **BROTHER KONSTANTINOS FTO**; MULTI Rifle, D-Charges, Disco Baller, Boarding Pistol, CCW; Deactivator | Wildcard max 1; counts as Crosier and Order Sergeant |
| 2 | 26 | 0 | AP SMG, Flammenspeer, D-Charges, Boarding Pistol, CCW; Infiltration, Surprise Attack (-3), Deactivator | — |

### Knight Hospitaller Kyle Hawkins

**ID 1586 · AVA 1 · HI** — `MOV 15-5 | CC 23 | BS 14 | PH 13 | WIP 13 | ARM 3 | BTS 6 | W 2 | S 2`. Martial Arts L3, Frenzy, Combat Instinct, Specialist Operative, Stealth, Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 32 | 0 | MULTI Marksman Rifle, Pulzar, Flash Pulse, MULTI Pistol, DA CCW | Wildcard max 1; counts as Knight Hospitaller |
| 2 | 26 | 0 | Boarding Shotgun, Flash Pulse, Boarding Pistol, DA CCW; BS Attack (+1B) | same |

### Padre-Inquisidor Mendoza

**ID 1562 · AVA 1 · HI** — `MOV 15-5 | CC 22 | BS 14 | PH 13 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 2`. Martial Arts L2, Frenzy, Mimetism (-6), Religious Troop, enhanced CC/BS attack traits.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 40 | 0 | Heavy Shotgun, Grenades, Boarding Pistol, DA CCW; Forward Deployment (+20), Transmutation | — |
| 3 | 45 | 0 | MULTI Rifle, Grenades, Boarding Pistol, DA CCW; Forward Deployment (+20), Transmutation | — |
| 4 | 40 | 0 | **MENDOZA FTO**; MULTI Rifle, Grenades, Boarding Pistol, DA CCW; TinBot: Firewall (-3), Number 2 | Wildcard max 1 |

### Teutonic Knights

**ID 30 · AVA 3 · HI** — `MOV 15-5 | CC 22 | BS 13 | PH 14 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`. Martial Arts L2, Limited Cover, Impetuous, Religious Troop, Terrain (Jungle), enhanced Dodge.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 18 | 0 | Light Shotgun, Panzerfaust, Pistol, DA CCW | Military Orders required-choice max 3 |
| 2 | 19 | 0 | As 1; TinBot: Firewall (-3) | same |
| 3 | 28 | 1.5 | Missile Launcher, Zapper, Pistol, DA CCW | same |
| 5 | 19 | 0 | SMG, Panzerfaust, Pistol, DA CCW; Specialist Operative | same |
| 6 | 29 | 1.5 | Spitfire, Pistol, DA CCW; X Visor, NCO | same |
| 7 | 18 | 0 | Lieutenant; Light Shotgun, Panzerfaust, Pistol, DA CCW | same |

### Knight of Justice

**ID 1489 · AVA 2 · HI** — `MOV 15-5 | CC 23 | BS 14 | PH 14 | WIP 13 | ARM 5 | BTS 9 | W 2 | S 2`. Martial Arts L2, Stealth, Religious Troop, Terrain (Mountain), Number 2.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 46 | 1.5 | Missile Launcher, Heavy Pistol, DA CCW | Wildcard max 2; counts as Knight Hospitaller |
| 2 | 42 | 1.5 | Spitfire, Heavy Pistol, DA CCW | same |
| 3 | 45 | 0.5 | MULTI Marksman Rifle, Pitcher, D-Charges, Heavy Pistol, DA CCW; Hacking Device, Hacker | same |
| 4 | 41 | 0 | MULTI Marksman Rifle, Flash Pulse, D-Charges, Heavy Pistol, DA CCW; Forward Observer | same |
| 5 | 42 | 1.5 | Lieutenant; Spitfire, Heavy Pistol, DA CCW | same |
| 8 | 45 | 1 | Spitfire, D-Charges, Heavy Pistol, DA CCW; Forward Deployment (+10) | same |
| 9 | 41 | 0 | Lieutenant; MULTI Marksman Rifle, Flash Pulse, D-Charges, Heavy Pistol, DA CCW; Forward Observer | same |

### Team Crux Father-Knights

**ID 1815 · AVA 1 · HI** — `MOV 15-5 | CC 22 | BS 14 | PH 14 | WIP 13 | ARM 5 | BTS 6 | W 2 | S 2`. Albedo (-6), Martial Arts L2, BS Attack (+1SD), Berserk, Natural Born Warrior, Specialist Operative, Stealth, Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 47 | 0 | AP SMG, Flash Pulse, D-Charges, CrazyKoala, Pistol, DA CCW; Surprise Attack (-3), Forward Deployment (+20), Hidden Deployment | — |
| 2 | 48 | 0.5 | AP SMG, Flash Pulse, D-Charges, Armed Turret (Combi Rifle), Pistol, DA CCW; Surprise Attack (-3), Forward Deployment (+20), Hidden Deployment | — |
| 3 | 54 | 0 | MULTI Marksman Rifle, D-Charges, CrazyKoala, MULTI Pistol, DA CCW; Forward Deployment (+20) | — |
| 4 | 46 | 0 | **CRUX KNIGHT FTO**; MULTI Marksman Rifle, Drop Bears, D-Charges, MULTI Pistol, DA CCW | Wildcard max 1 |
| 5 | 49 | 1.5 | **CRUX KNIGHT FTO**; Spitfire, Drop Bears, D-Charges, MULTI Pistol, DA CCW | Wildcard max 1 |
| 6 | 50 | 0 | **CRUX KNIGHT FTO**; as 4; Strategic Deployment | Wildcard max 1 |

### Knight Commander

**ID 1561 · AVA 1 · MI** — `MOV 10-10 | CC 20 | BS 13 | PH 12 | WIP 13 | ARM 2 | BTS 6 | W 1 | S 2`. Holomask, Martial Arts L2, Immunity (Shock), Religious Troop, enhanced Dodge / BS Attack.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Light Shotgun, Pulzar, Pistol, Shock CCW; Chain of Command | Military Orders max 1; counts as Crosier |
| 2 | 20 | 0 | Lieutenant; Boarding Shotgun, Pulzar, Pistol, Shock CCW | same |
| 3 | 24 | 0 | Lieutenant (+1 Order); Boarding Shotgun, Pulzar, Pistol, Shock CCW | same |

### Fugazi Dronbot

**ID 19 · AVA 1 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Remote Presence, Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) | — |

### Tech-Bees

**ID 935 · AVA 1 · LI** — `MOV 10-10 | CC 12 | BS 11 | PH 10 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 2`. Specialist Operative, TAGCom, Deactivator, GizmoKit.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 2 | 9 | 0 | Adhesive Launcher Rifle, Flash Pulse, Pistol, PARA CCW (-3); Deployable Repeater | — |

### Dart, Optimate Huntress

**ID 1130 · AVA 1 · SK** — `MOV 10-10 | CC 16 | BS 13 | PH 13 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. MSV1, Camouflage, Mimetism (-3), Forward Deployment (+20), Surprise Attack (-3), Stealth, NWI, Climbing Plus, Specialist Operative, Decoy (1), Terrain (Total), Immunity (Shock).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 35 | 0 | AP SMG, Viral Tactical Bow, E/M Grenades, Pistol, CCW | — |
| 2 | 35 | 0 | AP SMG, Viral Tactical Bow, Shock Mine, Pistol, CCW | — |
| 3 | 36 | 0.5 | As 2; Minelayer | — |
| 4 | 42 | 0.5 | As 2; Minelayer; Sharvara K-9 Peripheral | — |

## Fireteams

This section is **canonical**. The Unit → Fireteam index below is derivative.

### Chart limits

| Type | Raw source | Meaning |
|---|---:|---|
| Core | 1 | Maximum 1 |
| Haris | 1 | Maximum 1 |
| Duo | 256 | InfinityDB-normalized meaning: unlimited |

### FT-MO-01 — Military Orders Fireteams

**Types:** Core, Haris, Duo

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Crosier | 1560 | 0 | 5 | Yes | — | — |
| Teutonic Knight | 30 | 0 | 3 | Yes | — | — |
| Knight of Santiago FTO | 27 | 0 | 2 | Yes | — | FTO |
| Order Sergeant FTO | 24 | 0 | 3 | No | Crosier | FTO |
| Knight Commander | 1561 | 0 | 1 | No | Crosier | — |
| Black Friar | 771 | 0 | 2 | No | — | — |
| Curator | 1587 | 0 | 1 | No | — | — |
| Infirmarer | 1487 | 0 | 1 | No | — | — |
| Confessor | 1913 | 0 | 1 | No | Spec-Ops | Optional Spec-Ops mode |

The source marks Crosier, Teutonic Knight, and Santiago FTO as the required-choice rows for this formation. Counts-as/equivalence is preserved separately rather than being silently treated as an FTO restriction.

### FT-MO-02 — Order Sergeants Fireteams

**Types:** Haris, Duo

| Member | Unit ID | Min | Max | Required | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Order Sergeant FTO | 24 | 1 | 3 | No | — | FTO |
| Curator | 1587 | 0 | 1 | No | Order Sergeant | — |
| Infirmarer | 1487 | 0 | 1 | No | Order Sergeant | — |
| Knight of Santiago FTO | 27 | 0 | 1 | No | — | FTO |
| Black Friar | 771 | 0 | 1 | No | — | — |
| Bulleteer | 35 | 0 | 1 | No | — | — |
| Confessor | 1913 | 0 | 1 | No | Spec-Ops | Optional Spec-Ops mode |

At least one Order Sergeant FTO is required by explicit `min: 1`.

### FT-MO-03 — Crusade Fireteams

**Types:** Core, Haris, Duo

| Member | Unit ID | Min | Max | Required | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Knight Hospitaller FTO | 6 | 1 | 5 | No | — | FTO |
| Knight of Santiago FTO | 27 | 0 | 2 | No | — | FTO |
| Joan of Arc | 20 | 0 | 1 | No | Knight Hospitaller | — |
| Joan of Arc v2 | 42 | 0 | 1 | No | Knight Hospitaller | — |

At least one Knight Hospitaller FTO is required by explicit `min: 1`.

### FT-MO-04 — Velox Fireteams

**Type:** Duo

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Motorized Knight of Montesa | 1209 | 0 | 2 | Yes | — | — |
| Bulleteer | 35 | 0 | 2 | Yes | — | — |
| Joan of Arc v2 | 42 | 0 | 1 | Yes | — | — |
| Infirmarer | 1487 | 0 | 1 | Yes | — | — |

All four source member rows are marked `required: true`; they form the source required-choice set rather than requiring all four unit types simultaneously.

### Wildcards

All rows below are in the chart's **Wildcards** row. Parenthetical values are Counts-as labels, not join-scope restrictions.

| Wildcard | Unit ID | Max | Counts as | FTO restriction |
|---|---:|---:|---|---|
| Knight of Justice | 1489 | 2 | Knight Hospitaller | — |
| Knight of Montesa | 28 | 1 | — | FTO |
| Crux Knight | 1815 | 1 | — | FTO |
| Brother Konstantinos FTO | 47 | 1 | Crosier, Order Sergeant | FTO |
| De Fersen | 40 | 1 | Knight Hospitaller | — |
| Hawkins | 1586 | 1 | Knight Hospitaller | — |
| Mendoza | 1562 | 1 | — | FTO |

Wildcard status does not remove a Fireteam's native minimum/required-choice conditions. The canonical Fireteam row and applicable Counts-as rules remain authoritative for composition.

## Unit → Fireteam access index

| Unit | Fireteam access |
|---|---|
| Military Order Curator | FT-MO-01 max 1; FT-MO-02 max 1 and counts as Order Sergeant |
| Black Friar | FT-MO-01 max 2; FT-MO-02 max 1 |
| Bulleteer | FT-MO-02 max 1; FT-MO-04 Velox required-choice max 2 |
| Tikbalang | — |
| Infirmarer | FT-MO-01 max 1; FT-MO-02 max 1/counts as Order Sergeant; FT-MO-04 required-choice max 1 |
| Order Sergeant | FT-MO-01 max 3/counts as Crosier, FTO only; FT-MO-02 min 1/max 3, FTO only |
| Trinitarian | — |
| Crosier | FT-MO-01 required-choice max 5 |
| Warcor | — |
| Sierra Dronbot | — |
| Joan of Arc | FT-MO-03 max 1; counts as Knight Hospitaller |
| Knight of Santiago | FT-MO-01 required-choice max 2; FT-MO-02 max 1; FT-MO-03 max 2; **FTO profiles only**; Combat Jump options cannot join |
| Raveneye | — |
| Knight of Montesa | Wildcard max 1, **FTO profile only** |
| Pathfinder | — |
| Mulebot | — |
| Holy Sepulchre | — |
| Joan of Arc v2 | FT-MO-03 max 1/counts as Knight Hospitaller; FT-MO-04 required-choice max 1 |
| De Fersen | Wildcard max 1; counts as Knight Hospitaller |
| Knight Hospitaller | FT-MO-03 min 1/max 5, **FTO profiles only** |
| Clipper | —; FTO-labelled option has no MO Fireteam chart row |
| Palbot | — |
| Crusader Brethren | — |
| Peacemaker | — |
| Motorized Knight of Montesa | FT-MO-04 required-choice max 2 |
| Seraph | — |
| Konstantinos | Wildcard max 1, **FTO profile only**; counts as Crosier and Order Sergeant |
| Hawkins | Wildcard max 1; counts as Knight Hospitaller |
| Mendoza | Wildcard max 1, **FTO profile only** |
| Teutonic Knight | FT-MO-01 required-choice max 3 |
| Knight of Justice | Wildcard max 2; counts as Knight Hospitaller |
| Crux Knight | Wildcard max 1, **FTO profiles only** |
| Knight Commander | FT-MO-01 max 1; counts as Crosier in that row |
| Fugazi | — |
| Tech-Bee | — |
| Dart | — |
| Confessor Spec-Ops | FT-MO-01 max 1 and FT-MO-02 max 1 when Spec-Ops mode is in use |
| Confessor Team-Ops | — in the ordinary Military Orders chart |

## Tactical tags

Derived analysis aids, not official characteristics.

| Unit | Tags |
|---|---|
| Crosier | cheerleader, long-range ARO, long-range attack, specialist, MSV gunner, link anchor |
| Teutonic Knight | close assault, mid-range attack, long-range ARO, specialist, NCO, link anchor |
| Santiago | close assault, mid-range attack, KHD, specialist, airborne option, link anchor |
| Order Sergeant | cheap link member, hacker, long-range ARO, DZ defense |
| Curator | Engineer, tech-counter, deployable support, link support |
| Infirmarer | Doctor, close assault support, link support |
| Black Friar | MSV2, long-range ARO, mid-range attack, anti-camo, link support |
| Knight Commander | Lieutenant, Chain of Command, LT-order generation, decoy/Holomask, link support |
| Hospitaller | durable attack, Doctor, long-range attack, close assault, Crusade anchor |
| Joan v1/v2 | Lieutenant, Chain of Command, Tactical Awareness, Inspiring Leadership, close assault, link support |
| De Fersen | apex hacker, hacker, close assault, mid-range attack, Wildcard |
| Knight of Justice | hacker, specialist, long-range ARO, mid-range attack, Wildcard |
| Crux Knight | hidden deployment, midfield specialist, close assault, Wildcard |
| Montesa | fast/midfield attack, specialist, Wildcard FTO option |
| Motorized Montesa | fast attack, specialist, enemy-DZ attacker, Velox |
| Tikbalang | TAG, long-range attack, NCO, mobile attack |
| Seraph | TAG, long-range/mid-range attack, NCO, Super-Jump |
| Bulleteer | REM attack, Mimetism (-6), mid-range attack, Velox |
| Peacemaker | midfield defense, network projection, forward REM attack |
| Pathfinder | network projection, Sensor, specialist, Tactical Awareness option |
| Mulebot | Baggage, EVO, REM support, cheerleader |
| Fugazi | cheap order, network projection, flash ARO |
| Sierra | long-range ARO, Total Reaction |
| Trinitarian | midfield defense, midfield specialist, KHD, long-range ARO, network projection |
| Raveneye | DZ defense, midfield defense, tech-counter, specialist |
| Crusader | airborne, enemy-DZ attacker, specialist, network projection via Disco Baller |
| Holy Sepulchre | attack, NCO, network projection, deception |
| Dart | midfield attack, midfield specialist, anti-camo |
| Tech-Bee | tech-counter, TAG support, network projection |

## List-building patterns

Derived tactical guidance, not official Army characteristics or Fireteam rules.

### No mandatory chassis

Military Orders does not have a single mandatory unit or mandatory Fireteam. A robust list normally wants to solve four structural problems instead:

- **Midfield presence:** often a Trinitarian, Dart, forward Montesa, Peacemaker, or another piece that does not need to walk from the deployment zone before becoming relevant.
- **Hacking plan:** especially important when the list contains several HI/TAGs. This can be offensive hacking, KHD protection, TinBots, repeater projection, or a plan to remove hostile hackers by other means.
- **Cheap Regular Orders and defence:** Fugazi, Raveneye, Crosiers, Mulebots, and similar support keep expensive pieces supplied with Orders and prevent the army from becoming all premium bodies.
- **A second mission plan:** if the primary attacker dies, another specialist or attack package must still be able to score and finish the game.

The Knight Commander Lieutenant (+1 Order) is particularly synergistic with NCO attack pieces such as the Holy Sepulchre AP HMG, Seraph, Tikbalang, or Teutonic Knight Spitfire, but it is an architecture choice rather than a compulsory inclusion.

### Seraph vs Holy Sepulchre

Both are solo attack pieces with no Military Orders Fireteam access, and both can exploit NCO. Their list-building roles are different.

| Question | Holy Sepulchre NCO AP HMG | Seraph |
|---|---|---|
| Commitment | 53 points / 1 SWC | 72–74 points / 1.5 SWC |
| Order economy | NCO | NCO + Tactical Awareness |
| Primary strengths | AP HMG, ARM 5/BTS 9, Stealth, Holoprojector, Surprise Attack (-3), smaller S5 footprint | BS 15, ARM 7 / 3 W, Remote Presence, Super-Jump, Tactical Awareness, stronger movement and brute-force durability |
| Best use | Efficient long-range solo gun that leaves points for the rest of the list | Centerpiece attack engine expected to consume many activations and carry a larger share of the attack plan |
| Main constraint | Less raw durability and self-generated activity than the TAG | ~20 more points, larger S7 geometry, more of the list is committed to one model |

**Prefer the Holy Sepulchre** when the army also wants substantial midfield, hacking, Fireteam, or secondary-attack investment. The AP HMG profile is a strong long-range door opener without turning the entire list into a TAG-support shell. Stealth, BTS 9, Holoprojector, and the smaller silhouette also make it more comfortable on some dense tables or into hacking-heavy opposition.

**Prefer the Seraph** when the list is intentionally built around a centerpiece. Tactical Awareness plus NCO lets it spend a very large active turn without taking every flexible Regular Order from the rest of the army. Its BS 15, ARM 7, 3 W, Remote Presence, and Super-Jump make it better suited to brute-forcing difficult positions and exploiting elevation.

Seraph profile choice:

- **MULTI HMG:** default when the TAG is meant to dominate long lanes and act as the primary ranged breaker.
- **AP Spitfire + Auxbot:** stronger consideration on dense tables or missions that pull the TAG into the midfield, where AP, the Auxbot, and close-range template pressure matter more than HMG reach.

A useful shorthand is **Sepulchre = efficient solo heavy gunfighter; Seraph = centerpiece attack engine**.

### Fireteam philosophy

Do not start MO list construction by assuming a five-model Core is mandatory. Start with the models the mission and attack plan actually need, then create the smallest useful legal Fireteam around them. Duo/Haris-sized packages often preserve more points for independent midfield pieces and a second attack vector.

The four native formations have distinct purposes:

- **Military Orders Fireteam:** the broad default toolbox. It must satisfy the chart's required-choice structure through Crosier, Teutonic Knight, or Santiago FTO. This is a natural home for a cheap support shell or a compact knight attack team, with Wildcards adding specialist tools.
- **Order Sergeants Fireteam:** cheap utility Haris/Duo. It requires at least one Order Sergeant FTO and can bring support such as a Black Friar, Bulleteer, Santiago FTO, Curator, or Infirmarer. Use it when the main solo attacker already consumes many points and the Fireteam's job is support, ARO, or secondary attack.
- **Crusade Fireteam:** premium Joan/Hospitaller/Santiago architecture. It requires at least one Hospitaller FTO. Take it because the list deliberately wants the durable knight package, not merely to obtain a Fireteam bonus.
- **Velox Duo:** specialized fast package using the Motorized Montesa, Bulleteer, Joan v2, and/or Infirmarer required-choice set. Use it when the list wants coordinated speed or a fast secondary attack/scoring package.

Useful compact examples include a **Crux FTO + Teutonic Knight specialist/TinBot package**, or a cheap **Black Friar + Crosier/Order Sergeant support team**, provided the canonical formation's required-choice/minimum rules are satisfied. A Seraph or Holy Sepulchre usually benefits from such a secondary/support Fireteam because neither can join one itself.

### Montesa: foot vs motorized

The two Montesa entries solve different problems rather than being simple variants of the same role.

**Motorized Montesa — choose for repeated speed and table-wide scoring.** MOV 20-15 lets it cross large distances with very few Orders, making the 23-point Paramedic particularly attractive when objectives are spread out, a Turn 3 scoring swing is likely, or the specialist must change flanks. The cost is S4/motorcycle geometry: it is harder to hide and more constrained by narrow terrain than the S2 foot knight. Motorized Montesas can join only the Velox Fireteam.

**Forward-deployed foot Montesa — choose for midfield position and S2 geometry.** The 26-point Paramedic begins Forward Deployment (+20), so much of the one-time approach to the midfield is already paid before Turn 1. It is preferable when the model mostly needs to reach the centre once and remain there, or when terrain makes an S4 motorcycle awkward. The Red Fury and Spitfire variants are more explicitly gunfighter-oriented and compete with MO's many other premium shooters.

**FTO foot Montesa — choose as a Fireteam efficiency piece.** The 20-point Paramedic with Boarding Shotgun and Blitzen is a Wildcard and is the cheapest way to get a durable Montesa specialist into a Fireteam. It lacks the forward deployment of the independent foot profiles and the extreme movement of the bike; its reason to exist is efficient linked utility.

Practical defaults:

- **Solo mission runner:** Motorized Montesa Paramedic, 23 points.
- **Fireteam specialist:** Montesa FTO Paramedic, 20 points.
- **Midfield S2 specialist that should start forward and stay there:** Forward-deployed Montesa Paramedic, 26 points.

### Practical build order

A reliable MO construction sequence is:

1. Choose the primary attack engine: Seraph, Holy Sepulchre, Tikbalang, Joan, Crux-led package, etc.
2. Add midfield presence rather than assuming the primary attacker must solve every objective.
3. Add a fast or asymmetric secondary scorer such as Montesa, Crusader, Trinitarian, or Dart.
4. Add the hacking defence/offence appropriate to the number of HI/TAGs being exposed.
5. Build the smallest useful legal Fireteam from pieces already wanted.
6. Fill the remaining Order/defensive structure with efficient support such as Raveneye, Fugazi, Crosiers, Mulebots, Curator/Palbot, or other mission-specific tools.

This usually produces a more resilient MO list than starting from an expensive five-knight Fireteam and trying to solve the mission with whatever points remain.

## Video and competitive-play research (October 2026)

**Scope and confidence.** Community tactical opinion is subordinate to the **N5.3/September 2026 Army data and canonical Fireteams above**. An initial 2026-10-17 vidIQ pass lacked caption access; on **2026-10-19**, YouTubeMCP and PodcastMCP returned primary transcripts for the specifically identified sources below. Older lists and pre-October 2025 conclusions are historical examples, not live profile/Fireteam authority. Transcript takeaways below are attributed, with genuine differences of opinion retained.

### Recommended viewing and what each source establishes

| Priority | Source (published) | Why watch / evidence available | Evidence level |
|---|---|---|---|
| 1 | [Robert Shepherd — *Infinity N5 Faction Focus: Military Orders*](https://www.youtube.com/watch?v=JrMTA91V7wc) ([creator's companion article](https://buymeacoffee.com/robertshepherd/infinity-n5-faction-focus-military-orders), 2026-07-04, **85m 25s**) | Newest identified full dedicated MO faction focus. The creator explicitly frames MO as one of PanO's most difficult factions to build lists for, potentially a new-player trap because premium knights tempt players to omit support, and promises ways to use knight strengths despite these restrictions. | YouTube transcript reviewed 2026-10-19 |
| 2 | [Ryanj4043 — *N5: Military Orders Post Update Guide*](https://www.youtube.com/watch?v=xjs6rsspz8I) (**2025-12-22 UTC**, **52m 42s**) | Direct post-October-update discussion. Chapters: [impact 01:07](https://www.youtube.com/watch?v=xjs6rsspz8I&t=67s); [Fireteams 06:05](https://www.youtube.com/watch?v=xjs6rsspz8I&t=365s); LI 11:17; MI 17:41; [knights 22:50](https://www.youtube.com/watch?v=xjs6rsspz8I&t=1370s); skirmishers 42:44; [example list 45:56](https://www.youtube.com/watch?v=xjs6rsspz8I&t=2756s). Dates in community indexes sometimes show Dec 23. | YouTube transcript reviewed 2026-10-19 |
| 3 | [Sneaky Snake — *In Nomine Domini: A Comprehensive Overview of Military Orders*](https://www.youtube.com/watch?v=kRaambqovmw) (2025-10-20) | Specialist MO player examining strengths, weaknesses, profiles and Fireteam possibilities after the overhaul. | YouTube transcript reviewed 2026-10-19 |
| 4 | [Tactical Awareness S3E42 — *Military Orders (REDUX!)*](https://www.youtube.com/watch?v=RP6Uyyc447k) (2025-11-24) | Explicit focus on how the October update made MO a genuine hacking faction; Owen and Ash publish two example Army export codes in the [source index](https://forum.corvusbelli.com/threads/n5-recap-panoceanian-tacticas.43511/). | PodcastMCP transcript reviewed 2026-10-19 + published lists |
| 5 | [WIP12 E188 — *Military Orders with Sneaky Snake*](https://podcasts.apple.com/at/podcast/e188-military-orders-with-sneaky-snake/id1567047414?i=1000717137809) (2025-07-14) | Experienced MO player's IGL run (13th of 170+) with **actual published 300-point lists**; emphasis on knight-heavy lists and Trinitarian snipers. Predates the October patch. | PodcastMCP transcript reviewed 2026-10-19 + period list exports |
| Supplemental | [Sneaky Snake — *Fireteams Overview for Military Orders*](https://www.youtube.com/watch?v=VNieWyaL97M) (2025-04-06) | Detailed discussion of Crosier, Teutonic, Order Sergeant and Crusade formations. Historical Fireteam comments require a current chart cross-check. | [Secondary, unreviewed AI account](https://www.bureau-aegis.org/forum/index.php?msg=224393) |
| Supplemental | [Ryanj4043 — *N5: Military Orders Faction Overview*](https://www.youtube.com/watch?v=ODl0hOCIf3g) (2025-04-14 UTC, 63m 08s) | Early N5 unit-by-unit overview, predating the October update. The close/mid-range *shooting* interpretation, rather than automatic rush-to-melee, is summarized in a secondary article; re-check all profile evaluations against current Army data. | vidIQ metadata; tactical claims only from [secondary, unreviewed AI account](https://www.bureau-aegis.org/forum/index.php?msg=224610), not transcript |
| Supplemental | [Infinity the Dante — *Tournament List Building for Infinity N5: A Tale of Five Armies*](https://www.youtube.com/watch?v=feSXzclNpE8) (2025-02-27) | A **mission-packet-first** list-building demonstration, including [Military Orders List 1 at 14:50](https://www.youtube.com/watch?v=feSXzclNpE8&t=890s) and [List 2 at 21:35](https://www.youtube.com/watch?v=feSXzclNpE8&t=1295s). Use to compare why two lists cover different mission requirements, **not** as current exact-profile guidance (pre-October overhaul). | Published description and chapter times; **not** transcript |

**Research hygiene:** The older summaries may contain outdated costs, unit equipment, formation bonuses or mistaken terms. Resolve mechanics against the September 2026 Army snapshot **in this file**, and assess the videos' *strategic reasoning* separately. Videos discovered are not evidence that their subtitles or exact words were independently examined.

### Earlier discovery notes: provenance update

The prior vidIQ-only observations remain in the historical summary below, but **no longer describe the evidence status** of Robert's, Ryan's, Sneaky's or the two MO podcasts: their transcripts were subsequently checked. Unreviewed supplemental videos (older Ryan overview and Infinity the Dante list-building) retain their original lower-confidence labels. The primary transcript-based synthesis follows near the end of this research section.

### Patterns repeated across independent sources

1. **Close/mid-range firefights, not blind sword charges.** The knights' strong BS, two Wounds, short/mid-range weapons, templates and close-combat backup want to win the firefight first, then close on objectives. Avoid crossing the whole board under ARO merely because a model has excellent CC. This is a useful reading of Ryan's earlier faction overview, not a statement about a particular current profile.
2. **Buy orders with cheap units before accumulating expensive knights.** Crosiers, the 7-point Fugazi (AVA **1**, not a spam unit), Mulebots, Warcor and Tech-Bee make premium attack pieces usable. Having three exceptional attackers with an insufficient useful order pool is usually worse than having one primary, one complementary attacker/scorer and reliable support. Do not rigidly chase a 15-model target if it eliminates essential capabilities.
3. **Compact knight teams often beat the all-knight brick.** A full five-knight package can work, but cost, delivery geometry and hacking exposure make it a deliberate commitment. A cheap Crosier shell plus small Teutonic/Santiago team is a flexible alternative. The key comparison is *orders to cross the table and accomplish objectives*, not only peak Fireteam bonus.
4. **Midfield is insurance, not an optional afterthought.** Trinitarian infiltrators, Dart, forward Montesa, Peacemaker and appropriately chosen Crux profiles provide presence when the heavy spearhead stalls. The opponent should not be able to defeat MO simply by blocking one obvious approach lane.
5. **October 2025 hacking changes give MO an additional axis of play.** De Fersen's normal Hacking Device/Trinity (+1SD), Knight of Justice HD + Pitcher, Order Sergeant FTO HD + Pitcher, Santiago KHD/TinBot, Trinitarian KHD/Deployable Repeater, Peacemaker/Pathfinder/Fugazi repeaters and Tech-Bee repeater can be combined into an actual network. This is *an option*, not a requirement to build a dedicated hacking list in every mission.
6. **Defence should delay and tax, not consume the entire list.** Hidden/camouflaged Trinitarian sniper, Raveneye E/M/Cybermine, a Black Friar heavy rocket launcher, a Curator turret/mine, and cheap Flash Pulse threats create multiple problems that do not rely on a lone exposed expensive ARO piece.

These points align with the [post-update Tactical Awareness episode description](https://forum.corvusbelli.com/threads/n5-recap-panoceanian-tacticas.43511/), [Sneaky Snake tournament episode](https://podcasts.apple.com/at/podcast/e188-military-orders-with-sneaky-snake/id1567047414?i=1000717137809) and [community list-building discussion](https://www.reddit.com/r/InfinityTheGame/comments/1mhckxa). They are **patterns**, not statistical auto-includes or transcript-verified unanimity.

### Two concrete architectures from competitive discussion

**A. Teutonic/Santiago/Crux pressure, backed by hidden AROs.** Sneaky Snake's *Panic Room IGL 25* list was published with:
- Group 1: Santiago **Lieutenant Spitfire**; Santiago **KHD MULTI Rifle/TinBot**; Crux **FTO MULTI Marksman Rifle**; Teutonic **SMG specialist**, **TinBot Panzerfaust**, **NCO Spitfire**; Order Sergeant **FTO heavy rocket launcher**; Curator **armed-turret**; Fugazi; Tech-Bee.
- Group 2: **two Trinitarian MULTI Sniper Rifles**, Raveneye **Cybermine**, Mulebot Repeater and Warcor.
- Published period example: 300 points / 6 SWC / 15 units. [Full contemporary list in WIP12 source index](https://forum.corvusbelli.com/threads/n5-recap-panoceanian-tacticas.43511/); [creator's IGL discussion](https://www.youtube.com/watch?v=zg-ahZCSZx0).

**Why this matters:** This is positive evidence against "you must run TAGs" or "you must start from a five-model Crosier Core." Instead it invests in a **knight-heavy close/midfield package**, a Santiago KHD/TinBot, NCO attacks and **two distinct hidden long-range ARO problems**. The opposing player must account for concealed snipers while dealing with mobile two-Wound attackers. It is an **example**, not a current exact-cost recipe; re-enter profiles in N5.3 Army.

**B. Cheap Crosier backbone with distributed knights.** His second published *Boring MO pt.2* list included a Black Friar HRL, **Crosier Paramedic + two ordinary Crosiers + Knight Commander LT**, a **Teutonic NCO Spitfire + specialist + TinBot**, **Joan v2**, **Santiago KHD/TinBot**, plus **Hospitaller HMG + Doctor** and Fugazi/Tech-Bee support. [Published list](https://forum.corvusbelli.com/threads/n5-recap-panoceanian-tacticas.43511/).

**Why this matters:** The alternative invests in a comparatively cheap order/ARO shell and several **independently useful** heavy troops instead of only one big striking unit. The contrast between A and B is itself useful: MO can prioritize **hidden midfield denial** or **wider backup heavy-weapon/recovery coverage**. The document's canonical Fireteam chart determines which portions can actually link.

### Practical Fireteam packages to test in the current chart

| Package | Intended job | Important qualification |
|---|---|---|
| **Crosier(s) + Knight Commander LT + Black Friar or Order Sergeant FTO HRL** in Military Orders | Affordable order battery, LT camouflage/deception, ranged ARO | Uses FT-MO-01 required-choice/Crosier equivalence; do not mistake a cheap link for an unkillable defensive fortress |
| **Teutonic NCO Spitfire + Teutonic SMG specialist + Teutonic TinBot** in Military Orders | Efficient knight assault/mission team with a short-range answer, disposable Panzerfausts, firewall | Teutonics have **Impetuous/Limited Cover**; avoid assuming safe free moves while keeping a link; consider LT-order/NCO economy separately |
| **Santiago FTO KHD/TinBot + Teutonic NCO/specialist** in Military Orders | Specialist + hacker protection embedded into an assault package | Check required-choice and exact FTO; **Santiago Combat Jump profiles cannot link** |
| **Order Sergeant FTO hacker/Pitcher + Bulleteer Spitfire + Curator or Infirmarer** in Order Sergeants | Compact hacking projection plus Mimetism (-6) mobile gun and engineer/doctor support | Explicit **Order Sergeant FTO min 1**; the Bulleteer may only join the chart's eligible formation, not a generic Crusade |
| **Joan (v1/v2) + Hospitaller FTO Doctor/HMG + Santiago FTO KHD** in Crusade | Premium durable assault and recovery package | Explicit **Hospitaller FTO min 1**; costs compete with midfield, secondary plans and order generators |
| **Motorized Montesa Paramedic + Bulleteer or Joan v2** in Velox Duo | Quick scoring/short-range pressure; use when both pieces need to work in the same part of the table | Velox is a Duo; motorcycle base access/positioning and the two different models' ideal activation schedules matter |

These are **construction motifs**, not guaranteed solved lists. See canonical FT-MO-01 to 04 for legality. If a Fireteam is repeatedly consuming orders on low-impact movement, compare it against running its members independently.

### Lieutenant, CoC and NCO decision tree

- **Passive LT + NCO shell:** Knight Commander **LT (+1 Order), 24 points**, with a **separate** NCO such as Teutonic Spitfire, Sepulchre AP HMG, Tikbalang or Seraph. Current data: the commander also has a **20-point ordinary LT** and a **23-point CoC**, all materially different list-construction choices.
- **Fighting LT:** Santiago FTO Spitfire or KHD LT, a Joan LT, De Fersen LT, Hospitaller LT, Knight of Justice LT or Teutonic Panzerfaust LT when the points/plan justify it. Ask *which turn the LT must fight*, whether exposed attackers have a succession plan, and whether the LT order will be spent through NCO instead. Don't choose a combat LT simply because it is a knight.
- **Joan as CoC instead of LT:** Joan v2 **45-point CoC** may serve as the independent attack/insurance piece behind a safer LT, while a premium Joan LT supplies command economy when her exposure is manageable. Use the **single-Joan constraint** and relevant Crusade/Velox rows.
- **Knight Commander CoC:** inexpensive succession insurance **when located separately** from the LT risk. **Do not put the Lieutenant and their only CoC insurance in the same vulnerable Fireteam/cluster** if one template, attack angle or hacking chain could remove both. Holomask concealment can complicate the enemy's LT hunt but cannot replace a plan for LoL.
- **Conserve Orders, not merely models:** a list with a survivable LT but no efficient attack route still wastes the lieutenant's command advantage. Check whether the NCO actually wants the extra order each turn before purchasing it.

### Low-profile roles worth explicitly testing

- **Double Trinitarian MSR:** observed in the IGL list, creates uncertainty and covered lanes without having to expose both snipers from deployment. Opportunity cost: two **25-point / 1.5 SWC** models consume three of six SWC; ask whether missions need infiltrating FO/KHD specialists more than double long-range ARO.
- **Trinitarian FO SMG (+1SD), FO/minelayer, KHD or deployable-repeater minelayer:** flexible midfield button/denial options if an MSR's SWC is expensive. A KHD assassin may exploit Camouflage/Surprise Attack, but **do not infer a hidden-deployment state** from Camouflage alone.
- **Black Friar HRL versus MULTI Rifle/Drop Bears/Thunderbolt:** HRL is a comparatively cheap burst of ARO/template denial; other profiles emphasize movement and repeat engagements. MSV2 and Albedo make it a relevant anti-visual-tools choice, but do not call the HRL obligatory.
- **Order Sergeant FTO hacker versus Escort Sergeant:** FTO can join eligible teams and brings a **Pitcher**; Escort variants trade linking for an **Auxbot**, with Neurocinetics HRL or hacker options for independent defence. Choose based on whether the team can actually exploit FTO; don't assume Escort profiles are legal Fireteam filler.
- **Curator turret versus Deployable Cover/mines, with Palbot:** useful *system* of Engineer reach, deployed nuisance pieces and support for REMs/TAGs. A turret is a defensive upgrade, not permission to leave the engineer exposed.
- **Tech-Bee, 9 points:** beyond being a cheap order, has **Deployable Repeater**, TAGCom and GizmoKit; check combat-group placement and the applicable TAGCom rule when relying on its bonus.
- **Crux FTO versus hidden/forward Crux:** FTO MULTI Marksman/Drop Bears provides a premium **linked gun + specialist**; the non-FTO AP SMG **Hidden Deployment + Forward Deployment (+20)** variants instead buy an independent ambush/objective threat. One is not interchangeable with the other.
- **Raveneye E/Marat plus E/M Mine versus Cybermine:** a cheap defensive specialist that deters different movement/hacking approaches. Favors a position from which it can force costly enemy Discover, Dodge, clearance or short-range engagements.
- **Fugazi AVA 1, Pathfinder, Peacemaker and Mulebot:** treat these as *different* budget/network tools. Fugazi is the especially efficient seven-point order/repeater, but there is only **one**; Pathfinder offers Sensor/FO and optional Tactical Awareness; Peacemaker pushes repeater and template pressure forward; Mulebot offers cheap Baggage/repeater or EVO.

### Where published approaches disagree

- **"Knights first" versus "cheap link first":** Sneaky Snake's published competitive example demonstrates a genuine knight-heavy MO list; Ryan's earlier published overview emphasizes a cheap Crosier Core as a foundation. These are **two different successful construction hypotheses**, not a universal requirement. Build both for the mission packet.
- **TAG centerpiece versus S5 gunfighter + specialists:** a [community discussion](https://www.reddit.com/r/InfinityTheGame/comments/1mhckxa) includes preference for the Tikbalang over the Holy Sepulchre, while other players value Sepulchre's solo NCO and more flexible points allocation. Existing Seraph/Sepulchre comparison above remains relevant; **no universal winner**.
- **Full knight Core versus small attack team:** some players deliberately flood the table with linked armour; others note that five expensive knights are difficult to deliver and can overcommit to one route. A compact team is the safer *starting hypothesis*, not proof full Crusade/Military Orders Cores are bad.
- **April 2025 'little hacking' narrative versus post-October 2025 toolkit:** older critiques describe restricted hacking/projection. The post-update [Tactical Awareness description](https://forum.corvusbelli.com/threads/n5-recap-panoceanian-tacticas.43511/) explicitly calls out MO's now-useful hacking game. Current Knight of Justice/De Fersen/Order Sergeant/Santiago options supersede prepatch assertions.
- **Trinitarian sniper tax:** two were used successfully in a specific tournament environment. Others may favor a single sniper plus FO/KHD infiltrators to improve objective reach; check the mission packet and total SWC.

**Table-side checklist:** What opens the first hostile ARO? What attacks a repeater network? Which piece starts inside objective distance? What spends the LT/NCO/TacAware orders? Which hidden or disposable defender forces the opponent to spend an extra two Orders? Where is the LT/CoC physically separated? What scores if the primary knight/TAG is gone by Turn 2?


### Primary transcript audit — 2026-10-19 (MO + shared PanO TAG/REM tools)

**Read these first (actual subtitles/transcripts, not metadata):**

| Source | Most useful material | Confidence / period |
|---|---|---|
| [Robert Shepherd, *N5 Military Orders faction focus*](https://www.youtube.com/watch?v=JrMTA91V7wc) (2026-07-04) | [Cheap-order squeeze ~02:00](https://www.youtube.com/watch?v=JrMTA91V7wc&t=120s), [Knight Commander ~13:00](https://www.youtube.com/watch?v=JrMTA91V7wc&t=780s), [Tik/Seraph ~65:00](https://www.youtube.com/watch?v=JrMTA91V7wc&t=3900s), [example list ~76:00](https://www.youtube.com/watch?v=JrMTA91V7wc&t=4560s) | **Transcript checked**; best recent broad review |
| [Ryanj4043, *MO post-update guide*](https://www.youtube.com/watch?v=xjs6rsspz8I) (2025-12) | [Two-stage attackers ~03:00](https://www.youtube.com/watch?v=xjs6rsspz8I&t=180s), [modular Fireteams ~06:00](https://www.youtube.com/watch?v=xjs6rsspz8I&t=360s), [Knight of Justice/hacking ~34:00](https://www.youtube.com/watch?v=xjs6rsspz8I&t=2040s), [sample list ~46:00](https://www.youtube.com/watch?v=xjs6rsspz8I&t=2760s) | **Transcript checked**, post-October refresh |
| [Sneaky Snake, *In Nomine Domini*](https://www.youtube.com/watch?v=kRaambqovmw) (2025-10) | [MO structural costs ~08:00](https://www.youtube.com/watch?v=kRaambqovmw&t=480s), [Seraph/Tik ~74:00](https://www.youtube.com/watch?v=kRaambqovmw&t=4440s), [all PanO REMs ~78:00](https://www.youtube.com/watch?v=kRaambqovmw&t=4680s) | **Transcript checked**, post-refresh |
| [Sneaky Snake, *MO weapons guide*](https://www.youtube.com/watch?v=IRP_OjWDTMU) (2025-10) | [Crosier and Trinitarian MSR ARO ~02:00](https://www.youtube.com/watch?v=IRP_OjWDTMU&t=120s), [TAG investment ~36:00](https://www.youtube.com/watch?v=IRP_OjWDTMU&t=2160s) | **Transcript checked**; owner acknowledges limited personal TAG experience |
| [Tactical Awareness S3E42, *Military Orders Redux*](https://www.youtube.com/watch?v=RP6Uyyc447k) (2025-11) | [Hacking after update ~07–20m](https://www.youtube.com/watch?v=RP6Uyyc447k), [two very different list constructions ~24–32m](https://www.youtube.com/watch?v=RP6Uyyc447k) | **Podcast transcript checked** using episode `6xyHjc3R0N37bDHl0HiROO` |
| [WIP12 E188, *Sneaky Snake on MO*](https://podcasts.apple.com/at/podcast/e188-military-orders-with-sneaky-snake/id1567047414?i=1000717137809) (2025-07) | Santiago + double Trinitarian MSR tournament core; [Seraph/Tik ~48–55m](https://www.youtube.com/watch?v=NRIOoAyV1O0); [Peacemaker critique ~57m](https://www.youtube.com/watch?v=NRIOoAyV1O0) | **Podcast transcript checked**; **pre-October refresh**, use tactical reasoning only |
| [Loss of Lieutenant E142, *N5 TAG tier list*](https://open.spotify.com/episode/1h5CJfZC5zBPxdg66o7xIN) (2025-04) | **Seraph debate ~26–31m**; raw TAG quality vs cost of supporting it in MO | **Podcast transcript checked**; older N5 rules/meta |

#### Actual patterns and decisions (with the **why**)

1. **Plan a long-range opener, then the midfield finish.** Ryan divides attackers into *phase 1*: HMG/TAG/Sepulchre/Hospitaller or other long-range tools that suppress hard AROs; *phase 2*: Santiago, Teutonic, Joan, Montesa and boarding-shotgun specialists that move through the opened lanes to score. A list with only phase-2 Spitfires may spend too many Orders crossing defended 24–32-inch lanes. Robert independently notes MO's expensive and restricted long-range options.
2. **Low end, not knight quality, is the key list constraint.** Robert's objection is specifically the lack of cheap *useful* Regular Orders: Fugazi **AVA 1**, 11-point baseline Crosiers, limited inexpensive extras and 8-point Mulebots with awkward S4 deployment. A premium gun plus knight team needs a deliberate order/secondary-scoring budget; 13–14 models can still work if NCO/TacAware and secondary specialists are doing enough.
3. **Crosier utility is no longer mere tax.** Ryan likes the **24-point MSV2 HMG** as an inexpensive anti-visual-tech first-stage tool or backup gun, **19-point MSR Minelayer** as an ARO/E/M mine package, and small **Duo/Haris** packages that can switch tasks; he explicitly does *not* claim BS12 makes the HMG an apex gun. Robert rates it an occasional desperation/backup choice because it lacks premium gunfighter stats. Pick it to solve MSV/long-lane coverage cheaply, not to replace every TAG/Hospitaller.
4. **Order Sergeant FTO hacker + Pitcher is efficient *network projection*.** Robert specifically argues against buying a very expensive HI Pitcher merely to extend **De Fersen**: the 18-point linkable Order Sergeant can do that job. Trinitarian deployable-repeater/minelayer, Peacemaker, Pathfinder and Fugazi expand the network; **Knight of Justice hacker** can throw its own Pitcher. This is why post-October MO can field an actual hacking plan, whereas older "MO has poor hacking" diagnoses are date-dependent.
5. **Build distinct Fireteams for distinct jobs.** Ryan favors *optionality*: Crosier/MSV gun + Order Sergeant Pitcher, Santiago FTO + inexpensive escort, or a Teutonic/NCO/paramedic core; Tactical Awareness demonstrates both a **hacker/Guided combined-arms list** and a **durable-knight/Blitzen-Panzerfaust tower** backed by Baggage. A full five-knight Crusade is not a universal default; it is justified when its HMG/Doctor/TinBot pieces all need the same route.
6. **Redundant scoring and asymmetric AROs matter.** Sneaky's tournament group used Santiago LT Spitfire + KHD/TinBot and a Crux/Teutonic attack package with *two* Trinitarian MSRs. The second Teutonic specialist remained useful after the Crux died. His transcript also documents the **limits**: Tri MSRs can lose to mimetic TAGs or effective Triangulated Fire. Hidden snipers deter approaches; they are not an answer to every active-turn attacker.
7. **Point-defense is not just the most expensive ARO.** Sneaky's REM discussion likes Sierra's 360° Total Reaction in MO because HI firepower is costly to leave on guard, while Robert likes cheap *linked* Black Friar Albedo/MSV2 or Crosier/E/M setups selectively. Raveneye mine, Curator turret, Flash Pulse and Warcor can delay at lower investment. Do not buy a Sierra, Friar and two Trinitarian snipers by reflex; examine the specific lanes/threats.

#### TAGs, motorized troops and shared PanO comparisons — N5.3 data

**No unit of type `VH` appears on the current MO roster.** Its motorcycle unit is **Motorized Montesa (HI, S4)**, not a vehicle profile. **Redeye is not available in MO** even though another PanO sectorial can take it; do not import NCA examples as legal MO lists.

| Option | Best reason to include | Why/when it disappoints |
|---|---|---|
| **Tikbalang of Montesa — 68 pts, 1.5 SWC** | **Default efficient long-range gun**: BS15 + Mimetism (-3), Climbing Plus, HMG, NCO + Tactical Awareness, smaller S6; can open fire lanes and reposition for fewer points than Seraph. | **No AP HMG and no MO Tik LT (+1)**; struggle against hard ARM unless another piece brings AP/E/M/hacking. **No Pathfinder Fireteam** in MO: unlike Kestrel, cannot copy Tik + TacAware Pathfinder Duo. |
| **Seraph MULTI HMG — 74 pts, 1.5 SWC** | **Premium reach and relocation**: BS15, ARM7, 3 STR, Super-Jump, NCO + TacAware, MULTI HMG; can attack from surprising elevation at 24–32-inch ranges and return to safety. Robert and Sneaky **both favor this as the safer default** because the rangeband enables the jumping gun plan. | Large S7 target, a very expensive centerpiece and a thinner specialist/support shell. Avoid exposing it during reactive turn just because it is armored; plan Engineer/Palbot access and a backup scorer. |
| **Seraph AP Spitfire + Auxbot — 72 pts, 1.5 SWC** | **Dense table/short-mid fork**: AP against armor and Auxbot template pressure complement the TAG's speed and CC deterrence. WIP12 hosts appreciate the dramatic Auxbot fork. | Sneaky found Spitfire rangebands made it harder to exploit Super-Jump; Robert prefers HMG reach. The Auxbot does not justify fighting long-range AROs with a Spitfire. |
| **Holy Sepulchre NCO AP HMG — 53 pts, 1 SWC** | **Less-expensive pseudo-TAG**: AP HMG, Stealth, Holoprojector/Surprise Attack, BTS9/Warhorse, lower S5 footprint and NCO; frees ~15–21 points for midfield specialists, TinBots or another attack vector. | Robert warns it is still BS14 without persistent visual mods: use deliberate Surprise Attack peeks rather than asking it to win repeated open-ended gunfights. Ryan emphasizes its reduced hacking susceptibility versus TAGs. |
| **Motorized Montesa Paramedic — 23 pts, 0 SWC** | **Fast scoring and flank switch**: MOV20-15 on a motorcycle; optional Velox Duo for a planned mobile package. | S4 positioning, Limited Cover/Impetuous exposure and lane constraints. The **20-point FTO foot Montesa** provides a cheaper linked Blitzen/paramedic roadblock; the **26-point forward-deployed foot Paramedic** buys S2 midfield access. Neither foot profile is a vehicle. |

**Disagreement worth keeping:** Loss of Lieutenant's TAG panel liked Seraph's *raw* quality but downgraded its *in-MO* value because 72–74 points plus higher-than-average cost per supporting Order can leave the rest of the list too thin. Robert recommends trying the spectacular Seraph anyway, but often prefers the 68-point Tik as a **more repeatable gunfighting investment**. Sneaky says the TAGs are good **but MO is worse at supporting them than Kestrel/Vanilla**, where cheaper utility slots and (for Kestrel) Tik LT/FT interactions alter the arithmetic. This is *faction fit vs unit power*, not a disagreement about Seraph's stats.

#### REM selection — distinguish role from cheap Order

| REM | Select it because... | Tradeoff / rival |
|---|---|---|
| **Fugazi 7 pts; AVA 1** | Cheapest Regular Order, Mimetism(-3) Flash Pulse ARO, Repeater and rear-DZ AD deterrence. Sneaky describes it as his usual start. | Not a scalable two-bot battery here; exposed Repeater can open a hostile hacking vector. |
| **Mulebot 8 pts Baggage / 14 pts EVO / 17 pts TR Combi** | Baggage reloads valuable **Panzerfaust/Blitzen/Pitcher** stock; EVO supports Combat Jump and REM programs; 8-point version cheaply fills the Order pool. Robert shows Baggage beside multi-disposable knight AROs. | S4 deployment footprint; don't buy EVO without an actual target/program plan, or two baggage bots if there is no deployable space/reload use. |
| **Pathfinder 14 / 17 pts TacAware** | Fast independent **Sensor + FO + Repeater + Triangulated Fire** specialist, useful for clearing markers/reaching buttons while knights attack. TacAware helps self-fund. | **Cannot join any MO Fireteam**, unlike faction-specific tactics imported from Kestrel; vulnerable as a low-ARM repeater. |
| **Bulleteer 19 Shotgun / 22 Spitfire** | Mimetism(-6), fast gun and Repeater; **Spitfire** is a lower-cost gun/fork option in an Order Sergeant or Velox link; EVO investment becomes more valuable if also used elsewhere. | ARM1 single-Wound REM; shorter-band gun cannot replace the first long-range ARO opener. Build cover lanes or engineer recovery. |
| **Peacemaker 23–27 pts** | Forward Deployment (+20), repeater and **Auxbot Heavy Flamethrower / mine option** to threaten midfield and project De Fersen/Justice hacking; unlike Bulleteer it starts forward. | Sneaky specifically dislikes the **S4 deployment-space problem**, especially multiples, despite liking its profile. He favors the Auxbot/minelayer package; other players may accept the footprint for midfield lockout. |
| **Sierra 18 Thunderbolt(+1B) / 23 HMG** | Affordable **Total Reaction + 360°** backline ARO: keeps costly Knights free to attack, watches for AD, and is repairable. Thunderbolt saves 5 pts/1 SWC versus HMG; HMG brings its own range/damage pattern. | No mimetic defense; an exposed Sierra can be removed cheaply by dedicated ARO killers. Pick based on expected rangebands and SWC, not reflexively HMG. |
| **Clipper Guided ML 16 / FTO-labelled ML(+1B) 19** | Guided option becomes relevant **only** when Pitcher/Repeater/Spotlight plan is serious. Tactical Awareness used it with multiple high-end hackers. | **MO Fireteam chart does NOT link the FTO-labelled Clipper**; ordinary Guided setup is order- and support-hungry. |
| **Palbot 3 pts** | Remote Engineer reach for Tik/Seraph/REMs or Doctor reach for knights without moving the support specialist into danger. | Requires an actual controller and protected service route; it is not an independent order. |

#### Explicit differences of opinion, with explanation

- **Knight Commander LT(+1):** Ryan values Holomask LT/CoC flexibility and extra NCO fuel; **Robert calls the 24-point LT(+1) a possible trap** compared with the 18-point Teutonic LT: an expensive passive commander only makes sense if an NCO (especially Seraph) truly uses the added Order each turn. Never cluster your LT and *only* CoC insurance in one killable team.
- **Knight of Justice hacker vs De Fersen:** **Ryan** prefers the Justice hacker's **Pitcher, MULTI Marksman Rifle, D-Charges, BTS9 and Wildcard** multifunctionality in aggressive Haris packages; **Robert** calls De Fersen's WIP14 + Trinity(+1SD) an apex hacker and says a cheaper Order Sergeant Pitcher is enough to project him. Different jobs: autonomous attacking hacker vs best pure hacking contest.
- **Crosier/knight composition:** **Ryan** treats the now-useful Crosier HMG/MSR and flexible miniature links as serious options; **Sneaky** favors many real knights and sometimes runs without a Crosier Core; **Robert** argues both are plausible, but the elite-only build often fails its order budget. Start from mission roles, not an obligatory Core or "must run a TAG" dogma.
- **Teutonic / Montesa value:** **Robert** strongly favors 18–20-point Teutonic specialist/TinBot and **20-point foot Montesa FTO** as exceptional tough cheap ARO/scoring bodies (Blitzen/Panzerfaust, bonus special dice); **Ryan** questions whether updated Teutonic Spitfire/ML gun profiles justify expensive active/ARO commitments given Limited Cover, though still likes them as linked utility. Cheap defensive knight **≠** expensive knight main gun.
- **Hospitaller HMG teams:** **Ryan** plays a Hospitaller HMG-led Haris that clears first-stage targets while Doctor/Justice hacker follow and take objectives; **Robert** finds *multiple* Hospitallers a poor fit for MO's tight cheap-order economy, preferring a single premium shooter supported by lower-cost knights. Decide whether linked healing/guns actually saves Orders compared with a standalone Tik/Sepulchre.
- **Seraph / Tik / Sepulchre:** Raw Seraph movement and durability vs Tik's cheaper Mimetism gun vs Sepulchre's cheaper AP/Warhorse. Do not call any automatic; terrain, opponent ARM/hacking, need for long-range opener, and remaining 200+ points decide.

**Check current Army chart first.** Videos/podcasts may call historical legal Fireteams, AVAs or costs that changed by N5.3; this section extracts ideas only and deliberately preserves the latest reference's numbers and `FT-MO-01`–`04` legality.

### Shared PanO REM cross-check (2026-10-19): two viable Peacemaker roles

These are **additional primary-transcript opinions**, not replacements for the current Military Orders Fireteam chart or the MO-specific tactical evaluation above.

- **Peacemaker Minelayer (24 pts / 0.5 SWC) for reactive denial.** KingButt's [Vanilla PanO discussion (WIP12 E177)](https://open.spotify.com/episode/5YoQVh0YvxS2DCtIIGyskl) prioritizes a forward mine + Auxbot/template + Repeater package to make an enemy alpha expensive before the Peacemaker is activated. It supports MO's hacking/midfield-defence plan without needing a Fireteam; watch the S4 footprint.
- **Peacemaker +1B Boarding Shotgun/Auxbot (27 pts) for active assault.** Trent's [NCA discussion (WIP12 E201, ~57–59 min)](https://open.spotify.com/episode/3FT1No7zFHzpj7WC63hcCb) explicitly prefers the 27-point offensive version in lists that can exploit burst and projected Repeater/template pressure; he contrasts this with other players' preference for Minelayer. **Choose which job the list lacks** instead of treating either profile as a universal default. Any NCA/Kestrel Fireteam benefits in that discussion **do not transfer to MO**; use the chart above.
- **Sierra and Pathfinder remain situational for opposite reasons.** KingButt omits Sierra when Helots/Firefly turrets already cover reactive lanes—but **MO has no Helots/Fireflies in its pinned roster**, so a repairable 18-point TR Thunderbolt Sierra has less role overlap and can free knights to attack. Dante/Tristan [Vanilla PanO reaction](https://www.youtube.com/watch?v=qp458fqYq_s) instead value its repairable persistence. Pathfinder **17-point Tactical Awareness FO/Repeater/Sensor** is preferred for *independent scoring movement*, not because MO can link it (it cannot).
- **Crossover VH/TAG reading:** [WIP12 E180 Kestrel with Daboarder (~33–41 min)](https://open.spotify.com/episode/3JXkarf51Os0UUopYrM7IW) gives a strong **Redeye Blitzen** case for tempo/anti-VH defence; [WIP12 E201 NCA (~83–87 min)](https://open.spotify.com/episode/3FT1No7zFHzpj7WC63hcCb) argues for **GL Continuous Damage** alternate-angle utility. Redeye is **not on MO's current standard roster**, so these are comparative PanO design lessons, **not MO picks**. MO TAG decisions remain Tikbalang versus Seraph in their actual roster.

See [Vanilla PanO transcript-backed review](panoceania.md#transcript-backed-competitive-tactics-research-2026-10-19) for the full conflicting-opinion and source index.

## Validation and maintenance

- Standard roster represented: **36 units**.
- Optional-mode hooks: Confessor Spec-Ops and Confessor Team-Ops.
- Canonical Fireteam rows represented: **Military Orders, Order Sergeants, Crusade, Velox, Wildcards**.
- Limits preserved: `CORE 1`, `HARIS 1`, raw `DUO 256` = InfinityDB `unlimited`.
- Parenthetical source comments are stored as Counts-as/equivalence labels.
- FTO restrictions are applied only where the Fireteam member row/name contains an FTO marker/comment.
- No Fireteam access is inferred solely from a loadout having `FTO` in its name.
- Clipper option 5 is deliberately shown with no Fireteam access despite being labelled FTO because there is no Military Orders chart row for Clipper.
- Santiago Combat Jump options are deliberately excluded from Fireteams per the unit's explicit Army note.
- Main and Reinforcement Fireteams are not merged.

## Provenance

- Corvus Belli Army-derived source revision: `7.26246.158`.
- Army snapshot commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- Army data changed on / snapshot date: `2026-09-03`.
- InfinityDB semantic cross-check: `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Fireteam source: pinned Army `fireteamChart`, normalized using the same semantics documented in InfinityDB.
- Verified: `2026-10-15`.

## TAG tactical cross-reference (2026-10-23)

**Tikbalang of Montesa** is the more self-protecting mobile attacker (Mimetism, Climbing Plus, HFT; NCO for unused LT Orders), while **Seraph** brings AP Spitfire or MULTI HMG plus Pulzar, EXP CCW and Super-Jump to force closer angles. **Disagreement:** Tik is generally safer against opposing shooters; Seraph's AP and stronger close tools matter when armored targets/vertical approaches dominate. MO's tight order/support budget can make either expensive without a second scoring route.

Cross-faction **apex vs points-value** comparisons, matchup table, and direct MCP-reviewed podcast/video sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Current profile and Fireteam legality above remain authoritative.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Apex cyber shell:** **De Fersen HD + Trinity(+1SD), WIP14, 42/0.5**, a 2W combat Knight; **Knight of Justice HD 45/0.5** supplies a **BS14 Pitcher** and durable W2/BTS9 network entry. **Cheap alternative:** **Order Sergeant FTO HD/Pitcher 18/0.5** projects network without spending Knight money; **Trinitarian Camouflage/Infiltration KHD 24/0** is an independently scoring anti-Hacker. **Knight Santiago FTO KHD + TinBot 31/0** protects a legal team and can shoot; the 38pt Combat Jump KHD is **not** the FTO option. **Disagreement:** Tactical Awareness MO REDUX praises De Fersen's +SD Trinity/linked Firewall power but concedes even cheap enemy KHD can dice him. Buy premium Knights when the same model will fight and score, not for WIP alone.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**
