---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 401
sectorial_slug: haqqislam
sectorial_name: Vanilla Haqqislam
parent_faction: Haqqislam
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Vanilla Haqqislam standard roster, AVA, standard loadouts and points/SWC, canonical vanilla Fireteam chart and reverse access index, optional Spec-Ops/Team-Ops hooks, source relations, and the distinct Melek Reaction Group Reinforcement Fireteam chart."
---

# Vanilla Haqqislam

## Overview and provenance

Repository-native reference for **Vanilla Haqqislam** roster, profiles, points/SWC, AVA, and the Fireteams explicitly exposed by the current Army source.

Sources used:

- Army-derived Haqqislam source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `d4329bb596ffea5d568eb2435f74366c305a7630`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Schema note:

- The repository currently has no separate vanilla-faction reference schema. This file therefore keeps `reference_type: sectorial` and the established `sectorial_*` front-matter keys for compatibility, while `sectorial_name` explicitly identifies this as the **vanilla faction roster**.

Coverage notes:

- Covers the **56-unit standard Vanilla Haqqislam roster** in the pinned Army source.
- Army ID **401** is active (`discontinued: false`) and uses canonical slug `haqqislam`.
- `Haqqislam Team-Ops` and `Husam Spec-Ops` occur before the generic mercenary catalogue in the source but are optional game-mode content, so they are listed separately rather than counted in the 56 standard entries.
- Generic Soldier of Fortune / `merc-*` catalogue entries with empty faction lists are excluded from the standard roster.
- The current vanilla source **does contain a Fireteam chart**: Core 0, Haris 1, Duo 2. It defines two mixed membership pools, reproduced below.
- Every standard vanilla Fireteam-chart row has `required: false` and `min: 0`. This reference therefore does not invent a mandatory anchor troop for either pool.
- Fireteam legality comes from the canonical chart, not from an `FTO` profile name by itself. `KORSAN FTO` is explicitly present in Haqqislam Fireteams II; `Fiddler FTO`, `CLAIRE LAZHARI FTO`, and `RAFIQ REMOTE FTO` are not present in the vanilla chart and gain no vanilla Fireteam access from the label alone.
- `Scarface & Cordelia` is a genuine standard Vanilla Haqqislam entry in this source; its ordinary unit entry includes faction 401 and its enabled list choices remain bundled Scarface + Cordelia teams.
- `Triphammer` and `Fiddler` likewise explicitly include faction 401 in their ordinary source entries.
- `Sacha Xenotech Hunters` and `Zaybak Aero-unit` files exist in the broader Haqqislam source directory but do **not** occur in this pinned vanilla roster. `Zeybek Aero-unit` and `Haytham Aero-unit` do.
- Linked Reinforcement army ID: **499**, **Melek Reaction Group**. Its Fireteam chart is recorded separately and is not merged into the standard vanilla chart.

## Faction summary

| Field | Value |
|---|---|
| Faction | Vanilla Haqqislam |
| Army ID | 401 |
| Army slug | `haqqislam` |
| Army metadata status | Active |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 56 |
| Optional-mode units | Haqqislam Team-Ops; Husam Spec-Ops |
| Reinforcement roster | Melek Reaction Group, Army ID `499` |
| Fireteam limits | Core 0; Haris 1; Duo 2 |
| Fireteam pools | Haqqislam Fireteams I; Haqqislam Fireteams II |

## Standard roster index

| Unit | ID | AVA | Type | Order | Vanilla Fireteam access |
|---|---:|---:|---|---|---|
| Hassassin Ragiks | 307 | 2 | MI | Regular | — |
| Burkut | 1759 | 2 | HI | Regular | Fireteams II, max 2 |
| Maghariba Guard | 309 | 2 | TAG | Regular | Fireteams I, max 1 |
| Hassassin Farzans | 332 | 1 | SK | Regular | — |
| Khawarijs | 303 | 3 | MI | Regular | Fireteams II, max 1 |
| Warcors | 50 | 1 | LI | Irregular | — |
| Sunduqbut | 1590 | 1 | HI | Regular | — |
| Yara Haddad | 1548 | 1 | MI | Regular | Fireteams I, max 1 |
| Hunzakuts | 310 | 2 | SK | Irregular | — |
| Zamira Nazarova | 321 | 1 | WB | Irregular + Impetuous | — |
| Hafza Unit | 326 | 2 | LI | Regular | Fireteams I, max 1 |
| Zeybek Aero-unit | 1852 | 1 | VH | Regular | — |
| Janissaries | 308 | 2 | HI | Regular | Fireteams II, max 1 |
| Fiddler | 1564 | 1 | LI | Regular | —; FTO profile name alone does not grant access |
| Najjarun Engineers | 314 | 2 | LI | Regular | Fireteams I, max 1 |
| Hassassin Muyibs | 327 | 2 | MI | Regular | Fireteams II, max 2 |
| Hassassin Barids | 337 | 1 | LI | Regular | — |
| Muttawi'ah | 340 | 4 | LI | Irregular + Impetuous | — |
| Fanous Remotes | 318 | 1 | REM | Regular | — |
| Al Hawwa' Unit | 331 | 2 | SK | Regular | — |
| Sekban, Naval Special Unit | 339 | 2 | MI | Regular | Fireteams II, max 2 |
| Zuleyka Nazarova | 322 | 1 | WB | Irregular + Impetuous | — |
| Rafiq Remotes | 315 | 2 | REM | Regular | —; FTO profile name alone does not grant access |
| Husam Operative Leila Sharif | 849 | 1 | LI | Regular | Fireteams II, max 1 |
| Hassassin Fiday | 312 | 1 | SK | Regular | — |
| Asawira Regiment | 329 | 1 | HI | Regular | — |
| Hassassin Bokhtar | 1589 | 1 | HI | Regular | — |
| Zhayedan Intervention Troops | 305 | 3 | MI | Regular | Fireteams I, max 2 |
| Dr. Claire Lazhari | 1894 | 1 | LI | Regular | —; FTO profile name alone does not grant access |
| Naffatûn | 302 | 4 | LI | Regular | Fireteams I, max 2 |
| Shihab Remotes | 316 | 1 | REM | Regular | — |
| Nasmat Remotes | 333 | 4 | REM | Peripheral | — |
| Djanbazan Tactical Group | 306 | 3 | MI | Regular | Fireteams I, max 2 |
| Murabids Tuareg | 311 | 2 | SK | Regular | — |
| Korsan, Corsairs of the Gate | 1758 | 2 | LI | Regular | Fireteams II, **FTO profiles only**, max 2 |
| Daylami Infantry | 323 | 3 | LI | Irregular | — |
| Triphammer, Repurposed Industrial TAG | 1569 | 1 | TAG | Regular + Tactical Awareness | — |
| Haytham Aero-unit | 1851 | 1 | VH | Regular | — |
| Azra'il | 330 | 1 | HI | Regular | Fireteams I, max 1 |
| Ghulam Infantry | 301 | TOTAL | LI | Regular | — |
| Mukhtar, Active Response Unit | 1313 | 2 | MI | Regular | Fireteams I, max 2 |
| Medical Specialist Rahman Rouhani | 1549 | 1 | LI | Regular | Fireteams I, max 1 |
| Hassassin Nadhir | 1545 | 1 | LI | Regular | — |
| Shaytaniyah Remotes | 317 | 1 | REM | Regular | — |
| Kameel Remotes | 334 | 2 | REM | Regular | — |
| Sayiq TAG Support Pilots | 1849 | 1 | LI | Regular | — |
| Yuan Yuan | 378 | 2 | WB | Irregular + Impetuous | — |
| Shakush Light Armored Unit | 1546 | 2 | TAG | Regular + Tactical Awareness | Fireteams I, max 1 |
| Kum Motorized Troops | 313 | 2 | WB | Irregular + Impetuous | — |
| Knauf, Outlaw Sniper | 939 | 1 | LI | Regular | — |
| Saladin, O-12 Liaison Officer | 336 | 1 | MI | Regular | — |
| Scarface & Cordelia | 380 | 1 team | TAG + LI | 2 Regular + Tactical Awareness | — |
| Hassassin Lasiqs | 328 | 1 | LI | Regular | — |
| Bashi Bazouks | 325 | 2 | LI | Irregular | — |
| Odalisques | 324 | 4 | LI | Regular | Fireteams II, max 2 |
| RacerBots | 1905 | 2 | REM | Regular | — |

## Optional-mode entries

| Unit | ID | Mode | Vanilla Fireteam relevance |
|---|---:|---|---|
| Haqqislam Team-Ops | 1930 | Team-Ops | No row in the pinned vanilla Fireteam chart |
| Husam Spec-Ops | 1916 | Spec-Ops | No row in the pinned vanilla Fireteam chart |

## Unit details

### Hassassin Ragiks

**ID 307 · AVA 2 · MI** — `MOV 10-10 | CC 15 | BS 12 | PH 12 | WIP 15 | ARM 2 | BTS 0 | W 1 | S 2`. Combat Jump / Parachutist assault troop.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 23 | 0 | Boarding Shotgun (+1B), Boarding Pistol, CC Weapon | — |
| 29 | 1.5 | Spitfire, Boarding Pistol, CC Weapon | — |
| 25 | 0.5 | Boarding Shotgun, D-Charges, Boarding Pistol, CC Weapon; Hacking Device | — |

### Burkut

**ID 1759 · AVA 2 · HI** — `MOV 10-10 | CC 16 | BS 12 | PH 12 | WIP 14 | ARM 3 | BTS 6 | W 1 | S 2`. Engineer, Mimetism (-3), NWI, Religious Troop; GizmoKit and Deactivator.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 28 | 0 | Boarding Shotgun (+1B), Panzerfaust, AP Mine, D-Charges | Fireteams II |
| 30 | 0.5 | Submachine Gun, Light Rocket Launcher, D-Charges | same |
| 26 | 0 | Submachine Gun, E/Marat (+1B), AP Mine, D-Charges | same |
| 28 | 0 | Submachine Gun, Heavy Flamethrower (+1B), AP Mine, D-Charges | same |

### Maghariba Guard

**ID 309 · AVA 2 · TAG** — `MOV 15-10 | CC 16 | BS 14 | PH 17 | WIP 14 | ARM 8 | BTS 6 | W 3 | S 8`.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 72 | 1.5 | MULTI HMG, E/M Carbine (+2B), AP Heavy Pistol, AP CC Weapon; Jandab | Fireteams I, max 1 |
| 71 | 1.5 | MULTI HMG, Heavy Rocket Launcher, Grenade Launcher, Heavy Pistol (+1B) | same |
| 71 | 1.5 | MULTI HMG, Heavy Flamethrower (+1B), Mine Dispenser (Shock), AP Heavy Pistol | same |

### Hassassin Farzans

**ID 332 · AVA 1 · SK** — `MOV 10-10 | CC 16 | BS 12 | PH 11 | WIP 14 | ARM 0 | BTS 0 | W 1 | S 2`. Camouflage / infiltration specialist.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 24 | 0 | Boarding Shotgun, Shock Mine, Silenced Pistol; Chain of Command | — |
| 21 | 0.5 | Boarding Shotgun, Viral Mine, Silenced Pistol; Minelayer | — |
| 22 | 0 | Rifle, Light Shotgun, Flash Pulse, Shock Mine, D-Charges; Forward Observer | — |

### Khawarijs

**ID 303 · AVA 3 · MI** — `MOV 15-5 | CC 23 | BS 13 | PH 13 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. Mobile close-assault infantry; Viral CC Weapon.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 29 | 1 | Heavy Rocket Launcher, Light Shotgun | Fireteams II, max 1 |
| 35 | 1.5 | AP Spitfire, Pulzar (+1B) | same |
| 33 | 0 | Rifle, Light Shotgun, Pulzar (+1B), MULTI Pistol | same |
| 30 | 0 | Boarding Shotgun, Pulzar (+1B); Doctor (+1), MediKit | same |
| 38 | 0 | Mk12, Pulzar (+1B); MSV2, NCO | same |

### Warcors

**ID 50 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular Journalist.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 3 | 0 | Flash Pulse, Stun Pistol, PARA CC Weapon; 360º Visor variant | — |
| 3 | 0 | Flash Pulse, Stun Pistol, PARA CC Weapon; Sixth Sense variant | — |

### Sunduqbut

**ID 1590 · AVA 1 · HI** — `MOV 10-10 | CC 13 | BS 13 | PH 14 | WIP 12 | ARM 4 | BTS 3 | W 2 | S 2`. Camouflage / Neurocinetics profile family.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 49 | 1.5 | AP Spitfire, Light Shotgun; Camouflage / Surprise Attack package | — |
| 43 | 0.5 | Viral Rifle (+1B), Chain Rifle (+1B), Viral Mine; Minelayer | — |
| 47 | 1.5 | Feuerbach; Neurocinetics | — |
| 42 | 0 | Viral Rifle, Chain Rifle; Neurocinetics (+1B) | — |
| 50 | 1.5 | AP Spitfire, Light Shotgun; Neurocinetics | — |

### Yara Haddad

**ID 1548 · AVA 1 · MI** — `MOV 10-10 | CC 16 | BS 13 | PH 11 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. MSV2.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 24 | 0 | AP Marksman Rifle, Heavy Pistol (+1B), CC Weapon | Fireteams I, max 1 |
| 24 | 0 | Same weapons; Lieutenant | same |

### Hunzakuts

**ID 310 · AVA 2 · SK** — Irregular Camouflage / infiltration utility specialists.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 18 | 0.5 | Rifle, Grenade Launcher, Shock Mine, Boarding Pistol; Deployable Repeater | — |
| 18 | 0.5 | Sniper Rifle, Shock Mine | — |
| 19 | 0 | Rifle, Light Shotgun, Shock Mine; Forward Observer | — |
| 15 | 0 | Boarding Shotgun, D-Charges; Forward Observer | — |

### Zamira Nazarova

**ID 321 · AVA 1 · WB** — `MOV 20-15 | CC 22 | BS 12 | PH 13 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 4`. Irregular, Impetuous, Motorcycle.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 11 | 0 | Light Shotgun, Smoke Grenades, Smoke Grenade Launcher, AP Heavy Pistol (+1B), E/M CC Weapon | — |

### Hafza Unit

**ID 326 · AVA 2 · LI** — `MOV 10-10 | CC 14 | BS 12 | PH 10 | WIP 14 | ARM 2 | BTS 0 | W 1 | S 2`. Holomask.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 15 | 0 | Rifle, Light Shotgun | Fireteams I, max 1 |
| 16 | 1.5 | Heavy Rocket Launcher, Assault Pistol | same |
| 22 | 1 | Spitfire | same |
| 20 | 0 | Rifle, Light Shotgun; Chain of Command | same |
| 17 | 0 | Rifle, Light Shotgun, Flash Pulse; Deployable Repeater, Forward Observer | same |
| 15 | 0 | Rifle, Light Shotgun; Lieutenant | same |
| 19 | 0 | Rifle, Light Shotgun; Lieutenant (+1 Order) | same |

### Zeybek Aero-unit

**ID 1852 · AVA 1 · VH** — `MOV 20-5 | BS 13 | PH 12 | WIP 14 | ARM 5 | BTS 6 | W 3 | S 7`. Aerial vehicle profile with included operator.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 33 | 1.5 | AP Spitfire, Smoke Grenade Launcher; includes Zeybek Operator | — |

### Janissaries

**ID 308 · AVA 2 · HI** — `MOV 10-10 | CC 18 | BS 14 | PH 14 | WIP 14 | ARM 4 | BTS 6 | W 2 | S 2`.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 31 | 0 | AP Rifle, Light Shotgun, Pulzar, Heavy Pistol, CC Weapon | Fireteams II, max 1 |
| 38 | 1.5 | HMG, Pulzar, Heavy Pistol | same |
| 28 | 0 | Boarding Shotgun, Pulzar, Heavy Pistol; TinBot Firewall | same |
| 32 | 0 | AP Rifle package; TinBot Firewall | same |
| 36 | 1.5 | Missile Launcher | same |
| 35 | 0 | Doctor profile; MediKit | same |
| 31 | 0 | AP Rifle package; Lieutenant | same |
| 32 | 0 | Lieutenant; TinBot Firewall | same |

### Fiddler

**ID 1564 · AVA 1 · LI** — `MOV 15-10 | CC 18 | BS 12 | PH 12 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Engineer with Jackbot variants.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 29 | 0 | **Fiddler FTO**; Contender (+1B), Drop Bears, D-Charges, Breaker Pistol, PARA CC Weapon; Super-Jump | **No vanilla FT row** |
| 36 | 0 | Fiddler plus 1 synchronized Jackbot; Climbing Plus | — |
| 43 | 0 | Fiddler plus 2 synchronized Jackbots; Climbing Plus | — |

### Najjarun Engineers

**ID 314 · AVA 2 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Engineer.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 15 | 0 | Rifle, Light Shotgun, D-Charges | Fireteams I, max 1 |
| 16 | 0 | Rifle, Light Shotgun, D-Charges; Deployable Cover | same |
| 17 | 0 | Rifle, Light Shotgun, D-Charges; Armed Turret (Rifle) | same |

### Hassassin Muyibs

**ID 327 · AVA 2 · MI** — `MOV 10-10 | CC 18 | BS 13 | PH 11 | WIP 14 | ARM 3 | BTS 3 | W 1 | S 2`.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 21 | 1 | Rifle, Grenade Launcher, Smoke Grenade Launcher, Kobra Pistol | Fireteams II, max 2 |
| 25 | 0 | Rifle, Light Shotgun, Panzerfaust, Viral Mine; Minelayer | same |
| 32 | 1.5 | Spitfire, D-Charges; X Visor, Tactical Awareness | same |
| 22 | 1.5 | Heavy Rocket Launcher, D-Charges; X Visor, Tactical Awareness | same |
| 26 | 0 | Rifle, Light Shotgun, Panzerfaust; Doctor (+1) | same |
| 23 | 0 | Rifle, Light Shotgun, Panzerfaust, Flash Pulse; Forward Observer | same |
| 21 | 1 | Rifle, Grenade Launcher, Smoke Grenade Launcher; Lieutenant | same |

### Hassassin Barids

**ID 337 · AVA 1 · LI** — `MOV 10-10 | CC 14 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Network/hacking specialist.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 16 | 0.5 | Rifle, Pitcher, Breaker Pistol; Hacking Device | — |
| 14 | 0 | Rifle, Pitcher, Breaker Pistol; Killer Hacking Device / Trinity upgrade | — |
| 12 | 0 | Rifle, Pitcher, Flash Pulse; Forward Observer | — |
| 16 | 1 | Rifle, Pitcher, Breaker Pistol; Lieutenant, Hacking Device | — |
| 12 | 0 | Rifle, Pitcher, Flash Pulse; Lieutenant, Forward Observer | — |

### Muttawi'ah

**ID 340 · AVA 4 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 12 | WIP 15 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular and Impetuous.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 5 | 0 | Chain Rifle, Smoke Grenades, Breaker Pistol | — |
| 5 | 0 | Chain Rifle, E/Marat, Smoke Grenades | — |
| 6 | 0 | Chain Rifle, Jammer, Smoke Grenades | — |
| 7 | 0 | Boarding Shotgun, E/Marat, Smoke Grenades | — |
| 8 | 0 | Boarding Shotgun, Jammer, Smoke Grenades | — |

### Fanous Remotes

**ID 318 · AVA 1 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater utility REM.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 7 | 0 | Flash Pulse, PARA CC Weapon; Repeater, Mimetism (-3) | — |

### Al Hawwa' Unit

**ID 331 · AVA 2 · SK** — `MOV 10-10 | CC 14 | BS 11 | PH 11 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Camouflage / infiltration specialist.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 24 | 0.5 | Boarding Shotgun, D-Charges, Cybermine, Silenced Pistol; Hacking Device | — |
| 22 | 0.5 | Shock Marksman Rifle, Shock Mine, Silenced Pistol; Minelayer | — |
| 19 | 0 | Boarding Shotgun, Flash Pulse, D-Charges, Silenced Pistol; Forward Observer | — |
| 22 | 0 | Boarding Shotgun, D-Charges, Cybermine, Silenced Pistol; Killer Hacking Device | — |
| 21 | 0.5 | Submachine Gun, Grenade Launcher, Shock Mine, Silenced Pistol; Minelayer | — |

### Sekban, Naval Special Unit

**ID 339 · AVA 2 · MI** — `MOV 10-10 | CC 17 | BS 13 | PH 11 | WIP 14 | ARM 3 | BTS 3 | W 1 | S 2`. 360º Visor, NCO.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 19 | 0 | Boarding Shotgun, Chain-colt, Pistol, CC Weapon | Fireteams II, max 2 |
| 27 | 1 | Red Fury, Chain-colt, Pistol, CC Weapon | same |
| 19 | 1.5 | Heavy Rocket Launcher, Chain-colt, Pistol, CC Weapon | same |
| 24 | 0 | AP Rifle, Light Shotgun, Chain-colt; Specialist Operative | same |
| 23 | 0 | Boarding Shotgun, Chain-colt; Doctor (+1), MediKit | same |
| 24 | 0 | AP Rifle, Light Shotgun, Chain-colt; Lieutenant, Specialist Operative | same |
| 28 | 1.5 | Spitfire, Chain-colt | same |

### Zuleyka Nazarova

**ID 322 · AVA 1 · WB** — `MOV 20-15 | CC 22 | BS 11 | PH 13 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 4`. Irregular, Impetuous, Motorcycle.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 12 | 0 | Light Flamethrower (+1B), Smoke Grenades, Smoke Grenade Launcher, Breaker Pistol (+2B), EXP CC Weapon | — |

### Rafiq Remotes

**ID 315 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Sensor, Forward Observer.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 13 | 0 | Rifle, Light Shotgun, Flash Pulse, PARA CC Weapon; Triangulated Fire | — |
| 19 | 0.5 | **RAFIQ REMOTE FTO**; Red Fury, Flash Pulse, PARA CC Weapon | **No vanilla FT row** |

### Husam Operative Leila Sharif

**ID 849 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Killer Hacker.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 22 | 0 | Shock Marksman Rifle, E/M Mine, D-Charges, Breaker Pistol, CC Weapon; Killer Hacking Device | Fireteams II, max 1 |

### Hassassin Fiday

**ID 312 · AVA 1 · SK** — Impersonation assault specialist.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 25 | 0 | Rifle, Light Shotgun, Smoke Grenades, Pistol, DA CC Weapon | — |
| 26 | 0 | Rifle, Light Shotgun, Smoke Grenades, Shock Mine, Pistol, DA CC Weapon | — |
| 23 | 0 | Boarding Shotgun, Smoke Grenades, Pistol, DA CC Weapon | — |

### Asawira Regiment

**ID 329 · AVA 1 · HI** — `MOV 15-5 | CC 23 | BS 14 | PH 14 | WIP 14 | ARM 4 | BTS 9 | W 2 | S 2`.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 33 | 0 | AP Rifle, Light Shotgun, Nanopulser, Pistol, DA CC Weapon | — |
| 35 | 0 | Viral Rifle, Light Shotgun, Nanopulser | — |
| 32 | 0 | Boarding Shotgun (+1B), Nanopulser, MULTI Pistol | — |
| 38 | 1.5 | AP Spitfire, Nanopulser | — |
| 37 | 0 | AP Rifle package; Doctor (+1), MediKit | — |
| 35 | 0 | Boarding Shotgun package; Doctor (+1), MediKit | — |
| 33 | 0 | AP Rifle package; Lieutenant | — |
| 38 | 1.5 | AP Spitfire package; Lieutenant | — |

### Hassassin Bokhtar

**ID 1589 · AVA 1 · HI** — `MOV 15-5 | CC 20 | BS 13 | PH 13 | WIP 14 | ARM 4 | BTS 3 | W 2 | S 2`.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 46 | 1.5 | Red Fury, Viral Pistol, Shock CC Weapon; Tactical Awareness | — |
| 45 | 0 | Viral Rifle, Light Shotgun, D-Charges, Viral Pistol; Paramedic, Tactical Awareness | — |
| 52 | 1.5 | Red Fury; Parachutist, Tactical Awareness | — |
| 49 | 0 | Boarding Shotgun assault profile; Parachutist | — |
| 46 | 1.5 | Red Fury package; Lieutenant | — |
| 45 | 0 | Viral Rifle specialist package; Lieutenant | — |

### Zhayedan Intervention Troops

**ID 305 · AVA 3 · MI** — `MOV 10-10 | CC 16 | BS 12 | PH 11 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 22 | 0 | Breaker Rifle, Light Shotgun | Fireteams I, max 2 |
| 31 | 1.5 | HMG | same |
| 27 | 0.5 | AP Sniper Rifle | same |
| 26 | 1.5 | Missile Launcher | same |
| 27 | 0 | Boarding Shotgun; Doctor | same |
| 22 | 0 | Breaker Rifle package; Lieutenant | same |
| 31 | 1.5 | HMG; Lieutenant | same |

### Dr. Claire Lazhari

**ID 1894 · AVA 1 · LI** — `MOV 15-5 | CC 16 | BS 13 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Doctor utility character.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 33 | 0 | Breaker Combi Rifle, Nanopulser (+1B), Viral Pistol (+1B), PARA CC Weapon; Doctor | — |
| 33 | 0 | **CLAIRE LAZHARI FTO**; FTO-labelled Doctor profile | **No vanilla FT row** |

### Naffatûn

**ID 302 · AVA 4 · LI** — `MOV 10-10 | BS 11 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Direct-template line infantry.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 11 | 0 | Rifle, Light Flamethrower, Grenades | Fireteams I, max 2 |
| 11 | 0 | Rifle, Heavy Flamethrower | same |
| 11 | 0 | Rifle, Light Flamethrower, Grenades; Lieutenant | same |

### Shihab Remotes

**ID 316 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. 360º Visor, Total Reaction.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 23 | 1 | HMG, PARA CC Weapon | — |
| 18 | 0 | Thunderbolt (+1B), PARA CC Weapon | — |

### Nasmat Remotes

**ID 333 · AVA 4 · REM** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Servant Peripheral.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 3 | 0 | PARA CC Weapon; Servant | — |

### Djanbazan Tactical Group

**ID 306 · AVA 3 · MI** — `MOV 10-10 | CC 14 | BS 12 | PH 11 | WIP 14 | ARM 3 | BTS 0 | W 1 | S 2`. MSV2, Regeneration, Immunity (Shock).

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 22 | 0 | Rifle, Light Shotgun | Fireteams I, max 2 |
| 31 | 1.5 | HMG | same |
| 27 | 0.5 | AP Sniper Rifle; BS Attack (Shock) | same |
| 27 | 0.5 | Rifle, Light Shotgun; Hacking Device | same |
| 26 | 0 | Rifle, Light Shotgun; Doctor (+1), MediKit | same |
| 22 | 1 | Rifle, Light Shotgun; Lieutenant | same |
| 26 | 0 | Shock Marksman Rifle | same |
| 28 | 1 | Red Fury | same |

### Murabids Tuareg

**ID 311 · AVA 2 · SK** — Hidden Deployment / Camouflage infiltration specialist with WIP 15.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 26 | 0 | Boarding Shotgun, Shock Mine | — |
| 27 | 0.5 | Sniper Rifle, Shock Mine | — |
| 33 | 0.5 | Rifle, Light Shotgun, D-Charges, Shock Mine; Hacking Device | — |
| 28 | 0 | Submachine Gun, D-Charges, Shock Mine; Killer Hacking Device | — |
| 32 | 0 | Rifle, Light Shotgun, Shock Mine; Doctor | — |
| 29 | 0.5 | Rifle, Light Shotgun, Viral Mine; Minelayer | — |

### Korsan, Corsairs of the Gate

**ID 1758 · AVA 2 · LI** — `MOV 15-5 | CC 21 | BS 11 | PH 13 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Natural Born Warrior, Climbing Plus.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 14 | 0 | **KORSAN FTO**; Chain Rifle (+2B), Heavy Pistol, Shock CC Weapon | Fireteams II |
| 18 | 0 | **KORSAN FTO**; Submachine Gun, Grenades (+1B), Heavy Pistol | same |
| 13 | 0 | **KORSAN FTO**; Chain Rifle, Drop Bears, Heavy Pistol | same |
| 16 | 0 | **KORSAN FTO**; Boarding Shotgun, Heavy Pistol | same |
| 16 | 0 | **KORSAN FTO**; Chain Rifle, Contender, Heavy Pistol | same |
| 21 | 0 | Submachine Gun / Grenades forward-deployment profile | **No FT** |
| 21 | 0 | Boarding Shotgun Parachutist profile | **No FT** |

### Daylami Infantry

**ID 323 · AVA 3 · LI** — Irregular light infantry with disposable-weapon and Camouflage variants.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 5 | 0 | Light Shotgun | — |
| 10 | 0.5 | Rifle, Grenade Launcher | — |
| 6 | 0 | Light Shotgun, Panzerfaust | — |
| 10 | 0 | Marksman Rifle profile | — |
| 9 | 0 | Camouflage; Rifle, Light Shotgun | — |
| 8 | 0 | Camouflage; Light Shotgun, Panzerfaust | — |

### Triphammer, Repurposed Industrial TAG

**ID 1569 · AVA 1 · TAG** — Full Power `MOV 15-10 | CC 17 | BS 13 | PH 16 | WIP 12 | ARM 7 | BTS 3 | W 3 | S 7`. Tactical Awareness; Turtlemek ancillary REM.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 53 | 1.5 | AP Spitfire, Heavy Flamethrower, AP CC Weapon | — |
| 52 | 1.5 | AP Spitfire, Chain-colt (+1B), AP CC Weapon | — |
| 52 | 0 | Heavy Shotgun, Thunderbolt (+1B), AP CC Weapon | — |
| 48 | 0 | Heavy Shotgun, Heavy Rocket Launcher, Panzerfaust (+1B), AP CC Weapon | — |

### Haytham Aero-unit

**ID 1851 · AVA 1 · VH** — `MOV 20-5 | BS 13 | PH 13 | WIP 14 | ARM 3 | BTS 6 | W 2 | S 7`. Aerial attack vehicle.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 33 | 1.5 | Red Fury, Panzerfaust, AP Heavy Pistol (+1B) | — |
| 29 | 0 | Heavy Shotgun (+1B), Chain Rifle, Panzerfaust | — |

### Azra'il

**ID 330 · AVA 1 · HI** — `MOV 10-10 | CC 15 | BS 13 | PH 11 | WIP 14 | ARM 5 | BTS 3 | W 2 | S 5`.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 37 | 1.5 | AP HMG, Chain Rifle, AP Heavy Pistol | Fireteams I, max 1 |
| 41 | 1.5 | Feuerbach, Chain Rifle, AP Heavy Pistol; BS Attack (+1B) | same |

### Ghulam Infantry

**ID 301 · AVA TOTAL · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 11 | 0 | Rifle, Light Shotgun | — |
| 20 | 1 | HMG | — |
| 17 | 1.5 | Missile Launcher | — |
| 16 | 0.5 | Rifle, Light Shotgun; Hacking Device | — |
| 15 | 0 | Rifle, Light Shotgun; Doctor (+1), MediKit | — |
| 12 | 0 | Rifle, Light Shotgun, Flash Pulse; Forward Observer | — |
| 13 | 0 | Rifle, Light Shotgun, E/M Mine; Deployable Repeater | — |
| 11 | 0 | Rifle, Light Shotgun; Lieutenant | — |
| 15 | 1 | Rifle, Grenade Launcher, Smoke Grenade Launcher; NCO | — |
| 12 | 0 | Rifle, Light Shotgun, Panzerfaust; Number 2 | — |
| 15 | 0 | Rifle, Light Shotgun; Lieutenant (+1 Command Token) | — |
| 13 | 0 | Rifle, Light Shotgun; Commlink (+2), Specialist Operative | — |

### Mukhtar, Active Response Unit

**ID 1313 · AVA 2 · MI** — `MOV 15-5 | BS 13 | WIP 14 | ARM 2 | BTS 6 | W 1 | S 2`. NWI mobile specialist family.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 25 | 0 | Viral Rifle, Nanopulser (+1B) | Fireteams I, max 2 |
| 26 | 0 | Boarding Shotgun, Nanopulser; Doctor | same |
| 25 | 0 | Rifle, Light Shotgun, Flash Pulse, D-Charges; Forward Observer | same |
| 29 | 0.5 | Hacking Device profile | same |
| 34 | 1 | Red Fury, Nanopulser; MSV2 | same |

### Medical Specialist Rahman Rouhani

**ID 1549 · AVA 1 · LI** — Doctor character with NWI.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 21 | 0 | Submachine Gun, Flash Pulse, Pistol; Doctor (+1), MediKit | Fireteams I, max 1 |

### Hassassin Nadhir

**ID 1545 · AVA 1 · LI** — Concealed reactive / ambush infantry.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 26 | 0.5 | AP Marksman Rifle | — |
| 23 | 0 | Rifle, Light Shotgun, Panzerfaust | — |
| 20 | 0 | Submachine Gun, Flammenspeer | — |
| 26 | 0 | Submachine Gun, Thunderbolt | — |
| 29 | 0.5 | AP Marksman Rifle, Viral Mine; Minelayer | — |

### Shaytaniyah Remotes

**ID 317 · AVA 1 · REM** — Guided missile REM.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 16 | 1.5 | Missile Launcher, PARA CC Weapon; Guided | — |
| 19 | 1.5 | Missile Launcher (+1B), PARA CC Weapon; Guided | — |

### Kameel Remotes

**ID 334 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 4`. Baggage support REM.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 8 | 0 | Deactivator, Repeater, PARA CC Weapon; Baggage | — |
| 14 | 0.5 | EVO Hacking Device; Baggage / support package | — |
| 16 | 0 | Rifle, Light Shotgun, PARA CC Weapon; Repeater, Total Reaction | — |

### Sayiq TAG Support Pilots

**ID 1849 · AVA 1 · LI** — TAG-support pilot unit; the source exposes separate Shakush and Maghariba support profiles.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 9 | 0 | Shakush Pilot: Submachine Gun, D-Charges; GizmoKit | — |
| 10 | 0 | Maghariba Pilot: Light Shotgun; GizmoKit, MediKit / Paramedic support | — |

### Yuan Yuan

**ID 378 · AVA 2 · WB** — Irregular, Impetuous airborne warband.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 6 | 0 | Chain Rifle, Smoke Grenades, Heavy Pistol, AP CC Weapon | — |
| 7 | 0 | Chain Rifle, Smoke Grenades, Pistol, DA CC Weapon | — |
| 11 | 0 | Boarding Shotgun, Smoke Grenades, AP CC Weapon | — |
| 11 | 0 | Rifle, Smoke Grenades, AP CC Weapon | — |

### Shakush Light Armored Unit

**ID 1546 · AVA 2 · TAG** — Tactical Awareness light TAG; Jandab operator support.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 58 | 1.5 | HMG (Continuous Damage), Heavy Flamethrower, AP CC Weapon | Fireteams I, max 1 |
| 56 | 1.5 | AP Spitfire, Heavy Flamethrower, AP CC Weapon | same |

### Kum Motorized Troops

**ID 313 · AVA 2 · WB** — Irregular, Impetuous motorcycle warband.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 6 | 0 | Chain Rifle, Smoke Grenades, Pistol, Shock CC Weapon | — |
| 7 | 0 | Light Shotgun, Smoke Grenades, Pistol, DA CC Weapon | — |
| 9 | 0 | Boarding Shotgun, Smoke Grenades, Pistol, E/M CC Weapon | — |
| 11 | 0 | Rifle, Light Shotgun, Smoke Grenades, Pistol, E/M CC Weapon | — |

### Knauf, Outlaw Sniper

**ID 939 · AVA 1 · LI** — Mercenary character included directly in the vanilla roster.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 31 | 1.5 | MULTI Sniper Rifle, AP Heavy Pistol, CC Weapon; Surprise Attack / Decoy package | — |

### Saladin, O-12 Liaison Officer

**ID 336 · AVA 1 · MI** — command character; Counterintelligence.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 38 | 0 | E/Mitter, Light Shotgun, Nanopulser, Pistol, Shock CC Weapon; Chain of Command | — |
| 39 | 0 | Same core kit; Lieutenant, Strategos L2, +1 Command Token | — |

### Scarface & Cordelia

**ID 380 · AVA 1 team · TAG + LI** — enabled Army-list choices bundle **Scarface Turner** and **Cordelia Turner**. Scarface is `MOV 15-10 | CC 22 | BS 13 | PH 16 | WIP 13 | ARM 7 | BTS 6 | W 3 | S 7`; Cordelia is `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Scarface supplies Tactical Awareness; Cordelia is an Engineer.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 80 | 1.5 | Scarface Loadout Alpha + Cordelia Turner | — |
| 76 | 1.5 | Scarface Loadout Beta + Cordelia Turner | — |
| 76 | 1.5 | Scarface Loadout Gamma + Cordelia Turner | — |

### Hassassin Lasiqs

**ID 328 · AVA 1 · LI** — Viral-weapon marksman / specialist.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 25 | 1 | Viral Sniper Rifle | — |
| 25 | 0.5 | Viral Marksman Rifle profile | — |
| 22 | 0 | Viral Rifle, Light Shotgun, Flash Pulse; Forward Observer | — |

### Bashi Bazouks

**ID 325 · AVA 2 · LI** — Irregular Holoprojector / Parachutist assault infantry.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 13 | 0 | Contender / close-range assault package | — |
| 14 | 0 | T2 Boarding Shotgun package | — |
| 16 | 0 | Rifle, Light Shotgun, E/M Mine; Specialist Operative | — |
| 14 | 0 | Breaker Rifle package | — |
| 12 | 0 | Submachine Gun package | — |

### Odalisques

**ID 324 · AVA 4 · LI** — `MOV 15-5 | CC 19 | BS 12 | PH 10 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. Sixth Sense, NWI, Combat Instinct, Natural Born Warrior.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 19 | 0 | Submachine Gun, Contender, Pulzar, Pistol, PARA CC Weapon | Fireteams II, max 2 |
| 21 | 0 | Submachine Gun, Contender, Pulzar, MULTI Pistol, PARA CC Weapon | same |
| 24 | 0 | Rifle, Light Shotgun, Pulzar, Pistol, PARA CC Weapon; BS Attack (+1B) | same |
| 22 | 0 | Boarding Shotgun, Pulzar, Pistol, PARA CC Weapon; BS Attack (+1B) | same |
| 26 | 0 | Viral Marksman Rifle, Pulzar, MULTI Pistol, PARA CC Weapon; Marksmanship | same |
| 21 | 0 | Submachine Gun, Pulzar, Flash Pulse; Paramedic, MediKit | same |

### RacerBots

**ID 1905 · AVA 2 · REM** — `MOV 20-10 | CC 13 | BS 11 | PH 12 | WIP 11 | ARM 0 | BTS 3 | W 1 | S 2`. Fast disposable control REMs.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 9 | 0 | RacerBot Mk-I: Adhesive Launcher Rifle, PARA Mine, PARA CC Weapon (-6) | — |
| 9 | 0 | RacerBot Mk-II: Heavy Riotstopper, Mine Dispenser (PARA), PARA CC Weapon (-6) | — |

## Canonical vanilla Fireteam chart

### Global limits

| Type | Limit |
|---|---:|
| Core | 0 |
| Haris | 1 |
| Duo | 2 |

The pinned Army chart gives every member row below `required: false` and `min: 0`. Membership is therefore a pool, constrained by the normal Fireteam size/type rules, the global caps above, and each row's maximum. No mandatory anchor is added here.

### Haqqislam Fireteams I

**Type:** Duo

| Entry | Min | Max | Profile restriction / note |
|---|---:|---:|---|
| NAFFATÛN | 0 | 2 | — |
| ZHAYEDAN | 0 | 2 | — |
| MUKHTAR | 0 | 2 | — |
| DJANBAZAN | 0 | 2 | — |
| HAFZA | 0 | 1 | — |
| AZRA'IL | 0 | 1 | — |
| NAJJARUN Engineer | 0 | 1 | — |
| MAGHARIBA | 0 | 1 | — |
| SHAKUSH | 0 | 1 | — |
| ROUHANI | 0 | 1 | — |
| YARA HADDAD | 0 | 1 | — |

### Haqqislam Fireteams II

**Types:** Duo, Haris

| Entry | Min | Max | Profile restriction / note |
|---|---:|---:|---|
| BURKUT | 0 | 2 | — |
| KORSAN FTO | 0 | 2 | **FTO profiles only** |
| ODALISQUE | 0 | 2 | — |
| SEKBAN | 0 | 2 | — |
| KHAWARIJ | 0 | 1 | — |
| MUYIB | 0 | 2 | — |
| JANISSARY | 0 | 1 | — |
| LEILA SHARIF | 0 | 1 | — |

## Reverse Fireteam access index

| Troop / profile | Pool | Types | Max | Notes |
|---|---|---|---:|---|
| Naffatûn | Fireteams I | Duo | 2 | — |
| Zhayedan | Fireteams I | Duo | 2 | — |
| Mukhtar | Fireteams I | Duo | 2 | — |
| Djanbazan | Fireteams I | Duo | 2 | — |
| Hafza | Fireteams I | Duo | 1 | — |
| Azra'il | Fireteams I | Duo | 1 | — |
| Najjarun Engineer | Fireteams I | Duo | 1 | — |
| Maghariba Guard | Fireteams I | Duo | 1 | — |
| Shakush | Fireteams I | Duo | 1 | — |
| Rouhani | Fireteams I | Duo | 1 | — |
| Yara Haddad | Fireteams I | Duo | 1 | — |
| Burkut | Fireteams II | Duo / Haris | 2 | — |
| Korsan FTO | Fireteams II | Duo / Haris | 2 | FTO profiles only |
| Odalisque | Fireteams II | Duo / Haris | 2 | — |
| Sekban | Fireteams II | Duo / Haris | 2 | — |
| Khawarij | Fireteams II | Duo / Haris | 1 | — |
| Muyib | Fireteams II | Duo / Haris | 2 | — |
| Janissary | Fireteams II | Duo / Haris | 1 | — |
| Leila Sharif | Fireteams II | Duo / Haris | 1 | — |

All standard roster entries absent from this reverse index have no Fireteam access in the pinned vanilla chart. In particular, the current source does not add `Fiddler FTO`, `CLAIRE LAZHARI FTO`, or `RAFIQ REMOTE FTO` to either vanilla pool.

## Reinforcement relationship and source relations

Linked Reinforcement army: **Melek Reaction Group (Army ID 499)**.

The vanilla source also carries explicit relation groups pairing ordinary and Reinforcement versions of two named characters:

- Husam Operative Leila Sharif: ordinary unit ID `849` ↔ Reinforcement ID `1665`.
- Medical Specialist Rahman Rouhani: ordinary unit ID `1549` ↔ Reinforcement ID `1666`.

These are source-level duplicate-character / roster relations and are kept distinct from Fireteam membership.

## Reinforcement Fireteams — Melek Reaction Group

Source revision: `7.26246.158`.

These rows are intentionally separate from the standard vanilla Haqqislam Fireteam chart. The current Reinforcement source exposes global `spec` values of **Core 0; Haris 0; Duo 0** while its team rows explicitly declare Fireteam types. This reference preserves both facts instead of inventing non-zero global caps.

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

## Validation notes

- Standard roster count reconciled to **56** ordinary matched-play entries: the 58 pre-catalogue source entries minus `Haqqislam Team-Ops` and `Husam Spec-Ops` optional modes.
- Generic `merc-*` catalogue copies with empty faction lists are excluded.
- Army ID `401` is `discontinued: false` in the pinned N5 Army metadata.
- `Scarface & Cordelia`, `Triphammer`, and `Fiddler` are retained because their ordinary source entries explicitly include faction 401.
- Directory-only files do not establish vanilla membership: `Sacha Xenotech Hunters` and `Zaybak Aero-unit` are not in the pinned vanilla roster; `Zeybek Aero-unit` and `Haytham Aero-unit` are.
- The complete standard vanilla Fireteam chart is represented: global Core 0 / Haris 1 / Duo 2; Haqqislam Fireteams I (Duo); Haqqislam Fireteams II (Duo/Haris).
- All rows in both standard vanilla pools are `required: false`, `min: 0`; no anchor requirement is invented.
- `KORSAN FTO` profile-only Fireteam access is preserved. `Fiddler FTO`, `CLAIRE LAZHARI FTO`, and `RAFIQ REMOTE FTO` are not granted vanilla Fireteam access because they are absent from the canonical vanilla chart.
- Source relations pairing ordinary and Reinforcement Leila Sharif / Rouhani are recorded separately from Fireteam membership.
- Linked Reinforcement army resolves to **Melek Reaction Group (499)** and its chart is kept separate, including the unusual current source combination of global `spec` 0/0/0 and explicitly typed Fireteam rows.
- Source data and Fireteam normalization were rechecked on **2026-10-15** against the pinned Army snapshot and InfinityDB commit listed in the front matter.

## Community tactics — transcript-backed Vanilla N5 research (2026-10-22)

> **Authority, date and terminology:** These are **community analyses**, not replacements for the pinned **N5.3 / Army 7.26246.158** roster, options, 56-unit AVA and Fireteam chart above (last verified 2026-10-15). **Vanilla: no Core, one Haris, two Duos**; the two mixed Fireteam pools are **not interchangeable**. In particular, a 2025-10-13 podcast predates the **2025-10-15 N5.2 update**, which gave Saladin **Inspiring Leadership** and changed the viability of Irregular-heavy lists. Automatically transcribed "Shaykh Bakr / Shaykh Bakr Aero-unit" in Robert Shepherd's 2025 video is the **Zeybek Aero-unit** (33-point AP Spitfire/Smoke), *not a third named Haqqislam Vehicle or a separate current roster entry*. The two playable vanilla aerial Vehicles in the pinned source are **Haytham and Zeybek**. When in doubt about a remembered skill or old example, use the current roster/rules.

### The short answer: what actually makes Vanilla Haqqislam strong?

- **Saladin Lieutenant (39) + efficiently priced former Irregulars** is the defining post-October-2025 archetype. Inspiring Leadership lets **Muttawi'ah, Daylami, Hunzakut, Kum/Zamira/Zuleyka**, etc., generate Regular Orders while the relevant effect applies; Strategos L2 and the extra Command Token help **reserve deployment, reorganize combat groups and repeatedly Coordinate attacks/smoke/movement**. A 15-model Saladin list can be 15 useful Regular Orders **without paying for 15 conventional line infantry**. See [current N5 Saladin skills](https://human-sphere.com/Saladin) and the [N5.2 Saladin update discussion](https://forum.corvusbelli.com/threads/crazy-saladin-lists.43718/).
- **Cheap protection enables quality attack pieces**: Ghazi Jammers and expendable Camo Daylami threaten approach lanes; coordinating fast bikes/flyers and choosing the right **Mukhtar, Janissary, Asawira, Azra'il, Fiday, TAG or Vehicle** converts that screen into objectives/kills. High average **WIP** helps Discover, objective buttons, hacking and medical support, not just gunfighting.
- **The actual list-building question is not "what is the best unit?" but "what defeats the defenses stopping my objectives?"** Bring answers to enemy MSV/mimetism, armor/TAGs, hacking, marker states and inaccessible objectives. Haqq excels at matching **one problem with a specialized tool**, not at universally superior gun stats.
- **Liability:** Saladin is a relatively obvious high-value Lt. Losing him may cause **Loss of Lieutenant plus loss of Inspiring Leadership**, turning many Orders Irregular. Protect against Guided/spotlight attacks and backfield entry; do not rely on a fragile, one-layer deployment-zone defense.
- **If deliberately skipping Saladin**, the faction still has quality individuals, but Irregular Order economics worsen substantially. Take the non-Saladin Lt/CoC/NCO path because it enables a *specific* mission/team plan, not by copying a Saladin swarm and assuming all its Orders remain Regular.

### Compact module guide — every pick needs a reason

| Choice in current Vanilla roster | Main payoff / best use | Tradeoff or disagreement |
|---|---|---|
| **Saladin Lt (39) / CoC (38)** | Lt is the force multiplier for **Inspiring Leadership, Strategos L2, Counterintelligence** and Command-Token/Coordinated-Order play. Reserve key attack pieces, move an Order to the group that needs it, Coordinate bike smoke or multiple disposable Panzerfaust ARO clearances. | Lt is vulnerable/high-priority and imposes the Saladin shell game. **CoC Saladin lacks the Lt-only leadership plan**: the 2026 list guide advises against it except for a deliberately distinct plan. Bashi Holomask can complicate targeting, but doesn't magically hide Repeater coverage or guaranteed Lt identity. |
| **Ghazi Muttawi'ah (5–8), especially 6pt Jammer** | **AVA4** inexpensive Jammer/smoke/template area denial; Saladin turns their Irregular Orders into useful Regular group economy. Great corner defense and order-draining screen; can Coordinate if legally eligible. | Jammer matters only if positioned to stop the actual enemy route. Impetuous movement must be staged safely; a defensive net is not a plan to score objectives. |
| **Daylami (8pt Camo Panzerfaust + LSG)** | **AVA3** hidden-ish roadblocks; cheap chance to threaten elite models with a disposable Panzerfaust while consuming enemy Discover/clearance Orders. Under Saladin also a Regular Order. | Fragile; if enemy has good Sensor/template routes, they may die without trading. They should **buy time for the real attack**. |
| **Zuleyka (9), Zamira (11), regular Kum (6–11)** | Motorcycles provide **early smoke, fast coordinated positioning and brutal short-range trades**. Zuleyka leans close assault, Zamira better pistol/shooting and E/M interaction; both can punish backfield openings. | **Non-Saladin** Kum/biker Irregular Orders are harder to fund. Bikes are vulnerable to terrain, templates and overextension; don't park them in predictable reactive lines. |
| **Hunzakut FO (15) / FO+Repeater (19)** | **AVA2** cheap Camo Infiltration specialists. 15pt for efficient mission scoring, 19pt when **Deployable Repeater** is needed to project the Barid/Leila hacking net; excellent value if Saladin makes it Regular. | Irregular without leadership; 1W and limited fighting capacity. 19pt upgrade is not universally needed; select by network plan. |
| **Barid KHD/Pitcher + Leila Sharif** | Barid's hacker/Pitcher can project **actual hacking influence** beyond the deployment zone; Leila brings KHD, Combat Instinct/Carbonite and wildcard Haris eligibility (Fireteams II). Together they threaten hackable rush pieces and protect the Saladin DZ. | **Hacking needs a network**: a lone Guided missile bot without Pitcher/repeater/FO setup underperforms. Spending Orders on speculative Pitcher shots is not automatically efficient after N5 changes. |
| **Mukhtar MSV2 Red Fury / FO / Doctor / Hacker** | **Mimetism, NWI, Forward Deployment** and MSV2: flexible mobile shooter/specialist. Vanilla **Fireteams I Duo** can combine Mukhtar + another eligible gun, specialist or support; a Mukhtar fighting through coordinated smoke is especially potent. | Not a heavy-armor killer with its Red Fury; medium cost and 1W+NWI can vanish under several hits. Has no native Haris in vanilla; its sectorial Mukhtar Haris does **not** carry over. |
| **Janissary HMG, Azra'il AP HMG/Feuerbach, Djanbazan MSV2** | Different gun answers: **Janissary** reliable BS14/modifier durability; **Azra'il** extreme long-range AP/Continuous-Damage pressure; **Djanbazan** smoke+MSV2 against units not able to see through smoke. | Strong guns consume SWC and orders; Djanbazan BS12 may be unreliable without the vision advantage. No Ramah Janissary Core or Qapu QK Azra'il Haris is legal here. |
| **Asawira / Yara Haddad / Khawarij** | **Asawira** is a compact resilient close-range hitter or Doctor; **Yara (24)** offers cheap MSV2/AP Marksman in Fireteams I; **Khawarij** contributes jump angles, MSV2/NCO or mission skills in Fireteams II. | Pick the actual role: Asawira is not automatically better than a Saladin-Coordinated attacker because it isn't in either vanilla FT chart; one expensive close-range brawler doesn't fix long-ranged AROs. |
| **Fiday** | **Impersonation** disrupts enemy deployment, forces cautious movement and threatens a priority target. A coordinated **long-range smoke delivery** can get it into close combat despite N5 loss of some easy template attacks. | **Robert Shepherd** and the April 2026 guide say Fiday is **less automatic in N5**: setup/Order intensive versus simply fielding more smoke, bikes or a gun. Its main value may be a *threat/roadblock* rather than a guaranteed Turn-1 kill. |
| **Nadhir / Sunduqbut / Farzan viral minelayer** | Nadhir provides Hidden Deployment ARO/ambush; Sunduqbut brings a more expensive Camo/Neurocinetics or viral denial package; **Farzan minelayer** secures objectives with viral mines. | Spend on hidden defense or problem-piece only when the enemy plan justifies it. Sunduqbut costs 42–50 points—competes with a real attacking unit; can be too much for a Saladin cheap-Orders plan. |
| **Bashi Bazouk / Korsan / Ragik / Yuan Yuan** | Cheap **Parachutist/Combat Jump** and edge attacks create a second offensive vector while primary guns force opponents to stay behind cover. Bashi offers Holomask/decoy for Lt protection; Korsan for mobile close assault or FTO Haris support. | Need secure entry edges and enough Orders; they are not all comparable. **Korsan FTO only** can join vanilla Fireteams II; non-FTO parachutist Korsan cannot. |
| **Hafza Lt (+1 Lt Order) / CoC (20) + Ghulam NCO** | Non-Saladin alternative: hidden Lt +1 Order/CoC with NCO smoke/support, or **Shakush + Hafza FO Duo** (Fireteams I) to carry a button-pusher along with Tactical Awareness. | These are **alternative plans**: giving up Saladin sacrifices Inspiring Leadership. If Saladin is Lt, multiple NCOs do not become free Orders; understand how Strategos changes Lt-Order use. |
| **Odalisque / Burkut / Sekban / Muyib** | Fireteams II Haris can use **Odalisque durability/Disco Baller**, Burkut engineer + short-range tech, Sekban NCO/specialist, or Muyib deployment tools around a Janissary/Khawarij gun. | Some members are costly, and **Fireteams II cannot import Fireteams I members**. Research videos praising Qapu or Ramah mixed teams are *role examples*, not vanilla membership permission. |
| **RacerBots (9) / specialist-support utility** | Fast **20-10 MOV**, Adhesive Launcher or Riotstopper / PARA-mine disposable control attacks can delay an elite assault or pin a target long enough for the main threat to finish it. | **AVA2 REM**, not a central gun or specialist, and no returned source strongly establishes them as a default pick; treat as mission-/terrain-specific tech rather than community consensus. |

### Repeatable list patterns

1. **Saladin "Army of Cheese" / Order wall:** 39pt Saladin, **2–4 Ghazi**, **1–3 Camo Panzerfaust Daylami**, a Hunzakut (FO or Repeater), one or two **bikes**, then deliberately choose **one armored/gun centerpiece + a mission specialist/hacker**. Aim for useful 15-model coverage: cheap converted Orders are powerful because the same models also impose Jammer/Camo/ARO threats. Deployment-zone safety is critical: losing Saladin undermines both leadership and the list's economy. [April 2026 list review](https://www.youtube.com/watch?v=dySCSPJ9vmA).
2. **"Knights of the Sky" / twin flyers:** Same Saladin defensive shell but invest in **Haytham (33/29) + Zeybek (33)**. **Haytham MSV1 + Mimetism (-6)** hunts ordinary Mimetism and enemy flyers; **Zeybek Albedo (-6) + AP Spitfire / smoke GL** pressures MSV guns and tougher targets. The pair has complementary matchups; **Zeybek's smoke can help Haytham or ground MSV pieces reposition**, provided the smoke isn't counterproductive. This spends Orders/SWC and asks for a strong plan to hide S7 No-Cover vehicles. [April 2026 list review](https://www.youtube.com/watch?v=dySCSPJ9vmA).
3. **Traditional "toolbox" without Saladin:** A protected Hafza Lt, **Shakush + Hafza FO Duo**, Mukhtar/Djanbazan Fireteams I Duo, a Fireteams II Haris (e.g., Janissary + Odalisque + Leila, each eligible), Fiday/hacking/specialists and cheaper Regular backing. Works for mission-specific choices but **do not pretend the Irregular troops generate Regular Orders**.
4. **TAG with coordinated chaff:** **Maghariba or Shakush** plus Ghazi/Daylami roadblocks, a **Doctor/Engineer and anti-hacker support**. Under Saladin, the inexpensive former-Irregulars let you afford the TAG without the usual Order starvation. Go two-TAG only if all the fighters still have Orders, objective specialists and protection.
5. **Fireteam discipline (canonical):** Vanilla is **Core 0, Haris 1, Duo 2**. **Pool I is Duo-only** and can place *one* Maghariba or Shakush with **eligible Hafza/Najjarun/Rouhani/Yara/Mukhtar/etc.** **Pool II** supports *one* Haris with Janissary, Khawarij, Odalisques, Sekban, Burkut, Muyib, Leila or **Korsan FTO**. **No Rafiq FTO, Fiddler FTO, Claire Lazhari FTO** link membership. Both groups have no mandatory anchor in the pinned source; follow per-row maxima. **Two Maghariba can be bought (AVA2) but not combined as two Maghariba inside Pool I's Duo (max1).**

### The complete vanilla TAG / Vehicle / REM ecosystem

| Eligible choice (pinned N5.3) | Why / best fit | Counterpoint / current legality |
|---|---|---|
| **Maghariba Guard TAG (AVA2)** 71–72pts / 1.5SWC | **BS14, ARM8, W3, S8**, 360° Visor, Tactical Awareness, Baggage + Jandab. All variants have MULTI HMG: **E/M Carbine (+2B)** versus armor/HI; **HRL+GL** for other firing bands; **HFT (+1B) + Shock Mine Dispenser** creates replenishable mine coverage. Saladin's cheap converted Orders subsidize it. | Extremely hard to hide S8; a large target for guided/hacking/counter-TAG weapons. **Only 1 Maghariba per Fireteams I Duo**, despite AVA2. Double-Maggie is a points/mission gamble, not a normal link. **Robert** likes the efficiency but flags huge silhouette. |
| **Shakush TAG (AVA2)** 58pt Continuous HMG / 56pt AP Spitfire | Compact **BS14 ARM6 W3** TacAware gun; HMG long-range Continuous Damage is effective against elite infantry, AP Spitfire into armor. **Shakush + Hafza FO** is an economical **legal** Pool I Duo that can move with the TAG's Order. Jandab included; Sayiq support pilot is separate. | **Robert** judges it solid, **Ramah reviewers** debate whether a Janissary HMG delivers better value, and **Qapu** often prefers Iguana instead. In *Vanilla*, evaluate mission and relative opportunity cost, not other sectorials' TAG roster. |
| **Scarface & Cordelia (AVA1 bundled)** 76/80pts / 1.5SWC | Mobile TAG gun + Cordelia **Engineer and her own Regular Order**, with strong active assault and close combat. Useful when a repair/support specialist would be taken anyway. | Can't buy Scarface alone; bundled price makes it harder to justify vs Maghariba/Shakush. **No vanilla FT row**; Qapu's Zırhlı mix doesn't transfer. |
| **Triphammer TAG (AVA1)** 48–53pts / 0–1.5SWC | Low-cost Tactical Awareness armored threat; **zero-SWC** Heavy Shotgun/HRL or Thunderbolt profiles preserve SWC for Azra'il/Janissary/Vehicle. Select when points/SWC demand a budget TAG. | **Robert's least-favored/most situational TAG** in Vanilla: BS13, BTS3 and less flexible gun reach than the main battle TAGs. **No vanilla FT row**; Qapu TAG Duo not legal. |
| **Haytham Aero-unit (VH AVA1)** 33pt Red Fury/Panzerfaust or 29pt BSG | **20-5 MOV, MSV1, Mimetism (-6), Continuous Damage** and aerial maneuver produce plunging shots, dangerous soft-target hunting and **especially strong anti-flyer** attacks against other vehicles depending on Mimetism. Better default general-purpose flyer when opponents rely on Mimetism. | **S7 / No Cover / W2** vehicle, vulnerable if exposed; Red Fury struggles against heavy armor. Dedicated post-N5.2 vehicle review rates it near **#4 among eight flyers**, good but relatively one-dimensional. |
| **Zeybek Aero-unit (VH AVA1)** 33pt AP Spitfire + Smoke GL | **20-5 MOV, ARM5, W3** and included Operator. **Albedo(-6) versus MSV/Marksmanship**, plus AP Spitfire and smoke, can answer the exact vision pieces that hinder Haytham or smoke-shooters. Post-N5.2 weapon/modifier changes made it extremely attractive; Robert's [Vehicle ranking](https://www.youtube.com/watch?v=N6TYjMgU4ZM) puts it **#2 among the eight** because it fills a high-value faction gap. | Pre-October Tactical Awareness questioned its older niche/efficiency; **that criticism is dated**. Albedo does not debuff ordinary visors-less enemies, and flyer No Cover/S7/escape mechanics still need thoughtful protection. **No "Shaykh Bakr" separate unit** in the pinned roster; 2025 auto-transcripts are phonetically misreading **Zeybek**. |
| **Rafiq REM (AVA2)** 13pt sensor/FO/repeater or 19pt Red Fury FTO | 13pt **Sensor + Triangulated Fire + FO/Repeater** clears Camo and scores buttons; low-order-cost midfield hacking extension. The FTO Red Fury is a modest mobile gun if its profile is desired. | **Rafiq FTO has no Vanilla Fireteam row**, even though it *does* in Qapu/Ramah. Buying FTO to get a link here is a legality error. |
| **Shihab REM (AVA1)** 23pt TR HMG / 18pt TR Thunderbolt (+1B) | Cheap independent **Total Reaction/360°** ARO support to cover a lane Saladin cannot risk guarding. Repair with **Najjarun or other Engineer + Nasmat**. | **Only AVA1 in Vanilla**, unlike Qapu/Ramah AVA2. Cannot copy the double-Shihab defense popular in Ramah. ARO bots are removable by dedicated counters; combine with Ghazi/Camo depth. |
| **Shaytaniyah REM (AVA1)** 16pt Guided ML / **19pt ML(+1B), Guided per Vanilla pinned source** | A **Targeted → Guided** missile plan with Barid Pitcher, Hunzakut/Rafiq FO/repeaters, Leila and other hacking setup forces enemies to respect non-LOS threat. | **Both Vanilla loadouts labeled Guided in this reference**; don't transfer Ramah's different text to Vanilla or vice versa. 1.5SWC is wasted if you never establish Targeted. |
| **Kameel REM (AVA2)** 8pt Baggage/Repeater, 14pt EVO, 16pt TR Rifle | Reloads **Pitchers, mines and Jammer / disposable networks**, helps sustain an attrition list and contributes cheap Regular Order. **EVO** when supportware or an airborne/TAG plan justifies it. | Maghariba already has Baggage for its mines; second Kameel/EVO is not a reflex pick. |
| **Fanous REM (AVA1)** 7pt flash/repeater | Cheapest conventional Regular-order **Flash Pulse and zone repeater** to shore up leadership DZ and hacking coverage. | **Only one** in Vanilla, despite higher availability in Ramah. In Saladin lists compare it to a 5–8pt Ghazi/Daylami that also contributes a Regular Order *and* an offensive deterrent. |
| **RacerBots (AVA2)** 9pt Adhesive Launcher/PARA Mine or Riotstopper/PARA Mine Dispenser | **20-10 MOV**: fast cheap disruption, counter-rush and temporary area-denial against elite bodies, including targets too tough for routine bullets. | They're specialist tools, not default cheap attack guns. No Fireteam row; avoid depending on a PARA trade to defeat a prepared opponent. |
| **Nasmat peripheral + separate Sayiq pilot** | Nasmat extends Engineer/Doctor reach; 9pt Shakush / 10pt Maghariba Sayiq pilot helps a TAG-specific support plan; included Jandabs have their own ancillary mission functions. | **Peripheral and bundled Jandab do not create Regular Orders**. Spending points on a pilot/repair package must be justified by keeping your expensive TAG working. |

**Parent-faction crossover is for tactics, not roster changes.** [Ramah N5](https://www.youtube.com/watch?v=dvSrZU73hxA) provides Haytham/Maghariba/Shakush, Shihab and repair discussion; [Qapu Khalqi N5](https://www.youtube.com/watch?v=rOy0x0BLuNU) provides TAG comparison and Pitcher+Baggage examples; [Hassassin Bahram N5](https://www.youtube.com/watch?v=yHpAnRDw_E8) gives Fiday/mine/repeater positional insights. **Do not** import their Fireteam sizes, high REM AVA, Iguana, Tarik, or sectorial-only profiles into current Vanilla.

### Debated conclusions (include all relevant views)

1. **Saladin all the time?** **Robert Shepherd** expects the overwhelming majority of strong current lists to be Saladin + former Irregulars; [April 2026 list-building guide](https://www.youtube.com/watch?v=dySCSPJ9vmA) strongly dismisses **CoC Saladin** because it discards Lt-only benefits. **Counter-view:** Reddit and Corvus players worry Saladin swarm is overpowering/monotonous, while some want other leadership and fully Regular toolboxes. **Practical:** Saladin offers superior cheap-order conversion but creates an obvious failure point and can be less natural in armies relying on specialist active Orders rather than many Coordinated Orders. ([Community tactical criticism](https://www.reddit.com/r/InfinityTheGame/comments/1px4kn4/how_to_tackle_the_new_haqq_a_bit_of_a_rant/))
2. **Fiday alpha-strike or defensive roadblock?** N4's low-risk template delivery weakened in N5; **Robert** likes supplying smoke via fast coordinated bikers/flyer then committing to CC; **April 2026 reviewer** often starts it outside the enemy DZ as a threat demanding Orders rather than relying on immediate assassination. **Pick according to table and mission.**
3. **Haytham vs Zeybek vs both:** **October 13, 2025 Tactical Awareness** is skeptical of Zeybek's pre-update niche and praises Haytham's reliable Mimetism; **post-October Vehicle review** ranks Zeybek #2 because **AP Spitfire, Albedo and smoke** now offset MSV counters; **April 2026 guide** proposes both together because each preys on the other's counters. **Pick by opposition, SWC/Orders and terrain.**
4. **TAG investment or mixed skirmishers:** **Robert** considers Maghariba and Shakush reasonably costed and even multiple TAGs possible *with* Saladin discount Orders; the **Ramah reviewers** emphasize how often the same points instead buy a more coherent specialist-defense network. **Vanilla does TAGs better than Ramah economically**, but not every mission needs two large targets.
5. **Guided/hacking or cheap ambush:** Podcast players explore missile REMs, Killer Hackers and unusual defenses. Community list critics argue a guided bot without Pitchers/safe Targeted projection wastes SWC; **Robert** favors a *light, purpose-built* network in many Saladin lists instead of sacrificing gunfighting for a full hacking castle. Both work where mission/opponent supports them.
6. **MSV smoke shooter:** **Djanbazan** linked AP Sniper/HMG offers traditional smoke-based punishment; **Mukhtar** trades long HMG bands for Mimetism, mobility/Forward Deployment and potentially better solo action. **Yara** gives inexpensive MSV2/AP marksman for cheap Duo utility. The best gun depends on target range, smoke matchup and desired mission coverage.
7. **Go to 15 cheap Orders or make every model useful?** Pro-Saladin camp says a 5pt converted Regular Ghazi is great **even before** it fights; critics argue list slots spent on pure filler lose objective/attack capacity. **Resolution:** prioritize cheap units that *also* Jam, Camo/Panzerfaust, Smoke, FO, or project Repeaters, and don't buy five idle bots purely for the Order count.

### Best source shortlist and transcript status

**MCP transcripts actually retrieved/read for this update:**

1. **[Robert Shepherd — Infinity N5 Faction Focus: Haqqislam (2025-11-23)](https://www.youtube.com/watch?v=Dmv4pfdTbc0)** — **best complete reference** after N5.2: Saladin/Coordinated-Order engine, cheap troop economy, Fiday, specialist choices, four TAGs and the two Vehicles.
2. **[KARARGAH — Infinity N5 Haqqislam Guide: Army of Cheese vs Knights of the Sky (2026-04-05)](https://www.youtube.com/watch?v=dySCSPJ9vmA)** — **best explicit list-building primer:** evaluates leadership vulnerability, Ghazi/Daylami shell, TAG/multi-flyer configurations and Fiday's newer role; author cautions these are personal experiences, not tournament consensus.
3. **[Robert Shepherd — Infinity Explained: Aerial Vehicles Analysis and Ranking (post-2025-10)](https://www.youtube.com/watch?v=N6TYjMgU4ZM)** — most useful specialized **Vehicle** review: Haytham matchup vs Zeybek Albedo/AP Spitfire/smoke, flyer risks, counterplay, conflicting rankings.
4. **[Tactical Awareness S3 — Haqqislam Prime (2025-10-13)](https://www.youtube.com/watch?v=qlKwZjGWDDY)** / **[Spotify](https://open.spotify.com/episode/4gx0VBfits4q9PNwUiPIJh)** — **full podcast transcript**; competing 300-pt list archetypes: linked defense Djanbazan/Janissary, Camo/impersonation/parachutists, double Maghariba, bikes, technical link discussion. **Pre-N5.2**: don't reuse old Saladin/Zeybek balance claims.
5. **[Tactical Awareness — N5 Update v5.2 (2025-10-16)](https://open.spotify.com/episode/66UWrxKSTHcyWP3LJDM0H4)** — **full podcast transcript**, explicitly covers Saladin acquiring Inspiring Leadership and changes to the Irregular-order economy.
6. **[Robert Shepherd — Ramah Taskforce N5](https://www.youtube.com/watch?v=dvSrZU73hxA)**; **[Qapu Khalqi N5](https://www.youtube.com/watch?v=rOy0x0BLuNU)**; **[Hassassin Bahram N5](https://www.youtube.com/watch?v=yHpAnRDw_E8)** — full video transcripts consulted selectively for *shared* Maghariba/Shakush/Haqq REM, Fiday and TAG-support insights; their Fireteams/AVA **do not** establish vanilla legality.
7. **[Tactical Awareness S1 — Haqqislam Prime (2023-02-27)](https://open.spotify.com/episode/4sT6tMyuRTGqYi1P4Y8K0d)** — historical **N4** podcast transcript retrieved. Useful to understand why pre-October N5 Saladin opinions diverge; **do not use for current loadouts**.

**Other surfaced material, not claimed as transcript-reviewed:** [Corvus Belli N5 Haqqislam tactica index](https://forum.corvusbelli.com/threads/n5-recap-haqqislam-tacticas.43463/), [Bureau Aegis N5 Vanilla resource index](https://www.bureau-aegis.org/forum/index.php?topic=17830.0), and [2026 Reddit Saladin list debate](https://www.reddit.com/r/InfinityTheGame/comments/1px4kn4/how_to_tackle_the_new_haqq_a_bit_of_a_rant/). [Counterintelligence German N5 Haqqislam deep dive (2025-03-28)](https://open.spotify.com/episode/2F3vEWh0Znz8UdU2uh0qoT) had an MCP German transcript retrieved but is pre-N5.2; not treated as current tournament verdict.

**Transcript-quality warning:** Some YouTube auto-captions invent phonetic names: "Shaykh Bakr" = **Zeybek** for the 33pt AP Spitfire/smoke flyer; "Hayam" = **Haytham**. Historical podcast claims about two Maghariba links, AVA3 Fanous, vehicle attributes and Guided missiles must be checked against the **pinned Vanilla** chart above. Source-verified roster restrictions take precedence over speech transcription.

## TAG tactical cross-reference (2026-10-23)

**Maghariba (71–72)** is the ARM8, BS14 S8 heavy platform when the table fits it; **Shakush (56–58)** buys a much cheaper durable HMG/Continuous Damage or AP Spitfire and more specialist points; **Triphammer (48–53)** is an even cheaper but swingy budget assault; **Scarface & Cordelia (76–80)** is a **two-model TAG+Engineer bundle**, not an apples-to-apples TAG price. Choose according to range, S8 staging, and how much scoring/repair support remains.

For the two-tier **apex/points-value** comparison, TAG counterplay, matchup matrix and direct transcript sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Treat current profiles, points/SWC and canonical Fireteam data above as authoritative.

## Vehicle (VH) tactical cross-reference (2026-10-23)

**Haytham AVA1:** **33/1.5 Red Fury+Panzerfaust+AP Heavy Pistol** is a mobile **MSV1** hunter of Mimetism/VH; **29/0 Heavy Shotgun(+1B)/Chain Rifle/Panzerfaust** is a cheaper short flank. **Zeybek AVA1:** **33/1.5 AP Spitfire+Smoke GL**, **Albedo/anti-MSV** and **Operator** transition answer enemies shutting down Haqq's smoke game. **Neither is a Duo.** Albedo is not generic Mimetism against normal opponents. No Cover/S7/hackability limit both; keep specialists and Engineer/GizmoKit support.

See [VH apex/value tier list and matchup guide](../../notes/list-building/vehicles-vh.md). **Current profiles, AVA and canonical Fireteam chart above remain authoritative.**
