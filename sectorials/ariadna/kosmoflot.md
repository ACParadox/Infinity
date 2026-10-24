---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 306
sectorial_slug: kosmoflot
sectorial_name: Kosmoflot
parent_faction: Ariadna
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "36 standard logical units; optional Intel Spec-Ops and Ariadna Team-Ops hooks; complete standard Fireteam chart; linked L'Équipe Argent reinforcement Fireteam chart"
---

# Kosmoflot

This file is the repository-native factual reference for **Kosmoflot (Army ID 306)** under the N5.3 baseline. It records the standard roster, profiles/loadouts, AVA, points/SWC, Fireteam legality, optional game-mode hooks, and the linked **L'Équipe Argent (Army ID 399)** Reinforcement Fireteam chart.

The structured Army source is pinned to revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `d4329bb596ffea5d568eb2435f74366c305a7630`. InfinityDB commit `4e2662be3f43387fbae42b3790a711b3e98570c4` is the normalized identity/reference baseline. Parenthetical Fireteam comments are preserved as `Counts as` labels. Structured `required: true` rows are treated as a required-choice set rather than as an instruction that every marked troop type must be present simultaneously.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Kosmoflot |
| Parent faction | Ariadna |
| Army ID | 306 |
| Rules baseline | N5.3 |
| Main roster units | 36 logical units |
| Optional game-mode units | Ariadna Team-Ops; Intel Spec-Ops |
| Linked Reinforcement roster | L'Équipe Argent, Army ID 399 |
| Fireteam chart | yes |

InfinityDB's current identity summary describes Kosmoflot as an expeditionary Ariadnan force mixing veterans from several nations with mobile assault units, close-combat threats, and flexible support.

## Fireteam chart limits and sectorial-level restrictions

| Constraint | Value / wording |
|---|---|
| Core | up to 1 |
| Haris | up to 1 |
| Duo | source sentinel `256`; treated as unrestricted by the sectorial chart, subject to normal Fireteam rules |
| Standard Fireteam rows | Rokots; Kosmoflot; Kosmosoldats; Chernobog; Varangian Guard |
| Wildcards | Volkolak; Patcher; Strannik; The Unknown Ranger; Cadin “FirstStrike” Donn |
| Main/Reinforcement mixing | No source-defined mixing exception; keep the charts separate |
| Required-choice semantics | In the Kosmoflot Fireteam row, `SCOT GUARD FTO` and `FRONTOVIK` are both source-marked `required: true`; this is normalized as a required-choice set: at least one qualifying member from that set is required |
| Scot Guard restriction | Only loadouts explicitly named `SCOT GUARD FTO` qualify for the Kosmoflot Fireteam row; non-FTO loadouts 8 and 9 do not |

## Unit roster index

| Unit ID | Unit | AVA | Troop type | Classification | Regularity | Notes |
|---:|---|---:|---|---|---|---|
| 1518 | Rokots | 5 | LI | Line Troops | Regular | Rokot Fireteam anchor |
| 243 | Kazak Doktor | 2 | LI | Support Troops | Regular | Doctor; Rokot Fireteam access |
| 257 | Traktor Mul Unit | 2 | REM | Support Troops | Regular | Baggage / Guided support |
| 1152 | Pavel Aleksei McMannus | 1 | SK | Character | Regular | — |
| 1582 | Mekhaniks, Flight Engineers Corps | 2 | LI | Specialist Trained Troops | Regular | Engineer; counts as Rokot in FT-01 |
| 1136 | Frontoviks, Separate Assault Battalion | 5 | LI | Veteran Troops | Regular | Access to FT-01, FT-02 and FT-03 |
| 1461 | Varangian Guard | 4 | WB | Mercenary Troops | Regular + Impetuous | FT-05 anchor |
| 1284 | 112, Emergency Service (Motorized) | 1 | LI | Support Troops | Regular | Doctor; Motorcycle |
| 228 | Para-Commandos | 3 | LI | Specialist Trained Troops | Regular | — |
| 1522 | Polaris Team | 2 teams | mixed | compound | Regular | Masha + Bearpode; same Combat Group |
| 777 | The Unknown Ranger | 1 | MI | Character | Regular | Wildcard; Tactical Awareness |
| 258 | Equipe Mirage-5 | 1 team | mixed | Character | mixed | Margot + Duroc compound team |
| 50 | Warcors, War Correspondents | 1 | LI | Mercenary Troops | Irregular | Journalist |
| 240 | Irmandinhos | 4 | WB | Line Troops | Irregular + Impetuous | Engineer |
| 255 | 112, Emergency Service | 2 | LI | Support Troops | Regular | Loadout is named FTO but no standard Kosmoflot FT row grants access |
| 1843 | Kibervolk Patrol | 2 teams | mixed | compound | Regular | Kibervolk + Dozer KVP; same Combat Group |
| 1555 | Wolfgang Amadeus Wolff | 1 | WB | Character | Regular | FT-01 and FT-05 |
| 1940 | Ioann Bann, Varangian Dog-Warrior | 1 | WB | Character | Irregular + Impetuous | FT-05; counts as Varangian |
| 1584 | Chernobog Armored Detachment | 2 | TAG | Mechanized Troops | Regular + Tactical Awareness | FT-04 Duo |
| 1585 | Patchers, Structural Response Team | 2 | HI | Specialist Trained Troops | Regular | Wildcard; counts as Rokot |
| 1749 | Denma Connolly | 1 | WB | Character | Regular + Impetuous | FT-05; counts as Varangian |
| 259 | William Wallace | 1 | WB | Character | Regular | FT-05; counts as Varangian |
| 237 | 1st Highlanders S.A.S. | 3 | SK | Specialist Trained Troops | Regular | — |
| 265 | Wardrivers, Mercenary Hackers | 1 | LI | Mercenary Troops | Regular | FT-01 |
| 263 | Uxía McNeill | 1 | SK | Character | Regular | — |
| 1520 | Volkolak Assault Troopers | 3 | HI | Elite Troops | Regular | Wildcard |
| 1847 | Mekhamobilya Support Pilots | 1 | LI | Support Troops | Regular | FT-01; Chernobog pilot support |
| 261 | The Scots Guards, 6th Caledonian Infantry Regiment | 5 | MI | Specialist Trained Troops | Regular | Only FTO loadouts enter FT-02 |
| 1525 | Cadin “FirstStrike” Donn | 1 | WB | Character | Regular | Wildcard |
| 1581 | Remontnikbot V-5 Elektronik | 2 | REM | Support / Peripheral | no independent order | Peripheral (Servant) |
| 1588 | Raveneye Officers | 1 | LI | Support Troops | Regular | Forward Observer / Minelayer |
| 1519 | Zenit-7 Detachment | 2 | LI | Elite Troops | Regular | Camouflage / Decoy |
| 1583 | Strannik Outer Patrol | 2 | MI | Specialist Trained Troops | Regular | Wildcard |
| 256 | Dozers, Field Engineers | 1 | LI | Support Troops | Regular | Engineer |
| 248 | Highlander Caterans | 2 | LI | Specialist Trained Troops | Irregular | Camouflage (1 Use) |
| 1521 | Armata-4 Proyekt “Kosmosoldat” | 2 | HI | Headquarters Troops | Regular | FT-03 anchor |

### Optional game-mode entries

| Unit ID | Unit | Coverage | Fireteam relevance |
|---:|---|---|---|
| 1929 | Ariadna Team-Ops | Team-Ops game mode | none in the standard chart |
| 1915 | Intel Spec-Ops | Spec-Ops game mode | may join FT-01 Rokots, max 1; source comment `Spec-Ops` |

Soldier-of-Fortune catalogue records exposed with no Kosmoflot faction membership are not part of this standard roster.

## Unit details

### Rokots

**Unit ID:** 1518  
**Slug:** `rokots`  
**AVA:** 5  
**Troop type:** LI  
**Classification:** Line Troops

#### Base profile

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 10 | 11 | 13 | 1 | 0 | 1 | 2 |

**Skills:** Courage.

#### Loadouts

| Profile ID | FTO | SWC | Points | Weapons / equipment | Skills / flags |
|---:|---|---:|---:|---|---|
| 1 | — | 0 | 8 | Chain Rifle, Light Shotgun, Pistol, CCW | — |
| 4 | — | 0 | 9 | SMG, Grenades, D-Charges, Pistol, CCW | — |
| 6 | — | 0 | 10 | SMG, Grenades, Flash Pulse, D-Charges, Pistol, CCW | Forward Observer |
| 7 | — | 0 | 11 | SMG, Grenades, Pistol, CCW; MediKit | Paramedic |
| 8 | — | 0 | 12 | Rifle, Light Shotgun, Pistol, CCW | Infiltration; Camouflage (1 Use) |
| 9 | — | 0 | 10 | SMG, Grenades, D-Charges, Pistol, CCW | Infiltration; Camouflage (1 Use) |
| 10 | — | 0 | 9 | SMG, Grenades, D-Charges, Pistol, CCW | Lieutenant |
| 13 | — | 0 | 11 | SMG, Grenades, Pistol, CCW | Commlink (+2); Specialist Operative |

### Kazak Doktor

**Unit ID:** 243  
**Slug:** `kazak-doktor`  
**AVA:** 2  
**Troop type:** LI  
**Classification:** Support Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 11 | 11 | 13 | 1 | 0 | 1 | 2 |

**Skills/equipment:** Doctor; MediKit.

| Profile ID | SWC | Points | Weapons | Flags |
|---:|---:|---:|---|---|
| 1 | 0 | 12 | Rifle, Pistol, CCW | — |

### Traktor Mul Unit

**Unit ID:** 257  
**Slug:** `traktor-mul`  
**AVA:** 2  
**Troop type:** REM  
**Classification:** Support Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 13 | 10 | 9 | 12 | 2 | 0 | 1 STR | 4 |

**Skills/equipment:** Remote Presence; Courage; Baggage; ECM: Guided (-6).

| Profile ID | SWC | Points | Weapons / equipment | Skills |
|---:|---:|---:|---|---|
| 1 | 0 | 5 | PARA CCW (-3); Deactivator | — |
| 2 | 1 | 9 | Katyusha MRL, PARA CCW (-3) | BS Attack (Guided) |
| 3 | 1 | 14 | Uragan MRL, PARA CCW (-3) | BS Attack (Guided); Total Reaction |

### Pavel Aleksei McMannus

**Unit ID:** 1152  
**Slug:** `pavel-aleksei-mcmannus`  
**AVA:** 1  
**Troop type:** SK  
**Classification:** Character

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 23 | 12 | 12 | 13 | 1 | 0 | 1 | 2 |

**Skills:** Martial Arts L3; Surprise Attack (-3); Camouflage; Courage; Forward Deployment (+20); Mimetism (-3); Terrain (Total); Specialist Operative; Stealth; Frenzy; Berserk; Immunity (Shock).

| Profile ID | SWC | Points | Weapons |
|---:|---:|---:|---|
| 1 | 0 | 33 | Ohotnik, D-Charges, Shock Mine, Boarding Pistol, AP+T2 CCW |

### Mekhaniks, Flight Engineers Corps

**Unit ID:** 1582  
**Slug:** `mekhaniks-flight-engineers-corps`  
**AVA:** 2  
**Troop type:** LI  
**Classification:** Specialist Trained Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 15 | 11 | 11 | 13 | 2 | 0 | 1 | 2 |

**Skills/equipment:** Engineer; Terrain (Zero-G); Deactivator; GizmoKit.

| Profile ID | SWC | Points | Weapons / equipment | Differences |
|---:|---:|---:|---|---|
| 1 | 0 | 20 | Rifle, D-Charges, Panzerfaust, Armed Turret (Adhesive Launcher Rifle), AP Heavy Pistol, CCW | — |
| 2 | 0 | 19 | Boarding Shotgun, D-Charges, Heavy Pistol, PARA Mine, CCW | BS Attack (T2) |
| 3 | 0 | 17 | SMG, D-Charges, E/M Mine, AP Heavy Pistol, CCW | Minelayer |

### Frontoviks, Separate Assault Battalion

**Unit ID:** 1136  
**Slug:** `frontoviks-separate-assault-bat`  
**AVA:** 5  
**Troop type:** LI  
**Classification:** Veteran Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 17 | 12 | 11 | 13 | 2 | 0 | 1 | 2 |

**Skills:** Courage; Mimetism (-3); Warhorse.

| Profile ID | SWC | Points | Weapons / equipment | Differences |
|---:|---:|---:|---|---|
| 1 | 0 | 21 | T2 Rifle, Assault Pistol, CCW | — |
| 2 | 1 | 30 | AP Spitfire, Assault Pistol, CCW | — |
| 3 | 1.5 | 19 | Heavy Rocket Launcher, Assault Pistol, CCW | — |
| 6 | 0 | 26 | T2 Rifle, Panzerfaust, D-Charges, Assault Pistol, CCW; Deactivator | Engineer |
| 7 | 0 | 23 | T2 Rifle, Assault Pistol, CCW; MediKit | Paramedic |
| 8 | 0.5 | 28 | AP Sniper Rifle, Assault Pistol, CCW | MSV1 |
| 9 | 0 | 21 | T2 Rifle, Assault Pistol, CCW | Lieutenant |

### Varangian Guard

**Unit ID:** 1461  
**Slug:** `varangian-guard`  
**AVA:** 4  
**Troop type:** WB  
**Classification:** Mercenary Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 23 | 10 | 14 | 13 | 2 | 0 | 1 | 2 |

**Skills:** Berserk (+3); Impetuous; No Cover; Dogged; Religious Troop. **Orders:** Regular + Impetuous.

| Profile ID | SWC | Points | Weapons |
|---:|---:|---:|---|
| 1 | 0 | 10 | Chain Rifle, Heavy Pistol, AP CCW, Grenades, Smoke Grenades |
| 3 | 0 | 13 | Boarding Shotgun, Smoke Grenades, Heavy Pistol, AP CCW |
| 4 | 0 | 12 | SMG, Chain Rifle, Smoke Grenades, Heavy Pistol, AP CCW |
| 5 | 0 | 13 | SMG, Chain-colt (+1B), Smoke Grenades, Heavy Pistol, AP CCW |
| 6 | 0 | 13 | SMG, Chain Rifle, Smoke Grenades, Heavy Pistol, Trench-Hammer, AP CCW |

### 112, Emergency Service (Motorized)

**Unit ID:** 1284  
**Slug:** `112-emergency-service-motorized`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Support Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 20-10 | 16 | 11 | 12 | 13 | 0 | 0 | 1 | 4 |

**Skills/equipment:** Doctor; Courage; Mimetism (-3); Limited Cover; MediKit; Motorcycle.

| Profile ID | SWC | Points | Weapons |
|---:|---:|---:|---|
| 4761 | 0 | 19 | Light Shotgun, Smoke Grenade Launcher, Smoke Grenades, Boarding Pistol, CCW |

### Para-Commandos

**Unit ID:** 228  
**Slug:** `para-commandos`  
**AVA:** 3  
**Troop type:** LI  
**Classification:** Specialist Trained Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 16 | 12 | 11 | 14 | 2 | 3 | 1 | 2 |

**Skills:** Mimetism (-3); Parachutist; Terrain (Zero-G).

| Profile ID | SWC | Points | Weapons / equipment | Differences |
|---:|---:|---:|---|---|
| 1 | 0 | 18 | Rifle, Boarding Pistol, CCW | — |
| 4 | 1 | 29 | AP Spitfire, Boarding Pistol, CCW | — |
| 6 | 0 | 21 | Boarding Shotgun, Flash Pulse, D-Charges, Boarding Pistol, CCW | BS Attack (+1SD); Forward Observer |
| 8 | 0 | 19 | SMG, D-Charges, Boarding Pistol, CCW; MediKit | Paramedic |

### Polaris Team

**Unit ID:** 1522  
**Slug:** `polaris-team`  
**AVA:** 2 teams  
**Classification:** compound team

A Polaris Team is composed of **1 Polaris Bearpode and 1 Masha**. Both must belong to the same Combat Group.

#### Masha

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 11 | 11 | 13 | 2 | 0 | 1 | 2 |

Masha component: **9 points**, Light Shotgun, Pistol, CCW.

#### Polaris Bearpode

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-10 | 24 | 5 | 16 | 12 | 4 | 3 | 2 | 6 |

**Skills:** Courage; Dogged; Climbing Plus; Immunity (ARM); No Cover; Frenzy; Berserk (+3); Dodge (+5).

| Team option | SWC | Points | Bearpode weapons | Orders |
|---|---:|---:|---|---|
| POLARIS TEAM ALPHA | 0 | 32 | Chain Rifle (+1B), Trench-Hammer, AP CCW, Grenades, Smoke Grenades | 2 Regular |
| POLARIS TEAM BETA | 0 | 40 | Heavy Shotgun, Chain-colt, Smoke Grenades, Trench-Hammer, AP CCW; Bearpode BS 11 | 2 Regular |

### The Unknown Ranger

**Unit ID:** 777  
**Slug:** `the-unknown-ranger`  
**AVA:** 1  
**Troop type:** MI  
**Classification:** Character

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-5 | 23 | 13 | 12 | 13 | 4 | 0 | 1 | 2 |

**Skills:** Martial Arts L1; Courage; Dodge (+2.5); Natural Born Warrior; Immunity (Shock); Mimetism (-3); Specialist Operative; Tactical Awareness; Stealth; NWI.

| Profile ID | SWC | Points | Weapons | Orders |
|---:|---:|---:|---|---|
| 1 | 0 | 39 | Mk12, Chain-colt, Heavy Pistol, T2 CCW | Regular + Tactical |
| 2 | 1 | 42 | AP Spitfire, Chain-colt, Heavy Pistol, T2 CCW | Regular + Tactical |

### Equipe Mirage-5

**Unit ID:** 258  
**Slug:** `equipe-mirage-5`  
**AVA:** 1 team  
**Classification:** Character compound team

#### Lieutenant Margot Berthier

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 16 | 14 | 12 | 13 | 3 | 3 | 1 | 2 |

**Skills:** BS Attack (Shock); Immunity (Shock); Terrain (Total); Parachutist (Deployment Zone); Mimetism (-3); Specialist Operative; Immunity (IMM-B); Combat Instinct; Tactical Awareness; Dodge (+1SD); MediKit (PH=14).

Margot component: **36 points**, AP Rifle, Grenade Launcher, Light Shotgun, D-Charges, Pistol, CCW; Regular + Tactical Awareness.

#### Sergent Duroc

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-10 | 23 | 10 | 16 | 13 | 3 | 3 | 2 | 6 |

**Skills:** Martial Arts L2; Courage; Dodge (+2.5); Parachutist (Deployment Zone); Super-Jump; Impetuous; Immunity (ARM); No Cover.

Duroc component: **24 points**, Chain Rifle (+1B), Grenades, Smoke Grenades, AP CCW; Irregular + Impetuous.

| Team option | SWC | Points | Orders |
|---|---:|---:|---|
| EQUIPE MIRAGE-5 (Margot & Duroc) | 2 | 60 | 1 Regular, 1 Irregular, 1 Tactical Awareness, 1 Impetuous |

### Warcors, War Correspondents

**Unit ID:** 50  
**Slug:** `warcors`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Mercenary Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 11 | 9 | 11 | 13 | 0 | 0 | 1 | 2 |

**Skills:** Journalist. **Order:** Irregular.

| Profile ID | SWC | Points | Weapons | Difference |
|---:|---:|---:|---|---|
| 1 | 0 | 3 | Flash Pulse, Stun Pistol, PARA CCW (-3) | 360º Visor |
| 2 | 0 | 3 | Flash Pulse, Stun Pistol, PARA CCW (-3) | Sixth Sense |

### Irmandinhos

**Unit ID:** 240  
**Slug:** `irmandinhos`  
**AVA:** 4  
**Troop type:** WB  
**Classification:** Line Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 21 | 10 | 14 | 13 | 1 | 0 | 1 | 2 |

**Skills/equipment:** Booty; Engineer; Impetuous; No Cover; Deactivator. **Orders:** Irregular + Impetuous.

| Profile ID | SWC | Points | Weapons |
|---:|---:|---:|---|
| 2 | 0 | 8 | Chain Rifle, D-Charges, Smoke Grenades, Pistol, AP CCW |
| 3 | 0 | 14 | Boarding Shotgun, D-Charges, Smoke Grenades, Pistol, AP CCW |

### 112, Emergency Service

**Unit ID:** 255  
**Slug:** `112-emergency-service`  
**AVA:** 2  
**Troop type:** LI  
**Classification:** Support Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 16 | 11 | 12 | 13 | 0 | 0 | 1 | 2 |

**Skills/equipment:** Doctor; Courage; MediKit.

| Profile ID | FTO | SWC | Points | Weapons |
|---:|---|---:|---:|---|
| 1 | `112 FTO` | 0 | 11 | Light Shotgun, Boarding Pistol, CCW |

The loadout name contains `FTO`, but the pinned standard Kosmoflot Fireteam chart contains no row granting this unit Fireteam access.

### Kibervolk Patrol

**Unit ID:** 1843  
**Slug:** `kibervolk-patrol`  
**AVA:** 2 teams  
**Classification:** compound team

A Kibervolk Patrol is composed of **1 Kibervolk and 1 Dozer KVP**. Both must belong to the same Combat Group.

#### Dozer KVP

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 11 | 11 | 13 | 1 | 0 | 1 | 2 |

**Skills/equipment:** Courage; Engineer; Deactivator; GizmoKit.

| Profile ID | SWC | Points | Weapons / equipment |
|---:|---:|---:|---|
| 1 | 0 | 11 | Light Shotgun, D-Charges, Pistol, CCW |
| 2 | 0 | 14 | Light Shotgun, D-Charges, Armed Turret (Rifle), Pistol, CCW |
| 3 | 0 | 12 | SMG, D-Charges, Pistol, CCW |

#### Kibervolk

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-15 | 21 | 2 | 15 | 13 | 1 | 0 | 1 STR | 5 |

**Skills/equipment:** Biometric Visor; CC Attack (+1B); Courage; Dodge (+5); Mimetism (-3); Sensor; Dogged.

| Profile ID | SWC | Points | Weapons |
|---:|---:|---:|---|
| 1 | 0 | 10 | Chain-colt, Trench-Hammer, Shock CCW |
| 2 | 0 | 12 | Chest Mine, CrazyKoala, Trench-Hammer, Shock CCW |

### Wolfgang Amadeus Wolff

**Unit ID:** 1555  
**Slug:** `wolfgang-amadeus-wolff`  
**AVA:** 1  
**Troop type:** WB  
**Classification:** Character

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-5 | 22 | 12 | 14 | 13 | 3 | 3 | 2 | 2 |

**Skills:** Martial Arts L3; BS Attack (Continuous Damage); Berserk (+3); Courage; Dodge (+5); Dodge (+3); Immunity (ARM); Climbing Plus; Terrain (Zero-G); Frenzy; Discover (+6).

| Profile ID | SWC | Points | Weapons |
|---:|---:|---:|---|
| 1 | 0 | 33 | MULTI Rifle (+1SD), Chain-colt, E/M Grenades (+1SD), Heavy Pistol, PARA CCW (-6), DA CCW |

### Ioann Bann, Varangian Dog-Warrior

**Unit ID:** 1940  
**Slug:** `ioann-bann-varangian-dog-warrior`  
**AVA:** 1  
**Troop type:** WB  
**Classification:** Character

#### Dogface

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-10 | 22 | 11 | 14 | 13 | 2 | 3 | 3 | 2 |

#### Dog-Warrior

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-10 | 23 | 11 | 16 | 13 | 4 | 6 | 3 | 6 |

**Skills:** Martial Arts L3; BS Attack (-3); Berserk; Dodge (+5); Immunity (ARM); No Cover; Super-Jump; Religious Troop; Impetuous; Dogface has Transmutation (1). **Order:** Irregular.

| Profile ID | SWC | Points | Weapons |
|---:|---:|---:|---|
| 1 | 0 | 32 | Chain Rifle (+1B), Viral Tactical Bow (+1SD), Smoke Grenades, AP Heavy Pistol (+1B), AP+T2 CCW |

### Chernobog Armored Detachment

**Unit ID:** 1584  
**Slug:** `chernobog-armored-detachment`  
**AVA:** 2  
**Troop type:** TAG  
**Classification:** Mechanized Troops

#### Full-power state

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-10 | 17 | 14 | 16 | 13 | 8 | 6 | 3 STR | 7 |

**Skills/equipment:** ECM: Guided (-6); Courage; Dodge (PH=9); Tactical Awareness; GizmoKit (PH=9); BS Attack (SR-1); Transmutation (2).

#### Battle-ravaged state

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-5 | 15 | 13 | 15 | 13 | 6 | 3 | 3 STR | 7 |

**Skills/equipment:** ECM: Guided (-3); BS Attack (SR-1); Courage; Dodge (PH=9); Tactical Awareness; GizmoKit (PH=9).

| Profile ID | SWC | Points | Weapons | Peripheral |
|---:|---:|---:|---|---|
| 1 | 1.5 | 70 | AP HMG, Heavy Rocket Launcher (+1B), Chest Mine, AP CCW | Samodelkin |
| 2 | 1.5 | 63 | AP HMG, Heavy Flamethrower, Chest Mine, AP CCW | Samodelkin |

**Samodelkin:** MOV 15-10, CC —, BS —, PH 10, WIP 12, ARM 0, BTS 0, W 1, S 1; Courage, Specialist Operative, Mimetism (-3), Peripheral (Ancillary).

### Patchers, Structural Response Team

**Unit ID:** 1585  
**Slug:** `patchers-structural-response-team`  
**AVA:** 2  
**Troop type:** HI  
**Classification:** Specialist Trained Troops

#### Full state

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 16 | 12 | 11 | 13 | 3 | 3 | 2 | 2 |

**Skills:** Courage; Dodge (+2.5); Immunity (Continuous Damage); Immunity (Shock); Specialist Operative; Terrain (Total); Transmutation (1); Climbing Plus.

#### Battle-ravaged state

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 15 | 12 | 10 | 13 | 2 | 0 | 2 | 2 |

**Skills:** Courage; Immunity (Continuous Damage); Immunity (Shock); Specialist Operative; Terrain (Total); Climbing Plus.

| Profile ID | SWC | Points | Weapons |
|---:|---:|---:|---|
| 1 | 0 | 24 | Vulkan Shotgun (+1B), Akrylat-Kanone, AP Heavy Pistol, AP CCW |
| 2 | 0 | 18 | Heavy Flamethrower (+1B), Adhesive Launcher Rifle, Grenades (Continuous Damage), AP Heavy Pistol, AP CCW |

### Denma Connolly

**Unit ID:** 1749  
**Slug:** `denma-connolly`  
**AVA:** 1  
**Troop type:** WB  
**Classification:** Character

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-5 | 23 | 11 | 14 | 12 | 1 | 3 | 1 | 2 |

**Skills:** Martial Arts L1; Berserk; Courage; Dodge (+5); Natural Born Warrior; MetaChemistry (ReRoll); No Cover; Impetuous. **Orders:** Regular + Impetuous.

| Profile ID | SWC | Points | Weapons |
|---:|---:|---:|---|
| 1 | 0 | 12 | Chain Rifle (+1B), Smoke Grenades, Heavy Pistol (+1B), AP+DA CCW |

### William Wallace

**Unit ID:** 259  
**Slug:** `william-wallace`  
**AVA:** 1  
**Troop type:** WB  
**Classification:** Character

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-10 | 24 | 13 | 14 | 15 | 3 | 0 | 2 | 2 |

**Skills:** CC Attack (-3); Berserk (+3); Courage; Dodge (+5); Natural Born Warrior; Immunity (Critical); Inspiring Leadership; Frenzy; Number 2; CC Attack (+1B).

| Profile ID | SWC | Points | Weapons | Difference |
|---:|---:|---:|---|---|
| 1 | 0 | 38 | T2 Rifle, Light Shotgun, Smoke Grenades, Boarding Pistol (+1B), EXP CCW | Chain of Command (Non Specialist) |
| 2 | 0 | 38 | same | Lieutenant |

### 1st Highlanders S.A.S.

**Unit ID:** 237  
**Slug:** `1st-highlanders-sas`  
**AVA:** 3  
**Troop type:** SK  
**Classification:** Specialist Trained Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 22 | 11 | 13 | 13 | 0 | 0 | 1 | 2 |

**Skills:** Martial Arts L2; Surprise Attack (-3); Camouflage; Courage; Dodge (+2.5); Infiltration; Mimetism (-3); Terrain (Total); Stealth.

| Profile ID | SWC | Points | Weapons | Difference |
|---:|---:|---:|---|---|
| 1 | 0 | 20 | Chain Rifle, Light Shotgun, D-Charges, Silenced Pistol, AP+Shock CCW | — |
| 2 | 0 | 20 | Chain Rifle, Grenades, D-Charges, Assault Pistol, AP+Shock CCW | — |
| 4 | 0 | 21 | Chain Rifle, Light Shotgun, Flash Pulse, D-Charges, Silenced Pistol, AP+Shock CCW | Forward Observer |
| 5 | 0 | 25 | Boarding Shotgun (+1B), D-Charges, E/M Mine, Silenced Pistol, AP+Shock CCW | Specialist Operative |
| 6 | 0.5 | 22 | Chain Rifle, Light Shotgun, D-Charges, AP Mine, Silenced Pistol, AP+Shock CCW | Minelayer |

### Wardrivers, Mercenary Hackers

**Unit ID:** 265  
**Slug:** `wardrivers-mercenary-hackers`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Mercenary Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 13 | 11 | 10 | 13 | 0 | 3 | 1 | 2 |

**Skills:** Sixth Sense; Hacker. **Hacking Device:** UPGRADE: Zero Pain.

| Profile ID | SWC | Points | Weapons / equipment |
|---:|---:|---:|---|
| 1 | 1 | 14 | Boarding Shotgun, Flash Pulse, Cybermine, Pistol, CCW; Hacking Device |
| 2 | 1 | 16 | same plus Disco Baller |

### Uxía McNeill

**Unit ID:** 263  
**Slug:** `uxia-mcneill`  
**AVA:** 1  
**Troop type:** SK  
**Classification:** Character

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 22 | 11 | 13 | 13 | 0 | 0 | 1 | 2 |

**Equipment:** MSV1. **Skills:** Martial Arts L2; Surprise Attack (-3); Courage; Camouflage; Dodge (+5); Mimetism (-3); Stealth; Terrain (Total); Frenzy; Infiltration (PH=19); BS Attack (+1B); Specialist Operative.

| Profile ID | SWC | Points | Weapons |
|---:|---:|---:|---|
| 1 | 0 | 25 | Boarding Shotgun, Grenades, Smoke Grenades, Boarding Pistol, AP+Shock CCW |
| 2 | 0 | 25 | Boarding Shotgun, D-Charges, Smoke Grenades, Assault Pistol, AP+Shock CCW |

### Volkolak Assault Troopers

**Unit ID:** 1520  
**Slug:** `volkolak-assault-troopers`  
**AVA:** 3  
**Troop type:** HI  
**Classification:** Elite Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-5 | 22 | 12 | 14 | 12 | 4 | 6 | 1 | 2 |

**Skills:** Courage; Natural Born Warrior; Immunity (ARM); NWI; Super-Jump; CC Attack (+1B); Dodge (-3); Dodge (+5); Immunity (IMM-B).

| Profile ID | SWC | Points | Weapons / equipment | Difference |
|---:|---:|---:|---|---|
| 1 | 1 | 38 | HMG, Chain-colt (+1B), Drop Bears (+1B), Heavy Pistol, AP+DA CCW | — |
| 2 | 1.5 | 35 | Missile Launcher, Chain-colt (+1B), Drop Bears (+1B), Heavy Pistol, AP+DA CCW | — |
| 3 | 0 | 31 | T2 Rifle, Chain-colt (+1B), Drop Bears (+1B), Heavy Pistol, AP+DA CCW | BS Attack (AP) |
| 4 | 0 | 33 | same; MediKit | BS Attack (AP); Paramedic |

### Mekhamobilya Support Pilots

**Unit ID:** 1847  
**Slug:** `mekhamobilya-support-pilots`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Support Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 11 | 11 | 13 | 1 | 0 | 1 | 2 |

**Skills:** Courage; Specialist Operative; TAGCom (Dodge PH+1, GizmoKit PH+1).

| Profile ID | FTO / name | SWC | Points | Weapons / equipment |
|---:|---|---:|---:|---|
| 1 | CHERNOBOG PILOT | 0 | 9 | SMG, D-Charges, Pistol, CCW; GizmoKit |

### The Scots Guards, 6th Caledonian Infantry Regiment

**Unit ID:** 261  
**Slug:** `the-scots-guards`  
**AVA:** 5  
**Troop type:** MI  
**Classification:** Specialist Trained Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 16 | 12 | 12 | 13 | 3 | 0 | 1 | 2 |

Loadout-specific skills/equipment are preserved below; **only rows named `SCOT GUARD FTO` qualify for FT-02**.

| Profile ID | FTO | SWC | Points | Weapons / equipment | Skills / differences |
|---:|---|---:|---:|---|---|
| 1 | yes | 1.5 | 31 | AP Spitfire, Pistol, CCW, Flash Pulse, D-Charges | source FTO profile |
| 2 | yes | 1.5 | 31 | Missile Launcher, Assault Pistol, CCW, Flash Pulse, D-Charges | source FTO profile |
| 3 | yes | 0 | 26 | T2 Marksman Rifle, Flash Pulse, Pistol, CCW, D-Charges | source FTO profile |
| 4 | yes | 0 | 22 | AP SMG (+1B), Panzerfaust, Flash Pulse, D-Charges, Pistol, CCW | source FTO profile |
| 8 | no | 1 | 32 | Heavy Rocket Launcher, Flash Pulse, D-Charges, Assault Pistol, CCW | Surprise Attack (-3); Camouflage; Forward Deployment (+10) |
| 9 | no | 0 | 32 | AP SMG (+1B), Panzerfaust, Flash Pulse, D-Charges, Pistol, CCW | Surprise Attack (-3); Camouflage; Forward Deployment (+10) |
| 10 | yes | 0 | 23 | AP SMG (+1B), Panzerfaust, Flash Pulse, D-Charges, Pistol, CCW; MediKit | Paramedic |
| 11 | yes | 1.5 | 26 | Heavy Rocket Launcher, Flash Pulse, D-Charges, Assault Pistol, CCW | MSV1 |

### Cadin “FirstStrike” Donn

**Unit ID:** 1525  
**Slug:** `cadin-firststrike-donn`  
**AVA:** 1  
**Troop type:** WB  
**Classification:** Character

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-5 | 23 | 12 | 14 | 13 | 3 | 3 | 2 | 2 |

**Skills:** Frenzy; Courage; Dodge (+5); Climbing Plus; CC Attack (+1B); Martial Arts L1; Berserk (+6); Natural Born Warrior.

| Profile ID | SWC | Points | Weapons |
|---:|---:|---:|---|
| 1 | 0 | 30 | T2 Boarding Shotgun, Flammenspeer, E/M Grenades (+1B), Boarding Pistol, AP+T2 CCW |

### Remontnikbot V-5 Elektronik

**Unit ID:** 1581  
**Slug:** `remontnikbot-v-5-elektronik`  
**AVA:** 2  
**Troop type:** REM  
**Classification:** Support / Peripheral

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 10 | 8 | 9 | 12 | 0 | 0 | 1 STR | 1 |

**Skills:** Courage; Mimetism (-3); Peripheral (Servant).

| Profile ID | SWC | Points | Weapons | Orders |
|---:|---:|---:|---|---|
| 1 | 0 | 2 | PARA CCW (-3) | no independent order |

### Raveneye Officers

**Unit ID:** 1588  
**Slug:** `raveneye-officers`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Support Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 15 | 11 | 10 | 13 | 1 | 3 | 1 | 2 |

**Skills/equipment:** Immunity (Shock); Minelayer; Forward Observer; Deactivator.

| Profile ID | SWC | Points | Weapons |
|---:|---:|---:|---|
| 1 | 0 | 12 | SMG, E/Marat, Flash Pulse, E/M Mine, Pistol, CCW |
| 2 | 0 | 12 | SMG, E/Marat, Flash Pulse, Cybermine, Pistol, CCW |

### Zenit-7 Detachment

**Unit ID:** 1519  
**Slug:** `zenit-7-detachment`  
**AVA:** 2  
**Troop type:** LI  
**Classification:** Elite Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 12 | 10 | 13 | 2 | 0 | 1 | 2 |

**Skills:** Surprise Attack (-3); BS Attack (Shock); Camouflage; Mimetism (-3); Decoy (1); Stealth; BS Attack (SR-1).

| Profile ID | SWC | Points | Weapons | Difference |
|---:|---:|---:|---|---|
| 2 | 0.5 | 25 | AP Marksman Rifle, Pistol, CCW | — |
| 3 | 0.5 | 30 | AP Marksman Rifle, Pistol, CCW | Chain of Command |
| 4 | 1 | 27 | AP Sniper Rifle, Light Shotgun, Pistol, CCW | Forward Observer |

### Strannik Outer Patrol

**Unit ID:** 1583  
**Slug:** `strannik-outer-patrol`  
**AVA:** 2  
**Troop type:** MI  
**Classification:** Specialist Trained Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 18 | 12 | 11 | 13 | 3 | 3 | 1 | 2 |

**Skills:** Terrain (Zero-G).

| Profile ID | SWC | Points | Weapons / equipment | Difference |
|---:|---:|---:|---|---|
| 1 | 0 | 18 | T2 Boarding Shotgun, Flash Pulse, D-Charges, Boarding Pistol, PARA CCW (-3) | Specialist Operative |
| 2 | 0 | 16 | SMG, Flash Pulse, Adhesive Launcher Rifle, D-Charges, Boarding Pistol, PARA CCW (-3) | Specialist Operative |
| 3 | 0 | 18 | SMG, Flash Pulse, Light Riotstopper, Boarding Pistol, PARA CCW (-3); MediKit | Doctor |

### Dozers, Field Engineers

**Unit ID:** 256  
**Slug:** `dozers-field-engineers`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Support Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 11 | 11 | 13 | 1 | 0 | 1 | 2 |

**Skills/equipment:** Courage; Engineer; Deactivator; GizmoKit.

| Profile ID | SWC | Points | Weapons / equipment |
|---:|---:|---:|---|
| 1 | 0 | 13 | Rifle, D-Charges, Pistol, CCW |
| 3 | 0 | 14 | Rifle, Blitzen, D-Charges, Pistol, CCW |
| 4 | 0 | 14 | Rifle, D-Charges, Pistol, CCW; Deployable Cover |
| 5 | 0 | 15 | Rifle, D-Charges, Armed Turret (Rifle), Pistol, CCW |

### Highlander Caterans

**Unit ID:** 248  
**Slug:** `highlander-caterans`  
**AVA:** 2  
**Troop type:** LI  
**Classification:** Specialist Trained Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 22 | 12 | 13 | 12 | 0 | 0 | 1 | 2 |

**Skills:** Surprise Attack (-3); Camouflage (1 Use); Mimetism (-3); Stealth; Climbing Plus. **Order:** Irregular.

| Profile ID | SWC | Points | Weapons | Difference |
|---:|---:|---:|---|---|
| 1 | 1 | 21 | T2 Sniper Rifle, Pistol, AP CCW | — |
| 2 | 0.5 | 21 | AP Sniper Rifle, Pistol, AP CCW | — |
| 3 | 1 | 23 | T2 Sniper Rifle, Pistol, AP CCW | Forward Deployment (+10) |

### Armata-4 Proyekt “Kosmosoldat”

**Unit ID:** 1521  
**Slug:** `armata-4-proyekt-kosmosoldat`  
**AVA:** 2  
**Troop type:** HI  
**Classification:** Headquarters Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 16 | 13 | 12 | 13 | 6 | 3 | 1 | 2 |

**Equipment:** MSV1. **Skills:** Courage; Immunity (Shock); NWI; Terrain (Zero-G); Warhorse; BS Attack (-3).

| Profile ID | SWC | Points | Weapons / equipment | Difference |
|---:|---:|---:|---|---|
| 1 | 1.5 | 44 | AP HMG, AP Heavy Pistol, CCW, Chain Rifle | — |
| 2 | 0 | 36 | T2 Rifle (+1B), Heavy Flamethrower, Panzerfaust, AP Heavy Pistol, CCW; MediKit | Paramedic |
| 3 | 1.5 | 44 | Portable Autocannon, Chain Rifle, AP Heavy Pistol, CCW | — |
| 4 | 1.5 | 44 | same | Lieutenant |
| 5 | 1 | 48 | same | Lieutenant (+1 Order) |

## Fireteams

The canonical rows below are authoritative for standard Kosmoflot Fireteam access. The reverse index that follows is derivative.

### FT-01 — Rokots Fireteams

**Types:** Core, Haris  
**Wildcard team:** no  
**Observation:** at least one Rokot is required by the source minimum.

| Member | Unit ID | Required | Min | Max | Counts as | FTO restriction | Allowed loadout IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Rokots | 1518 | no | 1 | 5 | — | — | all | anchor |
| Mekhaniks | 1582 | no | 0 | 2 | Rokot | — | all | source comment `(Rokot)` |
| Frontoviks | 1136 | no | 0 | 1 | Rokots | — | all | source comment `(Rokots)` |
| Mekhamobilya Support Pilots | 1847 | no | 0 | 1 | — | — | all | — |
| Kazak Doktor | 243 | no | 0 | 1 | — | — | all | — |
| Wardrivers | 265 | no | 0 | 1 | — | — | all | — |
| Wolfgang Amadeus Wolff | 1555 | no | 0 | 1 | — | — | all | — |
| Intel Spec-Ops | 1915 | no | 0 | 1 | — | Spec-Ops mode | mode-defined | optional game-mode row; source comment `Spec-Ops` |

### FT-02 — Kosmoflot Fireteams

**Types:** Core, Haris, Duo  
**Wildcard team:** no  
**Observation:** the two source rows are both marked `required: true`; normalize them as a required-choice set. At least one qualifying `SCOT GUARD FTO` or Frontovik is required. A source `required` flag does not mean both troop types must simultaneously be present.

| Member | Unit ID | Required | Min | Max | Counts as | FTO restriction | Allowed loadout IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Scot Guard FTO | 261 | required-choice | 0 | 5 | — | **FTO only** | 1, 2, 3, 4, 10, 11 | non-FTO 8 and 9 excluded |
| Frontoviks | 1136 | required-choice | 0 | 5 | — | — | all | — |

### FT-03 — Kosmosoldats Fireteams

**Types:** Haris, Duo  
**Wildcard team:** no

| Member | Unit ID | Required | Min | Max | Counts as | FTO restriction | Allowed loadout IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Kosmosoldat | 1521 | no | 1 | 2 | — | — | all | anchor |
| Frontoviks | 1136 | no | 0 | 1 | — | — | all | — |

### FT-04 — Chernobog Fireteams

**Types:** Duo  
**Wildcard team:** no

| Member | Unit ID | Required | Min | Max | Counts as | FTO restriction | Allowed loadout IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Chernobog | 1584 | no | 1 | 2 | — | — | all | anchor |

### FT-05 — Varangian Guard Fireteams

**Types:** Core, Haris, Duo  
**Wildcard team:** no

| Member | Unit ID | Required | Min | Max | Counts as | FTO restriction | Allowed loadout IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Varangian Guard | 1461 | no | 1 | 4 | — | — | all | anchor |
| William Wallace | 259 | no | 0 | 1 | Varangian | — | all | source comment `(Varangian)` |
| Denma Connolly | 1749 | no | 0 | 1 | Varangian | — | all | source comment `(Varangian)` |
| Wolfgang Amadeus Wolff | 1555 | no | 0 | 1 | Varangian | — | all | source comment `(Varangian)` |
| Ioann Bann | 1940 | no | 0 | 1 | Varangian | — | all | source comment `(Varangian)` |

### Wildcards

| Unit | Unit ID | Max | Counts as | FTO/profile restriction | Notes |
|---|---:|---:|---|---|---|
| Volkolak Assault Troopers | 1520 | 3 | — | all | Wildcard |
| Patchers | 1585 | 2 | Rokot | all | source comment `(Rokot)` |
| Strannik Outer Patrol | 1583 | 2 | — | all | Wildcard |
| The Unknown Ranger | 777 | 1 | — | all | Wildcard |
| Cadin “FirstStrike” Donn | 1525 | 1 | — | all | Wildcard |

Wildcards may join otherwise eligible standard Fireteams, but they do not waive each team's anchor, minimum, required-choice, profile-gating, or maximum-member restrictions.

## Unit → Fireteam access index

| Unit | Fireteam | Type | Access | Counts as | Profile restriction | Min/Max | Notes |
|---|---|---|---|---|---|---|---|
| Rokots | FT-01 Rokots | Core/Haris | native | — | all | 1–5 | anchor |
| Mekhaniks | FT-01 Rokots | Core/Haris | counts-as | Rokot | all | 0–2 | — |
| Frontoviks | FT-01 Rokots | Core/Haris | counts-as | Rokots | all | 0–1 | — |
| Frontoviks | FT-02 Kosmoflot | Core/Haris/Duo | required | — | all | 0–5 | member of required-choice set |
| Frontoviks | FT-03 Kosmosoldats | Haris/Duo | native | — | all | 0–1 | — |
| Mekhamobilya Support Pilots | FT-01 Rokots | Core/Haris | native | — | all | 0–1 | — |
| Kazak Doktor | FT-01 Rokots | Core/Haris | native | — | all | 0–1 | — |
| Wardrivers | FT-01 Rokots | Core/Haris | native | — | all | 0–1 | — |
| Wolfgang Amadeus Wolff | FT-01 Rokots | Core/Haris | native | — | all | 0–1 | — |
| Wolfgang Amadeus Wolff | FT-05 Varangian | Core/Haris/Duo | counts-as | Varangian | all | 0–1 | — |
| Intel Spec-Ops | FT-01 Rokots | Core/Haris | special | — | Spec-Ops mode | 0–1 | optional game-mode only |
| Scots Guards | FT-02 Kosmoflot | Core/Haris/Duo | required | — | FTO IDs 1,2,3,4,10,11 only | 0–5 | member of required-choice set |
| Kosmosoldat | FT-03 Kosmosoldats | Haris/Duo | native | — | all | 1–2 | anchor |
| Chernobog | FT-04 Chernobog | Duo | native | — | all | 1–2 | anchor |
| Varangian Guard | FT-05 Varangian | Core/Haris/Duo | native | — | all | 1–4 | anchor |
| William Wallace | FT-05 Varangian | Core/Haris/Duo | counts-as | Varangian | all | 0–1 | — |
| Denma Connolly | FT-05 Varangian | Core/Haris/Duo | counts-as | Varangian | all | 0–1 | — |
| Ioann Bann | FT-05 Varangian | Core/Haris/Duo | counts-as | Varangian | all | 0–1 | — |
| Volkolak | all eligible standard teams | varies | wildcard | — | all | max 3 | subject to team formation requirements |
| Patchers | all eligible standard teams | varies | wildcard | Rokot | all | max 2 | subject to team formation requirements |
| Strannik | all eligible standard teams | varies | wildcard | — | all | max 2 | subject to team formation requirements |
| The Unknown Ranger | all eligible standard teams | varies | wildcard | — | all | max 1 | subject to team formation requirements |
| Cadin “FirstStrike” Donn | all eligible standard teams | varies | wildcard | — | all | max 1 | subject to team formation requirements |

All standard roster units not listed in this reverse index have no Fireteam access in the pinned standard Kosmoflot chart.

## Reinforcement Fireteams — L'Équipe Argent

Linked Reinforcement army: **L'Équipe Argent (Army ID 399)**, source revision `7.26246.158`.

These rows are intentionally separate from the standard Kosmoflot chart. Reinforcement Fireteam limits in the pinned source are **Core 1; Haris 1; Duo 1**. The Reinforcement source contains 12 logical units: Reinf. Chasseurs, Reinf. 112 Emergency Service, Reinf. Para-Commandos, Reinf. Brigadier Jacques Bruant, Reinf. Equipe Mirage-5, Reinf. Wardrivers, Reinf. Beasthunters, Reinf. Briscards, Reinf. Moblots, Reinf. Wolfgang Amadeus Wolff, Reinf. Loup-Garous, and Reinf. Apaches.

### RFT-01 — Loup-Garou Reinforcement Fireteams

**Types:** Core, Haris, Duo

| Member | Unit ID | Required | Min | Max | Counts as | Profile restriction | Notes |
|---|---:|---|---:|---:|---|---|---|
| Loup-Garou REINF | 1626 | no | 1 | 5 | — | all | anchor |

### RFT-02 — Briscards Reinforcement Fireteams

**Types:** Core, Haris, Duo

| Member | Unit ID | Required | Min | Max | Counts as | Profile restriction | Notes |
|---|---:|---|---:|---:|---|---|---|
| Briscard REINF | 1627 | no | 1 | 4 | — | all | anchor |

### Reinforcement Wildcards

| Unit | Unit ID | Max | Counts as | Profile restriction | Notes |
|---|---:|---:|---|---|---|
| Moblot REINF | 1630 | 2 | — | all | Reinforcement Wildcard |
| Apache REINF | 1629 | 2 | Loup-Garou | all | source comment `(Loup-Garou)` |
| 112 FTO REINF | 1633 | 1 | — | FTO loadout | Reinforcement Wildcard |
| Brigadier Bruant REINF | 1637 | 1 | Briscards | all | source comment `(Briscards)` |
| Wolfgang Amadeus REINF | 1634 | 1 | Loup-Garou, Briscards | all | source comment `(Loup-Garou, Briscards)` |

### Reinforcement reverse index

| Unit | Fireteam | Access | Counts as | Max | Notes |
|---|---|---|---|---:|---|
| Loup-Garou REINF | RFT-01 | native | — | 5 | min 1 anchor |
| Briscard REINF | RFT-02 | native | — | 4 | min 1 anchor |
| Moblot REINF | all eligible Reinforcement teams | wildcard | — | 2 | — |
| Apache REINF | all eligible Reinforcement teams | wildcard | Loup-Garou | 2 | — |
| 112 FTO REINF | all eligible Reinforcement teams | wildcard | — | 1 | FTO profile only |
| Brigadier Bruant REINF | all eligible Reinforcement teams | wildcard | Briscards | 1 | — |
| Wolfgang Amadeus REINF | all eligible Reinforcement teams | wildcard | Loup-Garou, Briscards | 1 | — |

No Main/Reinforcement mixing is inferred from sharing a character or unit concept. Use the Reinforcement chart only for the linked Reinforcement group.


## Expanded faction tactical guide

The [expanded Kosmoflot tactical/list-building guide](../../notes/factions/kosmoflot.md) preserves alternative video-derived archetypes, Mirage-5/Smoke combinations, Rokot/Patcher/Chernobog and defensive Patrol choices. Its reconciliation flags **Scots Guard FTO without NCO**, **already-Regular Varangian/Denma Orders**, and the **bundled Kibervolk + Dozer KVP Patrol**. The current roster and Fireteam chart above remain authoritative.

## Community tactical field guide — N5 transcript synthesis (2026-10-19)

> **Opinion/analysis, not Army data.** The profile, point, SWC, AVA, Fireteam and rules facts **above** remain authoritative under the pinned N5.3 source. The analyses below come from recorded community discussions, chiefly January–July 2025 N5, and tournament retrospectives from N4. Verify any exact older rules/list suggestions against the current reference; do not copy podcast Army codes as current legal N5.3 lists. Speaker disagreements are retained.

### Fast evaluation

- **Identity:** an aggressive, flexible Ariadnan force built around cheap Rokot orders, unusually broad smoke/close-assault tools, infiltration, airborne flank attacks, and a few substantial long-range guns. Its price-efficient *breadth* lets it threaten several routes at once; it does not automatically win direct face-to-face shooting.
- **Main weaknesses:** defensive ARO depth, scarce elite BS/visual mods, inconsistent Fireteam bonuses, limited hacking, and too many expensive *effectively ~1.5-Wound* gunfighters. An opponent can win by controlling approach lanes, layering repeaters against the TAG/HI, and trading for the few mission specialists.
- **Practical principle:** first budget reliable button pushers, then one long-range problem-solver, one midfield attack, and one flank/close-assault plan. Several 2025 lists stacked bears, TAGs and Mirage-5 but had too little specialist coverage; the opponent need only protect objectives rather than kill everything.

### Useful list-building blocks — with reasons

| Job | Candidate / package | Why it works; constraint |
|---|---|---|
| Orders and cheap protection | **Rokots** (8–11 pt profiles); optionally a Lieutenant decoy | Low-cost **Regular** bodies fund the expensive assault pieces; chain rifles/grenades punish close attackers. BS10 and low resilience make a large Rokot team an order battery, not a guaranteed killer. |
| Flexible Core/Haris | **Rokots + Patcher + Frontovik / specialist** | Patcher is a **Wildcard that counts as Rokot**; two durable specialist bodies, templates and Frontovik AP/ARO weapons create a cheap, multi-role link. Check exact N5.3 composition and purity rules; a 2025 roundtable even caught an illegal list during discussion. |
| Defensive gun | **Frontovik HRL/AP sniper**, **Volkolak ML**, **Cateran T2 sniper** | Reach and threatening ammo make opponents spend orders or avoid lanes. Cateran is Irregular and only one-Wound; Volkolak/Frontovik cannot withstand repeated unfavorable face-to-face engagements. |
| Mobile gun / specialist | **Unknown Ranger** or **Kosmosoldat Portable Autocannon/AP HMG** | Ranger adds a specialist and Tactical Awareness to a strong midrange weapon; Kosmosoldat has MSV1, ARM6 and powerful ammo. The Kosmosoldat is still **1W + NWI**, vulnerable to hacking, and gains few free effective wounds for its cost. |
| Close assault and smoke | **Varangians, Denma, Irmandinhos, Wolfgang, Cadin** | Cheap smoke/templates and dangerous CC profiles trade up into much dearer models. Irmandinho is also an Engineer; Wolfgang is formidable but positioning-dependent, while melee approaches consume orders and invite sacrificial trades. |
| Midfield objectives | **S.A.S., Uxía, Pavel**, infiltrating Rokots | Camo/infiltration creates mission pressure without walking through long firing lanes. Keep at least one specialist alive rather than turning every midfield piece into a disposable ARO. |
| Airborne enemy-DZ threat | **Mirage-5 (Margot + Duroc)**; cheaper **Para-Commando** | Deployment-zone parachutists change how opponents deploy; Duroc delivers large-template/CC pressure while **Margot is a Specialist Operative**. At 60 pts/2 SWC, Mirage-5 is a major commitment, so budget sufficient orders and mission coverage. |
| Sensor + deployable DZ defenses | **Kibervolk + Dozer KVP** patrol | Kibervolk's fast Sensor, Mimetism, close combat and optional CrazyKoala combine with Dozer Engineer and optional rifle turret to screen camo and airborne lanes. Buying both members is compulsory; it is a **compound patrol, not a REM Fireteam**. |
| Specialist access on the move | **Motorized 112**, **Patchers**, **Raveneye** | The 19-pt motorcycle Doctor brings fast smoke and healing; Patchers bring resilient specialists; Raveneye provides FO + E/M/Cybermine protection. Motorized 112 is **LI on a motorcycle, not a standalone VH**. |

### Where experienced commentators disagree

| Decision | Case for | Counterargument / how to choose |
|---|---|---|
| **Chernobog mandatory?** | *Counterintelligence* describes BS14/AP HMG, ARM8, Tactical Awareness and ranged reach as nearly essential for dealing with hard opposing targets. | *Ryan4043* calls it viable but optional; specialists, Varangians, Patchers and other attacks can give more redundancy. Take a TAG when the table/missions need sustained ranged armor-piercing fire; otherwise buy multiple independent jobs. |
| **Chernobog: HRL 70 vs HFT 63?** | *Counterintelligence* prefers the extra **Heavy Rocket Launcher (+1B)** for active anti-armor/anti-group options and a stronger ranged ARO; a cheaper AP HMG still has burst to win active fights. | *Yellow Snake/GloriousEND* favors the 63-pt **Heavy Flamethrower**: saves seven points and improves close-range self-protection. *Tactical Awareness* hosts questioned the HRL's marginal value when the AP HMG already solves many shots, while acknowledging templates/longer-range ARO. Decide based on whether enemy approach or ranged ARO is the greater problem. |
| **Double Chernobog?** | *Tactical Awareness* deliberately builds two TAGs, using cheap orders and a surprise Mirage-5 to overload target priority; legally Chernobog can Duo with another Chernobog. | Roughly **126–140 points** in two vulnerable-to-hacking big bases severely restricts specialists, board control and recovery. A niche skew, not the default all-comers template. |
| **Polaris Alpha vs Beta?** | **Alpha 32 pts** has cheaper chain-rifle auto-hit leverage and more points for other roles. | **Beta 40 pts** adds a Heavy Shotgun and reliable smoke utility (PH16 throw), but must shoot rather than relying on the same direct-template pressure. Both cost two Regular order-generating members; smoke reliability versus trading price drives the choice. |
| **Fireteam focus?** | *Tactical Awareness* likes budget Rokot/Patcher/Frontovik Core/Haris combinations, special weapons and specialists while Mirage/bear attacks. | *Ryan4043* argues N5 purity and link restrictions make a “full” competitive fireteam expensive and less efficient than it looks: Volkolak's Wildcard doesn't count as Rokot for purity, and a Kosmosoldat Haris/Duo needs expensive partners. Use a team to **perform a role**, not simply to maximize headcount. |
| **S.A.S. as ARO roadblock?** | *Counterintelligence* identifies camouflaged infiltrator templates as one of few available midfield speed bumps. | The same discussion warns trading a ~21-point objective-capable S.A.S. for one intruder can lose the mission. Favor active midfield tasks except on kill-focused missions or when other specialists remain. |
| **How strong is Kosmoflot overall?** | *Tactical Awareness* and older *WIP12* tournament guests demonstrate high-order aggressive and unusual builds; cheap redundancy and multiple deployment angles can win games. | *Ryan4043* and some 2026 community players rate it below stronger sectorials/TAK: unreliable head-to-head gunfights, low-cost defense that folds to competent opponents, and premium units less durable than comparable heavy infantry. These are **opinions and meta-dependent**, not verified win-rate claims. |

### TAG, vehicle, REM and support architecture

- **TAG — Chernobog (AVA 2):** current N5.3 **63-pt AP HMG + Heavy Flamethrower** or **70-pt AP HMG + Heavy Rocket Launcher (+1B)**, both 1.5 SWC, chest mine, **Tactical Awareness**, ancillary Samodelkin specialist, and an available **Chernobog Duo**. BS14/ARM8 is a rare Kosmoflot long-range answer. **Transmutation (2)** reduces BS14→13, ARM8→6 and BTS6→3 after damage; **Dodge PH=9** and low repair PH make reactive escape/recovery unreliable. Prefer lane-clearing from cover and avoid exposing it to hostile repeater webs without first removing the hacker/relay. Bring a suitable Engineer or accept that lost structure may not be recoverable. A 9-pt **Mekhamobilya** pilot/support specialist exists but is not automatically worth its cost; the Samodelkin already adds a mission-capable ancillary. **Older spoken claims that the TAG is unhackable or a brokenly efficient TAG are not rules evidence.**
- **REM — Traktor Mul (AVA 2):** **5-pt Regular Baggage + Deactivator** is an outstanding order/area-support purchase; Baggage can restock eligible Disposable assets and helps order economy. **9-pt/1 SWC Katyusha** is a cheap **Guided** indirect-pressure option only if the list provides spotting/targeting and orders; do not overpay in orders for BS10 speculative guesses. **14-pt/1 SWC Uragan** has **Total Reaction + Guided** in the *current reference*, giving inexpensive ranged deterrence, but BS10 and S4 exposure are poor against dedicated gunfighters. *Counterintelligence/Yellow Snake* often prefer the cheap baggage order or other defenses over committing to a shaky artillery plan. **Disagreement check:** Yellow Snake's 2025 translated commentary describes an Uragan without Guided, **contrary to the current N5.3 profile above**—follow current data.
- **REM — Remontnikbot (AVA 2):** **2-pt Peripheral (Servant)** for an eligible Doctor/Engineer: extends repair/heal reach without exposing the controller, screens narrow approaches at low cost, and **generates no Regular order of its own**. In a Chernobog list, plan an Engineer's path in advance; a bot alone does not repair. A 2025 Yellow Snake speaker likes it as nearly free physical screening, while questioning how often the TAG will be worth risky repair.
- **Vehicle / motorcycle:** no separate **VH-classified troop** appears in this pinned **Kosmoflot** main roster. **Motorized 112** is a **19-pt LI Doctor with motorcycle, Mimetism (-3), smoke grenades/launcher and 20–10 MOV**. Its job is speedy healing, smoking an approach, and late objective play; its S4 base and weak direct firepower mean it is not a tank. *Tactical Awareness TAK/Vanilla Ariadna* compares faster/more specialized **Dynamo bikes** favorably, but those are **not** automatically Kosmoflot-legal.
- **Adjacent “robotic” pieces:** **Kibervolk Patrol is a two-member compound team**, not a REM; the **Chernobog Samodelkin is Ancillary**, and the **Mekhamobilya is an LI pilot**, not another TAG/vehicle. This distinction prevents imaginary order pools or Fireteam access.
- **Shared Ariadna research:** *Tactical Awareness: Vanilla Ariadna SOUP* explicitly discusses **Traktor Mul Katyusha Guided with Chasseur FO**, 5-pt Baggage deactivation/reload utility, and Chernobog Duo ideas; **Chasseur and TAK Dynamo synergies may not be imported into Kosmoflot** unless they are on its roster. *Tactical Awareness: TAK* independently praises the **5-pt Traktor** as a cost-efficient Regular Baggage order and gives motorcycle benchmarks.

### Starting shells (roles, not imported Army codes)

1. **Balanced pressure:** Rokot orders + Patcher/Frontovik flexible link, an S.A.S./Uxía mission specialist, a Varangian/Irmandinho smoke piece, plus **one of** Mirage-5 / Bearpode / Chernobog. Why: leaves enough points for scoring even when the first attacker dies.
2. **TAG anchor:** Chernobog + Engineer/optional Remontnikbot + 5-pt Traktor Baggage + midfield camo + smoke/short-range trade piece. Why: AP HMG breaks problem AROs while cheaper troops keep objectives live; avoid overinvesting in an exposed repair train.
3. **No-TAG saturation:** Mirage-5 + Polaris and/or Varangians + Raveneye/Kibervolk DZ traps + multiple S.A.S./Rokot specialists. Why: diverse angles deny easy counterdeployment, but the opponent can exploit any shortfall in long-range guns or orders.

### Reviewed video and podcast transcripts (recommended order)

*Video transcript retrieval: connected YouTube tool. Podcast transcripts: connected podcast tool when available. Automated captions/translations can mishear unit names and N5 terminology; source dates matter.*

1. **[Tactical Awareness S3 Ep10 — Kosmoflot / Zeroes & Heroes (Feb 2025)](https://www.youtube.com/watch?v=ceoF3KoyaaM)** — best *three different N5 lists*: double TAG skew, dual Kosmosoldat + Kibervolk/Katyusha support, and inexpensive links. **[Podcast episode](https://open.spotify.com/episode/0FZYrBdbYi3bNLX0Xbdl3l)**; *both YouTube and podcast transcripts checked*.
2. **[Counterintelligence — N5 Kosmoflot faction review (2025)](https://www.youtube.com/watch?v=gE1L8HWH9Fo)** — most detailed *unit-by-unit tactical discussion* for Chernobog/HRL tradeoffs, defenses, Dozer turrets, SAS and specialists; *YouTube transcript checked*.
3. **[Ryan4043 — N5 Kosmoflot, the Good and the Bad (2025)](https://www.youtube.com/watch?v=Gmgn-eLs5vM)** — best counterweight to optimistic reviews: why warbands/cheap troops work yet premium 1W+NWI models, defensive depth and Fireteam purity disappoint; *YouTube transcript checked*.
4. **[Ryan4043 — N5 Kosmoflot purchase guide (2025)](https://www.youtube.com/watch?v=zcKP8lay4IE)** — explains basic Rokot/SAS/smoke priorities vs optional Chernobog/Patcher/REM choices; *YouTube transcript checked*. Ignore mini prices as time-sensitive.
5. **[Yellow Snake / GloriousEND — full Kosmoflot N5 deep dive (June 2025, Russian)](https://www.youtube.com/watch?v=PGpQtInE9lg)** — excellent *explicit platform chapters*: **Chernobog 57:36**, **motorized 112 1:15:55**, **Kibervolk 1:21:52**, **Remontnikbot 1:53:11**, **Traktor Mul 1:54:21**. *Auto-translated YouTube transcript checked; Russian Spotify podcast transcript unavailable*. Notable dissent: prefers the **63-pt flamer Chernobog**, views cheap Traktor as best, and questions REM artillery return on investment.
6. **[Tactical Awareness — Ariadna SOUP / Vanilla, S3 Ep11 (2025)](https://www.youtube.com/watch?v=2QSbZQ8uJIU)** — shared **Traktor Mul** Baggage and Guided ideas, plus limitations of Chernobog Duo; *YouTube transcript checked*. Vanilla-only elements are NOT Kosmoflot options.
7. **[Tactical Awareness — Tartary Army Corps, S3 Ep08 (2025)](https://www.youtube.com/watch?v=YidfyTObBtA)** — shared **5-pt Traktor** economy and contrast with TAK-specific Dynamo motorcycles; *YouTube transcript checked*.
8. **[WIP12 E107 — Kosmoflot revisited, IGL Satellite (May 2023)](https://open.spotify.com/episode/5qfUlS9HoTzjFsIOYhCO46)** and **[E108 — Cyber Baltic Kosmoflot (May 2023)](https://open.spotify.com/episode/3BTDdz6P9kufbuMOEt0QgC)** — *podcast transcripts checked*: tournament use of cheap orders, bears, Chernobog and specialist coverage. These are **N4 history**, not evidence of present N5 mechanics.
9. **[MetaChemistry Ep35 — Faction Takedown Kosmoflot (Mar 2022)](https://open.spotify.com/episode/7zTXaqMfq4n8Gu3eHW94Dc)** — *podcast transcript checked*, useful specifically for what enemies can anticipate and counter, but N4 and superseded for profiles/rules.

## Provenance

- Corvus Belli Army-derived source revision: `7.26246.158`
- Army data changed on: 2026-09-03
- Kosmoflot source snapshot: `massayoshi/infinity-army-backup` commit `d4329bb596ffea5d568eb2435f74366c305a7630`, `n5/kosmoflot/7.26246.158.json` (blob `3776f6c7423966aff6d5024d1f47f200fa702b91`)
- L'Équipe Argent source snapshot: same repository/commit, `n5/l-equipe-argent/7.26246.158.json` (blob `b1b074b4037c52461e836b365cda75f9c5805f7c`)
- InfinityDB commit: `4e2662be3f43387fbae42b3790a711b3e98570c4`
- Rules baseline: N5.3
- Generated/verified: 2026-10-15

### Validation

1. All 36 standard logical roster units have a detailed entry.
2. Optional Team-Ops and Spec-Ops entries are separated from the ordinary roster.
3. Points/SWC and listed profile distinctions are transcribed from the pinned structured source.
4. All five standard Fireteam rows are represented.
5. Source minimum/maximum values, `required` flags, parenthetical `Counts as` labels, and Wildcard maxima are preserved.
6. Scot Guard FT-02 access is explicitly profile-gated to FTO IDs 1, 2, 3, 4, 10, and 11; non-FTO IDs 8 and 9 are excluded.
7. The Unit → Fireteam reverse index is derived from the canonical rows above.
8. The linked L'Équipe Argent Reinforcement chart is kept separate and includes both canonical Reinforcement rows and all five Reinforcement Wildcards.
9. Main and Reinforcement charts are not merged.
10. No unresolved source ambiguity remains that would require `status: partial` under `REFERENCE_DESIGN.md`.

## Command-unit apex/value cross-reference (2026-10-23)

**Wallace LT 38/0** makes genuinely Irregular **Irmandinhos** and other eligible models Regular while adding a free special Coordinated Order; **Varangians and Denma are already Regular**, so are not extra conversions. **Wallace CoC 38/0** offers durable smoke/CC succession as a non-LT choice; **Zenit-7 CoC 30/0.5** is a different role. **Kosmosoldat LT(+1) 48/1** may spend its own Orders but pinned **Scots Guard FTO does NOT have NCO**. Count actual available pooled Orders rather than a fictional LT→Scots Guard engine.

See [cross-game Lieutenant, Chain of Command and Order-package tiers](../../notes/list-building/command-units-apex-and-value.md). **Use this roster/Fireteam chart above for exact legality.**

## Mission specialist / button-pusher choices (N5.3)

Mission plan should preserve a **dedicated specialist among Irmandinho/Kibervolk Patrol/Rokot/Dynamo/Zenit** legal profiles rather than assuming Wallace attack pieces automatically push buttons. **Kibervolk Patrol includes one bundled Dozer KVP**; Engineer support is not two independently optional purchases. **Wallace LT** can regularize eligible *Irregular* models, but Varangians/Denma were already Regular. **Zenit CoC30/.5** is succession/scoring when mission recognizes CoC, not an all-purpose FO/Doctor. Late scoring still needs an intact Order route.

[Cross-game apex and value specialist tier guide](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). The unit profiles/Fireteams above control exact legality.

## Airborne / enemy-DZ attack profile choices (2026-10-23)

**Mirage-5 Margot+Duroc60/2** is the high-ceiling DZ-intrusion package: **both Parachutist(DZ)**, Margot BS14 AP Rifle/GL and personal TA/Specialist, Duroc 2W chain(+1B), Smoke/Super-Jump. The compound supplies **one Regular, one Irregular, one Tactical Awareness and one Impetuous token**, not two freely pooled Orders. It earns 60pts only if both bodies have jobs and opponent lacks covered side/rear edges. **Wallace LT38 Inspiring** supports eligible Irregulars from *on-table*, not an airborne LT. **Wallace CoC** is separate option; original pinned Scots Guard FTO has no NCO.

[Cross-game N5.3 airborne and DZ-attack apex/value tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **Pinned profiles and the canonical Fireteam chart above govern legality.**

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **Chernobog AP HMG** is the heavy **TAG** 3STR/TacAware anti-armor anchor with a greater direct-fire budget than most infantry HMGs; damage-state changes reduce its staying power. **Mirage-5 60/2** instead buys side/back attacks by landing path and Smoke rather than winning a frontal HMG FtF; both pieces pay heavily in Orders if their entry/target geometry is poor. Prefer cheaper specialist and supporting gun redundancy if a massive 1-turn strike prevents later objectives. [Separate TAG/non-TAG gunfighter tier guide](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## Warbands and inexpensive trading roles — N5.3

**Varangian Chain+Smoke10/0** is a standout **Regular+Impetuous** cheap CC23/Berserk/Smoke/Dogged order/body (unlike 5pt Irregular Galwegian). **Irmandinho8/0** is cheap Irregular Smoke+Engineer with D-Charges for mission, while **Denma12/0** adds 15-5/Berserk/AP+DA/MetaChemistry; use the 4pt premium to cross an important gap. **Ioann Bann32/0** is heavy dog-warrior with Viral bow+Smoke, not a throwaway. **Wallace LT38 Inspiring Leadership** can regularize eligible Irmandinhos, but Varangians and Denma are **already Regular**; **Wallace CoC38** is another legal loadout. FT-05 permits listed Varangians/Denma/Ioann with current limits only.

[Cross-game warband/cheap-trader apex and value tiers, targets and command packages](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). Profile-specific sectorial legality/Fireteams above control all selections.

## TAG tactical cross-reference (2026-10-23)

**Chernobog** adds AP HMG/HRL or HFT reach to Kosmoflot and has a local Duo option. Prefer the **63-point HFT** when saving for scoring troops and personal defence; **70-point HRL+1B** to contest hard/clustered lanes. Compare the entire legal FT-04 Duo against buying a different second gun/specialist, and keep screens against E/M/close attacks.

For the two-tier **apex/points-value** comparison, TAG counterplay, matchup matrix and direct transcript sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Treat current profiles, points/SWC and canonical Fireteam data above as authoritative.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Wardriver HD 14pts/1 SWC** supplies basic Carbonite/Oblivion/Spotlight and a Specialist in a faction otherwise built on Camo, warbands and potent direct fire. **Why:** without a thick Repeater network, it will generally cover a small area and can be a worse use of SWC than a dedicated attacker. Bring it only to punish a predictable hackable TAG/HI lane or meet a hacking-specific scenario; otherwise nonhackable pressure/impetuous movement and mission specialists do the work. Kosmoflot's current main roster does **not** inherit Nomad KHD hybrids just because units are shared elsewhere.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

For cross-faction **apex** and **points-value** rankings, the Order types, situational counterexamples and transcript-backed disagreements, see [Cheerleaders and Order Generators — N5.3](../../notes/list-building/cheerleaders-and-order-generators.md). Roster profiles/AVA/Fireteam legality above take precedence.

- **Roster-specific candidates**: 1518, 243, 257. Check their current profile prices, Training and second job; these are not claimed to be cheaper than generic REMs.

**List-building test:** count *transferable* Regular Orders by Combat Group after deployment; include required link members/command enablers, physical DZ footprint, and the unit's actual ARO/mission contribution. Do not treat Irregular, Tactical, Lieutenant or Peripheral activations as interchangeable generic Orders.


## ARO apex/value cross-reference (2026-10-23)

See [ARO units: N5.3 apex/value tiers, hidden-versus-visible and deployment/matchups](../../notes/list-building/aro-units-apex-and-value.md). The **current profile details here** control exact cost/SWC, Training and Fireteam eligibility; do not import another faction's link or specialist upgrades.

- **Cateran T2/AP Sniper (21pt)** — camouflaged long-range trade-up to HITAG, Irregular status: no transferable pool Order
- **Uragan Guided/TR** — low-cost reactive volume that can be recovered; compare with cheap Dozer and spotter infrastructure
- **Traktor Mul support** — rare Ariadna cheap reload/guided/total-reaction choices; only buy a real Guided program if FO route is viable
- **3pt Warcor Flash** — Irregular very-cheap ARO tax, not a transferable pool Order

**Choose by circumstance:** a hard long gun matters only when the opponent must cross its arc; cheaper mines, Camo markers, templates, Flash, DTWs and hacking force movement or risk without committing an entire attack plan. Budget a second layer and preserved counterattack, check pie-slicing, hidden Order cost, anti-visual bypass and repair routes.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Dozer13 WIP13 + Remontnikbot2** creates a cheap Servant-based **Chernobog/REM** repair radius; a single successful Engineer contact roll revives ordinary STR Unconscious per current target-specific rules. **Irmandinho8** contributes forward Smoke, cheap engineer and trade pressure but not guaranteed access to a dying TAG. **112 motorbike19** reaches endangered infantry on flanks; **Kazak Doktor12** is the static budget alternative, each 65% on first WIP13 medical roll. [Doctor/Engineer recovery odds and tier guide](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Varangian Guard10/0 Regular Smoke+CC23/Berserk** anchors strong *cheap forward-threat* play: important value is Regular Order and denial of enemy fire while stronger assault pieces advance. **Mirage-5 Duroc+Margot** is the premium two-body flank assault: **Duroc** pressures from unexpected DZ/edge rather than winning a Ninja-style Hidden first strike; check composite points/orders, not unit-alone price. **Ioann Bann** provides a tougher dog-warrior close fighter when the route is legal. **Uxía** and legal infiltration targets offer better starting proximity but inferior raw MA5 ceiling. [Close-combat apex/value, positioning and counter-CC](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Varangian10 Regular Smoke** (not panzer anti-TAG gun), **Duroc/Mirage-5** Smoke/flank, and **Uxía infiltration** create delivery; choose a current rostered **Frontovik Panzerfaust**, **Beasthunter Panzerfaust** or **Kazak/Traktor hard-ARO** for ranged wounds instead. **Mirage-5** is a two-model attack investment, not a 6pt direct can-opener; kill support/Engineer after landing an attack. Check exact profile against Kosmoflot rather than importing TAK's TankHunter APC weapon. [Non-hacking armor-killer value rankings and tactical matchups](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Unknown Ranger Specialist Operative + Tactical Awareness39/0** (W1+NWI, ARM4, Mimetism(-3), immunity, MA/NBW) provides unusually self-funded and hardy covered carrier as well as 39VP zone; separate **42/1 AP Spitfire** profiles change combat payoff. **S.A.S. FO21/0** infiltrates box before opponent, then must stay visible as a Model holding item; **Frontovik Paramedic23/0** is cheap cover-capable scoring support. **Volkolak W1+NWI/ARM4+BTS6+Immunity** protects a zone/engagement path, but doesn't gain Specialist automatically. **Polaris Masha+Bearpode** is a full dependent team, not a 9pt independently scoring Bearpode; **Ioann Bann32/0** transformed W3/ARM4 makes fast Irregular contested zone/Smoke screen, **not a Specialist carrier**. **Counter:** when the enemy can simply steal/touch the box, Ranger behind terrain + 2 cheap flank guards may outperform parking expensive Bearpode in open ARO.

[Cross-game objective holder and zone-domination apex/value tiers, scenario rules, and opposing transcript reviews](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Exact profiles/Fireteams above are authoritative.

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Kibervolk** has rare **Sensor + Biometric Visor**: Sensor clears eligible Camo/Hidden *within ZoC*, Biometric improves legal Discover versus IMP-1; neither is automatic universal detection. **Wardriver Disco Baller16/1** is a true anti-enemy-MSV/Marksmanship **Eclipse** crossing, while **Varangian Smoke10/0** efficiently masks ordinary fire but not MSV2. **Decision:** if the opponent deploys marker/IMP attackers, use Kibervolk to guard their approach; if an elite visor blocks an objective, spend Disco/setup Orders or find a covered fast flank. Avoid paying both packages when ordinary Smoke and mission route suffice.

[Cross-game anti-tech N5.3 apex/value, mechanics, matchups and checked conflicting transcripts](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## N5.3 peripheral / synchronized / multi-body apex-value update

**Polaris Team Alpha32/0 = Masha9pt + Bearpode23pt and TWO Regular Orders**; **Beta40/0 = Masha9 + Bearpode31** also 2 Regular. **Not Peripheral(Synchronized/Control)**; you can move/attack either as genuinely independent unit in same Combat Group, unlike Antipode pack. **S.A.S. FO21/0** or local mission Specialist must do objective interactions—Bearpode doesn't automatically inherit it. **Kazak Doctor +2pt Remontnikbot Servant** (if legal source option) allows wide recovery while Controller hides, *not additional Regular Order*. **Contrast:** 26pt Antipode pack is *not automatically imported from Vanilla/TAK* into Kosmoflot just because it has SAS/Polaris; Kosmoflot's 32pt double-Order Bearpode duo wins hard target pushing but exposes many points to heavy AROs.

[Cross-game multi-body apex/value and transcript disputes](../../notes/list-building/peripheral-synchronized-multibody-apex-value.md). Current sectorial roster and N5.3 rules decide actual type and access.
