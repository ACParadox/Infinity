---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 107
sectorial_slug: kestrel-colonial-force
sectorial_name: Kestrel Colonial Force
parent_faction: PanOceania
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Kestrel roster, standard loadouts, canonical Fireteam chart, and reverse Fireteam index. Spec-Ops and Team-Ops are represented as optional-mode hooks rather than expanded as ordinary matched-play roster entries."
---

# Kestrel Colonial Force

## Overview and provenance

This file is the repository-native reference for **Kestrel Colonial Force** roster, profile, points/SWC, AVA, and Fireteam questions.

Primary data basis:

- Corvus Belli Army-derived Kestrel source revision: `7.26246.158`.
- Historical/current N5.3 snapshot: `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- InfinityDB normalization / Fireteam semantics cross-check: commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

### Coverage rules

- This reference covers the **standard Kestrel matched-play roster** and the complete Kestrel `fireteamChart` present in the pinned Army source.
- Optional Soldier of Fortune entries whose source faction list is empty are **not** part of the base Kestrel roster and are excluded.
- `Indigo Spec-Ops` and `Indigo Team-Ops` are optional game-mode content. They are recorded where relevant, but are not treated as ordinary matched-play units for roster-completeness purposes.
- An `FTO` label on a profile does **not** by itself grant Fireteam access. Fireteam legality comes from the canonical chart below. Yamabushi is the important Kestrel example: it has FTO-labelled options but no Kestrel Fireteam chart row.
- The Kestrel Army document links Reinforcement section **Code: Capital** (`army_id: 199`). The pinned Code: Capital Army document does not expose a `fireteamChart`, so no Reinforcement Fireteam rows are merged into this file.

## Roster index

| Unit | Unit ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| Sierra Dronbot | 17 | 2 | REM | Regular | — |
| Clipper Dronbot | 18 | 1 | REM | Regular | — |
| Fugazi Dronbot | 19 | 1 | REM | Regular | — |
| Scarecrows Active Recon Group | 1812 | 3 | SK | Regular | — |
| Fennec Fusiliers | 1803 | 5 | LI | Regular | FENNECS native |
| Fireflies Clandestine Demo Squad | 1809 | 5 | MI | Regular | KESTREL native; ARMORED optional |
| Peacemaker Armbots | 36 | 2 | REM | Regular | — |
| Tech-Bees | 935 | 1 | LI | Regular | — |
| Redeye Close Air Support Squad | 1816 | 2 | VH | Regular | — |
| Pathfinder Dronbot | 16 | 2 | REM | Regular | Wildcard, max 1 |
| Palbots | 37 | 2 | REM | Peripheral | — |
| Blink Team | 1805 | 2 | LI | Regular | — |
| BCA Magistrates | 1804 | 2 | LI | Regular | FENNECS; COLCORP |
| Beasthunters Free Guild | 1570 | 1 | SK | Irregular | COLCORP, FTO profile only |
| Black A.I.R. | 1808 | 3 | MI | Regular | FENNECS, FTO profiles only |
| Father Lucien Sforza | 198 | 1 | MI | Regular | Wildcard, FTO profiles only |
| Trauma-Docs | 14 | 1 | LI | Regular | — |
| Mulebots | 38 | 2 | REM | Regular | — |
| Minescorp Jackals | 1813 | 4 | LI | Irregular | COLCORP, FTO profiles only |
| Yamabushi | 1824 | 2 | WB | Regular | —; FTO label alone grants no access |
| Richard Quinn | 1490 | 1 | LI | Regular | Wildcard: FENNECS / KESTREL |
| Tikbalangs | 33 | 2 | TAG | Regular | ARMORED native |
| Machinists | 15 | 1 | LI | Regular | — |
| Emily Handelman | 1072 | 1 | LI | Regular | Wildcard: FENNECS / COLCORP |
| Optimate Agent Maximus | 1862 | 1 | MI | Regular | FENNECS |
| Bulleteer Armbots | 35 | 2 | REM | Regular | ARMORED optional |
| Drummers Mobile Support Section | 1806 | 4 | LI | Regular | — |
| Team Crux Father-Knights | 1815 | 1 | HI | Regular | Wildcard, FTO profiles only |
| Hetkari Shooters | 1811 | 2 | HI | Regular | KESTREL native |
| Griffin Troops | 1810 | 3 | HI | Regular | FENNECS / KESTREL |
| Bipandra | 46 | 1 | LI | Regular | Wildcard: FENNECS / KESTREL |
| Squalos Mk-II | 1651 | 2 | TAG | Regular | ARMORED native |
| Banshees Airborne Assault Unit | 1807 | 3 | MI | Regular | — |
| Dr. Priya Harper | 1814 | 1 | LI | Regular | Wildcard, FTO profile only |
| Knauf | 939 | 1 | LI | Regular | — |
| Warcors | 50 | 1 | LI | Irregular | — |
| Maximus, Optimate and HexaDome Legend | 1720 | 1 | TAG | Regular | ARMORED optional |
| Dart, Optimate Huntress | 1130 | 1 | SK | Regular | — |
| Sāchā Xenotech Hunters | 1874 | 1 | LI | Irregular | — |
| Kazurabā Ruby Monday | 1890 | 1 | HI | Irregular | — |

Optional mode entries:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Indigo Spec-Ops | 1912 | Spec-Ops | May occupy the `INDIGO (Spec-Ops)` FENNECS row when that game mode is in use |
| Indigo Team-Ops | 1926 | Team-Ops | Mode-specific roster content; no ordinary Kestrel Fireteam row |

## Unit details

### Sierra Dronbot

**ID 17 · AVA 2 · REM · Support Troop**

`MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`

Skills/equipment: Remote Presence, Courage, Total Reaction, 360º Visor.

| Option | Pts | SWC | Loadout / profile notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 23 | 1 | HMG; PARA CCW (-3) | — |
| 2 | 18 | 0 | Thunderbolt (+1B); PARA CCW (-3) | — |

### Clipper Dronbot

**ID 18 · AVA 1 · REM · Support Troop**

`MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`

Skills/equipment: Remote Presence, Courage.

| Option | Pts | SWC | Loadout / profile notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 16 | 1.5 | Missile Launcher, Guided; PARA CCW (-3) | — |
| 5 | 19 | 1.5 | **CLIPPER DRONBOT FTO**; Missile Launcher (+1B); PARA CCW (-3) | —; no Kestrel chart row |

### Fugazi Dronbot

**ID 19 · AVA 1 · REM · Support Troop**

`MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`

Skills/equipment: Repeater, Remote Presence, Courage, Mimetism (-3).

| Option | Pts | SWC | Loadout | Fireteam |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | Flash Pulse; PARA CCW (-3) | — |

### Scarecrows Active Recon Group

**ID 1812 · AVA 3 · SK · Specially Trained**

`MOV 10-10 | CC 15 | BS 13 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`

Skills: Surprise Attack (-3), Camouflage, Hidden Deployment, Infiltration, Mimetism (-6), Stealth, Terrain (Total).

| Option | Pts | SWC | Loadout / role | Fireteam |
|---:|---:|---:|---|---|
| 1 | 26 | 0 | Boarding Shotgun, Nanopulser, D-Charges, Silenced Pistol, CCW; Deployable Repeater | — |
| 2 | 29 | 0.5 | SMG, Nanopulser, D-Charges, Silenced Pistol, CCW; Hacking Device | — |
| 3 | 27 | 0 | SMG, Nanopulser, D-Charges, Silenced Pistol, CCW; Killer Hacking Device | — |
| 4 | 27 | 0.5 | Boarding Shotgun, Nanopulser, D-Charges, AP Mine, Silenced Pistol, CCW; Minelayer | — |
| 5 | 25 | 0 | SMG, Nanopulser, D-Charges, Flash Pulse, Silenced Pistol, CCW; Forward Observer | — |

### Fennec Fusiliers

**ID 1803 · AVA 5 · LI · Line Troops**

`MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 2`

Skills: Terrain (Desert).

| Option | Pts | SWC | Loadout / profile notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 10 | 0 | Combi Rifle, Pistol, CCW | FENNECS |
| 2 | 18 | 1 | HMG, Pistol, CCW | FENNECS |
| 3 | 15 | 1.5 | Missile Launcher, Pistol, CCW | FENNECS |
| 4 | 12 | 0 | SMG, Light Rocket Launcher, Pistol, CCW | FENNECS |
| 5 | 14 | 0 | Thunderbolt (+1B), Shock Mine, Pistol, CCW; Triangulated Fire, Minelayer | FENNECS |
| 6 | 12 | 0 | Combi Rifle, Pistol, CCW; Commlink (+1), Specialist Operative | FENNECS |
| 7 | 16 | 0.5 | SMG, E/Mitter, Pistol, CCW; Hacking Device, FastPanda | FENNECS |
| 9 | 13 | 0 | Combi Rifle, Flash Pulse, Disco Baller, Pistol, CCW; Forward Observer, Sensor | FENNECS |
| 10 | 12 | 0 | Combi Rifle, Pistol, CCW; MediKit, Paramedic | FENNECS |
| 11 | 10 | 0 | Combi Rifle, Pistol, CCW; Lieutenant | FENNECS |

**Source note:** this pinned Army revision does **not** list Decoy on the Fennec Lieutenant profile.

### Fireflies Clandestine Demo Squad

**ID 1809 · AVA 5 · MI · Veteran Troops**

`MOV 10-10 | CC 17 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 6 | W 1 | S 2`

Skills/equipment: Albedo, BS Attack (SR-1), Immunity (Shock), Stealth, NCO, Terrain (Total).

| Option | Pts | SWC | Loadout / role | Fireteam |
|---:|---:|---:|---|---|
| 1 | 24 | 1.5 | Heavy Rocket Launcher, D-Charges, AP Mine, Assault Pistol, CCW | KESTREL; ARMORED optional |
| 2 | 19 | 0 | SMG, Panzerfaust, D-Charges, Pistol, CCW; Deployable Repeater | KESTREL; ARMORED optional |
| 3 | 23 | 0 | SMG, Panzerfaust, D-Charges, AP Mine, Pistol, CCW; Chain of Command | KESTREL; ARMORED optional |
| 4 | 23 | 0 | SMG, Panzerfaust, D-Charges, AP Mine, Pistol, CCW; Deactivator, GizmoKit, Engineer | KESTREL; ARMORED optional |
| 5 | 24 | 0 | SMG, Panzerfaust, D-Charges, AP Mine, Armed Turret (Marksman Rifle), Pistol, CCW; Minelayer | KESTREL; ARMORED optional |
| 6 | 25 | 0 | Combi Rifle, Panzerfaust, D-Charges, AP Mine, Pistol, CCW; MediKit, Paramedic | KESTREL; ARMORED optional |
| 7 | 24 | 0.5 | SMG, Panzerfaust, D-Charges, AP Mine, Pistol, CCW; Hacking Device | KESTREL; ARMORED optional |

### Peacemaker Armbots

**ID 36 · AVA 2 · REM · Support Troops**

`MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`

Skills/equipment: Repeater, Remote Presence, Courage, Forward Deployment (+20), Mimetism (-3). Uses Auxbot Peripheral profiles.

| Option | Pts | SWC | Loadout / profile notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Heavy Shotgun, Pulzar, PARA CCW (-3); Auxbot-3 | — |
| 3 | 24 | 0.5 | Heavy Shotgun, Pulzar, PARA CCW (-3); Auxbot-3B | — |
| 4 | 23 | 0 | Boarding Shotgun, Pulzar, PARA CCW (-3); BS Attack (+1B) | — |
| 5 | 27 | 0 | Boarding Shotgun, Pulzar, PARA CCW (-3); BS Attack (+1B); Auxbot-3 | — |

### Tech-Bees

**ID 935 · AVA 1 · LI · Support Troops**

`MOV 10-10 | CC 12 | BS 11 | PH 10 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 2`

Skills/equipment: Deactivator, GizmoKit, Specialist Operative, TAGCom [Dodge (PH+3), GizmoKit (PH+1)].

| Option | Pts | SWC | Loadout | Fireteam |
|---:|---:|---:|---|---|
| 2 | 9 | 0 | Deployable Repeater; Adhesive Launcher Rifle, Flash Pulse, Pistol, PARA CCW (-3) | — |

### Redeye Close Air Support Squad

**ID 1816 · AVA 2 · VH · Elite Troops**

`MOV 20-5 | CC — | BS 14 | PH 13 | WIP 13 | ARM 6 | BTS 6 | STR 2 | S 7`

Skills: Aerial, Courage, Dodge (-3), GizmoKit (PH=14), Mimetism (-6), Remote Presence, Super-Jump (Jet Propulsion), Terrain (Total), No Cover, Tech-recovery, Sensor.

| Option | Pts | SWC | Loadout | Fireteam |
|---:|---:|---:|---|---|
| 1 | 37 | 1.5 | Spitfire, Chain Rifle, Blitzen | — |
| 2 | 38 | 1.5 | Spitfire, Chain Rifle, Grenade Launcher (Continuous Damage) | — |

### Pathfinder Dronbot

**ID 16 · AVA 2 · REM · Support Troops**

`MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`

Skills/equipment: Deactivator, Repeater, Remote Presence, Courage, Triangulated Fire, Forward Observer, Sensor.

| Option | Pts | SWC | Loadout / profile notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3) | Wildcard max 1 |
| 2 | 17 | 0 | As above; Tactical Awareness | Wildcard max 1 |

### Palbots

**ID 37 · AVA 2 · REM · Support Peripheral**

`MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`

Skills: Peripheral (Servant), Courage, Mimetism (-3).

| Option | Pts | SWC | Loadout | Fireteam |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | PARA CCW (-3); Peripheral, no independent Order | — |

### Blink Team

**ID 1805 · AVA 2 · LI · Specially Trained**

`MOV 10-10 | CC 15 | BS 13 | PH 10 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`

Skills: Surprise Attack (-3), Camouflage, Hidden Deployment, Mimetism (-6), Stealth.

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 28 | 0 | Shock Marksman Rifle, Shock Mine, Assault Pistol, CCW | — |
| 2 | 32 | 1.5 | MULTI Sniper Rifle, Assault Pistol, CCW | — |
| 3 | 28 | 1.5 | Heavy Rocket Launcher, WildParrot, Assault Pistol, CCW; X Visor | — |

### BCA Magistrates

**ID 1804 · AVA 2 · LI · Specially Trained**

`MOV 10-10 | CC 15 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`

Skills/equipment: Biometric Visor, Counterintelligence, FT Master (Jackals), Immunity (Shock), Specialist Operative.

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 17 | 0 | Combi Rifle, Nanopulser, Heavy Pistol, Stun Pistol (+1B), CCW | FENNECS max 1; COLCORP 1-2 |
| 2 | 21 | 0 | MULTI Marksman Rifle, Nanopulser, Heavy Pistol, Stun Pistol (+1B), CCW | FENNECS max 1; COLCORP 1-2 |
| 3 | 21 | 0 | Option 1 weapons; Chain of Command | FENNECS max 1; COLCORP 1-2 |
| 4 | 25 | 0 | Option 2 weapons; Chain of Command | FENNECS max 1; COLCORP 1-2 |
| 5 | 19 | 0 | Option 1 weapons; Lieutenant, Strategos L1 | FENNECS max 1; COLCORP 1-2 |
| 6 | 23 | 0 | Option 2 weapons; Lieutenant, Strategos L1 | FENNECS max 1; COLCORP 1-2 |

### Beasthunters Free Guild

**ID 1570 · AVA 1 · SK · Mercenary Troops · Irregular**

`MOV 10-10 | CC 21 | BS 11 | PH 13 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`

Base skills: Mimetism (-3), Stealth, Super-Jump, Terrain (Total), Religious Troop.

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 9 | 0 | **BEASTHUNTER FTO**; Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CCW | COLCORP max 1 |
| 2 | 15 | 0 | Heavy Flamethrower, Tactical Bow, AP Mine, Pistol, DA CCW; Surprise Attack (-3), Camouflage, Forward Deployment (+20) | — |
| 3 | 15 | 0 | Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CCW; Surprise Attack (-3), Camouflage, Forward Deployment (+20) | — |
| 4 | 17 | 0 | Heavy Flamethrower (+1B), Panzerfaust, AP Mine, Pistol, DA CCW; Surprise Attack (-3), Camouflage, Forward Deployment (+20) | — |

### Black A.I.R.

**ID 1808 · AVA 3 · MI · Elite Troops**

`MOV 10-10 | CC 17 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`

Skills/equipment: MSV2, Mimetism (-3), Combat Instinct, Number 2, Terrain (Total).

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 26 | 0.5 | **BLACK A.I.R. FTO**; SMG, Nanopulser, D-Charges, Pistol, CCW; Hacking Device | FENNECS max 2 |
| 2 | 29 | 0.5 | **FTO**; K1 Marksman Rifle, Nanopulser, Flash Pulse, Pistol, CCW; Forward Observer | FENNECS max 2 |
| 3 | 33 | 1.5 | **FTO**; MULTI Sniper Rifle, Nanopulser, Pistol, CCW; Neurocinetics | FENNECS max 2 |
| 4 | 31 | 0 | SMG, Flash Pulse (+1B), D-Charges, Pistol, CCW; Killer Hacking Device; Parachutist (Deployment Zone) | — |

### Father Lucien Sforza

**ID 198 · AVA 1 · MI · Character**

`MOV 10-10 | CC 19 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`

Skills/equipment: X Visor, BS Attack (+1SD), Immunity (ARM), Combat Instinct, Stealth, NCO, Dogged, Religious Troop.

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 26 | 0 | Viral Rifle, Adhesive Launcher Rifle, Nanopulser, Heavy Pistol, PARA CCW; Holoprojector, Surprise Attack (-3), Forward Deployment (+10) | — |
| 2 | 23 | 0 | **SFORZA FTO**; Viral Rifle, Adhesive Launcher Rifle, Nanopulser, Heavy Pistol, PARA CCW | Wildcard max 1 |
| 3 | 26 | 0 | **SFORZA FTO**; as above; Albedo | Wildcard max 1 |

### Trauma-Docs

**ID 14 · AVA 1 · LI · Support Troops**

`MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`

Skills/equipment: MediKit, Doctor.

| Option | Pts | SWC | Loadout | Fireteam |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Pistol, CCW | — |

### Mulebots

**ID 38 · AVA 2 · REM · Support Troops**

`MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 4`

Skills/equipment: Baggage, Remote Presence, Courage.

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | Deactivator, Repeater; PARA CCW (-3) | — |
| 2 | 14 | 0.5 | EVO Hacking Device; PARA CCW (-3) | — |
| 3 | 17 | 0 | Repeater, Combi Rifle, PARA CCW (-3); Total Reaction | — |

### Minescorp Jackals

**ID 1813 · AVA 4 · LI · Support Troops · Irregular**

`MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 6 | 0 | **JACKAL FTO**; SMG, Panzerfaust, Boarding Pistol, CCW; Booty | COLCORP max 2 |
| 2 | 6 | 0 | **JACKAL FTO**; Light Rocket Launcher, Boarding Pistol, CCW; Booty | COLCORP max 2 |
| 3 | 10 | 0 | Boarding Shotgun, E/M Carbine, Shock Mine, Boarding Pistol, CCW; Infiltration | — |
| 4 | 10 | 0 | Combi Rifle, Blitzen, Boarding Pistol, CCW; Infiltration | — |
| 5 | 11 | 0.5 | Boarding Shotgun, E/M Grenade Launcher, Shock Mine, Boarding Pistol, CCW; Infiltration, Minelayer | — |

### Yamabushi

**ID 1824 · AVA 2 · WB**

`MOV 15-5 | CC 23 | BS 11 | PH 13 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`

Skills: Martial Arts L3, Forward Deployment (+10), Dodge (+5), Frenzy, Mimetism (-3), Stealth, Dogged, Religious Troop, CC Attack (Shock).

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 15 | 0 | **FTO-labelled**; Chain Rifle, Panzerfaust, Heavy Pistol, DA CCW | —; no Kestrel chart row |
| 2 | 16 | 0 | **FTO-labelled**; Chain Rifle, Tactical Bow, Heavy Pistol, DA CCW; MediKit, Paramedic | —; no Kestrel chart row |
| 3 | 16 | 0 | Chain Rifle, Panzerfaust, Heavy Pistol, DA CCW; Camouflage (1 Use) | — |
| 4 | 16 | 0 | Chain Rifle, Tactical Bow, Shock Mine, Heavy Pistol, DA CCW; Camouflage (1 Use) | — |
| 5 | 17 | 0 | Chain Rifle, Tactical Bow (+1B), Panzerfaust, Heavy Pistol, DA CCW; Camouflage (1 Use) | — |

### Richard Quinn

**ID 1490 · AVA 1 · LI · Character**

`MOV 10-10 | CC 13 | BS 13 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`

Skills/equipment: MSV1, Warhorse, Immunity (ARM).

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 26 | 0 | MULTI Marksman Rifle, Flash Pulse, D-Charges, Boarding Pistol (+1B), CCW; Forward Observer | Wildcard max 1, FENNECS / KESTREL only |
| 3 | 26 | 0 | MULTI Rifle, Flash Pulse, D-Charges, Disco Baller, Boarding Pistol (+1B), CCW; Forward Observer | Wildcard max 1, FENNECS / KESTREL only |

### Tikbalangs

**ID 33 · AVA 2 · TAG · Mechanized Troops**

`MOV 15-10 | CC 17 | BS 15 | PH 15 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`

Skills/equipment: ECM: Guided (-6), Remote Presence, BS Attack (SR-1), Courage, GizmoKit (PH=13), Mimetism (-3), Tactical Awareness, Terrain (Total), Climbing Plus, Dodge (PH=11).

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 69 | 1.5 | HMG, Heavy Flamethrower, Shock Mine, AP CCW; Crabbot | ARMORED native, max 2 |
| 4 | 73 | 1.5 | As above; Lieutenant (+1 Order); Crabbot | ARMORED native, max 2 |

### Machinists

**ID 15 · AVA 1 · LI · Support Troops**

`MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`

Skills/equipment: Deactivator, GizmoKit, Engineer.

| Option | Pts | SWC | Loadout | Fireteam |
|---:|---:|---:|---|---|
| 1 | 15 | 0 | Combi Rifle, D-Charges, Pistol, CCW | — |
| 8 | 16 | 0 | As above; Deployable Cover | — |
| 9 | 18 | 0 | As above; Armed Turret (Combi Rifle) | — |

### Emily Handelman

**ID 1072 · AVA 1 · LI · Character**

`MOV 10-10 | CC 17 | BS 13 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`

Skills/equipment: X Visor, Courage, Mimetism (-3), Number 2, Forward Observer, Dogged.

| Option | Pts | SWC | Loadout | Fireteam |
|---:|---:|---:|---|---|
| 1 | 22 | 0 | E/M Grenade Launcher, Nanopulser, Flash Pulse, Assault Pistol, CCW | Wildcard max 1, FENNECS / COLCORP only |
| 3 | 24 | 0 | Combi Rifle, Grenade Launcher, E/M Grenade Launcher, Nanopulser, Flash Pulse (+1B), Assault Pistol, CCW | Wildcard max 1, FENNECS / COLCORP only |

### Optimate Agent Maximus

**ID 1862 · AVA 1 · MI · Character**

`MOV 15-5 | CC 22 | BS 13 | PH 13 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`

Skills/equipment: CC Attack (-6), Courage, Dodge, Natural Born Warrior, Immunity (ARM), Number 2, Specialist Operative, Tactical Awareness, NWI, Cube 2.0.

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 48 | 1 | AP Thunderbolt (+2B), E/M Carbine, Heavy Pistol, AP+DA CCW; Minimus Peripheral | — |
| 2 | 45 | 1 | **MAXIMUS AGENT FTO**; same core weapons; TinBot (Repeater) | FENNECS max 1 |
| 3 | 48 | +1 | Option 1 weapons; Lieutenant; Minimus Peripheral | — |
| 4 | 45 | +1 | **FTO**; Option 2 weapons; Lieutenant; TinBot (Repeater) | FENNECS max 1 |

**Selection constraint:** Agent Maximus and TAG Maximus represent the same unique character identity; do not select both.

### Bulleteer Armbots

**ID 35 · AVA 2 · REM · Support Troops**

`MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`

Skills/equipment: Repeater, Remote Presence, Courage, Mimetism (-6).

| Option | Pts | SWC | Loadout | Fireteam |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Heavy Shotgun (+1B), PARA CCW (-3) | ARMORED optional, max 1 |
| 2 | 22 | 1 | Spitfire, PARA CCW (-3) | ARMORED optional, max 1 |

### Drummers Mobile Support Section

**ID 1806 · AVA 4 · LI · Specially Trained**

`MOV 10-10 | CC 14 | BS 13 | PH 10 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`

Equipment: 360º Visor. Each option includes the listed Drumbot Peripheral package.

| Option | Pts | SWC | Controller loadout / linked package | Fireteam |
|---:|---:|---:|---|---|
| 1 | 40 | 1 | Marksman Rifle, Pistol, CCW + Drumbot-1 | — |
| 2 | 42 | 1.5 | Marksman Rifle, Pistol, CCW + Drumbot-2 | — |
| 3 | 40 | 1 | Marksman Rifle, Pistol, CCW + Drumbot-3 | — |
| 4 | 42 | 1 | Marksman Rifle, Pistol, CCW + Drumbot-4; Forward Deployment (+10) | — |
| 5 | 21 | 0 | Marksman Rifle, Flash Pulse, Pistol, CCW; Forward Observer + Drumbot-5 | — |
| 6 | 28 | 1.5 | MULTI Sniper Rifle, Flash Pulse, Pistol, CCW; Forward Observer + Drumbot-5 | — |
| 7 | 47 | 1 | Marksman Rifle, Flash Pulse, Pistol, CCW; Forward Observer + Drumbot-1 + Drumbot-5 | — |
| 8 | 47 | 1 | Marksman Rifle, Flash Pulse, Pistol, CCW; Forward Observer + Drumbot-3 + Drumbot-5 | — |

Linked Drumbots supply the option-specific remote weapon package; use the pinned Army profile when exact Peripheral weapon interaction is material to a rules question.

### Team Crux Father-Knights

**ID 1815 · AVA 1 · HI · Elite Troops**

`MOV 15-5 | CC 22 | BS 14 | PH 14 | WIP 13 | ARM 5 | BTS 6 | W 2 | S 2`

Skills/equipment: Albedo, Martial Arts L2, BS Attack (+1SD), Berserk, Courage, Specialist Operative, Stealth, Religious Troop.

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 47 | 0 | AP SMG, Flash Pulse, D-Charges, CrazyKoala, Pistol, DA CCW; Surprise Attack (-3), Forward Deployment (+20), Hidden Deployment | — |
| 2 | 48 | 0.5 | AP SMG, Flash Pulse, D-Charges, CrazyKoala, Armed Turret (Combi Rifle), Pistol, DA CCW; Hidden Deployment, Forward Deployment (+20) | — |
| 3 | 54 | 0 | MULTI Marksman Rifle, D-Charges, CrazyKoala, MULTI Pistol, DA CCW; Forward Deployment (+20) | — |
| 4 | 46 | 0 | **CRUX KNIGHT FTO**; MULTI Marksman Rifle, Drop Bears, D-Charges, MULTI Pistol, DA CCW | Wildcard max 1 |
| 5 | 49 | 1.5 | **FTO**; Spitfire, Drop Bears, D-Charges, MULTI Pistol, DA CCW | Wildcard max 1 |
| 6 | 50 | 0 | **FTO**; MULTI Marksman Rifle, Drop Bears, D-Charges, MULTI Pistol, DA CCW; Strategic Deployment | Wildcard max 1 |

### Hetkari Shooters

**ID 1811 · AVA 2 · HI · Specially Trained**

`MOV 15-5 | CC 17 | BS 14 | PH 14 | WIP 12 | ARM 5 | BTS 6 | W 2 | S 2`

Skills: Marksmanship, Combat Instinct.

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 47 | 1.5 | Missile Launcher, Breaker Pistol, AP SMG, CCW | KESTREL required-choice member, max 1 |
| 2 | 48 | 1.5 | MULTI Red Fury, Breaker Pistol, CCW, E/Marat | KESTREL required-choice member, max 1 |
| 3 | 47 | 1.5 | Option 1; Lieutenant | KESTREL required-choice member, max 1 |
| 4 | 48 | 1.5 | Option 2; Lieutenant | KESTREL required-choice member, max 1 |

### Griffin Troops

**ID 1810 · AVA 3 · HI · Veteran Troops**

`MOV 15-5 | CC 16 | BS 14 | PH 12 | WIP 12 | ARM 4 | BTS 6 | W 2 | S 2`

Skills/equipment: MSV1, Courage, Terrain (Desert), Jump.

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 31 | 0 | MULTI Rifle, Pulzar, Pistol, CCW | FENNECS max 1; KESTREL max 3 required-choice |
| 2 | 37 | 1.5 | HMG, Pulzar, Pistol, CCW | FENNECS max 1; KESTREL max 3 required-choice |
| 3 | 38 | 1.5 | Feuerbach, Pulzar, Pistol, CCW | FENNECS max 1; KESTREL max 3 required-choice |
| 4 | 37 | 1 | HMG, Pulzar, Pistol, CCW; Lieutenant | FENNECS max 1; KESTREL max 3 required-choice |

### Bipandra

**ID 46 · AVA 1 · LI · Character**

`MOV 10-10 | CC 17 | BS 12 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`

Skills/equipment: Dodge, Immunity (Shock), Doctor, MediKit (+1B).

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Combi Rifle, Nanopulser (+1B), Pistol, CCW | Wildcard max 1, FENNECS / KESTREL only |
| 2 | 25 | 0 | As above; Tactical Awareness | Wildcard max 1, FENNECS / KESTREL only |

### Squalos Mk-II

**ID 1651 · AVA 2 · TAG · Mechanized Troops**

`MOV 15-10 | CC 18 | BS 15 | PH 15 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`

Skills/equipment: ECM: Guided (-6), BS Attack (+1SD), Courage, Dodge, Combat Instinct, Remote Presence, Tactical Awareness.

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 55 | 1 | MULTI Marksman Rifle, MULTI Pistol (+1B), CCW; Crabbot | ARMORED native, max 2 |
| 2 | 62 | 1.5 | HMG, Grenade Launcher, MULTI Pistol (+1B), CCW | ARMORED native, max 2 |
| 3 | 66 | 1.5 | MULTI HMG, MULTI Pistol (+1B), CCW; NCO | ARMORED native, max 2 |

### Banshees Airborne Assault Unit

**ID 1807 · AVA 3 · MI · Specially Trained**

`MOV 10-10 | CC 15 | BS 12 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`

Skills/equipment: MSV1, Parachutist, Combat Jump, Super-Jump (Jet Propulsion).

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Light Shotgun, Pulzar (+1B), D-Charges, Pistol, CCW | — |
| 2 | 22 | 0 | SMG, Pulzar (+1B), D-Charges, WildParrot, Pistol, CCW | — |
| 3 | 25 | 0.5 | SMG, Pulzar (+1B), D-Charges, Pistol, CCW; Hacking Device | — |
| 4 | 23 | 0 | SMG, Pulzar (+1B), D-Charges, Pistol, CCW; Killer Hacking Device | — |

### Dr. Priya Harper

**ID 1814 · AVA 1 · LI · Character**

`MOV 10-10 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`

Skills/equipment: Nanoscreen, X Visor, Booty, Dodge, Immunity (Shock), Specialist Operative, NWI, No Cover, Tactical Awareness.

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 32 | +1 | **DR HARPER FTO**; Plasma Carbine, Nanopulser, E/M Mine, Viral Pistol (+1B), CCW; Tactical Awareness | Wildcard max 1 |
| 2 | 35 | +1 | Same weapons; Forward Deployment (+20), Tactical Awareness | — |

### Knauf

**ID 939 · AVA 1 · LI · Character**

`MOV 10-10 | CC 21 | BS 13 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`

Skills/equipment: MSV1, Courage, Mimetism (-3), Stealth, Terrain (Total).

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 31 | 1.5 | MULTI Sniper Rifle, AP Heavy Pistol, CCW; Surprise Attack (-3), Decoy (1) | — |

### Warcors

**ID 50 · AVA 1 · LI · Mercenary Troops · Irregular**

`MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`

Skills: Journalist.

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor | — |
| 2 | 3 | 0 | As above; Sixth Sense | — |

### Maximus, Optimate and HexaDome Legend

**ID 1720 · AVA 1 · TAG · Character**

`MOV 15-10 | CC 24 | BS 14 | PH 13 | WIP 13 | ARM 6 | BTS 6 | W 4 | S 6`

Skills/equipment: ECM: Guided (-6), CC Attack (-6), BS Attack (SR-1), Courage, Dodge, Natural Born Warrior, Immunity (ARM), Tactical Awareness, Transmutation (Escape System), Cube 2.0.

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 82 | 1.5 | AP HMG, E/M Carbine, Heavy Pistol, AP+DA CCW | ARMORED optional, max 1 |
| 2 | 80 | 1 | AP Thunderbolt (+2B), E/M Carbine, Heavy Pistol, AP+DA CCW | ARMORED optional, max 1 |
| 3 | 82 | 0 | AP HMG, E/M Carbine, Heavy Pistol, AP+DA CCW; Lieutenant | ARMORED optional, max 1 |

**Selection constraint:** TAG Maximus and Agent Maximus are mutually exclusive representations of Maximus.

### Dart, Optimate Huntress

**ID 1130 · AVA 1 · SK · Character**

`MOV 10-10 | CC 16 | BS 13 | PH 13 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`

Skills/equipment: MSV1, Surprise Attack (-3), Camouflage, Courage, Forward Deployment (+20), Mimetism (-3), Immunity (Shock), Stealth, NWI, Terrain (Total), Climbing Plus, Specialist Operative, Decoy (1).

| Option | Pts | SWC | Loadout / notes | Fireteam |
|---:|---:|---:|---|---|
| 1 | 35 | 0 | AP SMG, Pistol, CCW, Viral Tactical Bow, E/M Grenades | — |
| 2 | 35 | 0 | As above; Shock Mine | — |
| 3 | 36 | 0.5 | As above; Shock Mine, Minelayer | — |
| 4 | 42 | 0.5 | As above; Minelayer; Sharvara K9 Peripheral | — |

### Sāchā Xenotech Hunters

**ID 1874 · AVA 1 · LI · Mercenary Troops · Irregular**

`MOV 10-10 | CC 17 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`

Skills: Forward Deployment (+10), Booty, Terrain (Total), Climbing Plus, Specialist Operative.

| Option | Pts | SWC | Loadout | Fireteam |
|---:|---:|---:|---|---|
| 1 | 6 | 0 | Flash Pulse, E/M Grenades (+1B), Stun Pistol (+1B), CCW | — |

### Kazurabā Ruby Monday

**ID 1890 · AVA 1 · HI · Character · Irregular**

`MOV 15-5 | CC 18 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 6 | W 2 | S 2`

Skills: BS Attack (+1B), Booty, Dodge, Immunity (IMM-B), Technorganic, Terrain (Total), Climbing Plus, Specialist Operative.

| Option | Pts | SWC | Loadout | Fireteam |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Adhesive Launcher Rifle, Flash Pulse, E/M Grenades, Stun Pistol, CCW | — |

## Fireteams

This section is the **canonical Fireteam definition** for Kestrel. If a unit-level note or the reverse index conflicts with this section, this section wins.

### Chart limits

| Type | Source limit |
|---|---:|
| Core | 1 |
| Haris | 1 |
| Duo | 256 |

`DUO: 256` is preserved from the Army source. Treat it as the source's effectively-unlimited chart-level Duo value rather than silently rewriting it to another number.

### FENNECS Fireteam

**Types:** Core, Haris

| Member | Min | Max | Required-choice | Restriction / counts-as / notes |
|---|---:|---:|---|---|
| Fennec | 1 | 5 | No | Native Fennec Fusiliers |
| Black A.I.R. FTO | 0 | 2 | No | FTO profiles only |
| Griffin | 0 | 1 | No | Source comment: `(Fennec)` |
| Magistrate | 0 | 1 | No | — |
| Maximus Agent | 0 | 1 | No | Agent Maximus; use FTO-labelled Agent profiles for Fireteam selection |
| Indigo | 0 | 1 | No | Spec-Ops only; optional mode |

At least one Fennec is required by the explicit `min: 1` row.

### KESTREL Fireteams

**Types:** Duo, Haris

| Member | Min | Max | Required-choice | Restriction / notes |
|---|---:|---:|---|---|
| Griffin | 0 | 3 | Yes | Source comment: `(Kestrel)` |
| Firefly | 0 | 3 | Yes | Source comment: `(Kestrel)` |
| Hetkari | 0 | 1 | Yes | — |

`required: true` rows form a required-choice set: a legal KESTREL Fireteam must contain at least one member from the Griffin / Firefly / Hetkari required set. It does **not** mean all three rows must be represented simultaneously.

### ARMORED Fireteams

**Type:** Duo

| Member | Min | Max | Required-choice | Restriction / notes |
|---|---:|---:|---|---|
| Tikbalang | 0 | 2 | Yes | Native armored anchor |
| Squalo Mk-II | 0 | 2 | Yes | Native armored anchor |
| Maximus Optimate | 0 | 1 | No | TAG Maximus |
| Firefly | 0 | 1 | No | — |
| Bulleteer | 0 | 1 | No | — |

A legal ARMORED Fireteam must contain at least one Tikbalang or Squalo Mk-II from the required-choice set.

### COLCORP Fireteams

**Types:** Duo, Haris

| Member | Min | Max | Required-choice | Restriction / notes |
|---|---:|---:|---|---|
| Magistrate | 1 | 2 | No | Source comment: `(ColCorp)`; explicit minimum 1 |
| Jackal FTO | 0 | 2 | No | FTO profiles only; source comment `(ColCorp)` |
| Beasthunter FTO | 0 | 1 | No | FTO profile only |

At least one Magistrate is required by the explicit `min: 1` row.

### Wildcards

| Wildcard | Max | Allowed Fireteams / restrictions |
|---|---:|---|
| Crux Knight FTO | 1 | Any legal Kestrel Fireteam; FTO profiles only |
| Pathfinder Dronbot | 1 | Any legal Kestrel Fireteam |
| Bipandra | 1 | FENNECS or KESTREL only |
| Dr. Harper FTO | 1 | Any legal Kestrel Fireteam; FTO profile only |
| Quinn | 1 | FENNECS or KESTREL only |
| Sforza FTO | 1 | Any legal Kestrel Fireteam; FTO profiles only |
| Emily | 1 | FENNECS or COLCORP only |

Wildcard access does not remove the native formation's required/minimum member conditions.

## Unit → Fireteam access index

This section is derivative. The canonical Fireteam tables above control legality.

| Unit | Fireteam access |
|---|---|
| Sierra Dronbot | — |
| Clipper Dronbot | — |
| Fugazi Dronbot | — |
| Scarecrows | — |
| Fennec Fusiliers | FENNECS Core/Haris; native, at least one Fennec in team |
| Fireflies | KESTREL Duo/Haris required-choice member; ARMORED Duo optional max 1 |
| Peacemaker | — |
| Tech-Bee | — |
| Redeye | — |
| Pathfinder | Wildcard max 1 in any legal Kestrel Fireteam |
| Palbot | — |
| Blink Team | — |
| BCA Magistrate | FENNECS max 1; COLCORP min 1 / max 2 |
| Beasthunter | COLCORP max 1, FTO profile only |
| Black A.I.R. | FENNECS max 2, FTO profiles only |
| Sforza | Wildcard max 1, FTO profiles only |
| Trauma-Doc | — |
| Mulebot | — |
| Minescorp Jackal | COLCORP max 2, FTO profiles only |
| Yamabushi | —; FTO-labelled options do not have chart access |
| Quinn | Wildcard max 1, FENNECS / KESTREL only |
| Tikbalang | ARMORED Duo required-choice member, max 2 |
| Machinist | — |
| Emily | Wildcard max 1, FENNECS / COLCORP only |
| Optimate Agent Maximus | FENNECS max 1; use FTO-labelled Agent profiles |
| Bulleteer | ARMORED Duo optional max 1 |
| Drummers | — |
| Crux Knight | Wildcard max 1, FTO profiles only |
| Hetkari | KESTREL Duo/Haris required-choice member, max 1 |
| Griffin | FENNECS max 1; KESTREL Duo/Haris required-choice member, max 3 |
| Bipandra | Wildcard max 1, FENNECS / KESTREL only |
| Squalo Mk-II | ARMORED Duo required-choice member, max 2 |
| Banshee | — |
| Dr. Harper | Wildcard max 1, FTO profile only |
| Knauf | — |
| Warcor | — |
| Maximus TAG | ARMORED Duo optional max 1 |
| Dart | — |
| Sāchā | — |
| Ruby Monday | — |
| Indigo Spec-Ops | FENNECS max 1 when Spec-Ops mode is in use |
| Indigo Team-Ops | — in ordinary Kestrel Fireteam chart |

## Tactical tags

These are repository analysis aids, not official Army characteristics.

| Unit | Useful tags |
|---|---|
| Fennec | cheap order, Lieutenant, hacker, Sensor/FO, Disco Baller, Minelayer, long-range gun |
| Firefly | NCO, Engineer, CoC, hacker, deployable repeater, mine/turret support, Kestrel link anchor |
| Magistrate | Strategos Lieutenant, Counterintelligence, CoC, Jackal support, FENNECS/COLCORP link |
| Jackal | cheap irregular, FTO filler, infiltration, E/M attack, Minelayer |
| Griffin | durable HI gunfighter, MSV1, Lieutenant, flexible FENNECS/KESTREL link |
| Hetkari | heavy long-range gunfighter, Lieutenant, KESTREL link anchor |
| Tikbalang | mobile TAG, TacAware, Mimetism, Climbing Plus, Lieutenant option, ARMORED anchor |
| Squalo Mk-II | TAG gunfighter, TacAware, NCO option, ARMORED anchor |
| Pathfinder | Sensor/FO, Repeater, TacAware option, Wildcard |
| Mulebot | Baggage, EVO, cheap support, TR option |
| Scarecrow | hidden/infiltrating hacker or KHD, repeater/mines, midfield specialist |
| Black A.I.R. | MSV2, FTO hacker/FO/sniper, airborne KHD option |
| Banshee | airborne attacker/specialist, hacker/KHD |
| Redeye | fast aerial attack/support, Sensor, Mimetism (-6) |
| Crux Knight | premium HI specialist, hidden-deployment options, FTO Wildcard |
| Emily | E/M grenade launcher, FO, scoped Wildcard |
| Quinn | MSV1 gunfighter/FO, Disco Baller option, scoped Wildcard |
| Bipandra | Doctor, TacAware option, scoped Wildcard |
| Dr. Harper | specialist, TacAware, FTO Wildcard |
| Bulleteer | fast Mimetism (-6) REM gunfighter, ARMORED Duo support |
| Peacemaker | forward-deployed repeater/attack REM |
| Dart | camouflaged midfield specialist/attacker |
| Beasthunter | cheap FTO template/Panzerfaust or camouflaged midfield attack |
| Yamabushi | warband-style CC/short-range attack, camo variants |

## Validation and maintenance

- Standard roster represented: **40 standard units**.
- Optional-mode hooks represented separately: Indigo Spec-Ops and Indigo Team-Ops.
- Canonical Kestrel Fireteam source rows represented: **FENNECS, KESTREL, ARMORED, COLCORP, Wildcards**.
- Fireteam chart limits preserved: `CORE 1`, `HARIS 1`, `DUO 256`.
- Wildcard scope restrictions preserved.
- FTO restrictions are profile-level where the chart/source requires them.
- Required-choice semantics are recorded separately from explicit `min` values.
- No Fireteam access is inferred solely from an `FTO` name.
- Agent Maximus and TAG Maximus mutual-exclusion constraint is recorded.
- Linked Reinforcement section: Code: Capital (`army_id: 199`); no `fireteamChart` field present in the pinned Reinforcement document.

### Refresh rule

When a newer Army source revision or InfinityDB normalization supersedes these provenance fields, set `status: stale` until the roster/profile/Fireteam diff has been reconciled. Do not silently mix newer live values into this file without updating the provenance block.