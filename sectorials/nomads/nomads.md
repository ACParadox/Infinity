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

**Unit selection evidence (23 Oct 2026):** [Nomads source-backed four-roster must-have / go-to / avoid audit](#must-have--go-to--avoid--source-backed-recommendations-2026). Tactical opinion only; the roster and Fireteam chart in this file remain authoritative.


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

## Airborne and enemy-DZ attack choices — N5.3 (2026-10-23)

**Hellcat BSG19/0, Bearcat KHD29–30/0, Meteor Repeater+Sensor19–21** cover three different AD jobs: *sacrifice/Adhesive trade*, **self-contained anti-Hacker/specialist fighter**, and **hacking-network projection**. Do not import **Carlota Parachutist(DZ)** or Corregidor Surface/Deepspace Fireteam structures unless current **Vanilla** list grants that option. **Meteor** has no automatic damage output without a real hacker/missile system. If target is one 10pt Order, a 64pt premium attacker is poor even if it reaches the backline.

See [current cross-game apex/value, landing odds and expected-trade tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **This roster and Fireteam chart control exact loadout/availability.**

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **Kriza Borac HMG45/1.5** is a strong **non-TAG** +1B/BS Attack(-3) FtF option, while **Vostok Mk12 38/0 or Spitfire37/1** trades raw Burst for Mimetism(-6), Climbing and 2STR recovery. **Intruder HMG38/1.5** supplies different Camo/MSV2/smoke attacks when vision MODs are main obstacle. **Szalamandra HRMC68/2** is the separate heavy **TAG** AP volume option when the list can still afford specialist/support redundancy. Vanilla FTO tags alone do not authorize Fireteam bonuses. [Combat apex/value with TAGs separately ranked](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## Warbands and inexpensive trading roles — N5.3

**Morlock Chain+Smoke+E/M CC6/0** is a standout *TAG disabling* budget piece only when a legal melee route exists: E/M CC requires **Silhouette contact**, unlike ranged Ghazi E/Marat. **McMurrough23/0** is the durable template/smoke+AP+DA alternative for 2+ turn threat, but Irregular+Impetuous. **Do not import Corregidor Jaguar/Diablo FT bonus or Bakunin Morlock AVA Total** into Vanilla. Smoke can feed legal **Intruder MSV2**, while Hackers/Repeaters often disable TAGs more safely than running a 6pt Morlock across open lanes.

[Cross-game warband/cheap-trader apex and value tiers, targets and command packages](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). Profile-specific sectorial legality/Fireteams above control all selections.

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

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Clockmaker18 WIP15 + Zondbot3** is standout pure **REM/TAG** insurance: 75% initial Engineer roll, up to **93.75%** with a legal Remote Presence Command Token reroll. **Daktari14 WIP13** handles VITA; **Sophotect-like dual roles aren't free**, so buy **Evader/Zoë/other combat Engineer** only when hacking/attack utility will be used. Two Zondbots in separate safe corners are better than clustering both beside the gun. [Doctor/Engineer apex/value, odds and media disagreement](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## N5.3 midfield area denial / speed bumps (tactical synthesis)

**Vanilla Moran AVA1** (Corregidor AVA2): the **15/.5 BSG + Repeater + CrazyKoala Minelayer** is excellent turn-zero physical/hacking denial, but cannot cover both flanks alone; pair it with a **Zero/ Spektr marker**, mobile Repeater/Pitcher or cheap template guard. The one-use Camo Moran is a **separate profile** without Repeater. **Counterpoint:** investing further in hacker/Guided packages can starve the army of independent shooters and SWC. Read exact vanilla AVA before copying Corregidor two-Moran advice.

[Cross-game apex/value and transcript analysis](../../notes/list-building/midfield-area-denial-and-speed-bumps-apex-value.md). This is tactical synthesis; exact loadouts and Fireteams remain above.

## N5.3 DZ defense / anti-alpha-strike tactical choices

**Warcor 360º3/0** (Irregular) provides cheap edge/rear Flash; **Transductor7/0 Flash+Repeater** is the Regular order/ARO filler; **Salyut8/0 Baggage+Repeater+Deactivator** is additional Regular logistic support behind the breach. **Moran15/.5 Repeater+CrazyKoala Minelayer** protects a *midfield approach*, but **vanilla AVA1**, and **Boost does not trigger against IMP/Camo markers**; it is not a complete anti-Fiday screen. Use a cheap template/flash/short-range defender at the next DZ corner and disperse Jazz/Interventors/Engineer to avoid one attacker chaining through all three. **Counter:** extra repeater/hacker/Guided expense can consume SWC and leave no conventional counterattack; physical backstop still needed.

[Whole-game DZ-defender apex/value guide, counters and transcripts](../../notes/list-building/dz-defenders-alpha-strike-and-impersonation-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Nomad smoke/templates** and legal **Morlock** cheap E/M CCW route are usually better *points value* than a premium melee-only fighter; **E/M attack on Hackable TAG/HI** is the specific trade-up target, not automatic damage into VITA LI. **Moran/Camo midfield guns/Repeaters** help disable the victim before reaching contact. **McMurrough** or other mercenary body, only where current rostered, buys smoke and high-PH 2W repeated assault at a higher investment. Fight NBW/Guard from outside LoF/ZoC if possible. [Dedicated CC assassin apex/value, delivery and counter-CC](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## N5.3 network projection — Pitchers, Repeaters, TinBots and disposable delivery

**Vanilla nominal network:** **Moran Repeater+Koala FO15/.5** is exceptional forward Turn-0 coverage, but **AVA1** (CJC has 2). **Moderator Pitcher10/0** is cheap Regular Order + 2-shot projector, unlinked **BS10** is shaky; **Jazz+Billie25/.5** combines HD+/Trinity/Pitcher with two Regular Orders and Billie Repeater; FTO Jazz22/.5 lacks Billie. **Meteor19/0** delivers a *native* Repeater by Combat Jump/Parachutist; **Transductor7/0** is a cheap Regular native-Repeater kamikaze option. **Tsyklon FTO Pitcher26–29/1 has NO vanilla Fireteam access** solely from its FTO label. **Dispute:** cheap versatile Vanilla network versus linked Tunguska special-die efficiency; save SWC for actual attacks when Guided is weak.

[Cross-game apex/value guide, exact delivery cost and transcript disagreements](../../notes/list-building/network-projection-repeaters-pitchers-apex-value.md). Profile and Fireteam tables above remain authoritative.

## N5.3 rare abilities & unusual combinations — tactical synthesis

**Vanilla Puppetactica**: **11pt Puppet Master + 9pt FO PuppetBot** is a **20pt+ Control/Transmutation specialist package**, not a 9pt standalone model/Order. **Chimera+3 Pupniks19/0** has rare **Eclipse+Viral CC+NBW/Climbing+** with synchronized forks but Impetuous/no Cover risks. **Coyote+attached BambaBot** versus **Coyote27+independent BambaDroid FO13** are completely different structures (latter roster-dependent and cannot assume AVA/FT from CJC). **Opposing:** puppet/Überfall bundles can improve physical board control without Guided, but adding them atop Jazz/Moran/Vertigo and TAGs may crowd out 10–15pt Regular Order support.

[Whole-game rare capability apex/value, rules, matchups and opposing MCP transcripts](../../notes/list-building/rare-capabilities-and-unique-combinations-apex-value.md). Use current profile and Fireteam chart above.

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Morlock6 E/M CCW+Smoke** is a minimal-cost anti-Hackable HI/TAG trade only if **base contact** is plausible; **Meteor Zond21 E/M Carbine airborne** offers flank fire, **Tsyklon Feuerbach29/1** sustained B2 AP+DA, **Evader Engineer29 Panzerfaust** role compression. **Moderator9 E/M Carbine** and **Corregidor cross-sectorial tech** depend on legal vanilla list profile. Against BS15 TAG, aim for Mimetism/cover/Repeaters-as-screen even with **no hacking** in this analysis; do not rate hacker-assisted Spotlight as a free anti-armor shot. [Anti-TAG/HI non-hacking apex/value rankings](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## Tactical cross-reference — indirect fire (2026-10-23)

**Vanilla Guided:** **Vertigo16/1.5** is strongest when **Interventor/Jazz/Mary** and existing Pitchers/Repeaters/one **Moran AVA1** already control hacking areas. The active Spotlight B2 **requires failed AP/BTS Saving Roll** to apply Targeted; enemy can still Reset/Dodge a subsequent Guided B1 attack. Tactical Awareness contrasts a missile-first named-hacker swarm with REM-centric direct shooting; do **not** import the two-Moran Corregidor shell to vanilla. [Indirect apex/value and source disagreement](../../notes/list-building/indirect-fire-speculative-guided-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Gecko Vulkan49/0** is standout cheap **TAG quadrant VP** (STR3/ARM6, TA) with chain template; **Szalamandra HRMC68/2** (STR3/ARM8/BTS9), **Gator73/1.5** (STR3/ARM8/TA/NCO) higher ranged ceiling but fewer independent objective troops. **Puppet Master11/0+FO PuppetBot9/0 =20/0 dependent** protects scoring by distributed bodies, **not 2 Regular Orders**; **Chimera+Pupniks19/0** Eclipse/multiple template/CC bodies screens dangerous entry squares. **Mobile Brigada Hacker36/.5** is actual W2/ARM5/BTS3 specialist; **27/0 BSG** is a 2W zone holder but *not* Specialist. **Opposing MetaChemistry/WIP12:** don't buy TAG plus puppet plus all-in Guided if it leaves too few 20–30pt models able to pick up/survive a box; a 15pt Moran in cover denies enemy access economically.

[Whole-game objective holding/zone apex/value, scenario scoring and opposing media](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Actual sectorial profiles and Fireteam chart remain authoritative.

## Force multipliers — N5.3 role/value cross-reference (2026-10-23)

**Salyut8 Baggage/Repeater vs14/.5 EVO**: the upgrade pays when **Vostok/Tsyklon/Rui Shi-equivalent eligible REM** attacks under Assisted Fire or a meaningful airborne/REM Supportware plan exists. Baggage reloads Pitchers/Mine Dispensers within ZoC or automatically States Phase; *does not* restore Non-Reloadable deployables. **Firewall TinBot benefits legal team only**; standalone Jazz+Billie has its own native repeater network, not magically armywide TinBot protection. **TAG-Treiber** eligibility must be verified from the selected roster. [Global role/value](../../notes/list-building/force-multipliers-special-abilities-apex-value.md).

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Interventor HD+18–23/.5 or Jazz HD+25/.5 + an actual Repeater network** projects **White Noise** against enemy MSV/Marksmanship; it does not block ordinary non-visor shooting. **Stempler FO/Sensor REM** is the budget Camo/Hidden ZoC detector; **Meteor Zond Sensor19–21** changes the angle with airborne entry but adds insertion risk. **Intruder MSV2 HMG** actively kills revealed Mimetism/Smoke defenders with legal Smoke support. **Kulak KHD20/0 Disco** gives **Eclipse, not White Noise**. **Counter:** all-visor defenses are vulnerable to enemy White Noise/Albedo; retain a non-visor gun and an objective runner.

[Cross-game anti-tech N5.3 apex/value, mechanics, matchups and checked conflicting transcripts](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## N5.3 peripheral / synchronized / multi-body apex-value update

**Apex cheap Control assault:** **Chimera+3 Pupniks19/0** supplies *four bodies moving on one activation*, Eclipse + Viral/DA CC and Climbing+, but only **one target-capable Spearhead** joins Chimera on target-requiring attack; clustered templates and killing fragile parent defeat the pack. **Puppetactica 11/0 Master + 9/0 FO PuppetBot(s)** yields remote 2W/Transmutation pickets plus Counterintelligence, **minimum20/0, useful two FO bots29/0**, NOT 2/3 extra pooled Orders; 14pt AP MMR and 16pt/1.5 Red Fury are alternate **paid** Spearheads. **Zondnautica BSG+ZondMate17/0** fast Impetuous vehicle that transforms to synchronized rider/bot, *not* two independent troopers. **Coyote BSG27/0+attached BambaBot** and **BambaDroid FO13/0** are fundamentally different: actual FO Droid is separately bought and requires Coyote same Combat Group. **Fiddler43/0 two JackBots** where legal gives Vulkan/Explode synchronized split attacks, **29/0 FTO has none**. **Opposing Shepherd/TA/Meta:** FO PuppetBots as cheap defenses vs Red Fury/EVO offense; protected Master or AD assassination determines if the extra bot points pay.

[Whole-game N5.3 Peripheral & Multi-Body Apex/Value guide](../../notes/list-building/peripheral-synchronized-multibody-apex-value.md). Source profiles, dependency and Fireteam tables above remain authoritative; media are opinions.

## Mission performance — battle-report evidence (2026-11-01)

| Mission(s) | Tested composition / scoring mechanism | Evidence |
|---|---|---|
| **B-Pong / beacon** | Zero / fast hacker, Moran Koalas/Repeater and Interventor/Jazz network protect pickup/withdrawal; strong counter-Pitchers require a safe alternate lane. | [#034](../../notes/battle-reports/031-040-n5-battle-report-tactical-analysis.md) |
| **Provisioning / cargo** | Hellcat Super-Jump pickup plus hacker/Pitcher protection and independent Specialists outscored a White Banner elite HI roster. | [#090](../../notes/battle-reports/081-090-n5-battle-report-tactical-analysis.md) |
| **Last Launch / extraction** | Moran/Chimera/Pupnik/Koala/Interventor/Gecko screens preserved a successful early extraction against Yu Jing's final close push. | [#201](../../notes/battle-reports/201-210-n5-battle-report-tactical-analysis.md) |
| **Uplink Center / late zone** | Jazz/Interventor/Kulak, Puppet FO/Zero and Moran can press objective rooms, with a recorded 3–3 against Kosmoflot. | [#230](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) |

**Limits:** These are **vanilla Nomads** mixtures, not proof that every model may appear together in Bakunin/Tunguska/Corregidor. Game-era qualitative evidence, not a win-rate or current Fireteam claim. [Full mission evidence audit](../../notes/battle-reports/cross-report-mission-performance-by-sectorial.md).

## Counterplay — observed N5 battle-report responses (2026-11-02)

| Threat / target | Observed response and limitation | Battle reports |
|---|---|---|
| **Vs hackable White Banner HI** | Protected Pitcher/Interventor/Jazz network plus Hellcat Super-Jump safely picked up Provisioning box while opponent's elite HI survived but couldn't score. | [#090](../../notes/battle-reports/081-090-n5-battle-report-tactical-analysis.md) |
| **Vs EI elite attack** | Fiddler/Jackbots and held Hellcat Hacker secured final Corporate Classified after Sheskiin alpha triggered Retreat incorrectly for opponent's plan (5–4). | [#139](../../notes/battle-reports/131-140-n5-battle-report-tactical-analysis.md) |
| **Vs Yu Jing gun Haris** | Moran CrazyKoala, Chimera/Pupnik, Morlock Smoke, Interventor and cheap bodies forced Zuyong/Rui Shi to spend too many Orders before Last Launch extraction (6–4). | [#201](../../notes/battle-reports/201-210-n5-battle-report-tactical-analysis.md) |

**Limit:** These played vanilla mixtures do not imply all named profiles co-exist in a single Nomads sectorial. Protect support Hacker from counter-pitcher. These are historical qualitative interactions, not current N5.3 profile/Fireteam or faction win-rate claims. [Full cross-report counterplay analysis](../../notes/battle-reports/n5-cross-report-counterplay-tags-hi-hacking-camo-impersonators-fireteams.md).

---

## Must-have / Go-to / Avoid — source-backed recommendations (2026)

Dated source-backed tactical preferences and miniature purchasing priorities; opinions do not override N5.3 roster, profile or Fireteam data above.

**Original audit title:** Nomads — Vanilla, Corregidor, Bakunin, Tunguska: Must-have / Go-to / Avoid

*Source-backed list-building audit — 23 October 2026. Applies to the canonical [Vanilla Nomads](nomads.md), [Corregidor](corregidor.md), [Bakunin](bakunin.md), and [Tunguska](tunguska.md) N5.3 rosters, pinned to the **3 September 2026 Army data**. These are named-player tactical opinions and tested constructions, **not measured global tournament pick rates**. Latest main's profile/AVA/Fireteam source controls over any 2024–2026 video. Full tactical companions: [Vanilla](../../notes/factions/vanilla-nomads.md), [CJC](../../notes/factions/corregidor.md), [Bakunin](../../notes/factions/bakunin.md), [Tunguska](../../notes/factions/tunguska.md).*

### Classification standard

- **Must-have / near-must:** a recorded presenter explicitly says “every list”, “always” or “auto-include”; or independently supported recurrent list core. Only “near-must” when credible examples omit it. The *job* can be essential without a particular unit being compulsory.
- **Go-to:** outstanding reliable value for its **actual job**, but list architecture, mission, terrain or overlapping tools can make it unnecessary. Do not assume all go-tos go into one 300-point list.
- **Never take / strong avoid:** direct recorded critique **of the named profile**, preferably comparing a same-faction replacement. Mark **contested/conditional** where a different speaker defends it, a current changed roster undermines the critique, or it has a real special use. None of the four armies has a supported universal ban covering every profile of an entire multi-role unit.
- Evidence marks: **explicit** = reviewer states the near-auto/negative claim; **repeat** = published list examples, not population statistics; **reasoned** = synthesis of reviewer observations + current roster, and therefore *not* pretended to be a direct podcast verdict.

### 1. Vanilla Nomads (Army 501)

**Near-must / most convincing defaults**

| Current profile | Why; why it is not literally universal | Direct recordings |
|---|---|---|
| **2× Morlocks 6/0** (AVA2) | Smoke, MA and Chain Rifle at an absurdly low points cost; place on separate approach lanes to screen expensive hacker/gun bodies and trade upward. **Irregular/Impetuous**, so check combat-group spendable Regular Orders. **Very strong personal auto-include**, not meta-wide quantitative consensus. | **[Robert Shepherd — N5 Vanilla Nomads Faction Focus (2026)](https://www.youtube.com/watch?v=dOtvw5FKOfo)** *explicitly states he basically always takes two in every Vanilla list*. |
| **Moran Repeater BSG 15/.5** (AVA1) | Infiltration, CrazyKoalas and a midfield Repeater create hacking defense and order tax from deployment. A 17/.5 rifle repeater is an alternative if range/D-Charges matter. The 16/18pt **Camo(1-use) Moran is not the Repeater profile**. **Near-universal first consideration**, but two-moran historical advice is illegal in Vanilla (AVA1). | **[Shepherd Vanilla 2026](https://www.youtube.com/watch?v=dOtvw5FKOfo)** calls it the next sensible inclusion after Morlocks; **[Tactical Awareness S3E26 Nomad Prime](https://open.spotify.com/episode/2PpxuDu2WlxipiqpVzHTdv)** explores hacker/Guided/network alternatives. |

**Go-to; any one can be the right pick without being mandatory**

| Unit | Why, when, alternatives | Transcript support |
|---|---|---|
| **Interventor HD+ 18–23/.5; KHD18/0** | WIP15 BTS9 efficient hacking, White Noise/Spotlight/Oblivion and optional FastPanda; one HD+ plus a KHD may be enough when a shooter and scoring units need points. **Interventor LT** is efficient, but is a potentially obvious, vulnerable 1W commander. | [Tactical Awareness Vanilla](https://open.spotify.com/episode/2PpxuDu2WlxipiqpVzHTdv); [Dante Vanilla N5](https://www.youtube.com/watch?v=hJKOZF1Je_g); [Shepherd Vanilla](https://www.youtube.com/watch?v=dOtvw5FKOfo). |
| **Jazz & Billie 25/.5** vs **Jazz FTO22/.5** | Billie variant supplies second Regular Order and extra Repeater/mine; FTO variant can use the *specific* Vanilla Fireteam I chart but loses Billie. Pick to complement your Repeater architecture; need not stack every hacker. | [TA Nomad Prime](https://open.spotify.com/episode/2PpxuDu2WlxipiqpVzHTdv); [Dante Vanilla](https://www.youtube.com/watch?v=hJKOZF1Je_g). |
| **Puppet Master11 + optional FO PuppetBots9** | Cheap Regular controller plus inexpensive 2W-style S1 defensive/order-tax and specialist bodies; controller required for bots and **bots do not produce separate Regular Orders**. Current Vanilla reference lists Master11/13/16; do not infer Tunguska-only Fireteam privileges. | [Shepherd Vanilla](https://www.youtube.com/watch?v=dOtvw5FKOfo) and [Shepherd Tunguska](https://www.youtube.com/watch?v=A2eKdenbcsw) emphasize low-investment ablative guards. |
| **Zero / Spektr**; **Stempler Sensor/FO/TacAware15–22**; **Transductor7 / Salyut8** | Independent scoring, second-flank defense and cheap Regular/Repeater support, particularly because Vanilla Moran is AVA1. Stempler18 with **TacAware** is self-mobilizing; **FTO-labelled Vostok/Tsyklon do NOT join Vanilla Fireteams**. | [Dante Vanilla](https://www.youtube.com/watch?v=hJKOZF1Je_g); [TA Nomad Prime](https://open.spotify.com/episode/2PpxuDu2WlxipiqpVzHTdv); [Shepherd Vanilla](https://www.youtube.com/watch?v=dOtvw5FKOfo). |
| **Szalamandra68/2** or **Gator73/1.5** or **Gecko49–55**; **Vostok34–38** | Explicitly choose a real gun: Szalamandra HRMC for hard long AROs, Gator NCO/TacAware/mines for flexible pressure, Gecko for inexpensive durable midrange, solo Vostok Mimetism(-6) with EVO/Engineer support. **No TAG is auto-include**. | [Loss of Lieutenant N5 TAG panel](https://open.spotify.com/episode/1h5CJfZC5zBPxdg66o7xIN); [TA Nomad Prime](https://open.spotify.com/episode/2PpxuDu2WlxipiqpVzHTdv); [Shepherd Vanilla](https://www.youtube.com/watch?v=dOtvw5FKOfo). |

**Explicit criticism, only valid within its role**

| Profile | Verdict and same-roster competition | Direct criticism and caveat |
|---|---|---|
| **Grenzer MULTI Sniper32/1.5** as an **unlinked default primary sniper** | **Strong avoid**: a 1W BS13/MSV1/Marksmanship gun uses the SWC of powerful dedicated ranged answers. **Intruder38/1.5** with MSV2/Camo is the more expensive high-ceiling competitor, while TAG guns fill different roles. | [Shepherd Vanilla 2026](https://www.youtube.com/watch?v=dOtvw5FKOfo) explicitly says the Grenzer sniper is “kind of bad” and advises not taking it. **Not strict dominance:** Grenzer has different availability/Fireteam/Anti-Camo utility; [Tunguska](../../notes/factions/tunguska.md) may link it, so don't transfer the *unlinked* verdict indiscriminately. |
| **Go-Pod32–33** as the **sole Turn 1 ARO-breaker** | **Avoid that role**: S7/No Cover/ARM2 and hackability give an extremely low safety floor. As post-clearance fast finisher, E/M flanker or Go-Bot fork it is genuinely different from a main TAG. | [Shepherd Tunguska](https://www.youtube.com/watch?v=A2eKdenbcsw) 60–69m negative; [Dante Vanilla](https://www.youtube.com/watch?v=hJKOZF1Je_g) more positive on mobility. **Contested, not never.** |

### Fast starting template (not a fixed shopping list)

| Army | **Near-default consideration** | Add **one** game plan | First cuts when over budget |
|---|---|---|---|
| **Vanilla** | Morlock ×1–2; Moran Repeater ×1; a hacker (Interventor/Jazz) and cheap Regular support | Szalamandra/Gator/Gecko gun, Guided network, or solo assisted Vostok + mission specialists | Unlinked Grenzer sniper; Go-Pod if acting as first ARO gun; duplicate high-price hackers |
| **Corregidor** | Moran Repeater ×1–2, Jazz, a real long gun (Intruder sniper often) | Deepspace Gecko/Evader/Stempler **or** Surface Territorial/Coyote/Bearcat; smoke/MSV | Territorial AP Red Fury when 0SWC MMR suffices; unnecessary Tomcat vs Hellcat overlap; Guided without targets |
| **Bakunin** | Morlock ×1, one path-control/CC threat, a real gun and a specialist | Chimera/Cenobite zone assault; Riot/Uhahu protected network; Vostok/Clockmaker or Lizard/Stigmata gun/denial | Generic Zellen as duplicate Morlock role; Moderator Spitfire; unplanned Go-Pod |
| **Tunguska** | Puppet Master11, Interventor HD+, cheap Transductors/warband screen | Hollow Men/Perseus team; Kriza/Szalamandra gun; Pitcher/Heckler/Meteor program | 40+pt Triggermen with no distinct role; unlinked Grenzer costly gun; Go-Pod before safer first attacker |

### Primary evidence queue — directly checked with connected video/podcast transcripts

| Priority | Recording | Most important directly grounded point |
|---|---|---|
| 1 | **[Robert Shepherd — Vanilla Nomads, 2026](https://www.youtube.com/watch?v=dOtvw5FKOfo)** | Explicit **two Morlocks**, Moran baseline; explicit Grenzer-sniper skepticism; network versus real guns |
| 2 | **[WIP12 E208 — Corregidor Post-Mazebreaker, June 2026](https://open.spotify.com/episode/342lz18SRGSZ8QWf1Zg3Z9)** | Intruder MULTI Sniper near-auto speaker's list; 2026 Vostok reappraisal; Gecko-Evader-Stempler; Surface Territorial MMR; **self-corrected “never Tomcat”** |
| 3 | **[Shepherd — Bakunin N5](https://www.youtube.com/watch?v=firJVr1eDWg)** | Morlock-over-Zellenkrieger explicit; Moderator Spitfire explicit avoid; Chimera strong but high-skill; Vostok teams |
| 4 | **[MetaChemistry #132 — Bakunin tournament winner](https://open.spotify.com/episode/1S2sIe6nlefj4TZlZuII9g)** | **No Stigmata/Go-Pod/Guided**, minimal hacking, Orphan MSV2 anti-smoke; third-party Go-Pod auto-include claim **and** winner's own nonuse |
| 5 | **[Shepherd — Tunguska N5](https://www.youtube.com/watch?v=A2eKdenbcsw)** | Explicit Puppet Master **basically always**; Interventor/Hollow Men; Go-Pod low-floor and Triggermen criticism |
| 6 | **[MetaChemistry #129 — Tunguska Takedown](https://open.spotify.com/episode/6XSTLXqQUFcjv9lYcDTZ6g)** | Elite Interventor hacking, expensive guns, **Denma/Zellen nearly every list**, opponents beat hacking/CC exposure |
| 7 | **[Tactical Awareness Tunguska](https://www.youtube.com/watch?v=PFAewbgodZc)** | Competing ambitious Go-Pod, Puppet-Red-Fury, Kriza and Triggermen ideas |
| 8 | **[Tactical Awareness Nomad Prime](https://open.spotify.com/episode/2PpxuDu2WlxipiqpVzHTdv)** | Gecko gun, mass hacking/Guided, EVO REM as three valid but mutually competing Vanila approaches |
| 9 | **[Dante Vanilla N5](https://www.youtube.com/watch?v=hJKOZF1Je_g)** · **[Dante Bakunin](https://www.youtube.com/watch?v=DVOHynBsg6o)** | Older opposing views on nomad hacker/REM utility and Riot-versus-Reverend efficiency |
| 10 | **[Tactical Awareness CJC](https://open.spotify.com/episode/1ngCemrrDVMMDgvWjNBMYY)** · **[Loss of Lieutenant TAG debate](https://open.spotify.com/episode/1h5CJfZC5zBPxdg66o7xIN)** | Mixed TAG and infrastructure builds; premium gun opportunity costs |

#### N5.3 guardrails

- **Do not transplant list legality across ships**. Corregidor **Surface and Deepspace are different selectable divisions**; Vostok/Jazz **FTO** variants are not always the same as their independent profile. Vanilla has **0 Core / 1 Haris / 2 Duo**; no general Fireteam privilege follows from the string `FTO`.
- **Lunokhod** footage in older Nomad analyses does **not** describe a unit in the pinned ordinary rosters; don't suggest the removed model as current go-to. **Bakunin Zoe standalone 23pt** in older footage is not current ordinary roster access: pinned Bakunin has paired Zoe+Π-Well FTO instead.
- **Go-Pod** and premium hackers have real, explicit opposing opinions. **Do not flatten** them into unambiguous auto-include or never-purchase verdicts.
- An interviewer calling a piece "auto-include" in **their personal event list** is **not** proof it is on every successful list. A unit absent from one tournament winner is likewise **not proof it is bad**.

### Whole-unit purchasing audit — skip the model, not one loadout (2026-10-30)

**No uncontested full-unit never-buy** is established for any of these four rosters. The following **model-level deferrals** are useful when choosing what to *purchase first*, but the stated niche or dissent prevents a categorical ban.

| Army | Entire model/unit to defer | Why / when to buy instead |
|---|---|---|
| **Vanilla Nomads** | **No supported whole-unit skip** | Grenzer **unlinked sniper** competes poorly with Intruder; Grenzer's other profiles/sectorial links remain different. Go-Pod as first-turn linebreaker is risky, but late mobility is a real role. |
| **Corregidor** | **No supported whole-unit skip** | Territorial AP Red Fury versus MMR, Tomcat versus Hellcat and Gecko Vulkan versus MMR are **loadout/role** comparisons, not reasons to avoid the whole unit. |
| **Bakunin — Zellenkrieger** | **Defer generic Zellenkrieger purchase** if you already use **Morlocks** for smoke/trades | [Shepherd Bakunin](https://www.youtube.com/watch?v=firJVr1eDWg) directly favors 6pt Morlock to generic 8pt Zellen. **Do not label all Zellenkrieger forbidden:** the FTO's Taskmaster/Riot synergies and Natural Born Warrior/other attributes create genuine choices. **Extreme Zellenkrieger** is *a different unit* and not covered by this verdict. |
| **Tunguska — Triggermen** | **Defer as a first premium gun/ARO miniature; disputed** | [Shepherd Tunguska](https://www.youtube.com/watch?v=A2eKdenbcsw) prefers Kriza HMG or much cheaper Reaktion for common roles; **K1 Decoy/Forward Deploy** and Tactical Awareness sniper experiments provide special uses. |
| **Tunguska — Go-Pod** | **Defer if you need a Turn-1 main attacker** | No Cover/S7/hackability is a bad ARO-breaking floor, but fast late flanking/Go-Bot tricks are unique; [Tactical Awareness](https://www.youtube.com/watch?v=PFAewbgodZc) offers an opposing positive interpretation. |

**Not model-level:** Moderator Spitfire and Grenzer Sniper are weapon/profile negatives; don't skip the whole Moderator/Grenzer miniature family. [Cross-faction shortlist](../../notes/factions/model-purchase-avoid-summary-2026.md).

### Worst-value, rarely necessary and proxy-first miniature purchases by army (2026-10-30)

**Question answered:** which entire Nomads *miniatures* are a low-priority buy, which profiles should usually be avoided even though their unit has good options, and which **perfectly useful** miniatures or extra copies can be **proxied before buying**? This is a *shopping order*, not a new “never take” consensus or a claim about measured tournament frequency. **“Rare / circumstantial” here means not needed for ordinary first-choice list architectures in the recorded commentary**; the source videos/podcasts do not provide a reliable pick-rate survey. Latest [N5.3 army/sectorial data]() is the authority for profiles, availability, silhouette and Fireteam memberships.

**Strength of the verdict:** **Skip by default; proxy if needed** is a genuine *whole-model purchasing* deferral grounded in a speaker’s negative everyday-role comparison. **Proxy/test before buying** is an *inference* from credible niches and opportunity cost, **not** a speaker's assertion of overall weakness. **Avoid profile only** means the *other loadouts/sculpts of the unit remain worthwhile*. **Proxy another copy** refers to duplicate physical models or weapon sculpts, not a ban on a legal simultaneous AVA. **Contested** keeps materially opposing speaker/tournament evidence visible.

#### 1. Vanilla Nomads — worst roles and unnecessary premium purchases

| Unit / specific use | Why it is a weak default or uncommon requirement | Miniature recommendation / counterargument |
|---|---|---|
| **Grenzer MULTI Sniper as an unlinked default ARO or active long gun** | **Direct negative** — [Shepherd Vanilla](https://www.youtube.com/watch?v=dOtvw5FKOfo) calls the 32pt/1.5SWC profile **“kind of bad”** outside its role; compare **Intruder MULTI Sniper**, other long guns or cheap Reaktion denial. Grenzer’s MSV/Sensor/NCO and some legal Vanilla small-team roles differ. | **Avoid this *sniper profile*; do not reject the complete Grenzer troop**. **Proxy** an occasional unlinked sniper variant with a correct-size unused MI/sniper sculpt. Tunguska has different legal links, so do not transfer the vanilla judgment. |
| **Go-Pod as Turn-1 main ARO breaker** | **Directly contested** — [Shepherd Tunguska review](https://www.youtube.com/watch?v=A2eKdenbcsw) rejects sending **S7, No Cover, ARM2, hackable** aerial VH into prepared defenses; [Dante Vanilla](https://www.youtube.com/watch?v=hJKOZF1Je_g) values fast flank/mobility after safer attackers clear threats. **Go-Bot** and late scoring/EMP are distinctive. | **Proxy/test whole vehicle first**, especially if it would be your only primary gun. **Not a hard never buy**: acquire when a repeated turn-2/3 mission route actually needs its movement. Use a suitable **S7/Vehicle** footprint, not infantry. |
| **Triggermen as a first generic expensive shooter** | **Cross-roster inference, with direct Tunguska skepticism:** 43–47pt investment offers specific K1/Neurocinetics/Decoy or forward utility but can be inferior at ordinary gun-opening to **Kriza45 HMG** or a TAG, and at cheap ARO to **Reaktion19/24**. Vanilla lacks a reason to collect every rare HI alternative. | **Skip blind purchase; proxy first** for a particular **K1/Decoy defensive or anti-ARM** mission. No assertion that unique Triggermen options are strictly dominated. |
| **Several full-cost hackers with identical network tasks** (e.g., extra Interventor, Mary, Heckler KHD, Jazz) | **Reasoned** — Interventor HD+, Jazz+Billie, Mary’s Oblivion(+1B)/Trinity, Heckler midfield FastPanda are *different*, but three expensive operators defending the same Repeater grid can sacrifice scoring and gunfighting. [Vanilla guide](../../notes/factions/vanilla-nomads.md). | **Proxy the *additional* named hacker before buying**; normally start with **one coherent network + one way to shoot/score**, not all hackers. **Do not skip an Interventor or Jazz on a single-profile critique**. |
| **Third expensive gun/attack HI or alternate TAG** (Gator, Szalamandra, Gecko, Kriza, Mobile Brigada) | **Reasoned/role-based:** **Szalamandra HRMC**, **Gator NCO/TacAware**, **Gecko compact midrange**, **Kriza burst** are distinct good choices, but a list that only has Orders for one attacking platform rarely justifies buying all chassis. A single extra TAG can crowd the Hacker and Engineer plan. | **Proxy the different TAG/chassis before purchasing**; buy **one proven main platform** and test alternates. If two TAGs appear **simultaneously**, use two correctly sized models. No universal TAG “worst” classification. |
| **Vertigo Guided Zond with no viable Spotlight/Targeted route** | **Reasoned; [Vanilla guide](../../notes/factions/vanilla-nomads.md):** a 16pt/1.5SWC Guided missile needs real projected Repeaters, hackers, targetable enemy positions and *Orders*. Without that, it loses SWC to a direct shooter. **Normal network tools may still be excellent.** | **Avoid unsupported Guided *loadout/strategy***, **not all Nomads REMs**. Use appropriate REM chassis as a temporary Vertigo proxy; do not buy separate artillery solely because you own a Hacker. |
| **Zoe & Π-Well / Puppetactica / Überfallkommando as unplanned add-on teams** | **Low-confidence shopping inference, not weak:** these are **compound/controlled teams** with additional body count and specialist defensive capabilities, each of which is strong in the right list. Their support/Orders/scale may already be covered by Jazz/Clockmaker, cheap Morlocks and Zeros. | **Proxy/test *full actual partner counts*** before buying a separate team for novelty; **not** a verdict against Puppet Master’s inexpensive Counterintelligence/Regular-Order value. A Master does not become three PuppetBots for free; a Chimera is not three Pupniks. |
| **Morlocks, Moran and Transductor** | **Not worst.** Shepherd's normal Vanilla shell uses **two Morlocks**, **one Moran Repeater** (Vanilla **AVA1**) and cost-efficient normal REMs. **Moran Camo(1 Use) profile lacks the Repeater** even if a miniature carries appropriate equipment. | **Prefer buying enough for your actual list**. **Do not buy a second Moran for Vanilla expecting AVA2**; that higher availability belongs to Corregidor. **No blanket proxy-first “bad model” claim.** |

**Direct anchors:** [Shepherd Vanilla](https://www.youtube.com/watch?v=dOtvw5FKOfo); [Dante Vanilla](https://www.youtube.com/watch?v=hJKOZF1Je_g); [Tactical Awareness Nomad Prime](https://open.spotify.com/episode/2PpxuDu2WlxipiqpVzHTdv); [Vanilla roster/tactics](../../notes/factions/vanilla-nomads.md). **Best savings come from not buying overlapping *whole premium gun and TAG alternatives*, not cutting the cheap network/scoring foundation.**

#### Across the four Nomads armies — additional proxy-first miniatures, even when good

**There is no checked-in Nomads physical inventory** under the obvious \`inventory/nomads.md\`, \`inventory/corregidor.md\`, \`inventory/bakunin.md\` or \`inventory/tunguska.md\` paths. **No claimed Nomads owned counts** are used here. A missing inventory file does not mean that you own none.

| Miniature somebody might buy | Better initial proxy/test option | Buy a separate model when… |
|---|---|---|
| **Named infantry/hackers** (Mary Problems, Jelena Kovač, Uhahu, Valerya Gromoz, Raoul Spector, Lupe Balboa, Perseus, Wolfgang, Cassandra Kusanagi, Agatha, Sforza) | An unused **correct-base/silhouette Corvus Belli infantry figure**, visibly distinct from the rest of your list, with the declared role written down. Do not assume two named AVA1 characters can be represented simultaneously by the same model. | The named capability is recurrent, *or* two similar-sized named characters are used concurrently and need unambiguous identities. A highly useful character can still be an excellent purchase even when testing by proxy is cheaper. |
| **Alternate hacker/gun sculpts** (Interventor HD+/KHD, Riot Grrl TinBot, Grenzer gun, Wildcats, Territorials, Evader, Moderator, Hollow Men, Stempler, Vostok) | Use one **same-unit/same-compatible-size miniature** and explicitly declare the chosen current N5.3 **profile/loadout**. FTO, Repeater, TacAware, TinBot and Counterintelligence are **profile-specific**. | You repeatedly field *two physically different bodies simultaneously*, or your event's proxy rules/readability demand dedicated representation. |
| **Morlocks/Zellen/Jaguars/Denma/Überfallkommando** | Borrow spare warband/CC sculpts when silhouette and unit count match; **Bakunin Morlock can initially represent generic Bakunin Zellen if allowed** but this does **not** make the Zellen unit or its rules identical. **Chimera requires three separately represented Pupniks**. | Your list has simultaneous multiple CC models beyond the available distinct pool, or a specific FTO body matters. **Do not proxy a solo Chimera as a complete squad.** |
| **Puppetactica Master + PuppetBots; Jazz + Billie; Zoe + Π-Well; Fiddler + Jackbots; Coyote + BambaDroids** | Test the whole **controller + required subordinate body count** with appropriately sized/scaled spare models; physical servants are not Regular Orders unless the chosen profile explicitly grants an independent Order. Check versions with/without extras. | You often field a two-or-more-body selection, or cannot meet separate body/silhouette count with spare proxies. **Jazz FTO has no Billie**; **Fiddler FTO has no Jackbots**; **Bakunin Zoe + Π-Well is paired in current standard roster**. |
| **Alternative Reaktion/Vertigo/Stempler/Salyut/Transductor/Meteor/Tsyklon/Vostok REMs** | Temporarily use an unused **correctly sized REM chassis**, with visible assignment to a specific trooper type. **S1 PuppetBots, S2 support remotes and larger combat REMs cannot be assumed interchangeable**; validate actual base and Silhouette. | Need distinct REM bodies in the **same list** (e.g., two Transductors, Stempler plus Vertigo), or the proposed chassis cannot reproduce the required footprint. |
| **TAG alternatives** (Gecko, Gator, Szalamandra, Stigmata, Lizard, Iguana, Anaconda) | Before purchasing a large kit, **borrow/proxy one correctly based/silhouetted TAG** and play several legal lists. Match gun/Engineer support concept; **not every TAG belongs to each sectorial**. | The specific armoured platform repeatedly earns the main-gun slot; buy extra *only* if multi-TAG/dual-Gecko lists are routine. |
| **Go-Pod aerial VH / Zondnautica / other mounted units** | Use a matching **Vehicle/appropriate motorcycle or composite-body** stand-in; these are **not** ordinary S2 troopers or generic TAGs. Respect **Zondnautica's transformation/body rules** and Go-Pod's applicable Go-Bot. | You choose the mobility strategy repeatedly and have proper physical forms/companions for that profile. |
| **Corregidor division-specific miniatures** | Proxy Surface **Coyote/Territorial/Shifta** and Deepspace **Gator/Evader** *from different lists*, never from the same made-up Surface+Deepspace blend. | You have actually selected one **current legal division and team**; only then fill any simultaneous physical gaps. |
| **Additional AVA copies for rare tools** (Triggermen, Sin-Eater, Grenzer, Sombra, Switcher, expensive second Hacker/Engineer) | Use the first suitable model or a distinct appropriately sized proxy. AVA is a legal maximum, *not a model-shopping goal*. | Multiple copies have already appeared **simultaneously and often** in your mission-driven lists. |

**Event/ownership caveats:** Reveal proxy substitutions and check current **Silhouette, base diameter, required partners, counts, and organized-play/organizer policy**. Ordinary infantry, heavy infantry, remotes, TAGs and S7 Vehicles **cannot automatically stand in for one another**. No separate plastic miniature is needed for a profile option **unless simultaneous distinct bodies or a stricter event rule calls for it**. Older ITS-season proxy language is not proof of current seasonal policy. **A proxy cannot grant a unit permission to join a Fireteam or a division in which it is not legal.**

**Practical buying shortlist:** **Strongest direct whole-model deferrals** are **Bakunin generic Zellenkrieger if Morlocks already do its only job**; **Tunguska Triggermen if bought as a generic first premium shooter**; and **Go-Pod in any army if bought solely as a Turn-1 ARO breaker** (contested by positive flank uses). **Strongest *profile-only* avoids** are **Vanilla unlinked Grenzer MULTI Sniper**, **Bakunin Moderator Spitfire**, **Corregidor Surface Territorial AP Red Fury where MMR is better**, **Deepspace Gecko Vulkan as a long-lane opener**, and **unsupported Vertigo Guided builds**. **Generally best proxy-first *good* purchases:** second TAG/alternate TAG chassis, extra Vostok/Tsyklon/REM, extra PuppetBot/Chimera/Coyote package beyond owned body counts, second/third premium character and fourth/fifth Fireteam gun sculpt. Keep the original positive/dissenting media opinions above when making an actual list.
