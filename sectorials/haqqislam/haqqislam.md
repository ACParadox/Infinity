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
