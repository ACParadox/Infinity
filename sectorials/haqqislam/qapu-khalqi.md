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

## Expanded faction tactical guide

For the full practical [Qapu Khalqi list-building and profile-selection guide](../../notes/factions/qapu-khalqi.md), see the dedicated tactical note. It consolidates the uploaded N5/N5.2 source leads, Holomask/command choices, small-team profiles and plays; **this roster remains authoritative**. Its N5.3 reconciliation explicitly preserves the current **Rafiq Remote FTO Wildcard** and the pinned **Odalisque/Sekban** skills.

## Community tactics — N5 transcript research (2026-10-22)

> **Status and precedence:** Tactical opinions only; keep the **N5.3 / Army 7.26246.158** roster, points, skills and **canonical Fireteam chart above** authoritative. Qapu Khalqi is **marked discontinued in the pinned Army metadata**, despite retaining the full 38-unit N5 reference. Most primary videos are August–September 2025 (**before** the October N5.2 update) and the original 2023 podcasts discuss **N4**. Their list compositions/point claims must be checked against the reference before reuse.

### Fast read: what wins, and why

- **QK = asymmetric combined-arms Fireteams:** choose one strong gun and economical linkable support; use **smoke versus ordinary shooters, White Noise versus appropriate MSV threats, AP/Continuous Damage versus armor, and airborne entries versus rear-zone defenses**. It is not a faction that typically wins by brute-force CC or elite statlines.
- **Prefer several small functional teams:** a gunfighter + NCO/specialist + Hafza often gets more useful jobs and Orders than a single cumbersome maximum Core. QK permits **one Core, two Haris, unlimited Duo**; don't build illegal three-Haris examples copied from older audio.
- **Default Lt shell game:** a **Hafza Lieutenant** uses Holomask and Fireteam flexibility to hide leadership. The **19-point (+1 Lt Order) option** can support an NCO plan; **20-point Chain of Command Hafza** protects a deliberately active Lt. Don't take several NCOs assuming one Lt Order can be spent multiple times.
- **Preferred guns are conditional:** **Azra'il** for sustained AP/high-impact damage; **Janissary** for BS14 and reliable modifier play; **Djanbazan** when smoke + MSV2 gets the useful matchup. You can field one or more, but each consumes SWC/Orders that could support scoring.
- **Midfield and close-combat are weaker than the roster breadth suggests:** Al Hawwa' and Samsa do useful scenario work, but not a deep hidden/camo midfield; Yuan Yuan and Bashi Bazouk give inexpensive disruptive entry angles, not dependable elite CC assassination.

### Unit and link module choices (current Army 403)

| Option | Why it works | When to leave it out / tactical limit |
|---|---|---|
| **Azra'il AP HMG (37) or Feuerbach (+1B) (41)** in Qapu Khalqi team | ARM5, 2W/S5, BS13; extreme AP firepower pressures HI/TAGs. AP HMG favors efficient active-turn Burst; Feuerbach threatens durable enemies at range and can contribute with other guns up close. | Does not have built-in Mimetism or a superior BS stat; fix poor matchups through White Noise, smoke, flanking, or attacking elsewhere. Robert prefers the cheaper HMG most often but likes both. |
| **Janissary HMG (38) / Missile Launcher (36)** in Bekçileri | BS14, 2W, ARM4/BTS6; a powerful, comparatively affordable infantry gun block that can include Hafza and support. TinBot Lt is a niche alternative to hidden Hafza if an active durable commander is needed. | 10-10 movement makes a full HI-heavy Core cumbersome; expensive to lose several team members. |
| **Djanbazan HMG (31) / AP Sniper (27)** in Qapu Khalqi team | MSV2 makes **Yuan Yuan/Ghulam smoke** into favorable vision-controlled shots; sniper is meaningful long-lane ARO, HMG more active. Regeneration offers some recovery. | BS12 and one Wound make them comparatively unreliable into units where smoke gives no advantage. Janissary may be the better consistent shooter; Warhorse/skill references in older videos must be checked against current profile. |
| **Hafza Lt / CoC / FO + gun** | Holomask reduces Lt identification, counts-as labels let an economical link support a premium shooter, and FO's deployable repeater extends hacking coverage. | Not an automatic *every team needs two Hafzas*: Fireteam same-type calculations must match current chart rather than historical commentary. |
| **Laxmee (24) + Leila Sharif / other hacker** | WIP14, BTS6 hacker with Pitcher/Cybermine package; Hacking Device Plus **White Noise** broadens approach into MSV guns while pitchers/repeaters threaten hackable pieces. Leila adds different hacker coverage. | Hackers are vulnerable if a projected repeater network is immediately counterattacked; manage support and don't overspend on a network that has no mission role. **Current Laxmee counts as Qapu Khalqi / Janissary, not Odalisque** (older transcript conflict). |
| **Sekban Doctor (23), Specialist (24), or cheap BSG (19)** | NCO converts an available Lt Order into team work, and linked Doctor (+1) restores important guns; 360°/short-range weapons help protect the link. | Often one is enough; their 1W baseline means they're more support than unbeatable spearheads. |
| **Burkut Engineer (26–30)** | NWI, ARM3/BTS6 plus engineering and E/Marat/mines/rockets give a chunky midfield-ready technician; also repairs support hardware. | Not cheap compared with a simple Engineer, and BS12 means not a premium gunfighter. **Current counts-as is Qapu Khalqi, not Sekban** (older transcript conflict). |
| **Odalisque Viral Marksman / Disco Baller / BSG** | NWI, Sixth Sense and useful direct/utility weapons create durable short/mid-range link filler with defenses many light specialists lack; Disco Baller adds a visibility trick. | Not every profile needs to fight: select based on whether the team needs survival, attack range or a specialist. |
| **Al Hawwa' FO (19), KHD (22), or Minelayer (21–22)** | Camouflage/Infiltration and WIP14 make this a primary button-pushing/forward hacking tool; mines and Cybermines complicate incoming moves. | Light and vulnerable when discovered; limited AVA and few substitutes make them worth protecting. |
| **Yuan Yuan (6–11)** | Cheap smoke, Impetuous movement and optional airborne entry let QK screen MSV2 gunfights or trade against vulnerable backfield pieces. | Irregular and unreliable at killing serious CC specialists; starting on table for smoke is often more useful than risky airborne deployment. |
| **Bashi Bazouk Contender/T2 Boarding Shotgun/specialist** | Parachutist/Holo deception threatens back arcs and objectives after enemy screens are weakened; expendable cheaper profiles make trading acceptable. | Irregular Orders and specialist timing complicate Group assignment. Opponents can screen table edges; preserve flexibility rather than forcing a bad entry. |
| **Korsan FTO (13–18) / Parachutist (21)** | FTO's cheap Drop Bears/BSG/close defense improve a link; non-FTO Parachutist threatens enemy-DZ soft targets and offers another approach angle. | **Only FTO profiles are Wildcards**. The 21-point airborne attacker must trade better than a low-cost Bashi. |
| **Druze hacker Duo or E/M Grenade Launcher** | Linked Pitchers + X-Visor can extend a repeater network; the E/M GL creates speculative equipment/area denial. | Two Druze hackers cost substantially more than just Laxmee and must be built around. **Druze Bayram Security Fireteams require at least one Druze;** do not assume other Wildcards replace that native anchor. |
| **Kaplan HRL/Engineer/Doctor in Bekçileri** | Attractive specialist-capable fireteam base, with HRL offering an inexpensive blast/template threat; Engineer/Doctor can be where the mission needs them. | Can struggle against Sekban's NCO utility or Janissary's superior gun stats; compare the *whole team cost*, not just the gun. |
| **Fiddler + 1–2 Jackbots (36/43)** | Engineer with Drop Bears and additional independent attack/space-control pressure; has a distinctive proactive role instead of a passive backfield repair job. | Costs significant points; **Fiddler FTO is not linkable in current QK chart despite the name**. |
| **Ghulam NCO Smoke GL (15), Fanous, Warcor** | Cheap Orders and area-control utilities sustain premium guns while NCO smoke can set Djanbazan attacks. | QK's best linkable combat modules are usually not Ghulam HMG cores. |

**Useful team templates (check every member against the canonical chart above):**

- **Qapu Haris:** Azra'il gun + Sekban Doctor + Hafza — high-threat active shooter, recovery, and NCO/support. Replace support according to mission; the membership and Counts-as values in the current reference remain decisive.
- **Qapu gun/utility:** Djanbazan HMG + Laxmee + Hafza — combine smoke shooter, White Noise/Pitcher and safe Lt/cheap filler, but **do not assume Laxmee counts as Odalisque** under current chart.
- **Bekçileri:** Janissary gun + Hafza + Kaplan/required anchor as applicable — efficient high-BS attack team; check **required-choice Janissary/Kaplan** entries, not just Wildcard membership.
- **Druze network Duo:** two Druze hackers/utility profiles — choose if deliberate Pitcher saturation is necessary, rather than for every list.
- **Zırhlı Duo:** Iguana / Scarface / Shakush / Triphammer with an eligible support member or second TAG. **Zırhlı is Duo-only**; its legal member set differs from the Qapu Khalqi shooter family.
- **Mission skeleton:** one primary gunfighting team + a secondary specialist/network team + Al Hawwa' + a few cheap orders/smoke/airborne threats; add a TAG if Orders and specialist reach remain healthy.

### TAGs, Vehicle and REMs — use the actual QK roster

| Profile (N5.3 reference) | Why choose it | Competing opinion / constraint |
|---|---|---|
| **Iguana TAG** — AVA1; **64-point AP HMG** or 68-point option | Main selling point after the N5 rework: BS14, Tactical Awareness, AP HMG, HFT (+1B), mine-dispensing/Repeater network and operator ejection mean it both attacks and creates defensive layers. Robert emphasizes its resilience/utility; Dante's 2025 event uses its active Repeater and mines with Laxmee and Baggage. | Low-ish TAG armor, hackability and vulnerability to close assault remain real; not an auto-include. Current operator/escape details must follow Army/rules, not a video's loose 'five wounds' shorthand. |
| **Shakush TAG** — AVA2; 58-point HMG or 56-point AP Spitfire | Cheapest dependable BS14 TAG shooter in QK, Tactical Awareness, and legal Zırhlı Duo. Good when sustained ranged fire matters more than network tricks. | Robert prefers the newly buffed Iguana for a small increase in cost; adding a second TAG eats specialists/orders. This is a *tradeoff*, not that Shakush is unusable. |
| **Triphammer TAG** — AVA2; 48–53 points | Most economical way into a high-ARM, 3-STR TAG with Tactical Awareness; zero-SWC loadouts free SWC for Azra'il/Djanbazan/Janissary. Two can form a Zırhlı Duo if deliberately building around TAG mass. | BS13, BTS3 and short/limited gun options versus a premium gun TAG; buy because a specific budget/SWC plan needs it, not just because it's cheap. |
| **Scarface & Cordelia** — bundled 76/80 points | Scarface brings AP HMG/AP Spitfire or other weapons, active fighting/CC and Tactical Awareness while Cordelia provides a Regular Order and Engineer support. Attractive **two-TAG** partner for Iguana if both have work to do. | Buying Scarface *requires* Cordelia; relative to a 64-point Iguana the full package can feel expensive. Their Army choice is bundled even if Zırhlı lists both as members. |
| **Zeybek Aero-unit (VH)** — AVA1, **33 pts / 1.5 SWC** AP Spitfire + Smoke GL | **QK's actual Vehicle:** 20-5 movement/ARM5 enables unusual aerial angles, mobility and smoke on a chassis separate from ground TAG roles. A niche complement when vertical attack and the table favor it. | Tactical Awareness N5 panel finds its smoke shots unreliable and matchups niche; don't plan as a dependable smoke battery or hard TAG answer. **Haytham and Shaykh Bakr from Vanilla Haqqislam are not QK roster entries** in this pinned source. |
| **Rafiq** — 13-point Sensor/FO, **19-point Red Fury FTO** | Ordinary Rafiq scouts/sensors camo, gets mission buttons and extends Repeaters; **FTO Red Fury is a genuine QK Wildcard** for a mobile gun/specialist-adjacent Duo/support role. | Crucial **sectorial difference**: FTO Wildcard is legal in **QK**, unlike Hassassin Bahram's non-linkable Rafiq FTO in the sibling reference. |
| **Shihab** — AVA2, 23-point TR HMG / 18-point TR Thunderbolt | Resilient-in-Orders static ARO guns. **Double Thunderbolt REMs** can cover separate lanes cheaply and be repaired by Najjarun/Burkut/Fiddler; good when your Fireteams must spend Orders attacking. | A dedicated counter can remove static AROs; give them overlapping coverage and repair access rather than exposing them both to one angle. |
| **Shaytaniyah** — 16-point Guided ML / 19-point +1B Guided ML | A guided threat rewards *actual* Targeted setup through Al Hawwa' FO/hacking, Laxmee, Druze, repeaters or other Forward Observers; alternate Burst makes it relevant for different defensive patterns. | **Both QK loadouts are marked Guided in this pinned file** (other sectorials may differ). If you cannot reliably Target, it is costly SWC without a plan. |
| **Kameel** — AVA2, 8-point support/Baggage, 14-point EVO, 16-point TR | Baggage reloads the pieces central to QK's **Pitcher + Iguana mines/deployables** plan. EVO buys supportware when needed; cheap bodies still help Order and repeater coverage. | EVO is not mandatory and paying for excess support can starve the assault. |
| **Fanous** — cheap Flash Pulse/Repeater, plus **Nasmat** servant | Efficient deployment-zone Repeater / emergency Flash ARO; Nasmat extends engineer/doctor work without risking the parent. | Nasmat is a Peripheral **without an Order**; no amount of support robots replaces a decent attack plan. |

**Cross-faction source interpretation:** **Vanilla Haqqislam** analysis helps value Shakush, Rafiq, Fanous and Baggage; **Nomad / Corregidor** material helps explain the shared Iguana's rework and vulnerabilities. **Do not** transplant Vanilla-only vehicles, TAG choices (Maghariba etc.), Fireteam combinations or REM AVA into QK. Zeybek is confirmed by this QK reference itself.

### Differences of opinion and date-sensitive contradictions

1. **"Strong flexible generalist" vs "mid-tier fragile legacy faction":** Robert Shepherd and Dante praise many good-value coordinated vectors and the reworked Iguana; the December 2025 **O-12 Podcast report** considers QK a capable, tricky, *mid-tier* faction whose links and low-stat guns can collapse when opponents break the right support. **Both useful:** QK has breadth, but a large collection of answers is not the same as guaranteed execution.
2. **Djanbazan smoke shooter vs Janissary reliability:** Djanbazan MSV2 + smoke can skew a fight at surprisingly low cost, and Dante likes AP Sniper/HMG combinations; Robert sometimes spends more for Janissary BS14 and better modifier play because BS12 can fail to convert favorable shots. **Pick by matchup**, not a blanket best gun.
3. **Azra'il AP HMG vs Feuerbach:** Robert sees the cheaper AP HMG as more flexible and consistent actively; the Feuerbach (+1B) offers special firepower and close-range secondary burst. Both reviewers praise Azra'il as the anti-armor anchor; profile is the debate.
4. **Iguana-first vs other TAGs / multi-TAG:** Robert finds post-rework Iguana the outstanding TAG and regards most other options as situational; Dante shows a **Scarface + Iguana** two-TAG list because QK can actually support it. The December written report likes pure TAG Duo flexibility. *Evaluate objective count, specialist access and available Regular Orders before committing to multiples.*
5. **Kaplan/Sekban/Druze:** Tournament experience values Kaplan's low-cost HRL/support and a medic/engineer when they solve actual missions; Sekban's NCO is often the efficient first utility addition; a deliberate Druze Pitcher Duo adds range/redundancy, but Robert would usually spend the points on Laxmee and other pieces. These are competing module choices, not a universal tier list.
6. **Yuan Yuan as parachutists or on-table smoke:** Dante's tournament stresses the rare useful AD vectors; Robert most often deploys them on-table because *reliable immediate smoke* benefits Djanbazan and other guns. Both plans work according to opponent screening.
7. **Important legality changes:** The 2025 Robert/Tactical/Dante transcripts sometimes describe **Laxmee as Odalisque** and **Burkut as Sekban**, or show team arrangements predating current composition. **Pinned N5.3 chart instead: Laxmee counts as Qapu Khalqi / Janissary; Burkut counts as Qapu Khalqi; Rafiq FTO and Korsan FTO are Wildcards; Fiddler FTO and Claire Lazhari FTO are *not* Fireteam members.** The **two Haris cap** also supersedes casual three-Haris narration.

### Best primary videos and podcasts (links, transcript status)

**Full YouTube/Spotify transcripts retrieved and reviewed through MCP:**

1. **[Robert Shepherd — Infinity N5 Faction Focus: Qapu Khalqi (2025-08-24)](https://www.youtube.com/watch?v=rOy0x0BLuNU)** — most useful *whole-army explanation*: efficient multi-team architecture, Hafza shell game, Laxmee/White Noise, Azra'il/Janissary/Djanbazan tradeoffs, post-rework Iguana, other TAGs, AD and weakness management.
2. **[Tactical Awareness S3 E30 — Qapu Khalqi (2025-08-08)](https://www.youtube.com/watch?v=n1vD-2YP0DM)** / **[podcast](https://open.spotify.com/episode/6rTsUzDqv5PcCQtNTI1ZA6)** — ~10–20 min Al Hawwa', MSV/smoke, Laxmee; ~20–40 min list roles, cheap orders and Bashi; ~40–60 min Druze, Burkut, Janissary, Azra'il, TAG options and **critical Zeybek skepticism**. Host disagreements retained; pre-N5.2.
3. **[Infinity the Dante — Qapu Khalqi: The Sky Is Falling! (2025-09-26)](https://www.youtube.com/watch?v=z4kV-SFZ5Uw)** — Fireteam modules, several attack vectors, Zırhlı, White Noise, air/AD threats and both mainstream and two-TAG sample lists. Pre-N5.2.
4. **[Infinity the Dante — Burn City Brawl Qapu Khalqi tournament report (2025-09)](https://www.youtube.com/watch?v=9BA7lqd1PMA)** — direct match examples: Iguana's Repeater/mines + Baggage + Laxmee, Shihab defensive bots, Djanbazan shooting, vulnerable/mobility-limited objective package.
5. **[Robert Shepherd — Vanilla Haqqislam N5 (2025-11-23)](https://www.youtube.com/watch?v=Dmv4pfdTbc0)** — selected transcript sections reviewed for **shared** Shakush and cheap REM/Repeater roles; other Vanilla-only TAGs/Vehicles are context only.
6. **[Robert Shepherd — Vanilla Nomads N5](https://www.youtube.com/watch?v=dOtvw5FKOfo)** — selected transcript sections reviewed for shared faction-level hacking/remote support and the context for Nomad TAG usage; not a QK legality source.

**Additional podcast/analysis with a narrower evidence role:**

- **[WIP12 E132 — Qapu Khalqi Revisited & Haqqislam Reinforcements (2023-10-23)](https://open.spotify.com/episode/1z93xIMsH1hM7GGrEUB4t3)** — MCP transcript retrieved for historical play patterns/Reinforcement perspective only; **N4**, not current legality.
- **[Tactical Awareness S1 E10 — Qapu Khalqi (2023-02-13)](https://open.spotify.com/episode/2OvUEoroS0PsqJiPsuMqjb)** — older N4 faction conversation, useful for context, not current N5 profiles.
- **[O-12 Podcast — Qapu Khalqi Report (2025-12-06, German text)](https://o12podcast.substack.com/p/qapu-khalqi-report-alte-tricks-neue)** — written critical counterpoint *after* N5.2, **not** represented as an MCP transcript.
- **[Bureau Aegis N5 Qapu tactical source index](https://www.bureau-aegis.org/forum/index.php?topic=17829.0)** and **[Corvus Belli Haqq tactics roundup](https://forum.corvusbelli.com/threads/n5-recap-haqqislam-tacticas.43463/)** — discovery/reference indexes; independently check dates and rules when using historical examples.

**Confidence:** Tactical patterns cross-confirmed by multiple perspectives; exact current points, roster and Fireteam legality **only** from the pinned repo. In particular, do not silently update formal Army provenance or drop the discontinued-status nuance just because videos discuss playable QK.

## Command-unit apex/value cross-reference (2026-10-23)

**Hafza LT(+1) 19/0** is the cheap Holomask command economy option: with a real **Sekban/Ghulam or other eligible NCO** it provides two Tactical activations without exposing the commander; **Hafza CoC 20/0** is a separate, protected succession choice. **Saladin/Farzan are not granted** by this Qapu roster. When assessing LT assassination, count loss of pooled link Orders, not merely the LT's point cost.

See [cross-faction Lieutenant, CoC and Order package tiers](../../notes/list-building/command-units-apex-and-value.md). **Current roster and canonical Fireteam chart above remain authoritative.**

## Mission specialist / button-pusher choices (N5.3)

**Hafza FO17/0 vs CoC20/0 vs LT(+1)19/0** are *different* Holomask utility/command choices; the FO is a useful cheap linked/near-side button, CoC can be mission Specialist when allowed. **Odalisque Paramedic** provides mobile non-Hacker scoring in eligible links; **Kaplan/Sekban Doctor/Engineer** support tech recovery as actually printed. **Rafiq FTO19/0.5 legal Wildcard** is not the same cheaper Rafiq profile; Sensor/Repeater/FO scoring only on selected bot profile. Plan distinct early and late console routes.

[Cross-game apex and value specialist tier guide](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). The unit profiles/Fireteams above control exact legality.

## Airborne / enemy-DZ attack profile choices (2026-10-23)

**Bashi Bazouk SMG12/0 or T2 BSG14/0** is a cheap **Irregular** Holomask/Holoprojector/normal Parachutist whose best payback may be forcing 2–3 enemy Orders to respond; **it cannot enter directly in enemy DZ from normal Parachutist**. **Korsan Parachutist21/0** can flank if that exact profile is bought; the 16pt FTO Korsan does not inherit it. The current Qapu roster's **Hafza CoC20** is an inexpensive succession/profile choice, **not** an off-table assassin. Prefer cost-effective support disruption to sacrificing 20+ points for one unimportant Regular.

[Cross-game N5.3 airborne and DZ-attack apex/value tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **Pinned profiles and the canonical Fireteam chart above govern legality.**

## Warbands and cheap high-upside trading — N5.3

Qapu's **Bashi Bazouk SMG12/0 or T2 BSG14/0** offers an extremely cheap **Irregular Parachutist+Holoprojector** late flank, but **not** a 5pt Ghazi/Daylami front-line unit; normal Parachutist cannot enter directly inside enemy DZ. Evaluate trade into vulnerable Regular Orders/Doctor/Engineer, or use it as an **ARO/Discover tax**. **Korsan** close/Chain/FD/Parachutist loadouts are different and only actual current options get link access. **Hafza CoC20** is succession and potential objective utility, not a cheap sacrificial template. Avoid importing Bahram AVA/Smoke options.

[Current cross-game warband apex/value, target counters and LT/CoC tiers](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). Pinned profile choices and canonical Fireteam chart in this roster remain authoritative.

## TAG tactical cross-reference (2026-10-23)

**Shakush** is the cheap armored gun, **Triphammer** saves points and adds flexible AP/HRL options, and **Iguana** is the specialized AP HMG/Repeater/operator plan. Compare with Qapu's efficient HI (notably Azra'il) before assuming a TAG is mandatory; the Zırhlı **required-choice** and companions must come from the canonical chart. Podcast criticism of Iguana's 'two wounds' is dated; check the present profile states.

For the two-tier **apex/points-value** comparison, TAG counterplay, matchup matrix and direct transcript sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Treat current profiles, points/SWC and canonical Fireteam data above as authoritative.

## Vehicle (VH) tactical cross-reference (2026-10-23)

**Zeybek AVA1 only** (no current Qapu Haytham): **33/1.5 AP Spitfire + Smoke GL** has **Albedo**, punishing MSV/Marksmanship units that constrain Qapu smoke/White Noise; the operator can retain a Regular Order and potentially score *after the correct damage transition*. It is the high-ceiling **anti-visor flanker**, not a conventional armored TAG, and has **no natural Mimetism** against unvisored return fire. S7/No Cover/Hackable and limited repair require clear escape and ground support.

See [VH apex/value tier list and matchup guide](../../notes/list-building/vehicles-vh.md). **Current profiles, AVA and canonical Fireteam chart above remain authoritative.**

## Hacker and KHD tactical cross-reference (2026-10-23)

**Laxmee HD+ 24/0.5** brings **White Noise + Pitcher + Cybermine**, particularly valuable for defeating MSV snipers that challenge Janissary/Djanbazan shooting; it is not a KHD unless printed. **Leila Sharif KHD+Carbonite+Firewall(-3), 22/0** adds anti-Hacker lethal Trinity and limited anti-HI control; **Druze HD/Pitcher 25/0.5 vs KHD/Pitcher 23/0** improves projection via current legal team and X-Visor; **Al Hawwa' Camouflage KHD 22/0** scores safely forward. **Ghulam HD16/0.5** is a cheap redundancy slot. **Why:** pair **Laxmee's White Noise/Oblivion** with **Leila's Trinity**, rather than buying two identical hack devices. Exact linked profiles and Fireteam source must be checked in this Qapu chart.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

Cross-faction [apex and cost-value Order-generator rankings](../../notes/list-building/cheerleaders-and-order-generators.md), circumstance guide and transcript disagreements. **This file remains authoritative for profiles, AVA, Training and Fireteam legality.**

- 7pt Fanous — Regular Flash/Repeater REM with Mimetism; excellent cheap network but limited S3 concealment.
- 8pt Kameel — Baggage/Repeater/Deactivator and Regular Order, particularly valuable with disposable launchers.
- 11pt Ghulam — S2 protected Regular Order; FO/Doctor/deployable repeater profiles can earn their premium.
- Korsan — low-cost Regular defensive/trading role when roster-legal; compare to passive Fanous before allocating slots.
- Warcor — Irregular Flash Pulse ARO distraction, NOT a passive transferable Regular Order.

**When to pick:** Prefer transferable, safe Regular Orders when the Combat Group needs fuel; choose the higher-priced option only when its smoke, template, weapon, repeater, Fireteam function or scoring ability has a real job. Do not count Irregular/Impetuous/Tactical/Lieutenant Orders or Peripheral bodies as interchangeable Regular pool Orders; account for DZ footprint and link/enabler package costs.


## ARO apex/value cross-reference (2026-10-23)

[Best ARO units across N5.3 — absolute apex vs points-value](../../notes/list-building/aro-units-apex-and-value.md) compares hidden reactive fire, TR/Neurocinetics, Flash/DTW/expendable defenders and why competing creators disagree. The **roster here** is authoritative for actual costs, Training, AVA and Fireteam construction.

- **Fanous Flashbot** — cheap regular network and ARO tax, not a full-strength gun
- **Ghulam cheap template/FO** — small-base Regular guard plus a mission secondary job; don't expose a linked gun solely to win AROs
- **Warcor 3pt Flash** — disposable Irregular Stun/Orders tax, not a generic Regular cheerleader

**Best circumstance:** long exposed lanes justify a real sniper/missile/linked gun; dense tables, DZ landings and mission rooms favor E/M, mine, Shotgun, Riotstopper and hidden traps. Cover the destination/approach, layer serial threats rather than two pie-sliceable visible guns, and preserve scoring units for the active turn.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Ghulam Doctor(+3)** is an excellent budget VITA support option if in the selected roster: its **WIP14+3 = 17 (85%)** can outperform generic WIP13 Doctor without extra Orders. **Claire Lazhari33** is a higher-cost **Doctor(2W) versus FTO Doctor(+3)** choice; use it for heavy VITA Fireteam recovery *when team eligibility is legal*. **Najjarun/Nasmat** (or roster-available Engineer) provides distinct STR and hack-state repair, particularly for REM-heavy plans. [Doctor/Engineer recovery odds and tier guide](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).
