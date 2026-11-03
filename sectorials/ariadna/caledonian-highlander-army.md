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

## Community tactics — transcript-based Caledonia research (2026-10-19)

> **Authority and dating:** The roster, costs, abilities and Fireteam tables **above** reflect pinned **N5.3 / September 2026 Army** data and supersede the **October 2025 N5.2-era** video/podcast opinions below. Treat specific presenter claims as advice, not verified current profiles. This is tactical analysis, not an amendment to the canonical Fireteam chart. In particular, the current file lists **Wallace non-Lt/Lt**, **Isobel non-hacker/hacker** (not the Chain of Command profiles described in some 2025 discussions), and a **Scots Guard FTO Missile Launcher**, despite a 2025 speaker lamenting its removal. Do not copy 2025 list codes or historic profiles uncritically.

### Game plan: solve shooting problems, then flood the midfield

- **Vision denial → favorable engagement → trade:** Cheap Galwegian/112/Grey/Cameronian smoke and a Wardriver **Disco Baller** disrupt exposed firelanes and MSV threats. Use the opening for **Uxia/SAS** objectives and attack angles, **Mormaer** AP HMG gunfights, or **Cameronians/McMurrough** close-range templates/CC. **Why:** CHA has great close assault and powerful select guns, but comparatively little durable, versatile, long-range ARO and limited sophisticated hacking.
- **Prioritize orders on the real attacker.** 6-point regular Volunteers, 5-point Baggage Traktor Muls and cheap warbands keep the list functional while paying for Mormaer + Wulver/Cadin/Uxia. The cheap pieces are useful only if the primary attack, objectives, protection and order allocation still fit.
- **Choose an actual plan, not every attractive model.** Podcasts repeatedly praise Uxia, Mormaer, dogs and Wardriver, but note that taking all of them plus multiple full Fireteams leaves little room for specialists/backup attacks. Reserve a credible second attack axis.
- **Don't force 6 SWC.** Caledonia's strength is often low-SWC T2/AP, smoke, melee and templates. Filling unused SWC with unnecessary HMGs can weaken the order pool or mission coverage. (Loss of Lieutenant ~49–52m.)

### Frequently recommended packages (why they work)

| Package / role | Why; how to play it | Watch for |
|---|---|---|
| **Mormaer HMG (49, 1.5 SWC, Tactical Awareness) + Grey + Scots Guard FTO** Heavy Caledonians Haris | Mormaer supplies high-damage AP long-range FtF threat; Grey adds smoke/T2 close cover cheaply; FTO **Paramedic** can take objectives and revive, while other FTO loadouts add range or ARO. Small mixed team carries attack + utility without buying three Mormaers. | Mormaer has **BTS 0 / W 1 + NWI**; Breaker/Viral and unfavorable reactive fights can erase the centerpiece. Avoid assuming high ARM makes it invincible; HMG Lt alternatives **do not** also give Tactical Awareness in pinned roster. |
| **Mormaer Lt (+1 Lt Order) versus Wallace Lt** | Mormaer Lt funds a costly heavy shooting approach and can exploit NCO Scots Guard in a linked plan; Wallace Lt historically powers a warband-heavy assault via Inspiring Leadership. Decide before buying the cheap irregular base or large heavy link. | 2025 presenters' Wallace/Isobel **Chain of Command** alternatives do **not** appear as such in the pinned N5.3 loadout table. Verify exact current Lt-order spending and troop skills before cloning historic combos. |
| **Wallace + cheap Galwegians Core** | Extremely economical assault pressure; smoke and close combat let the team advance together and contest short-range objectives; Wallace counts as Highlander. A team of all chain-rifle warbands has few useful long-range AROs. | Full Core and two-/three-dog packages compete with the Heavy Haris or Wulver Core; keep Wallace safe if he is Lt. |
| **Cameronian (18), one to three; optionally McMurrough (23)** | High speed, ARM4, two wounds, smoke, templates and CC create disproportionate damage for the price. Cameronians' T2 weapon + Natural Born Warrior help kill armored melee targets. Multiple threats stretch enemy reactions and can support coordinated pressure. | Impetuous/Irregular order accounting matters. Exposed dogs can die before connecting. McMurrough adds a different AP+DA melee package; compare matchups rather than assuming he replaces a Cameronians' T2/NBW. |
| **Uxía (25) + SAS FO/Minelayer** | Infiltrating attack/specialist tool plus hidden midfield specialists gives mission reach without relying on heavy troops to press buttons. Uxía's MSV1, extra burst and smoke interaction are especially valued; SAS AP mines guard approach routes. | Forward infiltration risks an isolated expensive trade; plan the extraction or accept the one-way role. Distinguish SAS FO for scoring vs Minelayer for area denial. |
| **Two Wulvers (Duo) or Wulvers + Cadin + FTO Scots Guard** | Duo buys the special Fireteam die for less than a large Core; Wulvers' Discover +6 helps clear Camouflage, 2W + mobility + short-range guns/grenades contest rooms. Cadin supplies E/M grenades, T2 Boarding Shotgun and extreme active-turn Berserk/CC; FTO Paramedic adds recovery/objectives. | Pure Wulver Core is expensive and can crowd out long guns/specialists. Cadin and Wulvers overlap on close combat; do not pay twice for an unneeded role. |
| **Wardriver Disco Baller (16, 1 SWC) in Scots Guard team or alone** | Delivers scarce hacking and nonlethal E/M/vision control; pairing with Scots FTO can gain Fireteam benefit and lets a normally hacking-light faction contest hack objectives or disrupt MSV firing positions. | BS11, BTS3, 1W; linked Scots-Guard tax can be steep. Fragile support is not a substitute for an actual robust hacking network. |
| **Highlander Grey T2 Boarding Shotgun (20) or T2 Rifle (25)** | Cost-efficient smoke carrier, nasty short/mid-range T2, and flexible Volunteer/Heavy Fireteam support. Useful second attack/trader alongside a Mormaer. | HMG (28, 1.5 SWC) gives a cheap BS13 long gun, but Frenzy and exposed-range matchups make it contentious as the *main* gun. |
| **Cateran T2/AP sniper (21–23), Armand MSV1 sniper (34), Scots FTO MSV1 HRL (26)** | Complementary defensive/attack choices: camouflaged Cateran holds a long lane, Armand offers durable Mimetism/visor tools, Scots gives a linkable specialist with MSV1 and template ARO. | Weakness of static AROs: a dense table may let opponents ignore a sniper; Irregular Caterans cost command resources unless regularized; Armand is costly. Don't build an entire DZ defense around a single line of fire. |

### Actual list archetypes

1. **Warband saturation:** Wallace Lt, 2–3 Cameronians, optionally McMurrough, smoke Galwegians, Uxía/SAS and 5-point Muls; add a Wardriver and at least one credible gun. **Why:** multiple independent cheap melee/template threats overwhelm single AROs and trade up. **Concern:** limited long-range dominance and exposure to area templates/vision counters.
2. **Heavy anchor:** Mormaer Lt or Tactical Awareness HMG, Grey + Scots FTO Haris, Uxía/SAS, cheap Volunteer/Traktor order base, one dog, Wardriver. **Why:** dedicated AP shooting opens lanes, compact specialists then score. **Concern:** loss of a 41–49-point Mormaer leaves the list without its key ranged solver.
3. **Wulver room-clearing Core:** Wulver AP Spitfire or Mk12 + Cadin + Scots FTO Paramedic, with Grey/Mormaer ranged support and Uxía/SAS. **Why:** fast 2W Discover-and-assault group dominates tight midfield and can recover casualties. **Concern:** costs and overlapping close-range tools can leave weak ARO/long-range backup.
4. **Budget Fireteam + many tools:** 2–4 Volunteers + HMG Grey or short-range Grey, with external dogs/Caterans/SAS/Uxía. **Why:** cheap legal Core provides a modest active gun/ARO and orders; spend elsewhere rather than concentrating points. **Concern:** BS13 Grey HMG is not Mormaer-level high-end FtF shooting.

### Real disagreements recorded — retain both sides

| Decision | Opinion A | Opinion B / deciding factor |
|---|---|---|
| **Wallace automatic?** | Tactical Awareness and WIP12 value Lt Wallace for turning an irregular warband plan into an order-rich assault; Wallace + cheap Highlanders is economical. | Tactical Awareness hosts also argue he is **not** automatic: Mormaer Lt(+1) with a heavy team plays differently. Pick based on desired irregular count, Lt risk and active attack. |
| **Mormaer exposed ARO?** | Tactical Awareness proposes an aggressive Mormaer Lt HMG as a deterrent or even intentionally expendable ARO, with Wallace backup in its October 2025 configuration. | Loss of Lieutenant warns **BTS0, 1W/NWI** makes every lost FtF dangerous, especially Viral/Breaker; active-turn FtF and selective MSV-target removal are safer. The backup-CoC portion of the historic plan is **not current N5.3**. |
| **Grey HMG or close Grey?** | WIP12 recommends 28-point Grey HMG plus low-cost Volunteers as an inexpensive long gun, especially with Fireteam bonuses. | Loss of Lieutenant calls the HMG mediocre as a centerpiece with Frenzy and stronger Mormaer choices; 20-point T2 BSG/25-point T2 Rifle is superior for smoke/close-point trade. |
| **Wulver Core versus Duo** | WIP12 favors a Wulver-heavy Core + Cadin + paramedic for Discover, grenade saturation and objective-room clearing. | Loss of Lieutenant prefers **two Wulvers** or smaller teams to gain key special-die benefit without tying too many points to a close-combat package; spec-fire grenade spam is disputed as order-inefficient. |
| **Scots Guards good or disappointing?** | Loss of Lieutenant praises MSV1 HRL, FTO Paramedic, Forward Observer/NCO and flexible Fireteam glue. | Other panelists say the rework removes distinctive camouflaged heavy-gun choices and leaves bland weapons, making them largely an obligatory support tax. **Current 2026 FTO Missile Launcher exists**; the older complaint concerned lost camouflaged alternatives, not current absence of all ML loadouts. |
| **Cadin vs regular Wulver** | Cadin's E/M grenades and T2 BSG excel at disarming TAG/HI targets and active-turn CC; strong pick alongside a ranged Wulver. | Ordinary Wulvers have strong Discover, two wounds and better prolonged board control; Cadin's extreme Berserk doesn't translate equally into reactive CC. |
| **Wardriver automatic?** | Loss of Lieutenant calls Disco Baller close to mandatory to solve MSV/tech problems; Tactical Awareness likes the affordable option. | Other speakers note BS11 and a costly linked Scots team to gain extra die; cheap screens, smoke, direct CC, and mission specialists sometimes provide better returns. |
| **Cateran sniper swarm?** | Viejo Melmak describes coordinated T2 Cateran sniping as a traditional way to eliminate hard AROs, with high Caledonian AVA. | Tactical Awareness notes static Irregular snipers can be avoided on dense boards; with Wallace order conversion they improve, but they remain map-dependent and take slots from specialists/dogs. |
| **Dozer needed?** | Tactical Awareness downplays Dozers because Caledonia has few critical engineering targets and no TAG. | A Dozer can still repair/recover Traktor Muls and handle Engineer objectives; include with a deliberate artillery/support role, not by default. |

### REM, Vehicle and TAG research — the *actual* Caledonia roster

- **Only REM = Traktor Mul (AVA 2).** **5 pts / 0 SWC Baggage + Deactivator** is the baseline: a cheap **Regular** order, broad resupply coverage, and a spare objective-compatible support body. Loss of Lieutenant's ~53–55m list puts **two Muls in group one** and the Disco Baller Wardriver **in group two**; the Muls are positioned to extend Baggage/reload coverage to another group. The 2025 Tactical Awareness roster also used the 5-point support variant.
- **9 pts / 1 SWC Katyusha Guided MRL:** choose for deliberate guided-fire plans **only** when FO/Spotlight/target-state setup and orders are allocated. CHA has SAS FOs, Scots Guard FTO FOs and Wardriver/Isobel hacking options, but no large repeater mesh; guided artillery is not inherently reliable just because Guided is printed on its profile.
- **14 pts / 1 SWC Uragan Guided MRL with Total Reaction:** choose for a dedicated defensive/template or Guided mission plan; BS10, one wound, ARM2, no camouflage, and supply costs make it a weak general replacement for Mormaer/Cateran ARO. Protect/position it and price in Dozer access if repair matters.
- **Dozer Engineer (13–15 pts)** is available; weigh its Engineer-objective role, turret/deployable-cover loadouts, and ability to recover Muls against cheaper bodies. No normal Servant-bot / TAG recovery web is implied by this roster.
- **Vehicles/TAGs: none on CHA's standard 23-unit N5.3 roster.** **Motorized 112 (19 pts)** is a mobile **LI Doctor on motorcycle**, not a VH trooper or TAG; smoke movement/rapid medical access is its contribution. No Chernobog, Vystrel, Kuryer, or other Ariadna/Mérovignian/Kosmoflot vehicle/TAG/REM can be assigned to CHA just because it exists elsewhere.
- **Against enemy TAGs:** Mormaer **AP HMG** punches ARM; **Cadin E/M grenades** or Wardriver Disco Ballers can disable/deny; **Cameronian T2** and McMurrough **AP+DA CCW** threaten from melee. Deliver them using smoke and lateral movement; avoid pure BS10–12 open-field gunfights.
- **Cross-sectorial REM transcript check (Tactical Awareness N5, February 2025):** [Tartary Part 2](https://open.spotify.com/episode/2VCGfZZhXpth6ahryGhPyw) (~20m) recommends the **5-point Baggage Mul** as inexpensive Regular-order support, and (~32m) considers two **Total Reaction Uragans** as a niche overlapping ARO/artillery shell. [Kosmoflot Part 3](https://open.spotify.com/episode/0FZYrBdbYi3bNLX0Xbdl3l) (~11–16m) uses **Katyusha Guided MRL** plus artillery/board-state interactions; speakers explicitly warn that its unassisted speculative fire is poor. [Vanilla Ariadna Part 4](https://open.spotify.com/episode/3WYxtimNdXjHDsMOWvEWw6) (~2–4m) pairs an FO with Katyusha Guided and a cheap Deactivator/Baggage Mul for reloads and mine clearing. [USAriadna Part 1](https://open.spotify.com/episode/4wIT3UwMB9LldCtHdfLU6k) (~14–15m) uses Baggage to reload disposable ARO weapons. **Transferable CHA lesson:** first buy the 5-point Mul for orders/Baggage; upgrade to Katyusha when you have a reliable FO + order plan; buy Uragan TR only for a specific defensive firelane/artillery plan. These other sectorials' non-CHA units, FOs and Fireteams are **not** CHA list options.
- **Source-scope check:** No separate, substantial post-2025 Caledonia-exclusive Vehicle/TAG analysis was found; broader Ariadna episodes concern platforms not necessarily selectable in CHA. Transfer **role principles**, never illegal roster entries.

### Transcripts and further reading (exact source provenance)

**Transcripts directly checked via PodcastMCP:**
- [Tactical Awareness S3E38 — Caledonia (27 Oct 2025; 51m)](https://open.spotify.com/episode/4WgaVJBlbSm3wHIsBPPsWb) — strongest contrasting **Wallace assault vs Mormaer Lt**, Cameronians, Uxía, mixed Haris and weak long ARO.
- [WIP12 E192 — Caledonia First Impressions (3 Oct 2025; 45m)](https://open.spotify.com/episode/5gLOPl1YiSrkGOQ9H0Rg5B) — extensive unit-by-unit / five Fireteam-family walkthrough, Wulvers, Cateran, Mormaer, Grenades, Grey Core.
- [Loss of Lieutenant E158 — Return of Lost Sectorials Part 2 (28 Oct 2025; Caledonia ~5–56m)](https://open.spotify.com/episode/1pQ6J6OGpzyu8QlxiFoo8D) — **best critical panel** for Grey HMG, Wulver Speculative Fire, Scots Guard rework, Mormaer exposure, Disco Baller and **dual Baggage Mul** example.

**YouTube transcripts directly checked with YoutubeMCP** (overlap with podcast audio is **not** independent confirmation):
- [Tactical Awareness Caledonia video](https://www.youtube.com/watch?v=rcD9YwMny9E) — same S3E38 recording.
- [Loss of Lieutenant episode 158 video](https://www.youtube.com/watch?v=EoQ3Ma7Hp7k) — same episode.
- [Viejo Melmak — Caledonia N5 (Spanish, 3 Oct 2025)](https://www.youtube.com/watch?v=uFhv362lnBQ) — army background, 4-dog builds and traditional coordinated Cateran T2 sniping.
- [Dice Gods — Six Armies Return to N5 (3 Oct 2025)](https://www.youtube.com/watch?v=Zl8_OvX0m3E) — brief cross-faction first reaction rather than deep Caledonia tactics.
- [Ryanj4043 — Out-of-Production Army Proxy Guide (1 Dec 2025)](https://www.youtube.com/watch?v=_WD3c5XdrX0) — **Caledonia section ~08:20–16:34**; collecting/proxy advice, not a substitute for a tactical unit review.

**Written cross-checks:** [Corvus Belli's October 2025 official Army changelog](https://infinityuniverse.com/en/news/army-update-october-25); [community N5 Caledonia tactics index](https://www.bureau-aegis.org/forum/index.php?topic=18023.0); [Goonhammer returning sectorials overview](https://www.goonhammer.com/infinity-n5-returning-sectorials-reviewed/) (linked; article text was not directly retrieved). **Current legal data:** the pinned **N5.3 September 2026** roster and Fireteam section **above**; do not silently overwrite with these 2025 snapshots.

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

## Hacker and KHD tactical cross-reference (2026-10-23)

**Isobel McGregor HD 25/0.5** is Caledonia's more integrated hacker/operative option; **Wardriver HD14/1** buys the basic anti-HI/TAG program suite at high SWC cost, but lacks a powerful natural repeater network. **Why:** Isobel can combine WIP13 general HD interaction with army-specific mission/link plans; Wardriver is mainly an emergency **Carbonite/Oblivion** answer against high-tech heavies. Against armies with few Hackable troopers, both compete poorly with Caledonia's efficient close-assault/Scots/McMurrough-style threats; do not invent a native KHD or Nomad-like Turn-0 network.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

For cross-faction **apex** and **points-value** rankings, the Order types, situational counterexamples and transcript-backed disagreements, see [Cheerleaders and Order Generators — N5.3](../../notes/list-building/cheerleaders-and-order-generators.md). Roster profiles/AVA/Fireteam legality above take precedence.

- **6pt Volunteer Chain Rifle/Light Shotgun**: extremely cheap S2 Regular body that can still guard a doorway

**List-building test:** count *transferable* Regular Orders by Combat Group after deployment; include required link members/command enablers, physical DZ footprint, and the unit's actual ARO/mission contribution. Do not treat Irregular, Tactical, Lieutenant or Peripheral activations as interchangeable generic Orders.


## ARO apex/value cross-reference (2026-10-23)

See [ARO units: N5.3 apex/value tiers, hidden-versus-visible and deployment/matchups](../../notes/list-building/aro-units-apex-and-value.md). The **current profile details here** control exact cost/SWC, Training and Fireteam eligibility; do not import another faction's link or specialist upgrades.

- **6pt Caledonian Volunteer Chain Rifle** — cheap Regular corridor guard; spend few points to force an enemy's next Order
- **Cateran T2/AP Sniper (21pt)** — camouflaged long-range trade-up to HITAG, Irregular status: no transferable pool Order
- **Traktor Mul support** — rare Ariadna cheap reload/guided/total-reaction choices; only buy a real Guided program if FO route is viable
- **3pt Warcor Flash** — Irregular very-cheap ARO tax, not a transferable pool Order

**Choose by circumstance:** a hard long gun matters only when the opponent must cross its arc; cheaper mines, Camo markers, templates, Flash, DTWs and hacking force movement or risk without committing an entire attack plan. Budget a second layer and preserved counterattack, check pie-slicing, hidden Order cost, anti-visual bypass and repair routes.

## Command-unit apex/value cross-reference (2026-10-23)

**Wallace LT 38/0** converts qualifying Irregular warbands with Inspiring Leadership and unlocks a special coordinated assault, whereas **Mormaer LT(+1) 41/0 T2 or 49/1 HMG** deliberately funds a tougher fighting-LT plan. Older **Scots Guard NCO** advice must be checked against this specific faction's chart (do not import Kosmoflot assumptions). Choose Wallace with many useful Irregulars, Mormaer when extra personal combat Orders and armor matter more.

See [cross-game Lieutenant, CoC and Order-economy tiers](../../notes/list-building/command-units-apex-and-value.md). **Refer to this pinned roster/Fireteam chart for profile legality.**

## Warbands and inexpensive trading roles — N5.3

**Galwegian Chain Rifle+Smoke5/0 (AVA Total)** is elite pure **value**: 5pt Irregular+Impetuous AP CC/CC22/PH14 can force a much pricier shooter to spend 2+ Orders on a template/smoke guard. It is **not guaranteed** to kill a 3W TAG. **Cameronian18/0** has 2W, PH16/S6 and better sustained CC/smoke pressure; **McMurrough23/0** adds Dogged/AP+DA. **Denma Connolly12/0 Regular+Impetuous** is a stronger self-directed advance but twice the Galwegian price. **Wallace LT38 Inspiring Leadership** makes eligible Irregular armies more flexible (Religious Troop exclusion); his **non-LT** profile should not be assumed to grant army-wide LT engine. In current Caledonia roster the first Wallace option is unlabeled in summary: check current profile if using it for **CoC** rather than importing Kosmoflot.

[Cross-game warband/cheap-trader apex and value tiers, targets and command packages](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). Profile-specific sectorial legality/Fireteams above control all selections.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

With multiple **cheap Dogged/Impetuous trading units**, do not overpay for a Doctor whose likely casualties **won't be eligible to revive** after Dogged. A roster-legal **112/Dozer/Irmandinho** should be valued for actual mission, Smoke and anti-state tasks. **Doctors fail lethally** on eligible No-Cube VITA targets without Cube reroll; recovery support is better reserved for a durable specialist or significant ARO worth bringing back. [Doctor/Engineer recovery odds and tier guide](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Galwegian5/0** is extraordinary **Irregular Smoke+CC22 AP** disposable attack/pinning value; **Cameronian18** gives 15-10 mobility, 2W and T2 CC with Smoke; **McMurrough23** trades up with 2W/Smoke/PH16 and **AP+DA**. **Uxía25** brings actual **infiltrating/marker-assisted entry** but CC22/AP+Shock is not a Hidden Mono Oniwaban; **Wallace38/0 CC24 EXP** and **Cadin30 AP+T2** are durable multifunction frontline duelists requiring careful orders. Against a serious NBW/Guard defender prefer warband smoke and templates before charging. [Close-combat apex/value, positioning and counter-CC](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Beasthunter9 Panzerfaust+HFT /15 Camo+FD** and **Dozer14 Blitzen** are the best budget ranged anti-armor profiles; **Scot Guard22 Panzerfaust+AP SMG** provides midcost short lethal threat. **S.A.S.25 E/M Mine+D-Charges** is positional shutdown, not guaranteed TAG death. **Wallace / McMurrough / Cameronians** are strong close attack/traders, but reaching TAG contact through templates and screens can cost more Orders than an ambush. E/M Mines tax recovery Orders. [Non-hacking armor-killer value rankings and tactical matchups](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**S.A.S. Forward Observer21/0** uses Infiltration/Camouflage to retrieve a box or dominate a midfield corner, but **cannot keep the Marker state while carrying**; 1W/ARM0 means leave under a **5pt Galwegian Smoke** screen and guard a covered exit. **Scot Guard FTO Paramedic23/0** (if in legal Scot Guard/Heavy Caledonian FT) gives a sturdier ARM3 W1 carrier and support. **Wulver T2 Rifle29/0** (2W ARM3) or **Mormaer T2 Rifle+Tactical Awareness41/0** (ARM5 W1) hold zone VP but *not* ordinary Supplies without specialist profile. **Cameronian18/0 W2 ARM4 + Smoke** and **McMurrough23/0** deter close assault and can contest a zone but are **Irregular/Impetuous, not free Regular specialists**. **Counter:** multiple Wulvers bunched in a fireteam are vulnerable to templates; S.A.S. + smoke + independent zone defender retains two scoring routes.

[Cross-game objective holder and zone-domination apex/value tiers, scenario rules, and opposing transcript reviews](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Exact profiles/Fireteams above are authoritative.

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Wardriver Disco Baller16/1** is an affordable, SWC-costed **Eclipse** route around enemy MSV/Marksmanship; its limited charges and setup Orders matter. **Galwegian/Cameronian Smoke** blocks ordinary guns, not an enemy MSV2. Against Mimetism/Camo, cheap Discover probes, close templates, and covered CC flanks may be better than buying a weak direct gun duel. **Opposing faction reviews:** some prioritize the Disco Baller as a scarce anti-visor answer; others prefer more Regular Orders/guns when map geometry already provides a bypass.

[Cross-game anti-tech N5.3 apex/value, mechanics, matchups and checked conflicting transcripts](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## Mission performance — battle-report evidence (2026-11-01)

| Mission(s) | Tested composition / scoring mechanism | Evidence |
|---|---|---|
| **Critical Intervention / confined rooms** | Wallace, McMurrough/Cameronian/Galwegians with Wulver/Kaden/Mormaer made layered room-door CC/template barriers vs White Banner. | [#086](../../notes/battle-reports/081-090-n5-battle-report-tactical-analysis.md) |
| **Close defense against expensive attackers** | Multiple short-range CC threats can tax heavy armor on narrow approach lanes; keep a real console/carrier route after stopping the attacker. | [#086](../../notes/battle-reports/081-090-n5-battle-report-tactical-analysis.md), [#161](../../notes/battle-reports/161-170-n5-battle-report-tactical-analysis.md) |

**Limits:** One decisive room example does not prove broad Caledonian superiority on every room or zone mission. Game-era qualitative evidence, not a win-rate or current Fireteam claim. [Full mission evidence audit](../../notes/battle-reports/cross-report-mission-performance-by-sectorial.md).

## Counterplay — observed N5 battle-report responses (2026-11-02)

| Threat / target | Observed response, timing and consequence | Battle reports |
|---|---|---|
| **Against elite HI / room Fireteams** | Wallace/McMurrough/Cameronians/Galwegians created layered templates, Wulver/Kaden hard CC and Mormaer long gun halted White Banner heavy infantry around Critical Intervention doorway. | [#086](../../notes/battle-reports/081-090-n5-battle-report-tactical-analysis.md) |
| **Against Camo and mobile tech** | Opponent Kestrel Redeye Sensor revealed Caledonian Camo then Black A.I.R. K1 pressured a Cameronian; maintain smoke/alternate lane instead of relying only on marker protection. | [#158](../../notes/battle-reports/151-160-n5-battle-report-tactical-analysis.md) |
| **Against TAG as conceptual threat** | Caledonian CC influenced a Combined champion's decision **not to field an Avatar list**, but that list was unplayed and is not proof of a killed Avatar. | [#155](../../notes/battle-reports/151-160-n5-battle-report-tactical-analysis.md) |

**Limit:** The clearly observed success is **room-entry delay versus HI**; do not claim a universal TAG or hacker hard counter from this sample. These are game-era actions, not current N5.3 profile/Fireteam legality or faction win rates. [Cross-report counterplay analysis](../../notes/battle-reports/n5-cross-report-counterplay-tags-hi-hacking-camo-impersonators-fireteams.md).

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

### 5. Caledonian Highlander Army

[Current roster / Fireteams](caledonian-highlander-army.md) · [Detailed guide](../../notes/factions/caledonia.md)

**Near-must considerations**

| Piece | Why; limit | Evidence |
|---|---|---|
| **Uxía** | 25pt camouflaged midfield attacker/specialist with Smoke/CC and excellent role compression. Hard to replace her blend of scoring and killing. | [Ryanj4043 — N5 Caledonia review (May 2026)](https://www.youtube.com/watch?v=iyKGgFUA1JA) endorses skirmisher mission roles; [TA S3E38](https://open.spotify.com/episode/4WgaVJBlbSm3wHIsBPPsWb) favors Uxía over Isobel in some contexts. |
| **SAS FO / Minelayer** | Essential *role* of independent forward objective scoring/control with camouflage; SAS is the easiest repeated solution. | Ryanj4043 Caledonia video; existing Caledonia guide. |
| **Cameronian (often one or two)** | Only 18 points for a high-speed Smoke/CC/trading missile. Very strong with Wallace, but Irregular in a conventional build. | [TA S3E38](https://open.spotify.com/episode/4WgaVJBlbSm3wHIsBPPsWb) explicitly praises Cameronians (~5–10m); [Ryanj4043 review](https://www.youtube.com/watch?v=iyKGgFUA1JA). |

**Go-to**

| Piece | Why; important qualification | Evidence |
|---|---|---|
| **Wallace LT, specifically in an Irregular-economy build** | Inspiring Leadership can convert 5pt Galwegians, 18pt Cameronians and Caterans/McMurrough into useful Regular-order infrastructure. This is an *army architecture*, not merely an expensive fighting LT. | TA S3E38 uses Wallace/Cameronian/McMurrough coordinated concepts; Ryanj4043 explicitly says Wallace is **optional**. |
| **Mormaer HMG** | ARM5 and substantial HMG reach; non-LT has Tactical Awareness, while LT profiles pursue different LT-order economy. | Ryanj4043 review; TA S3E38; Caledonia guide. |
| **Highlander Grey HMG / T2 BSG** | Economical linked ranged anchor/short-range threat with cheap Volunteer support. | Ryanj4043; Caledonia guide. |
| **45th Highlander / Galwegian Chain Rifle** | Five-point Smoke/template/CC trading unit; particularly attractive under Wallace, but 15-model slots remain scarce. | TA S3E38; Ryanj4043. |
| **McMurrough** | Strong independent Smoke/CC assassin, but no longer compulsory when cheaper Cameronians can fill much of the job. | TA S3E38 (~9m) actively compares McMurrough/Cameronians; Ryanj4043. |
| **Cateran** | Cheap concealed sniper pressure; Wallace converts its normal Irregular Order. | Ryanj4043 and Caledonia guide. |
| **Wulver AP Spitfire** | Solo or linked midrange gun capable of independent offense. Full Wulver team only when multiple assault bodies serve the plan. | Ryanj4043; Caledonia guide. |
| **Beasthunter FTO 9pt; Denma 12pt** | Highly efficient defensive/trading utility; Denma provides a native Regular Order. **Beasthunter FTO** is the eligible Fireteam option, not every Beasthunter loadout. | Caledonia guide synthesizes reviewed current options; current chart. |

**Conditional avoids:** **Premium Wulver Core / multiple expensive assault pieces solving the same job** when scoring/recovery are thin; **Wallace with few Irregulars**, where 8pt Volunteer or Mormaer LT may fit better; **risking Wallace for a normal trade** that collapses the economy.

**Historical correction:** old material's **Isobel CoC** advice does not match current N5.3 profiles; she currently has standard/Hacker options, **no Chain of Command**. Ryanj4043's transcript and older discussion may also describe rules/profiles differently; current roster wins.

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

#### 5. Caledonian Highlander Army (CHA)

| Weak, niche or redundant purchase | Why the buying case is weak or conditional | Miniature decision |
|---|---|---|
| **Wallace in a mostly Regular army** | **Direct/contested:** [Ryanj4043 Caledonia](https://www.youtube.com/watch?v=iyKGgFUA1JA) says he is *optional*; best when converting substantial **Galwegian, Cameronian, McMurrough and Cateran** irregular economy. His death also imperils that plan. | **Proxy/test first** if not already committed to a warband-heavy army. A Wallace-centric army is valid; not an all-profile avoid. |
| **McMurrough as a compulsory second expensive warband** | **Direct comparative role:** current **18pt Cameronians** already supply fast Smoke/CC/disruption; McMurrough's individual damage/tools have a use if that extra capability matters. | **Proxy before buying** if you already own enough Cameronians or equivalent Dog-Warriors. **Not bad**, just rarely a mandatory *additional* purchase. |
| **Full Wulver Core / duplicate Wulvers and other assault HI** | **Recorded architecture warning:** premium attack link with overlapping close guns competes with **Grey + cheap Volunteers, Uxía/SAS** scoring and Cateran/Traktor support. One Wulver Spitfire can still be excellent. | **Proxy extras; one useful Wulver first** if this is your chosen attack platform. Don't buy AVA5 Wulvers just to have a full team. |
| **Isobel McGregor bought as Chain of Command** | **Rules correction:** **Isobel has no CoC in current N5.3**, despite older advice; her standard/Hacker and Wildcard/support ability are real. | **Skip purchase motivated by nonexistent CoC**. **Proxy a model for the actual Hacker/utility role** and buy only if it recurs. |
| **Armand Le Muet / second Cateran sniper in an already ARO-heavy list** | **Inference:** camouflaged long-range snipers are legitimate but may duplicate **Cateran + Highlander Grey/Mormaer**; Armand's skills differ from a cheap Cateran. A mission with strong long firing lanes may reward the premium model. | **Proxy the extra sniper** rather than purchase to complete all sniper choices. **Do not blacklist a first Cateran.** |
| **Wardriver / expensive Isobel hacking pocket with no network or anti-heavy plan** | **Conditional from [Caledonia guide](../../notes/factions/caledonia.md):** useful surprise anti-tech/mission option, but many opponents will have better Repeaters/hackers; hacker points/SWC compete with nonhackable mission actions. | **Proxy first**, not a forced inclusion. In particular, **Wardriver and Isobel do not both become mandatory** just because CHA has limited hacking. |
| **Traktor Guided bought as a primary damage source; 112 motorized / extra generic support** | **Conditional:** Traktor **Baggage** provides cheap Order/reload, while Guided needs effective FO/Targeted routes; a mobile Doctor may be worthwhile when the army's best models are racing forward. | **Avoid only the default Guided strategy**. Proxy a specialty support variant if necessary; do not skip useful Traktor Baggage/112 roles. |
| **Cadin, Denma, extra Galwegians or extra Cameronians only to max AVA** | **Inference:** combat-capable characters and cheap warbands are attractive, but 15-trooper slots and early deaths can leave too little objective work. **Denma is Regular**; Galwegians/Cameronians are not automatically Regular without Wallace's actual rule. | **Proxy the extra character/warband body** and buy after the third or fourth proves useful. Prioritize the **Uxía/SAS** mission shell over a collection of redundant CC fighters. |

**Sources:** [TA Caledonia](https://open.spotify.com/episode/4WgaVJBlbSm3wHIsBPPsWb), [Ryanj4043](https://www.youtube.com/watch?v=iyKGgFUA1JA), [Caledonia guide](../../notes/factions/caledonia.md), [current roster](caledonian-highlander-army.md). **Do not classify Uxía, SAS, a cheap Cameronian, Galwegian, or one effective Grey/Mormaer gun as whole-unit skips.**

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
