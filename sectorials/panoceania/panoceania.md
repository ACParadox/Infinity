---
schema_version: 1
reference_type: faction
status: current
faction_id: 101
faction_slug: panoceania
faction_name: PanOceania
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard generic PanOceania roster and loadouts. Generic PanOceania has no standard Fireteam chart. Spec-Ops and Team-Ops are optional-mode hooks; RacerBots are components of Pilot-X Team rather than independent roster entries."
---

# PanOceania

## Overview and provenance

Repository-native reference for **generic / vanilla PanOceania** roster, profiles, points/SWC, and AVA.

Sources used:

- Army-derived PanOceania source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- InfinityDB normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4` where relevant.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **51-unit standard generic PanOceania roster** in the pinned Army source.
- The Army document contains 54 non-empty-faction source entries: 51 standard logical units, `Indigo Spec-Ops`, `Indigo Team-Ops`, and the `RacerBots` component entry used by `Pilot-X Team`.
- Soldier of Fortune entries with empty faction lists are excluded from the base roster.
- `Indigo Spec-Ops` and `Indigo Team-Ops` are optional game-mode content and are listed separately.
- `RacerBots Mk-III` cannot be selected independently; they are part of a `Pilot-X Team` package.
- Generic PanOceania has **no standard Fireteam chart**. `FTO` in a loadout name remains part of the Army profile name but does not create Fireteam access in vanilla.
- Vanilla AVA is taken from the canonical PanOceania profile group, not inherited from a sectorial. This matters for units such as Cutter, Swiss Guard, Tikbalang, Redeye, Hetkari, BCA Magistrate, Blink Team, Helot, Zulu-Cobra, Bolts, and others.
- Linked Reinforcement section: **Code: Capital** (`army_id: 199`). Reinforcement content is not merged into this base-roster reference.

## Selection constraints

- **Joan of Arc:** only one Joan may be selected across `Joan of Arc` (ID 20) and `Joan of Arc v2 / Mobility Armor` (ID 42).
- **Maximus:** only one Maximus may be selected across `Optimate Agent Maximus` (ID 1862) and `Maximus, Optimate and HexaDome Legend` (ID 1720).
- **Pilot-X Team:** one Pilot-X plus zero to two RacerBots Mk-III; RacerBots cannot be selected without Pilot-X, and all members of the Team must be in the same Combat Group.

## Roster index

| Unit | ID | AVA | Type | Order |
|---|---:|---:|---|---|
| Pathfinder Dronbot | 16 | 2 | REM | Regular |
| Dr. Priya Harper, Archeo-raider | 1814 | 1 | LI | Regular |
| Helot Militia | 1222 | 2 | LI | Irregular |
| Bulleteer Armbots | 35 | 2 | REM | Regular |
| Tech-Bees | 935 | 1 | LI | Regular |
| Teutonic Knights | 30 | 2 | HI | Regular |
| Zulu-Cobra | 1216 | 2 | LI | Regular |
| Neoterra Bolts | 4 | 3 | MI | Regular |
| Cutters, Varuna Naval Chasseurs | 12 | 1 | TAG | Regular |
| Nøkken | 1484 | 2 | LI | Regular |
| Banshees Airborne Assault Unit | 1807 | 2 | MI | Regular |
| Motorized Bounty Hunters | 1565 | 1 | LI | Irregular |
| Joan of Arc v2 (Mobility Armor) | 42 | 1 | HI | Regular |
| Pilot-X Team | 1903 | 1 team | LI + REM | Regular |
| Sierra Dronbot | 17 | 2 | REM | Regular |
| Palbots | 37 | 2 | REM | Peripheral |
| Karhu Special Group | 1485 | 2 | MI | Regular |
| Nisses | 3 | 2 | MI | Regular |
| Swiss Guard | 9 | 1 | HI | Regular |
| Tikbalangs | 33 | 1 | TAG | Regular |
| Team Crux Father-Knights | 1815 | 1 | HI | Regular |
| Fusilier Indigo Bipandra | 46 | 1 | LI | Regular |
| Locust, Clandestine Action Team | 769 | 2 | SK | Regular |
| Maximus, Optimate and HexaDome Legend | 1720 | 1 | TAG | Regular |
| Croc Men | 13 | 2 | SK | Regular |
| Squalos Mk-II | 1651 | 2 | TAG | Regular |
| Fugazi Dronbot | 19 | 2 | REM | Regular |
| Fennec Fusiliers | 1803 | 5 | LI | Regular |
| BCA Magistrates | 1804 | 1 | LI | Regular |
| Mulebots | 38 | 2 | REM | Regular |
| Blade-Ops | 1751 | 2 | LI | Regular |
| Aquila Guard | 8 | 1 | HI | Regular |
| Drummers Mobile Support Section | 1806 | 2 | LI | Regular |
| Fusiliers | 1 | Total | LI | Regular |
| Redeye Close Air Support Squad | 1816 | 1 | VH | Regular |
| Hetkari Shooters | 1811 | 1 | HI | Regular |
| ORC Troops | 5 | 2 | HI | Regular |
| Optimate Agent Maximus | 1862 | 1 | MI | Regular |
| Clipper Dronbot | 18 | 2 | REM | Regular |
| Blink Team | 1805 | 1 | LI | Regular |
| Peacemaker Armbots | 36 | 2 | REM | Regular |
| Black A.I.R. | 1808 | 1 | MI | Regular |
| Joan of Arc | 20 | 1 | HI | Regular |
| Patsy Garnett | 1225 | 1 | HI | Regular |
| Griffin Troops | 1810 | 2 | HI | Regular |
| Warcors | 50 | 1 | LI | Irregular |
| Machinists | 15 | 1 | LI | Regular |
| Fireflies Clandestine Demo Squad | 1809 | 2 | MI | Regular |
| Scarecrows Active Recon Group | 1812 | 2 | SK | Regular |
| Blockers, Attached Agents of the CDCI | 1750 | 1 | LI | Regular |
| Trauma-Docs | 14 | 1 | LI | Regular |

Optional-mode units:

| Unit | ID | Mode | Notes |
|---|---:|---|---|
| Indigo Spec-Ops | 1912 | Spec-Ops | Optional-mode hook; not an ordinary matched-play roster entry |
| Indigo Team-Ops | 1926 | Team-Ops | Optional-mode hook; not an ordinary matched-play roster entry |

## Unit details

### Pathfinder Dronbot

**ID 16 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Deactivator, Remote Presence, Courage, Triangulated Fire, Forward Observer, Sensor.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 14 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3) |
| 2 | 17 | 0 | As 1; Tactical Awareness |

### Dr. Priya Harper, Archeo-raider

**ID 1814 · AVA 1 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Nanoscreen, X Visor, Booty, Dodge, Immunity (Shock), Specialist Operative, NWI, No Cover, Tactical Awareness.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 32 | +1 | **DR HARPER FTO**; Plasma Carbine, Nanopulser, E/M Mine, Viral Pistol (+1B), CCW |
| 2 | 35 | +1 | Same weapons; Forward Deployment (+20) |

### Helot Militia

**ID 1222 · AVA 2 · LI · Irregular** — `MOV 10-10 | CC 12 | BS 11 | PH 10 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. No Cube, Immunity (Shock), Neurocinetics, Terrain (Aquatic), Stealth.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 11 | 0 | **HELOT MILITIAMAN FTO**; Shock Marksman Rifle, Pistol, CCW; Sensor |
| 3 | 13 | 1 | **HELOT MILITIAMAN FTO**; Red Fury, Pistol, CCW; Sensor |
| 4 | 10 | 0 | **HELOT MILITIAMAN FTO**; SMG, Light Rocket Launcher, Pistol, CCW; Sensor |
| 5 | 13 | 0 | Shock Marksman Rifle, Pistol, CCW; Camouflage (1 Use), Surprise Attack (-3) |
| 6 | 17 | 1.5 | MULTI Sniper Rifle, Pistol, CCW; Camouflage (1 Use), Surprise Attack (-3) |
| 7 | 15 | 1 | Red Fury, Pistol, CCW; Camouflage (1 Use), Surprise Attack (-3) |
| 8 | 12 | 0 | SMG, Light Rocket Launcher, Pistol, CCW; Camouflage (1 Use), Surprise Attack (-3) |

### Bulleteer Armbots

**ID 35 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Repeater, Remote Presence, Courage, Mimetism (-6).

| Opt | Pts | SWC | Loadout |
|---:|---:|---|
| 1 | 19 | 0 | Heavy Shotgun (+1B), PARA CCW (-3) |
| 2 | 22 | 1 | Spitfire, PARA CCW (-3) |

### Tech-Bees

**ID 935 · AVA 1 · LI** — `MOV 10-10 | CC 12 | BS 11 | PH 10 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 2`. Specialist Operative, TAGCom, Deactivator, GizmoKit.

| Opt | Pts | SWC | Loadout |
|---:|---:|---|
| 2 | 9 | 0 | Adhesive Launcher Rifle, Flash Pulse, Pistol, PARA CCW (-3); Deployable Repeater |

### Teutonic Knights

**ID 30 · AVA 2 · HI** — `MOV 15-5 | CC 22 | BS 13 | PH 14 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`. Martial Arts L2, Limited Cover, Impetuous, Religious Troop, Terrain (Jungle), enhanced Dodge.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 18 | 0 | Light Shotgun, Panzerfaust, Pistol, DA CCW |
| 2 | 19 | 0 | As 1; TinBot: Firewall (-3) |
| 3 | 28 | 1.5 | Missile Launcher, Zapper, Pistol, DA CCW |
| 5 | 19 | 0 | SMG, Panzerfaust, Pistol, DA CCW; Specialist Operative |
| 6 | 29 | 1.5 | Spitfire, Pistol, DA CCW; X Visor, NCO |
| 7 | 18 | 0 | Lieutenant; Light Shotgun, Panzerfaust, Pistol, DA CCW |

### Zulu-Cobra

**ID 1216 · AVA 2 · LI** — `MOV 10-10 | CC 14 | BS 13 | PH 11 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Camouflage, Surprise Attack (-3), Forward Deployment (+10), Mimetism (-3), Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 27 | 1 | Spitfire, Assault Pistol, E/M Mine, CCW |
| 2 | 23 | 0 | Combi Rifle, Jammer, Assault Pistol, CCW; Sensor, Triangulated Fire |
| 3 | 26 | 0 | Breaker Combi Rifle, Pitcher, Assault Pistol, CCW; Killer Hacking Device |
| 4 | 24 | 0 | Breaker Combi Rifle, Flash Pulse, Assault Pistol, CCW; Forward Observer |
| 5 | 23 | 0 | Combi Rifle, Jammer, Assault Pistol, CCW; Lieutenant, Sensor, Triangulated Fire |
| 6 | 26 | 0.5 | MULTI Marksman Rifle, E/M Mine, Assault Pistol, CCW; X Visor, Minelayer |

### Neoterra Bolts

**ID 4 · AVA 3 · MI** — `MOV 10-10 | CC 16 | BS 13 | PH 11 | WIP 12 | ARM 2 | BTS 6 | W 1 | S 2`. Warhorse, Immunity (Shock), Marksmanship, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 2 | 21 | 0 | Combi Rifle, Light Shotgun, Drop Bears, Pistol, CCW |
| 3 | 19 | 0 | Boarding Shotgun (+1B), Drop Bears, Pistol, CCW |
| 4 | 24 | 1.5 | Missile Launcher, Pistol, CCW |
| 5 | 25 | 1.5 | Spitfire, Pistol, CCW |
| 6 | 26 | 0 | Combi Rifle, Light Shotgun, Drop Bears; Chain of Command |
| 7 | 24 | 0.5 | Boarding Shotgun (+1B), E/M Mine; Hacking Device |
| 8 | 22 | 0 | Boarding Shotgun (+1B), E/M Mine; Killer Hacking Device |
| 9 | 23 | 0 | Combi Rifle, Light Shotgun, Drop Bears; MediKit, Paramedic |
| 10 | 26 | 1.5 | MULTI Sniper Rifle; MSV1 |
| 11 | 21 | 0 | Lieutenant; Combi Rifle, Light Shotgun, Drop Bears |

### Cutters, Varuna Naval Chasseurs

**ID 12 · AVA 1 · TAG** — `MOV 15-10 | CC 18 | BS 15 | PH 15 | WIP 12 | ARM 8 | BTS 6 | W 3 | S 7`. ECM: Guided (-6), Camouflage, Hidden Deployment, Surprise Attack (-3), Mimetism (-6), Remote Presence, Courage, Dodge (PH=11), GizmoKit (PH=13), Terrain (Aquatic), BS Attack (SR-1).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 97 | 2 | MULTI HMG, CCW (PS=5); NCO; Crabbot |
| 2 | 95 | 2.5 | MULTI HMG, CCW (PS=5); Lieutenant; Crabbot |

### Nøkken

**ID 1484 · AVA 2 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Bangbomb (+4), Forward Deployment (+20), Mimetism (-6), Terrain (Total).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 26 | 1.5 | Spitfire, Pistol, CCW |
| 2 | 27 | 0.5 | Combi Rifle, Light Shotgun; Hacking Device |
| 3 | 25 | 0 | Combi Rifle, Light Shotgun; Killer Hacking Device |
| 4 | 24 | 0.5 | Combi Rifle, Light Shotgun, Shock Mine; Minelayer |
| 5 | 22 | 0 | Boarding Shotgun (+1B), Panzerfaust, Flash Pulse; Forward Observer |
| 6 | 24 | 0 | Boarding Shotgun (+1B), Panzerfaust; MSV1 |

### Banshees Airborne Assault Unit

**ID 1807 · AVA 2 · MI** — `MOV 10-10 | CC 15 | BS 12 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. MSV1, Parachutist, Combat Jump, Super-Jump (Jet Propulsion).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 19 | 0 | Light Shotgun, Pulzar (+1B), D-Charges, Pistol, CCW |
| 2 | 22 | 0 | SMG, Pulzar (+1B), D-Charges, WildParrot, Pistol, CCW |
| 3 | 25 | 0.5 | SMG, Pulzar (+1B), D-Charges, Pistol, CCW; Hacking Device |
| 4 | 23 | 0 | SMG, Pulzar (+1B), D-Charges, Pistol, CCW; Killer Hacking Device |

### Motorized Bounty Hunters

**ID 1565 · AVA 1 · LI · Irregular · Impetuous** — `MOV 20-15 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Motorcycle, Booty (ReRoll), Limited Cover, Dodge (+5), Mimetism (-3).

| Opt | Pts | SWC | Loadout |
|---:|---:|---|
| 1 | 8 | 0 | Boarding Shotgun, Heavy Riotstopper, Pistol, PARA CCW (-6) |
| 2 | 9 | 0 | SMG, Chain-colt (+1B), Pistol, PARA CCW (-6) |
| 3 | 16 | 0.5 | Red Fury, Breaker Pistol, PARA CCW (-6) |

### Joan of Arc v2 (Mobility Armor)

**ID 42 · AVA 1 · HI** — `MOV 15-5 | CC 23 | BS 15 | PH 14 | WIP 15 | ARM 3 | BTS 6 | W 2 | S 2`. Martial Arts L3, Inspiring Leadership, Frenzy, NWI, Stealth, Religious Troop, Tactical Awareness, Number 2, Terrain (Total), X Visor.

All profiles: AP Spitfire, Pulzar (+1B), Pistol, EXP CCW.

| Opt | Pts | SWC | Differences |
|---:|---:|---:|---|
| 2 | 45 | 1.5 | Chain of Command; Non-Specialist |
| 3 | 51 | 1.5 | Chain of Command; Non-Specialist; Strategic Deployment |
| 4 | 45 | 1 | Lieutenant |
| 5 | 49 | 1 | Lieutenant (+1 Command Token) |
| 6 | 51 | 1 | Lieutenant; Strategic Deployment |

Only one Joan of Arc may be selected across IDs 20 and 42.

### Pilot-X Team

**ID 1903 · AVA 1 Team**. A Pilot-X Team contains one Pilot-X and zero to two RacerBots Mk-III; RacerBots cannot be taken without Pilot-X, and all members must belong to the same Combat Group.

**Pilot-X** — `MOV 10-10 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 2`. Hacking Device (Upgrade: Zero Pain), RemDriver (+1 BS, +5 CC, BTS=6).

| Element | Pts | SWC | Loadout / differences |
|---|---:|---:|---|
| Pilot-X | 21 | 1 | E/Mitter, Flash Pulse, MULTI Pistol, PARA CCW (-3); Hacker |
| RacerBot Mk-III | 8 each | 0 | Deployable Repeater, Light Riotstopper, Mine Dispenser (PARA), Stun Pistol, PARA CCW (-6); 360º Visor, Bangbomb (+4), ECM: Hacker (-3), Remote Presence |

### Sierra Dronbot

**ID 17 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage, Total Reaction, 360º Visor.

| Opt | Pts | SWC | Loadout |
|---:|---:|---|
| 1 | 23 | 1 | HMG, PARA CCW (-3) |
| 2 | 18 | 0 | Thunderbolt (+1B), PARA CCW (-3) |

### Palbots

**ID 37 · AVA 2 · REM Peripheral** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Peripheral (Servant), Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout |
|---:|---:|---|
| 1 | 3 | 0 | PARA CCW (-3); no independent Order |

### Karhu Special Group

**ID 1485 · AVA 2 · MI** — `MOV 15-5 | CC 14 | BS 13 | PH 11 | WIP 12 | ARM 2 | BTS 3 | W 1 | S 2`. MSV1, Courage, Mimetism (-3), Climbing Plus, Terrain (Total), NCO.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 22 | 0 | MULTI Rifle, Blitzen, AP Mine, Pistol, CCW |
| 2 | 22 | 0 | MULTI Rifle, E/Marat, AP Mine, Pistol, CCW |
| 3 | 34 | 1.5 | Feuerbach (+1B), AP Mine, Pistol, CCW |
| 4 | 25 | 0 | MULTI Rifle, Blitzen, D-Charges; Engineer, Deactivator, GizmoKit |
| 5 | 24 | 0 | MULTI Rifle, Blitzen, AP Mine; MediKit, Paramedic |

### Nisses

**ID 3 · AVA 2 · MI** — `MOV 15-5 | CC 14 | BS 13 | PH 12 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 2`. MSV2, Mimetism (-3), Terrain (Total), Climb 7.5.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 2 | 31 | 1.5 | HMG, Boarding Pistol, CCW |
| 3 | 29 | 1.5 | MULTI Sniper Rifle, Boarding Pistol, CCW |
| 5 | 30 | 0.5 | Combi Rifle, Light Shotgun, Boarding Pistol, CCW; Hacking Device |
| 6 | 28 | 0 | Combi Rifle, Light Shotgun, Boarding Pistol, CCW; MediKit, Paramedic |

### Swiss Guard

**ID 9 · AVA 1 · HI** — `MOV 10-10 | CC 15 | BS 15 | PH 14 | WIP 13 | ARM 5 | BTS 6 | W 2 | S 2`. Camouflage, Hidden Deployment, Mimetism (-6), Surprise Attack (-3), Stealth.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 2 | 56 | 1.5 | HMG, Pulzar, Heavy Pistol, AP CCW |
| 3 | 60 | 1.5 | Missile Launcher (+1SD), Light Shotgun, Pulzar, Heavy Pistol, AP CCW |
| 4 | 56 | 0.5 | MULTI Rifle, Pulzar, Flammenspeer, Heavy Pistol, AP CCW; Hacking Device, X Visor |
| 5 | 44 | 0 | AP SMG, Pulzar, Flammenspeer, Heavy Pistol, AP CCW; TinBot: Firewall (-3), Martial Arts L1, CC=21, Forward Deployment (+10) |
| 6 | 47 | 0 | As 5 + Killer Hacking Device |

### Tikbalangs

**ID 33 · AVA 1 · TAG** — `MOV 15-10 | CC 17 | BS 15 | PH 15 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`. ECM: Guided (-6), Remote Presence, BS Attack (SR-1), Courage, GizmoKit (PH=13), Mimetism (-3), Tactical Awareness, Terrain (Total), Climbing Plus, Dodge (PH=11).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 69 | 1.5 | HMG, Heavy Flamethrower, Shock Mine, AP CCW; Crabbot |
| 4 | 73 | 1.5 | As 1; Lieutenant (+1 Order); Crabbot |

### Team Crux Father-Knights

**ID 1815 · AVA 1 · HI** — `MOV 15-5 | CC 22 | BS 14 | PH 14 | WIP 13 | ARM 5 | BTS 6 | W 2 | S 2`. Albedo (-6), Martial Arts L2, BS Attack (+1SD), Berserk, Courage, Specialist Operative, Stealth, Religious Troop.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 47 | 0 | AP SMG, Flash Pulse, D-Charges, CrazyKoala, Pistol, DA CCW; Surprise Attack (-3), Forward Deployment (+20), Hidden Deployment |
| 2 | 48 | 0.5 | AP SMG, Flash Pulse, D-Charges, Armed Turret (Combi Rifle), Pistol, DA CCW; Surprise Attack (-3), Forward Deployment (+20), Hidden Deployment |
| 3 | 54 | 0 | MULTI Marksman Rifle, D-Charges, CrazyKoala, MULTI Pistol, DA CCW; Forward Deployment (+20) |
| 4 | 46 | 0 | **CRUX KNIGHT FTO**; MULTI Marksman Rifle, Drop Bears, D-Charges, MULTI Pistol, DA CCW |
| 5 | 49 | 1.5 | **CRUX KNIGHT FTO**; Spitfire, Drop Bears, D-Charges, MULTI Pistol, DA CCW |
| 6 | 50 | 0 | **CRUX KNIGHT FTO**; as 4; Strategic Deployment |

### Fusilier Indigo Bipandra

**ID 46 · AVA 1 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Doctor (ReRoll -3), Dodge (+2.5), Immunity (Shock), MediKit (+1B).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 23 | 0 | Combi Rifle, Nanopulser (+1B), Pistol, CCW |
| 2 | 25 | 0 | Same; Tactical Awareness |

### Locust, Clandestine Action Team

**ID 769 · AVA 2 · SK** — `MOV 10-10 | CC 16 | BS 12 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Hidden Deployment, Mimetism (-6), Forward Deployment (+20), Stealth, Surprise Attack (-3), Bangbomb (+4), Terrain (Total).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 3 | 24 | 0 | Boarding Shotgun, Grenades, Drop Bears, Boarding Pistol, CCW; Specialist Operative |
| 4 | 27 | 0 | MULTI Marksman Rifle, Boarding Pistol, CCW |
| 5 | 21 | 0 | SMG, D-Charges, WildParrot, Boarding Pistol, CCW |
| 6 | 29 | 0.5 | Breaker Combi Rifle, Pitcher, D-Charges, Boarding Pistol, CCW; Hacking Device (Firewall -3) |
| 7 | 27 | 0 | Breaker Combi Rifle, Pitcher, D-Charges, Boarding Pistol, CCW; Killer Hacking Device (Firewall -3) |
| 8 | 31 | 0.5 | Breaker Combi Rifle, Flash Pulse, D-Charges, Boarding Pistol, CCW; Hacking Device (Firewall -3), Camouflage (1 Use) |

### Maximus, Optimate and HexaDome Legend

**ID 1720 · AVA 1 · TAG** — `MOV 15-10 | CC 24 | BS 14 | PH 13 | WIP 13 | ARM 6 | BTS 6 | W 4 | S 6`. ECM: Guided (-6), CC Attack (-6), BS Attack (SR-1), Courage, Dodge, Natural Born Warrior, Immunity (ARM), Tactical Awareness, Transmutation (Escape System), Cube 2.0.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 82 | 1.5 | AP HMG, E/M Carbine, Heavy Pistol, AP+DA CCW |
| 2 | 80 | 1 | AP Thunderbolt (+2B), E/M Carbine, Heavy Pistol, AP+DA CCW |
| 3 | 82 | 0 | AP HMG, E/M Carbine, Heavy Pistol, AP+DA CCW; Lieutenant |

Only one Maximus may be selected across IDs 1720 and 1862.

### Croc Men

**ID 13 · AVA 2 · SK** — `MOV 10-10 | CC 14 | BS 12 | PH 12 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. X Visor, Camouflage, Hidden Deployment, Infiltration, Mimetism (-6), Surprise Attack (-3), Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 2 | 25 | 0 | Boarding Shotgun, Shock Mine, D-Charges, Silenced Pistol, CCW |
| 3 | 29 | 1.5 | MULTI Sniper Rifle, Shock Mine, Silenced Pistol, CCW |
| 4 | 33 | 0.5 | Combi Rifle, D-Charges, Shock Mine, Silenced Pistol, CCW; Hacking Device |
| 5 | 26 | 0.5 | Boarding Shotgun, D-Charges, Shock Mine, Silenced Pistol, CCW; Minelayer |
| 6 | 30 | 0 | Combi Rifle, Flash Pulse, D-Charges, Shock Mine, Silenced Pistol, CCW; Deployable Repeater, Forward Observer |

### Squalos Mk-II

**ID 1651 · AVA 2 · TAG** — `MOV 15-10 | CC 18 | BS 15 | PH 15 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`. ECM: Guided (-6), BS Attack (SR-1), Courage, Combat Instinct, Remote Presence, Tactical Awareness, enhanced Dodge/GizmoKit.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 55 | 1 | MULTI Marksman Rifle, MULTI Pistol (+1B), CCW; Crabbot |
| 2 | 62 | 1.5 | HMG, Grenade Launcher, MULTI Pistol (+1B), CCW; Crabbot |
| 3 | 66 | 1.5 | MULTI HMG, MULTI Pistol (+1B), CCW; NCO; Crabbot |

### Fugazi Dronbot

**ID 19 · AVA 2 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Remote Presence, Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout |
|---:|---:|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) |

### Fennec Fusiliers

**ID 1803 · AVA 5 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 2`. Terrain (Desert).

| Opt | Pts | SWC | Loadout / role |
|---:|---:|---:|---|
| 1 | 10 | 0 | Combi Rifle, Pistol, CCW |
| 2 | 18 | 1 | HMG, Pistol, CCW |
| 3 | 15 | 1.5 | Missile Launcher, Pistol, CCW |
| 4 | 12 | 0 | SMG, Light Rocket Launcher, Pistol, CCW |
| 5 | 14 | 0 | Thunderbolt (+1B), Shock Mine, Pistol, CCW; Triangulated Fire, Minelayer |
| 6 | 12 | 0 | Combi Rifle, Pistol, CCW; Commlink (+1), Specialist Operative |
| 7 | 16 | 0.5 | SMG, E/Mitter, Pistol, CCW; Hacking Device, FastPanda |
| 9 | 13 | 0 | Combi Rifle, Flash Pulse, Disco Baller, Pistol, CCW; Forward Observer, Sensor |
| 10 | 12 | 0 | Combi Rifle, Pistol, CCW; MediKit, Paramedic |
| 11 | 10 | 0 | Combi Rifle, Pistol, CCW; Lieutenant |

**Source note:** revision `7.26246.158` does **not** list Decoy on the Fennec Lieutenant.

### BCA Magistrates

**ID 1804 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Biometric Visor, Counterintelligence, FT Master (Jackals), Immunity (Shock), Specialist Operative.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 17 | 0 | Combi Rifle, Nanopulser, Heavy Pistol, Stun Pistol (+1B), CCW |
| 2 | 21 | 0 | MULTI Marksman Rifle, Nanopulser, Heavy Pistol, Stun Pistol (+1B), CCW |
| 3 | 21 | 0 | Option 1; Chain of Command |
| 4 | 25 | 0 | Option 2; Chain of Command |
| 5 | 19 | 0 | Option 1; Lieutenant, Strategos L1 |
| 6 | 23 | 0 | Option 2; Lieutenant, Strategos L1 |

### Mulebots

**ID 38 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 4`. Baggage, Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 8 | 0 | Deactivator, Repeater, PARA CCW (-3) |
| 2 | 14 | 0.5 | EVO Hacking Device, PARA CCW (-3) |
| 3 | 17 | 0 | Combi Rifle, Repeater, PARA CCW (-3); Total Reaction |

### Blade-Ops

**ID 1751 · AVA 2 · LI** — `MOV 10-10 | CC 16 | BS 13 | PH 10 | WIP 12 | ARM 2 | BTS 3 | W 1 | S 2`. BS Attack (SR-1), Immunity (Shock), Mimetism (-3), Stealth, Terrain (Total), Tactical Awareness.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 20 | 0 | **BLADE FTO**; Boarding Shotgun, D-Charges, Silenced Pistol, CCW |
| 2 | 23 | 0 | **BLADE FTO**; AP SMG, D-Charges, Silenced Pistol, CCW; Engineer, GizmoKit |
| 3 | 30 | 0 | AP SMG, E/Mitter, D-Charges, Silenced Pistol, CCW; Engineer, Forward Deployment (+20), Decoy (2) |
| 4 | 30 | 0 | AP SMG, E/Mitter, D-Charges, Silenced Pistol, CCW; Engineer, Parachutist, Decoy (2) |

### Aquila Guard

**ID 8 · AVA 1 · HI** — `MOV 15-5 | CC 15 | BS 15 | PH 14 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 2`. MSV3, ECM: Hacker (-3), Deactivator, Courage, enhanced Jump.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 3 | 52 | 1.5 | HMG, MULTI Pistol, Shock CCW |
| 5 | 49 | 0 | **AQUILA FTO**; MULTI Marksman Rifle, Disco Baller, MULTI Pistol, Shock CCW; Specialist Operative |
| 7 | 49 | 0 | **AQUILA FTO Lieutenant**; same as 5 |
| 8 | 52 | +1 | **AQUILA FTO Lieutenant**; same as 5; Strategos L1 |

### Drummers Mobile Support Section

**ID 1806 · AVA 2 · LI** — `MOV 10-10 | CC 14 | BS 13 | PH 10 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`. 360º Visor. Each option includes its listed Drumbot Peripheral package.

| Opt | Pts | SWC | Controller / Peripheral package |
|---:|---:|---:|---|
| 1 | 40 | 1 | Marksman Rifle, Pistol, CCW + Drumbot-1 (MULTI HMG) |
| 2 | 42 | 1.5 | Marksman Rifle, Pistol, CCW + Drumbot-2 (HRMC) |
| 3 | 40 | 1 | Marksman Rifle, Pistol, CCW + Drumbot-3 (Feuerbach, Neurocinetics) |
| 4 | 42 | 1 | Marksman Rifle, Pistol, CCW; Forward Deployment (+10) + Drumbot-4 (Mk12, Heavy Rocket Launcher) |
| 5 | 21 | 0 | Marksman Rifle, Flash Pulse, Pistol, CCW; Forward Observer + Drumbot-5 |
| 6 | 28 | 1.5 | MULTI Sniper Rifle, Flash Pulse, Pistol, CCW; BS Attack (-3), Forward Observer + Drumbot-5 |
| 7 | 47 | 1 | Marksman Rifle, Flash Pulse, Pistol, CCW; Forward Observer + Drumbot-1 + Drumbot-5 |
| 8 | 47 | 1 | Marksman Rifle, Flash Pulse, Pistol, CCW; Forward Observer + Drumbot-3 + Drumbot-5 |

Drumbots are REM Peripherals with 360º Visor, Mimetism (-3), Courage and Peripheral (Synchronized); use the pinned source for exact disabled Peripheral sub-option payloads if a rules interaction depends on them.

### Fusiliers

**ID 1 · AVA Total · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 10 | 0 | Combi Rifle, Pistol, CCW |
| 2 | 18 | 1 | HMG, Pistol, CCW |
| 4 | 15 | 1.5 | Missile Launcher, Pistol, CCW |
| 5 | 16 | 1 | MULTI Sniper Rifle, Pistol, CCW |
| 6 | 15 | 0.5 | Combi Rifle; Hacking Device |
| 8 | 12 | 0 | Combi Rifle, Flash Pulse; Deployable Repeater, Forward Observer |
| 9 | 12 | 0 | Combi Rifle; MediKit, Paramedic |
| 10 | 10 | 0 | Lieutenant; Combi Rifle |
| 12 | 12 | 0 | Combi Rifle; Commlink (+1), Specialist Operative |

### Redeye Close Air Support Squad

**ID 1816 · AVA 1 · VH** — `MOV 20-5 | CC — | BS 14 | PH 13 | WIP 13 | ARM 6 | BTS 6 | STR 2 | S 7`. Aerial, Courage, Dodge (-3), GizmoKit (PH=14), Mimetism (-6), Remote Presence, Super-Jump (Jet Propulsion), Terrain (Total), No Cover, Tech-Recovery, Sensor.

| Opt | Pts | SWC | Loadout |
|---:|---:|---|
| 1 | 37 | 1.5 | Spitfire, Chain Rifle, Blitzen |
| 2 | 38 | 1.5 | Spitfire, Chain Rifle, Grenade Launcher (Continuous Damage) |

### Hetkari Shooters

**ID 1811 · AVA 1 · HI** — `MOV 15-5 | CC 17 | BS 14 | PH 14 | WIP 12 | ARM 5 | BTS 6 | W 2 | S 2`. Marksmanship, Combat Instinct.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 47 | 1.5 | Missile Launcher, Breaker Pistol, AP SMG, CCW |
| 2 | 48 | 1.5 | MULTI Red Fury, Breaker Pistol, CCW, E/Marat |
| 3 | 47 | 1.5 | Option 1; Lieutenant |
| 4 | 48 | 1.5 | Option 2; Lieutenant |

### ORC Troops

**ID 5 · AVA 2 · HI** — `MOV 15-5 | CC 15 | BS 14 | PH 14 | WIP 12 | ARM 4 | BTS 3 | W 2 | S 2`.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 28 | 0 | MULTI Rifle, Pistol, CCW |
| 2 | 29 | 0 | MULTI Rifle; TinBot: Firewall (-3) |
| 3 | 34 | 1.5 | HMG |
| 4 | 26 | 0 | Boarding Shotgun (+1B) |
| 6 | 33 | 0.5 | MULTI Rifle; Hacking Device |
| 7 | 28 | 0 | Lieutenant; MULTI Rifle |
| 8 | 34 | 1 | Lieutenant; HMG |
| 10 | 35 | 1.5 | Feuerbach |
| 11 | 27 | 0 | Boarding Shotgun (+1B); TinBot: Firewall (-3) |

### Optimate Agent Maximus

**ID 1862 · AVA 1 · MI** — `MOV 15-5 | CC 22 | BS 13 | PH 13 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Albedo (-6), CC Attack (-6), Courage, Dodge (+2.5), Natural Born Warrior, Immunity (ARM), Number 2, Specialist Operative, Tactical Awareness, NWI, Cube 2.0.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 48 | 1 | MAXIMUS AGENT; AP Thunderbolt (+2B), E/M Carbine, Heavy Pistol, AP+DA CCW; Minimus Peripheral |
| 2 | 45 | 1 | **MAXIMUS AGENT FTO**; same core weapons; TinBot (Repeater), no Minimus |
| 3 | 48 | +1 | MAXIMUS AGENT; option 1 + Lieutenant; Minimus Peripheral |
| 4 | 45 | +1 | **MAXIMUS AGENT FTO**; option 2 + Lieutenant; no Minimus |

Only one Maximus may be selected across IDs 1862 and 1720.

### Clipper Dronbot

**ID 18 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CCW (-3); BS Attack (Guided) |
| 5 | 19 | 1.5 | **CLIPPER DRONBOT FTO**; Missile Launcher (+1B), PARA CCW (-3) |

### Blink Team

**ID 1805 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 13 | PH 10 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`. Surprise Attack (-3), Camouflage, Hidden Deployment, Mimetism (-6), Stealth.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 28 | 0 | Shock Marksman Rifle, Shock Mine, Assault Pistol, CCW |
| 2 | 32 | 1.5 | MULTI Sniper Rifle, Assault Pistol, CCW |
| 3 | 28 | 1.5 | Heavy Rocket Launcher, WildParrot, Assault Pistol, CCW; X Visor |

### Peacemaker Armbots

**ID 36 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Repeater, Remote Presence, Courage, Forward Deployment (+20), Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 23 | 0 | Heavy Shotgun, Pulzar, PARA CCW (-3); AUXBOT_3 |
| 3 | 24 | 0.5 | Heavy Shotgun, Pulzar, PARA CCW (-3); AUXBOT_3B with Minelayer |
| 4 | 23 | 0 | Boarding Shotgun, Pulzar, PARA CCW (-3); BS Attack (+1B); no Auxbot |
| 5 | 27 | 0 | Boarding Shotgun, Pulzar, PARA CCW (-3); BS Attack (+1B); AUXBOT_3 |

### Black A.I.R.

**ID 1808 · AVA 1 · MI** — `MOV 10-10 | CC 17 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. MSV2, Mimetism (-3), Combat Instinct, Number 2, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 26 | 0.5 | **BLACK A.I.R. FTO**; SMG, Nanopulser, D-Charges, Pistol, CCW; Hacking Device |
| 2 | 29 | 0.5 | **BLACK A.I.R. FTO**; K1 Marksman Rifle, Nanopulser, Flash Pulse, Pistol, CCW; Forward Observer |
| 3 | 33 | 1.5 | **BLACK A.I.R. FTO**; MULTI Sniper Rifle, Nanopulser, Pistol, CCW; Neurocinetics |
| 4 | 31 | 0 | SMG, Flash Pulse (+1B), D-Charges, Pistol, CCW; Killer Hacking Device; Parachutist (DZ) |

### Joan of Arc

**ID 20 · AVA 1 · HI** — `MOV 10-10 | CC 23 | BS 15 | PH 15 | WIP 15 | ARM 5 | BTS 6 | W 2 | S 2`. Martial Arts L3, Inspiring Leadership, Frenzy, Stealth, NWI, Religious Troop, Tactical Awareness, Number 2, BS Attack (SR-1), X Visor.

All profiles: MULTI Rifle, Pulzar (+1B), Pistol, EXP CCW.

| Opt | Pts | SWC | Differences |
|---:|---:|---:|---|
| 1 | 47 | 0 | Chain of Command; Non-Specialist |
| 2 | 53 | 0 | Chain of Command; Non-Specialist; Strategic Deployment |
| 3 | 47 | +1 | Lieutenant |
| 4 | 51 | +1 | Lieutenant (+1 Command Token) |
| 5 | 53 | +1 | Lieutenant; Strategic Deployment |

Only one Joan of Arc may be selected across IDs 20 and 42.

### Patsy Garnett

**ID 1225 · AVA 1 · HI** — `MOV 15-5 | CC 19 | BS 14 | PH 14 | WIP 13 | ARM 4 | BTS 3 | W 2 | S 2`. Warhorse, Forward Observer, Stealth, NCO, Terrain (Total), FT Master (Helots).

| Opt | Pts | SWC | Loadout |
|---:|---:|---|
| 1 | 34 | 0 | AP SMG, E/Mitter, Grenades, D-Charges, Flash Pulse, Pistol, Shock CCW (PS=6) |

### Griffin Troops

**ID 1810 · AVA 2 · HI** — `MOV 15-5 | CC 16 | BS 14 | PH 12 | WIP 12 | ARM 4 | BTS 6 | W 2 | S 2`. MSV1, Courage, Terrain (Desert), Jump.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 31 | 0 | MULTI Rifle, Pulzar, Pistol, CCW |
| 2 | 37 | 1.5 | HMG, Pulzar, Pistol, CCW |
| 3 | 38 | 1.5 | Feuerbach, Pulzar, Pistol, CCW |
| 4 | 37 | 1 | HMG, Pulzar, Pistol, CCW; Lieutenant |

### Warcors

**ID 50 · AVA 1 · LI · Irregular** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Journalist.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor |
| 2 | 3 | 0 | Same; Sixth Sense |

### Machinists

**ID 15 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`. Engineer, Deactivator, GizmoKit.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 15 | 0 | Combi Rifle, D-Charges, Pistol, CCW |
| 8 | 16 | 0 | Same + Deployable Cover |
| 9 | 18 | 0 | Combi Rifle, D-Charges, Armed Turret (Combi Rifle), Pistol, CCW |

### Fireflies Clandestine Demo Squad

**ID 1809 · AVA 2 · MI** — `MOV 10-10 | CC 17 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 6 | W 1 | S 2`. Albedo, BS Attack (SR-1), Immunity (Shock), Stealth, NCO, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 24 | 1.5 | Heavy Rocket Launcher, D-Charges, AP Mine, Assault Pistol, CCW |
| 2 | 19 | 0 | SMG, Panzerfaust, D-Charges, Pistol, CCW; Deployable Repeater |
| 3 | 23 | 0 | SMG, Panzerfaust, D-Charges, AP Mine, Pistol, CCW; Chain of Command |
| 4 | 23 | 0 | SMG, Panzerfaust, D-Charges, AP Mine, Pistol, CCW; Deactivator, GizmoKit, Engineer |
| 5 | 24 | 0 | SMG, Panzerfaust, D-Charges, AP Mine, Armed Turret (Marksman Rifle), Pistol, CCW; Minelayer |
| 6 | 25 | 0 | Combi Rifle, Panzerfaust, D-Charges, AP Mine, Pistol, CCW; MediKit, Paramedic |
| 7 | 24 | 0.5 | SMG, Panzerfaust, D-Charges, AP Mine, Pistol, CCW; Hacking Device |

### Scarecrows Active Recon Group

**ID 1812 · AVA 2 · SK** — `MOV 10-10 | CC 15 | BS 13 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Surprise Attack (-3), Camouflage, Hidden Deployment, Infiltration, Mimetism (-6), Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 26 | 0 | Boarding Shotgun, Nanopulser, D-Charges, Silenced Pistol, CCW; Deployable Repeater |
| 2 | 29 | 0.5 | SMG, Nanopulser, D-Charges, Silenced Pistol, CCW; Hacking Device |
| 3 | 27 | 0 | SMG, Nanopulser, D-Charges, Silenced Pistol, CCW; Killer Hacking Device |
| 4 | 27 | 0.5 | Boarding Shotgun, Nanopulser, D-Charges, AP Mine, Silenced Pistol, CCW; Minelayer |
| 5 | 25 | 0 | SMG, Nanopulser, D-Charges, Flash Pulse, Silenced Pistol, CCW; Forward Observer |

### Blockers, Attached Agents of the CDCI

**ID 1750 · AVA 1 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Biometric Visor, X Visor, BS Attack (+1B), Sensor, Discover (ReRoll).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 15 | 0 | Adhesive Launcher Rifle, Pitcher, Pulzar, Flash Pulse, MULTI Pistol, PARA CCW (-6); Specialist Operative |
| 2 | 19 | 0.5 | Adhesive Launcher Rifle, Pulzar, Flash Pulse, MULTI Pistol, PARA CCW (-6); Hacking Device (Firewall -3) |

### Trauma-Docs

**ID 14 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. Doctor, MediKit.

| Opt | Pts | SWC | Loadout |
|---:|---:|---|
| 1 | 14 | 0 | Combi Rifle, Pistol, CCW |

## Fireteams

Generic / vanilla PanOceania has **no standard Fireteam chart** in the pinned Army source. Any `FTO` text above is part of a profile/loadout name only and does not grant Fireteam access in generic PanOceania.
## Transcript-backed competitive tactics (research: 2026-10-19)

**Authority / important correction.** The roster and costs above are the **September 2026 N5.3 Army snapshot**, not the 2025 opinions below. This generic faction's pinned Army data has **no standard Fireteam chart**. Consequently the much-discussed **Joan + Blade Haris, Tikbalang + Karhu Duo, Bolt Haris, Patsy + Helot Haris, double Bulleteer Duo, and double Squalos Duo** in early N5 videos/podcasts are **historical suggestions, not validated current vanilla Fireteams**. Reuse the *roles and order-economy reasoning*, not those formations or their claimed special dice. Never infer links from FTO-labelled profiles.

### Fast list-building read

1. **Select two ways to win a shooting turn, not just the biggest gun.** The first attacker removes ARO pieces; the second attacks from a different range/angle or scores when the first fails. Cutter can endure repeated fights; Drummer HRMC needs redundancy because its controller/Peripheral is fragile. (KingButt, Dante, Swiss Miss.)
2. **Buy orders and denial before the third premium attacker.** Fugazi (7), Mulebot (8), Fennec/Fusilier utility, Helot ARO, Peacemaker midfield blocking, Firefly turret and Blink hidden threat all consume enemy Orders for disproportionately little investment. Preserve sufficient protected DZ space for S3/S4/S7 bases.
3. **Choose a command package deliberately.** Magistrate **19-point Strategos LT** is a safe, cheap command plan; **21-point CoC + Counterintelligence** is succession insurance for an exposed Joan v2, Tikbalang or Cutter LT. Alternatives include Firefly CoC and Bolt CoC. CoC is not a reason to expose the LT recklessly, and the Magistrate is AVA 1.
4. **Score through an independent specialist.** Pathfinder **17-point Tactical Awareness FO/Sensor/Repeater**, Zulu-Cobra camouflage specialists, Croc Man/Scarecrow hidden midfield, Banshee AD, Blade Engineer or Drummer FO are different delivery methods. At least one should still work if the primary gun is down or immobilized.
5. **Decide between hacking *support* and a genuine guided plan.** Cheap Fugazi/Peacemaker repeaters help defend TAGs; a Guided Clipper instead requires reliable Spotlight/Pitchers, EVO/order support and a plan against resets/Repeater loss. Do not automatically invest in both.
6. **After clearing lanes, rebuild your defensive puzzle.** Helot camouflage Neurocinetics, Firefly turret Minelayer, Peacemaker + Auxbot, a hidden Blink HRL and (optionally) an engineer-backed Sierra TR threaten different answers. They need not all be used in one list.

### Units and packages worth testing — *why*, not automatic picks

| Pick | Value proposition | Cost / alternative |
|---|---|---|
| **Magistrate Strategos LT / CoC** | Safe Counterintelligence + deployment/command edge **or** cheap insurance that liberates an aggressive LT. Multiple reviewers call it one of vanilla's largest N5 improvements. | One Magistrate only; an active LT also needs a meaningful plan to spend its LT Orders. |
| **Joan v2, 45–51 pts** | AP Spitfire, mobility, Tactical Awareness, CC threat and Inspiring Leadership make a standalone attack/command engine; converts useful Irregular Helot/Warcor/bounty-hunter Orders when LT. | Not a free **Haris** with Blade-Ops in the *current* reference; hackable and can over-concentrate roles. |
| **Helots, AVA 2** | Very cheap awkward AROs; one-use camouflage forces Discover/positioning before attackers can cleanly engage. Useful against early rushes. | Irregular absent Inspiring Leadership; camouflage versions cannot be evaluated as if they receive a vanilla Fireteam bonus. |
| **Firefly turret Minelayer, 24 pts** | Starts a layered defensive turret threat before the opponent's alpha and can add more to protect retreat/scoring lanes; NCO and other specialist options broaden use. | Static placements can be bypassed or sniped; don't over-invest Orders deploying turrets before needed attacks/objectives. |
| **Blink hidden HRL, 28 pts** | Mimetism (-6) / Hidden Deployment + X-Visor template/ WildParrot force the opponent to respect lanes that appear empty. | Surprise threat is finite; needs a useful angle, not just a hidden model for its own sake. |
| **Black A.I.R. Neurocinetics sniper / DZ Parachutist KHD** | First is an independent MSV2/MSR ARO problem; second attacks enemy DZ hackers and counter-camo defenders from an unexpected edge. | Sniper can be outshot by a superior long-range piece and buys little active-turn value; KHD needs a target/path. |
| **Zulu-Cobra / Scarecrow / Croc Man** | Camo specialists project objective pressure and deceptive attack lanes while protecting fragile orders; Zulu-Cobra KHD brings forward cyber threat. | Pay for the distinct mission/marker role, not redundant similar infiltrators. |
| **Karhu Feuerbach / Hetkari shooter** | Alternative high-quality guns so a fragile Drummer need not be the *only* ARO opener; Karhu MSV1 + Mimetism, Hetkari Marksmanship/Combat Instinct. | Compare points/range/cover, not old Fireteam burst claims. |
| **Fennec utility vs Fusilier** | FastPanda/Disco Baller/mine options can make an inexpensive order contributor actively useful; Fusilier remains a leaner cheap-order/LT choice. | Fennec's **sectorial** links cannot be imported into vanilla. |
| **Banshee / Blade Engineer** | AD/Parachutist attacks and classifieds from unexpected directions; Blade's Tactical Awareness/Engineer helps a dispersed TAG/REM force. | A projected Engineer is not guaranteed to reach or recover an overextended TAG. |

### TAG choices: the full attack-plan cost

| TAG | Why use it | When *not* to choose it |
|---|---|---|
| **Cutter 95–97 pts, AVA 1** | ARM 8, BS15, camouflage/Hidden Deployment, Mimetism(-6), MULTI HMG: apex long-range gun that can absorb failed exchanges and avoid direct targeting while concealed. KingButt uses it to clear AROs, then scores later. | ~one-third the list for **one model without Tactical Awareness**. Fewer points for alternate attackers, hackers, midfield and orders. **95-point option is LT**, 97-point is **NCO**; do not swap roles accidentally. |
| **Tikbalang 69 / 73 LT pts, AVA 1** | BS15 Mimetism(-3), Climbing Plus, Tactical Awareness and mobile HMG create high-efficiency angles while retaining TAG toughness. LT adds +1 LT Order. | Cannot use its former **Karhu Duo** in current vanilla. Against high ARM, no AP HMG; some reviewers prefer discounted Squalos or cheaper Hetkari for the required gunfight. |
| **Squalos Mk-II 55 / 62 / 66 pts, AVA 2** | Cheapest robust TAG engine: BS15 ARM6 W3, Tactical Awareness. **55** MULTI Marksman for cost; **62** HMG + Grenade Launcher for area/speculative option; **66** MULTI HMG **NCO** to use unused LT order(s). Two independent Squalos diversify threats. | No current vanilla Duo. Need support to avoid two isolated hackable centerpiece commitments; don't pay GL or NCO if list cannot exploit them. |
| **Maximus TAG** | Specialist heavyweight option with its own unique profile; reassess against the specific current loadout and mission. | Multiple early reviewers reject it as expensive compared to PanO's BS15 TAG efficiency; not a default centerpiece. |

**Recommended sequencing:** primary gun breaks visible AROs → eliminate key hackers/anti-TAG threats → an independent objective specialist advances → preserve a hidden/cheap second attacker and defence. KingButt's Cutter-first/Joan-later plan illustrates *sequencing*, but its period Joan–Blade Haris does **not** translate into a legal current vanilla formation.

### Vehicle: Redeye (the only standard VH in this roster)

**Current option comparison:** **37 points / 1.5 SWC** Spitfire + Chain Rifle + **Blitzen** versus **38 points / 1.5 SWC** Spitfire + Chain Rifle + **Continuous Damage Grenade Launcher**. Both: **BS14, ARM6, BTS6, STR2, Mimetism(-6), Aerial/Super-Jump, Sensor, No Cover**.

- **Pro-Redeye (Daboarder, WIP12 E180; Trent, E201):** extremely fast vertical approach reaches troops hidden behind the long-range ARO network where conventional PanO guns cannot shoot. A forward Redeye forces opponents to spend Orders addressing a DZ flanker; it can be an *order-taxing threat* even without killing its points. High ARM/BTS plus Mimetism reward careful angles, but **No Cover** and airborne hacking exposure still matter.
- **Blitzen camp (Daboarder):** E/M provides a reactive anti-TAG/HI/other-VH deterrent, including aerial duels; prefers this because speculative GL often never earns back the Orders spent firing.
- **Grenade-launcher camp (Trent; early KingButt *speculation*):** only +1 point supplies a different attack vector, bypasses difficult line of fire and threatens clustered enemies with Continuous Damage. Trent reports an actual difficult-TAG solution; KingButt explicitly **had not yet used Redeye** when proposing it.
- **Skeptical camp (Swiss Miss; Dante/Tristan):** ~37–38 points buys a short/mid-range Spitfire chassis that **cannot claim cover**, remains hackable, needs safe landing/flight geometry and competes with cheaper land-based shooters. It is not a universal inclusion.
- **Decision:** choose it for *angles and tempo* unavailable to ground attackers, not because its Spitfire outshoots a TAG on an open lane. **Blitzen** if enemy VH/HI/TAG deterrence is the missing role; **GL** if specific mission/terrain gives speculative or alternate-angle Continuous Damage value. Prefer an Engineer/hacking-counter plan if you expect it to survive multiple turns.

### REM decision guide (all current vanilla availability)

| REM | Use when | Skip / competing view |
|---|---|---|
| **Fugazi — 7 pts, AVA 2** | First-pass cheap Regular Orders, Flash Pulse/Mimetism(-3) ARO and repeaters anchoring hacker/anti-AD coverage. | Two S3 bases plus heavier REMs can crowd protected DZ and provide enemy attack pathways through their Repeaters. |
| **Mulebot — 8 Baggage / 14 EVO / 17 TR Combi, AVA 2** | 8pt order/reload platform; EVO if an eligible Bulleteer/Peacemaker/Drumbot, Combat Jump or other specific program makes it earn its 6pt/0.5 SWC premium. | Don't pay EVO merely by habit. Validate actual Supportware targets and activation timing, especially Drumbot Peripherals. |
| **Pathfinder — 14 / 17 TacAware, AVA 2** | Fast independent **FO+Sensor+Repeater**, WIP13; **17pt self-funded mission runner** and an answer to camo. KingButt compares its mission delivery favourably with lost Varuna Montesa. | Swiss Miss rates it poorly for duplicated Sensor; Dante/Tristan call it useful **but not automatic**. Pick it for repeated FO/scoring movement, not merely Sensor. |
| **Peacemaker — 23 / 24 Minelayer / 27 +1B Auxbot, AVA 2** | Forward-deployed Mimetism(-3) Repeater plus template-bearing Auxbot; **24pt Minelayer** for turn-zero denial and mine + flame fork (KingButt, Loss of Lieutenant); **27pt +1B** for aggressive boarding-shotgun exchanges (Trent). | One REM need not fill both defensive and attacking roles. Vulnerable to anti-REM hacking; S4 base/advance path matters. |
| **Sierra — 18 Thunderbolt(+1B) / 23 HMG, AVA 2** | Repairable **Total Reaction/360º** long-lane defence when you already have an Engineer and want an Order-producing ARO independent of Helots. Cheaper Thunderbolt saves SWC. | KingButt usually skips for Helots + Firefly turrets; Dante/Tristan like the repairable complement; Swiss Miss considers it a fine filler, not an apex gun. |
| **Bulleteer — 19 HS(+1B) / 22 Spitfire, AVA 2** | Budget MOV15-10 **Mimetism(-6)** Repeater gunfighter, especially Spitfire backed by EVO program and a different-range premium attacker. | A fragile independent REM, **not** a legal generic Duo; cannot substitute for an anti-armour long-range centerpiece. |
| **Clipper — 16 Guided ML / 19 FTO-labelled +1B ML, AVA 2** | **Guided** only with Spotlights, repeater reach, expendable Orders and risk management. Tactical Awareness demonstrates a double-Clipper + Fennec/Peacemaker spotting package as a deliberate build. | Dante dismisses Guided as forcing an inefficient engine in gun-first vanilla; Swiss Miss sees a viable conditional option. **FTO label gives no vanilla Fireteam.** |
| **Palbot — 3 pts peripheral** | Project one Engineer/Doctor's reach to multiple dispersed TAGs/REMs or specialists. | No independent Order; keep the controller safe and the service route plausible. |

**Difference of philosophy:** **gun-first (KingButt)** uses repeaters primarily as defence and generally does not pursue hacking/classifieds heavily. **hacking/guided package (Tactical Awareness)** deliberately buys Fennec FastPandas, Peacemakers, EVO and Clip­pers for Spotlight-to-missile pressure. Both are viable *concepts*, but the latter must demonstrate orders and delivery, not just available profiles. **No Fireteam is assumed for either.**

### Best transcript-verified viewing/listening — watch for the stated question

| Priority | Source and date | What the transcript establishes |
|---|---|---|
| 1 — primary faction | [WIP12 E177: Vanilla PanO with KingButt](https://open.spotify.com/episode/5YoQVh0YvxS2DCtIIGyskl) (2025-01-28) | Tournament-tested attack/score sequencing, Magistrate CoC, Cutter versus Drummer, Helot/Firefly defence, Peacemaker, Pathfinder, EVO; *some 2025 Fireteams invalid now*. |
| 2 — broad unit triage | [Swiss Miss Gaming: Infinity N5 Tier List — Panoceania](https://www.youtube.com/watch?v=EjN9xWKeBso) (2025-11-23) | Unit-by-unit why: great Blink/Black A.I.R./Magistrate/Peacemaker; skeptical Drummer/Pathfinder/Redeye; budget Bulleteer/Clipper. |
| 3 — opposing faction view | [Infinity the Dante with Tristan: Vanilla PanO Initial N5 Reaction](https://www.youtube.com/watch?v=qp458fqYq_s) (2025-02-25) | Two-gun redundancy, cheap LT+CoC, sceptical Black A.I.R. sniper/Guided, but pro-Fugazi/Bulleteer and repairable Sierra. |
| 4 — alternate archetypes | [Tactical Awareness S3E07: PanO Part 4 — Vanilla](https://www.youtube.com/watch?v=ZbwXcQ_IK5A) (2025-01-21) | Joan/irregular-orders concept, double-Squalos pressure, EVO/Peacemaker/Spotlight/**double Clipper** Guided engine. Examples are **historical**, not validated 2026 links. |
| 5 — VH deep dive | [WIP12 E180: Kestrel with Daboarder](https://open.spotify.com/episode/3JXkarf51Os0UUopYrM7IW) (2025-03-04; **Redeye ~33–41 min**, Peacemaker/Sierra later) | Strongest detailed case for Redeye *Blitzen* and mobility/order-tax, explicit acknowledgement of an opposing GL argument. Shared chassis; don't import Kestrel links. |
| 6 — VH and REM counterview | [WIP12 E201: Neoterran Capitaline Army with Trent](https://open.spotify.com/episode/3FT1No7zFHzpj7WC63hcCb) (2026-03-25; **Peacemaker ~57–59 min, Redeye ~83–87 min**) | Redeye *GL* alternate-angle case; **27pt +1B Peacemaker versus 24pt Minelayer** preference; NCA Fireteam privileges do not apply to generic PanO. |

**Evidence status:** All six sources above were examined via **YouTubeMCP or PodcastMCP transcript**, not merely searched by title. Their tactical claims are attributed interpretation, not updated Army data. A curated [Corvus Belli forum PanO N5 source index](https://forum.corvusbelli.com/threads/n5-recap-panoceanian-tacticas.43511/) supplies further viewing but is **not** a substitute for transcript review. For general REM support/placement reasoning, see [REMs](../../notes/list-building/rems.md).

## TAG tactical cross-reference (2026-10-23)

**Cutter** is the highest-ceiling concealed gun, but at 95–97 points without TacAware it needs a second independent scoring plan. **Tikbalang** buys Climbing Plus/Mimetism/mine and self-funded activations; **Squalos Mk-II** buys cheaper BS15 shooting and choice of AP-capable NCO MULTI HMG versus GL. **Maximus TAG** is a costly CC/anti-armor counter rather than the default value attacker. Do not import Jotum/Seraph/Uhlan access from other PanO sectorials.

Cross-faction **apex vs points-value** comparisons, matchup table, and direct MCP-reviewed podcast/video sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Current profile and Fireteam legality above remain authoritative.
