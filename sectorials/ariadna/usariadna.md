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

## Hacker and KHD tactical cross-reference (2026-10-23)

**Wardriver HD14/1 SWC** adds ordinary anti-HI/TAG **Carbonite/Oblivion/Spotlight**, but no premium anti-Hacker KHD/HD+ toolkit or automatic long-range Repeater access. **Why:** USAriadna normally wins through efficient shooting, mines/Camo, and several nonhackable infantry threats. Use the Wardriver as deliberate *counter-tech* for an enemy TAG/HI bottleneck or hacking scenario, not because every army needs a Hacker. Keeping SWC for conventional guns is usually more reliable when there is no meaningful hackable target.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

For cross-faction **apex** and **points-value** rankings, the Order types, situational counterexamples and transcript-backed disagreements, see [Cheerleaders and Order Generators — N5.3](../../notes/list-building/cheerleaders-and-order-generators.md). Roster profiles/AVA/Fireteam legality above take precedence.

- **USAriadna Grunts**: line infantry Regular Orders with defensive utility and Fireteam applications, rather than 7pt Flashbot economics

**List-building test:** count *transferable* Regular Orders by Combat Group after deployment; include required link members/command enablers, physical DZ footprint, and the unit's actual ARO/mission contribution. Do not treat Irregular, Tactical, Lieutenant or Peripheral activations as interchangeable generic Orders.


## ARO apex/value cross-reference (2026-10-23)

See [ARO units: N5.3 apex/value tiers, hidden-versus-visible and deployment/matchups](../../notes/list-building/aro-units-apex-and-value.md). The **current profile details here** control exact cost/SWC, Training and Fireteam eligibility; do not import another faction's link or specialist upgrades.

- **Marauder MSV1 HRL** — strong one-wound visor template; cover midfield approach, avoid plain shootout with premium active gun
- **Minuteman ML (+1SD)** — powerful linked long-lane reactive spike in USAriadna; one wound makes reliability/backup mandatory
- **Blackjack T2 Sniper** — 2W/ARM and BS Attack(-3) multi-role long-lane, but hacking and transmutation limitations matter
- **Grunt HFT / 0SWC sniper** — cheap S2 short-corner or modest rear gun; prioritize defending objectives and support
- **Traktor Mul support** — rare Ariadna cheap reload/guided/total-reaction choices; only buy a real Guided program if FO route is viable

**Choose by circumstance:** a hard long gun matters only when the opponent must cross its arc; cheaper mines, Camo markers, templates, Flash, DTWs and hacking force movement or risk without committing an entire attack plan. Budget a second layer and preserved counterattack, check pie-slicing, hidden Order cost, anti-visual bypass and repair routes.

## Airborne / enemy-DZ attack profile choices (2026-10-23)

**Van Zant33–35/0 (Parachutist(DZ), TA, Dogged)** is the premier reliable enemy-edge support/LT hunter: choose AP Rifle vs T2 BSG according to exposed soft targets versus armor. **6th Airborne Ranger19 SMG/20 BSG/20 FO** is cheaper *ordinary* Parachutist, **cannot directly enter enemy DZ** and is better for unguarded flank/late scoring. The extra 13–16pts to Van Zant buys direct DZ access and a personal extra Tactical Order, not an unconditional kill. Cover the edge with AROs if facing opposing AD.

[Cross-game N5.3 airborne and DZ-attack apex/value tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **Pinned profiles and the canonical Fireteam chart above govern legality.**

## Warbands and inexpensive trading roles — N5.3

**Desperado Chain Rifle+Smoke GL7/0** is among the best **fast 20-10 Irregular/Impetuous** trades: force a gunner's Dodge or template exchange, lay lateral smoke for a forward Specialist or threaten opposing cheap Orders. **Boarding Shotgun9/0** only if actual quality shooting/short-range target exists. **No standard USARF Galwegian5, Morlock6 or Dāturazi14 import.** **Van Zant33–35/0** has backline DZ Parachutist + TA and plays a different premium attack vector; use 7pt Desperado as smoke/screen instead of risking Van Zant for one cheap kill. Protect the on-table LT/CoC; this sectorial's Fireteam chart remains authoritative.

[Cross-game warband/cheap-trader apex and value tiers, targets and command packages](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). Profile-specific sectorial legality/Fireteams above control all selections.

## N5.3 midfield area denial / speed bumps (tactical synthesis)

**Foxtrot Boarding Shotgun + Shock Mine Minelayer 18/.5** is the inexpensive Regular Camo/Infiltration turn-zero obstacle. **Foxtrot FO 18/0** scores instead and does not deploy a mine at setup; Hardcase 12/0 is cheap Irregular Camo/Decoy and Beasthunter 15/0 provides close-range template and AP mine pressure, but neither duplicates Foxtrot Minelayer. Opposing concern: buying too many disposable midfield blockers can weaken USARF's counterattack and objective specialists.

[Whole-game area denial tiers and sources](../../notes/list-building/midfield-area-denial-and-speed-bumps-apex-value.md).

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Warband/low-cost LI casualties** often aren't worth 3–4 Orders of Doctor travel unless they are the last scoring Specialist. Use a roster-legal **112-style Doctor/Engineer** only when it supports an expensive ARO, vehicle or objective specialist; **No-Cube targets** have no ordinary Cube-based token reroll. Consider **GizmoKit PH and Repair WIP** separately; the 2–3pt Servant is an Order-efficiency investment, not an extra independent activation. [Doctor/Engineer recovery odds and tier guide](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## N5.3 DZ defense / anti-alpha-strike tactical choices

**Warcor 360º3/0** is cheap Irregular protection versus Van Zant/Hellcat-style reverse attacks (also relevant in a mirror match); **Foxtrot BSG+Shock Mine Minelayer 18/.5** secures an infiltrated *outer* crossing route while **Foxtrot FO18/0** scores without a starting mine. **Hardcase** cheap Camo/Decoy and **Beasthunter HFT/Panzerfaust** force close corners, but neither means a free initial deployed mine without the printed Minelayer skill. **Counter:** defensive Irregular saturation cannot replace a Regular attack group, and static mine paths cannot guard every DZ-edge/rooftop Combat Jump entry.

[Whole-game DZ defense value/apex and anti-IMP matchups](../../notes/list-building/dz-defenders-alpha-strike-and-impersonation-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Devil Dog + K-9 Antipode23** is USARF's key *two-body close assault*: 15-10 Devil Dog CC23/PH16 with smoke/chain rifle and 15-15 Antipode can create contact pressure or multiple-body CC, if geometry and controller rules permit; it isn't a cheap lone MA5 specialist. **Van Zant33–35** uses Parachutist enemy-DZ entry and AP+T2 CC as a *secondary* finisher after the correct gun angle. **Desperado7** has fast 20-10 Smoke/chain rifle for cheap trade but S4 moto and Irregular orders make isolated assassination unreliable; Foxtrot Camo/Infiltration CC14 is not a duelist. [Close-combat apex/value, positioning and counter-CC](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**USARF** relies on **Blackjack/Grunt/Marauder rifle, rockets and specialist screens**, plus **Desperado7 Smoke motorcycle** to gain a usable side angle; **Van Zant33/35** can flank an armored target from DZ edge but AP+T2 CC only works if actually reaching contact. **Devil Dog23 + K-9** can tie up a TAG in Engaged, but template guard and S6 constraints matter. **Standard rifles alone** are poor against ARM8+ in cover: choose a roster-legal hard ARO/anti-armor gun and avoid treating a fast smoke carrier as a guaranteed kill. [Non-hacking armor-killer value rankings and tactical matchups](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**5th Minuteman FO+NCO25/0** is **Non-Hackable** (not automatic hacker target), BS Attack(+1SD), Immunity(Shock, IMM-B), T2 Rifle+LFT and direct specialist eligibility: superb box-guard value for a covered area. **Marauder Paramedic21/0** ARM3/heavy flamer on a forward-deployed support role is a second cheaper carrier. **Unknown Ranger Specialist Operative+Tactical Awareness39/0** (Mimetism-3, W1+NWI, ARM4, immune to Shock) carries efficiently with dedicated Order and CC counter, compared with a more expensive heavy team. **Blackjack35/1–1.5** full W2/ARM5, battle-ravaged W2/ARM4, Transmutation, is **Hackable and not a Supplies Specialist**; useful *zone VP/support* gun and remains worth defending after transformation. **Opposing:** a 25pt Minuteman plus Marauder can cover two different scoring zones at lower concentration than one Blackjack+Unknown Ranger; prepare for templates rather than relying on Fireteam long ARO only.

[Cross-game objective holder and zone-domination apex/value tiers, scenario rules, and opposing transcript reviews](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Exact profiles/Fireteams above are authoritative.

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Wardriver Disco Baller16/1** is the scarce low-cost **enemy-MSV/Marksmanship blind** in an otherwise smoke-heavy force; **regular 8pt Disco-bearing utility profile** (if its exact roster option is selected) can create another emergency screen. **Desperado Smoke, Foxtrot/Grunt cover and close templates** often solve an expensive Mimetism/visor ARO by **avoiding it** rather than beating it in a BS contest. Against Camo, use cheap Discover probes, deployment mines and protected routes; there is no justification to rank every Camo marker as a premium kill target. **Counter:** ordinary Smoke doesn't block MSV2, and Disco's two-use/placement+follow-up Orders can exceed the value of simply scoring elsewhere.

[Full anti-tech N5.3 apex/value, exact mechanics, matchup selection and opposing transcripts](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## Mission performance — battle-report evidence (2026-11-01)

| Mission(s) | Tested composition / scoring mechanism | Evidence |
|---|---|---|
| **Hunting Party / defensive ground** | Blackjack duo plus Grunt sniper/Warcor and Foxtrot/Maverick/Beast Hunter elements maintained durable reactive zones vs O-12. | [#124](../../notes/battle-reports/121-130-n5-battle-report-tactical-analysis.md) |
| **Corporate Appropriation defense** | Foxtrot FO/Maverick/Minuteman/Van Zant can contest prototype and counterstrike, but #223's rear Van Zant attack failed to destroy the object. | [#223](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) |
| **Acquisition / Superiority lane fighting** | Marauder/Minuteman/Grunt ranged shells with cheap forward specialists have a plausible zone plan, with mixed outcomes. | [#057](../../notes/battle-reports/051-060-n5-battle-report-tactical-analysis.md), [#059](../../notes/battle-reports/051-060-n5-battle-report-tactical-analysis.md) |

**Limits:** Limited consistent scoring evidence; don't rank USARF above broad-area competitors based on this sample. Game-era qualitative evidence, not a win-rate or current Fireteam claim. [Full mission evidence audit](../../notes/battle-reports/cross-report-mission-performance-by-sectorial.md).

## Counterplay — observed N5 battle-report responses (2026-11-02)

| Threat / target | Observed response and limitation | Battle reports |
|---|---|---|
| **Against protected gunlines** | Blackjack duo/Grunt/Minuteman and cheap Foxtrot/Maverick screening absorbed O-12 pressure in Hunting Party; only a sustainable mission path turns resilience into points. | [#124](../../notes/battle-reports/121-130-n5-battle-report-tactical-analysis.md) |
| **TAG already in mission zone** | Varuna's hidden Cutter scored Area of Interest while Mavericks/smoke and Unknown Ranger/Minutemen failed to dislodge scoring weight; threaten a different zone or exact carrier. | [#203](../../notes/battle-reports/201-210-n5-battle-report-tactical-analysis.md) |
| **Airborne assassin counterexample** | Van Zant shot Voronin but mine/template and cover screens prevented finishing the Corporate target; one rear entry is not automatic success. | [#223](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) |

**Limit:** Sparse examples of direct anti-hacking or anti-Impersonation success; no USARF-wide dominance is inferred. These are historical qualitative interactions, not present N5.3 unit, Fireteam, or win-rate claims. [Full cross-report counterplay analysis](../../notes/battle-reports/n5-cross-report-counterplay-tags-hi-hacking-camo-impersonators-fireteams.md).

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

### 2. USAriadna Ranger Force

[Current roster / Fireteams](usariadna.md) · [Detailed guide](../../notes/factions/usariadna.md)

**Near-must / strong defaults**

| Piece | Why; limit | Evidence |
|---|---|---|
| **Foxtrot FO 18 / Minelayer 18 (0.5 SWC)** | On-table **Regular** camouflaged infiltrating mission piece or mine/marker roadblock. Forms the repeatable midfield scoring/control shell; not a primary gunfighter. | [Swiss Miss Gaming — N5 USARF Tier List (post-Oct-2025)](https://www.youtube.com/watch?v=AboAGci9_9A) praises specialist/Minelayer; [Robert Shepherd USARF](https://www.youtube.com/watch?v=mqNiL2ziIkU) supports the role. **Repeat + explicit praise.** |
| **1–2 Desperadoes (7pt base)** | Very cheap 8-4 smoke + Chain Rifle/trading/CC. Swiss Miss specifically says one or two belong in **most** builds. Irregular/Impetuous and S4 footprint still cost tactical flexibility. | [Swiss Miss USARF](https://www.youtube.com/watch?v=AboAGci9_9A), **explicit**; [TA USARF](https://open.spotify.com/episode/4wIT3UwMB9LldCtHdfLU6k) uses them in example lists. |

**Go-to**

| Piece | Why; trade-off | Evidence |
|---|---|---|
| **Unknown Ranger MSV1 Mk12 / AP Spitfire** | Tactical Awareness, Mimetism, NWI and Specialist Operative compress a strong shooter and scoring role. Expensive; MSV/visibility counter-tech can reduce his advantage. | [Swiss Miss USARF](https://www.youtube.com/watch?v=AboAGci9_9A) rates S tier; [TA USARF](https://open.spotify.com/episode/4wIT3UwMB9LldCtHdfLU6k) includes UR/Minuteman combinations. |
| **Minuteman FO/NCO T2; AP HMG / ML** | Post-Oct-2025 BS Attack (+1 Special Die), 6-2 move and NCO/specialist utility greatly improve old Minutemen. 1-Wound HI does not absorb extended fire. | Swiss Miss **explicit post-rework reassessment**; [Shepherd May 2025](https://www.youtube.com/watch?v=mqNiL2ziIkU) skepticism is **pre-update**. |
| **Blackjack AP HMG / T2 Sniper** | Two effective Wounds, threatening BS13/-3 shooting and efficient possible small Haris (e.g. Rosie + 112 FTO). **Hackable HI, not a TAG**; weaker after Transmutation. | Swiss Miss enthusiastic; [USARF guide](../../notes/factions/usariadna.md) documents later Loss of Lieutenant disagreement about only mid-tier value. |
| **Marauder MSV1 HRL / Paramedic** | Forward-deployed anti-Mimetism templates and cheap attack-specialist link support, but fragile 1-Wound attackers. | Swiss Miss; Shepherd USARF. |
| **Devil Dog + K-9** | Smoke, Sensor via K-9, fast CC and a disposable second attack body at 23pt baseline. **FTO is a different solo profile without K-9**. | [TA USARF](https://open.spotify.com/episode/4wIT3UwMB9LldCtHdfLU6k) explicitly *did not bring* Devil Dogs in three early-N5 lists; post-update Swiss Miss and the USARF guide rate them better. **Contested due to chronology.** |
| **Maverick AP Spitfire / FO** | Regular MSV1 bikes with fast attack/objective reach and Smoke GL. Limited Cover and exposed motorcycle lanes prevent universal use. | Swiss Miss compares 26pt AP Spitfire to budget Unknown Ranger; Shepherd is more cautious. |
| **Van Zant** | DZ-entry Parachutist and Tactical Awareness pressure enemy support troops, forcing defensive deployment. Not a substitute for Turn-1 on-table control. | Swiss Miss rates very highly; TA USARF hosts debate his reliability and threat value. |
| **Grunts LT / cheap specialists; Traktor Mul 5pt** | Preserve points and Regular Orders for the army's several 25–45pt pieces; avoid a full slow Grunt Core without a specific gun/support purpose. | Swiss Miss, Shepherd and TA USARF. |
| **Rosie CoC / 112 FTO** | Useful as inexpensive team composition and command resilience *when* a Blackjack, Minuteman or aggressive LT justifies them. Rosie CoC is not automatically required. | Swiss Miss / Shepherd; current chart. |

**Strong/conditional avoids**

| Profile or construction | Negative comparison and caveat | Recording |
|---|---|---|
| **Wild Bill as routine Grunt-team filler** | High delivery cost for short-range multi-pistol shooting; fragile and faster than his likely Fireteam. **Strong avoid unless specifically constructing a close-quarters plan**, not literally unusable. | [Swiss Miss USARF](https://www.youtube.com/watch?v=AboAGci9_9A) directly calls him a difficult piece to justify. |
| **Grunt AP Sniper as sole ARO anchor** | Cheap 0-SWC rifle is not comparable to the Blackjack, Marauder HRL or Minuteman ML if genuinely elite reactive fire is required. Remains workable *budget* backup. | Swiss Miss explicitly not impressed as main ARO; **conditional**, not a ban on Grunts. |
| **Massed Hardcases when Regular midfield Orders needed** | Many Irregular bodies compete for 15 slots, while Foxtrots and cheap Beasthunter utility cover crucial jobs. Not strictly outclassed if Decoy/camo distraction is the actual need. | Swiss Miss + Shepherd; **reasoned**. |

**Chronology warning:** TA January 2025 / Shepherd May 2025 preceded substantial **October 2025** changes to Minutemen, Blackjacks, Devil Dogs, Van Zant and Fireteams. Prefer post-update Swiss Miss for opinions about today's profiles.

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

#### 2. USAriadna Ranger Force (USARF)

| Weak, niche or redundant purchase | Evidence and meaningful exception | Miniature decision |
|---|---|---|
| **Wild Bill** | **Strongest direct full-model deferral — [Swiss Miss post-rework USARF](https://www.youtube.com/watch?v=AboAGci9_9A):** expensive short-range pistol delivery, fragile and awkward beside slow Grunt link partners. A dedicated close-range rush/room-clearing plan is the exception. | **Skip by default / proxy as a distinctive S2 gunslinger** if the specific pistol team is wanted. Do not buy only to complete the Grunt chart. |
| **Grunt AP Sniper as the only serious ARO** | **Direct profile critique — Swiss Miss:** a cheap 0-SWC budget backup cannot substitute for a **Blackjack**, **Marauder HRL** or **Minuteman ML** against hard targets. Basic Grunt LT/link/utility remains useful. | **Avoid just this gun-as-primary-ARO plan**, not Grunt miniatures. Proxy the occasional sniper profile with an otherwise unused line infantry sculpt. |
| **Massed Hardcases** | **Direct/reasoned:** Irregular camo distractions consume 15-model slots, while **Foxtrot** specialists/minelayers supply Regular Orders and can do objectives. Hardcase Decoy/ambush still offers a different cheap shell. | **Proxy extra copies**, especially before trying all AVA3; a single clearly declared Hardcase may be worth it for a specific Decoy/trading plan. |
| **6th Airborne Ranger as a generic Van Zant imitation** | **Recorded comparison:** ordinary AD FO20 can score cheaply, but a gun bought only for the rear-DZ raid often loses its distinctive advantage to **Van Zant's Parachutist (DZ), TacAware and threat footprint**. | **Proxy first** for a second/third gun-carrying AD model. **Do not blacklist** a cheap FO mission specialist or claim it has Van Zant's entry ability. |
| **Wardriver without a hacking/Disco task; Traktor Guided without FO targets** | **Conditional inference:** USARF's best practical tools are smoke, nonhackable gunfighting and Foxtrot missions; standalone mediocre infowar or low-BS Guided artillery doesn't automatically repay SWC and Orders. | **Proxy a Wardriver** with an unused S2 technician; **use the same Traktor chassis** for occasional artillery. The **5pt Baggage/Order** remains a valuable buy. |
| **Sāchā or other occasional low-price Irregular filler** | **Unrated by cited USARF reviewers, not proven poor:** 6pt specialty/forward deployment competes for slots with Desperadoes, Foxtrot and Warcor; price alone does not make it universal. | **Proxy first** with spare suitably based Ariadna infantry rather than buy a dedicated character for a rare filling problem. |
| **Devil Dog FTO / K-9 team; extra Maverick or Desperado bikes** | **Contested / silhouette caveat:** post-Oct-2025 reviews like Devil Dogs far more than earlier TA; **FTO is a SOLO profile without K-9**, while normal Devil Dog has a separately represented dog. Bikes bring genuine MSV1/Smoke/FO or cheap trading but have limited cover. | **Proxy/test the expensive *second* dog team or extra motorcycle**, not the first broadly useful fast piece. **Don't buy a K-9 solely for an FTO profile** or treat an S4 bike/S6 dog as S2 infantry. |
| **Several premium Blackjacks, Minutemen and Marauder gun sculpts for the same fire lane** | **Inference:** all three are legitimate post-update attackers, but buying the entire AVA worth of overlapping gunfighters may leave Foxtrot/button coverage thin. Pre-Oct-2025 “bad Minuteman/Blackjack” views are obsolete. | **Buy/proxy only enough for tested legal teams**; first good AP HMG/HRL and useful specialist are **not** “avoid” recommendations. |

**Evidence:** [Swiss Miss USARF](https://www.youtube.com/watch?v=AboAGci9_9A) (post-rework), [Shepherd USARF](https://www.youtube.com/watch?v=mqNiL2ziIkU) (pre-rework), [Tactical Awareness USARF](https://open.spotify.com/episode/4wIT3UwMB9LldCtHdfLU6k), [USARF guide](../../notes/factions/usariadna.md). **Keep** the first Foxtrot, one/two useful Desperadoes, and deliberate Unknown Ranger/Minuteman/Marauder/Blackjack gun plans.

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
