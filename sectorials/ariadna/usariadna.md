---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 304
sectorial_slug: usariadna
sectorial_name: USAriadna Ranger Force
parent_faction: Ariadna
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard USAriadna Ranger Force roster, standard loadouts, canonical Fireteam chart, reverse Fireteam index, and the distinct L'Équipe Argent Reinforcement Fireteam chart. Intel Spec-Ops and Ariadna Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# USAriadna Ranger Force

## Overview and provenance

Repository-native reference for **USAriadna Ranger Force (USARF / USAriadna)** roster, profiles, points/SWC, AVA, and Fireteam access.

Sources used:

- Army-derived USAriadna source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `d4329bb596ffea5d568eb2435f74366c305a7630`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **22-unit standard USAriadna roster** and the complete standard USAriadna `fireteamChart` in the pinned Army source.
- Army metadata currently marks **USAriadna Ranger Force as discontinued**, but a complete N5 roster and Fireteam chart remain present in the current Army data. `status: current` above refers to this reference being current with the pinned N5 data, not to the sectorial's discontinued flag.
- Soldier of Fortune / generic `merc-*` catalog entries whose source faction list is empty are excluded from the base roster.
- `Intel Spec-Ops` and `Ariadna Team-Ops` are optional game-mode content and are listed separately.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name by itself. This matters especially for Beasthunters: the source still calls the 9-point profile `BEASTHUNTER FTO`, but USAriadna's current Fireteam chart contains no Beasthunter row.
- Parenthetical Army-chart comments are treated as Counts-as / equivalence labels, not as join-scope restrictions.
- The structured `required: true` Minuteman and Marauder rows in USARF Fireteams are preserved as a **required-choice set**; this file does not reinterpret them as requiring one of each troop type simultaneously.
- USAriadna Grunts carry the source note **“Troops with F. Deployment cannot be part of Fireteams.”** The Forward Deployment Grunt option is therefore excluded from Fireteam membership even though Grunts are the native Grunt Fireteam troop.
- Devil Dog Fireteam access is profile-specific: only the `DEVIL DOG FTO` profile is represented by the USAMC Fireteam row. The ordinary Devil Dog + K-9 team profiles do not gain link access from that row.
- Linked Reinforcement army ID: **399**, **L'Équipe Argent**. Its Fireteam chart is recorded separately below and is not merged into the main USAriadna chart.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | USAriadna Ranger Force (USARF) |
| Parent faction | Ariadna |
| Army ID | 304 |
| Army slug | `usariadna` |
| Army metadata status | Discontinued |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 22 |
| Optional-mode units | Intel Spec-Ops; Ariadna Team-Ops |
| Reinforcement roster | L'Équipe Argent, Army ID `399` |
| Fireteam limits | Core 1; Haris 1; Duo unlimited |
| Fireteam chart | yes |

## Roster index

| Unit | ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| USAriadna Grunts | 230 | TOTAL | MI | Regular | Grunts; Forward Deployment profile cannot join |
| 112, Emergency Service | 255 | 2 | LI | Regular | Wildcard; counts as Grunt |
| Van Zant | 244 | 1 | LI | Regular + Tactical Awareness | — |
| Traktor Mul | 257 | 2 | REM | Regular | — |
| Wardrivers | 265 | 1 | LI | Regular | — |
| Beasthunters Free Guild | 1570 | 1 | SK | Irregular | —; `BEASTHUNTER FTO` name does not grant USARF access |
| Blackjacks | 775 | 3 | HI | Regular | Blackjacks |
| Warcors | 50 | 1 | LI | Irregular | — |
| 6th Airborne Rangers | 747 | 4 | LI | Regular | — |
| The Unknown Ranger | 777 | 1 | MI | Regular + Tactical Awareness | Wildcard; counts as USARF |
| Foxtrot Rangers | 235 | 4 | SK | Regular | — |
| Desperadoes | 752 | 6 | WB | Irregular + Impetuous | — |
| Rosalind "Rosie" Munroe | 990 | 1 | MI | Regular | Wildcard; counts as Grunt |
| Dozers | 256 | 2 | LI | Regular | Grunts max 1 |
| 112, Emergency Service (Motorized) | 1284 | 2 | LI | Regular | Mavericks max 1; counts as Maverick |
| 5th Minutemen | 232 | 5 | HI | Regular | Grunts max 1; USARF required-choice |
| Mavericks | 724 | 5 | MI | Regular + Impetuous | Mavericks |
| Wild Bill | 1482 | 1 | LI | Regular | Grunts max 1; counts as Grunt |
| Hardcases | 236 | 3 | SK | Irregular | — |
| Sāchā, Xenotech Hunters | 1874 | 1 | LI | Irregular | — |
| Marauders, 5307th Ranger Unit | 725 | 5 | MI | Regular | USARF required-choice |
| Devil Dog Teams | 726 | 3 | WB | Irregular + Impetuous | USAMC Duo, FTO profile only |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Intel Spec-Ops | 1915 | Spec-Ops | Grunts Fireteam row, max 1 when Spec-Ops mode is in use |
| Ariadna Team-Ops | 1929 | Team-Ops | No ordinary USAriadna Fireteam row |

## Unit details

### USAriadna Grunts

**ID 230 · AVA TOTAL · MI** — `MOV 10-10 | CC 14 | BS 11 | PH 11 | WIP 12 | ARM 3 | BTS 0 | W 1 | S 2`. Base profile has Immunity (Shock). Source note: **Forward Deployment profiles cannot be part of Fireteams.**

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 10 | 0 | Rifle, Pistol, CC Weapon | Grunts 1–5 |
| 2 | 10 | 0 | Heavy Flamethrower, Light Shotgun, Pistol, CC Weapon | Grunts 1–5 |
| 3 | 21 | 1 | HMG, Pistol, CC Weapon | Grunts 1–5 |
| 5 | 18 | 0 | AP Sniper Rifle, Pistol, CC Weapon; BS Attack (Shock) | Grunts 1–5 |
| 6 | 12 | 0.5 | Heavy Flamethrower, Light Shotgun, Pistol, CC Weapon; Forward Deployment | **No FT** by unit note |
| 7 | 11 | 0 | Rifle, Flash Pulse, Pistol, CC Weapon; Forward Observer | Grunts 1–5 |
| 8 | 12 | 0 | Rifle, Pistol, CC Weapon; MediKit, Paramedic | Grunts 1–5 |
| 9 | 10 | 0 | Rifle, Pistol, CC Weapon; Lieutenant | Grunts 1–5 |
| 12 | 12 | 0 | Rifle, Pistol, CC Weapon; Commlink (+2), Specialist Operative | Grunts 1–5 |

### 112, Emergency Service

**ID 255 · AVA 2 · LI** — `MOV 10-10 | CC 16 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Doctor with MediKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 11 | 0 | **112 FTO**; Light Shotgun, Boarding Pistol, CC Weapon | Wildcard max 1; counts as Grunt |

### Van Zant

**ID 244 · AVA 1 · LI** — `MOV 10-10 | CC 22 | BS 13 | PH 13 | WIP 14 | ARM 2 | BTS 0 | W 1 | S 2`. Parachutist assault character with Tactical Awareness.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 0 | AP Rifle, Chain-colt, AP Heavy Pistol, AP + T2 CC Weapon | — |
| 2 | 35 | 0 | T2 Boarding Shotgun, Chain-colt, AP Heavy Pistol, AP + T2 CC Weapon; profile BS Attack modifier | — |

### Traktor Mul

**ID 257 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 10 | PH 9 | WIP 12 | ARM 2 | BTS 0 | W 1 | S 4`. Baggage artillery/support REM.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 5 | 0 | PARA CC Weapon; Deactivator | — |
| 2 | 9 | 1 | Katyusha MRL, PARA CC Weapon; Guided | — |
| 3 | 14 | 1 | Uragan MRL, PARA CC Weapon; Guided, Total Reaction | — |

### Wardrivers, Mercenary Hackers

**ID 265 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 1 | Boarding Shotgun, Flash Pulse, Cybermine, Pistol, CC Weapon; Hacking Device, Hacker | — |
| 2 | 16 | 1 | Same plus Disco Baller | — |

### Beasthunters Free Guild

**ID 1570 · AVA 1 · SK** — `MOV 10-10 | CC 21 | BS 11 | PH 13 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 9 | 0 | **BEASTHUNTER FTO**; Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CC Weapon | —; no USAriadna chart row |
| 2 | 15 | 0 | Heavy Flamethrower, Tactical Bow, AP Mine, Pistol, DA CC Weapon; Camouflage / Forward Deployment package | — |
| 3 | 15 | 0 | Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CC Weapon; Camouflage / Forward Deployment package | — |
| 7 | 17 | 0 | Heavy Flamethrower, Panzerfaust, AP Mine, Heavy Pistol, DA CC Weapon; Camouflage / Forward Deployment package | — |

### Blackjacks, 10th Heavy Rangers Battalion

**ID 775 · AVA 3 · HI (Hackable)** — Full Power `MOV 10-10 | CC 15 | BS 13 | PH 10 | WIP 13 | ARM 5 | BTS 3 | W 2 | S 5`; Battle Ravaged `MOV 10-10 | CC 14 | BS 13 | PH 9 | WIP 13 | ARM 4 | BTS 0 | W 2 | S 5`. Both states have **Courage and BS Attack (-3)**; Full Power has **Transmutation (1)**. This is Heavy Infantry, **not a TAG**.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2862 | 35 | 1.5 | AP HMG, Chest Mine, Panzerfaust, Heavy Pistol, CC Weapon | Blackjacks 1–3 |
| 2863 | 35 | 1 | T2 Sniper Rifle, Submachine Gun, Chest Mine, Heavy Pistol, CC Weapon; BS Attack (AP) | Blackjacks 1–3 |

### Warcors, War Correspondents

**ID 50 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular Journalist.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CC Weapon; 360º Visor | — |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CC Weapon; Sixth Sense | — |

### 6th Airborne Rangers Regiment

**ID 747 · AVA 4 · LI** — `MOV 10-10 | CC 22 | BS 12 | PH 12 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Parachutist assault troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Submachine Gun, Pistol, AP CC Weapon | — |
| 2 | 31 | 1 | AP Spitfire, Pistol, AP CC Weapon | — |
| 3 | 20 | 0 | Boarding Shotgun, Pistol, AP CC Weapon | — |
| 5 | 20 | 0 | Submachine Gun, Flash Pulse, D-Charges, Pistol, AP CC Weapon; Forward Observer | — |

### The Unknown Ranger

**ID 777 · AVA 1 · MI** — `MOV 15-5 | CC 23 | BS 13 | PH 12 | WIP 13 | ARM 4 | BTS 0 | W 1 | S 2`. Tactical Awareness character and USAriadna Wildcard.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 39 | 0 | Mk12, Chain-colt, Heavy Pistol, T2 CC Weapon | Wildcard max 1; USARF |
| 2 | 42 | 1 | AP Spitfire, Chain-colt, Heavy Pistol, T2 CC Weapon | same |
| 3 | 42 | 0 | Mk12, Chain-colt, Heavy Pistol, T2 CC Weapon; MSV1 | same |
| 4 | 45 | 1 | AP Spitfire, Chain-colt, Heavy Pistol, T2 CC Weapon; MSV1 | same |

### 7th Foxtrot Rangers "Newport"

**ID 235 · AVA 4 · SK** — `MOV 10-10 | CC 14 | BS 11 | PH 13 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Camouflaged Infiltration troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 17 | 0 | Rifle, Shock Mine, Heavy Pistol, CC Weapon | — |
| 2 | 17 | 0 | Boarding Shotgun, Shock Mine, Heavy Pistol, CC Weapon | — |
| 7 | 20 | 0.5 | Sniper Rifle, Shock Mine, Heavy Pistol, CC Weapon | — |
| 8 | 18 | 0 | Rifle, Flash Pulse, Shock Mine, Heavy Pistol, CC Weapon; Forward Observer | — |
| 10 | 18 | 0.5 | Boarding Shotgun, Shock Mine, Heavy Pistol, CC Weapon; Minelayer | — |
| 11 | 17 | 1 | Rifle, Shock Mine, Heavy Pistol, CC Weapon; Lieutenant | — |

### Desperadoes

**ID 752 · AVA 6 · WB** — `MOV 20-10 | CC 21 | BS 11 | PH 13 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 4`. Motorcycle, Irregular, Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2570 | 7 | 0 | Chain Rifle, Smoke Grenade Launcher, Smoke Grenades, Heavy Pistol, AP CC Weapon | — |
| 2571 | 7 | 0 | Chain Rifle, Smoke Grenade Launcher, Smoke Grenades, Assault Pistol, Shock CC Weapon | — |
| 2572 | 9 | 0 | Boarding Shotgun, Smoke Grenade Launcher, Smoke Grenades, Heavy Pistol, AP CC Weapon | — |

### Grunt Intel Rosalind "Rosie" Munroe

**ID 990 · AVA 1 · MI** — `MOV 10-10 | CC 15 | BS 12 | PH 11 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 2`. Courage, Forward Deployment (+4), Immunity (Shock), Specialist Operative, Dogged.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | Light Rocket Launcher, Light Shotgun, D-Charges, Pistol, CC Weapon | Wildcard max 1; Grunt |
| 2 | 23 | 0 | Thunderbolt, D-Charges, Boarding Pistol, CC Weapon | same |
| 3 | 26 | 0 | Light Rocket Launcher, Light Shotgun, D-Charges, Pistol, CC Weapon; **Chain of Command** | same |

### Dozers, Field Engineers

**ID 256 · AVA 2 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Engineer with GizmoKit and Deactivator.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 13 | 0 | Rifle, D-Charges, Pistol, CC Weapon | Grunts max 1 |
| 3 | 14 | 0 | Rifle, Blitzen, D-Charges, Pistol, CC Weapon | Grunts max 1 |
| 4 | 14 | 0 | Rifle, D-Charges, Pistol, CC Weapon; Deployable Cover | Grunts max 1 |
| 5 | 15 | 0 | Rifle, D-Charges, Armed Turret (Rifle), Pistol, CC Weapon | Grunts max 1 |

### 112, Emergency Service (Motorized)

**ID 1284 · AVA 2 · LI** — `MOV 20-10 | CC 16 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 4`. Doctor on Motorcycle with MediKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4761 | 19 | 0 | Light Shotgun, Smoke Grenade Launcher, Smoke Grenades, Boarding Pistol, CC Weapon | Mavericks max 1; counts as Maverick |

### 5th Minutemen "Ohio"

**ID 232 · AVA 5 · HI (Non-Hackable)** — `MOV 15-5 | CC 20 | BS 13 | PH 13 | WIP 12 | ARM 3 | BTS 0 | W 1 | S 2`. Combat Instinct, **BS Attack (+1 Special Die)**, CC Attack (-6), Dodge (+2"), Immunity (IMM-B, Shock), MediKit (PH=15), Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4 | 27 | 1.5 | Missile Launcher, Light Flamethrower (+1B), AP Heavy Pistol, AP CC Weapon | Grunts max 1; USARF required-choice max 5 |
| 6 | 25 | 0 | T2 Rifle, Light Flamethrower (+1B), Flash Pulse, D-Charges, AP Heavy Pistol, AP CC Weapon; **Forward Observer, NCO** | same |
| 7 | 34 | 1.5 | AP HMG, AP Heavy Pistol, AP CC Weapon; **NCO** | same |
| 8 | 36 | 1.5 | AP HMG, AP Heavy Pistol, AP CC Weapon; **Lieutenant (+1 Command Token)** | same |
| 9 | 27 | 0 | T2 Rifle, Light Flamethrower (+1B), Flash Pulse, D-Charges, AP Heavy Pistol, AP CC Weapon; **Lieutenant (+1 Command Token), Forward Observer** | same |

### Mavericks, 9th Motorized Recon Battalion

**ID 724 · AVA 5 · MI** — `MOV 20-10 | CC 18 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 4`. Motorcycle, MSV1, Regular, Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2457 | 26 | 1 | AP Spitfire, Smoke Grenade Launcher, Pistol, AP CC Weapon | Mavericks 1–2 |
| 2458 | 16 | 0 | Boarding Shotgun, Smoke Grenade Launcher, Pistol, AP CC Weapon | Mavericks 1–2 |
| 2459 | 20 | 0.5 | Submachine Gun, Light Rocket Launcher, Smoke Grenade Launcher, Pistol, AP CC Weapon | Mavericks 1–2 |
| 2460 | 17 | 0 | Rifle, Flash Pulse, Smoke Grenade Launcher, Pistol, AP CC Weapon; Forward Observer | Mavericks 1–2 |

### Wild Bill, Legendary Gunslinger

**ID 1482 · AVA 1 · LI** — `MOV 15-5 | CC 15 | BS 13 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 22 | 0 | Contender, MULTI Pistol, CC Weapon | Grunts max 1; counts as Grunt |
| 2 | 24 | 0 | Rifle, MULTI Pistol, CC Weapon; BS Attack (Shock) | Grunts max 1; counts as Grunt |

### Hardcases, 2nd Irregular Frontiersmen Battalion

**ID 236 · AVA 3 · SK** — `MOV 10-10 | CC 15 | BS 11 | PH 13 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular camouflaged/decoy frontier troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 12 | 0 | Tactical Bow, Light Shotgun, Boarding Pistol, CC Weapon | — |
| 2 | 14 | 0 | Tactical Bow, Rifle, Boarding Pistol, CC Weapon | — |

### Sāchā, Xenotech Hunters

**ID 1874 · AVA 1 · LI** — `MOV 10-10 | CC 17 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`. Irregular specialist-style support troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 6 | 0 | Flash Pulse, E/M Grenades, Stun Pistol, CC Weapon | — |
| 2 | 8 | 0 | Flash Pulse, E/M Grenades, Disco Baller, Stun Pistol, CC Weapon | — |

### Marauders, 5307th Ranger Unit

**ID 725 · AVA 5 · MI** — `MOV 10-10 | CC 15 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 2`. Forward-deploying ranger infantry.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Rifle, Heavy Flamethrower, Heavy Pistol, CC Weapon | USARF required-choice max 5 |
| 2 | 28 | 1.5 | AP Spitfire, Heavy Pistol, CC Weapon | same |
| 3 | 18 | 0 | Boarding Shotgun, AP Mine, Heavy Pistol, CC Weapon | same |
| 4 | 30 | 0.5 | Sniper Rifle, Heavy Pistol, CC Weapon; MSV1 | same |
| 5 | 23 | 1.5 | Heavy Rocket Launcher, Heavy Pistol, CC Weapon; MSV1 | same |
| 6 | 21 | 0 | Rifle, Heavy Flamethrower, Heavy Pistol, CC Weapon; MediKit, Paramedic | same |
| 8 | 19 | 0 | Rifle, Heavy Flamethrower, Heavy Pistol, CC Weapon; Lieutenant | same |

### Devil Dog Teams, 2nd Assault Battalion of the USAMC

**ID 726 · AVA 3 · WB** — Devil Dog `MOV 15-10 | CC 23 | BS 11 | PH 16 | WIP 12 | ARM 4 | BTS 3 | W 2 | S 6`; K-9 Antipode `MOV 15-15 | CC 20 | BS 0 | PH 15 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 5`. Irregular, Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Devil Dog: Chain Rifle, Smoke Grenades, AP Heavy Pistol, AP CC Weapon; includes K-9 Antipode | — |
| 2 | 28 | 0 | Devil Dog: Heavy Shotgun, Smoke Grenades, Boarding Pistol, AP CC Weapon; includes K-9 Antipode | — |
| 3 | 22 | 0 | **DEVIL DOG FTO**: Heavy Shotgun, Grenades, Smoke Grenades, Boarding Pistol, AP CC Weapon; no K-9 included | USAMC Duo 1–2 |

## Canonical Fireteam chart

Global USAriadna limits from Army revision `7.26246.158`:

- **Core:** 1
- **Haris:** 1
- **Duo:** unlimited (`256` sentinel in Army data)

### Grunts Fireteams

**Types:** Core, Haris

| Entry | Min | Max | Counts as / restriction |
|---|---:|---:|---|
| GRUNT | 1 | 5 | Forward Deployment Grunt profiles cannot join |
| MINUTEMAN | 0 | 1 | — |
| DOZER | 0 | 1 | — |
| WILD BILL | 0 | 1 | Grunt |
| INTEL | 0 | 1 | Spec-Ops only |

### USARF Fireteams

**Types:** Core, Haris, Duo

The two marked rows are a **required-choice set**. A legal USARF Fireteam must satisfy the Army chart's required foundation using Minutemen and/or Marauders; `required: true` on both alternatives is not interpreted as requiring at least one of each.

| Entry | Min | Max | Required-choice | Counts as |
|---|---:|---:|---|---|
| MINUTEMAN | 0 | 5 | yes | USARF |
| MARAUDER | 0 | 5 | yes | USARF |

### Blackjack Fireteams

**Types:** Haris, Duo

| Entry | Min | Max | Note |
|---|---:|---:|---|
| BLACKJACK | 1 | 3 | — |

### Mavericks Fireteams

**Types:** Haris, Duo

| Entry | Min | Max | Counts as / note |
|---|---:|---:|---|
| MAVERICK | 1 | 2 | — |
| 112 MOTORIZED | 0 | 1 | Maverick |

### USAMC Fireteams

**Types:** Duo

| Entry | Min | Max | Profile restriction |
|---|---:|---:|---|
| DEVIL DOG | 1 | 2 | `DEVIL DOG FTO` profile only |

### Wildcards

| Entry | Max | Counts as / note |
|---|---:|---|
| 112 FTO | 1 | Grunt |
| ROSIE | 1 | Grunt |
| UNKNOWN RANGER | 1 | USARF |

Wildcards may join otherwise eligible Fireteams subject to the normal sectorial limits and profile restrictions above.

## Fireteam composition audit — N5.3 (19 November 2026)

**Scope:** Derived, profile-specific standard-roster examples only. The **preceding canonical Fireteam chart** remains authoritative if these illustrative tactical builds disagree with it. Profile/option numbers and individual points/SWC use the pinned Army `7.26246.158` data already transcribed in this file. Each example is an individual package, **not** a simultaneous 300-point army; obey overall AVA, 15-trooper, SWC, Combat Group and Fireteam limits when combining them. Reinforcement links use a **separate chart** and are not mixed in. An attached Peripheral, Ancillary or escape-system model is **not** an extra Fireteam member.

**How to read FT level:** N5/5.3 Fireteam Level follows the largest set of troopers with an identical Unit name or the *same applicable* `Counts as` name; it is **not automatically the physical size** of the Fireteam. Level 1 = joint activation, level 2 = BS Attack (+1 SD), level 3 = +3 Discover/+1 Dodge, level 4 = +1 BS, level 5 = Sixth Sense (bonuses cumulative). See [Fireteam Bonuses](../../rules/6_Command%20and%20Fireteams/Fireteam_Bonuses.md) and the [official wiki](https://infinitythewiki.com/Fireteam_Bonuses). The level shown assumes the **entire starting composition is present**; recalculate after members leave.

**Limits:** one Core, one Haris, unlimited Duos. Grunts family is **Core/Haris only** and needs a native Grunt; USARF is Core/Haris/Duo and needs a Minuteman and/or Marauder; Blackjack is Haris/Duo with a Blackjack anchor; Mavericks is Haris/Duo with a native Maverick; USAMC is Duo only with **Devil Dog FTO** (the 22-point option **without** a K-9 Peripheral). 112 FTO/Rosie/Wild Bill count as Grunts, and Unknown Ranger counts as USARF. **Forward Deployment Grunt** option 6 cannot link. Historic report #059 Grunt Duos are not legal under this pinned chart.

| Size / type / family | Exact profiles (points/SWC **per member**) | Total pts / SWC | FT level | Best-use assessment and evidence |
|---|---|---:|---:|---|
| 2 · Duo · Mavericks | Maverick opt 2457 — AP Spitfire **26/1**; 112 Motorized opt 4761 — Doctor/Smoke **19/0** | **45 / 1** | **L2** | **Best mobile value Duo.** Recorded in [#223](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md#L73); 112 Motorized counts as Maverick. |
| 2 · Duo · Blackjack | Blackjack opt 2862 — AP HMG **35/1.5**; Blackjack opt 2863 — T2 Sniper Rifle **35/1** | **70 / 2.5** | **L2** | **Best heavy ARO Duo candidate.** This two-Blackjack structure was played in [#124](../../notes/battle-reports/121-130-n5-battle-report-tactical-analysis.md#L121). |
| 2 · Duo · USARF | Minuteman opt 6 — NCO/FO T2 Rifle **25/0**; Marauder opt 6 — Paramedic **21/0** | **46 / 0** | **L2** | **Efficient scoring duo candidate** analogous to the Minuteman/Marauder Duo in [#223](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md#L73); exact two loadouts here not fully sourced to that report. |
| 2 · Duo · USAMC | Devil Dog FTO opt 3 — Heavy Shotgun (no K-9) **22/0**; Devil Dog FTO opt 3 — Heavy Shotgun (no K-9) **22/0** | **44 / 0** | **L2** | **FTO-only legal formation, situational.** Non-FTO Devil Dogs with K-9 Peripherals cannot be linked; no separate K-9 bodies count. |
| 3 · Haris · Grunts | Grunt opt 5 — AP Sniper **18/0**; Grunt opt 7 — Forward Observer **11/0**; Rosie opt 1 — Light Rocket Launcher **21/0** | **50 / 0** | **L3** | **Best inexpensive defensive Haris candidate.** Rosie counts as Grunt; her Forward Deployment is not the banned Grunt FD option. |
| 3 · Haris · USARF | Minuteman opt 7 — NCO AP HMG **34/1.5**; Marauder opt 4 — MSV1 Sniper **30/0.5**; Unknown Ranger opt 1 — Mk12 **39/0** | **103 / 2** | **L3** | **Premium attack Haris.** Similar *roles* to the recorded [#203](../../notes/battle-reports/201-210-n5-battle-report-tactical-analysis.md#L94) USARF Haris; exact profiles are a current-pin alternative. |
| 3 · Haris · Mavericks | Maverick opt 2457 — AP Spitfire **26/1**; Maverick opt 2460 — Forward Observer **17/0**; 112 Motorized opt 4761 — Doctor **19/0** | **62 / 1** | **L3** | **Fast mission Haris candidate.** Motorized 112 counts as Maverick; do not accidentally add a third native Maverick (max 2). |
| 4 · Core · Grunts | Grunt opt 5 — AP Sniper **18/0**; Grunt opt 1 — Rifle **10/0**; Grunt opt 8 — Paramedic **12/0**; Rosie opt 1 — Light Rocket Launcher **21/0** | **61 / 0** | **L4** | **Best cost-conscious four-body Core.** Mirrors the played formation in [#057](../../notes/battle-reports/051-060-n5-battle-report-tactical-analysis.md#L215), with exact N5.3 options. |
| 5 · Core · Grunts | Grunt opt 5 — AP Sniper **18/0**; Grunt opt 7 — Forward Observer **11/0**; Grunt opt 1 — Rifle **10/0**; Grunt opt 8 — Paramedic **12/0**; Rosie opt 1 — Light Rocket Launcher **21/0** | **72 / 0** | **L5** | **Best cheap level-five Core candidate.** [#203](../../notes/battle-reports/201-210-n5-battle-report-tactical-analysis.md#L94) played a different five-body Grunt-family Core including a Minuteman (therefore not automatically level five); this is a legal all-Grunt-equivalent reconstruction. |
| 5 · Core · USARF | Minuteman opt 6 — NCO/FO T2 Rifle **25/0**; Minuteman opt 7 — NCO AP HMG **34/1.5**; Marauder opt 4 — MSV1 Sniper **30/0.5**; Marauder opt 6 — Paramedic **21/0**; Unknown Ranger opt 1 — Mk12 **39/0** | **149 / 2** | **L5** | **Elite five-body Core candidate.** [#183](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md#L83) records the same mixed-USARF construction but different specific loadouts; all five count as USARF. High points concentration. |

**Evidence key:** `played / reported` refers to a linked formation **explicitly identified** in a numbered N5 battle report; when the report does not specify every loadout, this table identifies the example as an **N5.3 reconstruction** rather than an exact recovered export. Podcast/video discussion is a **player recommendation**, not proof that an identical composition was deployed. Other entries are **chart-legal test constructions**, not tested wins. Source preference: pinned [Army data and Fireteam chart in this file](#canonical-fireteam-chart), [official Fireteams Chart](https://infinitythewiki.com/Fireteams_Chart), then [report index](../../notes/battle-reports/n5-battle-reports-and-tournament-reports.md) and linked media. No claim is made that a package is optimal on every mission or terrain layout.

## Reverse Fireteam access index

| Troop / profile | Fireteam families | Notes |
|---|---|---|
| USAriadna Grunt | Grunts | Native 1–5; Forward Deployment profile excluded by source note |
| Minuteman | Grunts; USARF | Max 1 in Grunts; required-choice, max 5 in USARF |
| Dozer | Grunts | Max 1 |
| Wild Bill | Grunts | Max 1; counts as Grunt |
| Intel Spec-Ops | Grunts | Max 1; optional Spec-Ops mode only |
| Marauder | USARF | Required-choice; max 5; counts as USARF |
| Blackjack | Blackjacks | Native 1–3 |
| Maverick | Mavericks | Native 1–2 |
| 112 Motorized | Mavericks | Max 1; counts as Maverick |
| Devil Dog FTO | USAMC | FTO profile only; native 1–2 Duo row |
| 112 FTO | Wildcard | Max 1; Grunt |
| Rosie Munroe | Wildcard | Max 1; Grunt |
| Unknown Ranger | Wildcard | Max 1; USARF |

All standard roster units not listed in this reverse index have no Fireteam access in the pinned standard USAriadna chart.

## Reinforcement Fireteams — L'Équipe Argent

Linked Reinforcement army: **L'Équipe Argent (Army ID 399)**, source revision `7.26246.158`.

These rows are intentionally separate from the standard USAriadna chart. Reinforcement Fireteam limits in the pinned source are **Core 1; Haris 1; Duo 1**.

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

- **2026-10-22 profile-skill transcription repair:** restored Minutemen BS Attack (+1SD), NCO, Lieutenant (+1 Command Token), and related loadout skills, Blackjack BS Attack (-3) and Transmutation, and Rosie Chain of Command/ordinary skills omitted in the shortened original summary. Cross-checked against [Corvus Belli's October 2025 Army update](https://infinityuniverse.com/en/news/army-update-october-2025-part2) and the current N5 [Minuteman](https://human-sphere.com/Minuteman), [Blackjack](https://human-sphere.com/Blackjack), and [Rosie](https://human-sphere.com/Rosalind_Munroe) profile reproductions. Original roster costs, chart, pinned Army revision, and verification provenance preserved.

- Standard roster count reconciled to **22** ordinary USAriadna entries after excluding `Intel Spec-Ops`, `Ariadna Team-Ops`, and generic `merc-*` catalog entries with an empty faction list.
- Army ID `304` is explicitly marked `discontinued: true` in the pinned N5 Army metadata; this reference nevertheless uses the complete current N5 roster and Fireteam data shipped for that Army ID.
- Every standard `fireteamChart` row from Army revision `7.26246.158` is represented, including the Minuteman/Marauder USARF required-choice set and all profile-sensitive joins.
- Fireteam limits are preserved exactly: Core 1, Haris 1, Duo unlimited in USAriadna.
- The Grunt Forward Deployment restriction is preserved from the unit-level Army note rather than inferred from the Fireteam chart alone.
- `DEVIL DOG FTO` is kept distinct from the ordinary Devil Dog + K-9 team profiles.
- `BEASTHUNTER FTO` is not granted Fireteam access because there is no Beasthunter entry in the current USAriadna Fireteam chart.
- The linked Reinforcement army resolves to **L'Équipe Argent (399)** and its chart is preserved separately.
- Main and Reinforcement Wildcards are not merged.
- Source data and Fireteam normalization were rechecked on **2026-10-15** against the pinned Army snapshot and InfinityDB commit listed in the front matter.

**Tactical and purchasing analysis:** [USAriadna Ranger Force faction notes](../../notes/factions/usariadna.md). The factual roster, Fireteams and validation above remain authoritative.
