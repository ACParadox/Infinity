---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 302
sectorial_slug: caledonian-highlander-army
sectorial_name: Caledonian Highlander Army
parent_faction: Ariadna
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Caledonian Highlander Army roster, standard loadouts, canonical Fireteam chart, reverse Fireteam index, and the distinct L'Équipe Argent Reinforcement Fireteam chart. Intel Spec-Ops and Ariadna Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# Caledonian Highlander Army

## Overview and provenance

Repository-native reference for **Caledonian Highlander Army (CHA / Caledonia)** roster, profiles, points/SWC, AVA, and Fireteam access.

Sources used:

- Army-derived Caledonia source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `d4329bb596ffea5d568eb2435f74366c305a7630`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **23-unit standard Caledonia roster** and the complete standard Caledonia `fireteamChart` in the pinned Army source.
- Army metadata currently marks **Caledonian Highlander Army as discontinued**, but a complete N5 roster and Fireteam chart remain present in the current Army data. `status: current` above refers to this reference being current with the pinned N5 data, not to the sectorial's discontinued flag.
- Soldier of Fortune / generic `merc-*` catalog entries whose source faction list is empty are excluded from the base roster.
- `Armand 'Le Muet'` and `McMurrough` are retained because their ordinary Caledonia unit entries explicitly include faction ID `302`; they are not being imported from the generic empty-faction mercenary catalog.
- `Intel Spec-Ops` and `Ariadna Team-Ops` are optional game-mode content and are listed separately.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name by itself.
- Parenthetical Army-chart comments are treated as Counts-as / equivalence labels, not as join-scope restrictions.
- The structured `required: true` Mormaer and Highlander Grey rows in Heavy Caledonians are preserved as a required-choice set; this file does not reinterpret them as requiring both troop types simultaneously.
- Profile restrictions are preserved: Beasthunters join Volunteer teams only through `BEASTHUNTER FTO`; Scots Guards join Fireteams only through `SCOT GUARD FTO`; the standard `112 FTO` profile joins Volunteer teams.
- The Galwegians chart refers to Denma Connolly using the legacy/chart slug `denma-connolly-caledonian-zellenkrieger`, while the current unit source slug is `denma-connolly`; both resolve to the same troop entry.
- Linked Reinforcement army ID: **399**, **L'Équipe Argent**. Its Fireteam chart is recorded separately below and is not merged into the main Caledonia chart.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Caledonian Highlander Army (CHA) |
| Parent faction | Ariadna |
| Army ID | 302 |
| Army slug | `caledonian-highlander-army` |
| Army metadata status | Discontinued |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 23 |
| Optional-mode units | Intel Spec-Ops; Ariadna Team-Ops |
| Reinforcement roster | L'Équipe Argent, Army ID `399` |
| Fireteam limits | Core 1; Haris 1; Duo unlimited |
| Fireteam chart | yes |

## Roster index

| Unit | ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| Dozers, Field Engineers | 256 | 2 | LI | Regular | — |
| Cadin "FirstStrike" Donn | 1525 | 1 | WB | Regular | Wildcard; counts as Wulver |
| Traktor Mul | 257 | 2 | REM | Regular | — |
| 1st Highlanders S.A.S. | 237 | 4 | SK | Regular | — |
| 45th Highlanders Rifles 'Galwegian' | 239 | TOTAL | WB | Irregular + Impetuous | Galwegians |
| 2nd Irregular Cameronians Reg. | 254 | 3 | WB | Irregular + Impetuous | — |
| Beasthunters Free Guild | 1570 | 1 | SK | Irregular | Volunteers, FTO profile only |
| Caledonian Volunteers Corps | 245 | TOTAL | LI | Regular | Volunteers |
| 112, Emergency Service (Motorized) | 1284 | 2 | LI | Regular | — |
| William Wallace | 259 | 1 | WB | Regular | Wildcard; counts as Highlander / Wulver |
| 112, Emergency Service | 255 | 2 | LI | Regular | Volunteers, FTO profile; counts as Volunteer |
| Uxía 'Cherry' McNeill | 263 | 1 | SK | Regular | — |
| Warcors | 50 | 1 | LI | Irregular | — |
| Armand 'Le Muet' | 680 | 1 | MI | Regular | — |
| Denma Connolly | 1749 | 1 | WB | Regular + Impetuous | Volunteers; Galwegians |
| Caledonian Mormaers | 251 | 3 | HI | Regular; Tactical Awareness on non-Lt profiles | Heavy Caledonians required-choice |
| McMurrough | 283 | 1 | WB | Irregular + Impetuous | — |
| 3rd Highlander Grey Rifles | 250 | 5 | HI | Regular | Volunteers; Heavy Caledonians required-choice; counts as Mormaer in Heavy Caledonians |
| Highlander Caterans | 248 | 4 | LI | Irregular | — |
| 9th Wulver Grenadiers | 253 | 5 | WB | Regular | 9th Wulvers |
| Volunteer Intel Isobel McGregor | 264 | 1 | LI | Regular | Wildcard; counts as Volunteer / Mormaer |
| The Scots Guards | 261 | 5 | MI | Regular | Scots Guards / Heavy Caledonians / 9th Wulvers, FTO profiles only |
| Wardrivers, Mercenary Hackers | 265 | 1 | LI | Regular | Scots Guards |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Intel Spec-Ops | 1915 | Spec-Ops | Caledonian Volunteers Fireteam row, max 1 when Spec-Ops mode is in use |
| Ariadna Team-Ops | 1929 | Team-Ops | No ordinary Caledonia Fireteam row |

## Unit details

### Dozers, Field Engineers

**ID 256 · AVA 2 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Engineer support troop with GizmoKit and Deactivator.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 13 | 0 | Rifle, D-Charges, Pistol, CC Weapon | — |
| 3 | 14 | 0 | Rifle, Blitzen, D-Charges, Pistol, CC Weapon | — |
| 4 | 14 | 0 | Rifle, D-Charges, Pistol, CC Weapon; Deployable Cover | — |
| 5 | 15 | 0 | Rifle, D-Charges, Armed Turret (Rifle), Pistol, CC Weapon | — |

### Cadin "FirstStrike" Donn

**ID 1525 · AVA 1 · WB** — `MOV 15-5 | CC 23 | BS 12 | PH 14 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 30 | 0 | T2 Boarding Shotgun, Flammenspeer, E/M Grenades, Boarding Pistol, AP + T2 CC Weapon | Wildcard max 1; Wulver |

### Traktor Mul

**ID 257 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 10 | PH 9 | WIP 12 | ARM 2 | BTS 0 | W 1 | S 4`. Baggage artillery/support REM.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 5 | 0 | PARA CC Weapon; Deactivator | — |
| 2 | 9 | 1 | Katyusha MRL, PARA CC Weapon; Guided | — |
| 3 | 14 | 1 | Uragan MRL, PARA CC Weapon; Guided, Total Reaction | — |

### 1st Highlanders S.A.S.

**ID 237 · AVA 4 · SK** — `MOV 10-10 | CC 22 | BS 11 | PH 13 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Camouflaged/infiltrating close-assault specialists.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 20 | 0 | Chain Rifle, Light Shotgun, D-Charges, Silenced Pistol, AP + Shock CC Weapon | — |
| 2 | 20 | 0 | Chain Rifle, Grenades, D-Charges, Assault Pistol, AP + Shock CC Weapon | — |
| 4 | 21 | 0 | Chain Rifle, Light Shotgun, Flash Pulse, D-Charges, Silenced Pistol, AP + Shock CC Weapon; Forward Observer | — |
| 5 | 25 | 0 | Boarding Shotgun, D-Charges, E/M Mine, Silenced Pistol, AP + Shock CC Weapon | — |
| 6 | 22 | 0.5 | Chain Rifle, Light Shotgun, D-Charges, AP Mine, Silenced Pistol, AP + Shock CC Weapon; Minelayer | — |

### 45th Highlanders Rifles 'Galwegian'

**ID 239 · AVA TOTAL · WB** — `MOV 10-10 | CC 22 | BS 10 | PH 14 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Irregular, Impetuous smoke warband.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 10 | 0 | Rifle, Smoke Grenades, Pistol, AP CC Weapon | Galwegians 1–5 |
| 2 | 5 | 0 | Chain Rifle, Smoke Grenades, Pistol, AP CC Weapon | same |
| 3 | 10 | 0 | Boarding Shotgun, Smoke Grenades, Pistol, AP CC Weapon | same |

### 2nd Irregular Cameronians Reg.

**ID 254 · AVA 3 · WB** — `MOV 15-10 | CC 23 | BS 10 | PH 16 | WIP 12 | ARM 4 | BTS 3 | W 2 | S 6`. Irregular, Impetuous Dog-Warrior assault troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 18 | 0 | Chain Rifle, Grenades, Smoke Grenades, T2 CC Weapon | — |

### Beasthunters Free Guild

**ID 1570 · AVA 1 · SK** — `MOV 10-10 | CC 21 | BS 11 | PH 13 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 9 | 0 | **BEASTHUNTER FTO**; Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CC Weapon | Volunteers max 1 |
| 2 | 15 | 0 | Heavy Flamethrower, Tactical Bow, AP Mine, Pistol, DA CC Weapon; Camouflage / forward deployment package | — |
| 3 | 15 | 0 | Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CC Weapon; Camouflage / forward deployment package | — |
| 7 | 17 | 0 | Heavy Flamethrower, Panzerfaust, AP Mine, Heavy Pistol, DA CC Weapon; Camouflage / forward deployment package | — |

### Caledonian Volunteers Corps

**ID 245 · AVA TOTAL · LI** — `MOV 10-10 | CC 13 | BS 11 | PH 11 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | Rifle, Chain-colt, Pistol, CC Weapon | Volunteers 1–5 |
| 2 | 6 | 0 | Chain Rifle, Light Shotgun, Pistol, CC Weapon | same |
| 3 | 18 | 1 | HMG, Pistol, CC Weapon | same |
| 4 | 8 | 0.5 | Light Shotgun, Grenade Launcher, Pistol, CC Weapon | same |
| 5 | 12 | 0 | Rifle, Chain Rifle, D-Charges, Pistol, CC Weapon; camouflage-style specialist profile | same |
| 6 | 12 | 0.5 | Light Shotgun, Chain-colt, Grenade Launcher, Pistol, CC Weapon; camouflage-style profile | same |
| 7 | 10 | 0 | Rifle, Chain-colt, Pistol, CC Weapon; MediKit, Paramedic | same |
| 8 | 8 | 0 | Rifle, Chain-colt, Pistol, CC Weapon; Lieutenant | same |
| 10 | 10 | 0 | Rifle, Chain-colt, Pistol, CC Weapon; Commlink profile | same |

### 112, Emergency Service (Motorized)

**ID 1284 · AVA 2 · LI** — `MOV 20-10 | CC 16 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 4`. Doctor on Motorcycle with MediKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4761 | 19 | 0 | Light Shotgun, Smoke Grenade Launcher, Smoke Grenades, Boarding Pistol, CC Weapon | — |

### William Wallace

**ID 259 · AVA 1 · WB** — `MOV 15-10 | CC 24 | BS 13 | PH 14 | WIP 15 | ARM 3 | BTS 0 | W 2 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 38 | 0 | T2 Rifle, Light Shotgun, Smoke Grenades, Boarding Pistol, EXP CC Weapon | Wildcard max 1; Highlander / Wulver |
| 2 | 38 | 0 | Same weapons; Lieutenant | same |

### 112, Emergency Service

**ID 255 · AVA 2 · LI** — `MOV 10-10 | CC 16 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Doctor with MediKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 11 | 0 | **112 FTO**; Light Shotgun, Boarding Pistol, CC Weapon | Volunteers max 1; counts as Volunteer |

### Uxía 'Cherry' McNeill

**ID 263 · AVA 1 · SK** — `MOV 10-10 | CC 22 | BS 11 | PH 13 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Multispectral Visor L1, camouflage/infiltration assault character.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 25 | 0 | Boarding Shotgun, Grenades, Smoke Grenades, Boarding Pistol, AP + Shock CC Weapon | — |
| 2 | 25 | 0 | Boarding Shotgun, D-Charges, Smoke Grenades, Assault Pistol, AP + Shock CC Weapon | — |

### Warcors

**ID 50 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular Journalist.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CC Weapon; 360º Visor | — |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CC Weapon; alternate utility profile | — |

### Armand 'Le Muet', Freelance Killer

**ID 680 · AVA 1 · MI** — active form `MOV 10-10 | CC 21 | BS 13 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 2 | S 2`; inactive Symbiont Armor form `ARM 0 | BTS 0`, LI.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2338 | 33 | 1.5 | MULTI Sniper Rifle, Nanopulser, Shock Mine, Breaker Pistol, Viral CC Weapon; Minelayer | — |
| 2339 | 34 | 1.5 | MULTI Sniper Rifle, Nanopulser, Breaker Pistol, Viral CC Weapon; Multispectral Visor L1 | — |

### Denma Connolly

**ID 1749 · AVA 1 · WB** — `MOV 15-5 | CC 23 | BS 11 | PH 14 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`. Regular, Impetuous close-assault character.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 12 | 0 | Chain Rifle, Smoke Grenades, Heavy Pistol, AP + DA CC Weapon | Volunteers max 1; Galwegians max 1 |

### Caledonian Mormaers

**ID 251 · AVA 3 · HI** — `MOV 10-10 | CC 17 | BS 13 | PH 13 | WIP 13 | ARM 5 | BTS 0 | W 1 | S 2`. X Visor. Non-Lieutenant profiles generate Tactical Awareness.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 41 | 0 | T2 Rifle, Chain-colt, Heavy Pistol, AP CC Weapon; Tactical Awareness | Heavy Caledonians required-choice, max 3 |
| 2 | 49 | 1.5 | HMG, Chain-colt, Heavy Pistol, AP CC Weapon; Tactical Awareness | same |
| 3 | 41 | 0 | T2 Rifle, Chain-colt, Heavy Pistol, AP CC Weapon; Lieutenant (+1 Lt Order) | same |
| 4 | 49 | 1 | HMG, Chain-colt, Heavy Pistol, AP CC Weapon; Lieutenant (+1 Lt Order) | same |

### McMurrough, Mercenary Dog-Warrior

**ID 283 · AVA 1 · WB** — `MOV 15-10 | CC 23 | BS 11 | PH 16 | WIP 14 | ARM 4 | BTS 3 | W 2 | S 6`. Irregular, Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Chain Rifle, Grenades, Smoke Grenades, AP + DA CC Weapon | — |

### 3rd Highlander Grey Rifles

**ID 250 · AVA 5 · HI** — `MOV 15-5 | CC 23 | BS 13 | PH 13 | WIP 12 | ARM 3 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 25 | 0 | T2 Rifle, Light Shotgun, Grenades, Smoke Grenades, AP Heavy Pistol, AP CC Weapon | Volunteers max 3; Heavy Caledonians required-choice max 3 |
| 3 | 28 | 1.5 | HMG, Smoke Grenades, AP Heavy Pistol, AP CC Weapon | same |
| 4 | 20 | 0 | T2 Boarding Shotgun, Grenades, Smoke Grenades, AP Heavy Pistol, AP CC Weapon | same |
| 5 | 25 | 0 | T2 Rifle, Light Shotgun, Grenades, Smoke Grenades, AP Heavy Pistol, AP CC Weapon; Lieutenant | same |
| 6 | 28 | 1.5 | HMG, Smoke Grenades, AP Heavy Pistol, AP CC Weapon; Lieutenant | same |

In Heavy Caledonians, Highlander Greys carry the Army-chart `(Mormaers)` equivalence label.

### Highlander Caterans

**ID 248 · AVA 4 · LI** — `MOV 10-10 | CC 22 | BS 12 | PH 13 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular camouflage sniper.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 1 | T2 Sniper Rifle, Pistol, AP CC Weapon | — |
| 2 | 21 | 0.5 | AP Sniper Rifle, Pistol, AP CC Weapon | — |
| 3 | 23 | 1 | T2 Sniper Rifle, Pistol, AP CC Weapon; Forward Deployment | — |

### 9th Wulver Grenadiers

**ID 253 · AVA 5 · WB** — `MOV 15-5 | CC 23 | BS 12 | PH 14 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 30 | 0 | Heavy Shotgun, Panzerfaust, Grenades, Boarding Pistol, AP + Shock CC Weapon | 9th Wulvers 1–5 |
| 2 | 34 | 0 | Mk12, Grenades, Boarding Pistol, AP + Shock CC Weapon | same |
| 3 | 29 | 0 | T2 Rifle, Light Shotgun, Grenades, Boarding Pistol, AP + Shock CC Weapon | same |
| 5 | 37 | 1 | AP Spitfire, Grenades, Boarding Pistol, AP + Shock CC Weapon | same |

### Volunteer Intel Isobel McGregor

**ID 264 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 11 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 25 | 0 | T2 Rifle, D-Charges, E/M Mine, Flash Pulse, Assault Pistol, CC Weapon | Wildcard max 1; Volunteer / Mormaer |
| 3 | 25 | 0.5 | Same weapons; Hacking Device, Hacker | same |

### The Scots Guards, 6th Caledonian Infantry Regiment

**ID 261 · AVA 5 · MI** — `MOV 10-10 | CC 16 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 31 | 1.5 | **SCOT GUARD FTO**; AP Spitfire, Flash Pulse, D-Charges, Pistol, CC Weapon | Scots Guards; Heavy Caledonians max 1; 9th Wulvers max 1 |
| 2 | 31 | 1.5 | **SCOT GUARD FTO**; Missile Launcher, Flash Pulse, D-Charges, Assault Pistol, CC Weapon | same |
| 3 | 26 | 0 | **SCOT GUARD FTO**; T2 Marksman Rifle, Flash Pulse, D-Charges, Pistol, CC Weapon | same |
| 4 | 22 | 0 | **SCOT GUARD FTO**; AP Submachine Gun, Panzerfaust, Flash Pulse, D-Charges, Pistol, CC Weapon | same |
| 8 | 32 | 1 | SCOT GUARD; Heavy Rocket Launcher, Flash Pulse, D-Charges, Assault Pistol, CC Weapon; Camouflage / forward-deployment package | — |
| 9 | 32 | 0 | SCOT GUARD; AP Submachine Gun, Panzerfaust, Flash Pulse, D-Charges, Pistol, CC Weapon; Camouflage / forward-deployment package | — |
| 10 | 23 | 0 | **SCOT GUARD FTO**; AP Submachine Gun, Panzerfaust, Flash Pulse, Pistol, CC Weapon; MediKit, Paramedic | Scots Guards; Heavy Caledonians max 1; 9th Wulvers max 1 |
| 11 | 26 | 1.5 | **SCOT GUARD FTO**; Heavy Rocket Launcher, Flash Pulse, D-Charges, Assault Pistol, CC Weapon; Multispectral Visor L1 | same |

### Wardrivers, Mercenary Hackers

**ID 265 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 1 | Boarding Shotgun, Flash Pulse, Cybermine, Pistol, CC Weapon; Hacking Device, Hacker | Scots Guards max 1 |
| 2 | 16 | 1 | Same + Disco Baller; Hacking Device, Hacker | same |

## Canonical Fireteam chart

Sectorial Fireteam limits in the pinned source:

- **Core:** 1
- **Haris:** 1
- **Duo:** unlimited (`256` sentinel in Army data)

### Caledonian Volunteers Fireteams

**Types:** Core, Haris

| Entry | Min | Max | Counts as / profile restriction |
|---|---:|---:|---|
| VOLUNTEER | 1 | 5 | — |
| HIGHLANDER GREY | 0 | 3 | — |
| 112 FTO | 0 | 1 | Volunteer |
| BEASTHUNTER FTO | 0 | 1 | FTO profile only |
| DENMA CONNOLLY | 0 | 1 | — |
| INTEL | 0 | 1 | Spec-Ops only |

### Scot Guards Fireteams

**Types:** Core, Haris, Duo

| Entry | Min | Max | Counts as / profile restriction |
|---|---:|---:|---|
| SCOT GUARD FTO | 1 | 5 | FTO profiles only |
| WARDRIVER | 0 | 1 | — |

### Heavy Caledonians Fireteams

**Types:** Haris, Duo

The two marked rows are a **required-choice set**: an eligible Heavy Caledonians Fireteam must satisfy the Army chart's required foundation with Mormaers and/or Highlander Greys; the source flags both alternatives as `required: true` and does not mean one of each is mandatory.

| Entry | Min | Max | Required-choice | Counts as / profile restriction |
|---|---:|---:|---|---|
| CALEDONIAN MORMAER | 0 | 3 | yes | — |
| HIGHLANDER GREY | 0 | 3 | yes | Mormaers |
| SCOT GUARD FTO | 0 | 1 | no | FTO profiles only |

### Galwegians Fireteams

**Types:** Core

| Entry | Min | Max | Counts as / note |
|---|---:|---:|---|
| HIGHLANDER | 1 | 5 | — |
| DENMA CONNOLLY | 0 | 1 | Current unit slug `denma-connolly`; chart uses legacy slug `denma-connolly-caledonian-zellenkrieger` |

### 9th Wulver Fireteams

**Types:** Core, Haris, Duo

| Entry | Min | Max | Counts as / profile restriction |
|---|---:|---:|---|
| WULVER | 1 | 5 | — |
| SCOT GUARD FTO | 0 | 1 | FTO profiles only |

### Wildcards

| Entry | Max | Counts as / note |
|---|---:|---|
| WALLACE | 1 | Highlander, Wulver |
| ISOBEL McGREGOR | 1 | Volunteer, Mormaer |
| "FIRSTSTRIKE" DONN | 1 | Wulver |

Wildcards may join otherwise eligible Fireteams subject to the normal sectorial limits and the profile restrictions above.

## Reverse Fireteam access index

| Troop / profile | Fireteam families | Notes |
|---|---|---|
| 112 FTO | Volunteers | Max 1; counts as Volunteer |
| Beasthunter FTO | Volunteers | FTO profile only; max 1 |
| Cadin "FirstStrike" Donn | Wildcard | Max 1; Wulver |
| Caledonian Mormaer | Heavy Caledonians | Required-choice; max 3 |
| Caledonian Volunteer | Volunteers | Native 1–5 row |
| Denma Connolly | Volunteers; Galwegians | Max 1 in either listed family |
| Highlander Grey | Volunteers; Heavy Caledonians | Max 3; required-choice in Heavy; counts as Mormaer there |
| Isobel McGregor | Wildcard | Max 1; Volunteer / Mormaer |
| Scot Guard FTO | Scots Guards; Heavy Caledonians; 9th Wulvers | FTO profiles only; native 1–5 in Scots, max 1 in Heavy/Wulver |
| 45th Highlander | Galwegians | Native 1–5 row |
| Wallace | Wildcard | Max 1; Highlander / Wulver |
| Wardriver | Scots Guards | Max 1 |
| Wulver | 9th Wulvers | Native 1–5 row |

All standard roster units not listed in this reverse index have no Fireteam access in the pinned standard Caledonia chart.

## Reinforcement Fireteams — L'Équipe Argent

Linked Reinforcement army: **L'Équipe Argent (Army ID 399)**, source revision `7.26246.158`.

These rows are intentionally separate from the standard Caledonia chart. Reinforcement Fireteam limits in the pinned source are **Core 1; Haris 1; Duo 1**.

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

- Standard roster count reconciled to **23** ordinary Caledonia entries after excluding `Intel Spec-Ops`, `Ariadna Team-Ops`, and generic `merc-*` catalog entries with an empty faction list.
- Army ID `302` is explicitly marked `discontinued: true` in the pinned N5 Army metadata; this reference nevertheless uses the complete current N5 roster and Fireteam data shipped for that Army ID.
- Every standard `fireteamChart` row from Army revision `7.26246.158` is represented, including the Heavy Caledonians required-choice set and all profile-sensitive FTO joins.
- Fireteam limits are preserved exactly: Core 1, Haris 1, Duo unlimited in Caledonia.
- `SCOT GUARD FTO` is kept distinct from the non-FTO camouflaged Scots Guard profiles; non-FTO profiles are not granted Fireteam access merely because they belong to the same unit.
- `BEASTHUNTER FTO` is kept distinct from the camouflaged Beasthunter profiles.
- The Denma Connolly unit/chart slug mismatch is documented rather than silently normalized away.
- The linked Reinforcement army resolves to **L'Équipe Argent (399)** and its chart is preserved separately.
- Main and Reinforcement Wildcards are not merged.
- Source data and Fireteam normalization were rechecked on **2026-10-15** against the pinned Army snapshot and InfinityDB commit listed in the front matter.
