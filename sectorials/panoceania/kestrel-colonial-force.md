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
coverage: "Standard Kestrel roster, standard loadouts, canonical Fireteam chart, and reverse Fireteam index. Spec-Ops and Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# Kestrel Colonial Force

## Overview and provenance

Repository-native reference for **Kestrel Colonial Force** roster, profiles, points/SWC, AVA, and Fireteam access.

Sources used:

- Army-derived Kestrel source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **40-unit standard Kestrel roster** and the complete Kestrel `fireteamChart` in the pinned Army source.
- Soldier of Fortune entries with empty faction lists are excluded from the base roster.
- `Indigo Spec-Ops` and `Indigo Team-Ops` are optional game-mode content and are listed separately.
- Fireteam legality comes from the canonical chart in this file, not from an `FTO` loadout name by itself.
- Parenthetical Army-chart comments such as `(Fennec)`, `(Kestrel)`, and `(ColCorp)` are normalized by InfinityDB as **Counts-as / equivalence labels**, not as restrictions on which Fireteam a Wildcard may join.
- Linked Reinforcement section: **Code: Capital** (`army_id: 199`). Its pinned Army document has no `fireteamChart`, so no Reinforcement Fireteam rows are merged here.

## Roster index

| Unit | ID | AVA | Type | Order | Fireteam access |
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
| Pathfinder Dronbot | 16 | 2 | REM | Regular | Wildcard max 1 |
| Palbots | 37 | 2 | REM | Peripheral | — |
| Blink Team | 1805 | 2 | LI | Regular | — |
| BCA Magistrates | 1804 | 2 | LI | Regular | FENNECS; COLCORP |
| Beasthunters Free Guild | 1570 | 1 | SK | Irregular | COLCORP, FTO profile only |
| Black A.I.R. | 1808 | 3 | MI | Regular | FENNECS, FTO profiles only |
| Father Lucien Sforza | 198 | 1 | MI | Regular | Wildcard, FTO profiles only |
| Trauma-Docs | 14 | 1 | LI | Regular | — |
| Mulebots | 38 | 2 | REM | Regular | — |
| Minescorp Jackals | 1813 | 4 | LI | Irregular | COLCORP, FTO profiles only |
| Yamabushi | 1824 | 2 | WB | Regular | —; FTO-labelled options have no Kestrel chart row |
| Richard Quinn | 1490 | 1 | LI | Regular | Wildcard max 1; counts as Fennec/Kestrel |
| Tikbalangs | 33 | 2 | TAG | Regular | ARMORED native |
| Machinists | 15 | 1 | LI | Regular | — |
| Emily Handelman | 1072 | 1 | LI | Regular | Wildcard max 1; counts as Fennec/ColCorp |
| Optimate Agent Maximus | 1862 | 1 | MI | Regular | FENNECS max 1; no chart-level FTO restriction |
| Bulleteer Armbots | 35 | 2 | REM | Regular | ARMORED optional |
| Drummers Mobile Support Section | 1806 | 4 | LI | Regular | — |
| Team Crux Father-Knights | 1815 | 1 | HI | Regular | Wildcard, FTO profiles only |
| Hetkari Shooters | 1811 | 2 | HI | Regular | KESTREL native |
| Griffin Troops | 1810 | 3 | HI | Regular | FENNECS/Kestrel; counts as Fennec/Kestrel by row |
| Bipandra | 46 | 1 | LI | Regular | Wildcard max 1; counts as Fennec/Kestrel |
| Squalos Mk-II | 1651 | 2 | TAG | Regular | ARMORED native |
| Banshees Airborne Assault Unit | 1807 | 3 | MI | Regular | — |
| Dr. Priya Harper | 1814 | 1 | LI | Regular | Wildcard, FTO profile only |
| Knauf | 939 | 1 | LI | Regular | — |
| Warcors | 50 | 1 | LI | Irregular | — |
| Maximus, Optimate and HexaDome Legend | 1720 | 1 | TAG | Regular | ARMORED optional |
| Dart, Optimate Huntress | 1130 | 1 | SK | Regular | — |
| Sāchā Xenotech Hunters | 1874 | 1 | LI | Irregular | — |
| Kazurabā Ruby Monday | 1890 | 1 | HI | Irregular | — |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Indigo Spec-Ops | 1912 | Spec-Ops | `INDIGO (Spec-Ops)` row in FENNECS, max 1 |
| Indigo Team-Ops | 1926 | Team-Ops | No ordinary Kestrel Fireteam row |

## Unit details

### Sierra Dronbot

**ID 17 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage, Total Reaction, 360º Visor.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 1 | HMG; PARA CCW (-3) | — |
| 2 | 18 | 0 | Thunderbolt (+1B); PARA CCW (-3) | — |

### Clipper Dronbot

**ID 18 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 1.5 | Missile Launcher, Guided; PARA CCW (-3) | — |
| 5 | 19 | 1.5 | **CLIPPER DRONBOT FTO**; Missile Launcher (+1B); PARA CCW (-3) | —; no Kestrel chart row |

### Fugazi Dronbot

**ID 19 · AVA 1 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Remote Presence, Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | Flash Pulse; PARA CCW (-3) | — |

### Scarecrows Active Recon Group

**ID 1812 · AVA 3 · SK** — `MOV 10-10 | CC 15 | BS 13 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Surprise Attack (-3), Camouflage, Hidden Deployment, Infiltration, Mimetism (-6), Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 0 | Boarding Shotgun, Nanopulser, D-Charges, Silenced Pistol, CCW; Deployable Repeater | — |
| 2 | 29 | 0.5 | SMG, Nanopulser, D-Charges, Silenced Pistol, CCW; Hacking Device | — |
| 3 | 27 | 0 | SMG, Nanopulser, D-Charges, Silenced Pistol, CCW; Killer Hacking Device | — |
| 4 | 27 | 0.5 | Boarding Shotgun, Nanopulser, D-Charges, AP Mine, Silenced Pistol, CCW; Minelayer | — |
| 5 | 25 | 0 | SMG, Nanopulser, D-Charges, Flash Pulse, Silenced Pistol, CCW; Forward Observer | — |

### Fennec Fusiliers

**ID 1803 · AVA 5 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 2`. Terrain (Desert).

| Opt | Pts | SWC | Loadout / role | FT |
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

**Source note:** revision `7.26246.158` does **not** list Decoy on the Fennec Lieutenant.

### Fireflies Clandestine Demo Squad

**ID 1809 · AVA 5 · MI** — `MOV 10-10 | CC 17 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 6 | W 1 | S 2`. Albedo, BS Attack (SR-1), Immunity (Shock), Stealth, NCO, Terrain (Total).

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 1.5 | Heavy Rocket Launcher, D-Charges, AP Mine, Assault Pistol, CCW | KESTREL; ARMORED optional |
| 2 | 19 | 0 | SMG, Panzerfaust, D-Charges, Pistol, CCW; Deployable Repeater | KESTREL; ARMORED optional |
| 3 | 23 | 0 | SMG, Panzerfaust, D-Charges, AP Mine, Pistol, CCW; Chain of Command | KESTREL; ARMORED optional |
| 4 | 23 | 0 | SMG, Panzerfaust, D-Charges, AP Mine, Pistol, CCW; Deactivator, GizmoKit, Engineer | KESTREL; ARMORED optional |
| 5 | 24 | 0 | SMG, Panzerfaust, D-Charges, AP Mine, Armed Turret (Marksman Rifle), Pistol, CCW; Minelayer | KESTREL; ARMORED optional |
| 6 | 25 | 0 | Combi Rifle, Panzerfaust, D-Charges, AP Mine, Pistol, CCW; MediKit, Paramedic | KESTREL; ARMORED optional |
| 7 | 24 | 0.5 | SMG, Panzerfaust, D-Charges, AP Mine, Pistol, CCW; Hacking Device | KESTREL; ARMORED optional |

In the KESTREL row Fireflies carry the equivalence label **Counts as: Kestrel**.

### Peacemaker Armbots

**ID 36 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Repeater, Remote Presence, Courage, Forward Deployment (+20), Mimetism (-3); Auxbot Peripheral.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Heavy Shotgun, Pulzar, PARA CCW (-3); Auxbot-3 | — |
| 3 | 24 | 0.5 | Heavy Shotgun, Pulzar, PARA CCW (-3); Auxbot-3B | — |
| 4 | 23 | 0 | Boarding Shotgun, Pulzar, PARA CCW (-3); BS Attack (+1B) | — |
| 5 | 27 | 0 | Boarding Shotgun, Pulzar, PARA CCW (-3); BS Attack (+1B); Auxbot-3 | — |

### Tech-Bees

**ID 935 · AVA 1 · LI** — `MOV 10-10 | CC 12 | BS 11 | PH 10 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 2`. Deactivator, GizmoKit, Specialist Operative, TAGCom [Dodge (PH+3), GizmoKit (PH+1)].

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 2 | 9 | 0 | Deployable Repeater; Adhesive Launcher Rifle, Flash Pulse, Pistol, PARA CCW (-3) | — |

### Redeye Close Air Support Squad

**ID 1816 · AVA 2 · VH** — `MOV 20-5 | CC — | BS 14 | PH 13 | WIP 13 | ARM 6 | BTS 6 | STR 2 | S 7`. Aerial, Courage, Dodge (-3), GizmoKit (PH=14), Mimetism (-6), Remote Presence, Super-Jump (Jet Propulsion), Terrain (Total), No Cover, Tech-recovery, Sensor.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 37 | 1.5 | Spitfire, Chain Rifle, Blitzen | — |
| 2 | 38 | 1.5 | Spitfire, Chain Rifle, Grenade Launcher (Continuous Damage) | — |

### Pathfinder Dronbot

**ID 16 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Deactivator, Repeater, Remote Presence, Courage, Triangulated Fire, Forward Observer, Sensor.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3) | Wildcard max 1 |
| 2 | 17 | 0 | Same; Tactical Awareness | Wildcard max 1 |

### Palbots

**ID 37 · AVA 2 · REM Peripheral** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Peripheral (Servant), Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | PARA CCW (-3); no independent Order | — |

### Blink Team

**ID 1805 · AVA 2 · LI** — `MOV 10-10 | CC 15 | BS 13 | PH 10 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`. Surprise Attack (-3), Camouflage, Hidden Deployment, Mimetism (-6), Stealth.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 28 | 0 | Shock Marksman Rifle, Shock Mine, Assault Pistol, CCW | — |
| 2 | 32 | 1.5 | MULTI Sniper Rifle, Assault Pistol, CCW | — |
| 3 | 28 | 1.5 | Heavy Rocket Launcher, WildParrot, Assault Pistol, CCW; X Visor | — |

### BCA Magistrates

**ID 1804 · AVA 2 · LI** — `MOV 10-10 | CC 15 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Biometric Visor, Counterintelligence, FT Master (Jackals), Immunity (Shock), Specialist Operative.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 17 | 0 | Combi Rifle, Nanopulser, Heavy Pistol, Stun Pistol (+1B), CCW | FENNECS max 1; COLCORP 1-2 |
| 2 | 21 | 0 | MULTI Marksman Rifle, Nanopulser, Heavy Pistol, Stun Pistol (+1B), CCW | FENNECS max 1; COLCORP 1-2 |
| 3 | 21 | 0 | Option 1; Chain of Command | FENNECS max 1; COLCORP 1-2 |
| 4 | 25 | 0 | Option 2; Chain of Command | FENNECS max 1; COLCORP 1-2 |
| 5 | 19 | 0 | Option 1; Lieutenant, Strategos L1 | FENNECS max 1; COLCORP 1-2 |
| 6 | 23 | 0 | Option 2; Lieutenant, Strategos L1 | FENNECS max 1; COLCORP 1-2 |

In the COLCORP row Magistrates carry **Counts as: ColCorp**.

### Beasthunters Free Guild

**ID 1570 · AVA 1 · SK · Irregular** — `MOV 10-10 | CC 21 | BS 11 | PH 13 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. Mimetism (-3), Stealth, Super-Jump, Terrain (Total), Religious Troop.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 9 | 0 | **BEASTHUNTER FTO**; Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CCW | COLCORP max 1 |
| 2 | 15 | 0 | Heavy Flamethrower, Tactical Bow, AP Mine, Pistol, DA CCW; Surprise Attack (-3), Camouflage, Forward Deployment (+20) | — |
| 3 | 15 | 0 | Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CCW; Surprise Attack (-3), Camouflage, Forward Deployment (+20) | — |
| 4 | 17 | 0 | Heavy Flamethrower (+1B), Panzerfaust, AP Mine, Pistol, DA CCW; Surprise Attack (-3), Camouflage, Forward Deployment (+20) | — |

### Black A.I.R.

**ID 1808 · AVA 3 · MI** — `MOV 10-10 | CC 17 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. MSV2, Mimetism (-3), Combat Instinct, Number 2, Terrain (Total).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 0.5 | **BLACK A.I.R. FTO**; SMG, Nanopulser, D-Charges, Pistol, CCW; Hacking Device | FENNECS max 2 |
| 2 | 29 | 0.5 | **FTO**; K1 Marksman Rifle, Nanopulser, Flash Pulse, Pistol, CCW; Forward Observer | FENNECS max 2 |
| 3 | 33 | 1.5 | **FTO**; MULTI Sniper Rifle, Nanopulser, Pistol, CCW; Neurocinetics | FENNECS max 2 |
| 4 | 31 | 0 | SMG, Flash Pulse (+1B), D-Charges, Pistol, CCW; Killer Hacking Device; Parachutist (Deployment Zone) | — |

### Father Lucien Sforza

**ID 198 · AVA 1 · MI** — `MOV 10-10 | CC 19 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. X Visor, BS Attack (+1SD), Immunity (ARM), Combat Instinct, Stealth, NCO, Dogged, Religious Troop.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 0 | Viral Rifle, Adhesive Launcher Rifle, Nanopulser, Heavy Pistol, PARA CCW; Holoprojector, Surprise Attack (-3), Forward Deployment (+10) | — |
| 2 | 23 | 0 | **SFORZA FTO**; Viral Rifle, Adhesive Launcher Rifle, Nanopulser, Heavy Pistol, PARA CCW | Wildcard max 1 |
| 3 | 26 | 0 | **SFORZA FTO**; same; Albedo | Wildcard max 1 |

### Trauma-Docs

**ID 14 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. MediKit, Doctor.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Pistol, CCW | — |

### Mulebots

**ID 38 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 4`. Baggage, Remote Presence, Courage.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | Deactivator, Repeater; PARA CCW (-3) | — |
| 2 | 14 | 0.5 | EVO Hacking Device; PARA CCW (-3) | — |
| 3 | 17 | 0 | Repeater, Combi Rifle, PARA CCW (-3); Total Reaction | — |

### Minescorp Jackals

**ID 1813 · AVA 4 · LI · Irregular** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 6 | 0 | **JACKAL FTO**; SMG, Panzerfaust, Boarding Pistol, CCW; Booty | COLCORP max 2; Counts as ColCorp |
| 2 | 6 | 0 | **JACKAL FTO**; Light Rocket Launcher, Boarding Pistol, CCW; Booty | COLCORP max 2; Counts as ColCorp |
| 3 | 10 | 0 | Boarding Shotgun, E/M Carbine, Shock Mine, Boarding Pistol, CCW; Infiltration | — |
| 4 | 10 | 0 | Combi Rifle, Blitzen, Boarding Pistol, CCW; Infiltration | — |
| 5 | 11 | 0.5 | Boarding Shotgun, E/M Grenade Launcher, Shock Mine, Boarding Pistol, CCW; Infiltration, Minelayer | — |

### Yamabushi

**ID 1824 · AVA 2 · WB · Regular** — `MOV 15-5 | CC 23 | BS 11 | PH 13 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Martial Arts L3, Forward Deployment (+10), Dodge (+5), Frenzy, Mimetism (-3), Stealth, Dogged, Religious Troop, CC Attack (Shock).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 15 | 0 | **YAMABUSHI FTO**; Chain Rifle, Panzerfaust, Heavy Pistol, DA CCW | —; no chart row |
| 2 | 16 | 0 | **YAMABUSHI FTO**; Chain Rifle, Tactical Bow, Heavy Pistol, DA CCW; MediKit, Paramedic | —; no chart row |
| 3 | 16 | 0 | Chain Rifle, Panzerfaust, Heavy Pistol, DA CCW; Camouflage (1 Use) | — |
| 4 | 16 | 0 | Chain Rifle, Tactical Bow, Shock Mine, Heavy Pistol, DA CCW; Camouflage (1 Use) | — |
| 5 | 17 | 0 | Chain Rifle, Tactical Bow (+1B), Panzerfaust, Heavy Pistol, DA CCW; Camouflage (1 Use) | — |

### Richard Quinn

**ID 1490 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 13 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. MSV1, Warhorse, Immunity (ARM).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 0 | MULTI Marksman Rifle, Flash Pulse, D-Charges, Boarding Pistol (+1B), CCW; Forward Observer | Wildcard max 1; Counts as Fennec, Kestrel |
| 3 | 26 | 0 | MULTI Rifle, Flash Pulse, D-Charges, Disco Baller, Boarding Pistol (+1B), CCW; Forward Observer | Wildcard max 1; Counts as Fennec, Kestrel |

### Tikbalangs

**ID 33 · AVA 2 · TAG** — `MOV 15-10 | CC 17 | BS 15 | PH 15 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`. ECM: Guided (-6), Remote Presence, BS Attack (SR-1), Courage, GizmoKit (PH=13), Mimetism (-3), Tactical Awareness, Terrain (Total), Climbing Plus, Dodge (PH=11).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 69 | 1.5 | HMG, Heavy Flamethrower, Shock Mine, AP CCW; Crabbot | ARMORED required-choice, max 2 |
| 4 | 73 | 1.5 | Same; Lieutenant (+1 Order); Crabbot | ARMORED required-choice, max 2 |

### Machinists

**ID 15 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`. Deactivator, GizmoKit, Engineer.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 15 | 0 | Combi Rifle, D-Charges, Pistol, CCW | — |
| 8 | 16 | 0 | Same; Deployable Cover | — |
| 9 | 18 | 0 | Same; Armed Turret (Combi Rifle) | — |

### Emily Handelman

**ID 1072 · AVA 1 · LI** — `MOV 10-10 | CC 17 | BS 13 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. X Visor, Courage, Mimetism (-3), Number 2, Forward Observer, Dogged.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 22 | 0 | E/M Grenade Launcher, Nanopulser, Flash Pulse, Assault Pistol, CCW | Wildcard max 1; Counts as Fennec, ColCorp |
| 3 | 24 | 0 | Combi Rifle, Grenade Launcher, E/M Grenade Launcher, Nanopulser, Flash Pulse (+1B), Assault Pistol, CCW | Wildcard max 1; Counts as Fennec, ColCorp |

### Optimate Agent Maximus

**ID 1862 · AVA 1 · MI** — `MOV 15-5 | CC 22 | BS 13 | PH 13 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Albedo (-6), CC Attack (-6), Courage, Dodge (+2.5), Natural Born Warrior, Immunity (ARM), Number 2, Specialist Operative, Tactical Awareness, NWI, Cube 2.0.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 48 | 1 | MAXIMUS AGENT; AP Thunderbolt (+2B), E/M Carbine, Heavy Pistol, AP+DA CCW; Minimus Peripheral | FENNECS max 1; chart has no FTO marker |
| 2 | 45 | 1 | **MAXIMUS AGENT FTO**; same core weapons; TinBot (Repeater), no Minimus | FENNECS max 1 |
| 3 | 48 | +1 | MAXIMUS AGENT; option 1 + Lieutenant; Minimus Peripheral | FENNECS max 1; chart has no FTO marker |
| 4 | 45 | +1 | **MAXIMUS AGENT FTO**; option 2 + Lieutenant; no Minimus | FENNECS max 1 |

**Fireteam source note:** the FENNECS chart member is named `MAXIMUS AGENT` with no `FTO` marker/comment. InfinityDB therefore does not project a chart-level loadout restriction for this row. Preserve that distinction rather than inferring an FTO-only restriction from the existence of FTO loadouts.

**Selection constraint:** the Army source states: `There can only be one Maximus in each Army List.`

### Bulleteer Armbots

**ID 35 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Repeater, Remote Presence, Courage, Mimetism (-6).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Heavy Shotgun (+1B), PARA CCW (-3) | ARMORED optional max 1 |
| 2 | 22 | 1 | Spitfire, PARA CCW (-3) | ARMORED optional max 1 |

### Drummers Mobile Support Section

**ID 1806 · AVA 4 · LI** — `MOV 10-10 | CC 14 | BS 13 | PH 10 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`. 360º Visor. Each option includes its listed Drumbot Peripheral package.

| Opt | Pts | SWC | Controller / Peripheral package | FT |
|---:|---:|---:|---|---|
| 1 | 40 | 1 | Marksman Rifle, Pistol, CCW + Drumbot-1 (MULTI HMG) | — |
| 2 | 42 | 1.5 | Marksman Rifle, Pistol, CCW + Drumbot-2 (HRMC) | — |
| 3 | 40 | 1 | Marksman Rifle, Pistol, CCW + Drumbot-3 (Feuerbach, Neurocinetics) | — |
| 4 | 42 | 1 | Marksman Rifle, Pistol, CCW; Forward Deployment (+10) + Drumbot-4 (Mk12, Heavy Rocket Launcher) | — |
| 5 | 21 | 0 | Marksman Rifle, Flash Pulse, Pistol, CCW; Forward Observer + Drumbot-5 | — |
| 6 | 28 | 1.5 | MULTI Sniper Rifle, Flash Pulse, Pistol, CCW; BS Attack (-3), Forward Observer + Drumbot-5 | — |
| 7 | 47 | 1 | Marksman Rifle, Flash Pulse, Pistol, CCW; Forward Observer + Drumbot-1 + Drumbot-5 | — |
| 8 | 47 | 1 | Marksman Rifle, Flash Pulse, Pistol, CCW; Forward Observer + Drumbot-3 + Drumbot-5 | — |

Drumbots are REM Peripherals with 360º Visor, Mimetism (-3), Courage and Peripheral (Synchronized); use the pinned source for exact disabled Peripheral sub-option payloads if a rules interaction depends on them.

### Team Crux Father-Knights

**ID 1815 · AVA 1 · HI** — `MOV 15-5 | CC 22 | BS 14 | PH 14 | WIP 13 | ARM 5 | BTS 6 | W 2 | S 2`. Albedo, Martial Arts L2, BS Attack (+1SD), Berserk, Courage, Specialist Operative, Stealth, Religious Troop.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 47 | 0 | AP SMG, Flash Pulse, D-Charges, CrazyKoala, Pistol, DA CCW; Surprise Attack (-3), FD (+20), Hidden Deployment | — |
| 2 | 48 | 0.5 | AP SMG, Flash Pulse, D-Charges, CrazyKoala, Armed Turret (Combi Rifle), Pistol, DA CCW; Hidden Deployment, FD (+20) | — |
| 3 | 54 | 0 | MULTI Marksman Rifle, D-Charges, CrazyKoala, MULTI Pistol, DA CCW; FD (+20) | — |
| 4 | 46 | 0 | **CRUX KNIGHT FTO**; MULTI Marksman Rifle, Drop Bears, D-Charges, MULTI Pistol, DA CCW | Wildcard max 1 |
| 5 | 49 | 1.5 | **FTO**; Spitfire, Drop Bears, D-Charges, MULTI Pistol, DA CCW | Wildcard max 1 |
| 6 | 50 | 0 | **FTO**; MULTI Marksman Rifle, Drop Bears, D-Charges, MULTI Pistol, DA CCW; Strategic Deployment | Wildcard max 1 |

### Hetkari Shooters

**ID 1811 · AVA 2 · HI** — `MOV 15-5 | CC 17 | BS 14 | PH 14 | WIP 12 | ARM 5 | BTS 6 | W 2 | S 2`. Marksmanship, Combat Instinct.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 47 | 1.5 | Missile Launcher, Breaker Pistol, AP SMG, CCW | KESTREL required-choice max 1 |
| 2 | 48 | 1.5 | MULTI Red Fury, Breaker Pistol, CCW, E/Marat | KESTREL required-choice max 1 |
| 3 | 47 | 1.5 | Option 1; Lieutenant | KESTREL required-choice max 1 |
| 4 | 48 | 1.5 | Option 2; Lieutenant | KESTREL required-choice max 1 |

### Griffin Troops

**ID 1810 · AVA 3 · HI** — `MOV 15-5 | CC 16 | BS 14 | PH 12 | WIP 12 | ARM 4 | BTS 6 | W 2 | S 2`. MSV1, Courage, Terrain (Desert), Jump.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 31 | 0 | MULTI Rifle, Pulzar, Pistol, CCW | FENNECS max 1; KESTREL required-choice max 3 |
| 2 | 37 | 1.5 | HMG, Pulzar, Pistol, CCW | same |
| 3 | 38 | 1.5 | Feuerbach, Pulzar, Pistol, CCW | same |
| 4 | 37 | 1 | HMG, Pulzar, Pistol, CCW; Lieutenant | same |

Equivalence labels: **Counts as Fennec** in the FENNECS row; **Counts as Kestrel** in the KESTREL row.

### Bipandra

**ID 46 · AVA 1 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Dodge, Immunity (Shock), Doctor, MediKit (+1B).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Combi Rifle, Nanopulser (+1B), Pistol, CCW | Wildcard max 1; Counts as Fennec, Kestrel |
| 2 | 25 | 0 | Same; Tactical Awareness | Wildcard max 1; Counts as Fennec, Kestrel |

### Squalos Mk-II

**ID 1651 · AVA 2 · TAG** — `MOV 15-10 | CC 18 | BS 15 | PH 15 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`. ECM: Guided (-6), BS Attack (+1SD), Courage, Dodge, Combat Instinct, Remote Presence, Tactical Awareness.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 55 | 1 | MULTI Marksman Rifle, MULTI Pistol (+1B), CCW; Crabbot | ARMORED required-choice max 2 |
| 2 | 62 | 1.5 | HMG, Grenade Launcher, MULTI Pistol (+1B), CCW | ARMORED required-choice max 2 |
| 3 | 66 | 1.5 | MULTI HMG, MULTI Pistol (+1B), CCW; NCO | ARMORED required-choice max 2 |

### Banshees Airborne Assault Unit

**ID 1807 · AVA 3 · MI** — `MOV 10-10 | CC 15 | BS 12 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. MSV1, Parachutist, Combat Jump, Super-Jump (Jet Propulsion).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Light Shotgun, Pulzar (+1B), D-Charges, Pistol, CCW | — |
| 2 | 22 | 0 | SMG, Pulzar (+1B), D-Charges, WildParrot, Pistol, CCW | — |
| 3 | 25 | 0.5 | SMG, Pulzar (+1B), D-Charges, Pistol, CCW; Hacking Device | — |
| 4 | 23 | 0 | SMG, Pulzar (+1B), D-Charges, Pistol, CCW; Killer Hacking Device | — |

### Dr. Priya Harper

**ID 1814 · AVA 1 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Nanoscreen, X Visor, Booty, Dodge, Immunity (Shock), Specialist Operative, NWI, No Cover, Tactical Awareness.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 32 | +1 | **DR HARPER FTO**; Plasma Carbine, Nanopulser, E/M Mine, Viral Pistol (+1B), CCW | Wildcard max 1 |
| 2 | 35 | +1 | Same weapons; Forward Deployment (+20) | — |

### Knauf

**ID 939 · AVA 1 · LI** — `MOV 10-10 | CC 21 | BS 13 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. MSV1, Courage, Mimetism (-3), Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 31 | 1.5 | MULTI Sniper Rifle, AP Heavy Pistol, CCW; Surprise Attack (-3), Decoy (1) | — |

### Warcors

**ID 50 · AVA 1 · LI · Irregular** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Journalist.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor | — |
| 2 | 3 | 0 | Same; Sixth Sense | — |

### Maximus, Optimate and HexaDome Legend

**ID 1720 · AVA 1 · TAG** — `MOV 15-10 | CC 24 | BS 14 | PH 13 | WIP 13 | ARM 6 | BTS 6 | W 4 | S 6`. ECM: Guided (-6), CC Attack (-6), BS Attack (SR-1), Courage, Dodge, Natural Born Warrior, Immunity (ARM), Tactical Awareness, Transmutation (Escape System), Cube 2.0.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 82 | 1.5 | AP HMG, E/M Carbine, Heavy Pistol, AP+DA CCW | ARMORED optional max 1 |
| 2 | 80 | 1 | AP Thunderbolt (+2B), E/M Carbine, Heavy Pistol, AP+DA CCW | ARMORED optional max 1 |
| 3 | 82 | 0 | AP HMG, E/M Carbine, Heavy Pistol, AP+DA CCW; Lieutenant | ARMORED optional max 1 |

Only one Maximus may be selected across Agent Maximus and TAG Maximus.

### Dart, Optimate Huntress

**ID 1130 · AVA 1 · SK** — `MOV 10-10 | CC 16 | BS 13 | PH 13 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. MSV1, Surprise Attack (-3), Camouflage, Courage, Forward Deployment (+20), Mimetism (-3), Immunity (Shock), Stealth, NWI, Terrain (Total), Climbing Plus, Specialist Operative, Decoy (1).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 35 | 0 | AP SMG, Pistol, CCW, Viral Tactical Bow, E/M Grenades | — |
| 2 | 35 | 0 | Same; Shock Mine | — |
| 3 | 36 | 0.5 | Same; Shock Mine, Minelayer | — |
| 4 | 42 | 0.5 | Same; Minelayer; Sharvara K9 Peripheral | — |

### Sāchā Xenotech Hunters

**ID 1874 · AVA 1 · LI · Irregular** — `MOV 10-10 | CC 17 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`. Forward Deployment (+10), Booty, Terrain (Total), Climbing Plus, Specialist Operative.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 6 | 0 | Flash Pulse, E/M Grenades (+1B), Stun Pistol (+1B), CCW | — |

### Kazurabā Ruby Monday

**ID 1890 · AVA 1 · HI · Irregular** — `MOV 15-5 | CC 18 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 6 | W 2 | S 2`. BS Attack (+1B), Booty, Dodge, Immunity (IMM-B), Technorganic, Terrain (Total), Climbing Plus, Specialist Operative.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Adhesive Launcher Rifle, Flash Pulse, E/M Grenades, Stun Pistol, CCW | — |

## Fireteams

This section is **canonical**. The Unit → Fireteam index below is derivative.

### Chart limits

| Type | Raw source | Meaning |
|---|---:|---|
| Core | 1 | Maximum 1 |
| Haris | 1 | Maximum 1 |
| Duo | 256 | InfinityDB-normalized meaning: unlimited |

InfinityDB explicitly maps raw Fireteam limit `256` to `unlimited`.

### FENNECS Fireteam

**Types:** Core, Haris

| Member | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---|---|---|
| Fennec | 1 | 5 | No | — | — |
| Black A.I.R. FTO | 0 | 2 | No | — | FTO |
| Griffin | 0 | 1 | No | Fennec | — |
| Magistrate | 0 | 1 | No | — | — |
| Maximus Agent | 0 | 1 | No | — | **None in chart row** |
| Indigo | 0 | 1 | No | Spec-Ops | Optional Spec-Ops mode |

At least one Fennec is required by explicit `min: 1`.

### KESTREL Fireteams

**Types:** Duo, Haris

| Member | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---|---|---|
| Griffin | 0 | 3 | Yes | Kestrel | — |
| Firefly | 0 | 3 | Yes | Kestrel | — |
| Hetkari | 0 | 1 | Yes | — | — |

The `required: true` rows form the required-choice set recorded by the source projection: the team needs an eligible required-choice member; it does not require all three unit types simultaneously.

### ARMORED Fireteams

**Type:** Duo

| Member | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---|---|---|
| Tikbalang | 0 | 2 | Yes | — | — |
| Squalo Mk-II | 0 | 2 | Yes | — | — |
| Maximus Optimate | 0 | 1 | No | — | — |
| Firefly | 0 | 1 | No | — | — |
| Bulleteer | 0 | 1 | No | — | — |

A legal ARMORED team requires an eligible Tikbalang or Squalo Mk-II from the required-choice set.

### COLCORP Fireteams

**Types:** Duo, Haris

| Member | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---|---|---|
| Magistrate | 1 | 2 | No | ColCorp | — |
| Jackal FTO | 0 | 2 | No | ColCorp | FTO |
| Beasthunter FTO | 0 | 1 | No | — | FTO |

At least one Magistrate is required by explicit `min: 1`.

### Wildcards

All rows below are in the chart's **Wildcards** Fireteam row. Parenthetical values are **Counts-as labels**, not join-scope restrictions.

| Wildcard | Max | Counts as | FTO restriction |
|---|---:|---|---|
| Crux Knight | 1 | — | FTO |
| Pathfinder Dronbot | 1 | — | — |
| Bipandra | 1 | Fennec, Kestrel | — |
| Dr. Harper | 1 | — | FTO |
| Quinn | 1 | Fennec, Kestrel | — |
| Sforza | 1 | — | FTO |
| Emily | 1 | Fennec, ColCorp | — |

Wildcard status does not remove a Fireteam's native minimum/required-choice conditions.

## Unit → Fireteam access index

| Unit | Access |
|---|---|
| Sierra Dronbot | — |
| Clipper Dronbot | — |
| Fugazi Dronbot | — |
| Scarecrows | — |
| Fennec Fusiliers | FENNECS Core/Haris; native; min 1 Fennec in that formation |
| Fireflies | KESTREL Duo/Haris required-choice, max 3, Counts as Kestrel; ARMORED Duo optional max 1 |
| Peacemaker | — |
| Tech-Bee | — |
| Redeye | — |
| Pathfinder | Wildcard max 1 in legal Kestrel Fireteams |
| Palbot | — |
| Blink Team | — |
| BCA Magistrate | FENNECS max 1; COLCORP min 1/max 2 and Counts as ColCorp |
| Beasthunter | COLCORP max 1, FTO only |
| Black A.I.R. | FENNECS max 2, FTO only |
| Sforza | Wildcard max 1, FTO only |
| Trauma-Doc | — |
| Mulebot | — |
| Minescorp Jackal | COLCORP max 2, FTO only, Counts as ColCorp |
| Yamabushi | —; FTO-labelled loadouts have no Kestrel chart row |
| Quinn | Wildcard max 1; Counts as Fennec/Kestrel |
| Tikbalang | ARMORED required-choice, max 2 |
| Machinist | — |
| Emily | Wildcard max 1; Counts as Fennec/ColCorp |
| Optimate Agent Maximus | FENNECS max 1; chart row has no FTO marker |
| Bulleteer | ARMORED optional max 1 |
| Drummers | — |
| Crux Knight | Wildcard max 1, FTO only |
| Hetkari | KESTREL required-choice max 1 |
| Griffin | FENNECS max 1, Counts as Fennec; KESTREL required-choice max 3, Counts as Kestrel |
| Bipandra | Wildcard max 1; Counts as Fennec/Kestrel |
| Squalo Mk-II | ARMORED required-choice, max 2 |
| Banshee | — |
| Dr. Harper | Wildcard max 1, FTO only |
| Knauf | — |
| Warcor | — |
| Maximus TAG | ARMORED optional max 1 |
| Dart | — |
| Sāchā | — |
| Ruby Monday | — |
| Indigo Spec-Ops | FENNECS max 1 when Spec-Ops mode is in use |
| Indigo Team-Ops | — in the ordinary Kestrel chart |

## Tactical tags

Derived analysis aids, not official characteristics.

| Unit | Tags |
|---|---|
| Fennec | cheap order, Lieutenant, hacker, Sensor/FO, Disco Baller, Minelayer, long-range gun |
| Firefly | NCO, Engineer, CoC, hacker, deployable repeater, mine/turret support, link anchor |
| Magistrate | Strategos Lieutenant, Counterintelligence, CoC, Jackal support |
| Jackal | cheap irregular, FTO filler, infiltration, E/M attack, Minelayer |
| Griffin | durable HI gunfighter, MSV1, Lieutenant, flexible Fireteam member |
| Hetkari | heavy long-range gunfighter, Lieutenant, KESTREL anchor |
| Tikbalang | mobile TAG, TacAware, Mimetism, Climbing Plus, Lieutenant, ARMORED anchor |
| Squalo Mk-II | TAG gunfighter, TacAware, NCO option, ARMORED anchor |
| Pathfinder | Sensor/FO, Repeater, TacAware option, Wildcard |
| Mulebot | Baggage, EVO, cheap support, TR option |
| Scarecrow | hidden/infiltrating hacker or KHD, repeater/mines, midfield specialist |
| Black A.I.R. | MSV2, FTO hacker/FO/sniper, airborne KHD option |
| Banshee | airborne attacker/specialist, hacker/KHD |
| Redeye | fast aerial attack/support, Sensor, Mimetism (-6) |
| Crux Knight | premium HI specialist, hidden-deployment options, FTO Wildcard |
| Emily | E/M grenade launcher, FO, Wildcard, Fennec/ColCorp equivalence |
| Quinn | MSV1 gunfighter/FO, Disco Baller option, Wildcard, Fennec/Kestrel equivalence |
| Bipandra | Doctor, TacAware option, Wildcard, Fennec/Kestrel equivalence |
| Dr. Harper | specialist, TacAware, FTO Wildcard |
| Bulleteer | fast Mimetism (-6) REM gunfighter, ARMORED Duo support |
| Peacemaker | forward-deployed repeater/attack REM |
| Dart | camouflaged midfield specialist/attacker |
| Beasthunter | cheap FTO template/Panzerfaust or camouflaged midfield attack |
| Yamabushi | CC/short-range attack, camo variants; no Kestrel Fireteam access |

## Validation and maintenance

- Standard roster represented: **40 units**.
- Optional-mode hooks: Indigo Spec-Ops and Indigo Team-Ops.
- Canonical Fireteam rows represented: **FENNECS, KESTREL, ARMORED, COLCORP, Wildcards**.
- Limits preserved: `CORE 1`, `HARIS 1`, raw `DUO 256` = InfinityDB `unlimited`.
- Parenthetical source comments are stored as Counts-as/equivalence labels.
- FTO restrictions are applied only where the Fireteam member row itself contains an FTO marker/comment.
- No Fireteam access is inferred solely from a loadout having `FTO` in its name.
- Agent Maximus is deliberately **not** marked FTO-only because its chart row is `MAXIMUS AGENT` without an FTO marker.
- Yamabushi is deliberately shown with no Fireteam access despite having FTO-labelled profiles because there is no Kestrel chart row for Yamabushi.
- Maximus unique-character constraint is recorded.
- Linked Reinforcement section Code: Capital (`army_id: 199`) has no pinned `fireteamChart` to merge.

### Refresh rule

When a newer Army source revision or InfinityDB normalization supersedes the provenance above, set `status: stale` until roster/profile/Fireteam changes are reconciled. Do not silently mix newer live values into this file without updating the provenance block.

## TAG tactical cross-reference (2026-10-23)

**Default decision:** solo **Tikbalang LT (+1 Order)** for an aggressive high-order mobile gun *when the LT can be protected*; **Squalos NCO MULTI HMG** into armor or **HMG+GL** for inaccessible opponents; **Maximus TAG** only for CC/Immunity matchups. A **Tik LT + Pathfinder Duo does not gain two extra Duo activations** from the Tik's personal LT Orders. Compare the full partner cost and retain mission specialists. [Existing deeper tactical review](../../notes/factions/kestrel.md).

Cross-faction **apex vs points-value** comparisons, matchup table, and direct MCP-reviewed podcast/video sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Current profile and Fireteam legality above remain authoritative.

## Vehicle (VH) tactical cross-reference (2026-10-23)

**Redeye AVA2:** BS14, ARM6, Mimetism(-6), Sensor and 20–5 Aerial movement. Choose **37/1.5 Blitzen** for mobile E/M ARO; **38/1.5 Continuous Damage GL** for speculative/high-angle attacks. **Irregular Order #52 (Sep 2026)** proposes **double Redeye** with a Magistrate/Jackal/Fennec shell; **Shepherd** argues paying 3 SWC for two B4 Spitfires leaves too few elite ARO-clearing guns. Plan two safe S7 hiding points, Engineer/GizmoKit rescue and ground scorers; Redeyes cannot directly touch objectives.

See [VH apex/value tier list and matchup guide](../../notes/list-building/vehicles-vh.md). **This sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative.**

## Hacker and KHD tactical cross-reference (2026-10-23)

**Best rate:** **Fennec HD + FastPanda 16/0.5** cheaply moves the network forward, but WIP12 requires a backup. **Black A.I.R. FTO HD 26/0.5** adds **Combat Instinct** and MSV2/Mimetism(-3): with a real Repeater net it can deny Stealth and defend the Fennec link. **Scarecrow Camo KHD 27/0 vs HD 29/0.5** trades points for midfield mission safety; **Banshee KHD 23/0 vs HD 25/0.5** is an AD scoring/late hacker attack, not a Turn-0 network member. **Why:** don't confuse defending a wide network (Black A.I.R.) with cheaply projecting it (Fennec) or crossing the table (Banshee/Scarecrow). Check FTO chart before claiming a TinBot/bonus.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**
