---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 404
sectorial_slug: ramah-taskforce
sectorial_name: Ramah Taskforce
parent_faction: Haqqislam
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "37-unit standard Ramah Taskforce roster with standard profiles/loadouts; complete main Fireteam chart and reverse index; optional Husam Spec-Ops and Haqqislam Team-Ops hooks; linked 13-unit Melek Reaction Group reinforcement roster and Fireteam chart."
---

# Ramah Taskforce

## Overview and provenance

Repository-native factual reference for **Ramah Taskforce (Army ID 404)** roster, profiles, points/SWC, AVA, Fireteam access, and linked Reinforcements.

Sources used:

- Army-derived Ramah Taskforce source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `d4329bb596ffea5d568eb2435f74366c305a7630`.
- Ramah source blob: `19015770025b60a73cda1e41b59766ea9a778afd`.
- Linked Melek Reaction Group reinforcement source revision `7.26246.158`, source blob `1c4c1854468cb733649b98ed12d41317afc6c551`.
- InfinityDB normalization/identity baseline: commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **37-unit standard Ramah roster** whose source faction list includes Army `404`.
- Generic Soldier-of-Fortune / mercenary-catalog records whose source `factions` list is empty are excluded.
- `Husam Spec-Ops` and `Haqqislam Team-Ops` are optional game-mode entries, not ordinary matched-play roster entries.
- Fireteam legality comes from the canonical chart below, not from an `FTO` label alone.
- `BEASTHUNTER FTO` means Beasthunter option 1 only; `Fiddler FTO` means Fiddler option 1 only; the Armored Assault `RAFIQ REMOTE` row is explicitly marked `FTO`, therefore only Rafiq option 3 is eligible there.
- Parenthetical Army-chart comments are preserved as Counts-as/equivalence labels.
- Rows marked `required: true` in a multi-unit source set are represented as a **required-choice set**: at least one qualifying member from that set is required; they are not interpreted as requiring every marked troop type simultaneously.
- Reinforcement Army `499`, **Melek Reaction Group**, is kept separate from the main Ramah roster and chart.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Ramah Taskforce |
| Parent faction | Haqqislam |
| Army ID | 404 |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 37 |
| Optional-mode units | Husam Spec-Ops; Haqqislam Team-Ops |
| Linked Reinforcement roster | Melek Reaction Group, Army ID 499 |
| Fireteam limits | Core 1; Haris 1; Duo unlimited (`256` source sentinel) |
| Main Fireteam rows | Ramah Taskforce; Mukhtar; Janissaries; Armored Assault; Wildcards |

## Fireteam chart limits and sectorial-level restrictions

| Constraint | Value / wording |
|---|---|
| Core | up to 1 |
| Haris | up to 1 |
| Duo | unlimited by sectorial chart (`256` source sentinel) |
| FT-01 required-choice | At least one of Ghulam, Naffatûn, Zhayedan, Khawarij, or Namurr |
| FT-04 required-choice | At least one of Fasid, Shakush, Maghariba, or Rafiq Remote FTO |
| Beasthunter restriction | `BEASTHUNTER FTO`, option 1 only |
| Fiddler restriction | `Fiddler FTO`, option 1 only; Jackbot-bearing options 2–3 do not use this slot |
| Rafiq restriction | Armored Assault slot is marked `FTO`; option 3 only |
| Spec-Ops | Husam may use FT-01 only when the Spec-Ops mode is in use |
| Main/Reinforcement mixing | No source-defined mixing exception; keep charts separate |

## Unit roster index

`Total` represents source AVA `255`.

| Unit ID | Unit | AVA | Type | Classification | Order | Fireteam access |
|---:|---|---:|---|---|---|---|
| 309 | Maghariba Guard | 2 | TAG | Mechanized | Regular + Tactical | Armored Assault |
| 311 | Murabids Tuareg | 3 | SK | Elite | Regular | — |
| 1849 | Sayiq, Sword of Allah TAG Support Pilots | 1 | LI | Support | Regular | Ramah; pilot support |
| 1333 | Monstruckers | 2 | LI | Mercenary | Irregular | — |
| 303 | Khawarijs | 5 | MI | Elite | Regular | Ramah required-choice |
| 50 | Warcors | 1 | LI | Mercenary | Irregular | — |
| 1313 | Mukhtar Active Response Unit | 4 | MI | Veteran | Regular | Mukhtar |
| 317 | Shaytaniyah Remotes | 1 | REM | Support | Regular | — |
| 1482 | Wild Bill | 1 | LI | Character | Regular | Janissaries |
| 315 | Rafiq Remotes | 2 | REM | Support | Regular | Armored Assault, FTO option only |
| 1546 | Shakush Light Armored Unit | 2 | TAG | Mechanized | Regular + Tactical | Armored Assault |
| 464 | Valerya Gromoz | 1 | LI | Character | Regular | Wildcard |
| 305 | Zhayedan Intervention Troops | 5 | MI | Veteran | Regular | Ramah; counts as Ghulam |
| 314 | Najjarun Engineer | 1 | LI | Support | Regular | — |
| 1549 | Medical Specialist Rahman Rouhani | 1 | LI | Character | Regular | Wildcard |
| 1125 | Hakims | 2 | MI | Specialist Trained | Regular | — |
| 333 | Nasmat Remotes | 4 | REM | Support | no Order | Peripheral (Servant) |
| 334 | Kameel Remotes | 2 | REM | Support | Regular | — |
| 319 | Tarik Mansuri | 1 | MI | Character | Regular | Wildcard; counts as Khawarij |
| 1153 | Carmen Johns & Bâtard | 1 team | WB | Character | Irregular + Impetuous | — |
| 1570 | Beasthunters Free Guild | 1 | SK | Mercenary | Irregular | Ramah, FTO option only |
| 1851 | Haytham Aero-unit | 1 | VH | Elite | Regular | — |
| 301 | Ghulam Infantry | Total | LI | Line | Regular | Ramah required-choice |
| 1894 | Dr. Claire Lazhari | 1 | LI | Character | Regular | Wildcard |
| 1548 | Yara Haddad | 1 | MI | Character | Regular | Wildcard |
| 310 | Hunzakuts | 1 | SK | Specialist Trained | Irregular | — |
| 1314 | Nahab Aeromobile Team | 3 | LI | Veteran | Regular | — |
| 343 | Al Fasid Regiment | 3 | HI | Veteran | Regular | Janissaries; Armored Assault required-choice |
| 302 | Naffatûn | 5 | LI | Line | Regular | Ramah; counts as Ghulam |
| 316 | Shihab Remotes | 2 | REM | Support | Regular | — |
| 318 | Fanous Remotes | 3 | REM | Support | Regular | — |
| 1759 | Burkut, Aerospace Engineering Regiment | 2 | HI | Veteran | Regular | Wildcard; counts as Janissary |
| 849 | Husam Operative Leila Sharif | 1 | LI | Character | Regular | Wildcard; counts as Ghulam |
| 1316 | Hortlak Janissaries | 2 | HI | Veteran | Regular | Janissaries; counts as Janissary |
| 308 | Janissaries | 5 | HI | Veteran | Regular | Janissaries |
| 1315 | Namurr Experimental Operative Group | 2 | MI | Elite | Regular | Ramah required-choice; Wildcard |
| 1564 | Fiddler | 1 | LI | Character | Regular | Ramah, FTO option only |

### Optional-mode units

| Unit ID | Unit | Mode | Fireteam relevance |
|---:|---|---|---|
| 1916 | Husam Spec-Ops | Spec-Ops | Ramah FT-01, max 1, when Spec-Ops mode is active |
| 1930 | Haqqislam Team-Ops | Team-Ops | No ordinary Ramah Fireteam row |

## Unit details

### Maghariba Guard

**ID 309 · AVA 2 · TAG** — `MOV 15-10 | CC 16 | BS 14 | PH 17 | WIP 14 | ARM 8 | BTS 6 | STR 3 | S 8`  
**Common:** Baggage, ECM: Guided (-6), ECM: Hacker (-3), 360º Visor, BS Attack (SR-1), Tactical Awareness, Religious Troop, Terrain (Desert), Dodge (PH=10), GizmoKit (PH=11). Includes one Jandab Ancillary Remote.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 72 | 1.5 | MULTI HMG, E/M Carbine (+2B), AP Heavy Pistol, CCW (PS=4) | Armored Assault |
| 2 | 71 | 1.5 | MULTI HMG, Heavy Rocket Launcher, Grenade Launcher, Heavy Pistol (+1B), CCW (PS=4) | Armored Assault |
| 3 | 71 | 1.5 | MULTI HMG, Heavy Flamethrower (+1B), Mine Dispenser (Shock), AP Heavy Pistol, CCW (PS=4) | Armored Assault |

**Jandab:** `MOV 15-10 | PH 10 | WIP 12 | ARM 0 | BTS 0 | STR 1 | S 1`; Courage, Mimetism (-3), Specialist Operative, Peripheral (Ancillary), Terrain (Desert).

### Murabids Tuareg

**ID 311 · AVA 3 · SK** — `MOV 10-10 | CC 14 | BS 11 | PH 12 | WIP 15 | ARM 1 | BTS 0 | W 1 | S 2`  
**Common:** Camouflage, Hidden Deployment, Infiltration, Mimetism (-6), Surprise Attack (-3), Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 2 | 26 | 0 | Boarding Shotgun, Shock Mine, Pistol, CCW |
| 3 | 27 | 0.5 | Sniper Rifle, Shock Mine, Pistol, CCW |
| 4 | 33 | 0.5 | Rifle, Light Shotgun, D-Charges, Shock Mine, Pistol, CCW; Hacking Device (Firewall -3), Hacker |
| 5 | 28 | 0 | SMG, D-Charges, Shock Mine, Pistol, CCW; Killer Hacking Device (Firewall -3), Hacker |
| 6 | 32 | 0 | Rifle, Light Shotgun, Shock Mine, Pistol, CCW; MediKit; Doctor (2W) |
| 7 | 29 | 0.5 | Rifle, Light Shotgun, Viral Mine, Pistol, CCW; Minelayer |

### Sayiq, Sword of Allah TAG Support Pilots

**ID 1849 · AVA 1 · LI** — `MOV 10-10 | CC 16 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`  
**Common:** Courage, Specialist Operative, Terrain (Desert), Religious Troop, TAGCom; Dodge (PH+3), GizmoKit (PH+1).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 9 | 0 | **SHAKUSH PILOT**; SMG, D-Charges, Pistol, CCW; GizmoKit | Ramah max 1 |
| 2 | 10 | 0 | **MAGHARIBA PILOT**; Light Shotgun, Pistol, CCW; GizmoKit, MediKit, Paramedic | Ramah max 1 |

### Monstruckers

**ID 1333 · AVA 2 · LI** — `MOV 10-10 | CC 16 | BS 11 | PH 12 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`  
**Common:** Irregular, Engineer, Climbing Plus, Deactivator, GizmoKit.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 15 | 0 | Boarding Shotgun, Adhesive Launcher Rifle, E/M Grenades, Pistol, CCW |
| 2 | 12 | 0 | SMG, Chain Rifle, Drop Bears, Pistol, CCW |
| 3 | 15 | 0 | SMG, Chain Rifle, Drop Bears, Armed Turret (AP Rifle), Pistol, CCW |
| 4 | 16 | 0 | Rifle, Light Shotgun, Akrylat-Kanone, D-Charges, Pistol, CCW; 360º Visor |

### Khawarijs

**ID 303 · AVA 5 · MI** — `MOV 15-5 | CC 23 | BS 13 | PH 13 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`  
**Common:** CC Attack (-6), Dodge (+2.5), Natural Born Warrior, Religious Troop, BS Attack (SR-1), Immunity (ARM), Combat Instinct, Terrain (Desert), Super-Jump (7.5).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 3 | 29 | 1 | Heavy Rocket Launcher, Light Shotgun, Pistol, Viral CCW (PS=6) | Ramah |
| 4 | 35 | 1.5 | AP Spitfire, Pulzar (+1B), Pistol, Viral CCW (PS=6) | Ramah |
| 5 | 33 | 0 | Rifle, Light Shotgun, Pulzar (+1B), Disco Baller, Pistol, Viral CCW (PS=6); Chain of Command | Ramah |
| 6 | 30 | 0 | Boarding Shotgun, Pulzar (+1B), Pistol, Viral CCW (PS=6); MediKit, Doctor (+3) | Ramah |
| 9 | 38 | 0 | Mk12, Pulzar (+1B), Pistol, Viral CCW (PS=6); MSV2, NCO | Ramah |

### Warcors

**ID 50 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`; Journalist, Irregular.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); Sixth Sense |

### Mukhtar Active Response Unit

**ID 1313 · AVA 4 · MI** — `MOV 15-5 | CC 16 | BS 13 | PH 11 | WIP 14 | ARM 2 | BTS 6 | W 1 | S 2`  
**Common:** Courage, Forward Deployment (+10), Immunity (Shock), Mimetism (-3), No Wound Incapacitation.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 25 | 0 | Viral Rifle, Nanopulser (+1B), Pistol, CCW | Mukhtar |
| 2 | 26 | 0 | Boarding Shotgun, Nanopulser (+1B), Pistol, CCW; MediKit, Doctor (+3) | Mukhtar |
| 3 | 25 | 0 | Rifle, Light Shotgun, Flash Pulse, D-Charges, Pistol, CCW; Forward Observer | Mukhtar |
| 4 | 29 | 0.5 | Rifle, Light Shotgun, D-Charges, Pistol, CCW; Hacking Device, Hacker | Mukhtar |
| 5 | 34 | 1 | Red Fury, Nanopulser (+1B), Pistol, CCW; MSV2 | Mukhtar |

### Shaytaniyah Remotes

**ID 317 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`; Courage, Remote Presence.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 16 | 1.5 | Missile Launcher (Guided), PARA CCW (-3) |
| 3 | 19 | 1.5 | Missile Launcher (+1B), PARA CCW (-3) |

### Wild Bill

**ID 1482 · AVA 1 · LI** — `MOV 15-5 | CC 15 | BS 13 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`  
**Common:** BS Attack (SR-1), Courage, Dodge (+3), Marksmanship, No Wound Incapacitation.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 22 | 0 | Contender, MULTI Pistol (+1B), CCW | Janissaries max 1 |
| 2 | 24 | 0 | Rifle, MULTI Pistol (+1B), CCW; BS Attack (Shock) | Janissaries max 1 |

### Rafiq Remotes

**ID 315 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`  
**Common:** Deactivator, Repeater, Courage, Forward Observer, Remote Presence, Sensor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 13 | 0 | Rifle, Light Shotgun, Flash Pulse, PARA CCW (-3); Triangulated Fire | — |
| 3 | 19 | 0.5 | **RAFIQ REMOTE FTO**; Red Fury, Flash Pulse, PARA CCW (-3) | Armored Assault only |

### Shakush Light Armored Unit

**ID 1546 · AVA 2 · TAG** — `MOV 15-5 | CC 17 | BS 14 | PH 14 | WIP 14 | ARM 6 | BTS 6 | STR 3 | S 6`  
**Common:** BS Attack (SR-1), Courage, Dodge (PH=11), Tactical Awareness, GizmoKit (PH=11). Includes one Jandab Ancillary Remote.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 58 | 1.5 | HMG (Continuous Damage), Heavy Flamethrower, AP CCW (PS=6) | Armored Assault |
| 2 | 56 | 1.5 | AP Spitfire, Heavy Flamethrower, AP CCW (PS=6) | Armored Assault |

### Valerya Gromoz

**ID 464 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0.5 | Combi Rifle, Zapper, Pitcher, Pistol, CCW; Hacking Device with Total Control (+1B), Hacker | Wildcard |

### Zhayedan Intervention Troops

**ID 305 · AVA 5 · MI** — `MOV 10-10 | CC 16 | BS 12 | PH 11 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`  
**Common:** BS Attack (Shock), Warhorse, Combat Instinct, Marksmanship, Regeneration (PH=12).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 22 | 0 | Breaker Rifle, Light Shotgun, Pistol, CCW | Ramah; counts as Ghulam |
| 2 | 31 | 1.5 | HMG, Pistol, CCW | same |
| 3 | 27 | 0.5 | AP Sniper Rifle, Pistol, CCW | same |
| 4 | 26 | 1.5 | Missile Launcher, Pistol, CCW | same |
| 5 | 27 | 0 | Boarding Shotgun, Pistol, CCW; MediKit, Doctor (+3) | same |
| 6 | 22 | 0 | Breaker Rifle, Light Shotgun, Pistol, CCW; Lieutenant | same |
| 7 | 31 | 1.5 | HMG, Pistol, CCW; Lieutenant | same |

### Najjarun Engineer

**ID 314 · AVA 1 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`; Courage, Engineer, Deactivator, GizmoKit.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 15 | 0 | Rifle, Light Shotgun, D-Charges, Pistol, CCW |
| 2 | 16 | 0 | As option 1; Deployable Cover |
| 3 | 17 | 0 | As option 1; Armed Turret (Rifle) |

### Medical Specialist Rahman Rouhani

**ID 1549 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 11 | PH 11 | WIP 15 | ARM 1 | BTS 6 | W 1 | S 2`; Courage, Doctor (+3), No Wound Incapacitation, MediKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | SMG, Flash Pulse, Pistol, CCW | Wildcard |

### Hakims, Special Medical Assistance Team

**ID 1125 · AVA 2 · MI** — `MOV 10-10 | CC 14 | BS 12 | PH 11 | WIP 15 | ARM 2 | BTS 3 | W 1 | S 2`  
**Common:** Doctor (+3), Parachutist, Regeneration, Terrain (Total), Immunity (Shock), MediKit (+1B).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 25 | 0 | Boarding Shotgun (+1B), Boarding Pistol, CCW |
| 2 | 24 | 0 | SMG, E/Mitter, Boarding Pistol, CCW |
| 3 | 29 | 0 | Boarding Shotgun (+1B), Boarding Pistol, CCW; includes Nasmat A2 |
| 4 | 25 | 0 | SMG, Boarding Pistol, CCW; includes Nasmat A2 |

**Nasmat A2:** `MOV 15-10 | CC 8 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 1`; Peripheral (Servant), Courage, Mimetism (-3), Parachutist, Terrain (Total), PARA CCW (-3).

### Nasmat Remotes

**ID 333 · AVA 4 · REM** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 1`; Courage, Mimetism (-3), Peripheral (Servant).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 3 | 0 | PARA CCW (-3); no Order |

### Kameel Remotes

**ID 334 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | STR 1 | S 4`; Baggage, Courage, Remote Presence.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 8 | 0 | Repeater, Deactivator, PARA CCW (-3) |
| 2 | 14 | 0.5 | EVO Hacking Device, Hacker, PARA CCW (-3) |
| 3 | 16 | 0 | Repeater, Rifle, Light Shotgun, PARA CCW (-3); Total Reaction |

### Tarik Mansuri, Khawarij Amir

**ID 319 · AVA 1 · MI** — `MOV 15-10 | CC 23 | BS 13 | PH 14 | WIP 15 | ARM 3 | BTS 3 | W 2 | S 5`  
**Common:** CC Attack (-6), BS Attack (-3), Dodge (+5), Warhorse, Natural Born Warrior, Immunity (ARM), Combat Instinct, Stealth, Religious Troop, Terrain (Total), Super-Jump (7.5).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 49 | 1.5 | AP Spitfire, Pulzar (+1B), Heavy Pistol, DA CCW (PS=5) | Wildcard; counts as Khawarij |
| 3 | 46 | 0 | AP Rifle, Light Shotgun, Pulzar (+1B), Heavy Pistol, DA CCW (PS=5); Tactical Awareness | same |
| 5 | 47 | +1 | AP Rifle, Light Shotgun, Pulzar (+1B), Heavy Pistol, DA CCW (PS=5); Lieutenant (+1 Order) | same |
| 6 | 53 | 1.5 | AP Spitfire, Pulzar (+1B), Heavy Pistol, DA CCW (PS=5); Lieutenant (+1 Order) | same |

### Carmen Johns & Bâtard

**ID 1153 · AVA 1 team**

**Carmen:** `MOV 20-10 | CC 22 | BS 11 | PH 13 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 4`; Irregular, Impetuous, CC Attack (-6), Booty, Limited Cover, Courage, Dodge (+5), Natural Born Warrior, Mimetism (-3), Dogged, Motorcycle.  
**Loadout:** 17 pts / 0 SWC — Chain Rifle (+1B), Smoke Grenades, Grenades, AP Heavy Pistol (+1B), DA CCW (PS=6).

**Bâtard:** `MOV 15-15 | CC 22 | BS 0 | PH 15 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 5`; CC Attack (Shock), Courage, Dodge (+5), Mimetism (-3), Peripheral (Synchronized), Sensor, Dogged. Trench-Hammer (PS=5), Grenades (PS=6), AP CCW (PS=5).

### Beasthunters Free Guild

**ID 1570 · AVA 1 · SK** — `MOV 10-10 | CC 21 | BS 11 | PH 13 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`; Mimetism (-3), Stealth, Super-Jump, Terrain (Total), Religious Troop; Irregular.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 9 | 0 | **BEASTHUNTER FTO**; Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CCW (PS=5) | Ramah max 1 |
| 2 | 15 | 0 | Heavy Flamethrower, Tactical Bow, AP Mine, Pistol, DA CCW; Camouflage, Surprise Attack (-3), Forward Deployment (+20) | — |
| 3 | 15 | 0 | Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CCW; same camouflage package | — |

### Haytham Aero-unit

**ID 1851 · AVA 1 · VH** — `MOV 20-5 | CC — | BS 13 | PH 13 | WIP 14 | ARM 3 | BTS 6 | STR 2 | S 7`  
**Common:** MSV1, Aerial, Courage, Dodge (-3), Mimetism (-6), No Cover, Super-Jump (Jet Propulsion; 7.5), Terrain (Total), BS Attack (Continuous Damage), Tech-Recovery.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 33 | 1.5 | Red Fury, Panzerfaust, AP Heavy Pistol (+1B) |
| 2 | 29 | 0 | Heavy Shotgun (+1B), Chain Rifle, Panzerfaust |

### Ghulam Infantry

**ID 301 · AVA Total · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`; Terrain (Desert).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 11 | 0 | Rifle, Light Shotgun, Pistol, CCW | Ramah |
| 2 | 20 | 1 | HMG, Pistol, CCW | same |
| 4 | 17 | 1.5 | Missile Launcher, Pistol, CCW | same |
| 7 | 16 | 0.5 | Rifle, Light Shotgun, Pistol, CCW; Hacking Device, Hacker | same |
| 8 | 15 | 0 | Rifle, Light Shotgun, Pistol, CCW; MediKit, Doctor (+3) | same |
| 9 | 12 | 0 | Rifle, Light Shotgun, Flash Pulse, Pistol, CCW; Forward Observer | same |
| 10 | 13 | 0 | Rifle, Light Shotgun, E/M Mine, Pistol, CCW; Deployable Repeater | same |
| 11 | 11 | 0 | Rifle, Light Shotgun, Pistol, CCW; Lieutenant | same |
| 14 | 15 | 1 | Rifle, Grenade Launcher, Smoke Grenade Launcher, Pistol, CCW; NCO | same |
| 18 | 12 | 0 | Rifle, Light Shotgun, Panzerfaust, Pistol, CCW; Number 2 | same |
| 19 | 15 | 0 | Rifle, Light Shotgun, Pistol, CCW; Lieutenant (+1 Command Token) | same |
| 20 | 13 | 0 | Rifle, Light Shotgun, Pistol, CCW; Commlink (+2), Specialist Operative | same |

### Dr. Claire Lazhari

**ID 1894 · AVA 1 · LI** — `MOV 15-5 | CC 16 | BS 13 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`; BS Attack (Continuous Damage), MediKit (PH=17), Dodge (+3/+2.5), Immunity (Enhanced), No Wound Incapacitation.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 0 | Breaker Combi Rifle, Nanopulser (+1B), Viral Pistol (+1B), PARA CCW (-3), Disco Baller; MediKit; Doctor (2W) | Wildcard |
| 2 | 33 | 0 | **CLAIRE LAZHARI FTO**; same weapon suite; Doctor (+3) | Wildcard |

### Yara Haddad

**ID 1548 · AVA 1 · MI** — `MOV 10-10 | CC 16 | BS 13 | PH 11 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`; MSV2, Immunity (ARM), Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 0 | AP Marksman Rifle, Heavy Pistol (+1B), CCW | Wildcard |
| 3 | 24 | 0 | Same; Lieutenant | Wildcard |

### Hunzakuts

**ID 310 · AVA 1 · SK** — `MOV 10-10 | CC 14 | BS 11 | PH 12 | WIP 14 | ARM 0 | BTS 0 | W 1 | S 2`; Irregular, Surprise Attack (-3), Camouflage, Infiltration, Mimetism (-3), Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 18 | 0.5 | Rifle, Grenade Launcher, Shock Mine, Boarding Pistol, CCW; Deployable Repeater |
| 2 | 18 | 0.5 | Sniper Rifle, Shock Mine, Boarding Pistol, CCW |
| 3 | 19 | 0 | Rifle, Light Shotgun, Shock Mine, Boarding Pistol, CCW; Deployable Repeater, Forward Observer |
| 4 | 15 | 0 | Boarding Shotgun, D-Charges, Boarding Pistol, CCW; Forward Observer |

### Nahab Aeromobile Team

**ID 1314 · AVA 3 · LI** — `MOV 10-10 | CC 23 | BS 12 | PH 13 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`  
**Common:** Martial Arts L3, Berserk, Courage, Dodge (+5), Immunity (ARM/Critical), Decoy (2), Stealth, No Wound Incapacitation, Terrain (Total), BS Attack (-3), Frenzy, Jump (7.5), Bangbomb (+4).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 39 | 1 | Red Fury, Zapper, Pistol, Viral CCW (PS=6); Infiltration |
| 2 | 32 | 0 | Boarding Shotgun, Zapper, D-Charges, Pistol, Viral CCW; Infiltration, Specialist Operative |
| 3 | 36 | 0 | SMG, E/Mitter, Zapper, Pistol, Viral CCW; Infiltration, Killer Hacking Device, Hacker |
| 4 | 38 | 1 | Red Fury, Zapper, Pistol, Viral CCW; Parachutist |
| 5 | 31 | 0 | Boarding Shotgun, Zapper, D-Charges, Pistol, Viral CCW; Parachutist, Specialist Operative |
| 6 | 35 | 0 | SMG, E/Mitter, Zapper, Pistol, Viral CCW; Parachutist, Killer Hacking Device, Hacker |

### Al Fasid Regiment

**ID 343 · AVA 3 · HI** — `MOV 10-10 | CC 17 | BS 13 | PH 14 | WIP 14 | ARM 5 | BTS 6 | W 2 | S 5`; Albedo (-3), Warhorse, Minelayer, Sixth Sense, Combat Instinct.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 50 | 1.5 | HMG, Grenade Launcher, Smoke Grenade Launcher, Shock Mine, Heavy Pistol, CCW (PS=6); BS Attack (SR-1) | Janissaries / Armored Assault |
| 2 | 44 | 1.5 | Heavy Rocket Launcher, SMG, Shock Mine, Heavy Pistol, CCW (PS=6); BS Attack (+1SD) | same |

### Naffatûn

**ID 302 · AVA 5 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`; Terrain (Desert).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 11 | 0 | Rifle, Light Flamethrower (PS=6), Grenades, Pistol, CCW | Ramah; counts as Ghulam |
| 2 | 11 | 0 | Rifle, Heavy Flamethrower, Pistol, CCW | same |
| 3 | 11 | 0 | As option 1; Lieutenant | same |

### Shihab Remotes

**ID 316 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`; 360º Visor, Courage, Immunity (Shock), Remote Presence, Total Reaction.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 23 | 1 | HMG, PARA CCW (-3) |
| 2 | 18 | 0 | Thunderbolt (+1B), PARA CCW (-3) |

### Fanous Remotes

**ID 318 · AVA 3 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`; Repeater, Courage, Mimetism (-3), Remote Presence.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) |

### Burkut, Aerospace Engineering Regiment

**ID 1759 · AVA 2 · HI** — `MOV 10-10 | CC 16 | BS 12 | PH 12 | WIP 14 | ARM 3 | BTS 6 | W 1 | S 2`  
**Common:** Engineer, Immunity (Shock, Continuous Damage), Mimetism (-3), No Wound Incapacitation, Terrain (Zero-G), Religious Troop, Deactivator, GizmoKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 28 | 0 | Boarding Shotgun (+1B), Panzerfaust, AP Mine, D-Charges, Pistol, CCW | Wildcard; counts as Janissary |
| 2 | 30 | 0.5 | SMG, Light Rocket Launcher (PS=6), D-Charges, Pistol, CCW | same |
| 3 | 26 | 0 | SMG, E/Marat (+1B), AP Mine, D-Charges, Pistol, CCW | same |
| 4 | 28 | 0 | SMG, Heavy Flamethrower (+1B), AP Mine, D-Charges, Pistol, CCW | same |

### Husam Operative Leila Sharif

**ID 849 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`; Religious Troop, Combat Instinct; Killer Hacking Device with Carbonite + Firewall (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 22 | 0 | Shock Marksman Rifle, E/M Mine, D-Charges, Breaker Pistol, CCW; Hacker | Wildcard; counts as Ghulam |

### Hortlak Janissaries

**ID 1316 · AVA 2 · HI** — `MOV 10-10 | CC 15 | BS 13 | PH 12 | WIP 14 | ARM 3 | BTS 3 | W 1 | S 2`  
**Common:** MSV1, BS Attack (SR-1), Immunity (Shock), Mimetism (-3), Stealth, Religious Troop, No Wound Incapacitation, Combat Instinct.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 27 | 0 | AP SMG, E/Mitter, Pulzar (+1B), Viral Pistol, CCW | Janissaries; counts as Janissary |
| 2 | 31 | 0.5 | K1 Marksman Rifle, Pulzar, Viral Pistol, CCW | same |
| 3 | 31 | 0.5 | AP Sniper Rifle, Viral Pistol, CCW | same |
| 4 | 29 | 0 | AP SMG, Blitzen, Pulzar, Viral Pistol, CCW; Chain of Command | same |
| 5 | 28 | 0 | AP SMG, E/Mitter, Pulzar, Disco Baller, Viral Pistol, CCW; Deactivator | same |

### Janissaries

**ID 308 · AVA 5 · HI** — `MOV 10-10 | CC 18 | BS 14 | PH 14 | WIP 14 | ARM 4 | BTS 6 | W 2 | S 2`; Dodge (+2.5), Religious Troop, BS Attack (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 31 | 0 | AP Rifle, Light Shotgun, Pulzar, Heavy Pistol, CCW (PS=6) | Janissaries |
| 2 | 38 | 1.5 | HMG, Pulzar, Heavy Pistol, CCW (PS=6) | same |
| 4 | 28 | 0 | Boarding Shotgun, Pulzar, Heavy Pistol, CCW (PS=6); TinBot Firewall (-3) | same |
| 5 | 32 | 0 | AP Rifle, Light Shotgun, Pulzar, Heavy Pistol, CCW (PS=6); TinBot Firewall (-3) | same |
| 6 | 36 | 1.5 | Missile Launcher, Pulzar, Heavy Pistol, CCW (PS=6) | same |
| 10 | 35 | 0 | AP Rifle, Light Shotgun, Pulzar, Heavy Pistol, CCW; MediKit, Doctor (2W) | same |
| 11 | 31 | 0 | AP Rifle, Light Shotgun, Pulzar, Heavy Pistol, CCW; Lieutenant | same |
| 12 | 32 | 0 | AP Rifle, Light Shotgun, Pulzar, Heavy Pistol, CCW; TinBot Firewall (-3), Lieutenant | same |

### Namurr Experimental Operative Group

**ID 1315 · AVA 2 · MI** — `MOV 15-5 | CC 21 | BS 13 | PH 12 | WIP 14 | ARM 2 | BTS 6 | W 2 | S 2`  
**Common:** X-Visor, CC Attack (+1B), Courage, Dodge (+3/+2.5), Specialist Operative, Terrain (Total), Climbing Plus, Immunity (Enhanced), BS Attack (+1B).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 44 | 1 | Spitfire, Heavy Pistol, E/Marat, D-Charges, E/M CCW (PS=7) | Ramah / Wildcard |
| 3 | 41 | 0 | Breaker Rifle, Light Shotgun, Heavy Pistol, E/Marat, D-Charges, E/M CCW (PS=7); Tactical Awareness | Ramah / Wildcard |

### Fiddler, Aristeia!'s ex-toymaker

**ID 1564 · AVA 1 · LI** — `MOV 15-10 | CC 18 | BS 12 | PH 12 | WIP 14 | ARM 1 | BTS 3 | STR 1 | S 2`; CC Attack (+1B), Dodge (+3/+2.5), Engineer, Immunity (Critical), No Wound Incapacitation, GizmoKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 29 | 0 | **Fiddler FTO**; Contender (+1B), Drop Bears, D-Charges, Breaker Pistol, PARA CCW (-3); Super-Jump | Ramah max 1 |
| 2 | 36 | 0 | Same core weapons; Climbing Plus; includes 1 Jackbot | — |
| 3 | 43 | 0 | Same core weapons; Climbing Plus; includes 2 Jackbots | — |

**Jackbot:** `MOV 15-10 | CC 16 | BS 11 | PH 10 | WIP 12 | ARM 0 | BTS 3 | STR 1 | S 1`; Peripheral (Synchronized), Courage, Explode, Climbing Plus; Vulkan Shotgun.

## Fireteams

### FT-01 — Ramah Taskforce Fireteams

**Types:** Core, Haris, Duo  
**Wildcard team:** no  
**Required-choice:** at least one member from the source-required set `{Ghulam, Naffatûn, Zhayedan, Khawarij, Namurr}`.

| Member | Unit ID | Required set | Min | Max | Counts as | Profile restriction | Notes |
|---|---:|---|---:|---:|---|---|---|
| Ghulam | 301 | yes | 0 | 5 | — | all | source `required: true` |
| Naffatûn | 302 | yes | 0 | 5 | Ghulam | all | source comment `(Ghulam)` |
| Zhayedan | 305 | yes | 0 | 5 | Ghulam | all | source comment `(Ghulam)` |
| Khawarij | 303 | yes | 0 | 5 | — | all | source `required: true` |
| Namurr | 1315 | yes | 0 | 2 | — | all | source `required: true` |
| Sayiq | 1849 | no | 0 | 1 | — | all | — |
| Beasthunter FTO | 1570 | no | 0 | 1 | — | option 1 only | exact FTO name |
| Fiddler FTO | 1564 | no | 0 | 1 | — | option 1 only | Jackbot-bearing options excluded |
| Husam Spec-Ops | 1916 | no | 0 | 1 | — | Spec-Ops mode | source comment `Spec-Ops` |

### FT-02 — Mukhtar Fireteams

**Types:** Duo, Haris

| Member | Unit ID | Required | Min | Max | Counts as | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Mukhtar | 1313 | no | 1 | 3 | — | all |

### FT-03 — Janissaries Fireteams

**Types:** Core, Haris

| Member | Unit ID | Required | Min | Max | Counts as | Profile restriction |
|---|---:|---|---:|---:|---|---|
| Janissary | 308 | no | 1 | 5 | — | all |
| Hortlak | 1316 | no | 0 | 2 | Janissary | all |
| Al Fasid | 343 | no | 0 | 1 | — | all |
| Wild Bill | 1482 | no | 0 | 1 | — | all |

### FT-04 — Armored Assault Fireteams

**Types:** Duo  
**Required-choice:** at least one member from `{Al Fasid, Shakush, Maghariba, Rafiq Remote FTO}`.

| Member | Unit ID | Required set | Min | Max | Counts as | Profile restriction | Notes |
|---|---:|---|---:|---:|---|---|---|
| Al Fasid | 343 | yes | 0 | 2 | — | all | source `required: true` |
| Shakush | 1546 | yes | 0 | 2 | — | all | source `required: true` |
| Maghariba | 309 | yes | 0 | 2 | — | all | source `required: true` |
| Rafiq Remote | 315 | yes | 0 | 2 | — | option 3 only | source comment `FTO` |
| Zhayedan | 305 | no | 0 | 1 | — | all | — |

### Wildcards

| Unit | Unit ID | Max | Counts as | Profile restriction | Notes |
|---|---:|---:|---|---|---|
| Namurr | 1315 | 2 | — | all | — |
| Burkut | 1759 | 2 | Janissary | all | source `(Janissary)` |
| Tarik Mansuri | 319 | 1 | Khawarij | all | source `(Khawarij)` |
| Leila Sharif | 849 | 1 | Ghulam | all | source `(Ghulam)` |
| Yara Haddad | 1548 | 1 | — | all | — |
| Rahman Rouhani | 1549 | 1 | — | all | — |
| Valerya Gromoz | 464 | 1 | — | all | — |
| Claire Lazhari | 1894 | 1 | — | all | chart does not restrict wildcard access to her FTO option |

## Unit → Fireteam access index

| Unit | Fireteam | Type | Access | Counts as | Profile restriction | Min/Max |
|---|---|---|---|---|---|---|
| Ghulam | FT-01 Ramah | Core/Haris/Duo | required-choice | — | all | 0–5 |
| Naffatûn | FT-01 Ramah | Core/Haris/Duo | required-choice / counts-as | Ghulam | all | 0–5 |
| Zhayedan | FT-01 Ramah | Core/Haris/Duo | required-choice / counts-as | Ghulam | all | 0–5 |
| Khawarij | FT-01 Ramah | Core/Haris/Duo | required-choice | — | all | 0–5 |
| Namurr | FT-01 Ramah | Core/Haris/Duo | required-choice | — | all | 0–2 |
| Namurr | eligible main teams | varies | wildcard | — | all | max 2 |
| Sayiq | FT-01 Ramah | Core/Haris/Duo | native | — | all | 0–1 |
| Beasthunter | FT-01 Ramah | Core/Haris/Duo | native | — | option 1 FTO | 0–1 |
| Fiddler | FT-01 Ramah | Core/Haris/Duo | native | — | option 1 FTO | 0–1 |
| Husam Spec-Ops | FT-01 Ramah | Core/Haris/Duo | special | — | Spec-Ops mode | 0–1 |
| Mukhtar | FT-02 Mukhtar | Duo/Haris | native | — | all | 1–3 |
| Janissary | FT-03 Janissaries | Core/Haris | native | — | all | 1–5 |
| Hortlak | FT-03 Janissaries | Core/Haris | counts-as | Janissary | all | 0–2 |
| Al Fasid | FT-03 Janissaries | Core/Haris | native | — | all | 0–1 |
| Al Fasid | FT-04 Armored Assault | Duo | required-choice | — | all | 0–2 |
| Wild Bill | FT-03 Janissaries | Core/Haris | native | — | all | 0–1 |
| Shakush | FT-04 Armored Assault | Duo | required-choice | — | all | 0–2 |
| Maghariba | FT-04 Armored Assault | Duo | required-choice | — | all | 0–2 |
| Rafiq Remote | FT-04 Armored Assault | Duo | required-choice | — | option 3 FTO | 0–2 |
| Zhayedan | FT-04 Armored Assault | Duo | native | — | all | 0–1 |
| Burkut | eligible main teams | varies | wildcard | Janissary | all | max 2 |
| Tarik Mansuri | eligible main teams | varies | wildcard | Khawarij | all | max 1 |
| Leila Sharif | eligible main teams | varies | wildcard | Ghulam | all | max 1 |
| Yara Haddad | eligible main teams | varies | wildcard | — | all | max 1 |
| Rahman Rouhani | eligible main teams | varies | wildcard | — | all | max 1 |
| Valerya Gromoz | eligible main teams | varies | wildcard | — | all | max 1 |
| Claire Lazhari | eligible main teams | varies | wildcard | — | all | max 1 |

## Reinforcement Fireteams — Melek Reaction Group

**Linked Army ID:** 499  
**Source slug:** `melek-reaction-group`  
**Source chart-level spec:** Core `0`, Haris `0`, Duo `0`. The source nevertheless explicitly defines named Reinforcement Fireteams below; those named rows are preserved verbatim rather than discarded because of the chart-level zero values.

### Reinforcement roster index

| Unit ID | Reinforcement unit | AVA | Type | Notes |
|---:|---|---:|---|---|
| 1654 | Hafza Unit REINF. | 2 | LI | Wildcard; counts as Sekban REINF. |
| 1656 | Korsan, Corsairs of the Gate REINF. | 2 | LI | Sekban team; source chart marks FTO |
| 1662 | Al Hawwa' Unit REINF. | 2 | SK | Sekban and Azra'il teams |
| 1664 | Nasmat Remotes REINF. | 2 | REM | Peripheral (Servant) |
| 1660 | Burkut REINF. | 2 | HI | Wildcard; counts as Sekban REINF. |
| 1666 | Rahman Rouhani REINF. | 1 | LI | Wildcard |
| 1658 | Djanbazan Tactical Group REINF. | 1 | MI | Wildcard |
| 1659 | Sekban, Naval Special Unit REINF. | 4 | MI | Native reinforcement Fireteam anchor |
| 1655 | Odalisques REINF. | 2 | LI | Sekban team |
| 1665 | Leila Sharif REINF. | 1 | LI | Wildcard |
| 1663 | Rafiq Remotes REINF. | 1 | REM | Wildcard |
| 1657 | Hakims REINF. | 2 | MI | FTO profiles in Sekban team |
| 1661 | Azra'il REINF. | 2 | HI | Native Duo anchor |

### RFT-01 — Sekban Reinforcement Fireteams

**Types:** Core, Haris, Duo

| Member | Unit ID | Min | Max | Counts as | Restriction / notes |
|---|---:|---:|---:|---|---|
| Sekban REINF. | 1659 | 1 | 4 | — | native anchor |
| Odalisque REINF. | 1655 | 0 | 2 | — | — |
| Hakim FTO REINF. | 1657 | 0 | 2 | — | FTO profiles only |
| Korsan REINF. | 1656 | 0 | 2 | — | source chart comment `FTO` |
| Hawwa' REINF. | 1662 | 0 | 2 | — | — |

### RFT-02 — Azra'il Reinforcement Fireteam

**Types:** Duo

| Member | Unit ID | Min | Max | Notes |
|---|---:|---:|---:|---|
| Azra'il REINF. | 1661 | 1 | 2 | native anchor |
| Hawwa' REINF. | 1662 | 0 | 1 | — |

### Reinforcement Wildcards

| Unit | Unit ID | Max | Counts as | Notes |
|---|---:|---:|---|---|
| Hafza REINF. | 1654 | 2 | Sekban REINF. | source `(SEKBAN REINF)` |
| Burkut REINF. | 1660 | 2 | Sekban REINF. | source chart spells member slug `reinf-burtuk`; normalized to actual unit `reinf-burkut` |
| Djanbazan REINF. | 1658 | 1 | — | — |
| Rafiq Remote REINF. | 1663 | 1 | — | — |
| Leila Sharif REINF. | 1665 | 1 | — | — |
| Rouhani REINF. | 1666 | 1 | — | — |

No source-defined exception permits mixing these Reinforcement troops into Ramah's main Fireteams.

## Provenance and validation

- Corvus Belli Army-derived source revision: `7.26246.158`
- Army data changed on: `2026-09-03`
- Ramah source path: `n5/ramah-taskforce/7.26246.158.json`
- Ramah source blob: `19015770025b60a73cda1e41b59766ea9a778afd`
- Linked reinforcement source: `n5/melek-reaction-group/7.26246.158.json`
- Melek source blob: `1c4c1854468cb733649b98ed12d41317afc6c551`
- InfinityDB commit: `4e2662be3f43387fbae42b3790a711b3e98570c4`
- Generated / verified: `2026-10-15`

Validation performed:

1. Standard roster count reconciled to 37 logical Ramah units; optional Spec-Ops / Team-Ops separated.
2. Generic `factions: []` mercenary catalogue excluded.
3. All standard Ramah unit sections include current base profile data and source loadout points/SWC.
4. Main Fireteam membership, min/max, required-choice sets, Counts-as labels, Wildcards, and FTO restrictions reconciled against the source chart.
5. Rafiq, Beasthunter, and Fiddler FTO restrictions point to existing source loadouts.
6. Reverse Fireteam index reconciled to the canonical chart.
7. Melek Reaction Group roster and named Reinforcement Fireteams kept separate from the main chart.
8. Source typo `reinf-burtuk` in the reinforcement Wildcard chart is explicitly normalized to the actual `reinf-burkut` unit rather than creating a phantom unit.
