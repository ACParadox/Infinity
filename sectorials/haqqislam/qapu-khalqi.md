---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 403
sectorial_slug: qapu-khalqi
sectorial_name: Qapu Khalqi
parent_faction: Haqqislam
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Qapu Khalqi roster, standard loadouts, canonical Fireteam chart, reverse Fireteam index, and the distinct Melek Reaction Group Reinforcement Fireteam chart. Husam Spec-Ops and Haqqislam Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# Qapu Khalqi

## Overview and provenance

Repository-native reference for **Qapu Khalqi (QK)** roster, profiles, points/SWC, AVA, and Fireteam access.

Sources used:

- Army-derived Qapu Khalqi source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `d4329bb596ffea5d568eb2435f74366c305a7630`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **38-unit standard Qapu Khalqi roster** and the complete standard Qapu Khalqi `fireteamChart` in the pinned Army source.
- Army metadata currently marks **Qapu Khalqi as discontinued**, but a complete N5 roster and Fireteam chart remain present in the current Army data. `status: current` above means current with the pinned N5 data, not that the sectorial is non-discontinued.
- `Husam Spec-Ops` and `Haqqislam Team-Ops` are optional game-mode content and are listed separately.
- Generic Soldier of Fortune / `merc-*` catalog entries with an empty source faction list are excluded from the base roster, including duplicate mercenary copies of troops that already have ordinary Qapu entries.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name by itself. In particular, `Fiddler FTO` and `CLAIRE LAZHARI FTO` are **not** granted Qapu Fireteam access because neither unit appears in the current Qapu Fireteam chart.
- `KORSAN FTO` and `RAFIQ REMOTE FTO` are profile-sensitive Fireteam entries and only those profiles receive the chart access described below.
- Parenthetical Army-chart comments are treated as Counts-as / equivalence labels, not as join-scope restrictions.
- Multiple `required: true` rows in Qapu Khalqi, Zırhlı, and Bekçileri Fireteams are preserved as **required-choice sets**. This file does not reinterpret them as requiring one model from every marked row simultaneously.
- The Zırhlı chart independently lists `SCARFACE` and `CORDELIA TURNER` as required-choice rows. Army-list composition of the Scarface & Cordelia entry remains governed by its bundled two-model unit options; this reference does not invent a way to buy those profiles separately.
- Linked Reinforcement army ID: **499**, **Melek Reaction Group**. Its Fireteam chart is recorded separately and is not merged into the standard Qapu chart.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Qapu Khalqi (QK) |
| Parent faction | Haqqislam |
| Army ID | 403 |
| Army slug | `qapu-khalqi` |
| Army metadata status | Discontinued |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 38 |
| Optional-mode units | Husam Spec-Ops; Haqqislam Team-Ops |
| Reinforcement roster | Melek Reaction Group, Army ID `499` |
| Fireteam limits | Core 1; Haris 2; Duo unlimited |
| Fireteam chart | yes |

## Roster index

| Unit | ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| Nasmat Remotes | 333 | 2 | REM | Peripheral | — |
| Fanous Remotes | 318 | 3 | REM | Regular | — |
| Djanbazan Tactical Group | 306 | 5 | MI | Regular | Qapu Khalqi required-choice |
| Al Hawwa' Unit | 331 | 3 | SK | Regular | — |
| Shaytaniyah Remotes | 317 | 1 | REM | Regular | — |
| Wild Bill | 1482 | 1 | LI | Regular | Bekçileri max 1 |
| Kaplan Tactical Services | 338 | 5 | MI | Regular | Bekçileri required-choice |
| Ghulam Infantry | 301 | TOTAL | LI | Regular | Ghulam |
| Mobile Brigada | 382 | 1 | HI | Regular | — |
| Dr. Claire Lazhari | 1894 | 1 | LI | Regular | —; FTO profile name alone does not grant access |
| Shihab Remotes | 316 | 2 | REM | Regular | — |
| Kameel Remotes | 334 | 2 | REM | Regular | — |
| Triphammer | 1569 | 2 | TAG | Regular + Tactical Awareness | Zırhlı required-choice |
| Fiddler | 1564 | 1 | LI | Regular | —; FTO profile name alone does not grant access |
| Sekban, Naval Special Unit | 339 | 5 | MI | Regular | Ghulam; Qapu Khalqi required-choice; Bekçileri |
| Laxmee | 1344 | 1 | LI | Regular | Wildcard; counts as Qapu Khalqi / Janissary |
| Druze Shock Teams | 379 | 5 | MI | Regular | Druze Bayram Security |
| Hafza Unit | 326 | 4 | LI | Regular | Wildcard; multiple counts-as labels |
| Warcor | 50 | 1 | LI | Irregular | — |
| Corregidor Alguaciles | 296 | 4 | LI | Regular | Ghulam max 4 |
| Odalisques | 324 | 5 | LI | Regular | Ghulam; Qapu Khalqi required-choice; Zırhlı; Bekçileri |
| Iguana Squadron | 383 | 1 | TAG | Regular + Tactical Awareness | Zırhlı required-choice |
| Najjarun Engineer | 314 | 1 | LI | Regular | — |
| Medical Specialist Rahman Rouhani | 1549 | 1 | LI | Regular | Wildcard |
| Security Chief Arslan | 986 | 1 | MI | Regular | Druze max 1; counts as Druze |
| Burkut | 1759 | 3 | HI | Regular | Wildcard; counts as Qapu Khalqi |
| Freelance Operator Samsa | 1683 | 1 | MI | Regular | — |
| Zeybek Aero-unit | 1852 | 1 | VH | Regular | — |
| Azra'il | 330 | 3 | HI | Regular | Qapu Khalqi required-choice |
| Scarface & Cordelia | 380 | 1 team | TAG + LI | 2 Regular + Tactical Awareness | Zırhlı required-choice rows for Scarface / Cordelia |
| Rafiq Remotes | 315 | 1 | REM | Regular | Wildcard, FTO profile only; counts as Qapu Khalqi / Janissary |
| Husam Operative Leila Sharif | 849 | 1 | LI | Regular | Wildcard; counts as Ghulam |
| Korsan, Corsairs of the Gate | 1758 | 3 | LI | Regular | Wildcard, FTO profiles only |
| Sayiq TAG Support Pilots | 1849 | 1 | LI | Regular | — |
| Yuan Yuan | 378 | 3 | WB | Irregular + Impetuous | — |
| Shakush Light Armored Unit | 1546 | 2 | TAG | Regular + Tactical Awareness | Zırhlı required-choice |
| Janissaries | 308 | 5 | HI | Regular | Bekçileri required-choice |
| Bashi Bazouks | 325 | 4 | LI | Irregular | — |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Husam Spec-Ops | 1916 | Spec-Ops | Ghulam Fireteam row, max 1 when Spec-Ops mode is used |
| Haqqislam Team-Ops | 1930 | Team-Ops | No ordinary Qapu Fireteam row |

## Unit details

### Nasmat Remotes

**ID 333 · AVA 2 · REM** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Servant Peripheral support REM.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | PARA CC Weapon; Servant | — |

### Fanous Remotes

**ID 318 · AVA 3 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater utility REM.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | Flash Pulse, PARA CC Weapon; Repeater | — |

### Djanbazan Tactical Group

**ID 306 · AVA 5 · MI** — `MOV 10-10 | CC 14 | BS 12 | PH 11 | WIP 14 | ARM 3 | BTS 0 | W 1 | S 2`. MSV2, Regeneration (PH 13), Immunity (Shock).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 22 | 0 | Rifle, Light Shotgun, Pistol, CC Weapon | Qapu Khalqi required-choice |
| 2 | 31 | 1.5 | HMG, Pistol, CC Weapon | same |
| 3 | 27 | 0.5 | AP Sniper Rifle, Pistol, CC Weapon; BS Attack (Shock) | same |
| 4 | 27 | 0.5 | Rifle, Light Shotgun, Pistol, CC Weapon; Hacking Device | same |
| 5 | 26 | 0 | Rifle, Light Shotgun, Pistol, CC Weapon; MediKit, Doctor (+1) | same |
| 6 | 22 | 1 | Rifle, Light Shotgun, Pistol, CC Weapon; Lieutenant | same |
| 7 | 26 | 0 | Shock Marksman Rifle, Pistol, CC Weapon | same |
| 9 | 28 | 1 | Red Fury, Pistol, CC Weapon | same |

### Al Hawwa' Unit

**ID 331 · AVA 3 · SK** — `MOV 10-10 | CC 14 | BS 11 | PH 11 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Camouflage/infiltration specialist.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 0.5 | Boarding Shotgun, D-Charges, Cybermine, Silenced Pistol, CC Weapon; Hacking Device | — |
| 2 | 22 | 0.5 | Shock Marksman Rifle, Shock Mine, Silenced Pistol, CC Weapon; Minelayer | — |
| 3 | 19 | 0 | Boarding Shotgun, Flash Pulse, D-Charges, Silenced Pistol, CC Weapon; Forward Observer | — |
| 4 | 22 | 0 | Boarding Shotgun, D-Charges, Cybermine, Silenced Pistol, CC Weapon; Killer Hacking Device | — |
| 5 | 21 | 0.5 | Submachine Gun, Grenade Launcher, Shock Mine, Silenced Pistol, CC Weapon; Minelayer | — |

### Shaytaniyah Remotes

**ID 317 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Guided missile REM.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CC Weapon; Guided | — |
| 3 | 19 | 1.5 | Missile Launcher (+1B), PARA CC Weapon; Guided | — |

### Wild Bill

**ID 1482 · AVA 1 · LI** — `MOV 15-5 | CC 15 | BS 13 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 22 | 0 | Contender, MULTI Pistol (+1B), CC Weapon | Bekçileri max 1 |
| 2 | 24 | 0 | Rifle, MULTI Pistol (+1B), CC Weapon; BS Attack (Shock) | same |

### Kaplan Tactical Services

**ID 338 · AVA 5 · MI** — `MOV 10-10 | CC 15 | BS 12 | PH 11 | WIP 14 | ARM 2 | BTS 6 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | Combi Rifle, Adhesive Launcher Rifle, D-Charges, Boarding Pistol, CC Weapon | Bekçileri required-choice |
| 2 | 20 | 0 | Combi Rifle, Blitzen, Boarding Pistol, CC Weapon | same |
| 3 | 25 | 1.5 | MULTI Sniper Rifle, Boarding Pistol, CC Weapon | same |
| 4 | 20 | 1.5 | Heavy Rocket Launcher, Light Shotgun, Boarding Pistol, CC Weapon | same |
| 5 | 25 | 1 | Spitfire, Boarding Pistol, CC Weapon | same |
| 6 | 25 | 0 | Combi Rifle, Adhesive Launcher Rifle, D-Charges, Boarding Pistol, CC Weapon; Engineer | same |
| 7 | 24 | 0 | Combi Rifle, Blitzen, Boarding Pistol, CC Weapon; MediKit, Doctor | same |
| 8 | 21 | 0 | Combi Rifle, Blitzen, Boarding Pistol, CC Weapon; Specialist Operative | same |

### Ghulam Infantry

**ID 301 · AVA TOTAL · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 11 | 0 | Rifle, Light Shotgun, Pistol, CC Weapon | Ghulam 1–5 |
| 2 | 20 | 1 | HMG, Pistol, CC Weapon | same |
| 4 | 17 | 1.5 | Missile Launcher, Pistol, CC Weapon | same |
| 7 | 16 | 0.5 | Rifle, Light Shotgun, Pistol, CC Weapon; Hacking Device | same |
| 8 | 15 | 0 | Rifle, Light Shotgun, Pistol, CC Weapon; MediKit, Doctor (+1) | same |
| 9 | 12 | 0 | Rifle, Light Shotgun, Flash Pulse, Pistol, CC Weapon; Forward Observer | same |
| 10 | 13 | 0 | Rifle, Light Shotgun, E/M Mine, Pistol, CC Weapon; Deployable Repeater | same |
| 11 | 11 | 0 | Rifle, Light Shotgun, Pistol, CC Weapon; Lieutenant | same |
| 14 | 15 | 1 | Rifle, Grenade Launcher, Smoke Grenade Launcher, Pistol, CC Weapon; NCO | same |
| 18 | 12 | 0 | Rifle, Light Shotgun, Panzerfaust, Pistol, CC Weapon; Number 2 | same |
| 19 | 15 | 0 | Rifle, Light Shotgun, Pistol, CC Weapon; Lieutenant with enhanced command profile | same |
| 20 | 13 | 0 | Rifle, Light Shotgun, Pistol, CC Weapon; Commlink (+2), Specialist Operative | same |

### Mobile Brigada

**ID 382 · AVA 1 · HI** — `MOV 15-5 | CC 18 | BS 13 | PH 13 | WIP 13 | ARM 5 | BTS 3 | W 2 | S 2`. 360º Visor. **No Qapu Fireteam row.**

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 0 | MULTI Rifle, Boarding Pistol, CC Weapon; TinBot | — |
| 2 | 38 | 1.5 | HMG, Boarding Pistol, CC Weapon | — |
| 3 | 27 | 0 | Boarding Shotgun, Boarding Pistol, CC Weapon | — |
| 5 | 35 | 1.5 | Missile Launcher, Boarding Pistol, CC Weapon | — |
| 9 | 36 | 0.5 | Combi Rifle, D-Charges, Boarding Pistol, CC Weapon; Hacking Device, TinBot | — |
| 10 | 33 | 0 | MULTI Rifle, Boarding Pistol, CC Weapon; Lieutenant, TinBot | — |
| 11 | 27 | 0 | Boarding Shotgun, Boarding Pistol, CC Weapon; Lieutenant | — |

### Dr. Claire Lazhari

**ID 1894 · AVA 1 · LI** — `MOV 15-5 | CC 16 | BS 13 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Doctor utility character.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 0 | Breaker Combi Rifle, Nanopulser, Viral Pistol, PARA CC Weapon, Disco Baller; Doctor | — |
| 2 | 33 | 0 | **CLAIRE LAZHARI FTO**; same core kit with FTO-labelled Doctor profile | **No FT**: absent from canonical chart |

### Shihab Remotes

**ID 316 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. 360º Visor, Total Reaction.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 1 | HMG, PARA CC Weapon | — |
| 2 | 18 | 0 | Thunderbolt (+1B), PARA CC Weapon | — |

### Kameel Remotes

**ID 334 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 4`. Baggage support REM.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | PARA CC Weapon; Repeater/support package | — |
| 2 | 14 | 0.5 | PARA CC Weapon; EVO Hacking Device | — |
| 3 | 16 | 0 | Rifle, Light Shotgun, PARA CC Weapon; Total Reaction / support package | — |

### Triphammer, Repurposed Industrial TAG

**ID 1569 · AVA 2 · TAG** — Full Power `MOV 15-10 | CC 17 | BS 13 | PH 16 | WIP 12 | ARM 7 | BTS 3 | W 3 | S 7`; Battle Ravaged profile follows the Army damage-state entry. Tactical Awareness.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 53 | 1.5 | AP Spitfire, Heavy Flamethrower, AP CC Weapon | Zırhlı required-choice |
| 3 | 52 | 1.5 | AP Spitfire, Chain-colt (+1B), AP CC Weapon | same |
| 4 | 52 | 0 | Heavy Shotgun, Thunderbolt (+1B), AP CC Weapon | same |
| 5 | 48 | 0 | Heavy Shotgun, Heavy Rocket Launcher, Panzerfaust (+1B), AP CC Weapon | same |

### Fiddler

**ID 1564 · AVA 1 · LI** — `MOV 15-10 | CC 18 | BS 12 | PH 12 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Engineer with Jackbot variants.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 29 | 0 | **Fiddler FTO**; Contender, Drop Bears, D-Charges, Pulzar, PARA CC Weapon | **No FT**: absent from canonical chart |
| 2 | 36 | 0 | Fiddler plus 1 Jackbot | — |
| 3 | 43 | 0 | Fiddler plus 2 Jackbots | — |

### Sekban, Naval Special Unit

**ID 339 · AVA 5 · MI** — `MOV 10-10 | CC 17 | BS 13 | PH 11 | WIP 14 | ARM 3 | BTS 3 | W 1 | S 2`. 360º Visor, NCO.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Boarding Shotgun, Chain-colt, Pistol, CC Weapon | Ghulam max2; Qapu Khalqi required-choice; Bekçileri max1 |
| 2 | 27 | 1 | Red Fury, Chain-colt, Pistol, CC Weapon | same |
| 3 | 19 | 1.5 | Heavy Rocket Launcher, Chain-colt, Pistol, CC Weapon | same |
| 4 | 24 | 0 | AP Rifle, Light Shotgun, Chain-colt, Pistol, CC Weapon; Specialist Operative | same |
| 5 | 23 | 0 | Boarding Shotgun, Chain-colt, Pistol, CC Weapon; MediKit, Doctor (+1) | same |
| 6 | 24 | 0 | AP Rifle, Light Shotgun, Chain-colt, Pistol, CC Weapon; Lieutenant, Specialist Operative | same |
| 9 | 28 | 1.5 | Spitfire, Chain-colt, Pistol, CC Weapon | same |

### Laxmee

**ID 1344 · AVA 1 · LI** — `MOV 10-10 | CC 18 | BS 11 | PH 10 | WIP 14 | ARM 2 | BTS 6 | W 1 | S 2`. Hacker/network character.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 0.5 | Submachine Gun, Pitcher, Cybermine, D-Charges, Pistol, CC Weapon; hacking package | Wildcard max1; Qapu Khalqi / Janissary |

### Druze Shock Teams

**ID 379 · AVA 5 · MI** — `MOV 10-10 | CC 16 | BS 12 | PH 11 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. X Visor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 20 | 0 | Combi Rifle, Chain-colt, Viral Pistol, CC Weapon | Druze 1–5 |
| 2 | 28 | 1.5 | HMG, Chain-colt, Viral Pistol, CC Weapon | same |
| 3 | 21 | 0 | Combi Rifle, Chain-colt, Panzerfaust, Viral Pistol, CC Weapon | same |
| 4 | 24 | 1 | Combi Rifle, Chain-colt, Grenade Launcher, E/M Grenade Launcher, Viral Pistol, CC Weapon | same |
| 5 | 23 | 0 | Shock Marksman Rifle, Chain-colt, Viral Pistol, CC Weapon | same |
| 6 | 25 | 0.5 | Combi Rifle, Pitcher, D-Charges, Viral Pistol, CC Weapon; Hacking Device | same |
| 7 | 23 | 0 | Combi Rifle, Pitcher, D-Charges, Viral Pistol, CC Weapon; Killer Hacking Device | same |

### Hafza Unit

**ID 326 · AVA 4 · LI** — `MOV 10-10 | CC 14 | BS 12 | PH 10 | WIP 14 | ARM 2 | BTS 0 | W 1 | S 2`. Holomask.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 15 | 0 | Rifle, Light Shotgun, Pistol, CC Weapon | Wildcard max4 |
| 2 | 16 | 1.5 | Heavy Rocket Launcher, Assault Pistol, CC Weapon | same |
| 3 | 22 | 1 | Spitfire, Pistol, CC Weapon | same |
| 4 | 20 | 0 | Rifle, Light Shotgun, Pistol, CC Weapon; Chain of Command | same |
| 5 | 17 | 0 | Rifle, Light Shotgun, Flash Pulse, Pistol, CC Weapon; Deployable Repeater, Forward Observer | same |
| 6 | 15 | 0 | Rifle, Light Shotgun, Pistol, CC Weapon; Lieutenant | same |
| 9 | 19 | 0 | Rifle, Light Shotgun, Pistol, CC Weapon; Lieutenant (+1 Lieutenant Order) | same |

Counts as labels from the chart: **Ghulam, Qapu Khalqi, Odalisque, Sekban, Janissary**.

### Warcor

**ID 50 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular utility troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1–2 | 3 | 0 | Flash Pulse / Stun utility profiles | — |

### Corregidor Alguaciles

**ID 296 · AVA 4 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 10 | 0 | Combi Rifle, Pistol, CC Weapon | Ghulam max4 |
| 2 | 18 | 1 | HMG, Pistol, CC Weapon | same |
| 5 | 15 | 1.5 | Missile Launcher, Pistol, CC Weapon | same |
| 6 | 15 | 0.5 | Combi Rifle, Pistol, CC Weapon; Hacking Device | same |
| 8 | 12 | 0 | Combi Rifle, Flash Pulse, Pistol, CC Weapon; Deployable Repeater, Forward Observer | same |
| 9 | 12 | 0 | Combi Rifle, Pistol, CC Weapon; MediKit, Paramedic | same |
| 10 | 10 | 0 | Combi Rifle, Pistol, CC Weapon; Lieutenant | same |

### Odalisques

**ID 324 · AVA 5 · LI** — `MOV 15-5 | CC 19 | BS 12 | PH 10 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. Sixth Sense, No Wound Incapacitation, Combat Instinct.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4 | 19 | 0 | Submachine Gun, Contender, Pulzar, Pistol, PARA CC Weapon | Ghulam max2; Qapu required-choice; Zırhlı max1; Bekçileri max1 |
| 12 | 21 | 0 | Same core kit + Disco Baller | same |
| 13 | 24 | 0 | Rifle, Light Shotgun, Pulzar, Pistol, PARA CC Weapon; BS Attack (+1B) | same |
| 14 | 22 | 0 | Boarding Shotgun, Pulzar, Pistol, PARA CC Weapon; BS Attack (+1B) | same |
| 15 | 26 | 0 | Viral Marksman Rifle, Pulzar, MULTI Pistol, PARA CC Weapon; Marksmanship | same |
| 16 | 21 | 0 | Submachine Gun, Pulzar, Flash Pulse, Pistol, PARA CC Weapon; MediKit, Paramedic | same |

### Iguana Squadron

**ID 383 · AVA 1 · TAG** — `MOV 15-10 | CC 17 | BS 14 | PH 16 | WIP 13 | ARM 6 | BTS 6 | W 4 | S 7`. Tactical Awareness; ejection/operator mechanics per Army profile.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 64 | 1.5 | AP HMG, Heavy Flamethrower (+1B), CC Weapon; Mine Dispenser package | Zırhlı required-choice |
| 2 | 68 | 1.5 | AP HMG, Heavy Flamethrower (+1B), CC Weapon; alternate attack package | same |

### Najjarun Engineer

**ID 314 · AVA 1 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Engineer.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 15 | 0 | Rifle, Light Shotgun, D-Charges, Pistol, CC Weapon | — |
| 2 | 16 | 0 | Same + Deployable Cover | — |
| 3 | 17 | 0 | Same + Armed Turret (Rifle) | — |

### Medical Specialist Rahman Rouhani

**ID 1549 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 11 | PH 11 | WIP 15 | ARM 1 | BTS 6 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | Submachine Gun, Flash Pulse, Pistol, CC Weapon; MediKit, Doctor (+1) | Wildcard max1 |

### Security Chief Arslan

**ID 986 · AVA 1 · MI** — `MOV 10-10 | CC 17 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. MSV1, X Visor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 35 | 0 | MULTI Rifle, Light Shotgun, Viral Pistol, CC Weapon; Disco Baller | Druze max1; counts as Druze |
| 2 | 35 | 0 | Same; Lieutenant | same |

### Burkut

**ID 1759 · AVA 3 · HI** — `MOV 10-10 | CC 16 | BS 12 | PH 12 | WIP 14 | ARM 3 | BTS 6 | W 1 | S 2`. Engineer, GizmoKit, Deactivator, No Wound Incapacitation.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 28 | 0 | Boarding Shotgun, Panzerfaust, AP Mine, D-Charges, Pistol, CC Weapon | Wildcard max3; counts as Qapu Khalqi |
| 2 | 30 | 0.5 | Submachine Gun, Light Rocket Launcher, D-Charges, Pistol, CC Weapon | same |
| 3 | 26 | 0 | Submachine Gun, E/Marat, AP Mine, D-Charges, Pistol, CC Weapon | same |
| 4 | 28 | 0 | Submachine Gun, Heavy Flamethrower, AP Mine, D-Charges, Pistol, CC Weapon | same |

### Freelance Operator Samsa

**ID 1683 · AVA 1 · MI** — `MOV 15-5 | CC 15 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 0 | Plasma Rifle, D-Charges, Pistol, CC Weapon | — |

### Zeybek Aero-unit

**ID 1852 · AVA 1 · VH** — `MOV 20-5 | CC — | BS 13 | PH 12 | WIP 14 | ARM 5 | BTS 6 | W 3 | S 7`. Aerial vehicle profile.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 1.5 | AP Spitfire, Smoke Grenade Launcher; includes operator profile per Army entry | — |

### Azra'il

**ID 330 · AVA 3 · HI** — `MOV 10-10 | CC 15 | BS 13 | PH 11 | WIP 14 | ARM 5 | BTS 3 | W 2 | S 5`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 37 | 1.5 | AP HMG, Chain Rifle, AP Heavy Pistol, CC Weapon | Qapu Khalqi required-choice |
| 2 | 41 | 1.5 | Feuerbach, Chain Rifle, AP Heavy Pistol, CC Weapon; BS Attack (+1B) | same |

### Scarface & Cordelia

**ID 380 · AVA 1 team** — Scarface `MOV 15-10 | CC 22 | BS 13 | PH 16 | WIP 13 | ARM 7 | BTS 6 | W 3 | S 7`; Cordelia `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Army options bundle Scarface and Cordelia together and generate two Regular Orders plus Scarface's Tactical Awareness Order.

| Team opt | Pts | SWC | Scarface loadout | Included | FT |
|---:|---:|---:|---|---|---|
| 1 | 80 | 1.5 | Loadout Alpha: Mk12, Heavy Rocket Launcher, DA CC Weapon | Cordelia Turner | Zırhlı required-choice rows exist for Scarface and Cordelia |
| 2 | 76 | 1.5 | Loadout Beta: AP HMG, Panzerfaust, DA CC Weapon | Cordelia Turner | same |
| 3 | 76 | 1.5 | Loadout Gamma: AP Spitfire, Panzerfaust, DA CC Weapon | Cordelia Turner | same |

Cordelia is an Engineer with GizmoKit, Deactivator, D-Charges and her listed sidearms. The Fireteam chart names Scarface and Cordelia separately, but the roster entry does not make either a separately purchasable Army-list choice.

### Rafiq Remotes

**ID 315 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Sensor, Forward Observer, Remote Presence.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 13 | 0 | Rifle, Light Shotgun, Flash Pulse, PARA CC Weapon; Triangulated Fire | — |
| 3 | 19 | 0.5 | **RAFIQ REMOTE FTO**; Red Fury, Flash Pulse, PARA CC Weapon | Wildcard max1; counts as Qapu Khalqi / Janissary |

### Husam Operative Leila Sharif

**ID 849 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 22 | 0 | Shock Marksman Rifle, E/M Mine, D-Charges, Breaker Pistol, CC Weapon; Killer Hacking Device | Wildcard max1; counts as Ghulam |

### Korsan, Corsairs of the Gate

**ID 1758 · AVA 3 · LI** — `MOV 15-5 | CC 21 | BS 11 | PH 13 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Climbing Plus, Natural Born Warrior.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | **KORSAN FTO**; Chain Rifle, Heavy Pistol, Shock CC Weapon | Wildcard max3 |
| 2 | 18 | 0 | **KORSAN FTO**; Submachine Gun, Grenades, Heavy Pistol, Shock CC Weapon | same |
| 3 | 13 | 0 | **KORSAN FTO**; Chain Rifle, Drop Bears, Heavy Pistol, Shock CC Weapon | same |
| 4 | 16 | 0 | **KORSAN FTO**; Boarding Shotgun, Heavy Pistol, Shock CC Weapon | same |
| 5 | 16 | 0 | **KORSAN FTO**; Chain Rifle, Contender, Heavy Pistol, Shock CC Weapon | same |
| 6 | 21 | 0 | Submachine Gun, Grenades, Heavy Pistol, Shock CC Weapon; Forward Deployment | — |
| 7 | 21 | 0 | Boarding Shotgun, Heavy Pistol, Shock CC Weapon; Parachutist deployment profile | — |

### Sayiq TAG Support Pilots

**ID 1849 · AVA 1 · LI** — `MOV 10-10 | CC 16 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. TAG support/GizmoKit profile.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 9 | 0 | Shakush Pilot: Submachine Gun, D-Charges, Pistol, CC Weapon; GizmoKit / TAG support | — |

### Yuan Yuan

**ID 378 · AVA 3 · WB** — `MOV 10-10 | CC 22 | BS 10 | PH 14 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular, Impetuous airborne warband.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 6 | 0 | Chain Rifle, Smoke Grenades, Heavy Pistol, AP CC Weapon | — |
| 2 | 7 | 0 | Chain Rifle, Smoke Grenades, Pistol, DA CC Weapon | — |
| 3 | 11 | 0 | Boarding Shotgun, Smoke Grenades, Pistol, AP CC Weapon | — |
| 4 | 11 | 0 | Rifle, Smoke Grenades, Pistol, AP CC Weapon | — |

### Shakush Light Armored Unit

**ID 1546 · AVA 2 · TAG** — `MOV 15-5 | CC 17 | BS 14 | PH 14 | WIP 14 | ARM 6 | BTS 6 | W 3 | S 6`. Tactical Awareness.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 58 | 1.5 | HMG, Heavy Flamethrower, AP CC Weapon | Zırhlı required-choice |
| 2 | 56 | 1.5 | AP Spitfire, Heavy Flamethrower, AP CC Weapon | same |

### Janissaries

**ID 308 · AVA 5 · HI** — `MOV 10-10 | CC 18 | BS 14 | PH 14 | WIP 14 | ARM 4 | BTS 6 | W 2 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 31 | 0 | AP Rifle, Light Shotgun, Pulzar, Heavy Pistol, CC Weapon | Bekçileri required-choice |
| 2 | 38 | 1.5 | HMG, Pulzar, Heavy Pistol, CC Weapon | same |
| 4 | 28 | 0 | Boarding Shotgun, Pulzar, Heavy Pistol, CC Weapon; TinBot | same |
| 5 | 32 | 0 | AP Rifle, Light Shotgun, Pulzar, Heavy Pistol, CC Weapon; TinBot | same |
| 6 | 36 | 1.5 | Missile Launcher, Pulzar, Heavy Pistol, CC Weapon | same |
| 10 | 35 | 0 | AP Rifle, Light Shotgun, Pulzar, Heavy Pistol, CC Weapon; MediKit, Doctor | same |
| 11 | 31 | 0 | AP Rifle, Light Shotgun, Pulzar, Heavy Pistol, CC Weapon; Lieutenant | same |
| 12 | 32 | 0 | AP Rifle, Light Shotgun, Pulzar, Heavy Pistol, CC Weapon; Lieutenant, TinBot | same |

### Bashi Bazouks

**ID 325 · AVA 4 · LI** — `MOV 10-10 | CC 16 | BS 11 | PH 10 | WIP 12 | ARM 2 | BTS 0 | W 1 | S 2`. Irregular deception/airborne troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 13 | 0 | Contender, Boarding Pistol, CC Weapon | — |
| 2 | 14 | 0 | T2 Boarding Shotgun, Boarding Pistol, CC Weapon; AP attack package | — |
| 3 | 16 | 0 | Rifle, Light Shotgun, E/M Mine, Boarding Pistol, CC Weapon; Specialist profile | — |
| 5 | 14 | 0 | Breaker Rifle, Boarding Pistol, CC Weapon; Specialist profile | — |
| 8 | 12 | 0 | Submachine Gun, Boarding Pistol, CC Weapon; Specialist profile | — |

## Canonical Fireteam chart

Global Qapu Khalqi limits from Army revision `7.26246.158`:

- **Core:** 1
- **Haris:** 2
- **Duo:** unlimited (`256` sentinel in Army data)

### Ghulam Fireteams

**Types:** Core, Haris, Duo

| Entry | Min | Max | Counts as / restriction |
|---|---:|---:|---|
| GHULAM | 1 | 5 | — |
| ALGUACIL | 0 | 4 | — |
| ODALISQUE | 0 | 2 | Ghulam |
| SEKBAN | 0 | 2 | — |
| HUSAM | 0 | 1 | Spec-Ops only |

### Qapu Khalqi Fireteams

**Types:** Core, Haris, Duo

The four `required: true` rows form a **required-choice set**. They are alternative foundation entries, not a requirement to include all four troop families.

| Entry | Min | Max | Required-choice | Counts as |
|---|---:|---:|---|---|
| ODALISQUE | 0 | 5 | yes | Qapu Khalqi |
| SEKBAN | 0 | 5 | yes | Qapu Khalqi |
| DJANBAZAN | 0 | 5 | yes | — |
| AZRA'IL | 0 | 3 | yes | — |

### Zırhlı Fireteams

**Types:** Duo

The five marked rows are preserved as a **required-choice set**.

| Entry | Min | Max | Required-choice | Note |
|---|---:|---:|---|---|
| SHAKUSH | 0 | 2 | yes | — |
| TRIPHAMMER | 0 | 2 | yes | — |
| IGUANA | 0 | 1 | yes | — |
| SCARFACE | 0 | 1 | yes | Scarface profile belongs to bundled Scarface & Cordelia roster entry |
| CORDELIA TURNER | 0 | 1 | yes | Cordelia profile belongs to bundled Scarface & Cordelia roster entry |
| ODALISQUE | 0 | 1 | no | — |
| SEKBAN | 0 | 1 | no | — |

### Bekçileri Fireteams

**Types:** Core, Haris, Duo

Janissaries and Kaplans are the required-choice foundation entries.

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| JANISSARY | 0 | 5 | yes | — |
| KAPLAN | 0 | 5 | yes | — |
| ODALISQUE | 0 | 1 | no | Janissary, Kaplan |
| WILD BILL | 0 | 1 | no | — |
| SEKBAN | 0 | 1 | no | — |

### Druze Bayram Security Fireteams

**Types:** Core, Haris, Duo

| Entry | Min | Max | Counts as / note |
|---|---:|---:|---|
| DRUZE | 1 | 5 | — |
| ARSLAN | 0 | 1 | Druze |

### Wildcards

| Entry | Max | Counts as / profile restriction |
|---|---:|---|
| HAFZA | 4 | Ghulam, Qapu Khalqi, Odalisque, Sekban, Janissary |
| BURKUT | 3 | Qapu Khalqi |
| KORSAN FTO | 3 | FTO profiles only |
| RAFIQ REMOTE | 1 | **FTO profile only**; Qapu Khalqi, Janissary |
| LEILA SHARIF | 1 | Ghulam |
| ROUHANI | 1 | — |
| LAXMEE | 1 | Qapu Khalqi, Janissary |

Wildcards may join otherwise eligible Fireteams subject to the normal sectorial limits, counts-as labels, and profile restrictions above.

## Reverse Fireteam access index

| Troop / profile | Fireteam families | Notes |
|---|---|---|
| Ghulam | Ghulam | Native 1–5 |
| Alguacil | Ghulam | Max 4 |
| Odalisque | Ghulam; Qapu Khalqi; Zırhlı; Bekçileri | Ghulam max2; Qapu required-choice max5; max1 in Zırhlı/Bekçileri |
| Sekban | Ghulam; Qapu Khalqi; Zırhlı; Bekçileri | Ghulam max2; Qapu required-choice max5; max1 in Zırhlı/Bekçileri |
| Husam Spec-Ops | Ghulam | Max1; optional mode only |
| Djanbazan | Qapu Khalqi | Required-choice max5 |
| Azra'il | Qapu Khalqi | Required-choice max3 |
| Shakush | Zırhlı | Required-choice max2 |
| Triphammer | Zırhlı | Required-choice max2 |
| Iguana | Zırhlı | Required-choice max1 |
| Scarface | Zırhlı | Required-choice max1; bundled roster entry |
| Cordelia Turner | Zırhlı | Required-choice max1; bundled roster entry |
| Janissary | Bekçileri | Required-choice max5 |
| Kaplan | Bekçileri | Required-choice max5 |
| Wild Bill | Bekçileri | Max1 |
| Druze | Druze Bayram Security | Native 1–5 |
| Arslan | Druze Bayram Security | Max1; counts as Druze |
| Hafza | Wildcard | Max4; Ghulam/Qapu/Odalisque/Sekban/Janissary equivalence labels |
| Burkut | Wildcard | Max3; Qapu Khalqi |
| Korsan FTO | Wildcard | Max3; FTO profiles only |
| Rafiq Remote FTO | Wildcard | Max1; Qapu Khalqi / Janissary |
| Leila Sharif | Wildcard | Max1; Ghulam |
| Rouhani | Wildcard | Max1 |
| Laxmee | Wildcard | Max1; Qapu Khalqi / Janissary |

All standard roster units not listed in this reverse index have no Fireteam access in the pinned standard Qapu Khalqi chart. `Fiddler FTO` and `CLAIRE LAZHARI FTO` remain non-linkable here because the chart contains no corresponding unit row.

## Reinforcement Fireteams — Melek Reaction Group

Linked Reinforcement army: **Melek Reaction Group (Army ID 499)**, source revision `7.26246.158`.

These rows are intentionally separate from the standard Qapu chart. The pinned Reinforcement source exposes `spec` values of **Core 0; Haris 0; Duo 0** while its team rows explicitly declare Core/Haris/Duo eligibility. This reference preserves both facts rather than inventing non-zero global caps.

### Sekban Reinforcement Fireteams

**Types explicitly listed by Army:** Core, Haris, Duo

| Entry | Min | Max | Note |
|---|---:|---:|---|
| SEKBAN REINF. | 1 | 4 | — |
| ODALISQUE REINF. | 0 | 2 | — |
| HAKIM FTO REINF. | 0 | 2 | FTO profiles |
| KORSAN REINF. | 0 | 2 | FTO |
| HAWWA' REINF. | 0 | 2 | — |

### Azra'il Reinforcement Fireteam

**Type explicitly listed by Army:** Duo

| Entry | Min | Max | Note |
|---|---:|---:|---|
| AZRA'IL REINF. | 1 | 2 | — |
| HAWWA' REINF. | 0 | 1 | — |

### Reinforcement Wildcards

| Entry | Max | Counts as / note |
|---|---:|---|
| HAFZA REINF. | 2 | Sekban Reinforcement |
| BURKUT REINF. | 2 | Sekban Reinforcement |
| DJANBAZAN REINF. | 1 | — |
| RAFIQ REMOTE REINF. | 1 | — |
| LEILA SHARIF REINF. | 1 | — |
| ROUHANI REINF. | 1 | — |

Melek Reaction Group source units also include Reinforcement Al Hawwa, Nasmat, Hakim, Korsan, Odalisque, Sekban, Azra'il and the other entries referenced above. Reinforcement Wildcards are not merged into standard Qapu Wildcards.

## Validation notes

- Standard roster count reconciled to **38** ordinary Qapu Khalqi entries after excluding `Husam Spec-Ops`, `Haqqislam Team-Ops`, and generic empty-faction `merc-*` catalog entries.
- Army ID `403` is explicitly marked `discontinued: true` in the pinned N5 Army metadata; this reference nevertheless uses the complete current N5 roster and Fireteam data shipped for that Army ID.
- Every standard `fireteamChart` family from Army revision `7.26246.158` is represented: Ghulam, Qapu Khalqi, Zırhlı, Bekçileri, Druze Bayram Security, and Wildcards.
- Fireteam limits are preserved exactly for the standard sectorial: Core 1, Haris 2, Duo unlimited.
- Qapu Khalqi, Zırhlı, and Bekçileri `required: true` rows are preserved as required-choice sets rather than cumulative requirements.
- `KORSAN FTO` and `RAFIQ REMOTE FTO` profile restrictions are preserved.
- `Fiddler FTO` and `CLAIRE LAZHARI FTO` are not granted Fireteam access because the canonical Qapu chart contains no row for those units.
- The Scarface & Cordelia roster entry remains a bundled Army-list choice even though the Zırhlı chart names Scarface and Cordelia in separate rows.
- Linked Reinforcement army resolves to **Melek Reaction Group (499)**. Its chart is kept separate, including the unusual current source combination of `spec` values 0/0/0 and explicitly typed Fireteam rows.
- Source data and Fireteam normalization were rechecked on **2026-10-15** against the pinned Army snapshot and InfinityDB commit listed in the front matter.
