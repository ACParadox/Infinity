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
