---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 503
sectorial_slug: bakunin
sectorial_name: Bakunin
parent_faction: Nomads
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Bakunin roster, standard loadouts, canonical Fireteam chart, and reverse Fireteam index. Vortex Spec-Ops and Nomads Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# Bakunin

## Overview and provenance

Repository-native reference for **Bakunin** roster, profiles, points/SWC, AVA, and Fireteam access.

For concise transcript-reviewed tactical analysis, explicit disagreements, Fireteam-building guidance, **Stigmata/Lizard TAGs, Go-Pod vehicle and REM choices**, see [Bakunin — N5.3 Tactical and List-Building Guide](../../notes/factions/bakunin.md). This file remains the authoritative profile and Fireteam reference.

Sources used:

- Army-derived Bakunin source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **48-unit standard Bakunin roster** and the complete Bakunin `fireteamChart` in the pinned Army source.
- `Vortex Spec-Ops` and `Nomads Team-Ops` are optional game-mode content and are listed separately.
- Soldier of Fortune / generic mercenary-catalog entries whose source faction list is empty are excluded from the base roster.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name by itself.
- Parenthetical Army-chart comments such as `(Moderator)`, `(Reverend)`, `(Observance)`, and `(Riot Grrl)` are preserved as source equivalence/context labels; they are not silently expanded into restrictions beyond the chart row.
- Structured `required: true` rows in the Reverend, Observance, and Armored teams are preserved as required-choice sets; this reference does not reinterpret them as requiring every marked unit type simultaneously.
- FTO/profile restrictions are preserved: Vostok Wildcard access is FTO-only; Fiddler joins Riot Grrls only through the FTO profile; Zellenkrieger joins Riot Grrls only through the FTO profile; Zoe and Π-Well join Moderators through their FTO combination; both Tsyklon selectable profiles are FTO profiles.
- Linked Reinforcement army ID: **599**. Reinforcement Fireteam rows are not merged into the main chart here.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Bakunin |
| Parent faction | Nomads |
| Army ID | 503 |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 48 |
| Optional-mode units | Vortex Spec-Ops; Nomads Team-Ops |
| Reinforcement roster | Army ID `599` |
| Fireteam limits | Core 1; Haris 1; Duo unlimited |
| Fireteam chart | yes |

## Roster index

`AVA 255` is Army's Total/unlimited sentinel.

| Unit | ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| Vertigo Zonds | 410 | 1 | REM | Regular | — |
| Bran do Castro | 428 | 1 | SK | Regular | — |
| Reaktion Zonds | 409 | 1 | REM | Regular | — |
| Reverend Moiras | 396 | 5 | MI | Regular | Reverend; Observance |
| Extreme Zellenkrieger | 1748 | 1 | WB | Irregular + Impetuous | — |
| Meteor Zonds | 411 | 1 | REM | Regular | — |
| Zondbots | 425 | 4 | REM | Peripheral | — |
| Die Morlock Gruppe | 403 | 255 | WB | Irregular + Impetuous | Taskmasters |
| Salyut Zonds | 426 | 2 | REM | Regular | — |
| Denma Connolly | 1749 | 1 | WB | Regular + Impetuous | Taskmasters |
| Avicenna | 491 | 1 | LI | Regular | Moderators; Riot Grrls |
| Go-Pod | 1854 | 1 | VH | Regular | — |
| Vostok Sputniks | 1544 | 2 | REM | Regular | Wildcard, FTO profiles only |
| Mother Healer Agatha Wabara | 1608 | 1 | MI | Regular | Reverend; Observance |
| Fiddler | 1564 | 1 | LI | Regular | Riot Grrls, FTO profile only |
| Wolfgang Amadeus Wolff | 1555 | 1 | WB | Regular | Wildcard; source comment `(Moderator)` |
| Daktaris | 405 | 1 | LI | Regular | — |
| Moderators from Bakunin | 414 | 255 | LI | Regular | Moderators |
| Prowlers | 417 | 3 | MI | Regular | — |
| Initiated Observants | 1604 | 2 | MI | Regular | — |
| Orphans of the Observance | 1601 | 3 | MI | Regular | Moderators; Observance; Armored |
| Clockmakers | 406 | 2 | LI | Regular | Moderators |
| Zoe & Π-Well | 413 | 1 | LI + REM | Regular | Moderators, FTO combination only |
| Sin-Eater Observants | 418 | 3 | MI | Regular | — |
| Reverend Custodiers | 416 | 3 | MI | Regular | Reverend |
| Taskmasters | 781 | 3 | HI | Regular | Riot Grrls; Taskmasters |
| Daemonist Observant | 1606 | 1 | HI | Regular | — |
| Reverend Cenobites | 1603 | 3 | HI | Regular | Reverend; Observance |
| Tsyklon Sputniks | 423 | 2 | REM | Regular | Wildcard; both profiles FTO |
| Reverend Healers | 397 | 3 | MI | Regular | Reverend |
| Zeros | 401 | 3 | SK | Regular | — |
| Transductor Zonds | 412 | 2 | REM | Regular | — |
| Redsky Crew Marspiders | 1760 | 2 | LI | Regular | Armored |
| Uhahu | 1071 | 1 | LI | Regular | Riot Grrls |
| Casino Security Rounders | 1762 | 2 | LI | Regular | Moderators |
| Stigmata of the Observance | 1605 | 2 | TAG | Regular + Tactical Awareness | Armored |
| Robin Hook | 1607 | 1 | HI | Regular | Riot Grrls; Armored |
| Zellenkrieger | 1747 | 2 | WB | Irregular + Impetuous | Taskmasters; Riot Grrls FTO-only |
| Warcors | 50 | 1 | LI | Irregular | — |
| Mobile Brigada | 382 | 1 | HI | Regular | Armored |
| Corregidor Alguaciles | 296 | 2 | LI | Regular | Moderators |
| Lizard Squadron | 399 | 1 | TAG | Regular + Tactical Awareness | Armored |
| Bakunin Überfallkommando | 422 | 3 | WB | Irregular + Impetuous | — |
| Cassandra Kusanagi | 429 | 1 | MI | Regular | Reverend; Observance |
| TAG-Treiber | 1853 | 1 | LI | Regular | Moderators |
| Riot Grrls | 431 | 5 | HI | Regular | Moderators; Riot Grrls |
| Penitent Observants | 1602 | 3 | HI | Regular | Observance |
| Stempler Zonds | 408 | 2 | REM | Regular | —; FTO-labelled profile has no Bakunin Fireteam-chart row |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Vortex Spec-Ops | 1917 | Spec-Ops | Moderators Fireteam row, max 1 when Spec-Ops mode is in use |
| Nomads Team-Ops | 1931 | Team-Ops | No ordinary Bakunin Fireteam row |

## Unit details

### Vertigo Zonds

**ID 410 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage, BS Attack (Guided).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CCW (-3) | — |

### Bran do Castro, Triple Zero

**ID 428 · AVA 1 · SK** — `MOV 15-5 | CC 22 | BS 11 | PH 13 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Martial Arts L2, Camouflage, Surprise Attack (-3), Mimetism (-3), Infiltration (PH=16), Berserk, Courage, Specialist Operative, Stealth, Super-Jump, Terrain (Total), Immunity (Shock/BTS).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 27 | 0 | Boarding Shotgun, Boarding Pistol, DA CCW (PS 6) | — |
| 2 | 27 | 0 | SMG, E/M Grenades, Boarding Pistol, DA CCW (PS 6) | — |

### Reaktion Zonds

**ID 409 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage, Total Reaction, Climbing Plus, 360º Visor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 1 | HMG, PARA CCW (-3) | — |
| 2 | 19 | 0 | Thunderbolt (+1B), PARA CCW (-3) | — |

### Reverend Moiras

**ID 396 · AVA 5 · MI** — `MOV 10-10 | CC 19 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 2`. Mimetism (-6), Number 2, Stealth, NCO, Religious Troop, Immunity (Shock), Sixth Sense.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4 | 33 | 1.5 | HMG, Zapper, Pistol, Shock CCW | Reverend required-choice max 5; Observance max 1 |
| 5 | 31 | 1.5 | MULTI Sniper Rifle, Zapper, Pistol, Shock CCW | same |
| 6 | 29 | 1 | MULTI Rifle, E/M Grenade Launcher, Zapper, Pistol, Shock CCW | same |
| 8 | 26 | 0 | MULTI Rifle, Zapper, Pistol, Shock CCW; Lieutenant, Specialist Operative | same |
| 9 | 28 | 0 | MULTI Rifle, Zapper, Pistol, Shock CCW; Specialist Operative | same |

### Extreme Zellenkrieger

**ID 1748 · AVA 1 · WB** — `MOV 10-10 | CC 23 | BS 10 | PH 15 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 5`. CC Attack (-3), Berserk, Courage, Dodge (+5), Natural Born Warrior, Immunity (BTS), No Cover, MetaChemistry (ReRoll), Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 11 | 0 | Light Shotgun, Smoke Grenades, Heavy Pistol, DA CCW (PS 5) | — |
| 2 | 11 | 0 | Pulzar, Smoke Grenades, Heavy Pistol (+1B), DA CCW (PS 5) | — |

### Meteor Zonds

**ID 411 · AVA 1 · REM** — `MOV 15-10 | CC 14 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 6 | W 1 | S 3`. ECM: Hacker (-3), Repeater, Remote Presence, Triangulated Fire, Courage, Forward Observer, Parachutist, Sensor, Combat Jump, Super-Jump (Jet Propulsion).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | Light Shotgun, E/M Carbine, Flash Pulse, PARA CCW (-6) | — |
| 2 | 19 | 0 | Boarding Shotgun, Flash Pulse, PARA CCW (-6) | — |

### Zondbots

**ID 425 · AVA 4 · REM** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Peripheral (Servant), Remote Presence, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | PARA CCW (-3); Peripheral, no Order | — |

### Die Morlock Gruppe

**ID 403 · AVA 255 (Total) · WB** — `MOV 10-10 | CC 23 | BS 11 | PH 13 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Martial Arts L2, Courage, Dodge (+2.5), MetaChemistry, No Cover, Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 6 | 0 | Chain Rifle, Smoke Grenades, Assault Pistol, AP CCW (PS 6) | Taskmasters max 2 |
| 2 | 6 | 0 | Chain Rifle, Smoke Grenades, Kobra Pistol, DA CCW (PS 6) | same |
| 3 | 6 | 0 | Chain Rifle, Smoke Grenades, Kobra Pistol, E/M CCW (PS 6) | same |
| 4 | 9 | 0 | Boarding Shotgun, Smoke Grenades, Kobra Pistol, DA CCW (PS 6) | same |
| 6 | 12 | 0 | Combi Rifle, Smoke Grenade Launcher, Kobra Pistol, DA CCW (PS 6) | same |

### Salyut Zonds

**ID 426 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 4`. Baggage, Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | PARA CCW (-3); Deactivator, Repeater | — |
| 2 | 14 | 0.5 | PARA CCW (-3); EVO Hacking Device, Hacker | — |
| 3 | 17 | 0 | Combi Rifle, PARA CCW (-3); Repeater, Total Reaction | — |

### Denma Connolly

**ID 1749 · AVA 1 · WB** — `MOV 15-5 | CC 23 | BS 11 | PH 14 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`. Martial Arts L1, Berserk, Courage, Dodge (+5), Natural Born Warrior, MetaChemistry (ReRoll), No Cover, Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 12 | 0 | Chain Rifle (+1B), Smoke Grenades, Heavy Pistol (+1B), AP+DA CCW (PS 6) | Taskmasters max 1 |

### Avicenna, Mercenary Doctor

**ID 491 · AVA 1 · LI** — `MOV 15-5 | CC 16 | BS 11 | PH 11 | WIP 15 | ARM 2 | BTS 3 | W 1 | S 2`. Doctor (+3), Courage, Immunity (ARM), No Wound Incapacitation, MediKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 28 | 0 | Combi Rifle, Flash Pulse, Pistol, CCW, Nanopulser | Moderators max 1; Riot Grrls max 1 |

### Go-Pod

**ID 1854 · AVA 1 · VH** — `MOV 20-5 | CC — | BS 13 | PH 13 | WIP 13 | ARM 2 | BTS 6 | W 2 | S 7`. Aerial, Courage, Mimetism (-3), No Cover, Super-Jump, Tech-Recovery; includes a Go-Bot peripheral.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 0 | MULTI Rifle, E/Mitter; Go-Bot included | — |
| 2 | 32 | 1.5 | Heavy Rocket Launcher, AP SMG; BS Attack (SR-1); Go-Bot included | — |

### Vostok Sputniks

**ID 1544 · AVA 2 · REM** — `MOV 15-10 | CC 14 | BS 12 | PH 10 | WIP 13 | ARM 3 | BTS 6 | W 2 | S 4`. Remote Presence, Courage, Mimetism (-6), Climbing Plus, Immunity (AP).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4 | 38 | 0 | Mk12, Light Shotgun, PARA CCW (-3); Repeater | — |
| 5 | 35 | 0 | **VOSTOK FTO**; Mk12, Light Shotgun, PARA CCW (-3) | Wildcard max 2 |
| 6 | 37 | 1 | Spitfire, PARA CCW (-3); Repeater | — |
| 7 | 34 | 1 | **VOSTOK FTO**; Spitfire, PARA CCW (-3) | Wildcard max 2 |

### Mother Healer Agatha Wabara

**ID 1608 · AVA 1 · MI** — `MOV 15-5 | CC 23 | BS 13 | PH 12 | WIP 14 | ARM 3 | BTS 6 | W 1 | S 2`. Martial Arts L2, Berserk, Frenzy, Mimetism (-6), Stealth, Religious Troop, Dodge (+5), Immunity (Shock), Doctor (2W), MediKit (+1B).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 31 | 0 | Breaker Combi Rifle, Pulzar (+1B), Pistol, EXP CCW (PS 5) | Reverend max 1; Observance max 1 |
| 2 | 31 | 0 | Vulkan Shotgun, Pulzar (+1B), Pistol, EXP CCW (PS 5) | same |

### Fiddler

**ID 1564 · AVA 1 · LI** — `MOV 15-10 | CC 18 | BS 12 | PH 12 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Engineer, No Wound Incapacitation, CC Attack (+1B), Dodge bonuses, GizmoKit. Non-FTO profiles include JackBots.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 29 | 0 | **FIDDLER FTO**; Contender (+1B), Drop Bears, D-Charges, Breaker Pistol, PARA CCW (-3); Super-Jump | Riot Grrls max 1 |
| 2 | 36 | 0 | Same weapons; Climbing Plus; includes 1 JackBot | — |
| 3 | 43 | 0 | Same weapons; Climbing Plus; includes 2 JackBots | — |

### Wolfgang Amadeus Wolff

**ID 1555 · AVA 1 · WB** — `MOV 15-5 | CC 22 | BS 12 | PH 14 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`. Martial Arts L3, Berserk, Courage, Climbing Plus, Terrain (Zero-G), Frenzy, Immunity (ARM), BS Attack (Continuous Damage).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 0 | MULTI Rifle (+1SD), Chain-colt, E/M Grenades (+1SD), Heavy Pistol, PARA CCW (-6), DA CCW (PS 4) | Wildcard max 1; counts as Moderator per source comment |

### Daktaris

**ID 405 · AVA 1 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Doctor, MediKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Pistol, CCW | — |

### Moderators from Bakunin

**ID 414 · AVA 255 (Total) · LI** — `MOV 10-10 | CC 18 | BS 10 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`. Immunity (Shock).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 9 | 0 | Combi Rifle, Pistol, PARA CCW (-6) | Moderators 1–5 |
| 2 | 15 | 0.5 | Spitfire, Pistol, PARA CCW (-6) | same |
| 5 | 10 | 0 | Combi Rifle, Pitcher, Pistol, PARA CCW (-6) | same |
| 6 | 14 | 0.5 | Combi Rifle, Pistol, PARA CCW (-6); Hacking Device, Hacker | same |
| 8 | 11 | 0 | Combi Rifle, Pistol, PARA CCW (-6); MediKit, Paramedic | same |
| 9 | 9 | 0 | Combi Rifle, Pistol, PARA CCW (-6); Lieutenant | same |
| 10 | 9 | 0 | Boarding Shotgun, Pistol, PARA CCW (-6), E/M Carbine | same |
| 11 | 11 | 0 | Combi Rifle, Pistol, PARA CCW (-6); Commlink (+1), Specialist Operative | same |

### Prowlers

**ID 417 · AVA 3 · MI** — `MOV 10-10 | CC 16 | BS 12 | PH 11 | WIP 14 | ARM 2 | BTS 6 | W 1 | S 2`. Camouflage, Hidden Deployment, Surprise Attack (-3), Infiltration, Mimetism (-3), Specialist Operative, Stealth, Terrain (Total), Immunity (ARM).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 34 | 0 | MULTI Rifle, Adhesive Launcher Rifle, Disco Baller, Silenced Pistol, CCW | — |
| 4 | 36 | 1.5 | Spitfire, Nanopulser, D-Charges, Silenced Pistol, CCW | — |
| 5 | 30 | 0 | Boarding Shotgun, Nanopulser, D-Charges, Silenced Pistol, CCW; KHD, Hacker | — |

### Initiated Observants

**ID 1604 · AVA 2 · MI** — `MOV 10-10 | CC 18 | BS 12 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Mimetism (-3), Stealth, Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Boarding Shotgun, Boarding Pistol, CCW; Parachutist | — |
| 2 | 22 | 0 | Boarding Shotgun, D-Charges, Boarding Pistol, CCW; KHD, Hacker, Parachutist | — |
| 3 | 18 | 0 | Boarding Shotgun, D-Charges, Breaker Pistol (+1B), CCW; Camouflage (1 Use), Surprise Attack (-3), Infiltration | — |
| 4 | 18 | 0 | SMG, Breaker Pistol (+1B), CCW; Deployable Repeater, Camouflage (1 Use), Surprise Attack (-3), Infiltration, Minelayer | — |

### Orphans of the Observance

**ID 1601 · AVA 3 · MI** — `MOV 10-10 | CC 18 | BS 12 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Mimetism (-3), Stealth, Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 13 | 0 | SMG, Boarding Pistol, CCW | Moderators max 1; Observance required-choice max 3; Armored max 1 |
| 2 | 17 | 0 | SMG, D-Charges, Boarding Pistol, CCW; Engineer, GizmoKit | same |
| 3 | 21 | 0 | SMG, E/M Mine, D-Charges, Boarding Pistol, CCW; Repeater, Engineer, GizmoKit | same |
| 4 | 25 | 0 | MULTI Marksman Rifle, Boarding Pistol, CCW; MSV2 | same |

### Clockmakers

**ID 406 · AVA 2 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 15 | ARM 1 | BTS 3 | W 1 | S 2`. Engineer, Deactivator, GizmoKit (+1B).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 18 | 0 | Combi Rifle, D-Charges, Pistol, CCW | Moderators max 2; counts as Moderator per source comment |
| 2 | 19 | 0 | Same; Deployable Cover | same |
| 3 | 21 | 0 | Combi Rifle, D-Charges, Armed Turret (Combi Rifle), Pistol, CCW | same |

### Zoe & Π-Well

**ID 413 · AVA 1 · LI + REM**. **Zoe:** `MOV 10-10 | CC 16 | BS 11 | PH 10 | WIP 15 | ARM 1 | BTS 3 | W 1 | S 2`; Engineer, Hacking Device (Zero Pain upgrade), Deactivator, GizmoKit (+1B), Immunity (Shock/BTS). **Π-Well FTO:** `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`; Repeater, ECM: Hacker (-3), Remote Presence, Triangulated Fire, Mimetism (-6), Forward Observer, Sensor.

The selectable Bakunin Army options are the two FTO combinations below. The source also stores disabled constituent/synchronized Π-Well rows, but they are not separate selectable top-level Bakunin options.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 45 | 0.5 | **ZOE FTO**: Combi Rifle, D-Charges, Pistol, PARA CCW (-3), Hacker + **Π-WELL FTO**: Combi Rifle, Flash Pulse (+1B), Pitcher, PARA CCW (-6) | Moderators: Zoe FTO max 1 and Π-Well FTO max 1 |
| 2 | 42 | 0.5 | **ZOE FTO-2**: Boarding Shotgun, D-Charges, Pistol, PARA CCW (-3), Hacker + same Π-WELL FTO | same |

### Sin-Eater Observants

**ID 418 · AVA 3 · MI** — `MOV 10-10 | CC 14 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 2`. Mimetism (-3), Neurocinetics, Religious Troop, Immunity (Shock).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 28 | 1.5 | HMG, Pistol, CCW | — |
| 2 | 26 | 1.5 | MULTI Sniper Rifle, Pistol, CCW | — |
| 3 | 25 | 0 | Mk12, Pistol, CCW | — |
| 5 | 28 | 1 | MULTI Sniper Rifle, Pistol, CCW; Marksmanship | — |

### Reverend Custodiers

**ID 416 · AVA 3 · MI** — `MOV 10-10 | CC 14 | BS 12 | PH 11 | WIP 14 | ARM 3 | BTS 3 | W 1 | S 2`. Mimetism (-6), Stealth, Religious Troop, Immunity (Shock).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 26 | 0.5 | Combi Rifle, Pitcher, Pistol, CCW; Hacking Device with Carbonite (+1B), Hacker | Reverend required-choice max 3 |
| 3 | 24 | 0.5 | Boarding Shotgun, Pistol, CCW; Hacking Device Plus, Hacker | same |
| 4 | 28 | 0.5 | Combi Rifle, Pitcher, Pistol, CCW; Hacking Device Plus, Hacker | same |
| 5 | 28 | 0.5 | Same as Opt 4; Lieutenant | same |
| 6 | 24 | 0 | Combi Rifle, Pitcher, Pistol, CCW; KHD, Hacker | same |

### Taskmasters

**ID 781 · AVA 3 · HI** — `MOV 10-10 | CC 22 | BS 13 | PH 13 | WIP 13 | ARM 5 | BTS 6 | W 2 | S 5`. Martial Arts L1, Courage, Dodge (+2.5), Minelayer, Stealth, FT Master (Morlocks, Zellenkriegers, Connolly).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 40 | 1.5 | HMG, Shock Mine, Heavy Pistol, DA CCW (PS 6) | Riot Grrls max 3; Taskmasters 1–3 |
| 3 | 39 | 1 | Red Fury, Pulzar, CrazyKoala, Heavy Pistol, DA CCW (PS 6); TinBot Firewall (-3) | same |
| 4 | 34 | 1.5 | Heavy Rocket Launcher, Light Shotgun, CrazyKoala, Heavy Pistol, DA CCW (PS 6) | same |
| 5 | 44 | 1 | Red Fury, Pulzar, CrazyKoala, Heavy Pistol, DA CCW (PS 6); TinBot Firewall (-3), Strategic Deployment | same |
| 6 | 39 | 1 | Red Fury, Pulzar, CrazyKoala, Heavy Pistol, DA CCW (PS 6); TinBot Firewall (-3), Lieutenant | same |

### Daemonist Observant

**ID 1606 · AVA 1 · HI** — `MOV 10-10 | CC 22 | BS 11 | PH 13 | WIP 14 | ARM 3 | BTS 3 | W 2 | S 4`. Martial Arts L1, Counterintelligence, Guard, Decoy (1), Religious Troop, Biometric Visor, ECM: Hacker (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 32 | 0 | Vulkan Shotgun, Boarding Pistol (+1B), DA CCW (PS 6) | — |
| 2 | 36 | 0 | Same; Lieutenant (+1 Order) | — |

### Reverend Cenobites

**ID 1603 · AVA 3 · HI** — `MOV 15-5 | CC 22 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`. Martial Arts L3, Frenzy, Mimetism (-6), Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 20 | 0 | Chain Rifle (+1B), Flash Pulse, Heavy Pistol (+1B), DA CCW (PS 6) | Reverend max 2; Observance max 1 |
| 2 | 20 | 0 | Light Shotgun, Heavy Pistol, DA CCW (PS 6) | same |
| 4 | 26 | 1.5 | Heavy Rocket Launcher, Light Shotgun, Heavy Pistol, DA CCW (PS 6) | same |

### Tsyklon Sputniks

**ID 423 · AVA 2 · REM** — `MOV 15-10 | CC 14 | BS 12 | PH 10 | WIP 13 | ARM 3 | BTS 6 | W 1 | S 4`. Repeater, 360º Visor, X-Visor, Remote Presence, Courage, Climbing Plus.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 1 | **TSYKLON FTO**; Spitfire, Chain Rifle, Pitcher, PARA CCW (-6) | Wildcard max 2 |
| 2 | 29 | 1 | **TSYKLON FTO**; Feuerbach, Chain Rifle, Pitcher, PARA CCW (-6) | Wildcard max 2 |

### Reverend Healers

**ID 397 · AVA 3 · MI** — `MOV 10-10 | CC 22 | BS 12 | PH 12 | WIP 14 | ARM 3 | BTS 3 | W 1 | S 2`. Doctor, Mimetism (-6), Stealth, Religious Troop, Immunity (Shock), MediKit (+1B).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 31 | 0 | MULTI Rifle, Nanopulser, Pistol, Shock CCW | Reverend required-choice max 3 |
| 3 | 29 | 0 | Boarding Shotgun, E/Mitter, Pistol, Shock CCW | same |

### Zeros

**ID 401 · AVA 3 · SK** — `MOV 10-10 | CC 15 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Camouflage, Surprise Attack (-3), Infiltration, Mimetism (-3), Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Combi Rifle, Shock Mine, Pistol, CCW | — |
| 2 | 21 | 1.5 | MULTI Sniper Rifle, Shock Mine, Pistol, CCW | — |
| 3 | 17 | 0 | Boarding Shotgun, Shock Mine, PARA Mine, Pistol, CCW | — |
| 4 | 20 | 0 | Combi Rifle, E/M Mine, Pistol, CCW; Deployable Repeater | — |
| 5 | 24 | 0.5 | Combi Rifle, Shock Mine, Pistol, CCW; Hacking Device, Hacker | — |
| 6 | 22 | 0 | Combi Rifle, Shock Mine, Pistol, CCW; KHD, Hacker | — |
| 7 | 18 | 0.5 | Boarding Shotgun, Shock Mine, PARA Mine, Pistol, CCW; Minelayer | — |
| 8 | 20 | 0 | Combi Rifle, Shock Mine, Flash Pulse, Pistol, CCW; Forward Observer | — |

### Transductor Zonds

**ID 412 · AVA 2 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Remote Presence, Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) | — |

### Redsky Crew Marspiders

**ID 1760 · AVA 2 · LI** — `MOV 15-5 | CC 23 | BS 11 | PH 13 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. 360º Visor, GizmoKit, Martial Arts L1, CC Attack (+1B), Courage, Dodge (+2.5), Terrain (Zero-G), Climbing Plus, Stealth.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 18 | 0 | Heavy Flamethrower (+1B), Flash Pulse, Panzerfaust, Assault Pistol, DA CCW (PS 7) | Armored max 1 |
| 2 | 18 | 0 | Heavy Flamethrower (+1B), Flash Pulse, Grenades (+1B), Assault Pistol, DA CCW (PS 7) | same |
| 3 | 22 | 0 | Opt 1 weapons; Engineer | same |
| 4 | 19 | 0 | Heavy Flamethrower (+1B), Flash Pulse, Assault Pistol, DA CCW (PS 7); MediKit, Paramedic | same |

### Uhahu, Hacker for Hire

**ID 1071 · AVA 1 · LI** — `MOV 10-10 | CC 12 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Courage, No Wound Incapacitation, Immunity (Shock), Hacking Device Plus with Total Control (SR-2).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0.5 | Pitcher, D-Charges, Assault Pistol, CCW; Hacker | Riot Grrls max 1 |

### Casino Security Rounders

**ID 1762 · AVA 2 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Biometric Visor, MSV1, Marksmanship, NCO, Terrain (Zero-G).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 17 | 0 | Boarding Shotgun, Boarding Pistol, CCW | Moderators max 1; counts as Moderator per source comment |
| 2 | 24 | 0.5 | MULTI Marksman Rifle, Boarding Pistol, CCW | same |
| 3 | 26 | 1 | Red Fury, Boarding Pistol, CCW | same |
| 4 | 21 | 0.5 | SMG, Boarding Pistol, CCW; Hacking Device with Trinity upgrade, Hacker | same |

### Stigmata of the Observance

**ID 1605 · AVA 2 · TAG** — `MOV 15-10 | CC 20 | BS 13 | PH 14 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`. Hacking Device with Carbonite (SR-2), ECM: Guided (-6), ECM: Hacker (-3), BS Attack (SR-1), Tactical Awareness, Religious Troop, Remote Presence.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 56 | 1.5 | Heavy Flamethrower (+1B), Heavy Rocket Launcher (+1B), E/M CCW (PS 6); Hacker | Armored required-choice max 2 |

### Robin Hook, outlaw AI

**ID 1607 · AVA 1 · HI** — Full Power `MOV 15-5 | CC 13 | BS 11 | PH 11 | WIP 13 | ARM 1 | BTS 3 | W 2 | S 2`; Battle-Ravaged `CC 9 | PH 10 | ARM 0`. Remote Presence, Booty, Courage, Forward Deployment (+10), Stealth, Climbing Plus, Immunity (Enhanced), Transmutation, Super-Jump.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 20 | 0 | E/Mitter, Light Shotgun, Tactical Bow (+3 BS), Drop Bears, Heavy Pistol (+1B), PARA CCW (-9) | Riot Grrls max 1; Armored max 1 |

### Zellenkrieger

**ID 1747 · AVA 2 · WB** — `MOV 10-10 | CC 23 | BS 10 | PH 13 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`. CC Attack (-3), Berserk, Courage, Dodge (+2.5), Natural Born Warrior, MetaChemistry (ReRoll), No Cover, Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | Light Shotgun, Smoke Grenades, Heavy Pistol, DA CCW (PS 7) | Taskmasters max 1 |
| 2 | 8 | 0 | Pulzar, Smoke Grenades, Heavy Pistol (+1B), DA CCW (PS 7) | Taskmasters max 1 |
| 3 | 8 | 0 | **ZELLENKRIEGER FTO**; Pulzar (+1B), Heavy Pistol (+1B), DA CCW (PS 7) | Taskmasters max 1; Riot Grrls max 1 |

### Warcors

**ID 50 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Journalist.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor | — |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); Sixth Sense | — |

### Mobile Brigada

**ID 382 · AVA 1 · HI** — `MOV 15-5 | CC 18 | BS 13 | PH 13 | WIP 13 | ARM 5 | BTS 3 | W 2 | S 2`. Courage, Jump (7.5), 360º Visor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 0 | MULTI Rifle, Boarding Pistol (+1B), CCW; TinBot Firewall (-6) | Armored max 1 |
| 2 | 38 | 1.5 | HMG, Boarding Pistol (+1B), CCW | same |
| 3 | 27 | 0 | Boarding Shotgun, Boarding Pistol (+1B), CCW | same |
| 5 | 35 | 1.5 | Missile Launcher, Boarding Pistol (+1B), CCW | same |
| 9 | 36 | 0.5 | Combi Rifle, D-Charges, Boarding Pistol (+1B), CCW; Hacking Device, TinBot Firewall (-6), Hacker | same |
| 10 | 33 | 0 | MULTI Rifle, Boarding Pistol (+1B), CCW; TinBot Firewall (-6), Lieutenant | same |
| 11 | 27 | 0 | Boarding Shotgun, Boarding Pistol (+1B), CCW; Lieutenant | same |

### Corregidor Alguaciles

**ID 296 · AVA 2 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 10 | 0 | Combi Rifle, Pistol, CCW | Moderators max 2 |
| 2 | 18 | 1 | HMG, Pistol, CCW | same |
| 5 | 15 | 1.5 | Missile Launcher, Pistol, CCW | same |
| 6 | 15 | 0.5 | Combi Rifle, Pistol, CCW; Hacking Device, Hacker | same |
| 8 | 12 | 0 | Combi Rifle, Flash Pulse, Pistol, CCW; Deployable Repeater, Forward Observer | same |
| 9 | 12 | 0 | Combi Rifle, Pistol, CCW; MediKit, Paramedic | same |
| 10 | 10 | 0 | Combi Rifle, Pistol, CCW; Lieutenant | same |
| 11 | 12 | 0 | Combi Rifle, Pistol, CCW; Commlink (+1), Specialist Operative | same |

### Lizard Squadron

**ID 399 · AVA 1 · TAG** — `MOV 15-10 | CC 17 | BS 14 | PH 17 | WIP 13 | ARM 8 | BTS 6 | W 3 | S 7`. ECM: Guided (-6), ECM: Hacker (-3), Repeater, Tactical Awareness; includes a RobbyBot attendant.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 65 | 1.5 | MULTI HMG, Grenade Launcher, E/M Grenade Launcher, CCW (PS 5) | Armored required-choice max 1 |
| 2 | 64 | 1.5 | MULTI HMG, Heavy Flamethrower, CCW (PS 5) | same |
| 3 | 60 | 1.5 | AP Spitfire, Grenade Launcher, E/M Grenade Launcher, E/M Mine, CCW (PS 5); BS Attack (Shock) | same |

### Bakunin Überfallkommando

**ID 422 · AVA 3 · WB** — **Chimera:** `MOV 15-10 | CC 24 | BS 11 | PH 13 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`; CC Attack (-3), Dodge (+2.5), Natural Born Warrior, Climbing Plus, Impetuous, Immunity (Enhanced), No Cover. Includes three Pupnik peripherals.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4 | 19 | 0 | Chimera: Combi Rifle, Nanopulser, Eclipse Grenades, Pistol, Viral CCW (PS 6) + 3 Pupniks with DA CCW (PS 7) | — |

### Reverend Superior Cassandra Kusanagi

**ID 429 · AVA 1 · MI** — `MOV 10-10 | CC 20 | BS 14 | PH 12 | WIP 14 | ARM 3 | BTS 3 | W 1 | S 2`. Mimetism (-6), Immunity (Shock), Specialist Operative, Stealth, No Wound Incapacitation, Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 34 | 0 | MULTI Rifle (+1B), E/M Grenade Launcher, Zapper, Pistol, Shock CCW (PS 7) | Reverend max 1; Observance max 1 |
| 2 | 35 | 1.5 | AP Spitfire, Zapper, Pistol, Shock CCW (PS 7) | same |
| 3 | 34 | +1 | Opt 1; Lieutenant | same |
| 4 | 35 | 1.5 | Opt 2; Lieutenant | same |

### TAG-Treiber, NMF TAG Squadrons Support Pilots

**ID 1853 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Specialist Operative, TAGCom (Dodge PH+3 / GizmoKit PH+1).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 10 | 0 | **LIZARD PILOT**; SMG, E/Mitter, Pistol, PARA CCW (-3); GizmoKit | Moderators max 1 |

### Riot Grrls

**ID 431 · AVA 5 · HI** — `MOV 15-5 | CC 17 | BS 13 | PH 13 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`. Frenzy, Dodge (+3), BS Attack (SR-1), Combat Instinct, MSV1.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 3 | 24 | 0 | Boarding Shotgun, Boarding Pistol, CCW; TinBot Firewall (-6) | Moderators max 2; Riot Grrls 1–5 |
| 4 | 29 | 0 | MULTI Rifle, Disco Baller, Boarding Pistol, CCW | same |
| 5 | 30 | 1.5 | Missile Launcher, Boarding Pistol, CCW | same |
| 6 | 31 | 1.5 | Spitfire, Boarding Pistol, CCW | same |
| 7 | 29 | 0 | Combi Rifle, E/Mitter, Boarding Pistol, CCW; Specialist Operative | same |

### Penitent Observants

**ID 1602 · AVA 3 · HI** — `MOV 10-10 | CC 18 | BS 13 | PH 12 | WIP 13 | ARM 5 | BTS 3 | W 2 | S 5`. Mimetism (-3), Religious Troop, Warhorse, ECM: Hacker (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 34 | 1.5 | Red Fury (Continuous Damage), E/Marat, AP Heavy Pistol, CCW | Observance required-choice max 1 |
| 2 | 38 | 1.5 | Red Fury (Continuous Damage), E/M Grenade Launcher (+1B), AP Heavy Pistol, CCW | same |
| 3 | 37 | 1.5 | AP Spitfire, AP Heavy Pistol, CCW; BS Attack (Continuous Damage) | same |

### Stempler Zonds

**ID 408 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Deactivator, Repeater, Remote Presence, Triangulated Fire, Courage, Forward Observer, Sensor, Climbing Plus.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 15 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3) | — |
| 2 | 18 | 0 | Same; Tactical Awareness | — |
| 3 | 17 | 0 | **STEMPLER ZOND FTO**; same weapons; Super-Jump | —; no Bakunin chart row |
| 4 | 22 | 0 | Thunderbolt (+1B), Flash Pulse, PARA CCW (-3); BS 12, Tactical Awareness | — |

## Canonical Fireteam chart

Fireteam limits in the pinned source: **Core 1; Haris 1; Duo unlimited** (`DUO: 256` sentinel).

### Moderators Fireteams

**Types:** Haris, Core

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| MODERATOR | 1 | 5 | no | — |
| ALGUACIL | 0 | 2 | no | — |
| RIOT GRRL | 0 | 2 | no | — |
| CLOCKMAKER | 0 | 2 | no | Moderator |
| ROUNDER | 0 | 1 | no | Moderator |
| ORPHAN | 0 | 1 | no | — |
| TAG-TREIBER | 0 | 1 | no | — |
| AVICENNA | 0 | 1 | no | — |
| ZOE FTO | 0 | 1 | no | FTO combination only |
| Π-WELL FTO | 0 | 1 | no | FTO combination only |
| VORTEX | 0 | 1 | no | Spec-Ops mode only |

### Reverends Fireteams

**Types:** Haris, Core

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| REVEREND MOIRA | 0 | 5 | yes | Reverend |
| REVEREND HEALER | 0 | 3 | yes | Reverend |
| REVEREND CUSTODIER | 0 | 3 | yes | Reverend |
| CENOBITE | 0 | 2 | no | Reverend |
| KUSANAGI | 0 | 1 | no | Reverend |
| MOTHER AGATHA | 0 | 1 | no | Reverend |

The three `required-choice` rows are a required-choice set from the Army chart; they are not interpreted here as requiring one of every row simultaneously.

### Observance Fireteams

**Types:** Haris

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| ORPHAN | 0 | 3 | yes | Observance |
| PENITENT | 0 | 1 | yes | Observance |
| CENOBITE | 0 | 1 | no | Observance |
| REVEREND MOIRA | 0 | 1 | no | — |
| KUSANAGI | 0 | 1 | no | — |
| MOTHER AGATHA | 0 | 1 | no | Observance |

The two `required-choice` rows are a required-choice set from the Army chart; they are not interpreted here as requiring both unit types simultaneously.

### Riot Grrls Fireteams

**Types:** Duo, Haris, Core

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| RIOT GRRL | 1 | 5 | no | — |
| TASKMASTER | 0 | 3 | no | — |
| AVICENNA | 0 | 1 | no | Riot Grrl |
| Fiddler FTO | 0 | 1 | no | Riot Grrl; FTO profile only |
| ZELLENKRIEGER | 0 | 1 | no | FTO profile only |
| UHAHU | 0 | 1 | no | — |
| ROBIN HOOK | 0 | 1 | no | Riot Grrl |

### Taskmasters Fireteams

**Types:** Duo, Haris

| Entry | Min | Max | Required-choice | Note |
|---|---:|---:|---|---|
| TASKMASTER | 1 | 3 | no | — |
| MORLOCK | 0 | 2 | no | — |
| ZELLENKRIEGER | 0 | 1 | no | No chart-level FTO restriction |
| DENMA CONNOLLY | 0 | 1 | no | — |

### Armored Fireteams

**Types:** Duo

| Entry | Min | Max | Required-choice | Note |
|---|---:|---:|---|---|
| STIGMATON | 0 | 2 | yes | — |
| LIZARD | 0 | 1 | yes | — |
| ORPHAN | 0 | 1 | no | — |
| MOBILE BRIGADA | 0 | 1 | no | — |
| MARSPIDER | 0 | 1 | no | — |
| ROBIN HOOK | 0 | 1 | no | — |

The Stigmaton and Lizard `required-choice` rows are a required-choice set from the Army chart; they are not interpreted here as requiring both unit types simultaneously.

### Wildcards

| Entry | Max | Counts as / profile restriction |
|---|---:|---|
| VOSTOK | 2 | FTO profiles only (Opts 5 and 7) |
| TSYKLON FTO | 2 | Both selectable Tsyklon profiles are FTO |
| WOLFGANG AMADEUS | 1 | Moderator |

## Reverse Fireteam index

| Unit | Fireteam access |
|---|---|
| Moderators | Moderators Core/Haris, 1–5 |
| Corregidor Alguaciles | Moderators Core/Haris, max 2 |
| Riot Grrls | Moderators Core/Haris max 2; Riot Grrls Core/Haris/Duo, 1–5 |
| Clockmakers | Moderators Core/Haris max 2; counts as Moderator |
| Casino Security Rounders | Moderators Core/Haris max 1; counts as Moderator |
| Orphans | Moderators Core/Haris max 1; Observance Haris required-choice max 3; Armored Duo max 1 |
| TAG-Treiber | Moderators Core/Haris max 1 |
| Avicenna | Moderators Core/Haris max 1; Riot Grrls Core/Haris/Duo max 1 |
| Zoe FTO | Moderators Core/Haris max 1; FTO combination only |
| Π-Well FTO | Moderators Core/Haris max 1; FTO combination only |
| Vortex Spec-Ops | Moderators Core/Haris max 1 in Spec-Ops mode |
| Reverend Moiras | Reverend Core/Haris required-choice max 5; Observance Haris max 1 |
| Reverend Healers | Reverend Core/Haris required-choice max 3 |
| Reverend Custodiers | Reverend Core/Haris required-choice max 3 |
| Reverend Cenobites | Reverend Core/Haris max 2; Observance Haris max 1 |
| Cassandra Kusanagi | Reverend Core/Haris max 1; Observance Haris max 1 |
| Mother Agatha | Reverend Core/Haris max 1; Observance Haris max 1 |
| Penitent Observants | Observance Haris required-choice max 1 |
| Taskmasters | Riot Grrls Core/Haris/Duo max 3; Taskmasters Haris/Duo 1–3 |
| Fiddler FTO | Riot Grrls Core/Haris/Duo max 1; Opt 1 only |
| Zellenkrieger | Taskmasters Haris/Duo max 1, any profile; Riot Grrls Core/Haris/Duo max 1, FTO Opt 3 only |
| Uhahu | Riot Grrls Core/Haris/Duo max 1 |
| Robin Hook | Riot Grrls Core/Haris/Duo max 1; Armored Duo max 1 |
| Morlocks | Taskmasters Haris/Duo max 2 |
| Denma Connolly | Taskmasters Haris/Duo max 1 |
| Stigmata | Armored Duo required-choice max 2 |
| Lizard | Armored Duo required-choice max 1 |
| Mobile Brigada | Armored Duo max 1 |
| Marspiders | Armored Duo max 1 |
| Vostok FTO | Wildcard max 2; Opts 5 and 7 only |
| Tsyklon FTO | Wildcard max 2; both selectable profiles |
| Wolfgang Amadeus Wolff | Wildcard max 1; counts as Moderator |

## Reinforcement linkage

The pinned Bakunin Army data links Reinforcement roster **599**. This reference deliberately keeps Reinforcement roster entries and Reinforcement-specific Fireteams separate from the standard Bakunin chart.

## Source pinning

- Army source version: `7.26246.158`
- Army data changed on: `2026-09-03`
- Army backup commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`
- InfinityDB commit: `4e2662be3f43387fbae42b3790a711b3e98570c4`
- Rules baseline: N5.3 + N5 FAQ v0.1
- Verified/generated: `2026-10-15`

## Validation notes

- Standard roster count: 48 logical units, excluding Vortex Spec-Ops and Nomads Team-Ops optional modes and excluding generic mercenary-catalog entries with empty faction membership.
- All selectable standard Bakunin Army option rows from the pinned source are represented above; disabled constituent/peripheral rows are described under their owning logical unit rather than promoted to independent selectable roster entries.
- Fireteam member slugs resolve to roster units or the documented Vortex Spec-Ops hook.
- Profile-restricted Fireteam access is explicitly marked for Vostok, Fiddler, Zellenkrieger, Zoe, and Π-Well.
- The reverse Fireteam index is derivative; if any conflict is found, the canonical Fireteam chart above wins.
- Main and Reinforcement charts are not merged.

## TAG tactical cross-reference (2026-10-23)

**Lizard (60–65)** is the more conventional ARM8 Repeater/MULTI gun with useful E/M/GL variants; **Stigmata (56)** is unusually useful as a *hacking TAG* with Carbonite and heavy close/mid templates. They solve different problems: Lizard for ranged suppression and armor, Stigmata to exploit Bakunin's hacking net and contest dense objectives. **Podcast disagreement:** Lizard praised as practical top-tier value; Stigmata is not a straight gunfight replacement.

Cross-faction **apex vs points-value** comparisons, matchup table, and direct MCP-reviewed podcast/video sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Current profile and Fireteam legality above remain authoritative.
