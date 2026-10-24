---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 303
sectorial_slug: force-de-reponse-rapide-merovingienne
sectorial_name: Force de Réponse Rapide Merovingienne
parent_faction: Ariadna
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Force de Réponse Rapide Merovingienne roster, standard loadouts, canonical Fireteam chart, reverse Fireteam index, and the distinct L'Équipe Argent Reinforcement Fireteam chart. Intel Spec-Ops and Ariadna Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# Force de Réponse Rapide Merovingienne

## Overview and provenance

Repository-native reference for **Force de Réponse Rapide Merovingienne (FRRM)** roster, profiles, points/SWC, AVA, and Fireteam access.

Sources used:

- Army-derived FRRM source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `d4329bb596ffea5d568eb2435f74366c305a7630`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **22-unit standard FRRM roster** and the complete standard FRRM `fireteamChart` in the pinned Army source.
- Soldier of Fortune / generic mercenary-catalog entries whose source faction list is empty are excluded from the base roster.
- `Intel Spec-Ops` and `Ariadna Team-Ops` are optional game-mode content and are listed separately.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name by itself.
- Parenthetical Army-chart comments are treated as Counts-as / equivalence labels, not as join-scope restrictions.
- The structured `required: true` rows in the FRRM Fireteam are preserved as a required-choice set; this file does not reinterpret them as requiring both Moblots and Briscards simultaneously.
- Profile restrictions are preserved: Zouaves join as Wildcards only through their `ZOUAVE FTO` profiles; Knauf joins Métros only through `KNAUF FTO`; Apaches join Loup-Garou teams only through `APACHE FTO`; and Jacques Bruant is a Wildcard only through `BRIGADIER BRUANT FTO` profiles.
- Linked Reinforcement army ID: **399**, **L'Équipe Argent**. Its Fireteam chart is recorded separately below and is not merged into the main FRRM chart.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Force de Réponse Rapide Merovingienne |
| Parent faction | Ariadna |
| Army ID | 303 |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 22 |
| Optional-mode units | Intel Spec-Ops; Ariadna Team-Ops |
| Reinforcement roster | L'Équipe Argent, Army ID `399` |
| Fireteam limits | Core 1; Haris 1; Duo unlimited |
| Fireteam chart | yes |

## Roster index

| Unit | ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| Kuryer Unit | 1524 | 2 | REM | Regular | ETB |
| Zouaves | 249 | 3 | LI | Regular | Wildcard, FTO profiles only; counts as FRRM |
| Carmen Johns & Bâtard | 1153 | 1 | WB | Irregular + Impetuous | — |
| Knauf, Outlaw Sniper | 939 | 1 | LI | Regular | Métros, FTO profile only |
| Wardrivers, Mercenary Hackers | 265 | 2 | LI | Regular | Métros |
| Anaconda, Mercenary TAG Squad | 300 | 2 | TAG | Regular + Tactical Awareness | ETB |
| Equipe Mirage-5 | 258 | 1 | HI/WB | Mixed | — |
| Loup-Garous | 247 | 5 | LI | Regular | Loup-Garou |
| Métros, Troupes Métropolitaines | 246 | TOTAL | LI | Regular | Métros |
| 112, Emergency Service (Motorized) | 1284 | 3 | LI | Regular | ETB |
| Para-Commandos | 228 | 4 | LI | Regular | — |
| 112, Emergency Service | 255 | 3 | LI | Regular | Métros; counts as Métro |
| Vystrel Mobile Artillery Regiment | 1846 | 2 | REM | Regular | — |
| Briscards | 260 | 5 | MI | Regular | FRRM required-choice; counts as FRRM |
| Moblots | 233 | 5 | HI | Regular + Tactical Awareness | Métros; FRRM required-choice; ETB; counts as Métros / FRRM |
| Dozers, Field Engineers | 256 | 2 | LI | Regular | — |
| Warcors, War Correspondents | 50 | 1 | LI | Irregular | — |
| Apaches | 1757 | 2 | WB | Regular | Loup-Garou, FTO profiles only; counts as Loup-Garou |
| Traktor Mul | 257 | 2 | REM | Regular | — |
| Chasseurs | 252 | 4 | SK | Regular | — |
| Brigadier Jacques Bruant | 262 | 1 | LI | Regular | Wildcard, FTO profiles only; counts as Métros / FRRM |
| Wolfgang Amadeus Wolff | 1555 | 1 | WB | Regular | Wildcard; counts as Loup-Garou / FRRM |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Intel Spec-Ops | 1915 | Spec-Ops | Métros Fireteam row, max 1 when Spec-Ops mode is in use |
| Ariadna Team-Ops | 1929 | Team-Ops | No ordinary FRRM Fireteam row |

## Unit details

### Kuryer Unit

**ID 1524 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 9 | WIP 12 | ARM 2 | BTS 0 | W 1 | S 4`. Baggage, ECM: Guided (-6), Remote Presence, Courage, Minelayer, BS Attack (Guided), Warhorse.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 15 | 1 | Katyusha MRL, Chest Mine, Shock Mine, PARA CCW; BS Attack (-3) | ETB max 1 |
| 2 | 18 | 1 | Uragan MRL, Chest Mine, Shock Mine, PARA CCW; Total Reaction | ETB max 1 |

### Zouaves

**ID 249 · AVA 3 · LI** — `MOV 15-5 | CC 16 | BS 12 | PH 11 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. Forward Deployment (+10), Dodge (+3), Dodge (+2.5), Warhorse, Dogged, Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | **ZOUAVE FTO**; AP Rifle, Panzerfaust, Assault Pistol, CCW | Wildcard max 3; FRRM |
| 2 | 22 | 0 | **ZOUAVE FTO**; AP Rifle, Panzerfaust, E/M Mine, Assault Pistol, CCW | same |
| 4 | 22 | 0 | **ZOUAVE FTO**; AP Rifle, Flash Pulse, Panzerfaust, Assault Pistol, CCW; Forward Observer | same |
| 7 | 23 | 0 | **ZOUAVE FTO**; AP Rifle, Panzerfaust, Assault Pistol, CCW; MediKit, Paramedic | same |
| 9 | 30 | 1 | **ZOUAVE FTO**; AP Spitfire, Assault Pistol, CCW; NCO | same |
| 10 | 30 | 0.5 | T2 Marksman Rifle, Shock Mine, Assault Pistol, CCW; Minelayer, Sapper | — |

### Carmen Johns & Bâtard

**ID 1153 · AVA 1 · WB** — Carmen: `MOV 20-10 | CC 22 | BS 11 | PH 13 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 4`. Motorcycle, Booty, Courage, Dodge (+5), Natural Born Warrior, Mimetism (-3), Dogged, CC Attack (-6), Limited Cover, Impetuous.

**Bâtard** — `MOV 15-15 | CC 22 | BS 0 | PH 15 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 5`. Peripheral (Synchronized), Sensor, Courage, Dodge (+5), Mimetism (-3), Dogged, CC Attack (Shock).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4264 | 17 | 0 | **CARMEN + BÂTARD**; Carmen: Chain Rifle, Smoke Grenades, Smoke Grenade Launcher, AP Heavy Pistol, DA CCW; Bâtard: Grenades, Trench-Hammer, AP CCW; Irregular + Impetuous | — |

### Knauf, Outlaw Sniper

**ID 939 · AVA 1 · LI** — `MOV 10-10 | CC 21 | BS 13 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. MSV1, BS Attack (+1B), BS Attack (Shock), Courage, Mimetism (-3), Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 31 | 1.5 | MULTI Sniper Rifle, AP Heavy Pistol, CCW; Surprise Attack (-3), Decoy (1) | — |
| 2 | 30 | 1.5 | **KNAUF FTO**; MULTI Sniper Rifle, AP Heavy Pistol, Shock CCW | Métros max 1 |

### Wardrivers, Mercenary Hackers

**ID 265 · AVA 2 · LI** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`. Sixth Sense.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 1 | Boarding Shotgun, Flash Pulse, Cybermine, Pistol, CCW; Hacking Device (Zero Pain), Hacker | Métros max 1 |
| 2 | 16 | 1 | As Opt 1 + Disco Baller | same |
| 5 | 16 | 0.5 | Combi Rifle, Pitcher, Pistol, CCW; Hacking Device, Hacker | same |

### Anaconda, Mercenary TAG Squad

**ID 300 · AVA 2 · TAG** — `MOV 15-5 | CC 21 | BS 13 | PH 16 | WIP 13 | ARM 7 | BTS 6 | W 3 | S 7`. ECM: Guided (-6), BS Attack (SR-1), Courage, Dodge (PH=11), GizmoKit (PH=11), Tactical Awareness, Transmutation (Escape System -2), Warhorse, Immunity (AP).

**Anaconda Operator** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 3 | S 2`. Courage, Specialist Operative, Tactical Awareness, Warhorse, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 59 | 1.5 | AP Spitfire, Heavy Flamethrower, Thunderbolt, DA CCW; Operator has Spitfire, Smoke GL, Boarding Pistol, CCW | ETB, 1–2 Anacondas by chart row |
| 2 | 59 | 1.5 | HMG, Light Shotgun, Panzerfaust, DA CCW; same Operator | same |

### Equipe Mirage-5

**ID 258 · AVA 1 · HI/WB** — a fixed Margot + Duroc composition.

**Lieutenant Margot Berthier** — `MOV 10-10 | CC 16 | BS 14 | PH 12 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Mimetism (-3), Parachutist (Deployment Zone), Specialist Operative, Tactical Awareness, Combat Instinct, BS Attack (Shock), Immunity (Shock, IMM-B), Terrain (Total), Dodge (+1SD), MediKit (PH=14). AP Rifle, Grenade Launcher, Light Shotgun, D-Charges, Pistol, CCW.

**Sergent Duroc** — `MOV 15-10 | CC 23 | BS 10 | PH 16 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 6`. Martial Arts L2, Courage, Dodge (+2.5), Parachutist (Deployment Zone), Super-Jump, Impetuous, Immunity (ARM), No Cover. Chain Rifle, Grenades, Smoke Grenades, AP CCW.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 60 | 2 | **EQUIPE MIRAGE-5 (MARGOT & DUROC)**; Regular + Irregular + Tactical Awareness + Impetuous | — |

### Loup-Garous

**ID 247 · AVA 5 · LI** — `MOV 10-10 | CC 16 | BS 12 | PH 11 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. X Visor, BS Attack (SR-1), Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 17 | 0 | Viral Rifle, Light Riotstopper, Smoke Grenade Launcher, Heavy Pistol, PARA CCW | Loup-Garou 1–5 |
| 2 | 15 | 0 | Boarding Shotgun, Adhesive Launcher Rifle, Heavy Pistol, PARA CCW | same |
| 6 | 24 | 1 | VIRAL Sniper Rifle, Heavy Pistol, PARA CCW; Marksmanship | same |
| 7 | 24 | 0.5 | Viral Marksman Rifle, Heavy Pistol, PARA CCW; Marksmanship | same |

### Métros, Troupes Métropolitaines

**ID 246 · AVA TOTAL · LI** — `MOV 10-10 | CC 13 | BS 11 | PH 11 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | Rifle, Pistol, CCW, Chain-colt | Métros 1–5 |
| 2 | 18 | 1 | HMG, Pistol, CCW | same |
| 3 | 10 | 0.5 | Rifle, Chain-colt, Grenade Launcher, Pistol, CCW | same |
| 4 | 12 | 0 | Rifle, Chain Rifle, D-Charges, Pistol, CCW; Surprise Attack (-3), Camouflage (1 Use), Infiltration | same |
| 5 | 13 | 0 | Rifle, Chain-colt, Panzerfaust, Pistol, CCW; same camouflage/infiltration package | same |
| 6 | 14 | 0.5 | Rifle, Chain-colt, Grenade Launcher, Pistol, CCW; same camouflage/infiltration package | same |
| 7 | 10 | 0 | Rifle, Chain-colt, Pistol, CCW; MediKit, Paramedic | same |
| 8 | 8 | 0 | Rifle, Chain-colt, Pistol, CCW; Lieutenant | same |
| 10 | 10 | 0 | Rifle, Chain-colt, Pistol, CCW; Commlink (+1), Specialist Operative | same |

### 112, Emergency Service (Motorized)

**ID 1284 · AVA 3 · LI** — `MOV 20-10 | CC 16 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 4`. Doctor, Courage, Mimetism (-3), Limited Cover, MediKit, Motorcycle.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4761 | 19 | 0 | Light Shotgun, Smoke Grenade Launcher, Smoke Grenades, Boarding Pistol, CCW | ETB max 1 |

### Para-Commandos

**ID 228 · AVA 4 · LI** — `MOV 10-10 | CC 16 | BS 12 | PH 11 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. Mimetism (-3), Parachutist, Terrain (Zero-G).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 18 | 0 | Rifle, Boarding Pistol, CCW | — |
| 4 | 29 | 1 | AP Spitfire, Boarding Pistol, CCW | — |
| 6 | 21 | 0 | Boarding Shotgun, Flash Pulse, D-Charges, Boarding Pistol, CCW; BS Attack (+1SD), Forward Observer | — |
| 8 | 19 | 0 | SMG, D-Charges, Boarding Pistol, CCW; MediKit, Paramedic | — |

### 112, Emergency Service

**ID 255 · AVA 3 · LI** — `MOV 10-10 | CC 16 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Doctor, Courage, MediKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 11 | 0 | **112 FTO**; Light Shotgun, Boarding Pistol, CCW | Métros max 1; counts as Métro |

### Vystrel Mobile Artillery Regiment

**ID 1846 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 12 | PH 9 | WIP 12 | ARM 2 | BTS 0 | W 2 | S 4`. ECM: Guided (-6), BS Attack (SR-1), BS Attack (Shock), Courage, Remote Presence, Sapper.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0.5 | AP Sniper Rifle, Light Rocket Launcher, PARA CCW | — |
| 2 | 32 | 1.5 | Portable Autocannon, Light Rocket Launcher, PARA CCW; Neurocinetics | — |
| 3 | 26 | 0.5 | AP Sniper Rifle, Light Rocket Launcher, PARA CCW; Neurocinetics | — |

### Briscards

**ID 260 · AVA 5 · MI** — `MOV 10-10 | CC 16 | BS 12 | PH 12 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. MSV1, Courage, Warhorse, Terrain (Mountain), MediKit (PH=14), Climbing Plus.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 24 | 0.5 | AP Sniper Rifle, Assault Pistol, CCW; BS Attack (Shock) | FRRM required-choice, max 5; counts as FRRM |
| 3 | 20 | 1.5 | Heavy Rocket Launcher, Assault Pistol, CCW | same |
| 4 | 22 | 0 | AP Marksman Rifle, Flash Pulse, Assault Pistol, CCW; Forward Observer | same |
| 5 | 23 | 0 | AP Marksman Rifle, Assault Pistol, CCW; MediKit, Paramedic | same |
| 6 | 26 | 0 | AP Marksman Rifle, Flash Pulse, Assault Pistol, CCW; Lieutenant (+1 Command Token), Forward Observer | same |

### Moblots

**ID 233 · AVA 5 · HI** — `MOV 10-10 | CC 16 | BS 13 | PH 12 | WIP 14 | ARM 3 | BTS 3 | W 1 | S 2`. Non-Hackable, Tactical Awareness, Mimetism (-3), BS Attack (Shock), Dodge (+1SD), Immunity (Shock, IMM-B), Terrain (Jungle), Combat Instinct, MediKit (PH=14).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 32 | 1.5 | HMG, Boarding Pistol, CCW | Métros max 2; FRRM required-choice max 5; ETB max 1; counts as Métros / FRRM |
| 3 | 27 | 0 | AP Rifle, Light Shotgun, Flammenspeer, Boarding Pistol, CCW | same |
| 7 | 31 | 0 | AP Rifle, Light Shotgun, Flammenspeer, E/M Mine, D-Charges, Boarding Pistol, CCW; Engineer, Deactivator, GizmoKit | same |
| 8 | 29 | 0 | AP Rifle, Light Shotgun, Flammenspeer, Boarding Pistol, CCW; MediKit, Paramedic | same |
| 13 | 27 | 0 | AP Rifle, Light Shotgun, Flammenspeer, Boarding Pistol, CCW; Lieutenant | same |
| 14 | 32 | 1.5 | HMG, Boarding Pistol, CCW; Lieutenant | same |
| 15 | 32 | 1.5 | AP Spitfire, Boarding Pistol, CCW | same |

### Dozers, Field Engineers

**ID 256 · AVA 2 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Engineer, Courage, Deactivator, GizmoKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 13 | 0 | Rifle, D-Charges, Pistol, CCW | — |
| 3 | 14 | 0 | Rifle, Blitzen, D-Charges, Pistol, CCW | — |
| 4 | 14 | 0 | Rifle, D-Charges, Pistol, CCW; Deployable Cover | — |
| 5 | 15 | 0 | Rifle, D-Charges, Armed Turret (Rifle), Pistol, CCW | — |

### Warcors, War Correspondents

**ID 50 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Journalist; Irregular.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW; 360º Visor | — |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW; Sixth Sense | — |

### Apaches

**ID 1757 · AVA 2 · WB** — `MOV 15-5 | CC 22 | BS 11 | PH 13 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. Frenzy, BS Attack (+1B), Courage, Dodge (+2.5), Immunity (Shock), No Wound Incapacitation, Super-Jump, CC Attack (-6), CC Attack (+1B).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | **APACHE FTO**; Rifle, Chain-colt, Heavy Pistol, AP + Shock CCW | Loup-Garou max 2; counts as Loup-Garou |
| 2 | 14 | 0 | **APACHE FTO**; Chain Rifle, Grenades, Heavy Pistol, AP + Shock CCW | same |
| 3 | 17 | 0 | **APACHE FTO**; Light Shotgun, Heavy Pistol, AP + Shock CCW | same |
| 5 | 20 | 0 | Light Shotgun, Grenades, Heavy Pistol, AP + Shock CCW; Forward Deployment (+20), Berserk | — |
| 7 | 17 | 0 | Chain Rifle, Grenades, Heavy Pistol, AP + Shock CCW; Forward Deployment (+20), Berserk | — |

### Traktor Mul

**ID 257 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 10 | PH 9 | WIP 12 | ARM 2 | BTS 0 | W 1 | S 4`. Baggage, ECM: Guided (-6), Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 5 | 0 | PARA CCW; Deactivator | — |
| 2 | 9 | 1 | Katyusha MRL, PARA CCW; BS Attack (Guided) | — |
| 3 | 14 | 1 | Uragan MRL, PARA CCW; BS Attack (Guided), Total Reaction | — |

### Chasseurs

**ID 252 · AVA 4 · SK** — `MOV 10-10 | CC 14 | BS 11 | PH 13 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Surprise Attack (-3), Camouflage, Infiltration, Mimetism (-3), Sixth Sense, Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Rifle, Light Flamethrower, Shock Mine, Pistol, CCW | — |
| 3 | 20 | 0 | Rifle, Adhesive Launcher Rifle, D-Charges, Pistol, CCW | — |
| 4 | 20 | 0.5 | Rifle, Light Flamethrower, Shock Mine, Pistol, CCW; Minelayer | — |
| 5 | 20 | 0 | Rifle, Light Flamethrower, Flash Pulse, Shock Mine, Pistol, CCW; Forward Observer | — |

### Brigadier Jacques Bruant

**ID 262 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. X Visor, Mimetism (-3), Specialist Operative, Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 28 | 1 | **BRIGADIER BRUANT FTO**; AP Spitfire, Chain-colt, D-Charges, Heavy Pistol, CCW | Wildcard max 1; counts as Métros / FRRM |
| 2 | 33 | 1 | AP Spitfire, Chain-colt, D-Charges, Heavy Pistol, CCW; Surprise Attack (-3), Camouflage (1 Use), Infiltration | — |
| 3 | 28 | 1 | **BRIGADIER BRUANT FTO**; same weapons; Lieutenant | Wildcard max 1; counts as Métros / FRRM |
| 4 | 32 | 1 | **BRIGADIER BRUANT FTO**; same weapons; Lieutenant (+1 Order) | same |

Army source note: **Troops with Infiltration cannot be part of a Fireteam.** The infiltrating Bruant profile is therefore not represented by the Wildcard FTO row.

### Wolfgang Amadeus Wolff

**ID 1555 · AVA 1 · WB** — `MOV 15-5 | CC 22 | BS 12 | PH 14 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`. Martial Arts L3, BS Attack (Continuous Damage), Berserk (+3), Courage, Dodge (+5), Dodge (+3), Immunity (ARM), Climbing Plus, Terrain (Zero-G), Frenzy, Discover (+6).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 0 | MULTI Rifle, Chain-colt, E/M Grenades, Heavy Pistol, PARA CCW, DA CCW | Wildcard max 1; counts as Loup-Garou / FRRM |

## Canonical Fireteam chart

Fireteam limits in the pinned source: **Core 1; Haris 1; Duo unlimited** (`DUO: 256` sentinel).

### Métros Fireteams

**Types:** Core, Haris

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| MÉTRO | 1 | 5 | no | — |
| MOBLOT | 0 | 2 | no | Métros |
| 112 FTO | 0 | 1 | no | Métro |
| WARDRIVER | 0 | 1 | no | — |
| KNAUF FTO | 0 | 1 | no | FTO profile only |
| INTEL | 0 | 1 | no | Spec-Ops mode only |

### Loup-Garou Fireteams

**Types:** Core, Haris

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| LOUP-GAROU | 1 | 5 | no | — |
| APACHE FTO | 0 | 2 | no | Loup-Garou; FTO profiles only |

### FRRM Fireteams

**Types:** Core, Haris, Duo

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| MOBLOT | 0 | 5 | yes | FRRM |
| BRISCARD | 0 | 5 | yes | FRRM |

The two `required-choice` rows form the FRRM required-choice set; they are not interpreted as requiring both troop types simultaneously.

### ETB (Équipes Táctiques Blindées) Fireteams

**Types:** Duo

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| ANACONDA | 1 | 2 | no | — |
| 112 MOTORIZED | 0 | 1 | no | — |
| MOBLOT | 0 | 1 | no | — |
| TM KURYER | 0 | 1 | no | — |

### Wildcards

| Entry | Max | Counts as / profile restriction |
|---|---:|---|
| ZOUAVE FTO | 3 | FTO profiles only; FRRM |
| BRIGADIER BRUANT FTO | 1 | FTO profiles only; Métros, FRRM |
| WOLFGANG AMADEUS | 1 | Loup-Garou, FRRM |

Wildcards use the global Wildcard row of the FRRM chart and may join otherwise eligible FRRM Fireteams, subject to the chart and the profile restrictions above.

## Reverse Fireteam access index

| Unit / profile | Fireteam access | Counts as / restriction |
|---|---|---|
| 112 FTO | Métros | Métro |
| 112 Motorized | ETB | Max 1 |
| Anaconda | ETB | Native row; 1–2 Anacondas |
| Apache FTO | Loup-Garou | FTO profiles only; Loup-Garou |
| Briscards | FRRM | Required-choice; FRRM |
| Brigadier Bruant FTO | Wildcard | FTO profiles only; Métros, FRRM |
| Intel Spec-Ops | Métros | Optional Spec-Ops mode only |
| Knauf FTO | Métros | FTO profile only |
| Kuryer | ETB | Max 1 |
| Loup-Garou | Loup-Garou | Native 1–5 row |
| Métro | Métros | Native 1–5 row |
| Moblot | Métros; FRRM; ETB | Métros max 2; FRRM required-choice; ETB max 1; counts as Métros / FRRM |
| Wardriver | Métros | Max 1 |
| Wolfgang Amadeus | Wildcard | Loup-Garou, FRRM |
| Zouave FTO | Wildcard | FTO profiles only; max 3; FRRM |

All standard roster units not listed in this reverse index have no Fireteam access in the pinned standard FRRM chart.

## Reinforcement Fireteams — L'Équipe Argent

Linked Reinforcement army: **L'Équipe Argent (Army ID 399)**, source revision `7.26246.158`.

These rows are intentionally separate from the standard FRRM chart. Reinforcement Fireteam limits in the pinned source are **Core 1; Haris 1; Duo 1**.

### Loup-Garou Reinforcement Fireteams

**Types:** Core, Haris, Duo

| Entry | Min | Max | Counts as / note |
|---|---:|---:|---|
| LOUP-GAROU REINF | 1 | 5 | — |

### Briscards Reinforcement Fireteams

**Types:** Core, Haris, Duo

| Entry | Min | Max | Counts as / note |
|---|---:|---:|---|
| BRISCARD REINF | 1 | 4 | — |

### Reinforcement Wildcards

| Entry | Max | Counts as / profile restriction |
|---|---:|---|
| MOBLOT REINF | 2 | — |
| APACHE REINF. | 2 | Loup-Garou |
| 112 FTO REINF | 1 | — |
| BRIGADIER BRUANT REINF | 1 | Briscards |
| WOLFGANG AMADEUS REINF | 1 | Loup-Garou, Briscards |

Reinforcement Wildcards may join otherwise eligible L'Équipe Argent Reinforcement Fireteams, subject to the Reinforcement chart above.

## Validation notes

- Standard roster count reconciled to **22** ordinary FRRM entries after excluding `Intel Spec-Ops`, `Ariadna Team-Ops`, and generic mercenary-catalog entries.
- Every standard `fireteamChart` row from Army revision `7.26246.158` is represented, including profile-sensitive FTO joins and the FRRM required-choice set.
- The linked Reinforcement army resolves to **L'Équipe Argent (399)** and its three chart groups are preserved separately.
- Main and Reinforcement Wildcards are not merged.
- Source data and Fireteam normalization were rechecked on **2026-10-15** against the pinned Army snapshot and InfinityDB commit listed in the front matter.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Wardriver is FRRM's niche cyber counter:** the source includes **14pt/1 SWC HD+Zero Pain** for basic safe anti-heavy control and a **16pt/0.5 SWC Combi+Pitcher HD** variant. The *latter* is the more compelling network platform because it can project Repeater influence into midfield for fewer SWC; Zero Pain instead preserves an otherwise vulnerable hacker when enemy KHDs are present. **Why:** FRRM does not naturally field a dense premium Hacker/KHD suite, so its low-cost deployed specialists and conventional guns should remain the core of the plan. Use the Wardriver if the opponent brings TAG/HI or the mission rewards Spotlight; otherwise save its SWC.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

For cross-faction **apex** and **points-value** rankings, the Order types, situational counterexamples and transcript-backed disagreements, see [Cheerleaders and Order Generators — N5.3](../../notes/list-building/cheerleaders-and-order-generators.md). Roster profiles/AVA/Fireteam legality above take precedence.

- **Métros**: baseline S2 Regular pool bodies; take the cheapest useful defensive or link/specialist loadout rather than buying a weak heavy gun

**List-building test:** count *transferable* Regular Orders by Combat Group after deployment; include required link members/command enablers, physical DZ footprint, and the unit's actual ARO/mission contribution. Do not treat Irregular, Tactical, Lieutenant or Peripheral activations as interchangeable generic Orders.


## ARO apex/value cross-reference (2026-10-23)

See [ARO units: N5.3 apex/value tiers, hidden-versus-visible and deployment/matchups](../../notes/list-building/aro-units-apex-and-value.md). The **current profile details here** control exact cost/SWC, Training and Fireteam eligibility; do not import another faction's link or specialist upgrades.

- **Métro line/rocket guard** — cheap S2 defence vs deep strikes; use mines/Camo Chasseurs for actual route taxes
- **Chasseur Camo/Minelayer** — midfield hidden-information and mine trap; better at limiting route than direct sniper duels
- **Traktor Mul support** — rare Ariadna cheap reload/guided/total-reaction choices; only buy a real Guided program if FO route is viable
- **3pt Warcor Flash** — Irregular very-cheap ARO tax, not a transferable pool Order

**Choose by circumstance:** a hard long gun matters only when the opponent must cross its arc; cheaper mines, Camo markers, templates, Flash, DTWs and hacking force movement or risk without committing an entire attack plan. Budget a second layer and preserved counterattack, check pie-slicing, hidden Order cost, anti-visual bypass and repair routes.

## Warbands and inexpensive trading roles — N5.3

**Carmen Johns + Bâtard17/0** is an elite **fast Smoke+Chain+Sensor** threat and delivers anti-Camo/late lane pressure for fewer points than elite melee troops; synchronized Bâtard is **not a free separate Regular Order**. **Mirage-5 Margot+Duroc60/2** (fixed compound) provides much larger enemy-DZ template/CC attack ceiling, but it is not a 24pt standalone Duroc purchase. A **Paramedic Para-Commando19** can score after flank clearing instead of suiciding a 17pt duo. If the opponent has covered all bike lanes with mines/long guns, use a safer infiltrating midfield approach rather than forcing an expensive close attack.

[Cross-game warband/cheap-trader apex and value tiers, targets and command packages](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). Profile-specific sectorial legality/Fireteams above control all selections.

## N5.3 midfield area denial / speed bumps (tactical synthesis)

**Chasseur 20/.5 Shock Minelayer** is a genuine Camo/Infiltration speed bump with Sixth Sense, Light Flamethrower and a threatening corner; **AVA4 in FRRM**, compared with AVA2 in Vanilla Ariadna. **Chasseur 20/0 FO** scores but does not start the deployment mine; don't silently combine profiles. **Counterpoint:** too many Chasseurs create redundant mine corridors and not enough direct attack; mix clearable mines with an exposed target that is actually worth protecting.

[Cross-game apex/value, matchups, and transcript disagreements](../../notes/list-building/midfield-area-denial-and-speed-bumps-apex-value.md). Tactical evaluation, not a modification to Army profiles or Fireteam legality.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Forward-deployed/Parachutist infantry** may die outside a static deployment-zone Doctor's practical radius; favor **motorized/forward healer** where legal and safe, or treat the attacker as a planned trade. Engineer value rises only when there is a meaningful **STR Remote Presence/REM** target or hacking/E/M-state fix. Compared with raw WIP, **one covered movement order to reach contact** commonly decides whether medical support is worthwhile. [Doctor/Engineer recovery odds and tier guide](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**FRRM** primarily plays **midfield rifle/shotgun/template control**, not Shinobu-level assassination: **Chasseur19+ Camo/Infiltration CC14** gets behind screens but wins through mine/LFT positional threats, not melee; **Para-Commando18+** flanks with guns at CC16, not raw CC. **Loup-Garou17+** smoke/viral/PARA can *enable or defeat* approaching assailants. **Moblot32+** and **Zouave21+** are gunfighters/objective bodies; save points by **screening with Camo mines/Flamethrower** instead of forcing MA4/Mono matchups. [Close-combat apex/value, positioning and counter-CC](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**FRRM** has effective **Moblots/Métiers long-range guns, Loup-Garou Viral/PARA/Smoke GL**, and **Chasseur mine+LFT** positional threats, but no automatic **5pt Ghazi** or **29pt Oniwaban** equivalent in current roster. Prefer a **Panzerfaust/anti-materiel** profile where list permits, plus smoke/side angle. Against an enemy TAG, **jam its path with mines/templates** or remove its supporting Engineer; don't spend four Orders using basic Combi fire into ARM8+ Cover. Compare the current legal gun rather than importing TAK's TankHunter. [Non-hacking armor-killer value rankings and tactical matchups](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## Tactical cross-reference — indirect fire (2026-10-23)

**FRRM:** **Para-Commando FO21/0** (off-angle high-WIP FO) + **Traktor Katyusha Guided9/1** is the cheapest practical two-body artillery option; **Kuryer Katyusha15/1 ETB max1** earns its six-point premium through safe independent Speculative fire, Warhorse/Baggage/Minelayer. **Carmen+Bâtard17/0** is strong close-range PH-based Speculative; **Métro Grenade Launcher10/.5** is residual-Order low-cost harassment. **Do not import Kuryer as a general Wildcard**: source restricts to ETB. WIP12 E197 debated favorably both upgrades and downgrades depending on whether Guided is the only need. [Cross-faction analysis](../../notes/list-building/indirect-fire-speculative-guided-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Moblot Engineer31/0** or **Paramedic29/0** is a distinctive **Non-Hackable, Tactical Awareness, Mimetism(-3), Dodge(+1SD), Immunity Shock/IMM-B, ARM3** covered objective carrier; W1 means surviving by geometry, not 3W tanking. **Briscard FO22/0 / Paramedic23/0** supplies MSV1, Climbing+, reliable AP Marksman/score at low cost. **Chasseur FO20/0** Camo/Infiltration + LFT/Shock Mine protects the approach but becomes visible upon carrying an item. **Anaconda TAG59/1.5** (W3/ARM7, Transmutation Escape System, TA) flips a quadrant; its **ejected Operator** is separately Specialist Operative, **not a reason to treat the full TAG as eligible Supplies carrier**. **Opposing:** cheap Chasseur + Moblot/Briscard behind Loup-Garou smoke can defend two zones; 59pt Anaconda is stronger only if its gun and points swing are needed.

[Cross-game objective holder and zone-domination apex/value tiers, scenario rules, and opposing transcript reviews](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Exact profiles/Fireteams above are authoritative.

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Carmen Johns + Bâtard17/0** combines fast smoke/warband pressure with a synchronized **Sensor** carrier: Bâtard can help expose close **Camo/Hidden** while Carmen threatens follow-up, but the pair shares activation and is **not two independent Regular Orders**. **Wardriver Disco Baller16/1** can temporarily *bypass an enemy MSV* lane more cheaply than buying another elite sniper; ordinary Smoke is insufficient vs MSV2. **Counter:** exposed bikes and a synchronized Sensor need a safe approach; if a cheap marker is on the other flank, an ordinary Discover/mission detour can outperform spending several Orders chasing it.

[Full anti-tech N5.3 apex/value, exact mechanics, matchup selection and opposing transcripts](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).
