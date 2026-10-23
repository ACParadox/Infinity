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


## Community tactics from N5 video/podcast transcripts (reviewed 2026-10-19)

For detailed profile-by-profile choices, Fireteam architectures, defensive shell versus active-turn tradeoffs and annotated source leads, see the [Varuna N5.3 tactical and list-building guide](../../notes/factions/varuna.md). **Corrections:** current Varuna has no CoC profile; Quinn is not CoC. The roster and chart above are canonical.

**Evidence:** Opinions below come from N5-era creator transcripts (mostly October–December 2025), with cross-sectorial PanO REM material and one clearly marked historical podcast. **The current N5.3 profiles and Fireteams above take precedence over older speaker recollections.** This is tactical interpretation, not an alteration of roster rules.

### Winning with Varuna: a five-part checklist

1. **Layered ARO instead of a single sniper.** Combine Helots, Kamau visor/long guns, Montesa Blitzens, camo markers, mines, and potentially a Peacemaker. Opponents lose orders discovering or clearing several separate threats rather than winning one decisive FTF.
2. **Midfield scoring and pressure.** Zulu-Cobra KHD/Pitcher, foot Montesa, Croc Men, and advancing Undertow teams do the mission while the defense delays the opponent. Varuna's smaller, predictable roster makes redundancy and placement more useful than hoping to surprise an experienced opponent.
3. **A real answer to armored and Mimetism+MSV AROs.** ORC HMG/Feuerbach, Squalos, Cutter, or a line-of-fire solution such as Quinn's Disco Baller. Avoid depending solely on a Kamau sniper to win unfavourable protected lanes.
4. **Reach, not only denial.** Retrieval and enemy-zone missions punish Varuna's relatively slow infantry. Motorized Montesa, Echo-Bravo Parachutists, a TAG, or a carefully funded Guided plan can be necessary to chase a fleeing carrier or score far away.
5. **Orders, repairs and network discipline.** Tactical Awareness Pathfinders in legal teams, Squalos TA, Patsy's Helot Fireteam Master, and the Machinist turn valuable models into sustained progress. Do not expose your whole hacking network through an uncontrolled repeater.

### Building blocks — when to take them and why

| Pick | Good because | Cost / alternative |
|---|---|---|
| **Patsy + Helot FTOs** | Patsy's FT Master (Helots) makes linked Helots contribute Regularly; cheap Neurocinetics/Sensor guns support her NCO/FO advance. Red Fury can cover midrange; SMG/light rocket launcher is an economical close guard. | Helots die to quality gunfights; requires the **FTO** Helot profiles in a legal Varuna team. Keep an unlinked one-use Camo Helot if you want a concealed Discover tax instead. |
| **20pt foot Montesa FTO** | 2 Wounds, Mimetism (-3), Paramedic, boarding shotgun, Blitzen and BS Attack (+1SD) give an unusually cheap **assault plus mobile ARO** piece; Undertow team member. | Limited Cover is *not* full Cover; MSV can punish a careless exposed Knight. The separate exactly-two-foot-Montesa Forward Duo allows other profiles; non-FTO profiles do **not** enter Undertow. |
| **Zulu-Cobra KHD with Pitcher** | Camo, Forward Deployment, Surprise Attack and a mobile Pitcher deliver Pano's efficient specialist and attack-vector extension. Multiple transcript presenters consider it a near-default. | Network extension only matters with capable hackers/orders; the Pitcher can also create counter-hacking concerns. Jammer Camo LT and X-Visor Minelayer are credible alternatives for different jobs. |
| **Varuna ORC gun / Lieutenant** | BS14, 2W, ARM4, Stealth and Warhorse make ORC HMG/Feuerbach/Shotgun guns useful all game. Warhorse makes a MULTI Rifle+Firewall TinBot LT or HMG LT much less vulnerable to Isolation/Oblivion. | WIP12 and Immobilized/Carbonite remain relevant; anti-Isolation does not mean hack-proof. Exposing an ORC LT for routine shots still risks Loss of Lieutenant. |
| **Kamau visor or utility** | MSV2 MULTI Sniper / MSV1 HRL answers Mimetism; TA Paramedic, FO Sensor/Triangulated Fire and FastPanda Hacker fill specialist/repeater niches. | Some N5 hosts view ordinary Kamau shooting as inefficient compared with ORCs/TAGs; choose the **unique visor/skill**, not an automatic sniper obligation inherited from earlier editions. |
| **Quinn with Disco Baller** | Wildcard and line-of-sight/visibility control can bypass dangerous combinations of Mimetism and MSV instead of risking weak FTF odds; especially helpful **without a TAG**. | 26pts is a meaningful investment for one wound; a TAG or other control pieces may solve the same problem. A pre-N5 podcast rated Quinn poorly for different reasons. |
| **Croc Men / Echo-Bravo** | Hidden/Infiltration and mine/repeater specialists (Croc) or Parachutist+Decoy board-edge scoring and backfield threat (Echo-Bravo). | Neither is cheap enough to take without a job. Echo-Bravo is **not** a Combat Jump trooper; choose its deployment edge carefully. |

### Representative legal packages, not mandatory templates

- **Patsy + two Helot FTO Varuna Haris:** linked Helot Regular contribution plus overlapping FTO guns; optionally build a larger *legal* Varuna Core with allowed ORC/Kamau/Fusilier members. Pair with a separate Camo Helot for an unrevealed lane.
- **ORC + Varuna Machinist + Montesa FTO + two TA Pathfinders Undertow Core:** the two 17pt Pathfinders each contribute a Tactical Awareness order and also bring FO/Sensor, Deactivator and Repeaters. The Machinist repairs REMs; Montesa handles the approach and active/reactive close fighting. Spread the repeater wall **after** reaching the relevant lane, without gifting easy hackers a path in.
- **ORC HMG/Feuerbach or Kamau visor + foot Montesa FTO and/or TA Pathfinder Undertow Duo/Haris:** smaller, specialized gun+escort or gun+order-delivery option when the five-model Core consumes too many points and slots.
- **Squalos Mk-II + TA Pathfinder Cavalry Duo:** Squalos's native TA plus a Pathfinder's TA creates an order-rich TAG/specialist delivery unit; the **Squalos MULTI HMG NCO** can also consume an available LT order. Alternative Squalos + Bulleteer Duo adds a midrange attacker/repeater. A Motorized Montesa + Bulleteer instead builds around raw speed. **Two Bulleteers alone are not a legal Varuna Cavalry Duo.**
- **LT choice:** Fusilier with a possible decoy saves points; Zulu-Cobra Jammer LT combines Camo deception and area control but risks exposure when active; ORC Warhorse LT costs more but is usable in an aggressive squad. Keep LT and an independent backstop from being taken out in the same attack when feasible.

### TAGs, motorcycles and REMs (PanO cross-sectorial findings)

**Varuna's current 27-unit roster has no separate Vehicle (VH) entry.** The relevant vehicles/fast models for playstyle discussion are **Cutter and Squalos TAGs** and the **Motorized Montesa (Motorcycle HI)**, alongside REMs. Other sectorials' vehicles and Fireteam permissions are **not** Varuna choices.

| Platform | Reasons to bring it | Limits and opposing opinion |
|---|---|---|
| **Cutter NCO — 97pts / 2 SWC** | BS15, ARM8, Mimetism (-6), Camo/Hidden Deployment and MULTI HMG make an excellent protected long-range problem-solver. Hidden threat influences opposing deployment; NCO can spend the LT order, and engineer support protects the sunk cost. | **No Tactical Awareness** in current roster. Huge S7, costly, fewer specialists/orders: Tactical Awareness hosts often prefer a Squalos/ORC package and warn to finish behind defenses/marker protection. Dante's Faction Focus strongly values Cutter's sheer threat. **Double Cutter** was mentioned as a novelty, not consensus best list. |
| **Squalos Mk-II — 55pt MMR; 62pt HMG+GL; 66pt MULTI HMG+NCO** | BS15, ARM6, BTS6, 3 STR and **Tactical Awareness on each loadout**. MMR is efficient flexible gun; HMG+grenade launcher pressures unusual angles or dug-in targets; NCO MULTI HMG offers dedicated long-gun punch plus LT order. A TA Pathfinder Duo increases forward efficiency. | No Cutter-level Mimetism/Camo, so avoid taking visible return fire without a plan. Some prefer cheap MMR or NCO gun; others like GL to touch rooftops/hidden cover. Mission/terrain decides. |
| **Motorized Montesa** | 20-15 movement provides a rare quick flanker, good for distant objectives or pursuing a stolen objective; legal Cavalry partner options. | S4 base, Impetuous and Limited Cover constrain routes; unlike foot FTO, lacks Blitzen and +1SD. Dante/Tactical Awareness often favor foot Montesa for efficient general-purpose fighting, motorized for *speed-required* missions. |
| **Bulleteer Spitfire / +1B Heavy Shotgun** | 15-10 fast, Mimetism (-6), Repeater. Spitfire is cost-effective midrange attack; +1B shotgun bullies targets **without** template retaliation. EVO Marksmanship may amplify it when EVO and an Engineer serve other REMs too. | S4 ARM1 can lose a trade easily; EVO+Engineer overhead negates cheapness if purchased only for one bot. Swiss Miss likes the Spitfire in vanilla, while Dante says Varuna's Cavalry links provide less upside than some other PanO sectorials. |
| **Peacemaker + Auxbot (23pts), Minelayer Auxbot (24pts/.5)** | Forward-deployed shotgun/Pulzar, template Auxbot, Repeater and optional extra mine establish a wide field of threat and hacking projection, especially around objective rooms. Useful if an opponent otherwise blinds defenders with Disco Ball and walks through. | The same exposed Repeater can let better enemy hackers attack *your own* hackers/network. Fat chassis and an uncertain gunfight make it **situational**, not an autopick. |
| **TA Pathfinder (17pts) / Fugazi (7pts) / Baggage Mulebot (8pts)** | Pathfinder Wildcards (max 2) supply sensor, FO, deactivator, repeater, and extra **Fireteam movement orders**. Fugazi are efficient flash/repeater Regular-order fillers. Baggage can reload limited kit including Montesa Blitzens, Quinn Disco Ballers and Zulu Pitchers. | Two TA Pathfinders shine in Varuna Fireteams; their value does *not* generalize to unlinked vanilla lists. The 14pt/.5 EVO Mulebot is more compelling with **multiple combat REMs**, not as automatic infrastructure. |
| **Sierra TR / Clipper** | Sierra HMG (23/1) or Thunderbolt (+1B, 18/0) provides a 360-degree independent ARO when team guns are elsewhere. Clipper 16/1.5 Guided ML can exploit network targeting and Spotlight, while its **19/1.5 FTO option 5** is a different Wildcard +1B Missile Launcher choice. | Sierra is visible, often less deceptive than Helots and less tailored than Kamau MSV ARO. Guided needs *actual* targeting and order/hacking investment; don't conflate regular Clipper Guided with its FTO loadout. |
| **Varuna Machinist / Palbot / Tech-Bee** | Engineer and Palbot support Cutter, Squalos and the whole REM group; Machinist in Undertow also contributes Fireteam utility. 9pt Tech-Bee adds cheap specialist, Deployable Repeater and TAGCom support. | With mostly LI/HI and few REMs, repair investment competes with objective bodies and doctor support. |

### What experts disagreed about

- **Cutter or Squalos?** Dante's Faction Focus and the older IGL podcast describe Cutter as a unique opponent-shaping powerhouse. N5 Tactical Awareness calls it dangerous but thin on orders (no TA), and suggests **Squalos+Bulleteer/Pathfinder or ORCs** can be a better *whole-list* allocation. This is **best FTF threat vs board coverage/order depth**, not a universal ranking.
- **Patsy/ORCs or TAGs?** The **Feb 2024 N4-era IGL** discussion called Patsy/ORCs situational compared with TAGs. **2025 N5** Tactical Awareness and Loss of Lieutenant regard Patsy+Helot FTO as defining, and Warhorse ORCs more viable. Changes in profiles/FT rules explain part of that difference.
- **Helots: FTO versus camo?** Linked FTOs yield regularity, active mobility and often reactive burst; unlinked one-use Camo markers force Discover and disguise the real Zulu/hidden plan. Best mix depends on whether the list needs orders or deception.
- **Kamau: staple or overpriced?** Some hosts say ORC toughness and firepower now undercut generic Kamau guns. Others still build around **MSV2 sniper / MSV1 HRL** or TA Paramedic for unique tools. Use a Kamau for a specific need, not a legacy autopick.
- **Quinn: useful Disco Baller or points sink?** Dante's 2025 recommendation is **Quinn or TAG** versus protected visor/Mimetism pieces. IGL's **2024** evaluation preferred Kamau guns and struggled to justify Quinn. Earlier assessment predates the N5 profile/vision-control use case.
- **Peacemaker: strong or risky?** Swiss Miss and NCA REM analysis praise minelayer/Auxbot/repeater midfield control. Dante warns the repeater is vulnerable to stronger enemy hacking. Both are right in different matchups.
- **Pathfinder disagreement is faction-specific:** Robert Shepherd's NCA analysis calls 17pt TA Wildcard Pathfinders almost too efficient; Dante uses them as core Varuna order engines. Swiss Miss was cooler on **vanilla PanO** Pathfinders, where the same Fireteam use is unavailable; do not mistake that for a Varuna verdict.

### Lessons from MEGA 2025 event report

Dante finished **5th of roughly 21–22** players and especially praised layered Helot defenses and 20pt foot Montesas. Against difficult matchups he wanted **more reach and heavier weapons**: moving into midfield is not the same as catching a retreating objective carrier. Practical corrections: protect rear approaches from Parachutists; check ARO lines at model/table level, not from above; double-cover crucial angles; keep flexible pieces alive for late classifieds. Suggested future options: **Motorized Montesa, Echo-Bravo or Guided**. This is one player's tournament experience, not a faction win-rate estimate.

### Ranked transcript-checked media

**Varuna-focused:**
1. [Infinity the Dante — Tournament Listbuilding for Varuna, N5](https://www.youtube.com/watch?v=U8igbhbj2iw) — tested team packages, mission conditions and detailed why.
2. [Tactical Awareness S3 E41 — Varuna (Nov 2025 podcast)](https://open.spotify.com/episode/4RsrJBsOlJ3qnkjW3HCmgU) ([YouTube mirror](https://www.youtube.com/watch?v=DLgSwYvTGS4)) — three list perspectives, Patsy/Helots, Cutter vs Squalos, ORC and REM options.
3. [Loss of Lieutenant #157 — Return of Lost Sectorials (Oct 2025 podcast; Varuna segment approx. 1h58–2h20)](https://open.spotify.com/episode/1lq0RhEWwpegXr1kkKJzUr) — new FTO Helot + Patsy, Montesa, KHD Pitchers and TA Pathfinders.
4. [Infinity the Dante — Varuna Tournament Report, MEGA 2025](https://www.youtube.com/watch?v=QaAXC5Y332E) — actual results, practical oversights and speed/gun deficiencies.
5. [Infinity the Dante — Varuna N5 Initial Reaction](https://www.youtube.com/watch?v=FiH3eVJVHP4) — new profiles, LT and Fireteam builds.
6. [Infinity the Dante — Varuna Faction Focus](https://www.youtube.com/watch?v=YPfLiJ8IKR0) — Cutter, Squalos/GL, order economics; **auto-translation transcript was imperfect** so rely on canonical data above for exact details.

**TAG/REM material from other PanO/vanilla (tactics transferable, membership not):**
7. [Infinity the Dante — Faction Combat Remotes Guide (N5)](https://www.youtube.com/watch?v=xxGJYtQr6CE) — Bulleteer, Peacemaker, support overhead and repeater vulnerability.
8. [Robert Shepherd — N5 Neoterran Capitaline Army Faction Focus](https://www.youtube.com/watch?v=axa19k7qE1E) — 17pt Pathfinder TA engine, Peacemaker and REM vs premium gun balance.
9. [Swiss Miss Gaming — N5 PanOceania Tier List](https://www.youtube.com/watch?v=EjN9xWKeBso) — other opinions on Bulleteer, Peacemaker, Pathfinder, Clipper and Sierra in **vanilla**.

**Historical context only:** [Infinity Global League E144 — Varuna (February 2024)](https://open.spotify.com/episode/2hwVv91Hdba2LxjKVt7ZS3); transcript checked for contrasting views, but N4 roster and Fireteam values are **not** valid current facts.

## TAG tactical cross-reference (2026-10-23)

**Cutter** uses Camo/Hidden Deployment/Mimetism to avoid fair ARO engagements and make opponents cover multiple lanes, but its ~95-point cost reduces the independent attack/scoring budget. **Squalos Mk-II** is the alternative value gun with TacAware and Cavalry access; choose NCO MULTI versus armored targets or GL for indirect solutions. Do not assume the Cutter itself has the Squalos' Fireteam option.

Cross-faction **apex vs points-value** comparisons, matchup table, and direct MCP-reviewed podcast/video sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Current profile and Fireteam legality above remain authoritative.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Zulu-Cobra Camo KHD/Pitcher 26/0** is the strong forward anti-Hacker/specialist option; **Kamau HD + FastPanda 22/0.5** moves HD threats into midfield from an appropriate team while **Fusilier HD 15/0.5** is cheap insurance. **Croc Men Hidden HD 33/0.5** buys surprise and objective access, not superior raw cyber output; **Echo-Bravo HD 26/0.5** brings Parachutist specialist angles. **Choice:** Zulu-Cobra protects Cutter/other hackable attackers from enemy KHDs, Kamau/Fusilier's **Oblivion/Carbonite** handles enemy HI/TAG; do not claim the KHD can do both.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

See [Cheerleaders and Order Generators — N5.3 apex, points-value and matchup guide](../../notes/list-building/cheerleaders-and-order-generators.md) for complete comparative tables and verified transcript disagreements. The **current roster above controls** legality, AVA, Training and Fireteams.

- 7pt Fugazi — Flash/Mimetism/Repeater mobile Regular Order, excellent only with a protected S3 slot and available AVA.
- 8pt Mulebot — Baggage/Re­peater Regular Order, excellent if support reloads are useful and S4 bases fit.
- Fusiliers — cheap small-base Regular line, suitable for mandatory Fireteams, Lieutenant uncertainty and guarded rear objectives.
- Helot — excellent cheap Irregular ARO/roadblock, but does not provide a normal Regular pool Order by default.
- Warcor — 3pt Irregular Flash Pulse distraction, not a transferable Regular Order.

**Order audit:** add up only deployed eligible **Regular** Orders in each Combat Group; special LT/Tactical, Irregular and Peripheral activations are not transferable pool Orders. Buy the cheapest protected body that supplies the *second function the list truly needs*; consider large-base DZ crowding, expensive mandatory Fireteam slots, and whether another scoring specialist beats one more cheap Order.


## ARO apex/value cross-reference (2026-10-23)

See [Best ARO Units — N5.3 apex and cost-value tiers](../../notes/list-building/aro-units-apex-and-value.md) for gunfighter vs hidden-trap vs cheap Order-tax comparisons, when each wins, transcript disagreements and counterplay. **The roster, prices/AVA and canonical Fireteam chart above remain authoritative**; a shared unit's permissions do not transfer between armies.

- **Sierra Thunderbolt TR** — 18pt/0SWC multi-arc Regular ARO where profile legal; add Engineer/recovery if its lane matters repeatedly
- **Kamau MSV2 sniper / MSV1 HRL** — visored ranged denial and legal Fireteam support; fragile W1 if isolated
- **Helot Camo(1-use) LRL** — cheap, normally Irregular marker/template trap; value from target choice and delayed movement, not shared Orders
- **Warcor Flash Pulse** — 3pt Irregular zero-SWC Order-tax ARO; never count as a generic Regular Order
- **Fugazi Flash/Repeater** — 7pt Regular cheap secondary ARO and hacking net; not a main gun

**Deployment choice:** put the disposable/tax ARO on the approach, preserve a separate hidden/mission-denial gate where legal, and avoid leaving an expensive active-turn gun as your only exposed defence. Test pie-slicing, Smoke/Eclipse/White Noise, hacking, AD entry, recovery access and specialist survival before paying more SWC for a second sniper.
