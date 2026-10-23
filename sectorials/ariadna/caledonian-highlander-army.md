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
