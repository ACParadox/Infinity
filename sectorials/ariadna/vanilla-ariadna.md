---
schema_version: 1
reference_type: faction
status: current
sectorial_id: 301
sectorial_slug: vanilla-ariadna
sectorial_name: Vanilla Ariadna
parent_faction: Ariadna
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "51 standard Army-301 logical units; optional Intel Spec-Ops and Ariadna Team-Ops hooks; complete vanilla Ariadna Fireteam chart; linked L'Équipe Argent reinforcement Fireteam chart"
---

# Vanilla Ariadna

This file is the repository-native factual reference for **Vanilla Ariadna (Army ID 301)** under the N5.3 baseline. It records the Army-301 roster, profiles/loadouts, AVA, points/SWC, the current limited vanilla Fireteam chart, optional game-mode hooks, and the linked **L'Équipe Argent (Army ID 399)** Reinforcement Fireteam chart.

The structured Army source is pinned to revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `d4329bb596ffea5d568eb2435f74366c305a7630`. InfinityDB commit `4e2662be3f43387fbae42b3790a711b3e98570c4` is the normalized identity/reference baseline.

The source file also carries a generic mercenary catalogue with `factions: []`. Those catalogue-only entries are **not** part of this reference's standard Vanilla Ariadna roster. The standard roster below is the set of logical units whose source `factions` includes Army `301`; Intel Spec-Ops and Ariadna Team-Ops are recorded separately as optional game-mode entries.

## Faction summary

| Field | Value |
|---|---|
| Faction | Vanilla Ariadna |
| Parent faction | Ariadna |
| Army ID | 301 |
| Rules baseline | N5.3 |
| Standard roster units | 51 logical units |
| Optional game-mode units | Intel Spec-Ops; Ariadna Team-Ops |
| Linked Reinforcement roster | L'Équipe Argent, Army ID 399 |
| Fireteam chart | yes — limited vanilla chart |

## Fireteam chart limits and faction-level restrictions

| Constraint | Value / wording |
|---|---|
| Core | 0 |
| Haris | up to 1 |
| Duo | up to 2 |
| Standard Fireteam rows | Ariadna Fireteams I; Ariadna Fireteams II |
| Wildcards | none exposed by the pinned vanilla chart |
| Main/Reinforcement mixing | No source-defined mixing exception; keep charts separate |
| Apache restriction | Only profiles named `APACHE FTO` may use the FT-02 Apache slot |
| Barsuk restriction | Only profiles named `BARSUK FTO` may use the FT-02 Barsuk slot |
| Brigadier Bruant restriction | Only profiles named `BRIGADIER BRUANT FTO` may use the vanilla Fireteam rows; the infiltrating Bruant profile is explicitly barred from Fireteams by the source note |

## Unit roster index

`Total` below represents source AVA `255`.

| Unit ID | Unit | AVA | Troop type | Classification | Regularity | Notes |
|---:|---|---:|---|---|---|---|
| 227 | Line Kazaks | Total | LI | Line Troops | Regular | Lieutenant, FO, Paramedic and Commlink profiles |
| 257 | Traktor Mul Unit | 2 | REM | Support Troops | Regular | Baggage; Guided artillery / Total Reaction options |
| 1136 | Frontoviks | 2 | LI | Veteran Troops | Regular | FT-01 and FT-02 access |
| 241 | Antipode Assault Pack | 2 packs | WB | Support Troops | Regular | Handler + 3 Antipodes; Tactical Awareness |
| 237 | 1st Highlanders S.A.S. | 1 | SK | Specialist Trained Troops | Regular | Camo infiltrator |
| 939 | Knauf, Outlaw Sniper | 1 | LI | Character | Regular | MSV1 sniper |
| 265 | Wardrivers, Mercenary Hackers | 1 | LI | Mercenary Troops | Regular | Hacker; optional Disco Baller |
| 258 | Equipe Mirage-5 | 1 team | mixed HI/WB | Character | mixed | Margot + Duroc compound team |
| 1127 | Ratnik | 1 | HI | Headquarters Troops | Regular | Transmutation; Tactical Awareness |
| 233 | Moblots | 1 | HI | Veteran Troops | Regular | Tactical Awareness; FT-02 access |
| 1757 | Apaches | 2 | WB | Support Troops | Regular | FTO and Forward Deployment variants |
| 1461 | Varangian Guard | 4 | WB | Mercenary Troops | Regular + Impetuous | FT-01 access |
| 1284 | 112, Emergency Service (Motorized) | 1 | LI | Support Troops | Regular | Doctor; Motorcycle |
| 263 | Uxía McNeill | 1 | SK | Character | Regular | Infiltration PH=19; specialist |
| 1525 | Cadin “FirstStrike” Donn | 1 | WB | Character | Regular | CC assault character |
| 244 | Van Zant | 1 | LI | Character | Regular | Parachutist deployment-zone; Tactical Awareness |
| 260 | Briscards | 2 | MI | Veteran Troops | Regular | MSV1; FT-01 and FT-02 access |
| 234 | Veteran Kazaks | 2 | HI | Elite Troops | Regular | NWI; FT-01 and FT-02 access |
| 1150 | Vassily Plushenko | 1 | MI | Character | Regular | Camo TankHunter officer; Chain of Command / LT variants |
| 247 | Loup-Garous | 2 | LI | Specialist Trained Troops | Regular | X-Visor; FT-01 and FT-02 access |
| 1584 | Chernobog Armored Detachment | 1 | TAG | Mechanized Troops | Regular | Transmutation; ancillary Samodelkin |
| 259 | William Wallace | 1 | WB | Character | Regular | Inspiring Leadership; Number 2 |
| 228 | Para-Commandos | 2 | LI | Specialist Trained Troops | Regular | Parachutist |
| 1846 | Vystrel Mobile Artillery Regiment | 1 | REM | Support Troops | Regular | Sapper artillery platform |
| 248 | Highlander Caterans | 1 | LI | Specialist Trained Troops | Irregular | Camo sniper |
| 231 | TankHunters | 2 | MI | Elite Troops | Regular | Camo heavy weapons / CoC |
| 229 | Kazak Spetsnazs | 2 | MI | Elite Troops | Regular | Marksmanship; Camo or Parachutist variants |
| 1522 | Polaris Team | 1 team | mixed LI/WB | Support Troops | Regular | 1 Masha + 1 Bearpode; same Combat Group |
| 238 | Ariadna Scouts | 1 | SK | Elite Troops | Regular | Camo infiltrator; Ohotnik |
| 777 | The Unknown Ranger | 1 | MI | Character | Regular | Tactical Awareness; NWI; Specialist Operative |
| 1126 | Streloks | 2 | LI | Specialist Trained Troops | Regular | Camo; Decoy; optional K-9 Antipode |
| 1581 | Remontnikbot V-5 Elektronik | 2 | REM | Support Troops | no Order | Peripheral (Servant) |
| 1518 | Rokots | 2 | LI | Line Troops | Regular | Camo infiltrator and basic profiles |
| 235 | Foxtrot Rangers | 1 | SK | Specialist Trained Troops | Regular | Camo infiltrator |
| 243 | Kazak Doktor | 1 | LI | Support Troops | Regular | Doctor; FT-01 access |
| 768 | Colonel Yevgueni Voronin | 1 | LI | Character | Regular | Counterintelligence; Sensor; LT Strategos option |
| 1847 | Mekhamobilya Support Pilots | 1 | LI | Support Troops | Regular | Chernobog pilot; Specialist Operative |
| 252 | Chasseurs | 2 | SK | Specialist Trained Troops | Regular | Camo infiltrator; Sixth Sense |
| 239 | 45th Highlanders Rifles | 4 | WB | Line Troops | Irregular + Impetuous | FT-01 access |
| 255 | 112, Emergency Service | 2 | LI | Support Troops | Regular | Doctor; profile is named FTO but no vanilla chart slot |
| 1134 | Dynamo | 2 | LI | Specialist Trained Troops | Regular + Impetuous | Motorcycle; FT-01 access |
| 1844 | Konduktors | 1 | LI | Garrison Troops | Regular | FTO-labelled profiles but no vanilla chart slot |
| 242 | Dog-Warriors | 2 | WB | Support Troops | Irregular + Impetuous | Transmutation; FT-01 access |
| 50 | Warcors | 1 | LI | Mercenary Troops | Irregular | Journalist |
| 1519 | Zenit-7 Detachment | 1 | LI | Elite Troops | Regular | Camo; Decoy; CoC / FO options |
| 240 | Irmandinhos | 2 | WB | Line Troops | Irregular + Impetuous | Engineer; Booty; FT-01 access |
| 752 | Desperadoes | 2 | WB | Specialist Trained Troops | Irregular + Impetuous | Motorcycle |
| 256 | Dozers, Field Engineers | 1 | LI | Support Troops | Regular | Engineer; support-equipment variants |
| 262 | Brigadier Jacques Bruant | 1 | LI | Character | Regular | FTO profiles plus separate infiltrating profile |
| 1843 | Kibervolk Patrol | 1 patrol | mixed LI/WB | compound | Regular | 1 Dozer KVP + 1 Kibervolk; same Combat Group |
| 1845 | Barsuk | 2 | MI | Garrison Troops | Regular | FTO, FD and Camo variants |

## Unit details

### Line Kazaks

**Unit ID:** 227  
**Slug:** `line-kazaks`  
**AVA:** Total (`255`)  
**Troop type:** LI  
**Classification:** Line Troops

#### Base profile

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 11 | 11 | 13 | 1 | 0 | 1 | 2 |

**Characteristics:** Regular, Not Impetuous.

#### Loadouts

| Profile ID | FTO | SWC | Points | Weapons | Skills / equipment differences | Flags |
|---|---|---:|---:|---|---|---|
| 227-1-1 | — | 0 | 9 | Rifle; Pistol; CC Weapon | — | — |
| 227-1-2 | — | 1 | 20 | HMG; Pistol; CC Weapon | — | — |
| 227-1-5 | — | 1.5 | 17 | Missile Launcher; Pistol; CC Weapon | — | — |
| 227-1-6 | — | 0 | 10 | Rifle; Flash Pulse; Pistol; CC Weapon | Forward Observer | Specialist |
| 227-1-7 | — | 0 | 11 | Rifle; Pistol; CC Weapon | Paramedic; MediKit | Specialist |
| 227-1-8 | — | 0 | 9 | Rifle; Pistol; CC Weapon | Lieutenant | Lieutenant |
| 227-1-10 | — | 0 | 11 | Rifle; Pistol; CC Weapon | Commlink (+2); Specialist Operative | Specialist |

### Traktor Mul Unit

**Unit ID:** 257  
**Slug:** `traktor-mul`  
**AVA:** 2  
**Troop type:** REM  
**Classification:** Support Troops

#### Base profile

| MOV | CC | BS | PH | WIP | ARM | BTS | STR | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 13 | 10 | 9 | 12 | 2 | 0 | 1 | 4 |

**Skills:** Remote Presence; Courage.  
**Equipment:** Baggage; ECM: Guided (-6).  
**Characteristics:** Regular, Not Impetuous, Hackable.

#### Loadouts

| Profile ID | SWC | Points | Weapons | Skills / equipment differences |
|---|---:|---:|---|---|
| 257-1-1 | 0 | 5 | PARA CC Weapon (-3) | Deactivator |
| 257-1-2 | 1 | 9 | Katyusha MRL; PARA CC Weapon (-3) | BS Attack (Guided) |
| 257-1-3 | 1 | 14 | Uragan MRL; PARA CC Weapon (-3) | BS Attack (Guided); Total Reaction |

### Frontoviks, Separate Assault Battalion

**Unit ID:** 1136  
**Slug:** `frontoviks-separate-assault-bat`  
**AVA:** 2  
**Troop type:** LI  
**Classification:** Veteran Troops

#### Base profile

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 17 | 12 | 11 | 13 | 2 | 0 | 1 | 2 |

**Skills:** Courage; Mimetism (-3); Warhorse.

#### Loadouts

| Profile ID | SWC | Points | Weapons | Skills / equipment differences | Flags |
|---|---:|---:|---|---|---|
| 1136-1-1 | 0 | 21 | T2 Rifle; Assault Pistol; CC Weapon | — | — |
| 1136-1-2 | 1 | 30 | AP Spitfire; Assault Pistol; CC Weapon | — | — |
| 1136-1-3 | 1.5 | 19 | Heavy Rocket Launcher; Assault Pistol; CC Weapon | — | — |
| 1136-1-6 | 0 | 26 | T2 Rifle; Panzerfaust; D-Charges; Assault Pistol; CC Weapon | Engineer; Deactivator | Specialist |
| 1136-1-7 | 0 | 23 | T2 Rifle; Assault Pistol; CC Weapon | Paramedic; MediKit | Specialist |
| 1136-1-8 | 0.5 | 28 | AP Sniper Rifle; Assault Pistol; CC Weapon | MSV1 | — |
| 1136-1-9 | 0 | 21 | T2 Rifle; Assault Pistol; CC Weapon | Lieutenant | Lieutenant |

### Antipode Assault Pack

**Unit ID:** 241  
**Slug:** `antipode-assault-pack`  
**AVA:** 2 packs  
**Classification:** Support Troops

#### Handler

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 11 | 11 | 13 | 1 | 0 | 1 | 2 |

**Skills:** Tactical Awareness.  
**Loadout `241-1-1`:** 26 points / 0 SWC — Rifle, Smoke Grenade Launcher, Pistol, CC Weapon; includes 3 Antipodes and generates 1 Regular + 1 Tactical Awareness Order.

#### Antipode peripheral

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-15 | 20 | 0 | 15 | 13 | 0 | 0 | 1 | 5 |

**Skills:** Peripheral (Control); Surprise Attack (-3); Camouflage; Dodge (+5 cm); Mimetism (-3); Sensor; Stealth; Super-Jump; Terrain (Jungle); No Cover.  
**Included option `241-2-1`:** AP CC Weapon (PS=5); source points 5, disabled because it is included by the Handler.

### 1st Highlanders S.A.S.

**Unit ID:** 237  
**Slug:** `s-a-s`  
**AVA:** 1  
**Troop type:** SK  
**Classification:** Specialist Trained Troops

#### Base profile

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 22 | 11 | 13 | 13 | 0 | 0 | 1 | 2 |

**Skills:** Surprise Attack (-3); Martial Arts L2; Camouflage; Courage; Dodge (+2.5 cm); Infiltration; Mimetism (-3); Terrain (Total); Stealth.

#### Loadouts

| Profile ID | SWC | Points | Weapons | Skills / differences |
|---|---:|---:|---|---|
| 237-1-1 | 0 | 20 | Chain Rifle; Light Shotgun; D-Charges; Silenced Pistol; AP+Shock CC Weapon (PS=6) | — |
| 237-1-2 | 0 | 20 | Chain Rifle; Grenades; D-Charges; Assault Pistol; AP+Shock CC Weapon (PS=6) | — |
| 237-1-4 | 0 | 21 | Chain Rifle; Light Shotgun; Flash Pulse; D-Charges; Silenced Pistol; AP+Shock CC Weapon (PS=6) | Forward Observer |
| 237-1-5 | 0 | 25 | Boarding Shotgun (+1SD); D-Charges; E/M Mine; Silenced Pistol; AP+Shock CC Weapon (PS=6) | Specialist Operative |
| 237-1-6 | 0.5 | 22 | Chain Rifle; Light Shotgun; D-Charges; AP Mine; Silenced Pistol; AP+Shock CC Weapon (PS=6) | Minelayer |

### Knauf, Outlaw Sniper

**Unit ID:** 939  
**Slug:** `knauf-outlaw-sniper`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Character

#### Base profile

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 21 | 13 | 11 | 13 | 1 | 0 | 1 | 2 |

**Skills:** BS Attack (+1B); BS Attack (Shock); Courage; Mimetism (-3); Stealth; Terrain (Total).  
**Equipment:** MSV1.

**Loadout `939-1-1`:** 31 points / 1.5 SWC — MULTI Sniper Rifle, AP Heavy Pistol, CC Weapon; Surprise Attack (-3); Decoy (1).

### Wardrivers, Mercenary Hackers

**Unit ID:** 265  
**Slug:** `wardrivers-merc-hackers`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Mercenary Troops

#### Base profile

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 13 | 11 | 10 | 13 | 0 | 3 | 1 | 2 |

**Skills:** Sixth Sense.  
**Characteristics:** Cube, Regular, Not Impetuous.

| Profile ID | SWC | Points | Weapons | Skills / equipment differences |
|---|---:|---:|---|---|
| 265-1-1 | 1 | 14 | Boarding Shotgun; Flash Pulse; Cybermine; Pistol; CC Weapon | Hacker; Hacking Device (Upgrade: Zero Pain) |
| 265-1-2 | 1 | 16 | Boarding Shotgun; Flash Pulse; Cybermine; Disco Baller; Pistol; CC Weapon | Hacker; Hacking Device (Upgrade: Zero Pain) |

### Equipe Mirage-5

**Unit ID:** 258  
**Slug:** `equipe-mirage-5`  
**AVA:** 1 team  
**Classification:** Character compound unit

**Source note:** the selectable option is the Margot + Duroc compound team.

#### Lieutenant Margot Berthier

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 16 | 14 | 12 | 13 | 3 | 3 | 1 | 2 |

**Skills:** BS Attack (Shock); Immunity (Shock); Terrain (Total); Parachutist (Deployment Zone); Mimetism (-3); Specialist Operative; Immunity (IMM-B); Combat Instinct; Tactical Awareness; Dodge (+1SD); MediKit (PH=14).  
**Internal option `258-1-1`:** 36 points / 0 SWC — AP Rifle, Grenade Launcher, Light Shotgun, D-Charges, Pistol, CC Weapon; disabled as a standalone choice.

#### Sergent Duroc

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-10 | 23 | 10 | 16 | 13 | 3 | 3 | 2 | 6 |

**Skills:** Martial Arts L2; Courage; Dodge (+2.5 cm); Parachutist (Deployment Zone); Super-Jump; Impetuous; Immunity (ARM); No Cover.  
**Internal option `258-2-1`:** 24 points / 0 SWC — Chain Rifle (+1B), Grenades (PS=6), Smoke Grenades, AP CC Weapon (PS=4); disabled standalone.

#### Compound option

| Profile ID | SWC | Points | Includes | Orders |
|---|---:|---:|---|---|
| 258-C-1 | 2 | 60 | Margot `258-1-1` + Duroc `258-2-1` | 1 Regular, 1 Irregular, 1 Tactical Awareness, 1 Impetuous |

### Armata-2 Proyekt “Ratnik”

**Unit ID:** 1127  
**Slug:** `ratnik`  
**AVA:** 1  
**Troop type:** HI  
**Classification:** Headquarters Troops

#### Full-power profile

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 16 | 13 | 11 | 13 | 6 | 3 | 2 | 5 |

**Skills:** Tactical Awareness; BS Attack (+1B); Courage; Transmutation; Dogged.  
**Equipment:** Deactivator.

#### Battle-ravaged profile

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-5 | 14 | 13 | 10 | 13 | 4 | 0 | 2 | 5 |

**Skills:** Tactical Awareness; BS Attack (+1B); Dogged; Courage.

| Profile ID | SWC | Points | Weapons |
|---|---:|---:|---|
| 1127-1-4140 | 1.5 | 46 | AP Spitfire; Panzerfaust; Flammenspeer; AP Heavy Pistol; Trench-Hammer (PS=4); CC Weapon (PS=6) |
| 1127-1-4141 | 1.5 | 41 | Heavy Rocket Launcher; Heavy Shotgun; AP Heavy Pistol; Trench-Hammer (PS=4); CC Weapon (PS=6) |

### 13éme Moblots

**Unit ID:** 233  
**Slug:** `moblots`  
**AVA:** 1  
**Troop type:** HI  
**Classification:** Veteran Troops

#### Base profile

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 16 | 13 | 12 | 14 | 3 | 3 | 1 | 2 |

**Skills:** BS Attack (Shock); Dodge (+1SD); Immunity (Shock); Terrain (Jungle); Mimetism (-3); MediKit (PH=14); Tactical Awareness; Immunity (IMM-B); Combat Instinct.  
**Characteristics:** Regular, Non-Hackable.

| Profile ID | SWC | Points | Weapons | Skills / equipment differences | Flags |
|---|---:|---:|---|---|---|
| 233-1-2 | 1.5 | 32 | HMG; Boarding Pistol; CC Weapon | — | — |
| 233-1-3 | 0 | 27 | AP Rifle; Light Shotgun; Flammenspeer; Boarding Pistol; CC Weapon | — | — |
| 233-1-7 | 0 | 31 | AP Rifle; Light Shotgun; Flammenspeer; E/M Mine; D-Charges; Boarding Pistol; CC Weapon | Engineer; Deactivator; GizmoKit | Specialist |
| 233-1-8 | 0 | 29 | AP Rifle; Light Shotgun; Flammenspeer; Boarding Pistol; CC Weapon | Paramedic; MediKit | Specialist |
| 233-1-13 | 0 | 27 | AP Rifle; Light Shotgun; Flammenspeer; Boarding Pistol; CC Weapon | Lieutenant | Lieutenant |
| 233-1-14 | 1.5 | 32 | HMG; Boarding Pistol; CC Weapon | Lieutenant | Lieutenant |
| 233-1-15 | 1.5 | 32 | AP Spitfire (PS=5); Boarding Pistol; CC Weapon | — | — |

### Apaches, Équipe d'Intervention Urbaine

**Unit ID:** 1757  
**Slug:** `apaches`  
**AVA:** 2  
**Troop type:** WB  
**Classification:** Support Troops

#### Base profile

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-5 | 22 | 11 | 13 | 12 | 1 | 0 | 1 | 2 |

**Skills:** Frenzy; BS Attack (+1B); Courage; Dodge (+2.5 cm); Immunity (Shock); NWI; Super-Jump; CC Attack (-6); CC Attack (+1B).

| Profile ID | FTO | SWC | Points | Weapons | Skills / differences |
|---|---|---:|---:|---|---|
| 1757-1-1 | yes | 0 | 19 | Rifle; Chain-colt; Heavy Pistol; AP+Shock CC Weapon (PS=6) | — |
| 1757-1-2 | yes | 0 | 14 | Chain Rifle; Grenades; Heavy Pistol; AP+Shock CC Weapon (PS=6) | — |
| 1757-1-3 | yes | 0 | 17 | Light Shotgun; Heavy Pistol; AP+Shock CC Weapon (PS=6) | — |
| 1757-1-5 | no | 0 | 20 | Light Shotgun; Grenades; Heavy Pistol; AP+Shock CC Weapon (PS=6) | Forward Deployment (+20 cm); Berserk |
| 1757-1-7 | no | 0 | 17 | Chain Rifle; Grenades; Heavy Pistol; AP+Shock CC Weapon (PS=6) | Forward Deployment (+20 cm); Berserk |

### Varangian Guard

**Unit ID:** 1461  
**Slug:** `varangian-guard`  
**AVA:** 4  
**Troop type:** WB  
**Classification:** Mercenary Troops

#### Base profile

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 23 | 10 | 14 | 13 | 2 | 0 | 1 | 2 |

**Skills:** Berserk (+3); Impetuous; No Cover; Dogged; Religious Troop.

| Profile ID | SWC | Points | Weapons |
|---|---:|---:|---|
| 1461-1-3 | 0 | 13 | Boarding Shotgun; Smoke Grenades; Heavy Pistol; AP CC Weapon (PS=6) |
| 1461-1-4 | 0 | 12 | SMG; Chain Rifle; Smoke Grenades; Heavy Pistol; AP CC Weapon (PS=6) |
| 1461-1-5 | 0 | 13 | SMG; Chain-colt (+1B); Smoke Grenades; Heavy Pistol; AP CC Weapon (PS=6) |
| 1461-1-6 | 0 | 13 | SMG; Chain Rifle; Smoke Grenades; Heavy Pistol; Trench-Hammer; AP CC Weapon (PS=6) |

### 112, Emergency Service (Motorized)

**Unit ID:** 1284  
**Slug:** `112-emergency-service-motorized`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Support Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 20-10 | 16 | 11 | 12 | 13 | 0 | 0 | 1 | 4 |

**Skills:** Doctor; Courage; Mimetism (-3); Limited Cover.  
**Equipment:** MediKit; Motorcycle.  
**Loadout `1284-1-4761`:** 19 points / 0 SWC — Light Shotgun, Smoke Grenade Launcher, Smoke Grenades, Boarding Pistol, CC Weapon.

### Uxía “Cherry” McNeill

**Unit ID:** 263  
**Slug:** `uxia-mcneill`  
**AVA:** 1  
**Troop type:** SK  
**Classification:** Character

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 22 | 11 | 13 | 13 | 0 | 0 | 1 | 2 |

**Skills:** Martial Arts L2; Surprise Attack (-3); Courage; Camouflage; Dodge (+5 cm); Mimetism (-3); Stealth; Terrain (Total); Frenzy; Infiltration (PH=19); BS Attack (+1B); Specialist Operative.  
**Equipment:** MSV1.

| Profile ID | SWC | Points | Weapons |
|---|---:|---:|---|
| 263-1-1 | 0 | 25 | Boarding Shotgun; Grenades; Smoke Grenades; Boarding Pistol; AP+Shock CC Weapon (PS=5) |
| 263-1-2 | 0 | 25 | Boarding Shotgun; D-Charges; Smoke Grenades; Assault Pistol; AP+Shock CC Weapon (PS=5) |

### Cadin “FirstStrike” Donn

**Unit ID:** 1525  
**Slug:** `cadin-firststrike-donn`  
**AVA:** 1  
**Troop type:** WB  
**Classification:** Character

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-5 | 23 | 12 | 14 | 13 | 3 | 3 | 2 | 2 |

**Skills:** Frenzy; Courage; Dodge (+5 cm); Climbing Plus; CC Attack (+1B); Martial Arts L1; Berserk (+6); Natural Born Warrior.

**Loadout `1525-1-1`:** 30 points / 0 SWC — T2 Boarding Shotgun, Flammenspeer, E/M Grenades (+1B), Boarding Pistol (PS=6), AP+T2 CC Weapon (PS=5).

### Van Zant

**Unit ID:** 244  
**Slug:** `van-zant`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Character

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 22 | 13 | 13 | 14 | 2 | 0 | 1 | 2 |

**Skills:** Courage; Dodge (+2.5 cm); Parachutist (Deployment Zone); Dogged; Stealth; Martial Arts L3; Berserk (+3); Tactical Awareness; Immunity (Shock).

| Profile ID | SWC | Points | Weapons | Difference |
|---|---:|---:|---|---|
| 244-1-1 | 0 | 33 | AP Rifle; Chain-colt (+1B); AP Heavy Pistol; AP+T2 CC Weapon (PS=5) | — |
| 244-1-2 | 0 | 35 | T2 Boarding Shotgun; Chain-colt; AP Heavy Pistol; AP+T2 CC Weapon (PS=5) | BS Attack (+1B) |

### Briscards

**Unit ID:** 260  
**Slug:** `briscards`  
**AVA:** 2  
**Troop type:** MI  
**Classification:** Veteran Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 16 | 12 | 12 | 13 | 2 | 0 | 1 | 2 |

**Skills:** Courage; Warhorse; Terrain (Mountain); MediKit (PH=14); Climbing Plus.  
**Equipment:** MSV1.

| Profile ID | SWC | Points | Weapons | Skills / differences | Flags |
|---|---:|---:|---|---|---|
| 260-1-2 | 0.5 | 24 | AP Sniper Rifle; Assault Pistol; CC Weapon | BS Attack (Shock) | — |
| 260-1-3 | 1.5 | 20 | Heavy Rocket Launcher (+1B); Assault Pistol; CC Weapon | — | — |
| 260-1-4 | 0 | 22 | AP Marksman Rifle; Flash Pulse; Assault Pistol; CC Weapon | Forward Observer | Specialist |
| 260-1-5 | 0 | 23 | AP Marksman Rifle; Assault Pistol; CC Weapon | Paramedic; MediKit | Specialist |
| 260-1-6 | 0 | 26 | AP Marksman Rifle; Flash Pulse; Assault Pistol; CC Weapon | Lieutenant (+1 Command Token); Forward Observer | Lieutenant, Specialist |

### Veteran Kazaks

**Unit ID:** 234  
**Slug:** `veteran-kazaks`  
**AVA:** 2  
**Troop type:** HI  
**Classification:** Elite Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-5 | 17 | 13 | 12 | 14 | 4 | 3 | 1 | 2 |

**Skills:** Courage; Immunity (Shock); Mimetism (-3); Sixth Sense; NWI; Warhorse; Combat Instinct; Dodge (+1SD); Immunity (IMM-B); MediKit (PH=15); Terrain (Total).  
**Characteristics:** Regular, Non-Hackable.

| Profile ID | SWC | Points | Weapons | Skills / equipment differences | Flags |
|---|---:|---:|---|---|---|
| 234-1-2 | 1.5 | 45 | AP HMG; Heavy Pistol; CC Weapon | — | — |
| 234-1-4 | 0 | 38 | T2 Rifle; Light Flamethrower; Heavy Pistol; CC Weapon | X-Visor; Paramedic; MediKit | Specialist |
| 234-1-5 | 0 | 36 | T2 Rifle; Light Flamethrower; Flash Pulse; Heavy Pistol; CC Weapon | X-Visor; Forward Observer | Specialist |
| 234-1-6 | 0 | 36 | T2 Rifle; Light Flamethrower; Flash Pulse; Heavy Pistol; CC Weapon | X-Visor; Lieutenant; Forward Observer | Lieutenant, Specialist |
| 234-1-7 | 1 | 45 | AP HMG; Heavy Pistol; CC Weapon | Lieutenant | Lieutenant |

### Vassily Plushenko

**Unit ID:** 1150  
**Slug:** `vassily-plushenko`  
**AVA:** 1  
**Troop type:** MI  
**Classification:** Character

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 17 | 13 | 12 | 14 | 3 | 0 | 1 | 2 |

**Skills:** Surprise Attack (-3); Camouflage; Mimetism (-3); Stealth; Dogged; Courage; BS Attack (AP); Decoy (2).

| Profile ID | SWC | Points | Weapons | Skills / flags |
|---|---:|---:|---|---|
| 1150-1-1 | 0 | 39 | T2 Marksman Rifle; Akrylat-Kanone; D-Charges; Heavy Pistol; CC Weapon | Chain of Command |
| 1150-1-2 | 1 | 39 | T2 Sniper Rifle; D-Charges; Heavy Pistol; CC Weapon | Chain of Command |
| 1150-1-3 | 0 | 35 | T2 Marksman Rifle; Akrylat-Kanone; D-Charges; Heavy Pistol; CC Weapon | Lieutenant; Forward Observer |
| 1150-1-4 | 1 | 35 | T2 Sniper Rifle; D-Charges; Heavy Pistol; CC Weapon | Lieutenant; Forward Observer |

### Loup-Garous

**Unit ID:** 247  
**Slug:** `loup-garous`  
**AVA:** 2  
**Troop type:** LI  
**Classification:** Specialist Trained Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 16 | 12 | 11 | 13 | 2 | 0 | 1 | 2 |

**Skills:** BS Attack (SR-1); Religious Troop.  
**Equipment:** X-Visor.

| Profile ID | SWC | Points | Weapons | Differences |
|---|---:|---:|---|---|
| 247-1-1 | 0 | 17 | Viral Rifle; Light Riotstopper; Smoke Grenade Launcher; Heavy Pistol; PARA CC Weapon (-6) | — |
| 247-1-2 | 0 | 15 | Boarding Shotgun; Adhesive Launcher Rifle; Heavy Pistol; PARA CC Weapon (-6) | — |
| 247-1-6 | 1 | 24 | Viral Sniper Rifle; Heavy Pistol; PARA CC Weapon (-6) | Marksmanship |
| 247-1-7 | 0.5 | 24 | Viral Marksman Rifle; Heavy Pistol; PARA CC Weapon (-6) | Marksmanship |

### Chernobog Armored Detachment

**Unit ID:** 1584  
**Slug:** `chernobog-armored-detachment`  
**AVA:** 1  
**Troop type:** TAG  
**Classification:** Mechanized Troops

#### Full-power Chernobog

| MOV | CC | BS | PH | WIP | ARM | BTS | STR | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-10 | 17 | 14 | 16 | 13 | 8 | 6 | 3 | 7 |

**Skills:** Courage; Dodge (PH=9); Tactical Awareness; GizmoKit (PH=9); BS Attack (SR-1); Transmutation (2).  
**Equipment:** ECM: Guided (-6).

#### Battle-ravaged Chernobog

| MOV | CC | BS | PH | WIP | ARM | BTS | STR | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-5 | 15 | 13 | 15 | 13 | 6 | 3 | 3 | 7 |

**Skills:** BS Attack (SR-1); Courage; Dodge (PH=9); Tactical Awareness; GizmoKit (PH=9).  
**Equipment:** ECM: Guided (-3).

| Profile ID | SWC | Points | Weapons |
|---|---:|---:|---|
| 1584-1-1 | 1.5 | 70 | AP HMG; Heavy Rocket Launcher (+1B); Chest Mine; AP CC Weapon (PS=4) |
| 1584-1-2 | 1.5 | 63 | AP HMG; Heavy Flamethrower; Chest Mine; AP CC Weapon (PS=4) |

#### RB-235 Samodelkin ancillary

| MOV | CC | BS | PH | WIP | ARM | BTS | STR | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-10 | — | — | 10 | 12 | 0 | 0 | 1 | 1 |

**Skills:** Courage; Specialist Operative; Mimetism (-3); Peripheral (Ancillary).  
**Internal option `1584-2-1`:** 2 source points, disabled; included by either Chernobog loadout.

### William Wallace

**Unit ID:** 259  
**Slug:** `william-wallace`  
**AVA:** 1  
**Troop type:** WB  
**Classification:** Character

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-10 | 24 | 13 | 14 | 15 | 3 | 0 | 2 | 2 |

**Skills:** CC Attack (-3); Berserk (+3); Courage; Dodge (+5 cm); Natural Born Warrior; Immunity (Critical); Inspiring Leadership; Frenzy; Number 2; CC Attack (+1B).

**Loadout `259-1-1`:** 38 points / 0 SWC — T2 Rifle (PS=6), Light Shotgun, Smoke Grenades, Boarding Pistol (+1B), EXP CC Weapon (PS=5); Chain of Command (Non Specialist).

### 1er Régiment de Para-Commandos

**Unit ID:** 228  
**Slug:** `para-commandos`  
**AVA:** 2  
**Troop type:** LI  
**Classification:** Specialist Trained Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 16 | 12 | 11 | 14 | 2 | 3 | 1 | 2 |

**Skills:** Mimetism (-3); Parachutist; Terrain (Zero-G).

| Profile ID | SWC | Points | Weapons | Skills / equipment differences |
|---|---:|---:|---|---|
| 228-1-1 | 0 | 18 | Rifle; Boarding Pistol; CC Weapon | — |
| 228-1-4 | 1 | 29 | AP Spitfire; Boarding Pistol; CC Weapon | — |
| 228-1-6 | 0 | 21 | Boarding Shotgun; Flash Pulse; D-Charges; Boarding Pistol; CC Weapon | BS Attack (+1SD); Forward Observer |
| 228-1-8 | 0 | 19 | SMG; D-Charges; Boarding Pistol; CC Weapon | Paramedic; MediKit |

### Vystrel Mobile Artillery Regiment

**Unit ID:** 1846  
**Slug:** `vystrel-mobile-artillery-regiment`  
**AVA:** 1  
**Troop type:** REM  
**Classification:** Support Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | STR | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 13 | 12 | 9 | 12 | 2 | 0 | 2 | 4 |

**Skills:** BS Attack (SR-1); BS Attack (Shock); Courage; Remote Presence; Sapper.  
**Equipment:** ECM: Guided (-6).

| Profile ID | SWC | Points | Weapons | Difference |
|---|---:|---:|---|---|
| 1846-1-1 | 0.5 | 23 | AP Sniper Rifle; Light Rocket Launcher; PARA CC Weapon (-3) | — |
| 1846-1-2 | 1.5 | 32 | Portable Autocannon; Light Rocket Launcher; PARA CC Weapon (-3) | Neurocinetics |
| 1846-1-3 | 0.5 | 26 | AP Sniper Rifle; Light Rocket Launcher; PARA CC Weapon (-3) | Neurocinetics |

### Highlander Caterans

**Unit ID:** 248  
**Slug:** `highlander-caterans`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Specialist Trained Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 22 | 12 | 13 | 12 | 0 | 0 | 1 | 2 |

**Skills:** Surprise Attack (-3); Camouflage (1 Use); Mimetism (-3); Stealth; Climbing Plus.  
**Characteristics:** Irregular.

| Profile ID | SWC | Points | Weapons | Difference |
|---|---:|---:|---|---|
| 248-1-1 | 1 | 21 | T2 Sniper Rifle; Pistol; AP CC Weapon (PS=7) | — |
| 248-1-2 | 0.5 | 21 | AP Sniper Rifle; Pistol; AP CC Weapon (PS=7) | — |
| 248-1-3 | 1 | 23 | T2 Sniper Rifle; Pistol; AP CC Weapon (PS=7) | Forward Deployment (+10 cm) |

### TankHunters Regiment

**Unit ID:** 231  
**Slug:** `tankhunters`  
**AVA:** 2  
**Troop type:** MI  
**Classification:** Elite Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 13 | 12 | 13 | 3 | 0 | 1 | 2 |

**Skills:** Surprise Attack (-3); Camouflage; Courage; Mimetism (-3); Stealth.

| Profile ID | SWC | Points | Weapons | Skills / differences | Flags |
|---|---:|---:|---|---|---|
| 231-1-1 | 1.5 | 33 | AP HMG; D-Charges; AP Mine; Pistol; CC Weapon | — | — |
| 231-1-2 | 1.5 | 36 | Portable Autocannon (+1B); D-Charges; AP Mine; Pistol; CC Weapon | — | — |
| 231-1-3 | 1.5 | 28 | Missile Launcher; D-Charges; AP Mine; Pistol; CC Weapon | — | — |
| 231-1-4 | 0 | 25 | AP SMG; Panzerfaust; D-Charges; AP Mine; Pistol; CC Weapon | Chain of Command; Minelayer | Specialist |
| 231-1-5 | 0.5 | 24 | AP SMG; Panzerfaust; D-Charges; AP Mine; Pistol; CC Weapon | Forward Deployment (+20 cm); Minelayer | — |
| 231-1-6 | 0 | 25 | AP Rifle; Adhesive Launcher Rifle; D-Charges; AP Mine; Pistol; CC Weapon | Minelayer | — |
| 231-1-7 | 0 | 25 | AP Rifle; Adhesive Launcher Rifle; D-Charges; AP Mine; Pistol; CC Weapon | Lieutenant; Minelayer | Lieutenant |

### Kazak Spetsnazs

**Unit ID:** 229  
**Slug:** `kazak-spetsnazs`  
**AVA:** 2  
**Troop type:** MI  
**Classification:** Elite Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 21 | 12 | 12 | 13 | 2 | 0 | 1 | 2 |

**Skills:** Martial Arts L2; BS Attack (Shock); Courage; Marksmanship; Stealth; Mimetism (-3).

| Profile ID | SWC | Points | Weapons | Skills / differences |
|---|---:|---:|---|---|
| 229-1-1 | 1.5 | 36 | HMG; Silenced Pistol; AP CC Weapon (PS=7) | Surprise Attack (-3); Camouflage; Decoy (1) |
| 229-1-2 | 0.5 | 32 | AP Sniper Rifle (PS=4); Silenced Pistol; AP CC Weapon (PS=7) | Surprise Attack (-3); Camouflage; Decoy (1) |
| 229-1-3 | 0 | 27 | Boarding Shotgun (+1B); Grenades; D-Charges; Silenced Pistol; AP CC Weapon (PS=7) | Parachutist; Decoy (1) |
| 229-1-4 | 0 | 27 | AP SMG (+1B); Grenades; D-Charges; Silenced Pistol; AP CC Weapon (PS=7) | Parachutist; Decoy (1) |

### Polaris Team

**Unit ID:** 1522  
**Slug:** `polaris-team`  
**AVA:** 1 team  
**Classification:** Support Troops

**Source note:** a Polaris Team is composed of **1 Masha and 1 Polaris Bearpode**, and both must belong to the same Combat Group.

#### Masha

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 11 | 11 | 13 | 2 | 0 | 1 | 2 |

**Internal option `1522-1-1`:** 9 points / 0 SWC — Light Shotgun, Pistol, CC Weapon; disabled standalone.

#### Polaris Bearpode

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-10 | 24 | 5 | 16 | 12 | 4 | 3 | 2 | 6 |

**Skills:** Courage; Dogged; Climbing Plus; Immunity (ARM); No Cover; Frenzy; Berserk (+3); Dodge (+5 cm).

| Internal profile ID | Source points | Weapons | Differences |
|---|---:|---|---|
| 1522-2-1 | 23 | Chain Rifle (+1B, PS=6); Trench-Hammer (PS=3); AP CC Weapon (PS=3); Grenades (PS=6); Smoke Grenades | Alpha |
| 1522-2-2 | 31 | Heavy Shotgun (PS=4); Chain-colt (PS=6); Smoke Grenades; Trench-Hammer (PS=3); AP CC Weapon (PS=3) | Beta; BS=11 |

#### Selectable compound options

| Profile ID | SWC | Points | Includes | Orders |
|---|---:|---:|---|---|
| 1522-C-1 | 0 | 32 | Masha + Bearpode Alpha | 2 Regular |
| 1522-C-2 | 0 | 40 | Masha + Bearpode Beta | 2 Regular |

### Ariadna Scouts

**Unit ID:** 238  
**Slug:** `scouts`  
**AVA:** 1  
**Troop type:** SK  
**Classification:** Elite Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 15 | 12 | 13 | 13 | 1 | 0 | 1 | 2 |

**Skills:** BS Attack (AP); Surprise Attack (-3); Camouflage; Mimetism (-3); Terrain (Total); Stealth; Infiltration.

| Profile ID | SWC | Points | Weapons | Skills / differences | Flags |
|---|---:|---:|---|---|---|
| 238-1-1 | 0 | 27 | Ohotnik; D-Charges; Shock Mine; Silenced Pistol; CC Weapon | — | — |
| 238-1-2 | 0 | 27 | Ohotnik; D-Charges; PARA Mine; Silenced Pistol; CC Weapon | — | — |
| 238-1-3 | 0 | 23 | T2 Boarding Shotgun; D-Charges; Shock Mine; Silenced Pistol; CC Weapon | — | — |
| 238-1-4 | 0.5 | 25 | T2 Sniper Rifle; Shock Mine; Silenced Pistol; CC Weapon | — | — |
| 238-1-5 | 0.5 | 28 | Ohotnik; D-Charges; E/M Mine; Silenced Pistol; CC Weapon | Minelayer (2) | — |
| 238-1-7 | 0 | 28 | Ohotnik; D-Charges; Flash Pulse; Shock Mine; Silenced Pistol; CC Weapon | Forward Observer | Specialist |
| 238-1-8 | 0 | 27 | Ohotnik; D-Charges; PARA Mine; Silenced Pistol; CC Weapon | Lieutenant | Lieutenant |

### The Unknown Ranger

**Unit ID:** 777  
**Slug:** `the-unknown-ranger`  
**AVA:** 1  
**Troop type:** MI  
**Classification:** Character

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-5 | 23 | 13 | 12 | 13 | 4 | 0 | 1 | 2 |

**Skills:** Martial Arts L1; Courage; Dodge (+2.5 cm); Natural Born Warrior; Immunity (Shock); Mimetism (-3); Specialist Operative; Tactical Awareness; Stealth; NWI.

| Profile ID | SWC | Points | Weapons |
|---|---:|---:|---|
| 777-1-1 | 0 | 39 | Mk12; Chain-colt; Heavy Pistol; T2 CC Weapon (PS=6) |
| 777-1-2 | 1 | 42 | AP Spitfire; Chain-colt; Heavy Pistol; T2 CC Weapon (PS=6) |

### Streloks, Kazak Reconnaissance Unit

**Unit ID:** 1126  
**Slug:** `streloks`  
**AVA:** 2  
**Troop type:** LI  
**Classification:** Specialist Trained Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 16 | 11 | 11 | 13 | 1 | 0 | 1 | 2 |

**Skills:** Surprise Attack (-3); Camouflage; Forward Deployment (+20 cm); Mimetism (-3); Decoy (1); Stealth.

| Profile ID | SWC | Points | Weapons | Difference |
|---|---:|---:|---|---|
| 1126-1-2 | 0 | 24 | T2 Marksman Rifle; AP Mine; Pistol; CC Weapon | BS=12 |
| 1126-1-3 | 0 | 16 | SMG; Chain-colt; AP Mine; Pistol; CC Weapon | — |
| 1126-1-4 | 0 | 25 | SMG; Chain-colt; AP Mine; Pistol; CC Weapon | Includes K-9 Antipode |
| 1126-1-7 | 0 | 17 | Boarding Shotgun; AP Mine; Flash Pulse; Pistol; CC Weapon | Forward Observer |

#### K-9 Antipode included by `1126-1-4`

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-15 | 20 | 10 | 15 | 13 | 0 | 0 | 1 | 5 |

**Skills:** Peripheral (Synchronized); Surprise Attack (-3); Camouflage; Forward Deployment (+20 cm); Dodge (+5 cm); Mimetism (-3); Sensor; Stealth; Climbing Plus.  
**Included option `1126-2-1`:** Tactical Bow (PS=5), Trench-Hammer (PS=5), AP CC Weapon (PS=5); source 9 points, disabled standalone.

### Remontnikbot V-5 Elektronik

**Unit ID:** 1581  
**Slug:** `remontnikbot-v-5-elektronik`  
**AVA:** 2  
**Troop type:** REM  
**Classification:** Support Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | STR | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 10 | 8 | 9 | 12 | 0 | 0 | 1 | 1 |

**Skills:** Courage; Mimetism (-3); Peripheral (Servant).  
**Loadout `1581-1-1`:** 2 points / 0 SWC — PARA CC Weapon (-3); `minis: 0`; generates no Order.

### Rokots

**Unit ID:** 1518  
**Slug:** `rokots`  
**AVA:** 2  
**Troop type:** LI  
**Classification:** Line Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 10 | 11 | 13 | 1 | 0 | 1 | 2 |

**Skills:** Courage.

| Profile ID | SWC | Points | Weapons | Skills / differences | Flags |
|---|---:|---:|---|---|---|
| 1518-1-4 | 0 | 9 | SMG; Grenades; Pistol; D-Charges; CC Weapon | — | — |
| 1518-1-6 | 0 | 10 | SMG; Grenades; Flash Pulse; D-Charges; Pistol; CC Weapon | Forward Observer | Specialist |
| 1518-1-7 | 0 | 11 | SMG; Grenades; Pistol; CC Weapon | Paramedic; MediKit | Specialist |
| 1518-1-8 | 0 | 12 | Rifle; Light Shotgun; Pistol; CC Weapon | Infiltration; Camouflage (1 Use) | — |
| 1518-1-9 | 0 | 10 | SMG; Grenades; D-Charges; Pistol; CC Weapon | Infiltration; Camouflage (1 Use) | — |
| 1518-1-10 | 0 | 9 | SMG; Grenades; D-Charges; Pistol; CC Weapon | Lieutenant | Lieutenant |

### 7th Foxtrot Rangers “Newport”

**Unit ID:** 235  
**Slug:** `foxtrot-rangers`  
**AVA:** 1  
**Troop type:** SK  
**Classification:** Specialist Trained Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 11 | 13 | 13 | 0 | 0 | 1 | 2 |

**Skills:** Surprise Attack (-3); Camouflage; Infiltration; Mimetism (-3); Stealth; Terrain (Total).

| Profile ID | SWC | Points | Weapons | Difference | Flags |
|---|---:|---:|---|---|---|
| 235-1-1 | 0 | 17 | Rifle; Shock Mine; Heavy Pistol; CC Weapon | — | — |
| 235-1-2 | 0 | 17 | Boarding Shotgun; Shock Mine; Heavy Pistol; CC Weapon | — | — |
| 235-1-7 | 0.5 | 20 | Sniper Rifle; Shock Mine; Heavy Pistol; CC Weapon | — | — |
| 235-1-8 | 0 | 18 | Rifle; Flash Pulse; Shock Mine; Heavy Pistol; CC Weapon | Forward Observer | Specialist |
| 235-1-9 | 2 | 17 | Rifle; Shock Mine; Heavy Pistol; CC Weapon | Lieutenant | Lieutenant |

### Kazak Doktor

**Unit ID:** 243  
**Slug:** `kazak-doktor`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Support Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 11 | 11 | 13 | 1 | 0 | 1 | 2 |

**Skills:** Doctor.  
**Equipment:** MediKit.  
**Loadout `243-1-1`:** 12 points / 0 SWC — Rifle, Pistol, CC Weapon.

### Colonel Yevgueni Voronin

**Unit ID:** 768  
**Slug:** `col-yevgueni-voronin`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Character

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 22 | 11 | 12 | 14 | 0 | 0 | 1 | 4 |

**Skills:** Martial Arts L2; Guard; Sixth Sense; Sensor; Counterintelligence; Combat Instinct.

| Profile ID | SWC | Points | Weapons | Skills / flags |
|---|---:|---:|---|---|
| 768-1-1 | 0 | 18 | Light Shotgun (+1B); Flash Pulse; Pistol; AP CC Weapon (PS=5) | — |
| 768-1-2 | 0 | 22 | Light Shotgun (+1B); Flash Pulse; Pistol; AP CC Weapon (PS=5) | Lieutenant (+1 Command Token); Strategos L1 |

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
**Loadout `1847-1-1`:** 9 points / 0 SWC — SMG, D-Charges, Pistol, CC Weapon; GizmoKit; named `CHERNOBOG PILOT`.

### 4éme de Chasseurs

**Unit ID:** 252  
**Slug:** `chasseurs`  
**AVA:** 2  
**Troop type:** SK  
**Classification:** Specialist Trained Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 11 | 13 | 13 | 0 | 0 | 1 | 2 |

**Skills:** Surprise Attack (-3); Camouflage; Infiltration; Mimetism (-3); Sixth Sense; Stealth; Terrain (Total).

| Profile ID | SWC | Points | Weapons | Difference | Flags |
|---|---:|---:|---|---|---|
| 252-1-1 | 0 | 19 | Rifle; Light Flamethrower; Shock Mine; Pistol; CC Weapon | — | — |
| 252-1-3 | 0 | 20 | Rifle; Adhesive Launcher Rifle; D-Charges; Pistol; CC Weapon | — | — |
| 252-1-4 | 0.5 | 20 | Rifle; Light Flamethrower; Shock Mine; Pistol; CC Weapon | Minelayer | — |
| 252-1-5 | 0 | 20 | Rifle; Light Flamethrower; Flash Pulse; Shock Mine; Pistol; CC Weapon | Forward Observer | Specialist |

### 45th Highlanders Rifles “Galwegian”

**Unit ID:** 239  
**Slug:** `45th-highlanders-rifles`  
**AVA:** 4  
**Troop type:** WB  
**Classification:** Line Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 22 | 10 | 14 | 14 | 1 | 0 | 1 | 2 |

**Skills:** Berserk (+3); Courage; Dogged; Impetuous; No Cover; Dodge (+5 cm).  
**Characteristics:** Irregular, Impetuous.

| Profile ID | SWC | Points | Weapons |
|---|---:|---:|---|
| 239-1-1 | 0 | 10 | Rifle; Smoke Grenades; Pistol; AP CC Weapon (PS=5) |
| 239-1-2 | 0 | 5 | Chain Rifle; Smoke Grenades; Pistol; AP CC Weapon (PS=5) |
| 239-1-3 | 0 | 10 | Boarding Shotgun; Smoke Grenades; Pistol; AP CC Weapon (PS=5) |

### 112, Emergency Service

**Unit ID:** 255  
**Slug:** `112-emergency-service`  
**AVA:** 2  
**Troop type:** LI  
**Classification:** Support Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 16 | 11 | 12 | 13 | 0 | 0 | 1 | 2 |

**Skills:** Doctor; Courage.  
**Equipment:** MediKit.  
**Loadout `255-1-1`:** 11 points / 0 SWC — Light Shotgun, Boarding Pistol, CC Weapon; source name `112 FTO`. The pinned vanilla Fireteam chart does not list this unit.

### Dynamo Regiment of Kazak Light Cavalry

**Unit ID:** 1134  
**Slug:** `dynamo`  
**AVA:** 2  
**Troop type:** LI  
**Classification:** Specialist Trained Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 20-10 | 15 | 12 | 12 | 13 | 1 | 0 | 1 | 4 |

**Base weapon:** Mine Dispenser (Shock).  
**Skills:** Dodge (+2.5 cm); Dogged; Courage; Impetuous; Mimetism (-3); Limited Cover.  
**Equipment:** Motorcycle.

| Profile ID | SWC | Points | Weapons | Difference |
|---|---:|---:|---|---|
| 1134-1-4179 | 0 | 14 | SMG; Panzerfaust; Smoke Grenade Launcher; Boarding Pistol; CC Weapon | — |
| 1134-1-4180 | 1 | 25 | AP Spitfire; Smoke Grenade Launcher; Boarding Pistol; CC Weapon | — |
| 1134-1-4182 | 0.5 | 16 | Boarding Shotgun; Smoke Grenade Launcher; Boarding Pistol; CC Weapon | Paramedic; MediKit |

### Konduktors, Transtartaric Railway Troops

**Unit ID:** 1844  
**Slug:** `konduktors-transtartaric-railway-troops`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Garrison Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 15 | 10 | 11 | 12 | 1 | 0 | 1 | 2 |

| Profile ID | FTO | SWC | Points | Weapons | Skills / differences |
|---|---|---:|---:|---|---|
| 1844-1-1 | yes | 0 | 7 | Chain Rifle; Light Shotgun; Shock Mine; Pistol; CC Weapon | — |
| 1844-1-2 | yes | 0 | 16 | Shock Marksman Rifle; Pistol; CC Weapon | BS=12 |
| 1844-1-3 | no | 0 | 12 | Rifle; Chain-colt; Flammenspeer; Pistol; CC Weapon | Camouflage (1 Use); Infiltration |
| 1844-1-4 | yes | 0 | 10 | Rifle; Pistol; CC Weapon | Paramedic; MediKit |

The pinned vanilla Fireteam chart does not expose a Konduktor slot despite these FTO labels.

### Dog-Warriors

**Unit ID:** 242  
**Slug:** `dog-warriors`  
**AVA:** 2  
**Troop type:** WB  
**Classification:** Support Troops

#### Dogface form

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-10 | 21 | 10 | 14 | 12 | 1 | 0 | 3 | 2 |

**Skills:** Courage; Super-Jump; Impetuous; Immunity (ARM); No Cover; Transmutation (1); Berserk; Dodge (+2.5 cm).

#### Dog-Warrior form

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-10 | 23 | 10 | 16 | 12 | 3 | 3 | 3 | 6 |

**Skills:** Courage; Super-Jump; Impetuous; Immunity (ARM); No Cover; Berserk; Dodge (+2.5 cm).

**Loadout `242-1-837`:** 21 points / 0 SWC — Chain Rifle (+1B), Grenades (PS=6), Smoke Grenades, AP CC Weapon (PS=4). Generates 1 Irregular + 1 Impetuous Order.

### Warcors, War Correspondents

**Unit ID:** 50  
**Slug:** `warcors-war-correspondents`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Mercenary Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 11 | 9 | 11 | 13 | 0 | 0 | 1 | 2 |

**Skills:** Journalist.  
**Characteristics:** Irregular.

| Profile ID | SWC | Points | Weapons | Difference |
|---|---:|---:|---|---|
| 50-1-1 | 0 | 3 | Flash Pulse; Stun Pistol; PARA CC Weapon (-3) | 360º Visor |
| 50-1-2 | 0 | 3 | Flash Pulse; Stun Pistol; PARA CC Weapon (-3) | Sixth Sense |

### Zenit-7 Detachment

**Unit ID:** 1519  
**Slug:** `zenit-7-detachment`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Elite Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 12 | 10 | 13 | 2 | 0 | 1 | 2 |

**Skills:** Surprise Attack (-3); BS Attack (Shock); Camouflage; Mimetism (-3); Decoy (1); Stealth; BS Attack (SR-1).

| Profile ID | SWC | Points | Weapons | Difference | Flags |
|---|---:|---:|---|---|---|
| 1519-1-2 | 0.5 | 25 | AP Marksman Rifle; Pistol; CC Weapon | — | — |
| 1519-1-3 | 0.5 | 30 | AP Marksman Rifle; Pistol; CC Weapon | Chain of Command | Specialist |
| 1519-1-4 | 1 | 27 | AP Sniper Rifle; Light Shotgun; Pistol; CC Weapon | Forward Observer | Specialist |

### Irmandinhos

**Unit ID:** 240  
**Slug:** `irmandinhos`  
**AVA:** 2  
**Troop type:** WB  
**Classification:** Line Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 21 | 10 | 14 | 13 | 1 | 0 | 1 | 2 |

**Skills:** Booty; Engineer; Impetuous; No Cover.  
**Equipment:** Deactivator.  
**Characteristics:** Irregular, Impetuous.

| Profile ID | SWC | Points | Weapons |
|---|---:|---:|---|
| 240-1-2 | 0 | 8 | Chain Rifle; D-Charges; Smoke Grenades; Pistol; AP CC Weapon (PS=6) |
| 240-1-3 | 0 | 14 | Boarding Shotgun; D-Charges; Smoke Grenades; Pistol; AP CC Weapon (PS=6) |

### Desperadoes

**Unit ID:** 752  
**Slug:** `desperadoes`  
**AVA:** 2  
**Troop type:** WB  
**Classification:** Specialist Trained Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 20-10 | 21 | 11 | 13 | 13 | 1 | 0 | 1 | 4 |

**Skills:** Courage; Dodge (+2.5 cm); Sixth Sense; Impetuous; Mimetism (-3); No Cover.  
**Equipment:** Motorcycle.  
**Characteristics:** Irregular, Impetuous.

| Profile ID | SWC | Points | Weapons |
|---|---:|---:|---|
| 752-1-2570 | 0 | 7 | Chain Rifle; Smoke Grenade Launcher; Smoke Grenades; Heavy Pistol (+1B); AP CC Weapon (PS=7) |
| 752-1-2571 | 0 | 7 | Chain Rifle; Smoke Grenade Launcher; Smoke Grenades; Assault Pistol (+1B); Shock CC Weapon (PS=7) |
| 752-1-2572 | 0 | 9 | Boarding Shotgun; Smoke Grenade Launcher; Smoke Grenades; Heavy Pistol (+1B); AP CC Weapon (PS=7) |

### Dozers, Field Engineers

**Unit ID:** 256  
**Slug:** `dozers-field-engineers`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Support Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 11 | 11 | 13 | 1 | 0 | 1 | 2 |

**Skills:** Courage; Engineer.  
**Equipment:** Deactivator; GizmoKit.

| Profile ID | SWC | Points | Weapons | Equipment difference |
|---|---:|---:|---|---|
| 256-1-1 | 0 | 13 | Rifle; D-Charges; Pistol; CC Weapon | — |
| 256-1-3 | 0 | 14 | Rifle; Blitzen; D-Charges; Pistol; CC Weapon | — |
| 256-1-4 | 0 | 14 | Rifle; D-Charges; Pistol; CC Weapon | Deployable Cover |
| 256-1-5 | 0 | 15 | Rifle; D-Charges; Armed Turret (Rifle); Pistol; CC Weapon | — |

### Brigadier Jacques Bruant

**Unit ID:** 262  
**Slug:** `brigadier-jacques-bruant`  
**AVA:** 1  
**Troop type:** LI  
**Classification:** Character

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 15 | 13 | 11 | 13 | 2 | 0 | 1 | 2 |

**Common skills:** Mimetism (-3); Specialist Operative; Stealth; Terrain (Total).  
**Equipment:** X-Visor.  
**Source note:** troops with Infiltration cannot be part of a Fireteam.

| Profile ID | FTO | SWC | Points | Weapons | Skills / differences | Flags |
|---|---|---:|---:|---|---|---|
| 262-1-1 | yes | 1 | 28 | AP Spitfire; Chain-colt; D-Charges; Heavy Pistol; CC Weapon | — | Specialist |
| 262-1-2 | no | 1 | 33 | AP Spitfire; Chain-colt; D-Charges; Heavy Pistol; CC Weapon | Surprise Attack (-3); Camouflage (1 Use); Infiltration | Specialist; cannot join FT |
| 262-1-3 | yes | 1 | 28 | AP Spitfire; Chain-colt; D-Charges; Heavy Pistol; CC Weapon | Lieutenant | Lieutenant, Specialist |

### Kibervolk Patrol

**Unit ID:** 1843  
**Slug:** `kibervolk-patrol`  
**AVA:** 1 patrol  
**Classification:** Compound unit

**Source note:** a Kibervolk Patrol is composed of **1 Kibervolk and 1 Dozer KVP**, and both must belong to the same Combat Group. Source relations enforce the pairing.

#### Dozer KVP

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-10 | 14 | 11 | 11 | 13 | 1 | 0 | 1 | 2 |

**Skills:** Courage; Engineer.  
**Equipment:** Deactivator; GizmoKit.

| Profile ID | SWC | Points | Weapons |
|---|---:|---:|---|
| 1843-1-1 | 0 | 11 | Light Shotgun; D-Charges; Pistol; CC Weapon |
| 1843-1-2 | 0 | 14 | Light Shotgun; D-Charges; Armed Turret (Rifle); Pistol; CC Weapon |
| 1843-1-3 | 0 | 12 | SMG; D-Charges; Pistol; CC Weapon |

#### Kibervolk

| MOV | CC | BS | PH | WIP | ARM | BTS | STR | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 15-15 | 21 | 2 | 15 | 13 | 1 | 0 | 1 | 5 |

**Skills:** CC Attack (+1B); Courage; Dodge (+5 cm); Mimetism (-3); Sensor; Dogged.  
**Equipment:** Biometric Visor.

| Profile ID | SWC | Points | Weapons |
|---|---:|---:|---|
| 1843-2-1 | 0 | 10 | Chain-colt; Trench-Hammer (PS=4); Shock CC Weapon (PS=4) |
| 1843-2-2 | 0 | 12 | Chest Mine; CrazyKoala; Trench-Hammer (PS=4); Shock CC Weapon (PS=4) |

### Barsuk, Territorial Defense Regiment

**Unit ID:** 1845  
**Slug:** `barsuk-territorial-defense-reg`  
**AVA:** 2  
**Troop type:** MI  
**Classification:** Garrison Troops

| MOV | CC | BS | PH | WIP | ARM | BTS | W | S |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 10-5 | 15 | 11 | 11 | 12 | 3 | 0 | 1 | 2 |

**Skills:** Immunity (Shock).

| Profile ID | FTO | SWC | Points | Weapons | Skills / differences |
|---|---|---:|---:|---|---|
| 1845-1-1 | yes | 0 | 10 | Heavy Flamethrower; Light Shotgun; Pistol; CC Weapon | — |
| 1845-1-2 | yes | 0 | 19 | AP Marksman Rifle (PS=6); Pistol; CC Weapon | BS Attack (Shock) |
| 1845-1-3 | no | 0 | 12 | Heavy Flamethrower; Light Shotgun; Pistol; CC Weapon | Forward Deployment (+20 cm) |
| 1845-1-4 | no | 0 | 11 | Heavy Flamethrower; Light Shotgun; Pistol; CC Weapon | Camouflage (1 Use); Decoy |
| 1845-1-5 | no | 0 | 19 | AP Marksman Rifle (PS=6); Pistol; CC Weapon | Camouflage (1 Use); Decoy |
| 1845-1-6 | no | 0 | 12 | Thunderbolt; Pistol; CC Weapon | Camouflage (1 Use); Decoy |

## Optional game-mode units

These source entries are available to Ariadna game modes but are excluded from the 51-unit standard-roster count.

### Intel Spec-Ops

**Unit ID:** 1915  
**Slug:** `intel-spec-ops`  
**AVA:** 1  
**Mode skill:** Infinity Spec-Ops

The pinned source exposes an initial MI profile (MOV 10-10, CC14, BS12, PH12, WIP13, ARM2, BTS0, W1, S2), an enhanced Full Power HI profile (MOV 15-5, CC20, BS13, PH11, WIP14, ARM5, BTS0, W2, S2), a Battle Ravaged profile, six selectable Intel loadouts (18–27 points, 0–1 SWC), B2M SpecBot options, and Spec-Ops upgrade tables. Preserve the source's Spec-Ops tables rather than treating them as ordinary standard-roster loadouts.

### Ariadna Team-Ops

**Unit ID:** 1929  
**Slug:** `ariadnateam-ops`  
**Mode skill:** Infinity Team-Ops

The pinned source exposes Intel-1, Intel Heavy and B2M SpecBot groups with their dedicated Team-Ops options and upgrade tables. These are mode-specific constructs and are not counted as normal Vanilla Ariadna roster units.

## Fireteams

The `fireteamChart` object is authoritative. The older top-level `fireteams` array is empty in the pinned source and does not override the chart.

### FT-01 — Ariadna Fireteams I

**Types:** Duo  
**Source name:** `Ariadna Fireteams I`  
**Wildcard team:** no

| Member | Unit ID | Required | Min | Max | Counts as | FTO restriction | Allowed loadout IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Dynamo | 1134 | no | 0 | 2 | — | — | all | — |
| Loup-Garou | 247 | no | 0 | 2 | — | — | all | — |
| Briscard | 260 | no | 0 | 2 | — | — | all | — |
| Frontovik | 1136 | no | 0 | 1 | — | — | all | — |
| Veteran Kazak | 234 | no | 0 | 1 | — | — | all | — |
| Ratnik | 1127 | no | 0 | 1 | — | — | all | — |
| Chernobog | 1584 | no | 0 | 1 | — | — | all main Chernobog loadouts | Ancillary remote is included, not a separate member |
| Irmandinho | 240 | no | 0 | 1 | — | — | all | — |
| Highlander | 239 | no | 0 | 2 | — | — | all | 45th Highlanders Rifles |
| Varangian | 1461 | no | 0 | 2 | — | — | all | — |
| Kazak Doktor | 243 | no | 0 | 1 | — | — | all | — |
| Dog-Warrior | 242 | no | 0 | 1 | — | — | all | — |
| Colonel Voronin | 768 | no | 0 | 1 | — | — | all | — |
| Brigadier Bruant FTO | 262 | no | 0 | 1 | — | FTO | `262-1-1`, `262-1-3` | Infiltrating profile `262-1-2` cannot join |

### FT-02 — Ariadna Fireteams II

**Types:** Duo, Haris  
**Source name:** `Ariadna Fireteams II`  
**Wildcard team:** no

| Member | Unit ID | Required | Min | Max | Counts as | FTO restriction | Allowed loadout IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Frontovik | 1136 | no | 0 | 2 | — | — | all | — |
| Loup-Garou | 247 | no | 0 | 2 | — | — | all | — |
| Briscard | 260 | no | 0 | 2 | — | — | all | — |
| Apache FTO | 1757 | no | 0 | 1 | — | FTO | `1757-1-1`, `1757-1-2`, `1757-1-3` | Non-FTO profiles 5 and 7 excluded |
| Barsuk FTO | 1845 | no | 0 | 1 | — | FTO | `1845-1-1`, `1845-1-2` | Non-FTO profiles 3–6 excluded |
| Moblot | 233 | no | 0 | 1 | — | — | all | — |
| Veteran Kazak | 234 | no | 0 | 1 | — | — | all | — |
| Brigadier Bruant FTO | 262 | no | 0 | 1 | — | FTO | `262-1-1`, `262-1-3` | Infiltrating profile `262-1-2` cannot join |

## Unit → Fireteam access index

| Unit | Fireteam | Type | Access | Counts as | Profile restriction | Min/Max | Notes |
|---|---|---|---|---|---|---|---|
| Dynamo | FT-01 | Duo | native | — | all | 0–2 | — |
| Loup-Garou | FT-01; FT-02 | Duo; Duo/Haris | native | — | all | 0–2 in each | — |
| Briscard | FT-01; FT-02 | Duo; Duo/Haris | native | — | all | 0–2 in each | — |
| Frontovik | FT-01; FT-02 | Duo; Duo/Haris | native | — | all | 0–1 / 0–2 | — |
| Veteran Kazak | FT-01; FT-02 | Duo; Duo/Haris | native | — | all | 0–1 | — |
| Ratnik | FT-01 | Duo | native | — | all | 0–1 | — |
| Chernobog | FT-01 | Duo | native | — | main loadouts | 0–1 | — |
| Irmandinho | FT-01 | Duo | native | — | all | 0–1 | — |
| 45th Highlanders Rifles | FT-01 | Duo | native | — | all | 0–2 | Source member label `HIGHLANDER` |
| Varangian Guard | FT-01 | Duo | native | — | all | 0–2 | — |
| Kazak Doktor | FT-01 | Duo | native | — | all | 0–1 | — |
| Dog-Warriors | FT-01 | Duo | native | — | all | 0–1 | — |
| Colonel Voronin | FT-01 | Duo | native | — | all | 0–1 | — |
| Brigadier Jacques Bruant | FT-01; FT-02 | Duo; Duo/Haris | native | — | FTO profiles `262-1-1`, `262-1-3` | 0–1 | Infiltrating profile excluded |
| Apaches | FT-02 | Duo/Haris | native | — | FTO profiles `1757-1-1`, `1757-1-2`, `1757-1-3` | 0–1 | — |
| Barsuk | FT-02 | Duo/Haris | native | — | FTO profiles `1845-1-1`, `1845-1-2` | 0–1 | — |
| Moblots | FT-02 | Duo/Haris | native | — | all | 0–1 | — |

All standard-roster units not listed in this reverse index have no access in the pinned vanilla Ariadna Fireteam chart.

## Reinforcement Fireteams — L'Équipe Argent

Linked Reinforcement army: **L'Équipe Argent (Army ID 399)**, source revision `7.26246.158`.

These rows are intentionally separate from the standard Vanilla Ariadna chart. Reinforcement Fireteam limits in the pinned source are **Core 1; Haris 1; Duo 1**.

### RFT-01 — Reinf. Loup-Garou Reinforcement Fireteams

**Types:** Duo, Haris, Core

| Member | Required | Min | Max | Notes |
|---|---|---:|---:|---|
| Loup-Garou REINF | no | 1 | 5 | Native Reinforcement team |

### RFT-02 — Reinf. Briscards Reinforcement Fireteams

**Types:** Duo, Haris, Core

| Member | Required | Min | Max | Notes |
|---|---|---:|---:|---|
| Briscard REINF | no | 1 | 4 | Native Reinforcement team |

### Reinforcement Wildcards

| Unit | Max | Counts as / restriction | Notes |
|---|---:|---|---|
| Moblot REINF | 2 | — | Wildcard |
| Apache REINF | 2 | Loup-Garou | Wildcard |
| 112 FTO REINF | 1 | — | Wildcard |
| Brigadier Bruant REINF | 1 | Briscards | Wildcard |
| Wolfgang Amadeus REINF | 1 | Loup-Garou, Briscards | Wildcard |

Main and Reinforcement troopers are not merged by this reference; no source exception was found permitting cross-chart Fireteam composition.

## Provenance

- Corvus Belli Army source revision: `7.26246.158`
- Army data changed on: 2026-09-03
- Source snapshot repository: `massayoshi/infinity-army-backup`
- Source snapshot commit: `d4329bb596ffea5d568eb2435f74366c305a7630`
- Vanilla Ariadna source: `n5/ariadna/ariadna.json` / current snapshot content for revision `7.26246.158`
- Linked Reinforcement source: `n5/l-equipe-argent/7.26246.158.json`
- InfinityDB identity/reference baseline: `4e2662be3f43387fbae42b3790a711b3e98570c4`
- Generated and verified: 2026-10-15

### Validation notes

1. Standard-roster membership is selected from source units whose `factions` includes Army ID `301`; generic mercenary catalogue records with `factions: []` are excluded.
2. The standard roster contains 51 logical units; Intel Spec-Ops and Ariadna Team-Ops are recorded separately as optional-mode hooks.
3. Standard unit loadouts, profile IDs, points and SWC in this file are transcribed from the pinned structured source.
4. Compound-unit source restrictions are preserved for Antipode Assault Pack, Mirage-5, Polaris Team, Chernobog/Samodelkin, Strelok K-9 and Kibervolk Patrol.
5. The canonical vanilla Fireteam chart is preserved from `fireteamChart`: Core 0, Haris 1, Duo 2, with two source team rows.
6. Apache, Barsuk and Brigadier Bruant FTO restrictions are resolved to exact loadout IDs.
7. The top-level source `fireteams: []` field is not treated as overriding the non-empty `fireteamChart` object.
8. The linked L'Équipe Argent Reinforcement chart is kept separate from the main vanilla chart.

## Command-unit apex/value cross-reference (2026-10-23)

**Voronin LT 22/0 Strategos L1/Counterintelligence/Sensor** is extremely affordable flexible command; **Wallace LT 38/0 Inspiring Leadership** is better when several genuinely **Irregular** attackers become Regular. **Wallace CoC 38/0** is a *different non-LT fighter* and does **not** regularize the army until succession. **TankHunter CoC 25/0 Minelayer** offers protected camouflaged succession, while **Vassily CoC 39** adds a gun/midfield role at higher cost. Morat Warhorse does not transfer to Ariadna.

See [cross-game Lieutenant, Chain of Command and Order-package tiers](../../notes/list-building/command-units-apex-and-value.md). **Use this roster/Fireteam chart above for exact legality.**

## Mission specialist / button-pusher choices (N5.3)

**Strelok FO17/0** with Camo/FD+20/Decoy(1) is among the cheapest **midfield objective openers**; **Dynamo/other biker specialists** are faster lateral closers but more exposed. **TankHunter CoC25/0** combines concealed succession, Minelayer and Specialist access; **Vassily LT+FO35** is an alternate Camo/Decoy(2) command scoring asset but do not risk a vital LT merely for a console. Pair Doctor/paramedic/Engineer from legal roster for actual medical/tech Classifieds.

[Cross-game apex and value specialist tier guide](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). The unit profiles/Fireteams above control exact legality.

## Airborne / enemy-DZ attack profile choices (2026-10-23)

**Van Zant AP Rifle33/0 or T2 BSG35/0** is reliable *enemy-DZ Parachutist(DZ)* with **TA, Dogged and MA3**, excellent for 2+ exposed Order/support kills; **Mirage-5 Margot+Duroc60/2** is a compound **two-body** DZ pressure package (1 Regular +1 Irregular + Margot TA + Impetuous), not two generic Regular Orders. **Strelok/Chasseur camo** gives safer midfield deployment when edge screens are heavy. **Wallace CoC/LT** are different on-table choices; do not assign them direct airborne attack. Count actual enemy CoC/Warhorse before hunting Lt.

[Cross-game N5.3 airborne and DZ-attack apex/value tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **Pinned profiles and the canonical Fireteam chart above govern legality.**

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **Spetsnaz Camo HMG36/1.5** combines Marksmanship/Mimetism(-3)/Surprise for a cheap **non-TAG** anti-Cover first shot; it has only 1W and lacks AP for top armor. **Veteran Kazak AP HMG45/1.5** instead buys robust NWI/Warhorse and **nonhackable AP** sustained attacks. **Chernobog** is a separate **TAG** multi-STR/TacAware AP breakthrough for the bigger investment, while **Van Zant/Mirage** are alternative rear-attack delivery pieces avoiding frontal FtF rather than extra HMGs. [Separate TAG and non-TAG ratings](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## Warbands and inexpensive trading roles — N5.3

**Galwegian Chain5** availability must be checked on Vanilla roster; **Irmandinho Engineer+Smoke+Chain8/0** is an unusually cheap useful specialist/trader, **Desperado bike Chain+Smoke GL7/0** is extreme lateral speed, **Dog-Warrior21/0** buys durability and **PH-based grenade Speculative Fire**, not just CC. **Varangian Guard 12/0 SMG+Chain+Smoke** if legal is a different Regular/Irregular order package from Kosmoflot 10pt version. **Carmen+Bâtard17/0** offers fast Smoke/Chain/paired Sensor where selected; **Mirage60/2 Duroc** is not independently purchasable as cheap warband. **Wallace LT versus CoC** options are profile-specific; don't blanket regularize Religious models.

[Cross-game warband/cheap-trader apex and value tiers, targets and command packages](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). Profile-specific sectorial legality/Fireteams above control all selections.

## TAG tactical cross-reference (2026-10-23)

**Chernobog (63 HFT / 70 HRL)** is a rare true high-ARM AP HMG chassis in Ariadna, useful when durable conventional ranged attack is missing. Its Transmutation/damage progression means judge the *remaining useful role* after a failed armor save; cheap camo specialists/warbands still need points and Orders. Ariadna cannot simply assume another faction's Repeater/Firewall support infrastructure.

For the two-tier **apex/points-value** comparison, TAG counterplay, matchup matrix and direct transcript sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Treat current profiles, points/SWC and canonical Fireteam data above as authoritative.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Only a thin standard cyber package:** the **Wardriver HD14/1 SWC** (a 16pt option brings Disco Baller) provides Carbonite/Oblivion/Spotlight, but **WIP13, few Repeaters and 1 SWC** make it a *situational counter-tech* rather than an Interventor-style net. There is **no equivalent broad native KHD network** in the pinned Vanilla roster. **Why:** Ariadna's largely non-Hackable attack pieces and cheap Camo/warbands often deny enemy hacking by simply not being legal HD targets; spend SWC on a true ranged ARO/attacker first unless the mission or enemy TAG/HI makes a Wardriver's cyber effect worth more.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

Cross-faction [apex and cost-value Order-generator rankings](../../notes/list-building/cheerleaders-and-order-generators.md), circumstance guide and transcript disagreements. **This file remains authoritative for profiles, AVA, Training and Fireteam legality.**

- Line Kazak — S2 baseline Regular Order with table-defense/decoy benefits; its cheapest loadout beats passive expensive guns.
- Warcor — Irregular Flash Pulse ARO distraction, NOT a passive transferable Regular Order.
- Baggage — prioritize a legal 8pt basic bot if actually on roster, remembering its large base.

**When to pick:** Prefer transferable, safe Regular Orders when the Combat Group needs fuel; choose the higher-priced option only when its smoke, template, weapon, repeater, Fireteam function or scoring ability has a real job. Do not count Irregular/Impetuous/Tactical/Lieutenant Orders or Peripheral bodies as interchangeable Regular pool Orders; account for DZ footprint and link/enabler package costs.


## ARO apex/value cross-reference (2026-10-23)

See [ARO units: N5.3 apex/value tiers, hidden-versus-visible and deployment/matchups](../../notes/list-building/aro-units-apex-and-value.md). The **current profile details here** control exact cost/SWC, Training and Fireteam eligibility; do not import another faction's link or specialist upgrades.

- **Cateran T2/AP Sniper (21pt)** — camouflaged long-range trade-up to HITAG, Irregular status: no transferable pool Order
- **Tankhunter Camo ML/Panzerfaust/Autocannon** — hidden-information threat and serious anti-armor; Minelayer closes approach, 1W/expensive gun remains fragile
- **Chasseur Camo/Minelayer** — midfield hidden-information and mine trap; better at limiting route than direct sniper duels
- **Uragan Guided/TR** — low-cost reactive volume that can be recovered; compare with cheap Dozer and spotter infrastructure
- **Traktor Mul support** — rare Ariadna cheap reload/guided/total-reaction choices; only buy a real Guided program if FO route is viable

**Choose by circumstance:** a hard long gun matters only when the opponent must cross its arc; cheaper mines, Camo markers, templates, Flash, DTWs and hacking force movement or risk without committing an entire attack plan. Budget a second layer and preserved counterattack, check pie-slicing, hidden Order cost, anti-visual bypass and repair routes.

## N5.3 midfield area denial / speed bumps (tactical synthesis)

**Scout Ohotnik + E/M Mine Minelayer (2) 28/.5** creates two Camo/infiltrated anti-HI/TAG crossing hazards before activation. **Chasseur 20/.5 Shock Mine Minelayer with Light Flamethrower** is the cheaper cornerguard; **Strelok SMG 16/0 Camo/Decoy + AP Mine** contributes uncertainty and a cheap body but **does not have Minelayer**, so laying its own mine costs an Order. **Foxtrot FO 18/0** is the scoring alternative, also without Minelayer. Choose multiple cheap screens versus one Scout depending on available routes, Sensor/Deactivator opponents and objective coverage.

[Whole-game midfield denial, profile and matchup tiers](../../notes/list-building/midfield-area-denial-and-speed-bumps-apex-value.md).

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Irmandinho8** packs Engineer, Smoke, Chain Rifle and disruption for exceptional 8pt **trader/support value**, but its Irregular/Impetuous orders and exposed approach do not replace a protected mechanic. **Dozer13 WIP13 + Remontnik2** is the low-cost reliable physical route to **Chernobog/REM** recovery. **112 Doctor11 or motorized19** gives VITA recovery; most No-Cube patients cannot spend a Command Token to reroll a failed Doctor, so 65% must be treated honestly. [Doctor/Engineer recovery odds and tier guide](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## N5.3 DZ defense / anti-alpha-strike tactical choices

**Warcor 360º 3/0** gives an inexpensive *Irregular* Flash ARO against rear-edge/Combat Jump; **Chasseur Shock Minelayer+Light Flamethrower 20/.5** can cover the *midfield-to-DZ corridor* while also being an infiltrating Camo problem. **Traktor Mul Baggage/Deactivator 5/0** supplies a cheap Regular logistics Order and can help counter mines, but **not a true sentry** or 360º guard. **Counter:** a 3pt Warcor alone will not stop Van Zant/Hellcat from taking an entire clustered support line; cross-cover a corner with a close-template guard and physically separate the Doctors/Order fillers. Buying too many Irregular speed bumps can undercut the active-turn pool.

[Whole-game DZ-defender apex/value guide, counters and transcripts](../../notes/list-building/dz-defenders-alpha-strike-and-impersonation-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Van Zant33–35/0** reaches an **enemy-DZ edge** and can finish an isolated target with AP+T2 CC, but its value is *entry + gunfire*, not a true MA5 duel. **Galwegian5/0** brings Irregular Smoke + AP CC22 to tie up expensive gunmen cheaply; **Dog-Warrior21** moves 15-10 and brings Berserk/Smoke and greater resilience. **S.A.S.** infiltrating mines/shotguns suppress victim support first. Against enemy NBW/Guard, use grenades/templates and range: a cheap warband does not automatically win a TAG assassination just because CC is possible. [Close-combat apex/value, positioning and counter-CC](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Beasthunter9 Panzerfaust+HFT** or **Dynamo14 Panzerfaust+Smoke GL** are cheap counter-threats; **Dozer14 Blitzen** buys Engineer plus ranged E/M. **TankHunter AP HMG33/1.5** is best reusable B4 armor can-opener, **Portable Autocannon(+1B)36/1.5** stronger AP+EXP per uncancelled hit, **TankHunter AP SMG+Panzerfaust+FD24/.5** is a multi-modal midfield trap. **Ratnik46 AP Spitfire+Panzerfaust/TacAware** is a high-cost repeated attack; no faction-wide Hacker dependency. [Non-hacking armor-killer value rankings and tactical matchups](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## Tactical cross-reference — indirect fire (2026-10-23)

**Conditional artillery:** **Traktor Guided Katyusha9/1, Uragan Guided+Total Reaction14/1**, with 5pt Baggage option separately. Cheap FO (Chasseur/Strelok/other eligible trooper) should score and set Targeted before spending extra SWC on the missile. Dog-Warrior/other PH-grenade models instead attack safely via **Speculative B1** with no Targeted setup. This list has thinner Spotlight/Repeater coverage than Nomads: a dedicated multi-piece hacker network can be worse than durable physical pressure. [Full apex/value comparison](../../notes/list-building/indirect-fire-speculative-guided-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Objective holders by job:** **Unknown Ranger Specialist/Tactical Awareness39/0** (Mimetism-3, W1+NWI, ARM4, T2, mobile) is a resilient 39VP center; **Veteran Kazak FO36/0** (where roster permits) W1+NWI/Mimetism/IMM-B/Warhorse carries box under cover. **S.A.S. FO21/0** and **Chasseur FO20/0** are inexpensive Infiltration/Camo pickup pieces, but cannot remain markers once carrying. **Ratnik HRL41/1.5 / AP Spitfire46/1.5**, full W2/ARM6/transmutation, gives non-Specialist VP mass to a zone; **Dog-Warrior/Ioann/McMurrough** hold/contest with wounds and Smoke but may be Irregular/Impetuous and normally cannot pick up as Specialists. **Counter:** Ariadna cannot replace good scenario positioning with hacker threats; several separate infiltrating specialists + 5pt Smoke screens often preserve scoring more reliably than one expensive non-Specialist hull.

[Cross-game objective holder and zone-domination apex/value tiers, scenario rules, and opposing transcript reviews](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Exact profiles/Fireteams above are authoritative.

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Antipode Assault Pack and K-9 / other rostered fast Sensor bodies** are the main **Camo/Hidden** search plan: physical speed is what gets the +6 WIP ZoC effect where it matters; **Voronin LT Sensor** can cover home lines without using a fragile elite gun. **Smoke, fast flankers and templates** are often Ariadna's more economical answer to an opposing **MSV2/Mimetism** hard ARO than paying multiple Orders for a weak straight BS contest. **Kibervolk Biometric+Sensor** has rarer anti-IMP utility where the precise profile is legal. **Tradeoff:** Sensor reveals, but still requires a follow-up attack; do not assume a Sensor user can directly attack an IMP marker as if Camouflaged.

[Non-hacking & tech-specific counter-selection, N5.3 anti-tech apex/value and opposing MCP transcripts](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## N5.3 peripheral / synchronized / multi-body apex-value update

**Best Control/scout package:** **Antipode Handler26/0 + three Antipodes** (included) is **one Regular+one Tactical Awareness Order** for **3× MOV15-15 Camo/Sensor/CC20/AP+Super-Jump** attacking via **one chosen Spearhead** per target Skill. 4 bases ≠ 4 pooled Orders or 3 full independent melee attacks; Handler behind terrain/Smoke while fast pack scours midfield. **Strelok K-9 SMG+K-9 25/0** = Camo/FD+20 **synchronized K-9 Sensor/Climbing+** split-angle, whereas **Strelok FO17/0 has no dog**. **Polaris Alpha32/0 (Masha+Bearpode) = TWO independently generated Regular Orders**, unlike Control/Synchronized; Beta40/0 likewise, both bodies same Combat Group. **Opposing:** Antipode26 handles Camo, CC and Order economy better per point than Polaris32 on midfield sweep; Polaris has actual independent action/guns and hard W2 Bearpode, ideal when needing second body to shoot separately.

[Cross-game multi-body apex/value and transcript disputes](../../notes/list-building/peripheral-synchronized-multibody-apex-value.md). Current sectorial roster and N5.3 rules decide actual type and access.

## Battle-report effectiveness and combinations (qualitative, 2026-11-01)

**Observed effective engine:** The CanCon 2026 winning build featured **Voronin + two Strelok FO/Decoy + two Tankhunter autocannon threats + Scout E/M Minelayer**, backed by **Dynamo AP Spitfire/Paramedic Duo**, Dozer/Baggage and disposable Order/mission bodies. Decoy placement around hidden Tankhunters made opponents spend attention and Orders on false identities; Dynamos converted access into mission actions. [#161](../../notes/battle-reports/161-170-n5-battle-report-tactical-analysis.md), [#237](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md) are **the same champion/event**, not independent repetitions.

**Independent corroboration:** #223 shows **William Wallace** as an actual anti-materiel Corporate Appropriation finisher (and CoC), while a Tankhunter punished a split-Burst Unknown Ranger; Van Zant's counterstrike damaged but failed to destroy the target. #210 demonstrates that a **Bearpode** can spend many Orders for a cheap REM trade even when the Tankhunter contributes strongly. [#210](../../notes/battle-reports/201-210-n5-battle-report-tactical-analysis.md) · [#223](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md).

**Practical build:** Treat Tankhunter as denial/long-gun, Strelok/Scout as marker- and E/M-pressure, Dynamo/Wallace as mission conversion; do not assume **Mirage-5 or Van Zant** were present in the champion's actual played lists just because available in vanilla.

[Cross-report synthesis and evidence cautions](../../notes/battle-reports/cross-report-unit-effectiveness-and-combinations.md).

## Mission performance — battle-report evidence (2026-11-01)

| Mission(s) | Tested composition / scoring mechanism | Evidence |
|---|---|---|
| **Provisioning / Crossing Lines / Area of Interest / Hardlock** | Voronin + Strelok FO/Decoy + Tankhunter/Scout E/M with fast Dog Warrior/Dynamo/Kövlk/Sasha scoring and screens. | [#161](../../notes/battle-reports/161-170-n5-battle-report-tactical-analysis.md), [#237](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md) |
| **Corporate Appropriation** | Wallace destroys prototype in CC; Dynamo smoke + Sasha can retrieve/extract another way. | [#223](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md), [#237](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md) |

**Limits:** #161/#237 describe one CanCon winner; round five involved a consequential rules error. Available Mirage-5/Van Zant are not proof of being fielded. Game-era qualitative evidence, not a win-rate or N5.3 Fireteam claim. [Full cross-report mission synthesis](../../notes/battle-reports/cross-report-mission-performance-by-sectorial.md).

## Counterplay — observed N5 battle-report responses (2026-11-02)

| Threat / target | Observed response, timing and consequence | Battle reports |
|---|---|---|
| **TAG / elite HI** | Scout E/M mine isolated/IMM'd Marut LT and Dog Warriors/Galwegian attacked after the screen in a conceded CanCon Crossing Lines round; Tankhunter autocannons punish exposed armor. | [#237](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md), [#223](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) |
| **Hacking grids / hidden defense** | Non-Hackable Camo Strelok/Scout/Tankhunter and decoys force Discover while Dynamo smoke/Sasha bypasses exposed Cutter to complete Corporate; focus mission rather than hackable gun duel. | [#161](../../notes/battle-reports/161-170-n5-battle-report-tactical-analysis.md), [#237](../../notes/battle-reports/231-240-n5-battle-report-tactical-analysis.md) |
| **Impersonator / DZ striker** | Mines/Koala and layered rear guard forced arriving Van Zant to spend route resources; he killed Voronin but failed to destroy objective after taking too many defenses. | [#223](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) |

**Limit:** #161 and #237 are the same event; a #237 round has a consequential rules issue, and Van Zant #223 belongs to USAriadna opponent, not vanilla roster used. These are game-era actions, not current N5.3 profile/Fireteam legality or faction win rates. [Cross-report counterplay analysis](../../notes/battle-reports/n5-cross-report-counterplay-tags-hi-hacking-camo-impersonators-fireteams.md).

---

## Must-have / Go-to / Avoid — source-backed recommendations (2026)

Dated source-backed tactical preferences and collection priorities; opinions do not override N5.3 roster, profile or Fireteam data above.

**Original audit title:** Ariadna — Vanilla, USAriadna, TAK, Kosmoflot, Caledonia, FRRM: Must-have / Go-to / Avoid

*Source-backed list-building audit — 23 October 2026. Covers all six standard Ariadna armies under **N5.3** using the current repository [sectorial references]() (Army `7.26246.158`, data dated 3 September 2026; verified 15 October 2026). Video/podcast views are **named-player tactical opinions and example army lists**, not measured tournament pick rates. The latest `main` roster, AVA, profiles and canonical Fireteam chart control over recordings, especially those predating the October 2025 balance update.*

**Companion guides:** [Vanilla](../../notes/factions/vanilla-ariadna.md) · [USAriadna](../../notes/factions/usariadna.md) · [Kosmoflot](../../notes/factions/kosmoflot.md) · [Caledonia](../../notes/factions/caledonia.md) · [FRRM](../../notes/factions/merovingienne.md). TAK currently relies on its [current sectorial reference](tartary-army-corps.md) and the recordings listed below.

### Classification and evidence standards

- **Must-have / near-must:** repeated first-choice inclusion across independently built example lists, or an explicit reviewer “always / most lists / auto-include” judgment. **Near-must is not universal:** a role can be indispensable without any one profile being mandatory.
- **Go-to:** repeatedly attractive price/role efficiency. Not all go-to units belong in the same 300-point list; missions, fire lanes, SWC, Orders and competing packages decide.
- **Never take / strong avoid:** a directly stated negative review of a **specific profile or construction**, ideally with a viable same-roster alternative. Use **conditional** or **contested** if the profile has a niche, there is dissent or the source is pre-rework. There is **no evidenced blanket ban on an entire Ariadna unit family**.
- **Evidence:** **explicit** = specific presenter says so; **repeat** = multiple independently constructed sample lists; **reasoned** = synthesis of recorded strengths/weaknesses plus current reference, **not** a claimed quotation.
- A recorded list choice alone does not prove “most players” use a unit. Transcripts may mangle Ariadna proper names, so check names and legality against the current repository. The standard lists here do **not** import `L'Équipe Argent` Reinforcements, which have separate charts.

### Quick comparison

| Army | Closest near-must | Most strongly supported avoidance |
|---|---|---|
| Vanilla Ariadna | Dynamo AP Spitfire + Paramedic Duo | No unconditional exclusion established |
| USAriadna Ranger Force | Foxtrot specialist / Minelayer, cheap Desperado smoke | Wild Bill as routine Fireteam filler; Grunt sniper as *sole* serious ARO |
| Tartary Army Corps | Dynamo mobility + TankHunter ambush | Pavel as general-purpose value pick (contested); Konduktor as a Strelok replacement |
| Kosmoflot | Mirage-5, Patcher support | Redundant premium frontal guns; Wallace without Irregular-economy benefit |
| Caledonia | Uxía/SAS midfield, Cameronians | Premium assault-role duplication; Wallace in a largely Regular build |
| FRRM / Mérovingienne | Moblot + economical Métros | Infiltrating Bruant, especially costly Bruant + Zouave NCO order package |

### 1. Vanilla Ariadna

[Current roster / Fireteams](vanilla-ariadna.md) · [Detailed faction guide](../../notes/factions/vanilla-ariadna.md)

**Near-must**

| Piece | Why; limit | Evidence |
|---|---|---|
| **Dynamo AP Spitfire + Paramedic Duo** (**41 pts / 1.5 SWC**) | Fast AP gun, mobile objective specialist, Smoke and two Shock Mine Dispensers. Can lay mines to force an ARO fork, then attack from a favorable angle; a 5pt Traktor can replenish disposable equipment. **Closest thing to a general Vanilla default**, but Limited Cover and exposed bike paths can punish mistakes. | [Robert Shepherd — TAK Faction Focus (2026)](https://www.youtube.com/watch?v=eM5cM_Y18vk) directly praises Dynamos in **TAK and Vanilla**; [Tactical Awareness Ariadna SOUP](https://open.spotify.com/episode/3WYxtimNdXjHDsMOWvEWw6) takes Dynamo Duos; [WIP12 Ariadna with Logan](https://open.spotify.com/episode/1Crhc3Ma9WS4OoxmH6BnFi) calls them dependable. **Explicit + repeat.** |

**Go-to**

| Piece | Why; when to choose | Evidence |
|---|---|---|
| **TankHunter portable autocannon** | Camouflage + powerful anti-ARM reactive/ambush shooting. Select high-value reveals, not every trivial ARO. | [Loss of Lieutenant #164 — CanCon winning Vanilla](https://open.spotify.com/episode/0X4QIoP24cKONtltxClHMH); [Vanilla SOUP](https://open.spotify.com/episode/3WYxtimNdXjHDsMOWvEWw6). |
| **Strelok Decoy / Minelayer** | Makes the TankHunter/Scout marker shell costly to Discover and flank; midfield mines and disguise remain useful without constant Orders. | LoL #164 and the [existing Vanilla guide](../../notes/factions/vanilla-ariadna.md). |
| **Vystrel Neurocinetics** | Sapper and dangerous reactive long-range gun cover the lanes the bikes do not. Favor on open tables or when the primary active gun is midrange. | [Tactical Awareness TAK](https://open.spotify.com/episode/2VCGfZZhXpth6ahryGhPyw), [Vanilla guide](../../notes/factions/vanilla-ariadna.md). |
| **Col. Voronin LT + Wallace CoC** | Strategos/Counterintelligence command tempo with a CoC safety net and secondary close attacker. **60-point combined commitment** is too costly for some mission-first builds. Current Vanilla Wallace is **not** an LT option. | LoL #164; Vanilla guide; current reference. **Reasoned from recorded command approach.** |
| **Dog-Warrior / Polaris** | Independent Smoke, heavy close-range disruption and PH-based Speculative Fire behind terrain; Polaris adds a separate multi-model Regular-order package. | LoL #164; Vanilla guide. |
| **Mirage-5; alternatively Van Zant** | Threatens rear/DZ approach and changes enemy deployment even if not fielded; choose by intended attack/specialist mission. | [Tactical Awareness Vanilla SOUP](https://open.spotify.com/episode/3WYxtimNdXjHDsMOWvEWw6); LoL #164. Hosts disagree about optimal raider. |
| **Kibervolk Patrol** | Compact Dozer KVP + Kibervolk package for Engineer, Sensor, counter-CC and deployable DZ defense. **Bundled patrol**, not independently selected models; **Kibervolk does not have Climbing Plus**. | LoL #164; current reference; Vanilla guide records Shepherd's acknowledged Climbing Plus error. |
| **Traktor Mul Baggage** | 5pt Regular Order, Deactivator and reload service for Mine Dispensers/disposables. Bring if the table has room for an S4 support base. | [WIP12 Ariadna](https://open.spotify.com/episode/1Crhc3Ma9WS4OoxmH6BnFi); TA Vanilla. |

**Avoid / contested:** No video or podcast establishes a universal “never take” profile. **Chernobog as a default over multiple camo/mission assets** is an *architecture trade-off*, not a ban: it supplies ARM8/AP HMG/Tactical Awareness but is large, hackable and expensive. Some TA presenters prefer stronger sectorial Fireteams, while Shepherd's CanCon 2026 results support a Vanilla independent-threat package. Do **not** conclude Shepherd fielded Mirage-5/Van Zant in his winning lists; his reported value included the *threat* of these pieces.

### Direct media evidence queue

The links below are audit sources; a recording's publication date is essential when evaluating pre/post-update opinions.

| Scope | Primary recordings and direct use |
|---|---|
| **Vanilla** | [Tactical Awareness S3E11 — Ariadna SOUP (24 Feb 2025)](https://open.spotify.com/episode/3WYxtimNdXjHDsMOWvEWw6), three independent lists and skepticism about Vanilla; [WIP12 E185 — Ariadna with Logan (13 May 2025)](https://open.spotify.com/episode/1Crhc3Ma9WS4OoxmH6BnFi), Dynamos and practical roles; [Loss of Lieutenant #164 — Shepherd CanCon winner (7 Feb 2026)](https://open.spotify.com/episode/0X4QIoP24cKONtltxClHMH), tournament-tested defensive shell/command choices. |
| **USAriadna** | [Tactical Awareness S3E08 (30 Jan 2025)](https://open.spotify.com/episode/4wIT3UwMB9LldCtHdfLU6k), early-N5 three-list comparison and Devil Dog dissent; [Shepherd USARF (pre-October 2025)](https://www.youtube.com/watch?v=mqNiL2ziIkU); [Swiss Miss N5 USARF Tier List (post-Oct 2025)](https://www.youtube.com/watch?v=AboAGci9_9A), updated unit tier ratings including Wild Bill/Grunt/Desperado critiques. |
| **TAK** | [Shepherd TAK Faction Focus (2026)](https://www.youtube.com/watch?v=eM5cM_Y18vk), Dynamos, TankHunters, Veteran Kazaks, Ratnik skepticism; [WIP12 E203 with Copper (15 Apr 2026)](https://open.spotify.com/episode/0fLvDDDa2baw7lxt3J4qo9), current good/bad/ugly plus explicit Pavel debate and Konduktor-versus-Strelok; [TA S3E09 (3 Feb 2025)](https://open.spotify.com/episode/2VCGfZZhXpth6ahryGhPyw), sample lists/Vystrel. |
| **Kosmoflot** | [Tactical Awareness S3E10 (10 Feb 2025)](https://open.spotify.com/episode/0FZYrBdbYi3bNLX0Xbdl3l) / [YouTube](https://www.youtube.com/watch?v=ceoF3KoyaaM), three independent Mirage-5 inclusions and differing support/Fireteam shells. Early N5 profile claims must be checked against September 2026 Army reference. |
| **Caledonia** | [Tactical Awareness S3E38 (27 Oct 2025)](https://open.spotify.com/episode/4WgaVJBlbSm3wHIsBPPsWb), Wallace/Cameronian concepts; [Ryanj4043 — N5 CHA Faction Review (2026)](https://www.youtube.com/watch?v=iyKGgFUA1JA), scope/role coverage, explicit Wallace optionality; [Loss of Lieutenant E158 (28 Oct 2025)](https://open.spotify.com/episode/1pQ6J6OGpzyu8QlxiFoo8D). |
| **FRRM** | [WIP12 E197 with Logan (26 Nov 2025)](https://open.spotify.com/episode/3YNuQVF24bJmCGdxL1FjK5) / [YouTube](https://www.youtube.com/watch?v=GmVfuKSIkXg), direct Moblot/Metro/Anaconda positives and Bruant/Zouave negatives; [Tactical Awareness S3E39](https://open.spotify.com/episode/2Pqi3i2SyoSGyKciy7r2gD) / [YouTube](https://www.youtube.com/watch?v=VROiGibXnEs), counterexamples; [Loss of Lieutenant E157 (18 Oct 2025)](https://open.spotify.com/episode/1lq0RhEWwpegXr1kkKJzUr), competitive alternative interpretations. |

**Audit result:** The source standard supports many **go-to** recommendations, a handful of **near-must** packages, and only a few serious **strong avoids** (especially FRRM). A mission-dependent, disputed, or pre-rework negative comment is **not** evidence for a universal “never take.” This distinction is deliberate and should survive future refreshes.

### Whole-unit purchasing audit — full-unit shopping skips (2026-10-30)

The old avoid section mostly rates **profiles, pairings and list architecture**, not entire units. **No source-backed absolute all-profile ban** exists across these six rosters. Here are only defensible **conditional whole-model deferrals**.

| Army | Entire model/unit buying decision | Why / exception |
|---|---|---|
| **Vanilla Ariadna** | **No verified whole-unit avoid** | Chernobog versus several camo/scoring pieces is a costly **architecture**, but its ARM8/AP HMG/Tactical Awareness has a distinct heavy-attack purpose. |
| **USARF — Wild Bill** | **Defer as generic Grunt-team add-on; conditional** | [Swiss Miss USARF](https://www.youtube.com/watch?v=AboAGci9_9A) says the expensive, short-range and fragile package is hard to justify. Buy only for a **planned close-quarter pistol delivery**; don't extrapolate this to Wild Bill in another sectorial. |
| **TAK** | **No verified whole-unit avoid** | Strong objections concern excess premium shooters or specific team arrangements, not a model whose every profile fails its job. |
| **Kosmoflot** | **No verified whole-unit avoid** | Wallace with too few Irregulars and a second expensive gun team are poor **build choices**, not universal model bans. |
| **Caledonia** | **No verified whole-unit avoid** | Premium Wulver Core overload and Wallace without an Irregular economy are situational packages. |
| **FRRM — Brigadier Jacques Bruant** | **Defer if buying solely for the default midfield gun/LT-order combo** | [WIP12 E197](https://open.spotify.com/episode/3YNuQVF24bJmCGdxL1FjK5) is strongly negative on expensive single-Wound infiltrating Bruant and his paired **Zouave NCO** engine. A specific surprise line or command plan can still pay off; not a proved all-profile ban. |
| **FRRM — generic Zouave** | **Do not mark whole unit avoid** | Expensive FTO FO/Paramedic/Panzerfaust are criticized but **Sapper** and unusual mission cases are positively defended by a presenter in the same source. |

**Shopping principle:** do not translate “avoid a Bruant + Zouave NCO *package*” into “neither miniature is ever worth owning.” [Cross-faction buying shortlist](../../notes/factions/model-purchase-avoid-summary-2026.md).

### Worst, uncommon and proxy-first purchases by sectorial (2026-10-30)

**Scope and confidence.** This answers a different question from the unit-role tables above: **“Which whole miniature can I skip buying, which uncommon specialist should I proxy until I actually use it, and which *bad profile* should I avoid without rejecting its whole unit?”** An **AVA limit is not a shopping target**. Video/podcast reviews are **opinion and illustrative lists, not tournament selection-frequency data**; “uncommon” means **not a normal first purchase in these reviewed builds**, not measured rare usage. The latest [N5.3 roster]() and its **Fireteam, silhouette, peripherals and availability** rules override old recordings.

**Buying labels:**
- **Skip by default; proxy if needed:** the **normal whole-model job** has explicit negative commentary or an unusually weak price/role comparison. The exception is recorded; **no Ariadna model is proven mathematically useless in every scenario**.
- **Proxy first:** a full unit with a credible specialty, but you should establish *a specific list and mission use* before buying its sculpt; this is an **inferred shopping recommendation**, not a presenter's alleged quotation.
- **Avoid profile only:** the unit has legitimate alternate profiles. **Never extrapolate to all its miniatures.**
- **One enough / proxy the extra:** owning/fielding multiple is an elective skew rather than a default; distinguish genuine duplicate bodies from alternate loadout sculpts. **Contested** flags genuine source disagreement or tournament examples.

#### 1. Vanilla Ariadna

| Weak, niche or redundant purchase | Why the default purchase is questionable | Miniature decision |
|---|---|---|
| **Chernobog TAG as an automatic centerpiece** | **Contested:** 63–70pt heavy ARM8/AP HMG/TacAware can win open lanes, but S7, hacking vulnerability, degraded state, costly repair and specialist shortage compete against **multiple TankHunters, Dynamo Duo, Scouts/Streloks and a Dog-Warrior**. [Vanilla analysis](../../notes/factions/vanilla-ariadna.md) documents LoL #142 B-versus-C debate. | **Proxy/test first** with a suitable TAG-sized model. **Not a worst unit** if your army deliberately wants the armoured attack plan. **Do not buy a second** solely because TAG alternative lists exist. |
| **Ratnik or Veteran Kazak as an extra generic solo heavy gun** | **Contested / cross-TAK role comparison:** they provide armour and distinctive link/weapon roles but compete against efficient camo ambush pieces; Ratnik can degrade. The Veteran has strong independent uses in suitable teams. | **Proxy the *additional* heavy infantry**, not an outright full-unit avoid. Especially avoid multiple premium attackers all consuming the same active-turn Orders. |
| **Brigadier Jacques Bruant as an expensive infiltrating gun** | **Direct criticism transfers only to this role:** WIP12 FRRM explains the 1W, one-use Camo/AP Spitfire investment often loses to cheaper specialist/marker coverage. Vanilla has yet more independent camo alternatives. | **Proxy first / skip normal dedicated purchase**. A surprise angle or his other eligible loadout can still earn value; **do not mistake an FRRM FTO Fireteam for a Vanilla right**. |
| **Kuryer/Traktor Guided artillery as a default missile investment** | **Conditional:** cheap **Traktor Baggage5** is excellent; **Katyusha/Uragan Guided** requires real **Targeted** setup and Orders. Vanilla lacks a free high-grade network; premium TankHunter/Vystrel AROs may be better. | **Avoid the artillery *loadout* by default, not the Traktor chassis**. Use a correctly sized existing REM as a Guided test; no second dedicated artillery model merely for one weapon configuration. |
| **Knauf or another third long-range dedicated sniper** | **Inference from role overlap:** **TankHunter**, **Vystrel**, **Cateran** and sniper-capable camo troops already make multiple reactive threats. Knauf's MSV1/Mimetism may be unique in a particular matchup, but does not score by itself. | **Proxy first** if the additional shooter serves no new anti-visor/LoF requirement. Same principle applies to extra Vystrels/TankHunters purchased solely to fill AVA. |
| **Wallace + Voronin command suite when not using it** | **Build error, not weak models:** ~60pt combined commitment can be useful as command insurance/economy, but Vanilla can also use cheap LT + independent threats. Wallace in Vanilla is **CoC**, not a standard Vanilla LT. | **Proxy whichever *new* character is missing until the exact succession/order plan is tested**. Keep Voronin/Wallace if already owned for their other legal roles. |
| **112 Motorized and second specialty bike outside a mobile scoring list** | **Inference:** 19pt Doctor bike/Smoke provides recovery, but an **active Dynamo + Paramedic** package already gives high-speed mission work. No blanket assertion that a Doctor and Paramedic are functionally identical. | **Proxy extra** motorized medic/biker before buying a duplicate; if the Doctor's *actual* recovery rules matter, he is worthwhile. |
| **Mirage-5, Van Zant, Polaris/Kibervolk compound teams** | **Not bad units:** each has major off-board attack, Smoke/bear pressure or two-body DZ-control value, but a **distinct physical team/partner** and Order/points commitment. An army will rarely require *all* these options at once. | **Proxy/test whichever *additional* package you are not already using**, with separately represented partners. Prioritize dedicated sculpts only for a recurring tactic; do **not** treat absence from a particular winning list as evidence they are weak. |

**Evidence:** [Loss of Lieutenant #164 tournament Vanilla](https://open.spotify.com/episode/0X4QIoP24cKONtltxClHMH), [Tactical Awareness Vanilla SOUP](https://open.spotify.com/episode/3WYxtimNdXjHDsMOWvEWw6), [Vanilla guide](../../notes/factions/vanilla-ariadna.md), [FRRM WIP12 Bruant criticism](https://open.spotify.com/episode/3YNuQVF24bJmCGdxL1FjK5). **Do not skip** first useful **Dynamo**, **Strelok**, **TankHunter**, **Scout**, **Vystrel** or **Traktor Baggage** based on a criticism of their *other loadouts*.

#### Cross-Ariadna miniature substitutions — buying versus proxying (including owned TAK figures)

There are two very different reasons to proxy: **(A) weak or infrequent overall use** (Wild Bill, infiltrating Bruant, certain Pavel/Ratnik roles), and **(B) a good model whose existing equivalent, alternate sculpt or *second copy* would be an unnecessary purchase** (TankHunter guns, character FO, Dog-Warrior variants). The following recommendations are **inferred from the roster and reported ownership**; none pretends to be a speaker's exact words.

| Proposed dedicated purchase | Proxy-first recommendation | Purchase threshold and cautions |
|---|---|---|
| **Another TAK TankHunter/Scout/Strelok, Kazak Spetsnaz or extra premium Frontovik/Veteran** | Reuse an **unused camo soldier** or **spare Line Kazak/Frontovik/HI** of the correct **silhouette/base**, e.g., your existing **Ariadna Spec-Ops** proxy. Keep the role visually identifiable. | Buy additional sculpt **only** when you use two differently named troopers *simultaneously* and have enough properly distinguishable models. You already reported **3 TankHunters, 2 Scouts, 1 Strelok, 2 Spetsnaz**. |
| **Pavel, Vassily, Sāchā, character/FO/Doctor variants** | **Owned Pavel and Vassily**; use a distinct specialist/camo model for an occasional named variant where appropriate. Your **existing HVT for Sāchā** is already a reported proxy; a **Dozer/Kazak Doktor** can test **foot 112** if its size and visual role can be made unambiguous. | Named characters are generally AVA1 and do not need separate miniatures for every loadout. **A Kazak Doctor and a Dozer are not functionally interchangeable in rules**, only candidates as declared physical proxies when not simultaneously fielded. |
| **Another Konduktor, Vystrel, Traktor/Kuryer or alternative artillery gun** | **Two owned Konduktors, two Vystrels and a two-model shared Traktor/Kuryer pool** already cover common tests. Represent **Kuryer vs Traktor** with appropriate matched REM chassis and declared profiles. | Buy a new chassis only if simultaneous bodies exceed the *physical pool* or actual silhouette/base differs; don't count two shared models as four. |
| **Second Ratnik or duplicate large armored centerpieces** | **Own one Ratnik**; test a second only with a matching **HI size/base**, never a standard S2 soldier if the silhouette differs. Use proxy TAG for Chernobog/Anaconda as appropriate. | Buy an extra expensive armored sculpt after actual repeated double-armour lists, not solely because of AVA. |
| **Dog-Warriors, Cameronians, Devil Dogs, McMurrough, Polaris, Ioann Bann, Carmen, Kibervolk** | Your **existing 2 Dog-Warriors and separate dog/Devil Dog models** can supply *one at a time* distinct large-beast proxy roles **when the actual silhouette/base matches**. For **Kibervolk**, test its complete **Kibervolk + Dozer KVP** package using appropriate spare dog and Dozer models. | **Not automatically all S5/S6 equal.** Transformed forms, peripheral counts, Masha/Bearpode/ Bâtard, and current legal unit silhouettes must all be satisfied. Do not re-use one physical dog as two simultaneous game pieces. |
| **Unknown Ranger, Foxtrot, Chasseur, SAS, Zenit-7, Mirage specialists** | Test generic compatible **TAK camo/FO** models for other sectorials and another distinctive S2 soldier for the Unknown Ranger (where allowed). Prior Ariadna expansion planning also identified **Chasseur → TAK camo** and **Kibervolk → dog + Dozer**. | Buy unique sculpts when they repeatedly feature in an army **with no proxy collision**. **Mirage-5 always needs separate Margot and Duroc representations**, even if one suitable soldier/dog is already owned. |
| **Alternative motorized 112, Dynamo, Maverick or Desperado sculpt** | Reuse a distinct **motorcycle model** from the existing two Dynamos / one 112 motorcycle where the new army legally fields it, with correct **bike/S4 base and clear declaration**. | Do not interpret the motorcycle as a standard S2 trooper or automatically treat **motorcycles as Vehicle (VH) units**. Buy more only for simultaneous bike squads or unsuitable physical geometry. |
| **Multiple Wardrivers or extra Traktor artillery purely for anti-tech/Guided** | The **one reported TAK Wardriver** and **two shared artillery chassis** can be reused in legal Ariadna rosters as clearly declared support or loadout variants. | Buy only if two simultaneous different hacker/REM models are required. A Hacking Device in one sectorial does not grant other sectorials free **Guided** access or Fireteam permission. |

**Tournament proxy policy:** Always match **current model footprint/base and Silhouette**, reveal every declared proxy to your opponent, and check the **current-season ITS and organizer rules** before bringing conversions or another faction's miniature. It is not safe to treat older season-specific event proxy wording as current 2026 policy. **A list's compound units must have all required pieces**; proxies do not create extra model counts, and an unavailable unit or illegal Fireteam remains illegal even if a physical model fits.

**Buy-order conclusion:** If already collecting TAK/Caledonia, the highest payoff normally comes from **new capabilities and missing mission roles**, not duplicating an existing TankHunter, Vystrel, dog warrior, artillery chassis or front-line HMG merely to reach AVA. **Most defensible default purchasing skips:** **USARF Wild Bill**; **FRRM infiltrating Bruant** (especially Bruant + Zouave NCO); and **TAK Pavel as an unplanned generic skirmisher**, although your Pavel is already owned. **Ratnik is contested**: you own one, so there is no reason to buy a second without a tested Mobility build. **Other good proxy-first niche models:** **Kosmoflot Wallace when Irregular conversion is unnecessary, second Chernobog or Polaris**; **Caledonia McMurrough if existing Cameronians suffice**; **FRRM Anaconda, Wolfgang or Knauf** until their particular legal list recurs. These are **not** blanket unit bans.
