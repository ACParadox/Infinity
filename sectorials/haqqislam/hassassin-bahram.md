---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 402
sectorial_slug: hassassin-bahram
sectorial_name: Hassassin Bahram
parent_faction: Haqqislam
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "33-unit standard Hassassin Bahram roster, all standard loadouts, complete main Fireteam chart and reverse Fireteam index; optional Husam Spec-Ops and Haqqislam Team-Ops hooks; linked Reinforcement Army 499 is identified but not merged into the main chart."
---

# Hassassin Bahram

## Overview and provenance

Repository-native factual reference for **Hassassin Bahram** roster, profiles, points/SWC, AVA, and Fireteam access.

Sources used:

- Army-derived Hassassin Bahram source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `d4329bb596ffea5d568eb2435f74366c305a7630`.
- InfinityDB normalization/identity baseline at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **33-unit standard Hassassin Bahram roster** and the complete main `fireteamChart` exposed by the pinned Army source.
- Generic Soldier of Fortune / mercenary-catalog entries whose source `factions` list is empty are excluded from the base roster.
- `Husam Spec-Ops` and `Haqqislam Team-Ops` are optional game-mode content and are listed separately.
- Fireteam legality comes from the canonical chart below, not from an `FTO` profile name by itself. Rafiq Remote FTO and Claire Lazhari FTO are therefore **not** assigned Fireteam access because the Bahram chart has no row for them.
- `BOKHTAR FTO` restricts Bahram-team access to Bokhtar options 1, 2, 5, and 6. Yasbir's Wildcard access is restricted to his `HASSASSIN HUSAM YASBIR FTO` option 1.
- Parenthetical chart comments such as `(Bahram)` and `(Ghulam, Bahram)` are preserved as Counts-as / equivalence labels, consistent with the repository Fireteam convention; they are not silently reinterpreted as join-scope restrictions.
- The structured `required: true` rows in **Hassassin Bahram Fireteams** are preserved as a required-choice set: a legal team must satisfy the source-required Bahram-member condition, but this file does not reinterpret the data as requiring every marked troop type simultaneously.
- Linked Reinforcement Army ID: **499**. Reinforcement roster and Fireteams are not merged into this main-sectorial chart.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Hassassin Bahram |
| Parent faction | Haqqislam |
| Army ID | 402 |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 33 |
| Optional-mode units | Husam Spec-Ops; Haqqislam Team-Ops |
| Reinforcement roster | Army ID `499` |
| Fireteam limits | Core 1; Haris 1; Duo unlimited |
| Fireteam chart | yes |

## Fireteam chart limits and sectorial-level restrictions

| Constraint | Value / wording |
|---|---|
| Core | up to 1 |
| Haris | up to 1 |
| Duo | unlimited (`256` in source chart) |
| Main team families | Ghulam Fireteams; Hassassin Bahram Fireteams; Shakush Fireteams |
| Wildcards | Asawira; Yasbir FTO; Leila Sharif; Yara Haddad |
| Bahram required-choice set | Govad, Muyib, Lasiq, or Bokhtar FTO rows are source-marked `required: true`; preserve as the Bahram-member requirement rather than requiring all four troop types |
| Bokhtar restriction | Only `BOKHTAR FTO` options 1, 2, 5, 6 may use the Bahram Fireteam row |
| Yasbir restriction | Only option 1, `HASSASSIN HUSAM YASBIR FTO`, has Wildcard access |
| Spec-Ops restriction | Husam may use the Ghulam row only when Spec-Ops mode is in use |
| Main/Reinforcement mixing | No source-defined mixing exception; keep Army 402 and Reinforcement Army 499 charts separate |

## Roster index

| Unit | ID | AVA | Type | Classification | Order | Fireteam access |
|---|---:|---:|---|---|---|---|
| Yara Haddad | 1548 | 1 | MI | Character | Regular | Wildcard |
| Rafiq Remotes | 315 | 2 | REM | Support Troops | Regular | — |
| Hassassin Farzans | 332 | 3 | SK | Spec. Trained Troops | Regular | — |
| Kameel Remotes | 334 | 2 | REM | Support Troops | Regular | — |
| Hussein Al-Djabel | 335 | 1 | SK | Character | Regular | — |
| Hassassin Fiday | 312 | 2 | SK | Spec. Trained Troops | Regular | — |
| Avicenna | 491 | 1 | LI | Character | Regular | Ghulam; Shakush |
| Hassassin Husam Yasbir | 341 | 1 | LI | Character | Regular | Wildcard, FTO option 1 only; counts as Ghulam / Bahram |
| Hassassin Muyibs | 327 | 6 | MI | Spec. Trained Troops | Regular | Ghulam; Bahram; Shakush |
| Hassassin Barid | 337 | 2 | LI | Spec. Trained Troops | Regular | Ghulam |
| Ghazi Muttawi'ah | 340 | 4 | LI | Line Troops | Irregular + Impetuous | — |
| Hassassin Ragiks | 307 | 4 | MI | Elite Troops | Regular | — |
| McMurrough | 283 | 1 | WB | Character | Irregular + Impetuous | — |
| Sunduqbut | 1590 | 2 | HI | Spec. Trained Troops | Regular | — |
| Hassassin Áyyār | 779 | 2 | HI | Elite Troops | Regular | — |
| Dr. Claire Lazhari | 1894 | 1 | LI | Character | Regular | —; FTO-labelled option has no Bahram chart row |
| Shihab Remotes | 316 | 1 | REM | Support Troops | Regular | — |
| Shaytaniyah Remotes | 317 | 1 | REM | Support Troops | Regular | — |
| Hassassin Govads | 304 | 5 | MI | Spec. Trained Troops | Regular | Ghulam; Bahram |
| Asawira Regiment | 329 | 3 | HI | Headquarters Troops | Regular | Wildcard |
| Warcors | 50 | 1 | LI | Mercenary Troops | Irregular | — |
| Hassassin Bokhtar | 1589 | 2 | HI | Elite Troops | Regular + Tactical Awareness | Bahram, FTO options only |
| Hassassin Shujae | 1547 | 2 | SK | Veteran Troops | Regular | — |
| Hassassin Lasiqs | 328 | 3 | LI | Spec. Trained Troops | Regular | Bahram |
| Najjarun Engineer | 314 | 1 | LI | Support Troops | Regular | — |
| Nasmat Remotes | 333 | 2 | REM | Support Troops | Peripheral / no Order | — |
| Fanous Remotes | 318 | 1 | REM | Support Troops | Regular | — |
| Hassassin Nadhir | 1545 | 2 | LI | Spec. Trained Troops | Regular | — |
| Husam Operative Leila Sharif | 849 | 1 | LI | Character | Regular | Wildcard; counts as Ghulam / Bahram |
| Daylami Infantry | 323 | 5 | LI | Garrison Troops | Irregular | — |
| Sayiq TAG Support Pilots | 1849 | 1 | LI | Support Troops | Regular | Ghulam; Shakush |
| Shakush Light Armored Unit | 1546 | 2 | TAG | Mechanized Troops | Regular + Tactical Awareness | Shakush |
| Ghulam Infantry | 301 | 4 | LI | Line Troops | Regular | Ghulam |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Husam Spec-Ops | 1916 | Spec-Ops | Ghulam Fireteam row, max 1 when Spec-Ops mode is in use |
| Haqqislam Team-Ops | 1930 | Team-Ops | No ordinary Hassassin Bahram Fireteam row |

## Unit details

### Yara Haddad

**ID 1548 · AVA 1 · MI · Character** — `MOV 10-10 | CC 16 | BS 13 | PH 11 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. Multispectral Visor L2, Immunity (ARM), Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 0 | AP Marksman Rifle, Heavy Pistol (+1B), CCW | Wildcard |
| 2 | 27 | 0 | As 1; Strategic Deployment | Wildcard |
| 3 | 24 | 0 | As 1; Lieutenant | Wildcard |
| 4 | 27 | 0 | As 1; Lieutenant, Strategic Deployment | Wildcard |

### Rafiq Remotes

**ID 315 · AVA 2 · REM · Support Troops** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Deactivator, Repeater; Courage, Forward Observer, Remote Presence, Sensor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 13 | 0 | Rifle, Light Shotgun, Flash Pulse, PARA CCW (-3); Triangulated Fire | — |
| 3 | 19 | 0.5 | **RAFIQ REMOTE FTO**; Red Fury, Flash Pulse, PARA CCW (-3) | —; no chart row |

### Hassassin Farzans

**ID 332 · AVA 3 · SK · Spec. Trained Troops** — `MOV 10-10 | CC 16 | BS 12 | PH 11 | WIP 14 | ARM 0 | BTS 0 | W 1 | S 2`. Camouflage, Infiltration, Mimetism (-3), Surprise Attack (-3), BS Attack (Shock), Stealth, Terrain (Total), Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 0 | Boarding Shotgun, Shock Mine, Silenced Pistol, CCW; Chain of Command | — |
| 2 | 21 | 0.5 | Boarding Shotgun, Viral Mine, Silenced Pistol, CCW; Minelayer | — |
| 3 | 22 | 0 | Rifle, Light Shotgun, Flash Pulse, Shock Mine, D-Charges, Silenced Pistol, CCW; Forward Observer | — |

### Kameel Remotes

**ID 334 · AVA 2 · REM · Support Troops** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 4`. Baggage, Courage, Remote Presence.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | PARA CCW (-3); Deactivator, Repeater | — |
| 2 | 14 | 0.5 | PARA CCW (-3); EVO Hacking Device, Hacker | — |
| 3 | 16 | 0 | Rifle, Light Shotgun, PARA CCW (-3); Repeater, Total Reaction | — |

### Hussein Al-Djabel

**ID 335 · AVA 1 · SK · Character** — `MOV 10-10 | CC 23 | BS 12 | PH 13 | WIP 15 | ARM 1 | BTS 0 | W 1 | S 2`. Martial Arts L4, Impersonation, Surprise Attack (-3), BS Attack (Continuous Damage), Stealth, Climbing Plus, Dodge (+5), Terrain (Total), Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 0 | Rifle, Light Shotgun, Nanopulser, Smoke Grenades, Silenced Pistol, Viral CCW (PS 5) | — |

### Hassassin Fiday

**ID 312 · AVA 2 · SK · Spec. Trained Troops** — `MOV 10-10 | CC 23 | BS 11 | PH 12 | WIP 15 | ARM 1 | BTS 0 | W 1 | S 2`. Martial Arts L3, Impersonation, Surprise Attack (-3), Dodge (+2.5), Stealth, Terrain (Total), Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 25 | 0 | Rifle, Light Shotgun, Smoke Grenades, Pistol, DA CCW (PS 6) | — |
| 3 | 26 | 0 | As 2; Shock Mine | — |
| 4 | 23 | 0 | Boarding Shotgun, Smoke Grenades, Pistol, DA CCW (PS 6) | — |

### Avicenna

**ID 491 · AVA 1 · LI · Character** — `MOV 15-5 | CC 16 | BS 11 | PH 11 | WIP 15 | ARM 2 | BTS 3 | W 1 | S 2`. MediKit; Courage, Immunity (ARM), Doctor (+3), No Wound Incapacitation.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 28 | 0 | Combi Rifle, Flash Pulse, Pistol, CCW, Nanopulser | Ghulam max 1; Shakush max 1 |

### Hassassin Husam Yasbir

**ID 341 · AVA 1 · LI · Character** — `MOV 10-10 | CC 22 | BS 12 | PH 12 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Bangbomb (+4); Martial Arts L2, Immunity (Shock), Specialist Operative, Stealth, Religious Troop, BS Attack (SR-1).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 25 | 0 | **HASSASSIN HUSAM YASBIR FTO**; Holomask; Viral Rifle, Light Shotgun (+1B), Drop Bears, Pistol, Viral CCW (PS 6) | Wildcard max 1; counts as Ghulam / Bahram |
| 3 | 29 | 0 | Viral Rifle, Light Shotgun (+1B), Smoke Grenades, Drop Bears, Pistol, Viral CCW (PS 6); Surprise Attack (-3), Parachutist, Decoy (2) | — |

### Hassassin Muyibs

**ID 327 · AVA 6 · MI · Spec. Trained Troops** — `MOV 10-10 | CC 18 | BS 13 | PH 11 | WIP 14 | ARM 3 | BTS 3 | W 1 | S 2`. Immunity (BTS), Number 2, Religious Troop, Dogged.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|---|
| 2 | 21 | 1 | Rifle, Grenade Launcher, Smoke Grenade Launcher, Kobra Pistol, CCW | Ghulam/Bahram/Shakush |
| 4 | 25 | 0 | Rifle, Light Shotgun, Panzerfaust, Viral Mine, Kobra Pistol, CCW; Minelayer | same |
| 5 | 32 | 1.5 | Spitfire, D-Charges, Kobra Pistol, CCW; X-Visor, Tactical Awareness | same |
| 6 | 22 | 1.5 | Heavy Rocket Launcher, D-Charges, Kobra Pistol, CCW; X-Visor, Tactical Awareness | same |
| 7 | 26 | 0 | Rifle, Light Shotgun, Panzerfaust, Kobra Pistol, CCW; MediKit, Doctor (+3) | same |
| 9 | 23 | 0 | Rifle, Light Shotgun, Panzerfaust, Flash Pulse, Kobra Pistol, CCW; Forward Observer | same |
| 11 | 21 | 1 | As opt 2; Lieutenant | same |

### Hassassin Barid

**ID 337 · AVA 2 · LI · Spec. Trained Troops** — `MOV 10-10 | CC 14 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Terrain (Desert), Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 0.5 | Rifle, Pitcher, Breaker Pistol, CCW; Hacking Device, Hacker | Ghulam max 2 |
| 2 | 14 | 0 | Rifle, Pitcher, Breaker Pistol, CCW; Killer Hacking Device with Trinity (-3), Hacker | same |
| 3 | 12 | 0 | Rifle, Pitcher, Flash Pulse, Breaker Pistol, CCW; Forward Observer | same |
| 4 | 16 | 1 | As opt 1; Lieutenant | same |
| 5 | 12 | 0 | As opt 3; Lieutenant | same |

### Ghazi Muttawi'ah

**ID 340 · AVA 4 · LI · Line Troops** — `MOV 10-10 | CC 14 | BS 11 | PH 12 | WIP 15 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular, Impetuous; Courage, Dogged, No Cover.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 5 | 0 | Chain Rifle, Smoke Grenades, Breaker Pistol, CCW | — |
| 2 | 5 | 0 | Chain Rifle, E/Marat, Pistol, CCW | — |
| 3 | 6 | 0 | Chain Rifle, Jammer, Pistol, CCW | — |
| 4 | 7 | 0 | Boarding Shotgun, E/Marat, Smoke Grenades, Pistol, CCW | — |
| 5 | 8 | 0 | Boarding Shotgun, Jammer, Smoke Grenades, Pistol, CCW | — |

### Hassassin Ragiks

**ID 307 · AVA 4 · MI · Elite Troops** — `MOV 10-10 | CC 15 | BS 12 | PH 12 | WIP 15 | ARM 2 | BTS 0 | W 1 | S 2`. Immunity (Shock), Parachutist, Combat Jump, Stealth, Dogged, Religious Troop, Super-Jump (Jet Propulsion).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 23 | 0 | Boarding Shotgun (+1B), Boarding Pistol, CCW | — |
| 3 | 29 | 1.5 | Spitfire, Boarding Pistol, CCW | — |
| 4 | 25 | 0.5 | Boarding Shotgun, D-Charges, Boarding Pistol, CCW; Hacking Device with Carbonite (PS 6), Hacker | — |

### McMurrough

**ID 283 · AVA 1 · WB · Character** — `MOV 15-10 | CC 23 | BS 11 | PH 16 | WIP 14 | ARM 4 | BTS 3 | W 2 | S 6`. Irregular, Impetuous; Martial Arts L2, Berserk, Courage, Dodge (+5), Immunity (ARM), No Cover, Super-Jump, Dogged.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Chain Rifle (+1B), Grenades (PS 6), Smoke Grenades, AP + DA CCW (PS 3) | — |

### Sunduqbut, Covert Heavy-Support Unit

**ID 1590 · AVA 2 · HI · Spec. Trained Troops** — `MOV 10-10 | CC 13 | BS 13 | PH 14 | WIP 12 | ARM 4 | BTS 3 | W 2 | S 2`. Structure; Remote Presence, BS Attack (SR-1), Camouflage (1 Use), Courage, Forward Deployment (+20), Decoy (1).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 49 | 1.5 | AP Spitfire, Light Shotgun, Pistol, CCW; Surprise Attack (-3) | — |
| 3 | 43 | 0.5 | Viral Rifle (+1B), Chain Rifle (+1B), Viral Mine, Pistol, CCW; Surprise Attack (-3), Minelayer | — |
| 4 | 47 | 1.5 | Feuerbach, Pistol, CCW; Neurocinetics | — |
| 5 | 42 | 0 | Viral Rifle, Chain Rifle, Pistol, CCW; Neurocinetics (+1B) | — |
| 6 | 50 | 1.5 | AP Spitfire, Light Shotgun, Pistol, CCW; Neurocinetics | — |

### Hassassin Áyyār

**ID 779 · AVA 2 · HI · Elite Troops** — `MOV 15-5 | CC 17 | BS 13 | PH 13 | WIP 14 | ARM 3 | BTS 3 | W 2 | S 2`. Bangbomb (+4), Holoprojector; Surprise Attack (-6), Triangulated Fire, Hidden Deployment, Specialist Operative, Stealth, Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 40 | 0 | AP Rifle, E/Mitter, Viral Pistol (+1B), CCW; BS Attack (+1B) | — |
| 2 | 39 | 0 | Thunderbolt (AP), Zapper, Viral Pistol (+1B), CCW; BS Attack (+1B) | — |
| 4 | 38 | 0 | Breaker Rifle, Zapper, Panzerfaust, Drop Bears, Viral Pistol (+1B), CCW; Forward Deployment (+10) | — |
| 5 | 39 | 0 | AP Marksman Rifle, Zapper, Drop Bears, Viral Pistol (+1B), CCW; Forward Deployment (+10) | — |
| 6 | 38 | 0 | Breaker Rifle, Zapper, Panzerfaust, Disco Baller, Viral Pistol (+1B), CCW; Forward Deployment (+10) | — |

### Dr. Claire Lazhari

**ID 1894 · AVA 1 · LI · Character** — `MOV 15-5 | CC 16 | BS 13 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Albedo (-3), Cube 2.0, Non-Hackable; BS Attack (Continuous Damage), Dodge (+3), Immunity (Enhanced), No Wound Incapacitation; MediKit (PH=17).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 0 | Breaker Combi Rifle, Nanopulser (+1B), Viral Pistol (+1B), PARA CCW (-3), Disco Baller; MediKit, Doctor (2W) | — |
| 2 | 33 | 0 | **CLAIRE LAZHARI FTO**; same weapons; MediKit, Doctor (+3) | —; no chart row |

### Shihab Remotes

**ID 316 · AVA 1 · REM · Support Troops** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. 360º Visor; Courage, Immunity (Shock), Remote Presence, Total Reaction.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 1 | HMG, PARA CCW (-3) | — |
| 2 | 18 | 0 | Thunderbolt (+1B), PARA CCW (-3) | — |

### Shaytaniyah Remotes

**ID 317 · AVA 1 · REM · Support Troops** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Courage, Remote Presence.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CCW (-3); BS Attack (Guided) | — |
| 3 | 19 | 1.5 | Missile Launcher (+1B), PARA CCW (-3) | — |

### Hassassin Govads

**ID 304 · AVA 5 · MI · Spec. Trained Troops** — `MOV 10-10 | CC 15 | BS 13 | PH 11 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. Multispectral Visor L1, Warhorse, Religious Troop, Combat Instinct.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 28 | 1.5 | HMG, Breaker Pistol, CCW | Ghulam/Bahram |
| 4 | 26 | 0.5 | AP Sniper Rifle, Breaker Pistol, CCW; BS Attack (Shock) | same |
| 5 | 26 | 1.5 | Missile Launcher, Breaker Pistol (+1B), CCW | same |
| 6 | 25 | 0.5 | Boarding Shotgun, Breaker Pistol, CCW, E/Mitter; Hacking Device, Hacker | same |
| 7 | 23 | 0 | Boarding Shotgun, Breaker Pistol, CCW, E/Mitter; Killer Hacking Device, Hacker | same |
| 9 | 25 | 0 | AP Rifle, Light Shotgun, AP Mine, D-Charges, Breaker Pistol, CCW; GizmoKit, Engineer | same |

### Asawira Regiment

**ID 329 · AVA 3 · HI · Headquarters Troops** — `MOV 15-5 | CC 23 | BS 14 | PH 14 | WIP 14 | ARM 4 | BTS 9 | W 2 | S 2`. Martial Arts L2, Frenzy, Berserk (+3), Dodge (+5), Regeneration, Stealth, Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 0 | AP Rifle, Light Shotgun, Pistol, Nanopulser, DA CCW (PS 5) | Wildcard |
| 2 | 35 | 0 | Viral Rifle (PS 6), Light Shotgun, Nanopulser, Pistol, DA CCW (PS 5) | Wildcard |
| 3 | 32 | 0 | Boarding Shotgun (+1B), Nanopulser, Disco Baller, Pistol, DA CCW (PS 5) | Wildcard |
| 4 | 38 | 1.5 | AP Spitfire, Nanopulser, Pistol, DA CCW (PS 5) | Wildcard |
| 5 | 37 | 0 | As 1; MediKit, Doctor (+3) | Wildcard |
| 6 | 35 | 0 | Boarding Shotgun (+1B), Nanopulser, Pistol, DA CCW (PS 5); MediKit, Doctor (+3) | Wildcard |
| 8 | 33 | 0 | As 1; Lieutenant | Wildcard |
| 10 | 38 | 1.5 | As 4; Lieutenant | Wildcard |

### Warcors

**ID 50 · AVA 1 · LI · Mercenary Troops** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular; Journalist.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor | — |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); Sixth Sense | — |

### Hassassin Bokhtar

**ID 1589 · AVA 2 · HI · Elite Troops** — `MOV 15-5 | CC 20 | BS 13 | PH 13 | WIP 14 | ARM 4 | BTS 3 | W 2 | S 2`. Multispectral Visor L1; Dodge (+3/+5), Mimetism (-3), Religious Troop, Super-Jump (Jet Propulsion), Tactical Awareness.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 46 | 1.5 | **BOKHTAR FTO**; Red Fury, Viral Pistol, Shock CCW (PS 7) | Bahram max 2 |
| 2 | 45 | 0 | **BOKHTAR FTO**; Viral Rifle, Light Shotgun, D-Charges, Viral Pistol, Shock CCW (PS 7); MediKit, Paramedic | Bahram max 2 |
| 3 | 52 | 1.5 | Red Fury, Viral Pistol, Shock CCW (PS 7); Parachutist | — |
| 4 | 49 | 0 | Boarding Shotgun (+1B), D-Charges, Viral Pistol, Shock CCW (PS 7); MediKit, Paramedic, Parachutist | — |
| 5 | 46 | 1.5 | **BOKHTAR FTO**; as 1; Lieutenant | Bahram max 2 |
| 6 | 45 | 0 | **BOKHTAR FTO**; as 2; Lieutenant | Bahram max 2 |

### Hassassin Shujae

**ID 1547 · AVA 2 · SK · Veteran Troops** — `MOV 10-10 | CC 17 | BS 13 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Bangbomb (+4); Forward Deployment (+20), Mimetism (-6), Specialist Operative, Stealth, Religious Troop, Terrain (Total), Surprise Attack (-3), Hidden Deployment.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 29 | 0 | AP Rifle, Light Shotgun, D-Charges, Breaker Pistol, CCW | — |
| 2 | 27 | 0 | Boarding Shotgun, Shock Mine, Breaker Pistol, CCW; Minelayer (2) | — |
| 3 | 27 | 0 | Submachine Gun, Flammenspeer, E/M Mine, Breaker Pistol, CCW; Minelayer (2) | — |
| 4 | 30 | 0 | Viral Rifle, Light Shotgun, D-Charges, Breaker Pistol, CCW | — |

### Hassassin Lasiqs

**ID 328 · AVA 3 · LI · Spec. Trained Troops** — `MOV 10-10 | CC 15 | BS 12 | PH 10 | WIP 14 | ARM 2 | BTS 0 | W 1 | S 2`. X-Visor; Marksmanship, Immunity (Shock), Mimetism (-3), Climbing Plus, Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 25 | 1 | Viral Sniper Rifle, Pistol, CCW | Bahram max 3; counts as Bahram |
| 3 | 25 | 0.5 | Viral Marksman Rifle, Pistol, CCW; BS Attack (AP) | same |
| 5 | 22 | 0 | Viral Rifle, Light Shotgun, Flash Pulse, Pistol, CCW; Forward Observer | same |

### Najjarun Engineer

**ID 314 · AVA 1 · LI · Support Troops** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. GizmoKit, Deactivator; Courage, Engineer.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 15 | 0 | Rifle, Light Shotgun, D-Charges, Pistol, CCW | — |
| 2 | 16 | 0 | As 1; Deployable Cover | — |
| 3 | 17 | 0 | As 1; Armed Turret (Rifle) | — |

### Nasmat Remotes

**ID 333 · AVA 2 · REM · Support Troops** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Peripheral; Courage, Mimetism (-3), Peripheral (Servant).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | PARA CCW (-3); no Order; Peripheral servant | — |

### Fanous Remotes

**ID 318 · AVA 1 · REM · Support Troops** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater; Courage, Mimetism (-3), Remote Presence.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) | — |

### Hassassin Nadhir

**ID 1545 · AVA 2 · LI · Spec. Trained Troops** — `MOV 10-10 | CC 14 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. BS Attack (Shock), Surprise Attack (-3), Forward Deployment (+10), Hidden Deployment, Mimetism (-6), Religious Troop, Terrain (Desert), Forward Observer.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 0.5 | AP Marksman Rifle, Pistol, CCW | — |
| 2 | 23 | 0 | Rifle, Light Shotgun, Panzerfaust, Pistol, CCW | — |
| 3 | 20 | 0 | Submachine Gun, Flammenspeer, Pistol, CCW | — |
| 4 | 26 | 0 | Submachine Gun, Thunderbolt, Pistol, CCW | — |
| 5 | 29 | 0.5 | AP Marksman Rifle, Viral Mine, Pistol, CCW; Minelayer | — |

### Husam Operative Leila Sharif

**ID 849 · AVA 1 · LI · Character** — `MOV 10-10 | CC 15 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Killer Hacking Device with Carbonite and Firewall (-3) upgrades; Religious Troop, Combat Instinct.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 22 | 0 | Shock Marksman Rifle, E/M Mine, D-Charges, Breaker Pistol, CCW; Hacker | Wildcard max 1; counts as Ghulam / Bahram |

### Daylami Infantry

**ID 323 · AVA 5 · LI · Garrison Troops** — `MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Irregular; Terrain (Desert).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 5 | 0 | Light Shotgun, Boarding Pistol, CCW | — |
| 2 | 10 | 0.5 | Rifle, Grenade Launcher, Boarding Pistol, CCW | — |
| 3 | 6 | 0 | Light Shotgun, Panzerfaust, Boarding Pistol, CCW | — |
| 4 | 10 | 0 | Marksman Rifle, Boarding Pistol, CCW | — |
| 5 | 9 | 0 | Rifle, Light Shotgun, Boarding Pistol, CCW; Camouflage (1 Use), Infiltration | — |
| 6 | 8 | 0 | Light Shotgun, Panzerfaust, Boarding Pistol, CCW; Camouflage (1 Use), Infiltration | — |

### Sayiq, Sword of Allah TAG Support Pilots

**ID 1849 · AVA 1 · LI · Support Troops** — `MOV 10-10 | CC 16 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Courage, Specialist Operative, Terrain (Desert), Religious Troop, TAGCom [Dodge (PH+3), GizmoKit (PH+1)].

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 9 | 0 | **SHAKUSH PILOT**; Submachine Gun, D-Charges, Pistol, CCW; GizmoKit | Ghulam max 1; Shakush max 1 |

### Shakush Light Armored Unit

**ID 1546 · AVA 2 · TAG · Mechanized Troops** — `MOV 15-5 | CC 17 | BS 14 | PH 14 | WIP 14 | ARM 6 | BTS 6 | W 3 | S 6`. Structure; BS Attack (SR-1), Courage, Dodge (PH=11), Tactical Awareness, Gizmokit (PH=11). Includes one Jandab Ancillary Remote.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 58 | 1.5 | HMG (Continuous Damage), Heavy Flamethrower, AP CCW (PS 6); Jandab included | Shakush 1–2 |
| 2 | 56 | 1.5 | AP Spitfire, Heavy Flamethrower, AP CCW (PS 6); Jandab included | Shakush 1–2 |

**Jandab Ancillary Remote:** `MOV 15-10 | CC — | BS — | PH 10 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 1`; Courage, Specialist Operative, Mimetism (-3), Peripheral (Ancillary). Included profile is disabled as a standalone purchase.

### Ghulam Infantry

**ID 301 · AVA 4 · LI · Line Troops** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Terrain (Desert).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 11 | 0 | Rifle, Light Shotgun, Pistol, CCW | Ghulam 1–4 |
| 2 | 20 | 1 | HMG, Pistol, CCW | same |
| 4 | 17 | 1.5 | Missile Launcher, Pistol, CCW | same |
| 7 | 16 | 0.5 | Rifle, Light Shotgun, Pistol, CCW; Hacking Device, Hacker | same |
| 8 | 15 | 0 | Rifle, Light Shotgun, Pistol, CCW; MediKit, Doctor (+3) | same |
| 9 | 12 | 0 | Rifle, Light Shotgun, Flash Pulse, Pistol, CCW; Forward Observer | same |
| 10 | 13 | 0 | Rifle, Light Shotgun, E/M Mine, Pistol, CCW; Deployable Repeater | same |
| 11 | 11 | 0 | Base loadout; Lieutenant | same |
| 14 | 15 | 1 | Rifle, Grenade Launcher, Smoke Grenade Launcher, Pistol, CCW; NCO | same |
| 18 | 12 | 0 | Rifle, Light Shotgun, Panzerfaust, Pistol, CCW; Number 2 | same |
| 19 | 15 | 0 | Base loadout; Lieutenant (+1 Command Token) | same |
| 20 | 13 | 0 | Base loadout; Commlink (+2), Specialist Operative | same |

## Optional game-mode units

### Husam Spec-Ops

**ID 1916 · AVA 1 · Spec-Ops mode only.** Initial profile: `MOV 10-10 | CC 14 | BS 12 | PH 11 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`, MI; Infinity Spec-Ops, Immunity (Shock), Terrain (Total), Religious Troop. Enhanced profile: `MOV 15-5 | CC 18 | BS 13 | PH 13 | WIP 14 | ARM 4 | BTS 6 | W 2 | S 2`, HI; Regeneration (PH=15), Terrain (Total), Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 27 | 1 | HMG, D-Charges, Pistol, CCW | Ghulam max 1, Spec-Ops mode |
| 2 | 24 | 1 | Viral Sniper Rifle, D-Charges, Pistol, CCW | same |
| 3 | 23 | 0 | Viral Rifle (PS 6), Light Shotgun, D-Charges, Pistol, CCW; MediKit (+1B), GizmoKit, Paramedic | same |
| 4 | 26 | 0.5 | Viral Rifle (PS 6), Light Shotgun, D-Charges, Pistol, CCW; Hacking Device, Hacker | same |
| 5 | 22 | 0 | Viral Rifle (PS 6), Light Shotgun, Flash Pulse, D-Charges, Pistol, CCW; Forward Observer | same |
| 6 | 24 | 0 | Viral Rifle (PS 6), Light Shotgun, D-Charges, Pistol, CCW; MediKit (+1B), Doctor | same |

### Haqqislam Team-Ops

**ID 1930 · Team-Ops mode only.** Contains Husam-1, Husam Heavy, and Alfank SpecBot Team-Ops profiles. The pinned Hassassin Bahram `fireteamChart` exposes **no ordinary Bahram Fireteam row** for Team-Ops; do not treat these profiles as standard matched-play roster entries.

## Fireteams

### FT-01 — Ghulam Fireteams

**Types:** Core, Haris  
**Wildcard team:** no  
**Observation:** At least one Ghulam is required by the source row. Husam is a Spec-Ops-mode entry.

| Member | Unit ID | Required | Min | Max | Counts as | FTO/profile restriction | Notes |
|---|---:|---|---:|---:|---|---|---|
| Ghulam | 301 | no | 1 | 4 | — | all | Native anchor |
| Barid | 337 | no | 0 | 2 | — | all | — |
| Muyib | 327 | no | 0 | 2 | — | all | — |
| Govad | 304 | no | 0 | 1 | — | all | — |
| Avicenna | 491 | no | 0 | 1 | — | all | — |
| Sayiq | 1849 | no | 0 | 1 | — | all | Shakush Pilot profile |
| Husam Spec-Ops | 1916 | no | 0 | 1 | — | Spec-Ops mode | Optional game mode only |

### FT-02 — Hassassin Bahram Fireteams

**Types:** Core, Haris, Duo  
**Wildcard team:** no  
**Observation:** The four source rows are marked `required: true`; preserve them as a required-choice **Bahram-member** set, not as a requirement to field every listed troop type.

| Member | Unit ID | Required set | Min | Max | Counts as | FTO/profile restriction | Notes |
|---|---:|---|---:|---:|---|---|---|
| Govad | 304 | yes | 0 | 5 | Bahram | all | Source comment `(Bahram)` |
| Muyib | 327 | yes | 0 | 5 | Bahram | all | Source comment `(Bahram)` |
| Lasiq | 328 | yes | 0 | 3 | Bahram | all | Source comment `(Bahram)` |
| Bokhtar | 1589 | yes | 0 | 2 | — | **FTO options 1, 2, 5, 6 only** | Source member name `BOKHTAR FTO` |

### FT-03 — Shakush Fireteams

**Types:** Duo  
**Wildcard team:** no

| Member | Unit ID | Required | Min | Max | Counts as | FTO/profile restriction | Notes |
|---|---:|---|---:|---:|---|---|---|
| Shakush | 1546 | no | 1 | 2 | — | all | Native anchor |
| Avicenna | 491 | no | 0 | 1 | — | all | — |
| Sayiq | 1849 | no | 0 | 1 | — | all | — |
| Muyib | 327 | no | 0 | 1 | — | all | — |

### FT-04 — Wildcards

| Unit | Unit ID | Max | Counts as | Profile restriction | Notes |
|---|---:|---:|---|---|---|
| Asawira | 329 | 3 | — | all | Wildcard |
| Hassassin Husam Yasbir | 341 | 1 | Ghulam; Bahram | **FTO option 1 only** | Source comment `(Ghulam, Bahram)` |
| Leila Sharif | 849 | 1 | Ghulam; Bahram | all | Source comment `(Ghulam, Bahram)` |
| Yara Haddad | 1548 | 1 | — | all | Wildcard |

## Unit → Fireteam access index

| Unit | Fireteam | Type | Access | Counts as | Profile restriction | Min/Max | Notes |
|---|---|---|---|---|---|---|---|
| Ghulam | FT-01 Ghulam | Core/Haris | native | — | all | 1–4 | Anchor |
| Barid | FT-01 Ghulam | Core/Haris | native | — | all | 0–2 | — |
| Muyib | FT-01 Ghulam | Core/Haris | native | — | all | 0–2 | — |
| Muyib | FT-02 Bahram | Core/Haris/Duo | required | Bahram | all | 0–5 | Required-choice set |
| Muyib | FT-03 Shakush | Duo | native | — | all | 0–1 | — |
| Govad | FT-01 Ghulam | Core/Haris | native | — | all | 0–1 | — |
| Govad | FT-02 Bahram | Core/Haris/Duo | required | Bahram | all | 0–5 | Required-choice set |
| Avicenna | FT-01 Ghulam | Core/Haris | native | — | all | 0–1 | — |
| Avicenna | FT-03 Shakush | Duo | native | — | all | 0–1 | — |
| Sayiq | FT-01 Ghulam | Core/Haris | native | — | all | 0–1 | — |
| Sayiq | FT-03 Shakush | Duo | native | — | all | 0–1 | — |
| Lasiq | FT-02 Bahram | Core/Haris/Duo | required | Bahram | all | 0–3 | Required-choice set |
| Bokhtar | FT-02 Bahram | Core/Haris/Duo | required | — | FTO opts 1,2,5,6 | 0–2 | Required-choice set |
| Shakush | FT-03 Shakush | Duo | native | — | all | 1–2 | Anchor |
| Asawira | all eligible main teams | varies | wildcard | — | all | max 3 | — |
| Yasbir | all eligible main teams | varies | wildcard | Ghulam; Bahram | FTO opt 1 only | max 1 | — |
| Leila Sharif | all eligible main teams | varies | wildcard | Ghulam; Bahram | all | max 1 | — |
| Yara Haddad | all eligible main teams | varies | wildcard | — | all | max 1 | — |
| Husam Spec-Ops | FT-01 Ghulam | Core/Haris | special | — | Spec-Ops mode | 0–1 | Not standard matched play |

## Reinforcements

The pinned Hassassin Bahram source links **Reinforcement Army ID 499**. Its roster and Fireteam chart are a distinct Reinforcement context and are deliberately not merged into the Army 402 main roster or Fireteam definitions above. No Main/Reinforcement mixing exception is inferred.

## Validation

Validated against the pinned structured source before marking `status: current`:

1. All 33 standard roster units whose source faction membership includes Army 402 are represented.
2. Husam Spec-Ops and Haqqislam Team-Ops are separated from the standard roster as optional game-mode hooks.
3. Generic mercenary catalogue entries with `factions: []` are excluded.
4. Standard loadout IDs, points, SWC, AVA, and profile distinctions are preserved.
5. The complete main Fireteam chart is represented: Ghulam, Hassassin Bahram, Shakush, and Wildcards.
6. Bokhtar and Yasbir FTO restrictions reference existing options.
7. Rafiq FTO and Claire Lazhari FTO are not granted Fireteam access without a source chart row.
8. Counts-as comments and required-choice semantics are preserved explicitly.
9. The reverse Unit → Fireteam index is consistent with the canonical Fireteam definitions.
10. Reinforcement Army 499 is kept separate from the main chart.

## Provenance

- Corvus Belli Army source revision: `7.26246.158`
- Army source snapshot: `massayoshi/infinity-army-backup@n5/hassassin-bahram/7.26246.158.json`
- Snapshot repository commit: `d4329bb596ffea5d568eb2435f74366c305a7630`
- Army data changed on: 2026-09-03
- InfinityDB baseline commit: `4e2662be3f43387fbae42b3790a711b3e98570c4`
- Fireteam source: pinned Army `fireteamChart`, normalized according to repository Fireteam conventions
- Generated/verified: 2026-10-15
