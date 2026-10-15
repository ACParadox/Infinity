---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 105
sectorial_slug: varuna-immediate-reaction-division
sectorial_name: Varuna Immediate Reaction Division
parent_faction: PanOceania
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Varuna Immediate Reaction Division roster, standard loadouts, canonical Fireteam chart, and reverse Fireteam index. Indigo Spec-Ops and Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# Varuna Immediate Reaction Division

## Overview and provenance

Repository-native reference for **Varuna Immediate Reaction Division (Varuna / VIRD)** roster, profiles, points/SWC, AVA, and Fireteam access.

Sources used:

- Army-derived Varuna source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **27-unit standard Varuna roster** and the complete Varuna `fireteamChart` in the pinned Army source.
- Current Army metadata marks Varuna Immediate Reaction Division as `discontinued: true`, but the N5.3 Army data still contains a complete selectable roster and Fireteam chart. This file records that current data rather than interpreting the metadata flag as a gameplay prohibition.
- Soldier of Fortune entries whose source faction list is empty are excluded from the base roster.
- `Indigo Spec-Ops` and `Indigo Team-Ops` are optional game-mode content and are listed separately.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name by itself.
- Helot Militia has both FTO and non-FTO profiles. Only the FTO profiles are native members of the Varuna Fireteam row.
- The Undertow Montesa row is explicitly `FTO (Undertow)`; only the on-foot Montesa FTO loadout is used there. The separate Forward Montesa Duo row has no FTO restriction in the source.
- Clipper Dronbot appears as a Wildcard with an explicit `FTO` restriction; only Clipper option 5 is Wildcard-capable.
- Uma Sørensen appears as a Wildcard with an explicit `FTO` restriction and counts as both Fusilier and Kamau; only her FTO options are used for Fireteams.
- Quinn counts as both Fusilier and Kamau. Patsy Garnett counts as both Undertow and Helot. Bipandra counts as Fusilier. Machinist Varuna Div counts as Kamau in Undertow.
- The structured `required: true` rows are preserved as required-choice sets; this file does not reinterpret them as requiring every marked unit type simultaneously.
- Parenthetical Army-chart comments such as `(Fusilier, Kamau)` and `(Undertow, Helot)` are Counts-as / equivalence labels, not join-scope restrictions.
- Linked Reinforcement section: **Code: Capital** (`army_id: 199`). No Reinforcement Fireteam rows are merged into the main chart here.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Varuna Immediate Reaction Division |
| Parent faction | PanOceania |
| Army ID | 105 |
| Army metadata | `discontinued: true` |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 27 |
| Optional-mode units | Indigo Spec-Ops; Indigo Team-Ops |
| Reinforcement roster | Code: Capital (`199`) |
| Fireteam limits | Core 1; Haris 1; Duo unlimited |
| Fireteam chart | yes |

## Roster index

| Unit | ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| Sierra Dronbot | 17 | 2 | REM | Regular | — |
| Croc Men | 13 | 4 | SK | Regular | — |
| Mulebots | 38 | 2 | REM | Regular | — |
| Echo-Bravo Rapid Reaction Unit | 1214 | 3 | LI | Regular | — |
| Kamau Amphibious Intervention Teams | 48 | 5 | LI | Regular | Varuna; Undertow required-choice; Cavalry |
| Clipper Dronbot | 18 | 2 | REM | Regular | Wildcard, FTO option only |
| Tech-Bees | 935 | 1 | LI | Regular | — |
| ORC Troops, Varuna Division | 5 | 5 | HI | Regular | Varuna; Undertow required-choice |
| Knights of Montesa | 28 | 2 | HI | Regular + Impetuous | Undertow FTO; Forward Montesa Duo |
| Palbots | 37 | 2 | REM | Peripheral | — |
| Cutters | 12 | 2 | TAG | Regular | — |
| Trauma-Docs | 14 | 1 | LI | Regular | — |
| Peacemaker Armbots | 36 | 1 | REM | Regular | — |
| Richard Quinn | 1490 | 1 | LI | Regular | Wildcard; counts as Fusilier and Kamau |
| Helot Militia | 1222 | 3 | LI | Irregular | Varuna required-choice, FTO profiles only |
| Patsy Garnett | 1225 | 1 | HI | Regular | Wildcard; counts as Undertow and Helot |
| Warcors | 50 | 1 | LI | Irregular | — |
| Motorized Knights of Montesa | 1209 | 2 | HI | Regular + Impetuous | Cavalry required-choice |
| Bulleteer Armbots | 35 | 2 | REM | Regular | Cavalry |
| Machinist Varuna Division | 15 | 2 | LI | Regular | Undertow; counts as Kamau |
| Fusilier Indigo Bipandra | 46 | 1 | LI | Regular | Varuna; counts as Fusilier |
| Pathfinder Dronbot | 16 | 2 | REM | Regular | Wildcard, max 2 |
| Squalos Mk-II | 1651 | 2 | TAG | Regular + Tactical Awareness | Cavalry required-choice |
| Fugazi Dronbots | 19 | 2 | REM | Regular | — |
| Fusiliers | 1 | T | LI | Regular | Varuna required-choice |
| Zulu-Cobra | 1216 | 3 | LI | Regular | — |
| Captain Uma Sørensen | 1491 | 1 | MI | Regular | Wildcard, FTO profiles only; counts as Fusilier and Kamau |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Indigo Spec-Ops | 1912 | Spec-Ops | Varuna Fireteam row, max 1 when Spec-Ops mode is in use |
| Indigo Team-Ops | 1926 | Team-Ops | No ordinary Varuna Fireteam row |

## Unit details

### Sierra Dronbot

**ID 17 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage, Total Reaction, 360º Visor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 1 | HMG, PARA CC Weapon (-3) | — |
| 2 | 18 | 0 | Thunderbolt (+1B), PARA CC Weapon (-3) | — |

### Croc Men

**ID 13 · AVA 4 · SK** — `MOV 10-10 | CC 14 | BS 12 | PH 12 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. X Visor, Camouflage, Hidden Deployment, Infiltration, Mimetism (-6), Surprise Attack (-3), Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 25 | 0 | Boarding Shotgun, Shock Mine, D-Charges, Silenced Pistol, CC Weapon | — |
| 3 | 29 | 1.5 | MULTI Sniper Rifle, Shock Mine, Silenced Pistol, CC Weapon | — |
| 4 | 33 | 0.5 | Combi Rifle, D-Charges, Shock Mine, Silenced Pistol, CC Weapon; Hacking Device | — |
| 5 | 26 | 0.5 | Boarding Shotgun, D-Charges, Shock Mine, Silenced Pistol, CC Weapon; Minelayer | — |
| 6 | 30 | 0 | Combi Rifle, Flash Pulse, D-Charges, Shock Mine, Silenced Pistol, CC Weapon; Deployable Repeater, Forward Observer | — |

### Mulebots

**ID 38 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 4`. Remote Presence, Courage, Baggage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | PARA CC Weapon (-3); Deactivator, Repeater | — |
| 2 | 14 | 0.5 | PARA CC Weapon (-3); EVO Hacking Device | — |
| 3 | 17 | 0 | Combi Rifle, PARA CC Weapon (-3); Repeater, Total Reaction | — |

### Echo-Bravo Rapid Reaction Unit

**ID 1214 · AVA 3 · LI** — `MOV 10-10 | CC 15 | BS 13 | PH 11 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`. Parachutist, Decoy (1), Terrain (Aquatic), Surprise Attack (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 0 | Boarding Shotgun (+1B), Light Rocket Launcher, Pistol, CC Weapon | — |
| 2 | 25 | 1 | Red Fury, Pistol, CC Weapon | — |
| 3 | 27 | 0 | Combi Rifle, Light Shotgun, WildParrot, Pistol, CC Weapon; Paramedic, MediKit | — |
| 4 | 26 | 0.5 | Combi Rifle, Panzerfaust, Pistol, CC Weapon; Hacking Device | — |

### Kamau Amphibious Intervention Teams

**ID 48 · AVA 5 · LI** — `MOV 15-5 | CC 15 | BS 13 | PH 11 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 2`. Immunity (Shock), Mimetism (-3), Stealth, Terrain (Aquatic).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 20 | 0 | Combi Rifle, E/M Carbine, Silenced Pistol, CC Weapon | Varuna / Undertow / Cavalry |
| 2 | 26 | 1 | HMG, Silenced Pistol, CC Weapon | Varuna / Undertow / Cavalry |
| 3 | 22 | 0.5 | Submachine Gun, Silenced Pistol, CC Weapon; Hacking Device, FastPanda | Varuna / Undertow / Cavalry |
| 4 | 25 | 0 | Combi Rifle, E/M Carbine, Silenced Pistol, CC Weapon; Paramedic, MediKit, Tactical Awareness | Varuna / Undertow / Cavalry |
| 5 | 23 | 1.5 | Heavy Rocket Launcher, Submachine Gun, Silenced Pistol, CC Weapon; MSV1 | Varuna / Undertow / Cavalry |
| 6 | 29 | 1.5 | MULTI Sniper Rifle, Silenced Pistol, CC Weapon; MSV2 | Varuna / Undertow / Cavalry |
| 7 | 23 | 0 | MULTI Rifle, Flash Pulse, Silenced Pistol, CC Weapon; Forward Observer, Sensor, Triangulated Fire | Varuna / Undertow / Cavalry |
| 9 | 20 | 0 | Combi Rifle, E/M Carbine, Silenced Pistol, CC Weapon; Lieutenant | Varuna / Undertow / Cavalry |

### Clipper Dronbot

**ID 18 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 1.5 | Missile Launcher (Guided), PARA CC Weapon (-3) | — |
| 5 | 19 | 1.5 | **CLIPPER DRONBOT FTO** — Missile Launcher (+1B), PARA CC Weapon (-3) | Wildcard only |

### Tech-Bees

**ID 935 · AVA 1 · LI** — `MOV 10-10 | CC 12 | BS 11 | PH 10 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 2`. Specialist Operative, TAGCom; Deactivator, GizmoKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 9 | 0 | Adhesive Launcher Rifle, Flash Pulse, Pistol, PARA CC Weapon (-3); Deployable Repeater | — |

### ORC Troops — Varuna Division

**ID 5 · AVA 5 · HI** — `MOV 15-5 | CC 15 | BS 14 | PH 14 | WIP 12 | ARM 4 | BTS 3 | W 2 | S 2`. Varuna profiles add Stealth, Terrain (Aquatic/Jungle), Warhorse.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 13 | 36 | 1.5 | Feuerbach, Pistol, CC Weapon | Varuna / Undertow |
| 14 | 28 | 0 | Boarding Shotgun (+1B), Pistol, CC Weapon; TinBot: Firewall (-3) | Varuna / Undertow |
| 15 | 30 | 0 | MULTI Rifle, Pistol, CC Weapon; TinBot: Firewall (-3) | Varuna / Undertow |
| 16 | 35 | 1.5 | HMG, Pistol, CC Weapon | Varuna / Undertow |
| 17 | 34 | 0.5 | MULTI Rifle, Pistol, CC Weapon; Hacking Device | Varuna / Undertow |
| 18 | 35 | 1 | HMG, Pistol, CC Weapon; Lieutenant | Varuna / Undertow |
| 23 | 30 | 0 | MULTI Rifle, Pistol, CC Weapon; TinBot: Firewall (-3), Lieutenant | Varuna / Undertow |

### Knights of Montesa

**ID 28 · AVA 2 · HI** — `MOV 10-10 | CC 23 | BS 13 | PH 13 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 2`. Martial Arts L2, Limited Cover, Terrain (Aquatic/Jungle), BS Attack (+1SD), Mimetism (-3), Religious Troop, Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 32 | 1.5 | Red Fury, Boarding Pistol, DA CC Weapon (PS=6); Forward Deployment (+20) | Forward Montesa only |
| 3 | 26 | 0 | Boarding Shotgun, Boarding Pistol, DA CC Weapon (PS=6); Paramedic, Forward Deployment (+20) | Forward Montesa only |
| 5 | 20 | 0 | **KNIGHTS OF MONTESA FTO** — Boarding Shotgun, Blitzen, Boarding Pistol, DA CC Weapon (PS=6); Paramedic | Undertow; Forward Montesa |
| 6 | 35 | 1.5 | Spitfire, Drop Bears, Boarding Pistol, DA CC Weapon (PS=6); Forward Deployment (+20) | Forward Montesa only |

### Palbots

**ID 37 · AVA 2 · REM Peripheral** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Peripheral (Servant), Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | PARA CC Weapon (-3) | — |

### Cutters, Varuna Naval Chasseurs

**ID 12 · AVA 2 · TAG** — `MOV 15-10 | CC 18 | BS 15 | PH 15 | WIP 12 | ARM 8 | BTS 6 | W 3 | S 7`. ECM: Guided (-6), Camouflage, Hidden Deployment, Surprise Attack (-3), Mimetism (-6), Remote Presence, Courage, Dodge (PH=11), GizmoKit (PH=13), Terrain (Aquatic), BS Attack (SR-1).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 97 | 2 | MULTI HMG, CC Weapon (PS=5); NCO; Crabbot | — |
| 2 | 95 | 2.5 | MULTI HMG, CC Weapon (PS=5); Lieutenant; Crabbot | — |

### Trauma-Docs

**ID 14 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. Doctor, MediKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Pistol, CC Weapon | — |

### Peacemaker Armbots

**ID 36 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Repeater, Remote Presence, Courage, Forward Deployment (+20), Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Heavy Shotgun, Pulzar, PARA CCW (-3); AUXBOT_3 | — |
| 3 | 24 | 0.5 | Heavy Shotgun, Pulzar, PARA CCW (-3); AUXBOT_3B with Minelayer | — |
| 4 | 23 | 0 | Boarding Shotgun, Pulzar, PARA CCW (-3); BS Attack (+1B); no Auxbot | — |
| 5 | 27 | 0 | Boarding Shotgun, Pulzar, PARA CCW (-3); BS Attack (+1B); AUXBOT_3 | — |

### Fusilier Indigo Richard Quinn

**ID 1490 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 13 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. MSV1, Warhorse, Immunity (ARM).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 0 | MULTI Marksman Rifle, Flash Pulse, D-Charges, Boarding Pistol (+1B), CC Weapon; Forward Observer | Wildcard; counts as Fusilier and Kamau |
| 3 | 26 | 0 | MULTI Rifle, Flash Pulse, D-Charges, Disco Baller, Boarding Pistol (+1B), CC Weapon; Forward Observer | Wildcard; counts as Fusilier and Kamau |

### Helot Militia

**ID 1222 · AVA 3 · LI** — `MOV 10-10 | CC 12 | BS 11 | PH 10 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular, No Cube, Immunity (Shock), Neurocinetics, Terrain (Aquatic), Stealth.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 11 | 0 | **HELOT MILITIAMAN FTO** — Shock Marksman Rifle, Pistol, CC Weapon; Sensor | Varuna only |
| 3 | 13 | 1 | **HELOT MILITIAMAN FTO** — Red Fury, Pistol, CC Weapon; Sensor | Varuna only |
| 4 | 10 | 0 | **HELOT MILITIAMAN FTO** — Submachine Gun, Light Rocket Launcher, Pistol, CC Weapon; Sensor | Varuna only |
| 5 | 13 | 0 | Shock Marksman Rifle, Pistol, CC Weapon; Camouflage (1 Use), Surprise Attack (-3) | — |
| 6 | 17 | 1.5 | MULTI Sniper Rifle, Pistol, CC Weapon; Camouflage (1 Use), Surprise Attack (-3) | — |
| 7 | 15 | 1 | Red Fury, Pistol, CC Weapon; Camouflage (1 Use), Surprise Attack (-3) | — |
| 8 | 12 | 0 | Submachine Gun, Light Rocket Launcher, Pistol, CC Weapon; Camouflage (1 Use), Surprise Attack (-3) | — |

### Patsy Garnett

**ID 1225 · AVA 1 · HI** — `MOV 15-5 | CC 19 | BS 14 | PH 14 | WIP 13 | ARM 4 | BTS 3 | W 2 | S 2`. Warhorse, Forward Observer, Stealth, NCO, Terrain (Total), FT Master (Helots).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 34 | 0 | AP Submachine Gun, E/Mitter, Grenades, D-Charges, Flash Pulse, Pistol, Shock CC Weapon (PS=6) | Wildcard; counts as Undertow and Helot |

### Warcors

**ID 50 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular, Journalist.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CC Weapon (-3); 360º Visor | — |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CC Weapon (-3); Sixth Sense | — |

### Motorized Knights of Montesa

**ID 1209 · AVA 2 · HI** — `MOV 20-15 | CC 23 | BS 13 | PH 13 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 4`. Motorcycle, Martial Arts L2, Limited Cover, Dodge (+2.5), Immunity (Shock), Mimetism (-3), Religious Troop, Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | Boarding Shotgun, Boarding Pistol, DA CC Weapon (PS=6) | Cavalry required-choice |
| 2 | 26 | 0 | MULTI Rifle, Boarding Pistol, DA CC Weapon (PS=6) | Cavalry required-choice |
| 3 | 29 | 1 | Red Fury, Boarding Pistol, DA CC Weapon (PS=6) | Cavalry required-choice |
| 4 | 23 | 0 | Boarding Shotgun, Boarding Pistol, DA CC Weapon (PS=6); Paramedic, MediKit | Cavalry required-choice |

### Bulleteer Armbots

**ID 35 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Repeater, Remote Presence, Courage, Mimetism (-6).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Heavy Shotgun (+1B), PARA CC Weapon (-3) | Cavalry max 1 |
| 2 | 22 | 1 | Spitfire, PARA CC Weapon (-3) | Cavalry max 1 |

### Machinist — Varuna Division

**ID 15 · AVA 2 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`. Engineer, Deactivator, GizmoKit. Varuna profiles add Mimetism (-3), Stealth, Terrain (Aquatic).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 3 | 17 | 0 | Combi Rifle, D-Charges, Pistol, CC Weapon | Undertow; counts as Kamau |
| 19 | 18 | 0 | Combi Rifle, D-Charges, Pistol, CC Weapon; Deployable Cover | Undertow; counts as Kamau |
| 20 | 20 | 0 | Combi Rifle, D-Charges, Armed Turret (Combi Rifle), Pistol, CC Weapon | Undertow; counts as Kamau |

### Fusilier Indigo Bipandra

**ID 46 · AVA 1 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Doctor (ReRoll -3), Dodge (+2.5), Immunity (Shock).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Combi Rifle, Nanopulser (+1B), Pistol, CC Weapon; MediKit (+1B) | Varuna; counts as Fusilier |
| 2 | 25 | 0 | Combi Rifle, Nanopulser, Pistol, CC Weapon; MediKit (+1B), Tactical Awareness | Varuna; counts as Fusilier |

### Pathfinder Dronbot

**ID 16 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage, Forward Observer, Sensor, Triangulated Fire; Deactivator, Repeater.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Flash Pulse, PARA CC Weapon (-3) | Wildcard, max 2 |
| 2 | 17 | 0 | Combi Rifle, Flash Pulse, PARA CC Weapon (-3); Tactical Awareness | Wildcard, max 2 |

### Squalos Mk-II

**ID 1651 · AVA 2 · TAG** — `MOV 15-10 | CC 18 | BS 15 | PH 15 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`. ECM: Guided (-6), BS Attack (SR-1), Courage, Dodge (+2.5), Dodge (PH=11), GizmoKit (PH=13), Combat Instinct, Remote Presence, Tactical Awareness.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 55 | 1 | MULTI Marksman Rifle, MULTI Pistol (+1B), CC Weapon (PS=5); Crabbot | Cavalry required-choice |
| 2 | 62 | 1.5 | HMG, Grenade Launcher, MULTI Pistol (+1B), CC Weapon (PS=5); Crabbot | Cavalry required-choice |
| 3 | 66 | 1.5 | MULTI HMG, MULTI Pistol (+1B), CC Weapon (PS=5); NCO; Crabbot | Cavalry required-choice |

### Fugazi Dronbots

**ID 19 · AVA 2 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Remote Presence, Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | Flash Pulse, PARA CC Weapon (-3) | — |

### Fusiliers

**ID 1 · AVA T · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 10 | 0 | Combi Rifle, Pistol, CC Weapon | Varuna required-choice |
| 2 | 18 | 1 | HMG, Pistol, CC Weapon | Varuna required-choice |
| 4 | 15 | 1.5 | Missile Launcher, Pistol, CC Weapon | Varuna required-choice |
| 5 | 16 | 1 | MULTI Sniper Rifle, Pistol, CC Weapon | Varuna required-choice |
| 6 | 15 | 0.5 | Combi Rifle, Pistol, CC Weapon; Hacking Device | Varuna required-choice |
| 8 | 12 | 0 | Combi Rifle, Flash Pulse, Pistol, CC Weapon; Deployable Repeater, Forward Observer | Varuna required-choice |
| 9 | 12 | 0 | Combi Rifle, Pistol, CC Weapon; Paramedic, MediKit | Varuna required-choice |
| 10 | 10 | 0 | Combi Rifle, Pistol, CC Weapon; Lieutenant | Varuna required-choice |
| 12 | 12 | 0 | Combi Rifle, Pistol, CC Weapon; Commlink (+1), Specialist Operative | Varuna required-choice |

### Zulu-Cobra

**ID 1216 · AVA 3 · LI** — `MOV 10-10 | CC 14 | BS 13 | PH 11 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Camouflage, Surprise Attack (-3), Forward Deployment (+10), Mimetism (-3), Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 27 | 1 | Spitfire, Assault Pistol, E/M Mine, CC Weapon | — |
| 2 | 23 | 0 | Combi Rifle, Jammer, Assault Pistol, CC Weapon; Sensor, Triangulated Fire | — |
| 3 | 26 | 0 | Breaker Combi Rifle, Pitcher, Assault Pistol, CC Weapon; Killer Hacking Device | — |
| 4 | 24 | 0 | Breaker Combi Rifle, Flash Pulse, Assault Pistol, CC Weapon; Forward Observer | — |
| 5 | 23 | 0 | Combi Rifle, Jammer, Assault Pistol, CC Weapon; Lieutenant, Sensor, Triangulated Fire | — |
| 6 | 26 | 0.5 | MULTI Marksman Rifle, E/M Mine, Assault Pistol, CC Weapon; X Visor, Minelayer | — |

### Captain Uma Sørensen

**ID 1491 · AVA 1 · MI** — `MOV 10-10 | CC 15 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Immunity (Shock), Combat Instinct, Mimetism (-3), Specialist Operative, Stealth, Terrain (Total), Climbing Plus.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 27 | 0 | Submachine Gun (+1B), E/M Mine, Silenced Pistol (+1B), CC Weapon; Camouflage, Surprise Attack (-3), Forward Deployment (+20) | — |
| 2 | 25 | 0 | **UMA SØRENSEN FTO** — Breaker Combi Rifle, Silenced Pistol (+1B), CC Weapon; X Visor | Wildcard; counts as Fusilier and Kamau |
| 3 | 23 | 0 | **UMA SØRENSEN FTO** — Submachine Gun (+1B), E/M Mine, Silenced Pistol (+1B), CC Weapon; X Visor | Wildcard; counts as Fusilier and Kamau |
| 4 | 25 | 0 | **UMA SØRENSEN FTO** — Breaker Combi Rifle, Silenced Pistol (+1B), CC Weapon; X Visor, Lieutenant | Wildcard; counts as Fusilier and Kamau |

## Fireteam chart limits

| Constraint | Value |
|---|---|
| Core | 1 |
| Haris | 1 |
| Duo | unlimited (`256` in Army chart) |
| Main/Reinforcement mixing | not merged; use the separate Reinforcement chart |

## Fireteams

### FT-VAR-01 — Varuna Fireteams

**Types:** Core, Haris, Duo

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Fusilier | 1 | 0 | 5 | Yes | — | — |
| Helot Militiaman | 1222 | 0 | 2 | Yes | — | **FTO options 1, 3, 4 only** |
| Kamau | 48 | 0 | 3 | No | — | — |
| ORC Varuna Division | 5 | 0 | 2 | No | — | — |
| Bipandra | 46 | 0 | 1 | No | Fusilier | — |
| Indigo | 1912 | 0 | 1 | No | Spec-Ops | Optional Spec-Ops mode |

Fusilier and Helot FTO are both marked `required: true` in the structured chart; they form the source required-choice set rather than this reference asserting that both unit types must be present simultaneously.

### FT-VAR-02 — Undertow Fireteams

**Types:** Core, Haris, Duo

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| ORC Varuna Division | 5 | 0 | 5 | Yes | Undertow | — |
| Kamau | 48 | 0 | 5 | Yes | Undertow | — |
| Knight of Montesa | 28 | 0 | 2 | No | Undertow | **FTO option 5 only** |
| Machinist Varuna Division | 15 | 0 | 2 | No | Kamau | — |

ORC Varuna and Kamau are both marked `required: true` in the structured chart; they form the source required-choice set rather than requiring both unit types simultaneously.

### FT-VAR-03 — Cavalry Fireteams

**Type:** Duo

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Squalos Mk-II | 1651 | 0 | 2 | Yes | — | — |
| Motorized Knight of Montesa | 1209 | 0 | 2 | Yes | — | — |
| Bulleteer | 35 | 0 | 1 | No | — | — |
| Kamau | 48 | 0 | 1 | No | — | — |

Squalos Mk-II and Motorized Montesa are both marked `required: true` in the structured chart; they form the source required-choice set.

### FT-VAR-04 — Forward Montesa Fireteams

**Type:** Duo

| Member | Unit ID | Min | Max | Required | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Knight of Montesa | 28 | 2 | 2 | No | — | none in source row |

The source row requires exactly two Knights of Montesa and does not carry an FTO marker. This is distinct from the FTO-restricted Montesa row in Undertow.

### Wildcards

All rows below are in the chart's **Wildcards** row. Parenthetical values are Counts-as labels, not join-scope restrictions.

| Wildcard | Unit ID | Max | Counts as | FTO/profile restriction |
|---|---:|---:|---|---|
| Pathfinder Dronbot | 16 | 2 | — | all |
| Clipper Dronbot | 18 | 1 | — | **FTO option 5 only** |
| Richard Quinn | 1490 | 1 | Fusilier, Kamau | all Quinn loadouts |
| Uma Sørensen | 1491 | 1 | Fusilier, Kamau | **FTO options 2, 3, 4 only** |
| Patsy Garnett | 1225 | 1 | Undertow, Helot | all |

Wildcard status does not remove the native minimum/required-choice conditions of the Fireteam being joined.

## Unit → Fireteam access index

| Unit | Fireteam access |
|---|---|
| Sierra Dronbot | — |
| Croc Man | — |
| Mulebot | — |
| Echo-Bravo | — |
| Kamau | FT-VAR-01 max 3; FT-VAR-02 required-choice max 5/counts as Undertow; FT-VAR-03 max 1 |
| Clipper | Wildcard max 1, **FTO option 5 only** |
| Tech-Bee | — |
| ORC Varuna Division | FT-VAR-01 max 2; FT-VAR-02 required-choice max 5/counts as Undertow |
| Knight of Montesa | FT-VAR-02 max 2/counts as Undertow/**FTO option 5 only**; FT-VAR-04 exactly 2/no FTO restriction in source |
| Palbot | — |
| Cutter | — |
| Trauma-Doc | — |
| Peacemaker | — |
| Richard Quinn | Wildcard max 1; counts as Fusilier and Kamau |
| Helot Militiaman | FT-VAR-01 required-choice max 2, **FTO options 1/3/4 only** |
| Patsy Garnett | Wildcard max 1; counts as Undertow and Helot |
| Warcor | — |
| Motorized Knight of Montesa | FT-VAR-03 required-choice max 2 |
| Bulleteer | FT-VAR-03 max 1 |
| Machinist Varuna Division | FT-VAR-02 max 2; counts as Kamau |
| Bipandra | FT-VAR-01 max 1; counts as Fusilier |
| Pathfinder | Wildcard max 2 |
| Squalos Mk-II | FT-VAR-03 required-choice max 2 |
| Fugazi | — |
| Fusilier | FT-VAR-01 required-choice max 5 |
| Zulu-Cobra | — |
| Uma Sørensen | Wildcard max 1, **FTO options 2/3/4 only**; counts as Fusilier and Kamau |
| Indigo Spec-Ops | FT-VAR-01 max 1 when Spec-Ops mode is used |
| Indigo Team-Ops | — |

## Derived tactical index

These tags are analytical conveniences for modular list-building, not Army characteristics.

| Unit / profile | Tactical tags |
|---|---|
| Fusiliers | cheerleader, specialist, long-range ARO, hacker, network projection |
| Kamau | long-range attack, long-range ARO, mid-range attack, specialist, hacker, tech-counter |
| ORC Varuna | long-range attack, mid-range attack, hacker, tech-counter |
| Helot Militia | long-range ARO, mid-range ARO, DZ defense, midfield defense |
| Richard Quinn | mid-range attack, specialist, tech-counter |
| Bipandra | specialist, medical support |
| Patsy Garnett | mid-range attack, specialist, Lieutenant-order support, close assault |
| Uma Sørensen | midfield specialist, midfield defense, close assault, Lieutenant option |
| Zulu-Cobra | midfield specialist, midfield defense, hacker, KHD, network projection, tech-counter |
| Croc Men | midfield specialist, midfield defense, hacker, network projection, long-range ARO |
| Echo-Bravo | airborne, enemy-DZ attacker, specialist, hacker |
| Cutter | TAG support, long-range attack, enemy-DZ attacker, Lieutenant/NCO option |
| Squalos Mk-II | TAG support, long-range attack, mid-range attack, Lieutenant-order support |
| Motorized Montesa | close assault, specialist, enemy-DZ attacker |
| Knight of Montesa | close assault, midfield specialist, mid-range attack |
| Sierra | long-range ARO, REM support |
| Clipper | long-range attack, guided attack, REM support |
| Bulleteer | mid-range attack, REM support, network projection |
| Peacemaker | midfield attack, midfield defense, network projection, REM support |
| Pathfinder | midfield specialist, network projection, tech-counter, REM support |
| Fugazi | cheerleader, network projection, REM support |
| Mulebot | cheerleader, REM support, hacker, network projection, baggage |
| Machinist Varuna | specialist, TAG support, REM support, tech-counter |
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
- Standard roster count validated from source-faction membership: **27** logical units, excluding optional Indigo Spec-Ops/Team-Ops and Soldier of Fortune entries with empty faction membership.
- Canonical Fireteam chart validated against the source `fireteamChart`: 4 native team rows + Wildcards; limits Core 1 / Haris 1 / Duo unlimited.
- All Fireteam maximums, required-choice flags, Counts-as labels, and explicit FTO markers are preserved.
- Profile-restricted Fireteam access is explicitly represented for Helot FTO, Knight of Montesa FTO in Undertow, Clipper FTO, and Uma Sørensen FTO.
- Forward Montesa is represented separately as an exact two-Montesa Duo with no FTO marker in the source row.
- Quinn's Fusilier/Kamau equivalence, Uma's Fusilier/Kamau equivalence, Patsy's Undertow/Helot equivalence, Bipandra's Fusilier equivalence, and Machinist Varuna's Kamau equivalence are preserved.
- Main and Reinforcement charts are not merged.
