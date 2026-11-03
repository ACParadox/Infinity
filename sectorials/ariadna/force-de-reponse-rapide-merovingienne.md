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

### 6. Force de Réponse Rapide Merovingienne (FRRM)

[Current roster / Fireteams](force-de-reponse-rapide-merovingienne.md) · [Detailed guide](../../notes/factions/merovingienne.md)

**Near-must / highest-value backbone**

| Piece | Why; limit | Evidence |
|---|---|---|
| **Moblot (AP Spitfire / Engineer / support)** | Tactical Awareness on current loadouts, Non-Hackable, WIP14, strong midrange weapons and mission utilities. FRRM's clearest broadly applicable premium investment; still **one Wound**, so favor positioning over direct attrition. | [WIP12 E197 with Logan (Nov 2025)](https://open.spotify.com/episode/3YNuQVF24bJmCGdxL1FjK5) (~35–41m); [TA S3E39](https://open.spotify.com/episode/2Pqi3i2SyoSGyKciy7r2gD) (~6–14m). |
| **Métro cheap orders / camo infiltrators** | 8–10pt Regular bodies support Moblots; one-use camo infiltrating Métros create a cheap mine/marker midfield buffer. A slow full Core is not always necessary. | WIP12 E197 (~27–33m), TA S3E39. |

**Go-to**

| Piece | Why; trade-off | Evidence |
|---|---|---|
| **Loup-Garou Smoke GL 17 / Viral Marksman 24** | Cheap 0-SWC Smoke/ Riotstopper and specialist Viral pressure where useful; Viral is not a TAG/REM solution. | WIP12 E197 (~21–26m), TA S3E39. |
| **Apache FTO 14** | Efficient **Regular** CC piece to join *Loup-Garou* link, bringing close threat to Smoke/viral fire. Solo forward-deployed **non-FTO** Apache has distinct use. | WIP12 E197 (~21m), TA S3E39, LoL E157 (~74m). |
| **Para-Commando FO 21** | WIP14/+1SD lateral scoring/marking and attack angle. Off-table entry delays its contribution to initial table Orders. | WIP12 E197 (~56–62m); TA S3E39. |
| **Mirage-5** | Margot's mobile gun/specialist plus Duroc's Smoke/CC make rear-edge approach a genuine tactical fork; 2 SWC is substantial. | WIP12 E197 (~56m) emphatically praises it; [LoL E157](https://open.spotify.com/episode/1lq0RhEWwpegXr1kkKJzUr) contrasts TAG investment. |
| **Chasseur FO / Minelayer** | Cheap on-table camouflaged mine/zone control. **Contested** vs Para-Commando as *offensive* specialist; they fulfill different deployment jobs. | WIP12 E197 (~62–65m) defends Chasseur screening, TA S3E39 (~42–45m) more skeptical of N5 cost after Sixth Sense changes. |
| **Anaconda** | Improved 59pt/1.5SWC Tactical Awareness TAG with ARM7/AP Immunity, escape specialist and ETB Duo support. Not automatically better than Mirage-5. | WIP12 E197 (~53m) explicitly upgrades it to “good”; LoL E157 (~94–102m) considers competing opportunity costs. |
| **Vystrel Neurocinetics / Briscard MSV1** | Long-lane reactive/visibility solutions beyond the default Moblot Spitfire band. | WIP12 E197 (~74–80m); LoL E157; TA S3E39. |
| **Traktor Baggage / Kuryer Guided** | 5pt Regular/Deactivator or opportunistic Guided fire when Para FO / network already enables it. **Kuryer ETB-only** for teams. | WIP12 E197 (~74–80m), [WIP12 E203 TAK](https://open.spotify.com/episode/0fLvDDDa2baw7lxt3J4qo9) cautions against all-in speculative setups. |

**Directly criticized profiles / constructions**

| Avoidance | Why; alternative / dissent | Evidence |
|---|---|---|
| **Brigadier Jacques Bruant infiltrating Camouflage (1 Use) at ~33pt** | **Strong avoid as general-purpose midfield gun**: one Wound, expensive, one-use camouflage, and X-Visor adds little when already infiltrated into ideal AP Spitfire bands. Cheaper Chasseur/Metro skirmishers and stronger guns specialize better. Not zero utility as a surprise angle. | [WIP12 E197](https://open.spotify.com/episode/3YNuQVF24bJmCGdxL1FjK5) **explicitly calls this “ugly”** at ~85–90m. |
| **Bruant + Zouave AP Spitfire NCO as default extra-LT-order engine** | **Strong avoid**: roughly **62pt / 2 SWC** for two 1-Wound pieces, and the NCO body is too frail for that investment. More Moblot/gun/specialist breadth usually safer. If specifically designed to exploit LT orders, it can still function. | WIP12 E197 ~86–95m explicitly analyzes this package and rejects its cost. |
| **Generic Zouave FTO FO / Paramedic / Panzerfaust in crowded 21–23pt role** | **Conditional avoid**: WIP12 compares them unfavorably with Chasseurs and Para-Commandos offering stronger utility or defense for nearby cost. Sapper / special scenarios are real counterexamples; **do not blanket-ban every Zouave profile**. | WIP12 E197 ~90–97m includes presenter defense of Sapper as a specialist scenario piece. |

**Rules caveats:** FRRM currently has **no Chain of Command**. `Apache FTO` only joins **Loup-Garou** teams; infiltrating Bruant and non-FTO Zouave do **not** inherit FTO Fireteam access. Consider 6-SWC budget: Mirage-5 2 + Moblot AP Spitfire 1.5 + Anaconda 1.5 already consumes 5. Don't silently copy older N4 Fireteam permissions.

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

#### 6. Force de Réponse Rapide Merovingienne (FRRM)

| Weak, niche or redundant purchase | Why it is a weak default | Miniature decision |
|---|---|---|
| **Brigadier Jacques Bruant infiltrating Camo(1 Use), ~33pts** | **Strongest direct FRRM whole-model defer:** [WIP12 E197](https://open.spotify.com/episode/3YNuQVF24bJmCGdxL1FjK5) calls it **“ugly”**: 1W, expensive and X-Visor adds limited value once infiltrated into useful AP Spitfire ranges. **FTO Bruant28** offers a different *linked* gun/mission contribution. | **Skip dedicated purchase by default; proxy first**. Only buy if a particular **surprise objective/attack** or **FTO legal team** keeps using him. This is **not proof every Bruant profile fails**. |
| **Bruant + Zouave NCO gun/order pairing** | **Direct, strongest negative *package*:** roughly 62pts/2SWC committed to fragile 1W pieces to exploit a precious LT order; **Moblot/Para-Commando/Chasseur** coverage generally safer. | **Avoid the default combo**, **not both whole unit types**. If testing it, proxy both before investing; the **Zouave Sapper** is a real separate use. |
| **Generic Zouave FTO FO/Paramedic/Panzerfaust in crowded 21–23pt jobs** | **Direct with presenter dissent:** expensive relative to **Chasseur** forward control and **Para-Commando** lateral scoring; **Sapper** position-specific survivability is a real exception. | **Proxy first** for routine Zouave specialist, or **avoid profile only**. Purchase if a legal FTO link or Sapper's table geometry makes it recurring. |
| **Anaconda TAG when Mirage-5 and a Moblot attack plan already cover the pressure** | **Genuinely contested:** [WIP12 E197](https://open.spotify.com/episode/3YNuQVF24bJmCGdxL1FjK5) explicitly says improved **59pt Anaconda is good**; [LoL E157](https://open.spotify.com/episode/1lq0RhEWwpegXr1kkKJzUr) debates TAG-versus-Mirage opportunities. The **ETB TAG + Kuryer/112/Moblot** can be its own strong build. | **Proxy-test first** if deciding between two substantial attack architectures. **Not “worst”: buy if its own ETB/TAG plan wins repeatedly**, not merely to own every Ariadna TAG. |
| **Kuryer Uragan/Guided or second long-range artillery beside Vystrel** | **Comparison:** **Kuryer TR18/1** offers ranged lane pressure, but **Vystrel** may be a better specialized ARO, and **Traktor Baggage5** a cheaper Order; Guided needs real **FO/Targeted**. **Kuryer team access is ETB only.** | **Proxy alternate REM chassis/loadout** before buying specialized artillery. **No unsupported global Wildcard Kuryer**; the first useful Vystrel or Traktor is not weak. |
| **Wardriver second model / unsupported lone Pitcher** | **Direct disagreement — LoL E157:** one presenter favors **Disco/Zero Pain**, another brings both; WIP12 worries about poor matchups against stronger hackers. Two devices cost SWC and may never yield the required Targeted network. | **Proxy the second Wardriver**, purchase only if two different profiles truly appear **simultaneously**. Don't ban first Disco/vision tool where necessary. |
| **Knauf FTO, Wolfgang, third Briscard/elite shooter with no unique lane** | **Inferred from [FRRM guide](../../notes/factions/merovingienne.md):** Knauf may buy linked MSV sniper, Wolfgang CC/continuous damage, Briscard MSV1/Climbing Plus. Costly 1W Fireteams or another gun can dilute mission spread; these are **credible positive niches**, not sourced duds. | **Proxy-test the extra named gun or specialist** and buy when the **actual profile/Fireteam** repeats. Knauf FTO belongs in **Métros**, not an arbitrary FRRM team. |
| **Second Para-Commando or excess Chasseurs** | **Mission-dependent:** WIP12 likes Chasseur mine/marker defence, TA questions post-Sixth-Sense cost, Para FO provides the off-board scoring path. They cannot replace each other's deployment utility. | **Proxy the *additional* trooper**, do **not** classify the **first Chasseur FO/Minelayer** or Para FO as weak. |
| **Extra Carmen Johns + Bâtard / Wolfgang close-quarters overlap** | **Inference:** Smoke/multibody CC threats are useful but compete with **Apache FTO**, Mirage-5, and expensive assault roles in typical 300pt lists. Carmen is a **two-model team**. | **Proxy-test only if needed**, providing an appropriate **Bâtard** model; never assume a single Carmen sculpt represents two bodies. |

**Sources:** [WIP12 E197](https://open.spotify.com/episode/3YNuQVF24bJmCGdxL1FjK5), [Tactical Awareness FRRM](https://open.spotify.com/episode/2Pqi3i2SyoSGyKciy7r2gD), [LoL E157](https://open.spotify.com/episode/1lq0RhEWwpegXr1kkKJzUr), [FRRM guide](../../notes/factions/merovingienne.md). **Strong buys remain:** a useful **Moblot**, affordable **Métros**, **Loup-Garou Smoke**, **Apache FTO**, **Chasseur** and a legitimate ranged counter.

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
