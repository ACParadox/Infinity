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

## Community tactics — N5 transcript-backed research (2026-10-22)

> **Precedence:** These are **community tactics, not Army data**. The authoritative roster, weapon options, AVA, costs and Fireteams are the pinned **N5.3 / Army 7.26246.158** sections above (verified 2026-10-15); current main roster has **37 entries**. **One Core, one Haris, unlimited Duos**. Match every suggested list against that chart. N5 videos from **August 2025** predate the October 2025 N5.2 update; Robert Shepherd's post-October N5 video and the November 2025 Tactical Awareness episode give useful later perspectives. Historical N4 podcast mechanics/points are NOT current legality.

### One-minute read

- **Strength:** highly mobile *problem-solvers* (Tarik/Khawarij, Namurr, Mukhtar, Nahab), strong burst/modifier infantry shooting (Janissary, Zhayedan), efficient cheap orders (Ghulam/Naffatûn/Fanous), an excellent **Haytham flyer**, and **Maghariba/Shakush** TAG access. You often have the right offensive *tool*; the challenge is paying for it without destroying your order/defense budget.
- **Weakness:** premium models are costly, and many fast super-soldiers are only one Wound or lack defense in the enemy active turn. Limited infiltrating midfield, thin expendable screening, narrow long-range anti-armor outside TAGs, and easy-to-attack expensive pieces make Ramah a **positioning and target-selection army**, not a simple shove-everything-forward elite faction.
- **Best general solution:** one premium active attacker **plus** a practical mission/defense backbone, not four unsupported premium units. Build deliberately for **going second**: a couple of Shihabs/Flash REMs, a Monstrucker/Nasmat to repair them, inexpensive template defenders, and depth protecting elite models from alpha strikes.
- **Sectorial identity disagreement:** Tactical Awareness emphasizes the unusually tough, efficient and fast *individual* super-soldiers, especially Tarik. Robert Shepherd considers post-October Ramah one of N5's **challenge factions** due to expensive profiles, structural gaps and required defense spending. Burlesford enjoys its improved N5 options but agrees it punishes sloppy list building. These are compatible observations: *excellent highlight models do not automatically make an effortless army*.

### Build from roles: units, use-case and *why*

| Unit / package (verified N5.3) | Why take it | Main opportunity cost / failure mode |
|---|---|---|
| **Tarik Mansuri** AP Spitfire (49) / TacAware AP rifle (46) / Lt variants | BS13 with BS Attack (-3), **2W, Super-Jump, 15-10 MOV**, CC23, ARM-immunity, strong mobility and meaningful CC. He changes attack angles, bypasses normal defensive approaches and can engage models too well-defended for ordinary BS13. TacAware can fund his own moves; Lt (+1 Order) can supercharge a prepared attack. | **46–53 pts**, possible obvious Lt and a tempting reactive-turn target. Protect/stage him instead of parking in the midfield. If Lt, bring credible **Chain of Command** (Khawarij or Hortlak) or a sound LoL plan; Lt orders and NCO availability must be checked per list. |
| **Khawarij** MSV2 Mk12/NCO (38), Doctor (+3) (30), CoC/Disco (33), AP Spitfire (35), HRL (29) | **15-5 MOV + Super-Jump**, CC23, ARM immunity, viral CC; bring the exact tool for movement, MSV+smoke, specialist recovery, Lt insurance, or a linkable assault gun. Doctor (+3) brings downed Tarik and other troopers back. | **Only 1 Wound** on 29–38 pt profiles: even immunity doesn't let them survive repeated saves or a failed aggressive leap. Big Tarik/Khawarij Core is exciting but a concentration risk; usually preserve multiple attack vectors. |
| **Namurr**, 41-pt Tactical Awareness Breaker Rifle / 44-pt Spitfire | **2W, Immunity (Enhanced), Specialist, Climbing Plus, X-Visor, E/Marat, E/M CCW, D-Charges**. Excellent *answer to hard targets* the Red Fury/Haytham might struggle with, and TacAware helps the costly specialist reach objectives. Can join a Ramah Fireteam or Wildcard; a pair can split missions. | 41–44 pts with ARM2 and close/mid-range guns. Spending most of the list on this one problem-solver leaves insufficient screens. Prefer her for **E/M access + objective utility**, not a generic turret. |
| **Mukhtar Haris/Duo**, MSV2 Red Fury (34), FO (25), Doctor (26), Hacker (29) | **Forward Deployment +10, Mimetism (-3), NWI, BTS6, 15-5 MOV**; Red Fury MSV2 makes a mobile visor shooter; FO/Doctor/Hacker creates a self-contained objective team. Pure Mukhtar Duo/Haris is its native team (not a Core). | Spend 25–34 pts each; their NWI doesn't make ARM2 safe when many hits connect. **Burlesford prefers a Khawarij gun** because its Super-Jump/CC tools can outperform this package, whereas Robert argues Mukhtars are some of the few fairly priced Ramah units. Both depend on scenario and whether active shooting or specialists are needed. |
| **Janissary HMG (38) / ML (36)** + Hortlak/Burkut | BS14, BS Attack (-3), **2W ARM4 BTS6** produces unusually reliable face-to-face infantry shooting; ML secures ARO, TinBot supports hackable HI teams. **Hortlak K1 Marksman (31), CoC (29), Disco (28)** and **Burkut Engineer** can attach as permitted, adding anti-armor, Lt insurance or repair. | 10-10 MOV means avoid overcommitting to a slow five-model Core; only **one Haris** overall. Robert notes Hortlak's good standalone profile can be crowded out by *having to pay for at least one Janissary* in a Janissaries team. |
| **Zhayedan HMG (31) / AP sniper (27)** + Ghulam NCO / Naffatûn | Marksmanship, Warhorse, Regeneration and counts-as **Ghulam** give strong mid-price, good-modifier active/ARO shooting embedded in a cheaper Ramah team, without committing to Janissary-only infrastructure. | One Wound and 10-10 MOV: protect him and use modifiers; still just BS12. Competes with Janissary if you can afford the tougher, more consistent primary gun. |
| **Ghulam NCO Smoke GL (15)** + inexpensive specialist / Zhayedan | Converts an available Lt Order into **smoke, speculative grenades, or repositioning**. Useful low-investment Duo in a second combat group, especially when the main group contains expensive guns. 11-pt Naffatûn adds a disposable flamethrower guard and counts as Ghulam. | The NCO order is not an additional Regular Order; do not build a smoke-shooting plan that assumes smoke succeeds on the first attempt. Smoke + MSV2 **Yara/Khawarij/Mukhtar** needs correct enemy vision-counter matchups. |
| **Yara Haddad (24)** | Cheap **MSV2 AP Marksman Rifle** Wildcard, a practical smoke shooter when a full specialist super-soldier team would be unaffordable. | 1W, BS13, short/mid-range bands; lighter than Mukhtar or linked Janissary. Excellent utility/secondary gun, not a replacement for heavy anti-armor. |
| **Leila Sharif / Valerya Gromoz** | **Leila KHD** with Combat Instinct/Carbonite can provide narrow anti-hacker and reactive coverage; **Valerya WIP14, Pitcher, Total Control** projects a hacking network in a legal team. | Ramah does not automatically want an expensive hacking castle: most super-soldiers are not hackable; TAGs, Janissaries and the flyer **are**. Choose a defensive/hacking plan for what you actually field. |
| **Tuareg** hidden/infiltrating KHD / Doctor / other | Hidden Deployment and WIP15 let a KHD ambush exposed enemy hackers and then reclaim camouflage; a hidden Doctor can stage ahead of the attack force for recovery. Valuable when enemy KHDs threaten your Haytham/TAGs. | Premium midfield tech; avoid challenging enemy apex hackers behind strong TinBots/Firewall. Not a substitute for cheap broad midfield board coverage. |
| **Hunzakut FO (15/19)** | Infiltrating Camouflage, mines and optional deployable Repeater project scenario control and hacking from a forward position. **AVA1** in Ramah is precious. | **Irregular**, 1W, AVA1. Don't assume Vanilla Haqqislam's AVA or Regular-order support carries over. |
| **Nahab** infiltrating/Parachutist Specialist (32/31), KHD (36/35), Red Fury (39/38) | Mimetism-free but **Decoy, NWI, MA3, Viral CC, Berserk, Zapper and Stealth** gives a surgical assault/objective threat with surprising melee power; Parachutist exploits a poorly screened edge, Infiltration pressures midfield objectives. | Expensive and difficult to conceal after exposing. Red Fury/Viral can struggle to convert against TAG-grade armor; Robert prefers the Parachutist on the appropriate mission instead of routinely paying for a midfield infiltrator. |
| **Carmen Johns & Bâtard (17)** | Motorcycle Smoke + synchronized warband, explosive close-range threat and Bâtard Sensor. Both Robert and Tactical Awareness describe this as unusually high-value for Ramah because it provides **smoke + disruption + a close-combat trade** outside a premium Fireteam. | Irregular, Impetuous and exposed; plan around line of fire and Orders. Don't rely on them surviving the enemy's full reactive turn. |
| **Hakim Parachutist Doctor (+3), optional Nasmat A2** | Arrives near a wounded forward assault group or scores late objectives without marching a slower Doctor across the table; excellent in a mission where edge-entry and recovery line up. | At 24–29 pts, a backfield Doctor is far cheaper if there is no reliable drop lane; **Nasmat A2** is a servant, not an extra Order or generic Airborne unit. |
| **Monstrucker (12–16) + Nasmat** | Cheap engineer for Shihab/TAGs/Haytham repair; Climbing Plus, Drop Bears/turret options add deployment-zone depth. Great in **second combat group** to make enemy Orders spent killing TR remotes potentially wasted. | **Irregular**; do not count its own Order as a Regular pool contribution. Protect it; it works best as a repair piece, not a front-line attacker. |
| **Beasthunter FTO (9) / Fiddler FTO (29)** | Beasthunter offers a cheap dangerous Panzerfaust/midfield ARO in the **Ramah** link. **Fiddler FTO** can engineer and Drop Bear with Super-Jump as a linkable utility specialist. | **Only specific FTO options** may join FT-01. Fiddler's **36/43 pt Jackbot options are not FT-01 members**; those are solo specialist/attack packages. |
| **Al Fasid HMG/GL/Smoke (50), HRL (44)** | Armor, Albedo, layered mines and anti-approach weapons allow a slower defensive/heavy-gun specialist in Janissaries or Armored Assault; unusual smoke/area denial on HI. | Frequently judged **overcosted** against Tarik, Janissary, cheap smoke and TAGs; buy only if its area-denial bundle answers a specific enemy rather than paying 44–50 pts for a generic gun. |

### Fireteam/list architecture: legal scaffolds to test

- **Ramah primary:** Khawarij NCO/MSV2 Mk12 + Khawarij Doctor + Tarik (or a smaller Khawarij/Tarik Duo) to exploit Super-Jump and recovery. Optional Khawarij **CoC** if Tarik Lt. Core is possible but expensive; the pinned chart's FT-01 *required-choice* set must be met.
- **Budget fire support:** Zhayedan HMG/AP Sniper + Ghulam NCO smoke + Ghulam Doctor/Naffatûn/Leila, using counts-as **Ghulam** and the FT-01 set. The point is reliable function without 100+ pts of single attack package.
- **Independent objective unit:** Mukhtar **Red Fury MSV2 + FO/Doctor** Duo; or pure Mukhtar Haris with Hacker if scenario wants multiple WIP14 specialists. **Mukhtar cannot form Core.**
- **Janissary strike team:** Janissary HMG + Hortlak K1/CoC + Valerya/eligible Wildcard. If you want a defensive ML in Core, budget for it explicitly; Janissary/Hortlak are not an FT-01 wildcard substitute.
- **Armored Assault Duo:** **Maghariba/Shakush + Rafiq FTO** to bring Sensor/Repeater/Red Fury and a special-purpose team while the TAG goes active. **Rafiq 13-point non-FTO cannot take the FT-04 slot**. Alternatives include a TAG + a permitted Wildcard such as Namurr when the role and cost make sense.
- **Balanced 15-model concept:** main-group active gun and objective piece(s); **second combat group** Shihab(s), **Monstrucker (+Nasmat)**, three Fanous if affordable, plus Ghulam NCO smoke / Zhayedan for productive spare Orders. The 1-Haris limit means not stacking several Haris regardless of what a recorded example list says.

**Order-budget test:** Before adding a second expensive attack troop or TAG, calculate actual **Regular Orders in each combat group**. Monstrucker and Hunzakut are Irregular; TacAware and NCO have restrictions. The cost of Tarik + Namurr + Mukhtar + Maghariba in one list is the deployment/ARO plan you no longer can afford. Multiple vectors matter only when they can each receive Orders.

### TAG, VH, REM and repair ecosystem — Ramah-specific

| Eligible asset | Why / how to use it | Counterpoint / restriction |
|---|---|---|
| **Maghariba Guard TAG (AVA2)** 72pt E/M Carbine (+2B) / 71pt HRL+GL / 71pt Heavy Flamethrower (+1B)+Shock Mine Dispenser | **BS14, ARM8, BTS6, STR3, S8, 360°**, Tactical Awareness, **Baggage and ancillary Jandab specialist**. HMG plus flexible secondary package; the mine version **self-reloads** due to Baggage and guards approaches; E/M +2B punishes hard HI/TAGs. Rafiq FTO or support pieces can form Armored Assault Duo. **Sayiq Maghariba Pilot** supports its dodge/repair plan. | Great discount from N4, but **S8 is hard to hide** and Ramah can struggle to afford other middleweight specialists. **Burlesford loves Maggie**; Robert calls her solid but warns the faction is less able to exploit the space she creates. Choose the exact loadout to solve a target or lane, not automatically the mine version. |
| **Shakush TAG (AVA2)** 58pt HMG Continuous Damage / 56pt AP Spitfire | **BS14, ARM6, STR3, TacAware**, smaller and cheaper than Maggie. Continuous HMG is effective into hard infantry; AP Spitfire gives a closer-range armor breaker; legal Armored Assault Duo, can pair with mission utility such as an allowed Wildcard. **Sayiq Shakush Pilot** improves support/dodge plan. | **Direct disagreement:** Robert views it as fine and serviceable; burlesford feels **Janissary HMG + supporting models** more often does useful work for fewer points. **Shakush + Namurr** TacAware Duo is potent but costs about 100 pts, so an elite-tech temptation rather than default. |
| **Haytham Aero-unit (VH, AVA1)** 33pt Red Fury/Panzerfaust/AP Pistol, 29pt BSG (+1B)/Chain Rifle | **Actual Ramah vehicle**, BS13, **Mimetism (-6), MSV1, Continuous Damage, aerial Jet Propulsion**, 20-5 movement; threatens unusual vertical angles, isolated units and **other enemy vehicles** whose Mimetism it partially bypasses. Robert's post-October faction focus considers this close to default in Ramah; the dedicated [Vehicles Explained review](https://www.youtube.com/watch?v=N6TYjMgU4ZM) ranks it roughly **4th/8**, especially as a flyer hunter. | S7, **No Cover**, ARM3 / STR2 and hackability mean it can disappear suddenly in reactive turn. Dedicated vehicle review notes Ramah **already has** multiple mobile gunfighters, so Haytham isn't a unique mission solution. Usually pick Red Fury for a balanced hunter; BSG is the cheaper short-range option. |
| **Rafiq REM (AVA2)** 13pt Sensor/FO/Repeater or **19pt Red Fury FTO** | Cheap one brings **Sensor + Triangulated Fire + Forward Observer + Repeater** for camo discovery/objectives; FTO gains a credible Red Fury and can Duo with a TAG, other Rafiq FTO or permitted partner in **Armored Assault**. | The FT-04 Rafiq row is explicitly **option 3 FTO only** and a *required-choice* candidate; **no ordinary Rafiq Fireteam access**. Evaluate a 19pt utility gun against an extra 7pt Fanous or 13pt solo scout. |
| **Shihab REM (AVA2)** 23pt Total Reaction HMG / 18pt Total Reaction Thunderbolt (+1B) | Exceptional economical **defensive backbone**; overlap lanes instead of putting whole army's defense on one premium infantry gun. **Monstrucker/Najjarun/Burkut** repairs them and can trade its cheap support cost for enemy Orders. | Passive AROs lose to deliberate counters and have limited STR1; consider two complementary rangebands / positioning rather than both standing in one corridor. Robert repeatedly recommends a **group-two TR bot + Monstrucker** architecture to fix Ramah's second-turn weakness. |
| **Shaytaniyah REM (AVA1)** 16pt **Guided** ML / 19pt **non-Guided** ML (+1B) | Guided build converts **Targeted** via Valerya/Leila/FO/Repeaters into off-angle anti-bunker shots. +1B variant is a different direct/ARO piece. | **Only opt1 explicitly has Guided in the Ramah pinned source**: **do not attribute Guided to opt3** or copy Qapu/Hassassin data blindly. Without reliable Targeted setup, the 16pt/1.5 SWC guided tax often doesn't produce output. |
| **Kameel REM (AVA2)** 8pt Baggage/Repeater, 14pt EVO, 16pt Total Reaction Rifle | Cheap group filler and deployable reloader; **EVO** supports remotes/TAG/airborne plans when mission requires. Maggie already has native Baggage, so a second reloader is less essential *just* for her mines than for broader package support. | Do not buy EVO by default; a Fanous, Ghulam or specialist might contribute more to a non-tech plan. |
| **Fanous REM (AVA3)** 7pt Flash Pulse + Repeater | Probably Ramah's most consistent low-cost route to 15 models with **cheap defensive AROs and hacking coverage**; AVA3 means spam is legal here unlike narrower sibling sectorials. | Orders and models count, but a Flash bot is **not** a midfield specialist or a reliable stop against hard assault pieces. |
| **Nasmat / Jandab peripherals and Sayiq pilot** | **Nasmat** extends doctors/engineers; **Jandab** is bundled with Maghariba/Shakush and contributes scenario/screening tasks; **Sayiq pilot** is bought separately as current roster and supports TAG mobility/repair. | Peripherals **do not add Regular Orders**. A TAG's Jandab isn't a second independently purchased TAG or Fireteam member. Sayiq **belongs to FT-01 Ramah team**, *not* automatically FT-04 Armored Assault. |

**Across Haqqislam:** [Robert Shepherd's Vanilla Haqqislam N5 guide](https://www.youtube.com/watch?v=Dmv4pfdTbc0) corroborates Shakush's price-to-shooting value and Maghariba's Baggage/area denial, but he emphasizes **S8 concealment**. The [Aerial Vehicles Analysis & Ranking](https://www.youtube.com/watch?v=N6TYjMgU4ZM) explains flyer risk and Haytham's favorable vehicle-on-vehicle matchup. Other Vanilla units (e.g. **Scarface, Triphammer and Zeybek**) are **not** in pinned Ramah's 37-unit standard roster. **Iguana** is likewise unavailable. Some 2025 auto-transcripts call Zeybek **“Shaykh Bakr”** phonetically; this does not establish a separate roster entry. Do not import units or another sectorial's Fireteams/AVA.

### Opposing opinions — keep both, choose by mission

1. **Ramah viability:** **Robert Shepherd (post-N5.2):** powerful individual attackers but one of N5's challenge factions, lacking affordable mid-priced synergy and passive defense. **Burlesford (pre-N5.2):** N5 markedly improved the faction; deeply versatile/enjoyable, but requiring serious skill and acknowledging competitive gaps. **Tactical Awareness (N5):** Tarik and elite soldier offense is exceptional; some regiments are outdated or hard to justify. **Implication:** build depth and repeatable defense before rewarding yourself with a third flashy unit.
2. **Tarik auto-include?** **Tactical Awareness:** Tarik is exceptional in fast attack and hard to counter; one host dislikes his near all-purpose profile. **Burlesford:** powerful, not mandatory; Lt or second-turn exposure can lose the game. **Robert:** serious offense, but 46–53 pts and relatively limited reactive defense need careful staging. **Implication:** choose an LT/CoC plan, win useful fights first, then withdraw Tarik.
3. **Khawarij vs Mukhtar:** **Burlesford** now defaults more often to Khawarij MSV/NCO because Super-Jump mobility + distinct CC roles trump some Mukhtar durability. **Robert** praises Mukhtars as unusually fairly priced and self-sufficient, though notes Vanilla can exploit them better. **Implication:** Khawarij when movement/CC and Lt synergy matter; Mukhtar when Forward Deployment, Mimetism and specialists matter.
4. **Maghariba vs Shakush vs Janissary:** **Burlesford** says Maggie is better than ever, but is dissatisfied with Shakush relative to **Janissary HMG**; **Robert** says both TAGs are good enough, yet expensive in a sectorial missing inexpensive mid-tier support. **Implication:** take Maggie for a specific S8 + Baggage/weapon use-case, Shakush for TacAware TAG fire, Janissary for efficient gunfighting.
5. **Haytham must-take?** **Robert's Ramah focus** recommends one in most lists because of an aggressive **MSV1/Mimetism/Continuous Damage** angle and elite enemy flyer hunting. **His dedicated Vehicle ranking** simultaneously says it offers almost purely gunfighting and Ramah already has mobile attackers. **Implication:** extremely strong into other VHs and exposed troops; omit it when mission needs specialists or anti-hard-target answers more than another gun.
6. **Al Fasid / Hortlak / Burkut:** **Tactical Awareness** generally questions Al Fasid's points next to faster super-soldiers; **Robert** finds Hortlak good on paper but hampered by Janissary link anchor, and Burkut can be pricey for BS12. **Burlesford** likes Burkut BSG in the close-fight niche. **Implication:** select a specific supporting E/Marat, CoC, TinBot/Engineer, blast or Disco role rather than treating them as direct upgrades.
7. **Heavy hacking or minimal?** **Tactical Awareness** includes Valerya + Leila + Fanous/Guided experiments; **Robert** often prefers one good hacker and repeaters because many fast MI are not hackable. **Implication:** expand hacking only if opponents, mission, and your own TAG/VH/HI load justify it.
8. **Full elite link vs redundancy:** Tarik + Khawarij Core can be very quick and imposing; solo/duo attack plus Mukhtar/other missions/screening has safer redundancy. Actual **one-Haris** constraint forces a choice between Khawarij/Ramah, Mukhtar, and Janissary Haris.

### Best sources, ranked by actionability / transcript status

**MCP full transcripts retrieved and reviewed (English):**

1. **[Robert Shepherd — Infinity N5 Faction Focus: Ramah Taskforce](https://www.youtube.com/watch?v=dvSrZU73hxA)** — post-October 2025 update; **best for competitive caveats, affordable defense plans, practical sample lists and Tarik/Khawarij/Namurr/Mukhtar balance**. Reviews Haytham, Maggie, Shakush and TR bot + Monstrucker backbone; partially tournament-informed, but presenter explicitly isn't a Ramah specialist.
2. **[burlesford — Infinity N5 Casual Faction Focus: Ramah Taskforce](https://www.youtube.com/watch?v=qfq4388HAzM)** — **2025-08-24**, very long unit-by-unit talk by a faction devotee; Khawarij preferred over Mukhtar, Maggie vs Shakush criticism, 15-model list construction and Fireteams. **Pre-N5.2**.
3. **[Tactical Awareness S3 E32 — Ramah Taskforce](https://www.youtube.com/watch?v=p2omBWM-gr0)** / **[Spotify](https://open.spotify.com/episode/1kGCzFYxHHqttlwOCGylOG)** — **reissued 2025-11-07**; explicit contrasting competitive opinions and sample lists. Approx **15–30 min** Tarik/Khawarij; **35–45 min** Nahab/Mukhtar; **45–60 min** Al Fasid/Burkut/Hortlak/Maggie/Hidden Tuareg; **60–70 min** Haytham and overall verdict.
4. **[Robert Shepherd — Infinity Explained: Aerial Vehicles Analysis and Ranking](https://www.youtube.com/watch?v=N6TYjMgU4ZM)** — **post-October 2025**; best *specialized vehicle* source: explains S7/No Cover/hacking, Haytham's MSV1 anti-flyer niche, limited utility relative to top-ranked VHs. Transcript calls Haytham roughly **4th of 8** in a close middle cluster.
5. **[Robert Shepherd — Infinity N5 Faction Focus: Vanilla Haqqislam](https://www.youtube.com/watch?v=Dmv4pfdTbc0)** — **2025-11-23**; shared Maghariba, Shakush, Mukhtar, Haytham and inexpensive REM roles. **Only Ramah-listed units apply**.
6. **[Tactical Awareness S3 — Haqqislam Prime](https://open.spotify.com/episode/4gx0VBfits4q9PNwUiPIJh)** — selected MCP podcast transcript reviewed for Vanilla cross-faction unit context, not Ramah list legality.

**Historical/secondary, not current profiles:**

- **[Tactical Awareness S1 E09 — Ramah N4](https://open.spotify.com/episode/0oXM0IlM47mnpvpU4bHiX5)** — Feb 2023; MCP transcript retrieved, for faction evolution and themes, not legality.
- **[WIP12 E77 — Ramah Taskforce](https://open.spotify.com/episode/5cVqXajwSaWzGFwLtEpvzJ)** — Oct 2022; MCP transcript retrieved; long-form veteran commentary, but **N4-era**.
- **[Corvus Belli forum community resource index](https://forum.corvusbelli.com/threads/n5-recap-haqqislam-tacticas.43463/)** and **[Bureau Aegis Ramah N5 roundup](https://www.bureau-aegis.org/forum/index.php?topic=17828.0)** — directories for other older/different-language material, not claimed as transcript-reviewed here.

**Notes on transcript reliability:** YouTube and Spotify automated transcripts have frequent spelling errors (Khawarij, Maghariba, Haytham etc.) and sometimes speakers misremember stats. E.g. an older Robert narration refers to Khawarij BS12 while the pinned N5.3 Army reference gives **BS13**; only use its **tactical argument**, never transcribe the erroneous number as authoritative. Game-state/list examples and skills may postdate or predate N5.3: preserve the exact canonical reference above.

## Mission specialist choices — N5.3 cross-game evaluation

**Tuareg KHD28/0 / HD33/.5** is a premier WIP15 Hidden/forward scoring hacker if this current roster permits it; **Ghulam FO/Doctor** are cheap type coverage and **Mukhtar/Khāwarij** actual high-mobility specialists score laterally. Select the **actual Doctor/Engineer/FO** option printed here, not its combat counterpart. A superior Ramah fighting team doesn't compensate for losing the only button-runner before turn three.

See [Mission Specialists / Button Pushers apex and value tiers](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). This roster and its Fireteam chart are the final authority for exact options.

## N5.3 airborne / enemy-DZ profile and value choices (2026-10-23)

**Nahab Parachutist Specialist Operative31/0, KHD35/0, Red Fury38/1** enters a legal side edge without a roll, combines **NWI/Decoy(2)/Viral CC/CC23/Zapper** with scoring or backline attack. **Nahab Infiltration SO32/0, KHD36/0, Red Fury39/1** are separate pre-positioned choices; no Nahab profile grants both delivery types or Combat Jump. **Hakim WIP15 Doctor(+3) Parachutist** can arrive to rescue the forward group/score a Classified, but cannot enter from the enemy-DZ edge using ordinary Parachutist. **Tuareg Hidden/Infiltration** is a delayed midfield alternative. Don't expose the last scoring specialist chasing one cheap Order.

[Cross-game N5.3 airborne/rear-strike apex-value and landing-risk tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **Use this roster and canonical Fireteam chart for exact legality.**

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **Mukhtar Viral Rifle25/0 or MSV2 Red Fury34/1** supplies a fast Mimetism(-3)/NWI **non-TAG** shooter forward deployed near useful angles. **Tarik AP Spitfire49/1.5** trades points for 15-10/Super-Jump and armored midrange kills, best when a route is already prepared. **Khawarij MSV2 Mk12 38/0** is the unusual 0-SWC anti-Mimetism midrange alternate. **Maghariba MULTI HMG71–72/1.5** is the separate durable **TAG** for open long lanes and high ARM, but S8/hacking and Engineer costs are real. [Gunfighter value and dedicated TAG comparison](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## TAG tactical cross-reference (2026-10-23)

**Maghariba** is the strong S8 long-gun/board-control chassis: pick it on accessible open tables where BS14/ARM8 can demand multiple enemy solutions. **Shakush** is the leaner HMG Continuous Damage/AP Spitfire source when the Maghariba's huge footprint or extra points would cost Ramah its scoring/recovery engine. Check the Armored Assault Fireteam requirement and total partner cost.

For the two-tier **apex/points-value** comparison, TAG counterplay, matchup matrix and direct transcript sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Treat current profiles, points/SWC and canonical Fireteam data above as authoritative.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Valerya Gromoz 19/0.5 WIP14 HD + Total Control(+1B)/Pitcher** offers exceptional budget anti-TAG control; **Leila Sharif 22/0 KHD+Carbonite** kills hackers and disables ordinary hackable targets via explicit upgrade. **Tuareg KHD 28/0 WIP15/Firewall(-3)** is a hidden high-quality assassin/scorer rather than generic network; **Ghulam HD16/0.5** is budget ordinary HD, and **Mukhtar HD29/0.5** buys independent Forward Deployment/NWI mission reach. **Nahab KHD35–36/0** pays for dangerous Infiltration/Parachutist melee attacks more than pure WIP value. **Why:** Ramah has high-mobility specialists but should not spend 30+ points on hackers unless their *physical* objective/close-assault role is needed; don't import Vanilla-only Barid or Haytham.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

Cross-faction [apex and cost-value Order-generator rankings](../../notes/list-building/cheerleaders-and-order-generators.md), circumstance guide and transcript disagreements. **This file remains authoritative for profiles, AVA, Training and Fireteam legality.**

- 7pt Fanous — Regular Flash/Repeater REM with Mimetism; excellent cheap network but limited S3 concealment.
- 8pt Kameel — Baggage/Repeater/Deactivator and Regular Order, particularly valuable with disposable launchers.
- 11pt Ghulam — S2 protected Regular Order; FO/Doctor/deployable repeater profiles can earn their premium.
- Warcor — Irregular Flash Pulse ARO distraction, NOT a passive transferable Regular Order.
- Baggage — prioritize a legal 8pt basic bot if actually on roster, remembering its large base.

**When to pick:** Prefer transferable, safe Regular Orders when the Combat Group needs fuel; choose the higher-priced option only when its smoke, template, weapon, repeater, Fireteam function or scoring ability has a real job. Do not count Irregular/Impetuous/Tactical/Lieutenant Orders or Peripheral bodies as interchangeable Regular pool Orders; account for DZ footprint and link/enabler package costs.


## ARO apex/value cross-reference (2026-10-23)

[Best ARO units across N5.3 — absolute apex vs points-value](../../notes/list-building/aro-units-apex-and-value.md) compares hidden reactive fire, TR/Neurocinetics, Flash/DTW/expendable defenders and why competing creators disagree. The **roster here** is authoritative for actual costs, Training, AVA and Fireteam construction.

- **Fanous Flashbot** — cheap regular network and ARO tax, not a full-strength gun
- **Ghulam cheap template/FO** — small-base Regular guard plus a mission secondary job; don't expose a linked gun solely to win AROs
- **Warcor 3pt Flash** — disposable Irregular Stun/Orders tax, not a generic Regular cheerleader
- **Total Reaction support** — use recoverable remote for routine lanes, rather than expose primary active gun

**Best circumstance:** long exposed lanes justify a real sniper/missile/linked gun; dense tables, DZ landings and mission rooms favor E/M, mine, Shotgun, Riotstopper and hidden traps. Cover the destination/approach, layer serial threats rather than two pie-sliceable visible guns, and preserve scoring units for the active turn.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Rouhani21 (WIP18 Doctor)** is a remarkably effective 90%-base linked VITA recovery piece; **Ghulam Doctor15 (WIP17)** is 85% for six points less. **Hakim24/25 Doctor(+3)** is best when a casualty is on the flank; **29/25 options with Parachutist Nasmat A2** cover a remote zone. **Claire33** is **Doctor(2W)** *or* **Doctor(+3) FTO**, mutually exclusive profiles. **Najjarun15 + Nasmat3** handles Maghariba/Shakush STR separately. [Doctor/Engineer recovery odds and tier guide](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## Tactical cross-reference — vision control (23 October 2026)

**Ghulam NCO Smoke GL15/1** is low-points ordinary Smoke using spare LT Orders; **Khawarij CoC + Disco33/0**, **Hortlak Disco28/0 with Deactivator**, and **Claire Doctor(2W)+Disco33/0** create true Eclipse access while performing distinct command, tough-infantry, and recovery jobs. **Yara Haddad24/0 MSV2** can use *normal Smoke* for an asymmetric gunfight; she cannot shoot freely through Eclipse. **Disagreement to test:** when a mission needs only a single open crossing, simple Smoke can save points; when an MSV sniper locks it, a Disco user with scoring/recovery utility is worth the premium. [Global vision-control tier guide](../../notes/list-building/vision-control-units-apex-and-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Asawira** is not the default Ramah melee purchase: use **current roster-legal Khawarij/Tarik** as strong mobile *close-range* threats only once their shooting/superjump/route is productive. **Carmen Johns + Bâtard** brings two-body pressure, Smoke and melee/trade value where rostered, but cannot be ranked as a Hidden/Impersonating specialist. A Ramah assault against a dedicated MA5/NBW defender should usually **shoot or exploit a template angle**, not initiate a head-on CC duel. [CC assassin apex/value, Guard, anti-CC and evidence](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## N5.3 network projection — Pitchers, Repeaters, TinBots and disposable delivery

**Valerya Gromoz19/.5** is a cheap HD/Pitcher + Total Control upgrade **Wildcard** for usable ranged projection; **Rafiq13/0 FO/Sensor/native Repeater**, **Fanous7/0 Flash+Repeater (AVA3)** and **Kameel8/0 Baggage/Repeater** are the excellent Regular foundation. **Hunzakut FO+Deployable Repeater19/0** is **Irregular, AVA1** infiltrated corner placement, not a free Turn-0 Minelayer. **Ghulam13/0** carries a deployable node but places later. **Opposing case:** Ramah often needs 2–3 strong attacks/specialists instead of a stationary cyber castle; against mass non-Hackable troops, cheap Fanous/Rafiq utility is sufficient.

[Cross-game network apex/value, profiles, matchups and transcript disagreements](../../notes/list-building/network-projection-repeaters-pitchers-apex-value.md). Exact local roster and Fireteams remain authoritative.

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Ghulam12 Panzerfaust** and **Beasthunter9 Panzerfaust/HFT (15 Camo+FD)** give cheap lethal threat; **Burkut26 SMG+E/Marat(+1B)** is harder-to-ignore electronic denial and **Hortlak31 K1 Marksman** repeatable armor-ignorant shot. **Haytham29 HSG+Panzerfaust VH** attacks flanks but risks Aerial exposure; **Maghariba72 TAG E/M Carbine(+2B)** buys far more than anti-TAG utility. Count physical reach/return fire and time until opponent's Engineer. [Anti-TAG/HI apex/value and E/M recovery guide](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## Tactical cross-reference — indirect fire (2026-10-23)

**Split alternatives:** **Shaytaniyah16/1.5 Guided Missile** uses Valerya/Leila, Hunzakut/FO and Repeaters; **19/1.5 Missile(+1B) is NON-Guided in this pinned Ramah reference**. **Al Fasid50/1.5 HMG+GL+Smoke GL** and **Maghariba71/1.5 HMG+GL** can make speculative attacks if weapon/range support them, but are expensive full attackers, not purpose-bought B1 lobbers. **Ghulam NCO15/1 GL+Smoke** spends a relevant LT Order on other utility. [Cross-game indirect guide](../../notes/list-building/indirect-fire-speculative-guided-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Namurr Tactical Awareness Specialist41/0** is the **carry-and-survive value apex**: W2, Immunity(Enhanced), Climbing+, Terrain, BS(+1B), E/Marat, can move/objective/escape on own Order; **44/1 Spitfire is a separate cost**. **Mukhtar FO25/0/Doctor26/0** FD+10/Mimetism(-3)/NWI is lower-cost distributed holder. **Tarik AP Rifle+Tactical Awareness46/0** (BS/CC powerhouse, 2W/No ordinary Specialist printed) flips VP zones but doesn't automatically pick up a box. **Shakush56–58/1.5** 3STR and **Maghariba71–72/1.5** 360º/ARM8/Baggage are strong guards/swing, not guaranteed eligible carriers; pay Engineer/actual Specialist. **Al Fasid44/1.5 HRL/Minelayer/Sixth Sense** defends interaction space; not a box holder by default. **Counter:** expensive multi-HI can be isolated/hacked; a protected Mukhtar in cover plus 7pt Fanous may be better than a Namurr sent into open lane.

[Whole-game objective holding/zone apex/value, scenario scoring and opposing media](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Actual sectorial profiles and Fireteam chart remain authoritative.

## Force multipliers — N5.3 role/value cross-reference (2026-10-23)

**Kameel8 Baggage/Repeater** is low-cost logistics and Regular Order; **14/.5 EVO** improves legitimate active REM/CJ situations through supportware, *not ordinary Spotlight*. **Janissary TinBot Firewall** defends only a *legal* team while carrier functions; a solo Hacker/REM elsewhere is not protected. **Maghariba Baggage and other TAG tools** are potent as an offensive resource and reloader but don't make the TAG a cost-effective *dedicated* support purchase. [Full force-multiplier guide](../../notes/list-building/force-multipliers-special-abilities-apex-value.md).

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Rafiq FO/Sensor/Triangulated Fire13/0** cheaply reveals **Camo/Hidden** inside ZoC; **Carmen+Bâtard17/0** adds a fast Sensor route through synchronized Bâtard. **Yara Haddad MSV2 AP Marksman24/0** is inexpensive direct anti-Mimetism, **Mukhtar MSV2 Red Fury34/1** a mobile high-Burst cleaner, and **Khawarij MSV2 Mk12/NCO38/0** trades cost for durable movement/command utility. **Khawarij CoC+Disco33/0** or other exact Eclipse carriers bypass enemy MSV/Marksmanship instead of fighting it. **Tradeoff:** Rafiq can Discover many markers for 13pt, whereas paying 34pt Mukhtar to search rather than shoot often wastes its damage ceiling.

[Full anti-tech N5.3 apex/value, exact mechanics, matchup selection and opposing transcripts](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## N5.3 peripheral / synchronized / multi-body apex-value update

**Maghariba Guard71–72/1.5** (ARM8, Baggage, 360º) **Jandab Ancillary** and **Shakush56–58/1.5 Jandab** differ from true synchronized Auxbot: included ancillary *must be Placed* after deploying TAG and gives no pooled Regular Order; can affect **Armored Assault** Fireteam status. **Nasmat3pt** Servants let Doctor Mukhtar26 or another eligible Doctor/Engineer repair/heal through far bot without spending many movement Orders, but no extra attacks/Orders, and one patient per Order. **Best decision:** need **2 simultaneous fighting positions now** → ordinary second Regular HI; need **late Specialist footprint without exposing TAG driver** → place Jandab; need **cheap rescue coverage** → Nasmat. **Opposing:** reliable repair/resupply network beats throwing Jandab forward Turn 1 solely as expendable body.

[Cross-game multi-body apex/value and transcript disputes](../../notes/list-building/peripheral-synchronized-multibody-apex-value.md). Current sectorial roster and N5.3 rules decide actual type and access.
