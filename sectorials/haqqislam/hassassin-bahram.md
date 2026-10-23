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

## Community tactics — transcript-backed N5 research (2026-10-22)

> **Evidence status:** The roster, profiles, equipment, points, AVA, and Fireteam chart **above** remain the N5.3 / Army `7.26246.158` authority. Everything below is *community tactical assessment*, not official rules or a change to the reference data. Several reviewed videos/podcasts predate the October 2025 N5.2 update and September 2026 Army snapshot; use their reasoning, **not their historical points or Fireteam claims**, where they disagree with the reference.

### One-minute read

- **Win asymmetrically:** Bahram is strong at attacking an opponent's *weak* piece from an unexpected angle, not at outshooting the enemy's best gunfighter. Create bad choices with Impersonation, hidden threats, mines, jammers, smoke and cheap AROs.
- **Three viable list identities:** (1) *Ambush/denial:* Shujae, Áyyār, Nadhir, Daylami, Sunduqbut; (2) *Professional Fireteam:* Ghulam + Barid smoke/pitchers, Asawira, Muyib/Govad/Lasiq; (3) *Hybrid:* some hidden threats **plus** a mobile gunfighter or Shakush. Building both tournament lists with differing offensive/defensive emphasis is more useful than treating one archetype as compulsory.
- **Hidden Deployment is not free:** A hidden unit generates **no Order while hidden**, and the Shujae/Áyyār/Nadhir lack Camouflage to re-conceal safely after revealing. Predict routes, do not reveal merely because a target appears, and budget active-turn Orders based on *visible* Regular troops.
- **Protect Order economy:** Cheap Daylami and Ghazi are excellent, but their Irregular/Impetuous Orders do not replace a workable Regular pool. Link some utility, keep specialists, and ensure pricey models get enough Orders to earn their cost.

### Building blocks — what they accomplish and why

| Block / options in current roster | Why take it | Limit / execution |
|---|---|---|
| **Ghulam NCO Smoke LGL + 1–2 Barids** (plus Ghulam anchor where needed) | Spends an otherwise idle Lieutenant Order on smoke; linked pitchers become more reliable, expanding cheap hacking and objective-control reach. Barid KHD can contest hostile hackers. | Not elite hacking or a dominant long-range gun team; don't overpay for link fillers. Review N5.3 Fireteam chart above for legal composition. |
| **Ghulam doctor + Asawira** | Low-cost Fireteam framework around a real active-turn HI; Asawira Doctor (+3) adds fighting and recovery in one slot. | Don't expose the whole link just to feed the Asawira one fight. |
| **Fiday / Hussein Al-Djabel** | Impersonation allows targeting an isolated Lieutenant, hacker or one-Wound support piece without crossing the board conventionally; Al-Djabel is the pricier close-combat specialist. | Not a reliable answer to a TAG or enemy CC specialist. WIP 15 enemy-DZ deployment risks failure; consider deploying outside the DZ and approaching while Impersonated. Reserve until key counters are visible. |
| **Shujae SMG + Flammenspeer + E/M Mine Minelayer (2)** | Hidden, Forward Deployment (+20), Mimetism (-6), specialist: a concealed template threat with mines constrains movement, then can score. Other Shujae profiles can hunt with AP/Viral weapons. | Predict placement and use patience; once revealed the 1-Wound unit is vulnerable. |
| **Áyyār Hidden Deployment + Triangulated Fire** | Surprise Attack (-6), Specialist Operative and high-impact AP/Breaker/Thunderbolt options punish a carefully selected opening; one of N5's distinctive ambush investments. | Roughly 38–40 points; limited protection after reveal and no automatic permission to win a poor gunfight. Strong player-skill dependency. |
| **Nadhir SMG + Flammenspeer (20 pts)** | Affordable hidden Forward Observer and disposable area-denial attack without spending Áyyār money. | Other Nadhir options compete with Shujae/Áyyār. Viral Minelayer is situationally useful for a different mine threat, but relatively costly. |
| **Daylami Panzerfaust / Camouflage (1 Use) Panzerfaust** | Low-cost disposable long-range threat; several force opponent to spend Orders removing or routing around them. Camo/Infiltration option pressures midfield. | Irregular Orders and low resilience. Don't sacrifice the entire Regular pool to maximize AVA. |
| **Ghazi Muttawi'ah Jammer / E/Marat / Smoke** | Cheap, expendable close-area denial against expensive pieces; jammer and E/Marat threaten threats that do not care about ordinary rifles. | Impetuous and Irregular; smoke isn't a license to feed them into MSV or templates. Some guides prefer pricier 8-point BSG+Jammer+Smoke for flexibility over 5–6 point basics. |
| **Lasiq Viral Sniper Duo / Viral Marksman Rifle** | Mimetism, Marksmanship, X-Visor and the Fireteam die improve unfavorable range/cover exchanges; sniper threatens longer lanes, AP Viral Marksman better works mid-range or actively. A specialist/Leila partner adds utility. | Competes for points/position with Govad, Sunduqbut and hidden defenders; no blanket best weapon choice. |
| **Muyib Tactical Awareness HRL or Spitfire + utility partner** | Flexible attack/ARO link with extra personal Order and useful doctor/FO/smoke/minelayer options. Bahram Duo can put specialist alongside main gun. | One-Wound gunfighters and spending SWC on too many short-range pieces reduce resilience. |
| **Bokhtar FTO + Yara Strategic Deployment** | Super-Jump (Jet Propulsion), MSV1, Tactical Awareness and forward positioning can create an aggressive, mobile specialist/striker module. | Expensive; an attacking Bokhtar **Lieutenant** merits the Farzan Chain of Command. FTO-only restrictions apply to Bahram teams. |
| **Sunduqbut Neurocinetics + Camo (1 Use)/Decoy** | A deceptive durable ARO marker: Feuerbach for armor/range, Viral for BTS targets, or AP Spitfire; forces awkward early enemy Orders and uncertainty. | Can be smoked out/hacked/isolated once exposed; active versions compete with cheaper specialist or Lasiq Fireteam choices. |
| **Farzan Chain of Command** | Camo/Infiltration specialist safeguards aggressive Lt plans and still scores or threatens objectives. | Adds cost; optional if running a deliberately safe rear-area Lt. |
| **McMurrough / Ragik** | McMurrough provides immediate smoke, jumping and dangerous melee pressure; Ragik offers off-table AD attack or a specialist hacker entry angle. | McMurrough is Irregular/Impetuous; Ragik's off-table Regular Order/timing must be incorporated into planning. |

### TAG, support REMs, and Vehicle availability (Army 402 only)

| Actual Bahram option | Practical role and reason | Caveat |
|---|---|---|
| **Shakush TAG** — 58-point Continuous Damage HMG or 56-point AP Spitfire; AVA 2 | BS14, ARM6, 3 STR, Tactical Awareness and included **Jandab** ancillary specialist offer an affordable self-sufficient mobile gun platform/objective pressure. HMG favors sustained lanes; AP Spitfire closer armor work. | Cannot solve everything by frontal aggression; high Silhouette, low count and predictable route. Compared with several excellent 20–40-point infantry, 56–58 points buys fewer separate threats. |
| **Shakush Duo** — Sayiq, Muyib, Avicenna or another Shakush per FT-03 | **Sayiq (9 pts)** supplies TAG-support GizmoKit/specialist utility; Muyib offers a wider tool kit. Jandab is an *included ancillary*, not an independently purchased REM. | A Duo is *optional*, not automatically best; **Hafza+Shakush** is discussed for **Vanilla Haqqislam** only and is **not** a legal Bahram Fireteam combination. |
| **Rafiq** 13-point FO/Sensor/Triangulated Fire Repeater; 19-point Red Fury FTO | Fast objective cleaner, Sensor against camouflage and a repeater projecting hacking; FTO profile trades points/SWC for anti-infantry shooting. | **Rafiq FTO cannot join a Bahram Fireteam** under the actual main chart despite the FTO label. |
| **Kameel** 8-point Baggage/Repeater, 14-point EVO, 16-point Total Reaction Rifle | 8-pointer is Order-efficient repeater/Baggage utility; EVO for a specific supportware/AD plan; 16-point Total Reaction option covers shorter lanes while sustaining the support network. Baggage supports reload-dependent plans. | EVO is not mandatory: buy its capability only if the army uses it. |
| **Fanous** 7-point Flash Pulse/Repeater | Very inexpensive Regular Order, emergency ARO and backfield hacker-network node. | Single REM isn't a complete defensive architecture; AVA 1. |
| **Shihab** 23-point HMG / 18-point Thunderbolt (+1B) Total Reaction + 360° Visor | Durable-in-Orders static long-lane deterrent on a cheap REM body; HMG for sustained open firing, Thunderbolt for a different weapon/point bracket. | Choose covered, overlapping deployment; still vulnerable to coordinated exposure, smoke and hard counters. |
| **Shaytaniyah** 16-point **Guided** Missile Launcher / 19-point **(+1B)** Missile Launcher | Guided loadout is meaningful **only with a real Targeted/Repeater plan** (Barid, FO, etc.). Burst-enhanced alternative is a different ARO/fire role. | Do **not** assume the 19-point option also has Guided; pinned Army lists Guided on the 16-point option only. |
| **Nasmat** 3-point servant | Extends Najjarun/doctor support reach without moving the parent specialist to the exposed repair/healing target. | Peripheral, **no Order**. |
| **Vehicle (VH)** | **None in the pinned 33-unit Bahram main roster.** | **Haytham**, **Shaykh Bakr**, and other vehicles discussed for *Vanilla* or other Haqq sectorials are **not** Bahram options merely because they share a faction. Confirm a new Army revision before changing this conclusion. |

**Repair/support sequence:** If taking Shakush, evaluate Jandab positioning, a Najjarun Engineer (possibly with Nasmat), Kameel Baggage/Repeater and Barid/Fanous network. Each piece has a separate job; do not add all of them automatically. TAG order/STR density and mission dictate support investment.

### Real disagreements — retain both sides

- **Shakush value:** *Positive:* Robert Shepherd's later Vanilla review finds the cheap BS14 Continuous Damage HMG TAG efficient; Jandab/Sayiq give objective and support coverage in Bahram. *Negative:* Tactical Awareness's N5 HB panel jokes that a Shakush slot is often better spent on **several more troops** or exceptional Asawira/Áyyār/Bokhtar/Sunduqbut, while Musterkrux (April 2026) finds TAG Duos mostly inefficient. **Resolution:** pick Shakush for a specific gun/lane/mission need, not as a Bahram auto-include; avoid transplanting Vanilla Hafza-Duo praise into Bahram.
- **Defense saturation vs usable Orders:** Tactical Awareness's Owen showcases an extreme defense-heavy low-Regular-Order tournament-winning list; Robert Shepherd/Musterkrux caution that Hidden Deployment plus Irregulars can starve your active turn. **Both valid:** saturation can deny a specific opponent, but count actual usable Orders *before* an ambush reveals.
- **Lasiq vs Sunduqbut vs Govad:** Lasiq advocates favor linked Mimetism/Marksmanship/Viral at range; Sunduqbut advocates prefer Decoy/Camo/Neurocinetics resilience and threat ambiguity; Govad advocates value MSV1/Combat Instinct/Warhorse in a link. Pick based on expected range, cover and opponent tricks rather than a universal ARO champion.
- **Avicenna vs Asawira Doctor:** Some hosts regard a 28-point dedicated Doctor as poor value beside an Asawira Doctor that can also fight; she still offers a fast WIP15 Doctor (+3), NWI and unusual survival package where that matters. No universal verdict.
- **Nadhir vs Shujae/Áyyār:** Cheap 20-point hidden FO has a real scoring/Flammenspeer niche; higher-budget hidden options have scarier kill/reveal potential. Mixing types helps force mistaken enemy assumptions.
- **Accessibility:** DDDDan describes one of the best defensive factions; Counterintelligence calls the defenses easy to *access* but hard to *pilot well* on offense. Hidden Deployment/Impersonation timing and which enemy piece to scalp create the learning curve.

### Source shortlist and transcript coverage

**Primary tactical sources (full MCP transcripts reviewed):**

1. **[Tactical Awareness S3 E31 — Hassassins Bahram (2025-08-15)](https://www.youtube.com/watch?v=63MLOgyNONs)** ([podcast](https://open.spotify.com/episode/4XI4lNMzeeye2Go6DbjcSi)). Most useful contrasting lists/opinions: ~25–45 min defensive layering, Sunduqbut, Shujae; ~45–65 min linked Ghulam/Barids, Áyyār and Shakush argument; ~65–90 min Bokhtar, Lt/CoC, Lasiq, Avicenna and Nadhir. **Predates N5.2.**
2. **[Robert Shepherd — Infinity N5 Faction Focus: Hassassin Bahram (2025-04-13)](https://www.youtube.com/watch?v=yHpAnRDw_E8)**. Best conceptual *why*: ambush vs Camouflage, hidden Orders, linked smoke/pitchers, limits of top-end gunfighting. **Predates N5.2.**
3. **[Counterintelligence Episode 3 — Hassassin Bahram (2025-02)](https://www.youtube.com/watch?v=Yqy3FwN7hjQ)**. Counterpoint on novice accessibility, Fiday/defense, specialist and link modules. **Predates N5.2.**
4. **[DDDDan Infinity — You Should Play Hassassins Bahram / purchase guide (2025-02)](https://www.youtube.com/watch?v=99hNbURNX30)**. Concise role and collection perspective, 15-troop/defense play and warning on technical Fiday/Áyyār.
5. **[Robert Shepherd — Infinity N5 Faction Focus: Vanilla Haqqislam (late 2025)](https://www.youtube.com/watch?v=Dmv4pfdTbc0)**. Reviewed for *shared* Shakush/REM utility and **Vanilla-only** TAGs/VHs; not a source for Bahram legal roster.
6. **[Tactical Awareness — N5 V5.2 balance update (2025-10-16)](https://open.spotify.com/episode/66UWrxKSTHcyWP3LJDM0H4)**. Full transcript reviewed for patch context (including pitcher changes); use current repository N5.3 rules/profile data rather than repeating period-specific claims.
7. **[Tactical Awareness — Haqqislam Prime N5 (2025-10-13)](https://open.spotify.com/episode/4gx0VBfits4q9PNwUiPIJh)**. Full transcript checked for shared-unit/vanilla context, not Bahram Fireteam legality.

**Additional useful sources (not used as transcript-grounded claims above):**

- **[Musterkrux — Infinity Faction Focus: Hassassin Bahram (2026-04-15)](https://www.tabletopbattles.com/infinity-faction-focus-hassassin-bahram)**. More recent written faction review with explicit linked loadout ideas, Shakush Duo skepticism and two example lists; article reviewed directly.
- **[Yellow Snake / GloriousEND — Hassassin Bahram N5 (Russian, 2025-11-13)](https://open.spotify.com/episode/1bXInrJXMyynx2r4zn3lxy)**. Unit-by-unit audio with **Shakush 48:41; Kameel 1:21:12; REMs 1:23:18**; podcast metadata/chapters checked, but transcript **not obtainable from MCP**, so no opinions attributed to it.
- **[Tactical Awareness S1 Hassassin faction guide (2023, N4)](https://www.youtube.com/watch?v=zDwdPdy0GjE)**. Historical context only; not evidence for N5.3 profiles or points.

## Command-unit apex/value cross-reference (2026-10-23)

**Farzan CoC 24/0** is among the strongest multi-role backups: Camouflage/infiltration/mine-and-mission value protects an **active Bokhtar or other expensive LT** while still scoring. A cheap Ghulam commander is viable when exposure is low; don't pay for CoC only to throw the Farzan away as first assault. **Saladin's Vanilla Haqq list-wide Inspiring engine is not automatically available to Hassassins.**

See [cross-faction Lieutenant, CoC and Order package tiers](../../notes/list-building/command-units-apex-and-value.md). **Current roster and canonical Fireteam chart above remain authoritative.**

## TAG tactical cross-reference (2026-10-23)

**Shakush (56–58)** is particularly useful *here* because Hassassin often needs a durable, reliable ranged attack/long-gun anchor. The HMG Continuous Damage threatens repeated failed saves; AP Spitfire is for armored targets at shorter bands. **Disagreement:** the 2025 TAG podcast ranks Shakush modestly against other TAGs, but Haqq players argue its **sectorial role scarcity** makes it much better than a global head-to-head comparison suggests.

For the two-tier **apex/points-value** comparison, TAG counterplay, matchup matrix and direct transcript sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Treat current profiles, points/SWC and canonical Fireteam data above as authoritative.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Barid KHD+Pitcher 14/0 versus HD+Pitcher 16/0.5**, both WIP14, is a premier infowar return for points. **Leila Sharif 22/0 KHD+Carbonite+Firewall(-3) and Combat Instinct** combines KHD Trinity, anti-HI control and stealth-proof reactive network defense in a permitted team. **Hassassin Govad KHD 23/0 or HD 25/0.5** supports a fighting link and WIP14, while **Ghulam HD16/0.5** is the cheap second ordinary HD. **Ragik WIP15 HD25/0.5** provides Combat Jump mission reach but cannot defend the board in Turn 0. **Why:** Barid is a low-cost Pitcher/specialist; Leila is a resilient hybrid network guard. Buying extra standard HDs without Hunzakut/Repeater reach is not added cyber control.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

Cross-faction [apex and cost-value Order-generator rankings](../../notes/list-building/cheerleaders-and-order-generators.md), circumstance guide and transcript disagreements. **This file remains authoritative for profiles, AVA, Training and Fireteam legality.**

- 7pt Fanous — Regular Flash/Repeater REM with Mimetism; excellent cheap network but limited S3 concealment.
- 8pt Kameel — Baggage/Repeater/Deactivator and Regular Order, particularly valuable with disposable launchers.
- 11pt Ghulam — S2 protected Regular Order; FO/Doctor/deployable repeater profiles can earn their premium.
- Barid FO/Pitcher — combines Regular Order, forward objective access and a mobile network projection threat.
- Ghazi Muttawi'ah — normally Irregular smoke/Jammer/E-M cheap defender; only count as pool Order with current legal conversion.

**When to pick:** Prefer transferable, safe Regular Orders when the Combat Group needs fuel; choose the higher-priced option only when its smoke, template, weapon, repeater, Fireteam function or scoring ability has a real job. Do not count Irregular/Impetuous/Tactical/Lieutenant Orders or Peripheral bodies as interchangeable Regular pool Orders; account for DZ footprint and link/enabler package costs.


## ARO apex/value cross-reference (2026-10-23)

The [N5.3 cross-faction ARO apex/value and matchup study](../../notes/list-building/aro-units-apex-and-value.md) compares hidden missile traps, Neurocinetics/TR, cheap templates/mines, DZ guards and conflicting creator opinions. Consult the **roster and Fireteam chart above** for legally available profiles, SWC, Training and AVA.

- **Sunduqbut Neurocinetics Feuerbach** — 47pt/1.5SWC durable hidden/ambush-capable long-lane anchor with serious armor punch; expensive if easily bypassed
- **Nadhir Flammenspeer/Panzerfaust** — cheap-to-medium concealed route trap; choose timing, not first possible shot
- **Daylami Panzerfaust** — 6pt/0SWC Irregular disposable defense, or 8pt Camo(1 use)/Infiltration; outstanding trading value, not reliable continuous lock
- **Ghazi Chain Rifle/E-M/Jammer** — ~5–6pt Irregular close-area screen, punishing TAG, Assassin and hacker routes; no general shared Regular Order
- **Warcor Flash** — 3pt Irregular ARO tax/late-game Stun attempt, not a Regular Order

**Practical deployment:** put cheap disposable/Flash/DTW or mine pressure on the approach; retain a separate unseen or recoverable threat for the decisive square; avoid exposing a premium active attacker and check opponent Smoke, MSV, hacking, AD and pie-slicing. No automatic order from an off-table Hidden model; Irregular ARO units do not supply generic Regular Orders.
