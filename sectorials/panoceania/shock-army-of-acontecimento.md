---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 102
sectorial_slug: shock-army-of-acontecimento
sectorial_name: Shock Army of Acontecimento
parent_faction: PanOceania
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Shock Army of Acontecimento roster, standard loadouts, canonical Fireteam chart, and reverse Fireteam index. Indigo Spec-Ops and Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# Shock Army of Acontecimento

## Overview and provenance

Repository-native reference for **Shock Army of Acontecimento (SAA / Acontecimento)** roster, profiles, points/SWC, AVA, and Fireteam access.

Sources used:

- Army-derived SAA source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **29-unit standard SAA roster** and the complete SAA `fireteamChart` in the pinned Army source.
- Current Army metadata marks Shock Army of Acontecimento as `discontinued: true`, but the N5.3 Army data still contains a complete selectable roster and Fireteam chart. This file records that current data rather than interpreting the metadata flag as a gameplay prohibition.
- Soldier of Fortune entries whose source faction list is empty are excluded from the base roster.
- `Indigo Spec-Ops` and `Indigo Team-Ops` are optional game-mode content and are listed separately.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name by itself. Beasthunter FTO **does** have an SAA chart row; Clipper Dronbot FTO does **not**.
- In the Acontecimento Fireteam, `KNIGHT OF MONTESA` is explicitly marked `FTO`; only the on-foot Montesa FTO loadout is used there. The separate Forward Montesa Duo row has no FTO restriction in the source.
- The structured `required: true` rows in Acontecimento and Moto-mecanizados Fireteams are preserved as required-choice sets; this file does not reinterpret them as requiring every marked unit type simultaneously.
- Scylla is unusual: Army exposes ordinary Scylla profiles and a selectable `Scylla FTO & Charybdis FTO` two-model package. The Fireteam chart separately lists `SCYLLA` with an FTO restriction and `CHARYBDIS FTO` as Wildcards. Both source layers are preserved below.
- Parenthetical Army-chart comments such as `(Bagh-Mari)` are Counts-as / equivalence labels, not join-scope restrictions.
- Linked Reinforcement section: **Code: Capital** (`army_id: 199`). No Reinforcement Fireteam rows are merged into the main chart here.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Shock Army of Acontecimento |
| Parent faction | PanOceania |
| Army ID | 102 |
| Army metadata | `discontinued: true` |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 29 |
| Optional-mode units | Indigo Spec-Ops; Indigo Team-Ops |
| Reinforcement roster | Code: Capital (`199`) |
| Fireteam limits | Core 1; Haris 1; Duo unlimited |
| Fireteam chart | yes |

## Roster index

| Unit | ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| Palbots | 37 | 4 | REM | Peripheral | — |
| Trauma-Docs | 14 | 1 | LI | Regular | — |
| Peacemaker Armbots | 36 | 2 | REM | Regular | — |
| Acontecimento Regulars | 21 | T | LI | Regular | Regulars; Acontecimento |
| Bagh-Mari Unit | 25 | 5 | MI | Regular | Regulars; Acontecimento required-choice |
| Kirpal Singh | 39 | 1 | MI | Regular | — |
| Bulleteer Armbots | 35 | 2 | REM | Regular | Acontecimento; Moto-mecanizados required-choice |
| Lt. Stephen Rao | 45 | 1 | MI | Regular | Wildcard; counts as Bagh-Mari |
| Warcors | 50 | 1 | LI | Irregular | — |
| Machinist SAA | 15 | 2 | LI | Regular | Regulars; Acontecimento; counts as Bagh-Mari in Acontecimento |
| Motorized Knights of Montesa | 1209 | 2 | HI | Regular + Impetuous | Moto-mecanizados required-choice |
| Tech-Bees | 935 | 1 | LI | Regular | — |
| Tikbalangs | 33 | 2 | TAG | Regular + Tactical Awareness | Moto-mecanizados required-choice |
| Sierra Dronbot | 17 | 1 | REM | Regular | — |
| Fugazi Dronbots | 19 | 3 | REM | Regular | — |
| Armand `Le Muet` | 680 | 1 | MI | Regular | — |
| Mulebots | 38 | 2 | REM | Regular | — |
| Akalis | 2 | 3 | MI | Regular | — |
| Beasthunters Free Guild | 1570 | 1 | SK | Irregular | Regulars, FTO option only |
| Guarda de Assalto | 26 | 2 | HI | Regular | — |
| Flight Officer Agnes Ferreira | 1504 | 1 | LI | Regular | Wildcard |
| Scylla / Charybdis FTO package | 721 | 1 | MI + REM | Regular | Wildcard, FTO package profiles |
| Dart, Optimate Huntress | 1130 | 1 | SK | Regular | — |
| Knights of Montesa | 28 | 2 | HI | Regular + Impetuous | Acontecimento FTO; Forward Montesa Duo |
| Pathfinder Dronbot | 16 | 1 | REM | Regular | Wildcard |
| Clipper Dronbot | 18 | 1 | REM | Regular | —; FTO-labelled option has no SAA chart row |
| Dragões | 11 | 1 | TAG | Regular + Tactical Awareness | Moto-mecanizados required-choice |
| ORC Troops | 5 | 5 | HI | Regular | Regulars; Acontecimento required-choice |
| Nagas | 59 | 2 | SK | Regular | — |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Indigo Spec-Ops | 1912 | Spec-Ops | Regulars and Acontecimento Fireteam rows, max 1 when Spec-Ops mode is in use |
| Indigo Team-Ops | 1926 | Team-Ops | No ordinary SAA Fireteam row |

## Unit details

### Palbots

**ID 37 · AVA 4 · REM Peripheral** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Peripheral (Servant), Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | PARA CC Weapon (-3) | — |

### Trauma-Docs

**ID 14 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. Doctor, MediKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Pistol, CC Weapon | — |

### Peacemaker Armbots

**ID 36 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Repeater, Remote Presence, Courage, Forward Deployment (+20), Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Heavy Shotgun, Pulzar, PARA CCW (-3); AUXBOT_3 | — |
| 3 | 24 | 0.5 | Heavy Shotgun, Pulzar, PARA CCW (-3); AUXBOT_3B with Minelayer | — |
| 4 | 23 | 0 | Boarding Shotgun, Pulzar, PARA CCW (-3); BS Attack (+1B); no Auxbot | — |
| 5 | 27 | 0 | Boarding Shotgun, Pulzar, PARA CCW (-3); BS Attack (+1B); AUXBOT_3 | — |

### Acontecimento Regulars

**ID 21 · AVA T · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Terrain (Jungle).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 10 | 0 | Combi Rifle, Pistol, CCW | Regulars min 1/max 5; Acontecimento max 2 |
| 2 | 16 | 1 | Spitfire, Pistol, CCW | same |
| 3 | 12 | 0 | Combi Rifle, Flash Pulse; Deployable Repeater, Forward Observer | same |
| 4 | 20 | 1 | MULTI Sniper Rifle; Sapper | same |
| 5 | 17 | 0.5 | Combi Rifle, Cybermine; Hacking Device, FastPanda | same |
| 6 | 13 | 0 | Combi Rifle, Shock Mine; Triangulated Fire, Minelayer, Sensor | same |
| 7 | 12 | 0 | Combi Rifle; MediKit, Paramedic | same |
| 8 | 10 | 0 | Combi Rifle; Lieutenant | same |
| 10 | 12 | 0 | Combi Rifle; Commlink (+1), Specialist Operative | same |

### Bagh-Mari Unit

**ID 25 · AVA 5 · MI** — `MOV 10-10 | CC 16 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. MSV1, Warhorse, Mimetism (-3), Number 2, NCO, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Combi Rifle, Light Shotgun, Pistol, CCW | Regulars max 2; Acontecimento required-choice max 5 |
| 2 | 30 | 1.5 | HMG, Pistol, CCW | same |
| 3 | 29 | 0.5 | Combi Rifle, Light Shotgun; Hacking Device | same |
| 4 | 25 | 0 | Combi Rifle, Light Shotgun; MediKit, Paramedic | same |
| 5 | 21 | 0 | Combi Rifle, Light Shotgun; Lieutenant | same |
| 6 | 22 | 0 | Boarding Shotgun (+1B), Flash Pulse, D-Charges; Forward Observer | same |
| 7 | 29 | 1.5 | MULTI Sniper Rifle, Shock Mine; Minelayer | same |
| 8 | 27 | 1.5 | HMG; Lieutenant | same |

### Kirpal Singh, Akalis Sergeant

**ID 39 · AVA 1 · MI** — `MOV 10-10 | CC 21 | BS 13 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Martial Arts L1, Parachutist, Combat Jump, Stealth, Religious Troop, Immunity (Shock), NCO, Super-Jump (Jet Propulsion).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 0 | Boarding Shotgun (+1SD), D-Charges, Boarding Pistol, E/M CCW (PS 6); Chain of Command | — |
| 2 | 28 | 0 | Combi Rifle (AP), D-Charges, Assault Pistol, E/M CCW (PS 6); Specialist Operative | — |

### Bulleteer Armbots

**ID 35 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Repeater, Remote Presence, Courage, Mimetism (-6).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Heavy Shotgun (+1B), PARA CCW (-3) | Acontecimento max 1; Moto-mecanizados required-choice max 2 |
| 2 | 22 | 1 | Spitfire, PARA CCW (-3) | same |

### Lt. Stephen Rao, Bagh-Mari Unit

**ID 45 · AVA 1 · MI** — `MOV 10-10 | CC 16 | BS 13 | PH 11 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. MSV1, Warhorse, Mimetism (-3), Number 2, Specialist Operative, Terrain (Total), Immunity (Shock).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 25 | 0 | Combi Rifle, D-Charges, Assault Pistol, CCW; NCO | Wildcard max 1; counts as Bagh-Mari |
| 2 | 27 | 0 | Same; Lieutenant (+1 Command Token) | same |
| 3 | 27 | 0 | Same; Lieutenant (+1 Order); profile generates 2 Lieutenant Orders | same |

### Warcors

**ID 50 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Journalist.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor | — |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); Sixth Sense | — |

### Machinist SAA

**ID 15 · AVA 2 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`. Engineer, Deactivator, GizmoKit, Mimetism (-3), Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 6 | 17 | 0 | Combi Rifle, D-Charges, Pistol, CCW | Regulars max 1; Acontecimento max 2, counts as Bagh-Mari there |
| 14 | 18 | 0 | Same; Deployable Cover | same |
| 15 | 20 | 0 | Same; Armed Turret (Combi Rifle) | same |
| 16 | 19 | 0 | Same; Armed Turret (E/Mitter) | same |

### Motorized Knights of Montesa

**ID 1209 · AVA 2 · HI, S4** — `MOV 20-15 | CC 23 | BS 13 | PH 13 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 4`. Motorcycle, Martial Arts L2, Limited Cover, Dodge (+2.5), Immunity (Shock), Mimetism (-3), Religious Troop, Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | Boarding Shotgun, Boarding Pistol, DA CCW (PS 6) | Moto-mecanizados required-choice max 2 |
| 2 | 26 | 0 | MULTI Rifle, Boarding Pistol, DA CCW (PS 6) | same |
| 3 | 29 | 1 | Red Fury, Boarding Pistol, DA CCW (PS 6) | same |
| 4 | 23 | 0 | Boarding Shotgun, Boarding Pistol, DA CCW; MediKit, Paramedic | same |

### Tech-Bees

**ID 935 · AVA 1 · LI** — `MOV 10-10 | CC 12 | BS 11 | PH 10 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 2`. Specialist Operative, TAGCom [Dodge (PH+3), GizmoKit (PH+1)], Deactivator, GizmoKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 9 | 0 | Adhesive Launcher Rifle, Flash Pulse, Pistol, PARA CCW (-3); Deployable Repeater | — |

### Tikbalangs

**ID 33 · AVA 2 · TAG** — `MOV 15-10 | CC 17 | BS 15 | PH 15 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`. ECM: Guided (-6), Remote Presence, BS Attack (SR-1), Courage, GizmoKit (PH=13), Mimetism (-3), Tactical Awareness, Terrain (Total), Climbing Plus, Dodge (PH=11).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 69 | 1.5 | HMG, Heavy Flamethrower, Shock Mine, AP CCW (PS 5); Crabbot | Moto-mecanizados required-choice max 2 |
| 4 | 73 | 1.5 | Same; Lieutenant (+1 Order); Crabbot | same |

### Sierra Dronbot

**ID 17 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. 360º Visor, Remote Presence, Courage, Total Reaction.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 1 | HMG, PARA CCW (-3) | — |
| 2 | 18 | 0 | Thunderbolt (+1B), PARA CCW (-3) | — |

### Fugazi Dronbots

**ID 19 · AVA 3 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Remote Presence, Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) | — |

### Armand `Le Muet`, Freelance Killer

**ID 680 · AVA 1 · MI** — active profile `MOV 10-10 | CC 21 | BS 13 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 2 | S 2`; inactive Symbiont profile `ARM 0 | BTS 0`. BS Attack (+1SD), Forward Deployment (+10), Natural Born Warrior, Mimetism (-6), Stealth, Transmutation.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2338 | 33 | 1.5 | MULTI Sniper Rifle, Nanopulser, Shock Mine, Breaker Pistol (+1B), Viral CCW (PS 7); Minelayer | — |
| 2339 | 34 | 1.5 | MULTI Sniper Rifle, Nanopulser, Breaker Pistol (+1B), Viral CCW (PS 7); MSV1 | — |

### Mulebots

**ID 38 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 4`. Baggage, Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | PARA CCW (-3); Deactivator, Repeater | — |
| 2 | 14 | 0.5 | PARA CCW (-3); EVO Hacking Device | — |
| 3 | 17 | 0 | Combi Rifle, PARA CCW (-3); Repeater, Total Reaction | — |

### Akalis, Sikh Commandos

**ID 2 · AVA 3 · MI** — `MOV 10-10 | CC 16 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. Parachutist, Combat Jump, Religious Troop, Super-Jump (Jet Propulsion).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Combi Rifle, E/M Carbine, Pistol, E/M CCW | — |
| 2 | 21 | 0 | Boarding Shotgun (+1B), D-Charges, Pistol, E/M CCW; Deployable Repeater, Specialist Operative | — |
| 3 | 26 | 1.5 | Spitfire, Pistol, E/M CCW | — |
| 4 | 25 | 0.5 | Combi Rifle, Pistol, E/M CCW; Hacking Device | — |

### Beasthunters Free Guild

**ID 1570 · AVA 1 · SK** — `MOV 10-10 | CC 21 | BS 11 | PH 13 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. Mimetism (-3), Stealth, Super-Jump, Terrain (Total), Religious Troop; non-FTO profiles add Camouflage, Surprise Attack (-3), and Forward Deployment (+20).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 9 | 0 | **BEASTHUNTER FTO**; Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CCW (PS 5) | Regulars max 1; FTO only |
| 2 | 15 | 0 | HFT, Tactical Bow, AP Mine, Pistol, DA CCW; Camo/FD | — |
| 3 | 15 | 0 | HFT, Panzerfaust, AP Mine, Pistol, DA CCW; Camo/FD | — |
| 4 | 17 | 0 | HFT (+1B), Panzerfaust, AP Mine, Pistol, DA CCW; Camo/FD | — |

### Guarda de Assalto

**ID 26 · AVA 2 · HI** — `MOV 15-5 | CC 17 | BS 15 | PH 14 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`. Combat Instinct, Mimetism (-3). Each loadout includes an AUXBOT with Light Shotgun, Light Flamethrower, Eclipse Grenade Launcher, PARA CCW (-3), Courage, Mimetism (-3), Combat Instinct, and Peripheral (Synchronized).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 40 | 0 | MULTI Rifle, Heavy Flamethrower, D-Charges, AP Heavy Pistol, CCW (PS 6) | — |
| 2 | 44 | 1.5 | Spitfire, Heavy Flamethrower, D-Charges, AP Heavy Pistol, CCW | — |
| 3 | 40 | 1.5 | Heavy Rocket Launcher (+1B), Heavy Flamethrower, D-Charges, AP Heavy Pistol, CCW | — |

### Flight Officer Agnes Ferreira

**ID 1504 · AVA 1 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 2`. Courage, Specialist Operative, Sixth Sense, Terrain (Zero-G).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 13 | 0 | SMG, Nanopulser, Pistol, CCW | Wildcard max 1 |
| 2 | 16 | 0 | Same; RemDriver (+1 BS, +5 CC) | same |
| 3 | 18 | 0 | SMG, Nanopulser (+1B), Pistol, CCW; Chain of Command | same |

### Scylla and Charybdis FTO

**ID 721 · AVA 1 · MI / REM package.** Scylla: `MOV 10-10 | CC 20 | BS 12 | PH 11 | WIP 13 | ARM 2 | BTS 6 | W 1 | S 2`; ECM: Hacker (-3), Courage, Immunity (Shock), Terrain (Jungle), Cube 2.0. Charybdis FTO: `MOV 15-10 | CC 15 | BS 11 | PH 10 | WIP 11 | ARM 0 | BTS 3 | W 1 | S 2`; ECM: Hacker (-3), Repeater, Remote Presence, Courage, Terrain (Jungle).

| Selection | Pts | SWC | Loadout / differences | FT |
|---|---:|---:|---|---|
| Scylla opt 1 | 32 | 0.5 | E/Mitter, Light Shotgun, Pitcher, Pistol, Shock CCW (PS 7); Hacking Device, Trinity (SR-2); synchronized Devabot Charybdis | — |
| Scylla opt 3 | 32 | 0.5 | Same weapons; EVO Hacking Device, Trinity (SR-2); synchronized Devabot Charybdis | — |
| **Scylla FTO & Charybdis FTO package** | **37** | **0.5** | top-level option 1 = Scylla profile option 7 + Charybdis FTO group option 1; 2 miniatures and 2 Regular Orders | Both profiles appear separately in Wildcards |

Raw profile components of the FTO package:

- `SCYLLA FTO`, profile option 7: Hacking Device with Trinity (SR-2), E/Mitter, Light Shotgun, Pitcher, Pistol, Shock CCW (PS 7); Wildcard max 1, FTO restricted.
- `CHARYBDIS FTO`, subgroup option 1: Heavy Flamethrower, Heavy Pistol, PARA CCW (-3), Repeater; raw subgroup option is disabled for standalone selection and is enabled through the combined 37-point package; Wildcard max 1.

### Dart, Optimate Huntress

**ID 1130 · AVA 1 · SK** — `MOV 10-10 | CC 16 | BS 13 | PH 13 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. MSV1, Surprise Attack (-3), Camouflage, Courage, Forward Deployment (+20), Mimetism (-3), Immunity (Shock), Stealth, NWI, Terrain (Total), Climbing Plus, Specialist Operative, Decoy (1), Cube 2.0.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 35 | 0 | AP SMG, Viral Tactical Bow (+1SD), E/M Grenades, Pistol, CCW | — |
| 2 | 35 | 0 | AP SMG, Viral Tactical Bow (+1SD), Shock Mine, Pistol, CCW | — |
| 3 | 36 | 0.5 | Same as opt 2; Minelayer | — |
| 4 | 42 | 0.5 | Same as opt 3; includes Sharvara_K-9 HoundBot | — |

Sharvara_K-9: `MOV 15-10 | CC 22 | BS 11 | PH 12 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 3`; Camouflage, Mimetism (-3), Forward Deployment (+20), Peripheral (Synchronized), CC Attack (-6), improved Dodge, Natural Born Warrior, Stealth; Flash Pulse, Heavy Riotstopper, E/Marat, DA CCW (PS 7), PARA CCW.

### Knights of Montesa

**ID 28 · AVA 2 · HI** — `MOV 10-10 | CC 23 | BS 13 | PH 13 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 2`. Martial Arts L2, Limited Cover, Terrain (Aquatic/Jungle), BS Attack (+1SD), Mimetism (-3), Religious Troop, Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 32 | 1.5 | Red Fury, Boarding Pistol, DA CCW (PS 6); Forward Deployment (+20) | Forward Montesa Duo; not the Acontecimento FTO profile |
| 3 | 26 | 0 | Boarding Shotgun, Boarding Pistol, DA CCW; MediKit, Paramedic, Forward Deployment (+20) | Forward Montesa Duo |
| 5 | 20 | 0 | **KNIGHTS OF MONTESA FTO**; Boarding Shotgun, Blitzen, MediKit, Boarding Pistol, DA CCW; Paramedic | Acontecimento max 2; also eligible for Forward Montesa source row |
| 6 | 35 | 1.5 | Spitfire, Drop Bears, Boarding Pistol, DA CCW; Forward Deployment (+20) | Forward Montesa Duo |

### Pathfinder Dronbot

**ID 16 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Deactivator, Repeater, Remote Presence, Courage, Triangulated Fire, Forward Observer, Sensor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3) | Wildcard max 1 |
| 2 | 17 | 0 | Same; Tactical Awareness | same |

### Clipper Dronbot

**ID 18 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CCW (-3); BS Attack (Guided) | — |
| 5 | 19 | 1.5 | **CLIPPER DRONBOT FTO**; Missile Launcher (+1B), PARA CCW (-3) | —; no SAA Fireteam-chart row |

### Dragões, Acontecimento Dragoons

**ID 11 · AVA 1 · TAG** — `MOV 15-10 | CC 18 | BS 15 | PH 15 | WIP 13 | ARM 8 | BTS 6 | W 3 | S 7`. ECM: Guided (-6), BS Attack (SR-1), Courage, Dodge (PH=11), GizmoKit (PH=13), Immunity (Continuous Damage), Remote Presence, Tactical Awareness, Terrain (Jungle).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 76 | 1.5 | Hyper-Rapid Magnetic Cannon, Heavy Flamethrower (+1B), AP CCW (PS 5); Crabbot | Moto-mecanizados required-choice max 1 |

### ORC Troops

**ID 5 · AVA 5 · HI** — `MOV 15-5 | CC 15 | BS 14 | PH 14 | WIP 12 | ARM 4 | BTS 3 | W 2 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 28 | 0 | MULTI Rifle, Pistol, CCW | Regulars max 2; Acontecimento required-choice max 5 |
| 2 | 29 | 0 | MULTI Rifle; TinBot: Firewall (-3) | same |
| 3 | 34 | 1.5 | HMG | same |
| 4 | 26 | 0 | Boarding Shotgun (+1B) | same |
| 6 | 33 | 0.5 | MULTI Rifle; Hacking Device | same |
| 7 | 28 | 0 | MULTI Rifle; Lieutenant | same |
| 8 | 34 | 1 | HMG; Lieutenant | same |
| 10 | 35 | 1.5 | Feuerbach | same |
| 11 | 27 | 0 | Boarding Shotgun (+1B); TinBot: Firewall (-3) | same |

### Nagas

**ID 59 · AVA 2 · SK** — `MOV 10-10 | CC 16 | BS 12 | PH 12 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Surprise Attack (-3), Courage, Camouflage, Infiltration, Mimetism (-3), Stealth, Dogged, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 3 | 29 | 1.5 | MULTI Sniper Rifle, Nanopulser, Pistol, CCW; BS Attack (+1SD) | — |
| 4 | 25 | 0.5 | Boarding Shotgun, Nanopulser, Shock Mine, Pistol, CCW; Minelayer | — |
| 5 | 27 | 0 | AP SMG, Nanopulser, D-Charges, E/M Mine, Pistol, CCW; Killer Hacking Device | — |
| 6 | 29 | 0.5 | AP SMG, Nanopulser, D-Charges, Pistol, CCW; Hacking Device [Carbonite (+1SD)], Deployable Repeater | — |
| 7 | 25 | 0 | AP SMG, Nanopulser, Flash Pulse, D-Charges, Pistol, CCW; Deployable Repeater, Forward Observer | — |
| 8 | 26 | 0.5 | AP SMG, Nanopulser, Monofilament Mine, Pistol, CCW; Minelayer | — |

## Canonical Fireteam chart

Global chart limits: **Core 1 · Haris 1 · Duo unlimited** (`DUO: 256` in the raw Army data).

### FT-SAA-01 — Regulars Fireteams

**Types:** Core, Haris

| Member | Unit ID | Min | Max | Required | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Acontecimento Regular | 21 | 1 | 5 | No | — | — |
| ORC | 5 | 0 | 2 | No | — | — |
| Bagh-Mari | 25 | 0 | 2 | No | — | — |
| Machinist SAA | 15 | 0 | 1 | No | — | — |
| Beasthunter FTO | 1570 | 0 | 1 | No | — | option 1 only |
| Indigo | 1912 | 0 | 1 | No | Spec-Ops | Optional Spec-Ops mode |

At least one Acontecimento Regular is required by the explicit source `min: 1`.

### FT-SAA-02 — Acontecimento Fireteams

**Types:** Core, Haris, Duo

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| ORC | 5 | 0 | 5 | Yes | — | — |
| Bagh-Mari | 25 | 0 | 5 | Yes | — | — |
| Acontecimento Regular | 21 | 0 | 2 | No | — | — |
| Machinist SAA | 15 | 0 | 2 | No | Bagh-Mari | — |
| Knight of Montesa | 28 | 0 | 2 | No | — | **FTO option 5 only** |
| Bulleteer | 35 | 0 | 1 | No | — | — |
| Indigo | 1912 | 0 | 1 | No | Spec-Ops | Optional Spec-Ops mode |

ORC and Bagh-Mari are both marked `required: true` in the structured chart; they form the source required-choice set rather than this reference asserting that both unit types must be present simultaneously.

### FT-SAA-03 — Forward Montesa Fireteams

**Type:** Duo

| Member | Unit ID | Min | Max | Required | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Knight of Montesa | 28 | 2 | 2 | No | — | none in source row |

The source row requires exactly two Knights of Montesa and does not carry an FTO marker. This is distinct from the FTO-restricted Montesa row in FT-SAA-02.

### FT-SAA-04 — Moto-mecanizados Fireteams

**Type:** Duo

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Tikbalang | 33 | 0 | 2 | Yes | — | — |
| Motorized Knight of Montesa | 1209 | 0 | 2 | Yes | — | — |
| Bulleteer | 35 | 0 | 2 | Yes | — | — |
| Drãgao | 11 | 0 | 1 | Yes | — | — |

All four rows are marked `required: true` in the structured chart; they are preserved as the source required-choice set rather than interpreted as requiring all four unit types simultaneously.

### Wildcards

All rows below are in the chart's **Wildcards** row. Parenthetical values are Counts-as labels, not join-scope restrictions.

| Wildcard | Unit ID | Max | Counts as | FTO/profile restriction |
|---|---:|---:|---|---|
| Lt. Stephen Rao | 45 | 1 | Bagh-Mari | all Rao loadouts |
| Agnes | 1504 | 1 | — | all |
| Scylla | 721 | 1 | — | **Scylla FTO profile option 7**, supplied through the FTO package |
| Charybdis FTO | 721 | 1 | — | **Charybdis FTO subgroup profile**, supplied through the FTO package |
| Pathfinder Dronbot | 16 | 1 | — | all |

Wildcard status does not remove the native minimum/required-choice conditions of the Fireteam being joined. The Scylla/Charybdis package remains subject to its Army selection relationship; the chart's separate Wildcard rows are preserved without inferring additional package-splitting permissions.

## Unit → Fireteam access index

| Unit | Fireteam access |
|---|---|
| Palbot | — |
| Trauma-Doc | — |
| Peacemaker | — |
| Acontecimento Regular | FT-SAA-01 min 1/max 5; FT-SAA-02 max 2 |
| Bagh-Mari | FT-SAA-01 max 2; FT-SAA-02 required-choice max 5 |
| Kirpal Singh | — |
| Bulleteer | FT-SAA-02 max 1; FT-SAA-04 required-choice max 2 |
| Stephen Rao | Wildcard max 1; counts as Bagh-Mari |
| Warcor | — |
| Machinist SAA | FT-SAA-01 max 1; FT-SAA-02 max 2/counts as Bagh-Mari |
| Motorized Knight of Montesa | FT-SAA-04 required-choice max 2 |
| Tech-Bee | — |
| Tikbalang | FT-SAA-04 required-choice max 2 |
| Sierra | — |
| Fugazi | — |
| Armand `Le Muet` | — |
| Mulebot | — |
| Akal Commando | — |
| Beasthunter | FT-SAA-01 max 1, **FTO option 1 only** |
| Guarda de Assalto | — |
| Agnes | Wildcard max 1 |
| Scylla | Wildcard max 1, **FTO option 7/package only** |
| Charybdis FTO | Wildcard max 1, **FTO package subgroup only** |
| Dart | — |
| Knight of Montesa | FT-SAA-02 max 2, **FTO option 5 only**; FT-SAA-03 exactly 2, no FTO restriction in source row |
| Pathfinder | Wildcard max 1 |
| Clipper | —; FTO-labelled option has no SAA chart row |
| Drãgao | FT-SAA-04 required-choice max 1 |
| ORC | FT-SAA-01 max 2; FT-SAA-02 required-choice max 5 |
| Naga | — |
| Indigo Spec-Ops | FT-SAA-01 max 1; FT-SAA-02 max 1 when Spec-Ops mode is used |
| Indigo Team-Ops | — |

## Derived tactical index

These tags are analytical conveniences for modular list-building, not Army characteristics.

| Unit / profile | Tactical tags |
|---|---|
| Acontecimento Regulars | cheerleader, specialist, long-range ARO, hacker, network projection, midfield defense |
| Bagh-Mari | long-range attack, long-range ARO, mid-range attack, specialist, hacker |
| Kirpal Singh | airborne, enemy-DZ attacker, specialist |
| Bulleteer | mid-range attack, REM support, network projection |
| Stephen Rao | specialist, Lieutenant support |
| Machinist SAA | specialist, TAG support, REM support, tech-counter |
| Motorized Montesa | close assault, specialist, enemy-DZ attacker |
| Tikbalang | TAG support, long-range attack, mid-range attack |
| Sierra | long-range ARO, REM support |
| Fugazi | cheerleader, network projection, REM support |
| Armand `Le Muet` | long-range attack, long-range ARO, midfield defense |
| Mulebot | cheerleader, REM support, hacker, network projection |
| Akalis | airborne, enemy-DZ attacker, specialist, hacker, network projection |
| Beasthunter | midfield defense, DZ defense |
| Guarda de Assalto | mid-range attack, close assault, vision control |
| Agnes | specialist, Lieutenant support |
| Scylla / Charybdis | hacker, network projection, tech-counter, REM support |
| Dart | midfield specialist, midfield defense, enemy-DZ attacker |
| Knight of Montesa | close assault, midfield specialist, mid-range attack |
| Pathfinder | midfield specialist, network projection, tech-counter, REM support |
| Clipper | long-range attack, guided attack, REM support |
| Drãgao | TAG support, long-range attack, mid-range attack |
| ORC | mid-range attack, long-range attack, hacker, tech-counter |
| Naga | midfield specialist, midfield defense, hacker, KHD, network projection |
| Peacemaker | midfield attack, midfield defense, network projection, REM support |
| Tech-Bee | specialist, TAG support, network projection |
| Trauma-Doc / Palbot | specialist, support |
| Warcor | cheap ARO, cheerleader |

## Provenance and validation

- Corvus Belli Army-derived source revision: `7.26246.158`.
- Army snapshot commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- Army data changed on: 2026-09-03.
- InfinityDB semantics/reference commit: `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.
- Generated/verified: 2026-10-15.
- Standard roster count validated from source-faction membership: **29** logical units, excluding optional Indigo Spec-Ops/Team-Ops and Soldier of Fortune entries with empty faction membership.
- Canonical Fireteam chart validated against the source `fireteamChart`: 4 native team rows + Wildcards; limits Core 1 / Haris 1 / Duo unlimited.
- Regulars explicit `min: 1`, Forward Montesa exact `min: 2/max: 2`, all Fireteam maximums, required-choice flags, Counts-as labels, and FTO markers are preserved.
- Profile-restricted Fireteam access is explicitly represented for Beasthunter FTO, Knight of Montesa FTO, Scylla FTO, and Charybdis FTO.
- Clipper Dronbot's FTO-labelled loadout is intentionally **not** granted Fireteam access because the SAA chart contains no Clipper row.
- Scylla/Charybdis selection is represented as the source exposes it: ordinary Scylla options plus the selectable 37-point / 0.5-SWC two-model FTO package, with separate Wildcard rows preserved.
- Main and Reinforcement charts are not merged.
