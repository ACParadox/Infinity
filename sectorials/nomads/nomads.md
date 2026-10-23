---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 501
sectorial_slug: nomads
sectorial_name: Vanilla Nomads
parent_faction: Nomads
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Vanilla Nomads standard roster, AVA, standard loadouts and points/SWC, canonical vanilla Fireteam chart and reverse access index, optional Spec-Ops/Team-Ops hooks, source relations, and the distinct Vipera Pursuit Force Reinforcement Fireteam chart."
---

# Vanilla Nomads

## Overview and provenance

Repository-native reference for **Vanilla Nomads** roster, profiles, points/SWC, AVA, and the Fireteams explicitly exposed by the current Army source.

For concise tactical/list-building analysis (including reviewed video/podcast transcripts, opposing opinions, TAGs, Go-Pod and REMs), see [Vanilla Nomads — N5.3 Tactical and List-Building Guide](../../notes/factions/vanilla-nomads.md). This reference remains authoritative for legal rosters and profiles.

Sources used:

- Army-derived Nomads source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `d4329bb596ffea5d568eb2435f74366c305a7630`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Schema note:

- The repository currently has no separate vanilla-faction reference schema. This file therefore keeps `reference_type: sectorial` and the established `sectorial_*` front-matter keys for compatibility, while `sectorial_name` explicitly identifies this as the **vanilla faction roster**.

Coverage notes:

- Covers the **53-unit standard Vanilla Nomads roster** in the pinned Army source.
- `Vortex Spec-Ops` and `Nomads Team-Ops` are optional game-mode content and are listed separately rather than counted in the 53 standard entries.
- Generic Soldier of Fortune / `merc-*` catalogue entries with empty faction lists are excluded from the standard roster.
- Vanilla AVA is taken from the vanilla source, not inherited from Bakunin, Corregidor, or Tunguska. Sectorial AVA may be materially higher.
- The current vanilla source contains a Fireteam chart: **Core 0, Haris 1, Duo 2**.
- Every standard vanilla Fireteam-chart row has `required: false` and `min: 0`; no mandatory anchor is invented for either mixed pool.
- Fireteam legality comes from the canonical Army chart, not from an `FTO` profile label by itself. `JAZZ FTO` is explicitly present in Nomads Fireteams I. FTO-labelled Tsyklon, Vostok, Stempler, Switcher, Coyote, and Zoe profiles are not present in the vanilla chart and gain no vanilla Fireteam access from the label alone.
- Wolfgang Amadeus Wolff and Perseus are the two canonical vanilla Wildcards.
- Linked Reinforcement army ID: **599, Vipera Pursuit Force**. Its Fireteam chart is recorded separately and is not merged into the standard vanilla chart.

## Faction summary

| Field | Value |
|---|---|
| Faction | Vanilla Nomads |
| Army ID | 501 |
| Army slug | `nomads` |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 53 |
| Optional-mode units | Vortex Spec-Ops; Nomads Team-Ops |
| Reinforcement roster | Vipera Pursuit Force, Army ID `599` |
| Fireteam limits | Core 0; Haris 1; Duo 2 |
| Fireteam pools | Nomads Fireteams I; Nomads Fireteams II; Wildcards |

## Standard roster index

| Unit | ID | AVA | Type | Order / structure | Vanilla Fireteam access |
|---|---:|---:|---|---|---|
| Grenzers, Grenz Security Team | 393 | 1 | MI | Regular | I max 1; II max 1 |
| Bakunin Überfallkommando | 422 | 1 | WB | Irregular + Impetuous team | — |
| Zondbots | 425 | 2 | REM | Peripheral | — |
| Die Morlock Gruppe | 403 | 2 | WB | Irregular + Impetuous | I max 2 |
| Tsyklon Sputniks | 423 | 2 | REM | Regular | — |
| Meteor Zonds | 411 | 1 | REM | Regular | — |
| Wolfgang Amadeus Wolff | 1555 | 1 | WB | Regular | Wildcard max 1 |
| Evaders, EVA Tactical Group | 1543 | 1 | HI | Regular | I max 1 |
| Gator Squadron | 1580 | 1 | TAG | Regular + Tactical Awareness | I max 1 |
| Coyotes, Recon and Maneuver Team | 1896 | 1 | MI | Regular; BambaDroid options | — |
| Zeros | 401 | 2 | SK | Regular | — |
| Tunguska Interventors | 407 | 2 | LI | Regular | — |
| Securitate | 434 | 5 | LI | Regular | I max 2 |
| Sin-Eater Observants | 418 | 1 | MI | Regular | — |
| TAG-Treiber | 1853 | 1 | LI | Regular | — |
| Switchers Gruppa | 1848 | 1 | LI | Regular + Tactical Awareness | — |
| Kulak Payback Unit | 1761 | 2 | MI | Regular | I max 2; II max 2 |
| Shifta Insertion Group | 1902 | 1 | LI | Regular | — |
| Territorials | 1893 | 2 | MI | Regular + Tactical Awareness | — |
| Clockmakers | 406 | 1 | LI | Regular | — |
| Mary Problems | 1099 | 1 | LI | Regular | — |
| Hecklers | 1095 | 1 | SK | Regular | — |
| Reaktion Zonds | 409 | 1 | REM | Regular | — |
| Casino Security Rounders | 1762 | 2 | LI | Regular | II max 1 |
| Salyut Zonds | 426 | 2 | REM | Regular | — |
| Zondnautica Rapid Offensive Unit | 1091 | 1 | WB/REM | Regular mounted team | — |
| Kriza Boracs | 954 | 1 | HI | Regular | I max 1 |
| Taskmasters | 781 | 1 | HI | Regular | I max 1 |
| Warcors | 50 | 1 | LI | Irregular | — |
| Tunguska Triggermen | 1855 | 1 | HI | Regular | — |
| Mobile Brigada | 382 | 5 | HI | Regular | I max 2; II max 3 |
| RacerBots | 1905 | 2 | REM | Regular | — |
| Daktaris | 405 | 1 | LI | Regular | — |
| Moderators from Bakunin | 414 | 5 | LI | Regular | — |
| Moran, Maasai Hunter | 421 | 1 | SK | Regular | — |
| Vertigo Zonds | 410 | 1 | REM | Regular | — |
| Zoe & Π-Well | 413 | 1 team | LI + REM | Regular team / FTO variants | — |
| Szalamandra Squad | 420 | 1 | TAG | Regular | — |
| Gecko Squad | 432 | 2 | TAG | Regular + Tactical Awareness | I max 2 |
| Hellcats | 394 | 2 | MI | Regular | — |
| Bearcats | 1891 | 1 | HI | Regular | — |
| Puppetactica Company | 1098 | 1 master / 3 bots | LI + REM | Regular master + PuppetBots | — |
| Spektrs | 402 | 1 | SK | Regular | — |
| Transductor Zonds | 412 | 2 | REM | Regular | — |
| Jazz & Billie | 1551 | 1 team | LI + REM | Regular; Jazz FTO standalone option | I max 1, **Jazz FTO only** |
| Redsky Crew Marspiders | 1760 | 2 | LI | Regular | II max 1 |
| Go-Pod | 1854 | 1 | VH | Regular + peripheral | — |
| Stempler Zonds | 408 | 2 | REM | Regular | — |
| Vostok Sputniks | 1544 | 1 | REM | Regular | — |
| Perseus, Rogue Myrmidon | 1101 | 1 | WB | Regular | Wildcard max 1 |
| Intruders | 395 | 1 | MI | Regular | — |
| Corregidor Alguaciles | 296 | 5 | LI | Regular | — |
| Vigilantes | 1895 | 2 | MI | Regular | — |

## Optional-mode units

| Unit | ID | Mode | Vanilla Fireteam relevance |
|---|---:|---|---|
| Vortex Spec-Ops | 1917 | Spec-Ops | No ordinary vanilla chart row |
| Nomads Team-Ops | 1931 | Team-Ops | No ordinary vanilla chart row |

## Unit details

### Grenzers, Grenz Security Team

**ID 393 · AVA 1 · MI** — `MOV 10-10 | CC 16 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 6 | W 1 | S 2`. Veteran marksmen with MSV1.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 28 | 1.5 | Missile Launcher, Pistol, Breaker Pistol, CC Weapon | I max1; II max1 |
| 28 | 1 | Red Fury, Pistol, Breaker Pistol, CC Weapon | same |
| 29 | 0 | Combi Rifle, Light Flamethrower (+1B), Flash Pulse; Forward Observer, Sensor, NCO | same |
| 28 | 0 | Combi Rifle, Light Flamethrower (+1B); Biometric Visor, Discover (+3) | same |
| 32 | 1.5 | MULTI Sniper Rifle; Marksmanship | same |
| 28 | 0 | Biometric / Discover package; Lieutenant | same |

### Bakunin Überfallkommando

**ID 422 · AVA 1 team · WB** — Chimera `MOV 15-10 | CC 24 | BS 11 | PH 13 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`; Irregular and Impetuous assault team.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 19 | 0 | Chimera with Combi Rifle, Nanopulser, Eclipse Grenades, Pistol, Viral CC Weapon + 3 Pupniks | — |

### Zondbots

**ID 425 · AVA 2 · REM** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Servant Peripheral.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 3 | 0 | PARA CC Weapon (-3); Servant | — |

### Die Morlock Gruppe

**ID 403 · AVA 2 · WB** — `MOV 10-10 | CC 23 | BS 11 | PH 13 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Irregular, Impetuous, Martial Arts / MetaChemistry warbands.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 6 | 0 | Chain Rifle, Smoke Grenades, Assault Pistol, AP CC Weapon | I max2 |
| 6 | 0 | Chain Rifle, Smoke Grenades, Kobra Pistol, DA CC Weapon | same |
| 6 | 0 | Chain Rifle, Smoke Grenades, Kobra Pistol, E/M CC Weapon | same |
| 9 | 0 | Boarding Shotgun, Smoke Grenades, Kobra Pistol, DA CC Weapon | same |
| 12 | 0 | Combi Rifle, Smoke Grenade Launcher, Kobra Pistol, DA CC Weapon | same |

### Tsyklon Sputniks

**ID 423 · AVA 2 · REM** — `MOV 15-10 | CC 14 | BS 12 | PH 10 | WIP 13 | ARM 3 | BTS 6 | W 1 | S 4`. Repeater, 360º Visor, X-Visor, Remote Presence, Climbing Plus.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 26 | 1 | **TSYKLON FTO** — Spitfire, Chain Rifle, Pitcher, PARA CC Weapon | **No vanilla FT row** |
| 29 | 1 | **TSYKLON FTO** — Feuerbach, Chain Rifle, Pitcher, PARA CC Weapon | **No vanilla FT row** |
| 31 | 1 | Feuerbach, Chain Rifle, Pitcher; Forward Deployment (+10) | — |
| 31 | 1 | Spitfire, Chain Rifle, Pitcher, CrazyKoala; Forward Deployment (+10), Minelayer | — |

### Meteor Zonds

**ID 411 · AVA 1 · REM** — `MOV 15-10 | CC 14 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 6 | W 1 | S 3`. Airborne Repeater / Sensor REM with Combat Jump and Super-Jump.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 21 | 0 | Light Shotgun, E/M Carbine, Flash Pulse, PARA CC Weapon | — |
| 19 | 0 | Boarding Shotgun, Flash Pulse, PARA CC Weapon | — |

### Wolfgang Amadeus Wolff

**ID 1555 · AVA 1 · WB** — `MOV 15-5 | CC 22 | BS 12 | PH 14 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`. Close-combat character.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 33 | 0 | MULTI Rifle, E/M Grenades, Chain-colt, Heavy Pistol, PARA CC Weapon, DA CC Weapon | **Wildcard max1** |

### Evaders, EVA Tactical Group

**ID 1543 · AVA 1 · HI** — `MOV 10-10 | CC 15 | BS 13 | PH 12 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Durable specialist / engineer HI.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 31 | 1 | AP Spitfire, D-Charges, Pistol, CC Weapon; TinBot, Specialist Operative | I max1 |
| 23 | 0 | Boarding Shotgun (+1SD), D-Charges, AP Mine; TinBot, Specialist Operative | same |
| 32 | 1.5 | Feuerbach, D-Charges; TinBot, Specialist Operative | same |
| 29 | 0 | MULTI Rifle, Panzerfaust, D-Charges; GizmoKit, Engineer | same |
| 24 | 0 | Boarding Shotgun, D-Charges, AP Mine; GizmoKit, Engineer | same |
| 35 | 1.5 | AP Spitfire, D-Charges; GizmoKit, TinBot, Engineer | same |

### Gator Squadron

**ID 1580 · AVA 1 · TAG** — `MOV 15-10 | CC 21 | BS 14 | PH 15 | WIP 13 | ARM 8 | BTS 6 | W 3 | S 7`. Tactical Awareness / NCO assault TAG with Robbybot support.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 73 | 1.5 | MULTI HMG, Chain Rifle (+1B), Mine Dispenser (AP), E/M CC Weapon + Robbybot | I max1 |

### Coyotes, Recon and Maneuver Team

**ID 1896 · AVA 1 · MI** — Coyote `MOV 10-10 | CC 15 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 6 | W 1 | S 2`; MSV1, Forward Observer and forward-deployment options. BambaDroids require a Coyote in the same Combat Group; no more BambaDroids than Coyotes.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 27 | 0 | Boarding Shotgun, Flash Pulse, D-Charges; Forward Deployment (+10) + BambaBot-1 | — |
| 27 | 0 | Same Coyote + BambaBot-2 | — |
| 33 | 0 | MULTI Marksman Rifle, D-Charges; Forward Deployment (+10) + BambaBot-1 | — |
| 33 | 0 | Same Coyote + BambaBot-2 | — |
| 28 | 0 | SMG, Flash Pulse; Killer Hacking Device / Hacker, Forward Deployment (+10) + BambaBot-1 | — |
| 28 | 0 | Same Coyote + BambaBot-2 | — |
| 19 | 0 | **COYOTE FTO** — Boarding Shotgun, Flash Pulse, D-Charges | **No vanilla FT row** |
| 26 | 0 | **COYOTE FTO** — MULTI Marksman Rifle, D-Charges | **No vanilla FT row** |
| 23 | 0 | **COYOTE FTO** — SMG, E/Mitter, D-Charges; Killer Hacking Device / Hacker | **No vanilla FT row** |

### Zeros

**ID 401 · AVA 2 · SK** — `MOV 10-10 | CC 15 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Camouflage / Infiltration specialists.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 19 | 0 | Combi Rifle, Shock Mine | — |
| 21 | 1.5 | MULTI Sniper Rifle, Shock Mine | — |
| 17 | 0 | Boarding Shotgun, Shock Mine, PARA Mine | — |
| 20 | 0 | Combi Rifle, E/M Mine; Deployable Repeater | — |
| 24 | 0.5 | Combi Rifle, Shock Mine; Hacking Device | — |
| 22 | 0 | Combi Rifle, Shock Mine; Killer Hacking Device | — |
| 18 | 0.5 | Boarding Shotgun, Shock Mine, PARA Mine; Minelayer | — |
| 20 | 0 | Combi Rifle, Shock Mine, Flash Pulse; Forward Observer | — |

### Tunguska Interventors

**ID 407 · AVA 2 · LI** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 15 | ARM 1 | BTS 9 | W 1 | S 2`. Elite hackers.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 21 | 0.5 | Combi Rifle; Hacking Device Plus | — |
| 23 | 0.5 | Combi Rifle; Hacking Device Plus, FastPanda | — |
| 18 | 0.5 | Boarding Shotgun; Hacking Device Plus | — |
| 20 | 0.5 | Boarding Shotgun; Hacking Device Plus, FastPanda | — |
| 21 | 0.5 | Combi Rifle; Lieutenant, Hacking Device Plus | — |
| 23 | 0.5 | Combi Rifle; Lieutenant, Hacking Device Plus, FastPanda | — |
| 18 | 0 | Boarding Shotgun; Killer Hacking Device, FastPanda | — |

### Securitate

**ID 434 · AVA 5 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Warhorse line infantry.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 13 | 0 | Combi Rifle | I max2 |
| 21 | 1 | HMG | same |
| 22 | 1 | Feuerbach | same |
| 13 | 0 | Boarding Shotgun; Repeater | same |
| 18 | 0.5 | Combi Rifle; Hacking Device | same |
| 15 | 0 | Combi Rifle; MediKit / Paramedic | same |
| 13 | 0 | Combi Rifle; Lieutenant | same |
| 15 | 0 | Combi Rifle; Commlink (+1), Specialist Operative | same |

### Sin-Eater Observants

**ID 418 · AVA 1 · MI** — `MOV 10-10 | CC 14 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 2`. Mimetism (-3), Neurocinetics, Religious Troop, Immunity (Shock).

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 28 | 1.5 | HMG | — |
| 26 | 1.5 | MULTI Sniper Rifle | — |
| 25 | 0 | Mk12 | — |

### TAG-Treiber, NMF TAG Squadrons Support Pilots

**ID 1853 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Specialist / TAG support profiles.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 12 | 0 | Gecko Pilot: Combi Rifle, Assault Pistol (+1B); GizmoKit, Zero-G | — |
| 10 | 0 | Szalamandra Pilot: Light Shotgun, Cybermine; Killer Hacking Device | — |
| 11 | 0 | Gator Pilot: Boarding Shotgun, D-Charges, Kobra Pistol, PARA CC Weapon; CC Attack bonus | — |

### Switchers Gruppa

**ID 1848 · AVA 1 · LI** — Transmutation unit. Initial form `MOV 10-10 | CC 15 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`; enhanced form `MOV 15-10 | CC 23 | BS 13 | PH 14 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Tactical Awareness.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 25 | 0 | **SWITCHER FTO** — Combi Rifle, E/Mitter, Zapper, Pistol, Viral CC Weapon | **No vanilla FT row** |
| 27 | 0 | **SWITCHER FTO** — Thunderbolt, E/M Carbine, E/M Grenades; BS Attack (+1B) | **No vanilla FT row** |
| 20 | 0 | **SWITCHER FTO** — AP SMG, Flash Pulse (+1B), E/M Grenades; Forward Observer | **No vanilla FT row** |
| 21 | 0 | AP SMG, Flash Pulse (+1B), E/M Grenades, MadTraps | — |

### Kulak Payback Unit

**ID 1761 · AVA 2 · MI** — `MOV 10-10 | CC 18 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Mimetism (-3), Religious Troop, Immunity (Shock).

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 20 | 1 | Heavy Rocket Launcher, Pulzar (+1B), MULTI Pistol | I max2; II max2 |
| 23 | 0.5 | Boarding Shotgun (+1B), D-Charges; Chain of Command | same |
| 20 | 0 | AP SMG, D-Charges, Cybermine, Disco Baller; Killer Hacking Device | same |
| 19 | 0 | Boarding Shotgun (+1B), Flash Pulse, D-Charges; Forward Observer | same |
| 21 | 0 | Combi Rifle (+1B), Pulzar | same |

### Shifta Insertion Group

**ID 1902 · AVA 1 · LI** — `MOV 10-10 | CC 16 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Non-Hackable specialist with Triangulated Fire / Strategic Deployment utilities.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 21 | 0 | Light Shotgun (+1B), E/Marat, Flash Pulse, Disco Baller; Chain of Command | — |
| 17 | 0 | SMG, E/Marat, Flash Pulse, E/M Mine; Minelayer | — |
| 22 | 0 | Thunderbolt (+1B), E/M Mine; Minelayer | — |
| 21 | 0 | Thunderbolt (+1B); MediKit / Paramedic | — |

### Territorials, Territorial Domination Unit

**ID 1893 · AVA 2 · MI** — `MOV 10-10 | CC 14 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Non-Hackable; Tactical Awareness, Marksmanship, Combat Instinct.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 28 | 0 | AP SMG, E/Mitter, Panzerfaust, D-Charges; Deactivator, GizmoKit, Engineer | — |
| 26 | 0 | Boarding Shotgun (+1B), Panzerfaust, D-Charges; GizmoKit, Specialist Operative | — |
| 32 | 1.5 | AP Red Fury, D-Charges; Specialist Operative | — |
| 29 | 0 | AP Marksman Rifle; X-Visor | — |
| 32 | 1.5 | AP Red Fury, D-Charges; Lieutenant, Specialist Operative | — |
| 28 | 0 | AP SMG / E/Mitter / Panzerfaust engineer package; Lieutenant | — |

### Clockmakers

**ID 406 · AVA 1 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 15 | ARM 1 | BTS 3 | W 1 | S 2`. Engineer with Deactivator and improved GizmoKit.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 18 | 0 | Combi Rifle, D-Charges; Engineer | — |
| 19 | 0 | Combi Rifle, D-Charges; Deployable Cover, Engineer | — |
| 21 | 0 | Combi Rifle, D-Charges, Armed Turret (Combi Rifle); Engineer | — |

### Mary Problems, Tactical ÜberHacker

**ID 1099 · AVA 1 · LI** — `MOV 10-10 | CC 14 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 6 | W 1 | S 2`. Forward Deployment, Mimetism (-6), Climbing Plus, elite hacking suite.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 27 | 0.5 | SMG, Zapper, Pitcher; Hacking Device / Killer Hacking Device program package | — |

### Hecklers

**ID 1095 · AVA 1 · SK** — `MOV 10-10 | CC 15 | BS 12 | PH 11 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. One-use Camouflage, Forward Deployment, Mimetism and Stealth.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 20 | 0 | Boarding Shotgun (+1B), E/Marat | — |
| 24 | 1 | Red Fury | — |
| 23 | 0 | Combi Rifle, Cybermine, Assault Pistol; Killer Hacking Device | — |

### Reaktion Zonds

**ID 409 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. 360º Visor, Remote Presence, Total Reaction, Climbing Plus.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 24 | 1 | HMG, PARA CC Weapon | — |
| 19 | 0 | Thunderbolt (+1B), PARA CC Weapon | — |

### Casino Security Rounders

**ID 1762 · AVA 2 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. MSV1, Marksmanship, NCO, Biometric Visor, Zero-G.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 17 | 0 | Boarding Shotgun | II max1 |
| 24 | 0.5 | MULTI Marksman Rifle | same |
| 26 | 1 | Red Fury | same |
| 21 | 0.5 | SMG; Hacking Device / Hacker | same |

### Salyut Zonds

**ID 426 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 4`. Baggage support REM.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 8 | 0 | Deactivator, Repeater, PARA CC Weapon | — |
| 14 | 0.5 | EVO Hacking Device, PARA CC Weapon | — |
| 17 | 0 | Combi Rifle, PARA CC Weapon; Repeater, Total Reaction | — |

### Zondnautica Rapid Offensive Unit

**ID 1091 · AVA 1 · WB/REM team** — Mounted form `MOV 20-10 | CC 15 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 4`; dismounted operator and Zondmate profiles are included by the source.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 25 | 1.5 | Spitfire package; mounted Chain Rifle / Smoke Grenade Launcher + Zondmate | — |
| 17 | 0 | Boarding Shotgun package; mounted Chain Rifle / Smoke Grenade Launcher + Zondmate | — |
| 23 | 0.5 | Combi Rifle / Flash Pulse; Hacking Device + Zondmate | — |

### Kriza Boracs, Special Crisis Unit

**ID 954 · AVA 1 · HI** — `MOV 10-10 | CC 19 | BS 13 | PH 13 | WIP 13 | ARM 5 | BTS 6 | W 2 | S 5`. Heavy gunfighter with burst-modifying BS skill.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 45 | 1.5 | HMG | I max1 |
| 48 | 0 | Mk12, SMG; 360º Visor | same |
| 45 | 1.5 | HMG; Lieutenant | same |

### Taskmasters

**ID 781 · AVA 1 · HI** — `MOV 10-10 | CC 22 | BS 13 | PH 13 | WIP 13 | ARM 5 | BTS 6 | W 2 | S 5`. Martial Arts, Minelayer, Stealth and FT Master support package.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 40 | 1.5 | HMG, Shock Mine, Heavy Pistol, DA CC Weapon | I max1 |
| 39 | 1 | Red Fury, Pulzar, CrazyKoala; TinBot | same |
| 34 | 1.5 | Heavy Rocket Launcher, Light Shotgun, CrazyKoala | same |
| 44 | 1 | Red Fury package; Strategic Deployment | same |
| 39 | 1 | Red Fury package; Lieutenant | same |

### Warcors

**ID 50 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular Journalist.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 3 | 0 | Flash Pulse, Stun Pistol, PARA CC Weapon; 360º Visor | — |
| 3 | 0 | Flash Pulse, Stun Pistol, PARA CC Weapon; Sixth Sense | — |

### Tunguska Triggermen

**ID 1855 · AVA 1 · HI** — `MOV 15-5 | CC 17 | BS 13 | PH 12 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 4`. 360º Visor, Mimetism, Stealth, Regeneration and offensive modifiers.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 44 | 1.5 | MULTI Sniper Rifle, E/Marat (+1B), Pulzar (+1B), MULTI Pistol | — |
| 43 | 0 | K1 Combi Rifle, E/Marat (+1B), Pulzar (+1B), Drop Bears; Forward Deployment / Decoy package | — |
| 47 | 1.5 | MULTI Sniper Rifle package; Neurocinetics | — |

### Mobile Brigada

**ID 382 · AVA 5 · HI** — `MOV 15-5 | CC 18 | BS 13 | PH 13 | WIP 13 | ARM 5 | BTS 3 | W 2 | S 2`. 360º Visor heavy infantry.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 33 | 0 | MULTI Rifle, Boarding Pistol (+1B), CC Weapon; TinBot | I max2; II max3 |
| 38 | 1.5 | HMG, Boarding Pistol (+1B), CC Weapon | same |
| 27 | 0 | Boarding Shotgun, Boarding Pistol (+1B), CC Weapon | same |
| 35 | 1.5 | Missile Launcher, Boarding Pistol (+1B), CC Weapon | same |
| 36 | 0.5 | Combi Rifle, D-Charges; Hacking Device, TinBot | same |
| 33 | 0 | MULTI Rifle; Lieutenant, TinBot | same |
| 27 | 0 | Boarding Shotgun; Lieutenant | same |

### RacerBots

**ID 1905 · AVA 2 · REM** — `MOV 20-10 | CC 13 | BS 11 | PH 12 | WIP 11 | ARM 0 | BTS 3 | W 1 | S 2`. Fast disposable control REM.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 9 | 0 | RacerBot Mk-I: Adhesive Launcher Rifle, PARA Mine, PARA CC Weapon (-6) | — |
| 9 | 0 | RacerBot Mk-II: Heavy Riotstopper, Mine Dispenser (PARA), PARA CC Weapon (-6) | — |

### Daktaris

**ID 405 · AVA 1 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Doctor.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 14 | 0 | Combi Rifle, Pistol, CC Weapon; MediKit, Doctor | — |

### Moderators from Bakunin

**ID 414 · AVA 5 · LI** — `MOV 10-10 | CC 18 | BS 10 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`. Cheap line infantry.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 9 | 0 | Combi Rifle | — |
| 15 | 0.5 | Spitfire | — |
| 10 | 0 | Combi Rifle, Pitcher | — |
| 14 | 0.5 | Combi Rifle; Hacking Device | — |
| 11 | 0 | Combi Rifle; MediKit / Paramedic | — |
| 9 | 0 | Combi Rifle; Lieutenant | — |
| 9 | 0 | Boarding Shotgun, E/M Carbine | — |
| 11 | 0 | Combi Rifle; Commlink (+1), Specialist Operative | — |

### Moran, Maasai Hunter

**ID 421 · AVA 1 · SK** — `MOV 10-10 | CC 15 | BS 12 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Infiltration, Mimetism, Minelayer, Forward Observer and CrazyKoala network piece.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 18 | 0.5 | Combi Rifle, Flash Pulse, D-Charges, CrazyKoala; one-use Camouflage package | — |
| 16 | 0.5 | Boarding Shotgun, Flash Pulse (+1B), CrazyKoala; one-use Camouflage package | — |
| 17 | 0.5 | Combi Rifle, Flash Pulse, D-Charges, CrazyKoala; Repeater | — |
| 15 | 0.5 | Boarding Shotgun, Flash Pulse (+1B), CrazyKoala; Repeater | — |

### Vertigo Zonds

**ID 410 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Guided missile REM.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 16 | 1.5 | Missile Launcher, PARA CC Weapon; Guided | — |

### Zoe & Π-Well

**ID 413 · AVA 1 team · LI + REM** — Zoe `MOV 10-10 | CC 16 | BS 11 | PH 10 | WIP 15 | ARM 1 | BTS 3 | W 1 | S 2`; elite Engineer / Hacker paired with Π-Well.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 45 | 0.5 | **ZOE FTO & PI-WELL FTO** — Zoe Combi Rifle / D-Charges hacker package + Π-Well Combi Rifle / Flash Pulse / Pitcher | **No vanilla FT row** |
| 42 | 0.5 | **ZOE FTO-2 & PI-WELL FTO** — Zoe Boarding Shotgun variant + Π-Well | **No vanilla FT row** |

### Szalamandra Squad

**ID 420 · AVA 1 · TAG** — `MOV 15-10 | CC 17 | BS 14 | PH 16 | WIP 13 | ARM 8 | BTS 9 | W 3 | S 7`. Heavy TAG with Robbybot.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 68 | 2 | Hyper-Rapid Magnetic Cannon, Heavy Flamethrower, CC Weapon + Robbybot | — |

### Gecko Squad

**ID 432 · AVA 2 · TAG** — `MOV 15-5 | CC 15 | BS 13 | PH 14 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`. Tactical Awareness light TAG.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 54 | 1 | MULTI Marksman Rifle, Chain Rifle, Panzerfaust, CC Weapon + Robbybot | I max2 |
| 55 | 1 | Mk12, Chain Rifle, Blitzen, CC Weapon + Robbybot | same |
| 49 | 0 | Vulkan Shotgun, Chain Rifle, Panzerfaust, CC Weapon + Robbybot | same |

### Hellcats

**ID 394 · AVA 2 · MI** — `MOV 10-10 | CC 14 | BS 12 | PH 12 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Combat Jump / Parachutist airborne infantry.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 19 | 0 | Boarding Shotgun, Adhesive Launcher Rifle, D-Charges | — |
| 26 | 1.5 | Spitfire | — |
| 22 | 0.5 | Boarding Shotgun, D-Charges; Hacking Device | — |
| 23 | 0 | Combi Rifle; MediKit, Deployable Repeater, Paramedic | — |

### Bearcats, Airborne Heavy Regiment

**ID 1891 · AVA 1 · HI** — `MOV 15-5 | CC 15 | BS 13 | PH 13 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Airborne NWI heavy infantry.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 30 | 0 | Boarding Shotgun (+1B), D-Charges; Killer Hacking Device | — |
| 29 | 0 | AP SMG, Adhesive Launcher Rifle, D-Charges; Killer Hacking Device | — |
| 28 | 0 | AP SMG, D-Charges; Deactivator, GizmoKit, Engineer | — |
| 35 | 1.5 | Spitfire, D-Charges; Specialist Operative | — |
| 27 | 0 | AP SMG; MediKit, Deployable Repeater, Paramedic | — |

### Puppetactica Company

**ID 1098 · AVA 1 Puppet Master / 3 PuppetBots · LI + REM** — Puppet Master `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`; source relation requires the Puppet Master group when PuppetBots are selected.

Puppet Master:

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 11 | 0 | SMG, Shock Mine | — |
| 13 | 0 | SMG, Shock Mine; Minelayer | — |
| 16 | 0.5 | SMG, Shock Mine; Hacking Device | — |

PuppetBots:

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 9 | 0 | Boarding Shotgun, Flash Pulse, PARA CC Weapon; Forward Observer | — |
| 14 | 0 | AP Marksman Rifle, PARA CC Weapon; BS Attack (Shock) | — |
| 16 | 1.5 | Red Fury, PARA CC Weapon | — |

### Spektrs

**ID 402 · AVA 1 · SK** — `MOV 10-10 | CC 13 | BS 12 | PH 12 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Camouflage, Hidden Deployment, Infiltration, Mimetism (-6), Stealth.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 32 | 1.5 | MULTI Sniper Rifle, Shock Mine, Silenced Pistol | — |
| 28 | 0 | SMG, E/M Mine; Deployable Repeater | — |
| 35 | 0.5 | Combi Rifle, D-Charges; Hacking Device | — |
| 29 | 0 | Boarding Shotgun, Shock Mine, Flash Pulse; Forward Observer | — |
| 32 | 0.5 | Boarding Shotgun, D-Charges; Hacking Device | — |
| 33 | 1 | Combi Rifle, D-Charges, E/M Mine, Shock Mine; Minelayer | — |

### Transductor Zonds

**ID 412 · AVA 2 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 7 | 0 | Flash Pulse, PARA CC Weapon; Repeater | — |

### Jazz & Billie, Tactical Hacking Team

**ID 1551 · AVA 1 · LI + REM** — Jazz `MOV 10-10 | CC 16 | BS 11 | PH 10 | WIP 14 | ARM 0 | BTS 6 | W 1 | S 2`; elite hacker with either Billie or a standalone FTO profile.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 25 | 0.5 | Jazz hacker + Billie; Jazz SMG, Pitcher, Cybermine, Boarding Pistol; Billie Flash Pulse / E/M Mine package | — |
| 22 | 0.5 | **JAZZ FTO** — Combi Rifle, Pitcher, Cybermine, Boarding Pistol; Hacker, Number 2 | **I max1; FTO profile only** |

### Redsky Crew Marspiders

**ID 1760 · AVA 2 · LI** — `MOV 15-5 | CC 23 | BS 11 | PH 13 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. 360º Visor, Climbing Plus, GizmoKit and strong close-combat mobility.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 18 | 0 | Heavy Flamethrower (+1B), Flash Pulse, Panzerfaust, Assault Pistol, DA CC Weapon | II max1 |
| 18 | 0 | Heavy Flamethrower (+1B), Flash Pulse, Grenades (+1B), Assault Pistol, DA CC Weapon | same |
| 22 | 0 | Panzerfaust package; Engineer | same |
| 19 | 0 | Heavy Flamethrower (+1B), Flash Pulse; MediKit / Paramedic | same |

### Go-Pod

**ID 1854 · AVA 1 · VH** — `MOV 20-5 | BS 13 | PH 13 | WIP 13 | ARM 2 | BTS 6 | W 2 | S 7`; Aerial platform with Go-Bot peripheral.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 33 | 0 | MULTI Rifle, E/Mitter + Go-Bot | — |
| 32 | 1.5 | Heavy Rocket Launcher, AP SMG; BS Attack (Shock) + Go-Bot | — |

### Stempler Zonds

**ID 408 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Deactivator, Forward Observer, Sensor, Climbing Plus.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 15 | 0 | Combi Rifle, Flash Pulse, PARA CC Weapon | — |
| 18 | 0 | Same core package; Tactical Awareness | — |
| 17 | 0 | **STEMPLER FTO** — same core package; Super-Jump | **No vanilla FT row** |
| 22 | 0 | Thunderbolt (+1B), Flash Pulse, PARA CC Weapon; Tactical Awareness | — |

### Vostok Sputniks

**ID 1544 · AVA 1 · REM** — `MOV 15-10 | CC 14 | BS 12 | PH 10 | WIP 13 | ARM 3 | BTS 6 | W 2 | S 4`. Mimetism (-6), Remote Presence, Climbing Plus, Immunity (AP).

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 38 | 0 | Mk12, Light Shotgun, PARA CC Weapon; Repeater | — |
| 35 | 0 | **VOSTOK FTO** — Mk12, Light Shotgun, PARA CC Weapon | **No vanilla FT row** |
| 37 | 1 | Spitfire, PARA CC Weapon; Repeater | — |
| 34 | 1 | **VOSTOK FTO** — Spitfire, PARA CC Weapon | **No vanilla FT row** |

### Perseus, Rogue Myrmidon

**ID 1101 · AVA 1 · WB** — `MOV 10-10 | CC 23 | BS 13 | PH 13 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. Martial Arts, NWI, Mimetism (-6), Stealth, Super-Jump and smoke.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 34 | 0 | MULTI Rifle, Nanopulser, Smoke Grenades, AP Heavy Pistol, DA CC Weapon | **Wildcard max1** |
| 33 | 0 | Breaker Combi Rifle, Nanopulser, Smoke Grenades, AP Heavy Pistol, DA CC Weapon | **Wildcard max1** |

### Intruders, Corregidor Assault Commandos

**ID 395 · AVA 1 · MI** — `MOV 10-10 | CC 14 | BS 13 | PH 12 | WIP 14 | ARM 3 | BTS 3 | W 1 | S 2`. MSV2, Camouflage, Mimetism (-3).

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 38 | 1.5 | HMG, Heavy Pistol, CC Weapon | — |
| 33 | 0 | AP SMG (+1B), Pulzar (+1B), Grenades, D-Charges; Killer Hacking Device, Infiltration | — |
| 38 | 1.5 | MULTI Sniper Rifle (+1SD), Heavy Pistol, CC Weapon | — |

### Corregidor Alguaciles

**ID 296 · AVA 5 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 10 | 0 | Combi Rifle | — |
| 18 | 1 | HMG | — |
| 15 | 1.5 | Missile Launcher | — |
| 15 | 0.5 | Combi Rifle; Hacking Device | — |
| 12 | 0 | Combi Rifle, Flash Pulse; Deployable Repeater, Forward Observer | — |
| 12 | 0 | Combi Rifle; MediKit / Paramedic | — |
| 10 | 0 | Combi Rifle; Lieutenant | — |
| 12 | 0 | Combi Rifle; Commlink (+1), Specialist Operative | — |

### Vigilantes, Tactical Support and Surveillance Special Group

**ID 1895 · AVA 2 · MI** — `MOV 10-10 | CC 16 | BS 12 | PH 11 | WIP 13 | ARM 3 | BTS 6 | W 1 | S 2`. Non-Hackable; Camouflage, Counterintelligence, Forward Deployment (+20), Mimetism and Stealth.

| Pts | SWC | Loadout / differences | FT |
|---:|---:|---|---|
| 25 | 0.5 | AP SMG, Flash Pulse (+2B), Cybermine; Hacking Device, Sensor | — |
| 28 | 0 | MULTI Rifle, Light Flamethrower; Killer Hacking Device | — |
| 28 | 0.5 | MULTI Rifle, Light Flamethrower, D-Charges, AP Mine; Minelayer, Specialist Operative | — |
| 29 | 0 | MULTI Rifle, Light Flamethrower, D-Charges, Armed Turret (Combi Rifle); Specialist Operative | — |
| 26 | 0 | Boarding Shotgun (+1B), E/Mitter, Flash Pulse, D-Charges; Forward Observer | — |

## Canonical vanilla Fireteam chart

### Global limits

| Type | Limit |
|---|---:|
| Core | 0 |
| Haris | 1 |
| Duo | 2 |

All ordinary chart rows below have `min: 0` and `required: false`. The pools therefore define allowed membership and per-entry maxima; no mandatory anchor troop is added here.

### Nomads Fireteams I

**Type:** Duo

| Entry | Min | Max | Profile restriction / note |
|---|---:|---:|---|
| SECURITATE | 0 | 2 | — |
| GRENZER | 0 | 1 | — |
| KULAK | 0 | 2 | — |
| MOBILE BRIGADA | 0 | 2 | — |
| GECKO | 0 | 2 | — |
| MORLOCK | 0 | 2 | — |
| TASKMASTER | 0 | 1 | — |
| KRIZA BORAC | 0 | 1 | — |
| EVADER | 0 | 1 | — |
| GATOR | 0 | 1 | — |
| JAZZ | 0 | 1 | **FTO profile only** |

### Nomads Fireteams II

**Types:** Duo, Haris

| Entry | Min | Max | Profile restriction / note |
|---|---:|---:|---|
| MOBILE BRIGADA | 0 | 3 | — |
| KULAK | 0 | 2 | — |
| GRENZER | 0 | 1 | — |
| MARSPIDER | 0 | 1 | — |
| ROUNDER | 0 | 1 | — |

### Vanilla Wildcards

| Entry | Min | Max | Note |
|---|---:|---:|---|
| WOLFGANG AMADEUS | 0 | 1 | Wildcard |
| PERSEUS | 0 | 1 | Wildcard |

## Reverse Fireteam access index

| Troop / profile | Pool | Types | Max | Notes |
|---|---|---|---:|---|
| Securitate | Fireteams I | Duo | 2 | — |
| Grenzer | Fireteams I / II | Duo / Haris | 1 | — |
| Kulak | Fireteams I / II | Duo / Haris | 2 | — |
| Mobile Brigada | Fireteams I / II | Duo / Haris | 2 in I; 3 in II | — |
| Gecko | Fireteams I | Duo | 2 | — |
| Morlock | Fireteams I | Duo | 2 | — |
| Taskmaster | Fireteams I | Duo | 1 | — |
| Kriza Borac | Fireteams I | Duo | 1 | — |
| Evader | Fireteams I | Duo | 1 | — |
| Gator | Fireteams I | Duo | 1 | — |
| Jazz FTO | Fireteams I | Duo | 1 | **FTO profile only** |
| Marspider | Fireteams II | Duo / Haris | 1 | — |
| Rounder | Fireteams II | Duo / Haris | 1 | — |
| Wolfgang Amadeus Wolff | Wildcard | Any legal vanilla Fireteam | 1 | Wildcard |
| Perseus | Wildcard | Any legal vanilla Fireteam | 1 | Wildcard |

All standard roster entries absent from this reverse index have no Fireteam access in the pinned vanilla chart. In particular, an `FTO` label alone does not add Tsyklon, Vostok, Stempler, Switcher, Coyote, or Zoe profiles to vanilla Fireteams.

## Source relations

The vanilla source carries the following roster relations in addition to Fireteam membership:

- **Puppetactica Company:** PuppetBots are grouped with / dependent on the Puppet Master relation. This is roster construction logic, not a Fireteam.
- **Jelena Kovač:** ordinary unit ID `1550` ↔ Reinforcement ID `1739`.
- **Raoul Spector:** ordinary unit ID `1069` ↔ Reinforcement ID `1740`. The ordinary Raoul entry is not part of the 53-unit pinned standard vanilla resume, so this relation is recorded without adding Raoul to the standard roster.

## Reinforcement Fireteams — Vipera Pursuit Force

Linked Reinforcement army: **Vipera Pursuit Force (Army ID 599)**, source revision `7.26246.158`.

These rows are intentionally separate from the standard Vanilla Nomads Fireteam chart. The current Reinforcement source exposes global `spec` values of **Core 0; Haris 0; Duo 0** while its team rows explicitly declare Fireteam types. Both facts are preserved rather than synthesizing non-zero global caps.

### Vipera Reinforcement Fireteams

**Types explicitly listed by Army:** Duo, Haris, Core

| Entry | Min | Max | Required / counts-as note |
|---|---:|---:|---|
| MARSPIDER REINF. | 0 | 5 | `required: true`; counts as Vipera |
| KULAK REINF. | 0 | 4 | `required: true`; counts as Vipera |
| PROWLER REINF. | 0 | 2 | counts as Vipera |
| ROUNDER REINF. | 0 | 1 | — |

**Required-choice interpretation:** the two `required: true` rows are preserved as a required-choice set. A legal Vipera team must satisfy the chart's required member condition using Marspider and/or Kulak as defined by Army; this reference does **not** reinterpret the data as requiring both troop types simultaneously.

### Lizard Reinforcement Fireteam

**Type explicitly listed by Army:** Duo

| Entry | Min | Max | Note |
|---|---:|---:|---|
| LIZARD REINF. | 1 | 1 | Anchor |
| MARSPIDER REINF. | 0 | 1 | — |

### Reinforcement Wildcards

| Entry | Max | Counts as / note |
|---|---:|---|
| STEMPLER ZOND REINF. | 2 | — |
| TSYKLON REINF. | 2 | — |
| VOSTOK REINF. | 2 | — |
| JELENA KOVAČ REINF. | 1 | — |
| SPECTOR REINF. | 1 | Counts as Vipera |

## Validation notes

- Standard roster count reconciled to **53** ordinary matched-play entries after excluding `Vortex Spec-Ops` and `Nomads Team-Ops` optional modes and the later generic `merc-*` catalogue.
- Vanilla AVA is taken from the Nomads faction source and intentionally differs from sectorial AVA where the Army data differs.
- The complete standard vanilla Fireteam chart is represented: global Core 0 / Haris 1 / Duo 2; Nomads Fireteams I (Duo); Nomads Fireteams II (Duo/Haris); Wolfgang and Perseus Wildcards.
- Every ordinary vanilla chart row is `required: false`, `min: 0`; no anchor requirement is invented.
- `JAZZ FTO` profile-only Fireteam access is preserved. FTO-labelled Tsyklon, Vostok, Stempler, Switcher, Coyote and Zoe profiles are not granted vanilla Fireteam access because they are absent from the canonical vanilla chart.
- Puppetactica roster dependency is recorded as a source relation, not a Fireteam rule.
- Source relations for ordinary/Reinforcement Jelena Kovač and Raoul Spector are kept separate from Fireteam membership.
- Linked Reinforcement army resolves to **Vipera Pursuit Force (599)**. Its chart is kept separate, including the current source combination of global `spec` 0/0/0 and explicitly typed Core/Haris/Duo team rows.
- Vipera's multiple `required: true` rows are treated as a required-choice set rather than incorrectly requiring all marked rows simultaneously.
- Source data and Fireteam normalization were rechecked on **2026-10-15** against the pinned Army snapshot and InfinityDB commit listed in the front matter.

## Command-unit apex/value cross-reference (2026-10-23)

**Shifta CoC 21/0** provides an unusually cheap nonhackable, E/Marat/Disco Baller successor while adding actual DZ/mission denial. **Kulak CoC 23/0.5** has more direct assault potential but is not as economical when a sheltered backup is enough. A passive Interventor/Moderator LT with NCO exploitation is a different command architecture; **Shifta is not automatically legal in Bakunin, Corregidor or Tunguska**.

See [cross-game Lieutenant, CoC and Order-economy tiers](../../notes/list-building/command-units-apex-and-value.md). **Refer to this pinned roster/Fireteam chart for profile legality.**

## Mission specialist / button-pusher choices (N5.3)

**Shifta CoC21/0** is useful cheap succession that may also qualify for generic Specialist scoring; do not assume the profile is imported into sectorials. **Jazz/Moran** on the Vanilla roster where available supply complementary *backfield hacker + infiltrating FO* rather than redundant stationary specialists. **Evader Engineer vs SO** loadout and availability must be checked individually. Put a mission-scorer on a different flank from expensive attack Lieutenants.

[Cross-game apex and value specialist tier guide](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). The unit profiles/Fireteams above control exact legality.

## TAG tactical cross-reference (2026-10-23)

**Szalamandra HRMC (68)** is the concentrated long-range threat, **Gator MULTI HMG (73)** the armored NCO/TacAware/mine brawler, and **Gecko (49–55)** the budget TacAware/light-TAG angle and useful second TAG. Prefer cheaper Gecko when the plan needs two scoring axes; choose Gator when mine/close defence materially matters. Check the vanilla profile before assuming a Tunguska-only NCO benefit.

Cross-faction **apex vs points-value** comparisons, matchup table, and direct MCP-reviewed podcast/video sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Current profile and Fireteam legality above remain authoritative.

## Vehicle (VH) tactical cross-reference (2026-10-23)

**Go-Pod AVA1:** **33/0 MULTI Rifle/E/Mitter+Go-Bot** preserves precious SWC; **32/1.5 HRL+AP SMG** trades SWC for more direct firepower. Go-Bot gives a **Synchronized template/Flash Pulse fork**, not an extra Regular Order. **Disagreement:** some local scenes call it near-auto-include, while **Shepherd** argues ARM2/Mimetism(-3)/S7/No Cover and hostile Repeaters make it fragile. Best after a Nomad long gun/hacker clears serious AROs; reserve an exit Order.

See [VH apex/value tier list and matchup guide](../../notes/list-building/vehicles-vh.md). **This sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative.**

## Hacker and KHD tactical cross-reference (2026-10-23)

**Best routine duo:** **Interventor HD+ WIP15/BTS9 18–23/0.5** for safe White Noise/Oblivion, plus **Jazz HD+Trinity 25/0.5 + Billie** or another anti-Hacker for active control. **Mary Problems HD/KHD 27/0.5** uniquely gives forward Mimetism(-6), Climbing+ and a Pitcher; **Kulak KHD+Carbonite 20/0** and **Rounder HD+Trinity 21/0.5** are unusually inexpensive hybrids. **Zero KHD 22/0** scores from camouflage when hacking has no targets. **Opposing opinions:** Shepherd's Tunguska analysis prefers multiple cheap protected Interventors over Mary for long-term network control; Mary is preferable only when she personally needs forward position. Remember Jazz/Billie and Zoe/Π-Well are specific multi-model purchases, not generic extra orders.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

See the N5.3 [cross-game apex/value rankings and transcript-backed competing assessments](../../notes/list-building/cheerleaders-and-order-generators.md). The current roster and official Fireteam definitions above remain authoritative; unit access/cost may differ from vanilla.

- 7pt Transductor — cheap Regular Repeater/Flash REM (not a dedicated gunfighter); its S3 footprint and AVA constrain spam.
- 8pt Salyut — Baggage/Repeater Regular Order; reload support and deployment-zone density determine marginal value.
- 9pt Moderator — small-base Regular Fireteam/guard choice; compare against Transductor when an actual link or defence role is needed.
- 10pt Alguacil — inexpensive S2 Regular and Fireteam/LT material; upgrade only for a credible second job.
- 11pt Puppet Master — one Regular Order plus Counterintelligence; PuppetBots do not add Orders.

**Selection rule:** Count deployed, transferable Regular Orders per Combat Group, not total models or restricted bonus Orders; choose the lowest-cost protected Regular profile that *also* contributes a relevant Repeater, Baggage, Fireteam, template, ARO or Specialist job. Check Group slots and DZ hiding space before buying a third large-base REM or replacing a needed scoring piece.


## ARO apex/value cross-reference (2026-10-23)

The [N5.3 cross-faction ARO apex/value and matchup study](../../notes/list-building/aro-units-apex-and-value.md) compares hidden missile traps, Neurocinetics/TR, cheap templates/mines, DZ guards and conflicting creator opinions. Consult the **roster and Fireteam chart above** for legally available profiles, SWC, Training and AVA.

- **Reaktion 0SWC Thunderbolt TR** — 19pt recoverable midrange guard, complements a separate expensive gun/hidden layer
- **Triggerman Neurocinetics Sniper** — high-reactive-ceiling durable 47pt investment, but disputed versus cheaper TR + mine/hidden layers
- **PuppetBots + Master** — Flash/forward presence, Counterintelligence and activation compression; PuppetBots do not generate separate orders
- **Tsyklon Feuerbach/Pitcher FTO** — ranged defense and forward repeater pressure; only link when chart authorizes FTO
- **Moran Koala+Repeater** — route and hacking ARO rather than pure FtF shooting; particularly strong defending access squares

**Practical deployment:** put cheap disposable/Flash/DTW or mine pressure on the approach; retain a separate unseen or recoverable threat for the decisive square; avoid exposing a premium active attacker and check opponent Smoke, MSV, hacking, AD and pie-slicing. No automatic order from an off-table Hidden model; Irregular ARO units do not supply generic Regular Orders.
