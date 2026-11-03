---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 106
sectorial_slug: svalarheima-s-winter-force
sectorial_name: Svalarheima's Winter Force
parent_faction: PanOceania
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Svalarheima's Winter Force roster, standard loadouts, canonical Fireteam chart, and reverse Fireteam index. Indigo Spec-Ops and Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# Svalarheima's Winter Force

## Overview and provenance

Repository-native reference for **Svalarheima's Winter Force (SWF / WinterFor)** roster, profiles, points/SWC, AVA, and Fireteam access.

Sources used:

- Army-derived SWF source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **38-unit standard SWF roster** and the complete SWF `fireteamChart` in the pinned Army source.
- Soldier of Fortune entries whose source faction list is empty are excluded from the base roster.
- `Indigo Spec-Ops` and `Indigo Team-Ops` are optional game-mode content and are listed separately.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name by itself. Beasthunter and Clipper both have FTO-labelled options but no SWF Fireteam-chart row.
- Parenthetical Army-chart comments are treated as Counts-as / equivalence labels, not as join-scope restrictions.
- The structured `required: true` rows in WinterFor Alpha and WinterFor Beta are preserved as required-choice sets; this file does not reinterpret them as requiring every marked unit type simultaneously.
- Uma Sørensen is restricted to FTO profiles by her Wildcard row. Gunnar is restricted to the `GUNNAR FTO` profile because that is the Wildcard row name. Blade-Ops is restricted to `BLADE FTO` in the Fusilier Fireteam. WinterFor Beta explicitly uses `KNIGHT HOSPITALLER FTO`.
- Linked Reinforcement section: **Code: Capital** (`army_id: 199`). No Reinforcement Fireteam rows are merged into the main chart here.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Svalarheima's Winter Force |
| Parent faction | PanOceania |
| Army ID | 106 |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 38 |
| Optional-mode units | Indigo Spec-Ops; Indigo Team-Ops |
| Reinforcement roster | Code: Capital (`199`) |
| Fireteam limits | Core 1; Haris 2; Duo unlimited |
| Fireteam chart | yes |

## Roster index

| Unit | ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| Peacemaker Armbots | 36 | 2 | REM | Regular | — |
| Jotums | 44 | 2 | TAG | Regular | — |
| Fusilier Indigo Richard Quinn | 1490 | 1 | LI | Regular | Wildcard; counts as Fusilier |
| Tech-Bees | 935 | 1 | LI | Regular | — |
| Beasthunters Free Guild | 1570 | 1 | SK | Irregular | —; FTO-labelled option has no SWF chart row |
| Infirmarers of Saint Lazarus | 1487 | 2 | MI | Regular | Wildcard; counts as WinterFor Alpha / Nisse |
| Knight Hospitaller Kyle Hawkins | 1586 | 1 | HI | Regular | Fusiliers; WinterFor Beta; counts as Fusilier / Knight Hospitaller |
| Oktavia Grímsdóttir | 1501 | 1 | LI | Regular | Fusiliers |
| Bøyg Soldiers | 1507 | 2 | HI | Regular | WinterFor Beta required-choice |
| Knights Hospitaller | 6 | 3 | HI | Regular | WinterFor Beta required-choice, FTO profiles only |
| Locust | 769 | 2 | SK | Regular | — |
| Sierra Dronbots | 17 | 2 | REM | Regular | — |
| Valkyrie | 1343 | 1 | MI | Regular | Wildcard; counts as WinterFor Alpha |
| Kunai Solutions Ninjas | 1502 | 1 | SK | Regular | — |
| Nisses | 3 | 5 | MI | Regular | Nisses; WinterFor Beta |
| Knight of Justice | 1489 | 2 | HI | Regular | Wildcard |
| Captain Uma Sørensen | 1491 | 1 | MI | Regular | Wildcard, FTO profiles only; counts as Fusilier / Nisse |
| Pathfinder Dronbots | 16 | 2 | REM | Regular | — |
| Liang Kai | 1500 | 1 | WB | Regular + Impetuous | — |
| Blade-Ops | 1751 | 2 | LI | Regular | Fusiliers, FTO profiles only; counts as Fusilier |
| Shona Carano | 1505 | 1 | MI | Regular | Wildcard |
| Warcors | 50 | 1 | LI | Irregular | — |
| ORC Troops WinterFor | 5 | 5 | HI | Regular | Fusiliers; WinterFor Alpha required-choice |
| Fugazi Dronbots | 19 | 3 | REM | Regular | — |
| Palbots | 37 | 2 | REM | Peripheral | — |
| Trauma-Docs | 14 | 1 | LI | Regular | — |
| Nøkken | 1484 | 4 | LI | Regular | — |
| Mulebots | 38 | 2 | REM | Regular | — |
| Bulleteer Armbots | 35 | 2 | REM | Regular | Bulleteers Duo |
| Vargar Maximum Security Team | 1486 | 5 | MI | Regular | WinterFor Alpha required-choice |
| Pilot-X Team | 1903 | 1 Pilot-X + 0–2 RacerBots | LI + REM | Regular | — |
| Clipper Dronbot | 18 | 2 | REM | Regular | —; FTO-labelled option has no SWF chart row |
| Karhu Special Group | 1485 | 5 | MI | Regular | Fusiliers; WinterFor Alpha; WinterFor Beta; Bulleteers |
| Gunnar Lundmark | 1508 | 1 | MI | Regular | Wildcard, Gunnar FTO only; counts as Fusilier / Karhu |
| Fusiliers | 1 | T | LI | Regular | Fusiliers |
| Hannibal | 1345 | 1 | MI | Regular | Wildcard; counts as WinterFor Alpha |
| Machinist WinterFor | 15 | 1 | LI | Regular | Wildcard; counts as Nisse |
| Flight Officer Agnes Ferreira | 1504 | 1 | LI | Regular | Wildcard |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Indigo Spec-Ops | 1912 | Spec-Ops | Fusiliers Fireteam row, max 1 when Spec-Ops mode is in use |
| Indigo Team-Ops | 1926 | Team-Ops | No ordinary SWF Fireteam row |

## Unit details

### Peacemaker Armbots

**ID 36 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Repeater, Remote Presence, Courage, Forward Deployment (+20), Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Heavy Shotgun, Pulzar, PARA CCW (-3); AUXBOT_3 | — |
| 3 | 24 | 0.5 | Heavy Shotgun, Pulzar, PARA CCW (-3); AUXBOT_3B with Minelayer | — |
| 4 | 23 | 0 | Boarding Shotgun, Pulzar, PARA CCW (-3); BS Attack (+1B); no Auxbot | — |
| 5 | 27 | 0 | Boarding Shotgun, Pulzar, PARA CCW (-3); BS Attack (+1B); AUXBOT_3 | — |

### Jotums

**ID 44 · AVA 2 · TAG** — `MOV 15-10 | CC 18 | BS 15 | PH 17 | WIP 13 | ARM 10 | BTS 9 | W 3 | S 7`. ECM: Guided (-6), Remote Presence, Tactical Awareness, Terrain (Mountain), Immunity (Critical), BS Attack (SR-1).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 82 | 1.5 | MULTI HMG, Heavy Flamethrower, Panzerfaust, AP CCW (PS 3); Regular + Tactical Awareness | — |
| 2 | 82 | 2 | Same; Lieutenant | — |

Includes Crabbot ancillary remote.

### Fusilier Indigo Richard Quinn

**ID 1490 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 13 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. MSV1, Warhorse, Immunity (ARM).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 0 | MULTI Marksman Rifle, Flash Pulse, D-Charges, Boarding Pistol (+1B), CCW; Forward Observer | Wildcard max 1; counts as Fusilier |
| 3 | 26 | 0 | MULTI Rifle, Flash Pulse, D-Charges, Disco Baller, Boarding Pistol (+1B), CCW; Forward Observer | same |

### Tech-Bees

**ID 935 · AVA 1 · LI** — `MOV 10-10 | CC 12 | BS 11 | PH 10 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 2`. Specialist Operative, TAGCom, Deactivator, GizmoKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 9 | 0 | Adhesive Launcher Rifle, Flash Pulse, Pistol, PARA CCW (-3); Deployable Repeater | — |

### Beasthunters Free Guild

**ID 1570 · AVA 1 · SK** — `MOV 10-10 | CC 21 | BS 11 | PH 13 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`. Mimetism (-3), Stealth, Super-Jump, Religious Troop, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 9 | 0 | **BEASTHUNTER FTO**; Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CCW | —; no SWF chart row |
| 2 | 15 | 0 | Heavy Flamethrower, Tactical Bow, AP Mine; Camouflage, Surprise Attack (-3), Forward Deployment (+20) | — |
| 3 | 15 | 0 | Heavy Flamethrower, Panzerfaust, AP Mine; Camouflage, Surprise Attack (-3), Forward Deployment (+20) | — |
| 4 | 17 | 0 | Heavy Flamethrower (+1B), Panzerfaust, AP Mine; Camouflage, Surprise Attack (-3), Forward Deployment (+20) | — |

### Infirmarers of Saint Lazarus

**ID 1487 · AVA 2 · MI** — `MOV 15-5 | CC 21 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Martial Arts L1, Doctor, Religious Troop, Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 20 | 0 | Combi Rifle, Boarding Pistol, Shock CCW (PS 7) | Wildcard max 2; counts as WinterFor Alpha and Nisse |
| 2 | 17 | 0 | Boarding Shotgun, Boarding Pistol, Shock CCW (PS 7) | same |

### Knight Hospitaller Kyle Hawkins

**ID 1586 · AVA 1 · HI** — `MOV 15-5 | CC 23 | BS 14 | PH 13 | WIP 13 | ARM 3 | BTS 6 | W 2 | S 2`. Martial Arts L3, Frenzy, Combat Instinct, Specialist Operative, Stealth, Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 32 | 0 | MULTI Marksman Rifle, Pulzar, Flash Pulse, MULTI Pistol, DA CCW | Fusiliers max 1/counts as Fusilier; WinterFor Beta max 1/counts as Knight Hospitaller |
| 2 | 26 | 0 | Boarding Shotgun (+1B), Flash Pulse, Boarding Pistol, DA CCW | same |

### Oktavia Grímsdóttir

**ID 1501 · AVA 1 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. Albedo (-3), BS Attack (+1B), Courage, Combat Instinct, Dogged.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 30 | 1.5 | Missile Launcher, Contender, Heavy Pistol, CCW | Fusiliers max 1 |
| 2 | 26 | 1.5 | Heavy Rocket Launcher, Contender, Heavy Pistol, CCW; Sixth Sense | Fusiliers max 1 |

### Bøyg Soldiers

**ID 1507 · AVA 2 · HI** — `MOV 10-10 | CC 16 | BS 14 | PH 13 | WIP 12 | ARM 5 | BTS 6 | W 2 | S 5`. Albedo (-6), ECM: Hacker (-3), X-Visor, BS Attack (+1B), Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 44 | 1.5 | Missile Launcher, Disco Baller, Heavy Pistol, CCW | WinterFor Beta required-choice max 2 |
| 2 | 44 | 0 | Mk12, Disco Baller, Heavy Pistol, CCW | same |

### Knights Hospitaller

**ID 6 · AVA 3 · HI** — `MOV 10-10 | CC 22 | BS 14 | PH 14 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 2`. Martial Arts L2, Stealth, Religious Troop, Frenzy.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 27 | 0 | **FTO**; MULTI Rifle, TinBot Firewall (-3), Pistol, DA CCW | WinterFor Beta required-choice max 3 |
| 3 | 32 | 1.5 | **FTO**; HMG, Pistol, DA CCW | same |
| 4 | 26 | 0 | **FTO**; Boarding Shotgun, E/Mitter, Pistol, DA CCW | same |
| 7 | 30 | 0 | **FTO**; MULTI Rifle, MediKit; Doctor | same |
| 8 | 27 | 0 | **FTO**; MULTI Rifle, TinBot Firewall (-3); Lieutenant | same |
| 9 | 32 | 0 | Boarding Shotgun, Contender, D-Charges; Forward Deployment (+20) | —; non-FTO |
| 10 | 32 | 1 | **FTO**; HMG; Lieutenant | WinterFor Beta required-choice max 3 |

### Locust

**ID 769 · AVA 2 · SK** — `MOV 10-10 | CC 16 | BS 12 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Hidden Deployment, Mimetism (-6), Forward Deployment (+20), Stealth, Surprise Attack (-3), Bangbomb (+4), Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 3 | 24 | 0 | Boarding Shotgun, Grenades, Drop Bears, Boarding Pistol, CCW; Specialist Operative | — |
| 4 | 27 | 0 | MULTI Marksman Rifle, Boarding Pistol, CCW | — |
| 5 | 21 | 0 | SMG, D-Charges, WildParrot, Boarding Pistol, CCW | — |
| 6 | 29 | 0.5 | Breaker Combi Rifle, Pitcher, D-Charges; Hacking Device with Firewall (-3) | — |
| 7 | 27 | 0 | Breaker Combi Rifle, Pitcher, D-Charges; Killer Hacking Device with Firewall (-3) | — |
| 8 | 31 | 0.5 | Breaker Combi Rifle, Flash Pulse, D-Charges; Hacking Device with Firewall (-3), Camouflage (1 Use) | — |

### Sierra Dronbots

**ID 17 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage, Total Reaction, 360º Visor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 1 | HMG, PARA CCW (-3) | — |
| 2 | 18 | 0 | Thunderbolt (+1B), PARA CCW (-3) | — |

### Valkyrie

**ID 1343 · AVA 1 · MI** — `MOV 10-10 | CC 22 | BS 12 | PH 13 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Martial Arts L3, Berserk, Natural Born Warrior, Frenzy, NWI, Immunity (Enhanced).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 28 | 0 | Heavy Shotgun, Heavy Pistol, Grenades, EXP CCW | Wildcard max 1; counts as WinterFor Alpha |
| 2 | 33 | 0 | MULTI Rifle, Heavy Pistol, Grenades, EXP CCW | same |

### Kunai Solutions Ninjas

**ID 1502 · AVA 1 · SK** — `MOV 10-10 | CC 21 | BS 12 | PH 12 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. Camouflage, Hidden Deployment, Mimetism (-6), Martial Arts L3, Stealth, Climbing Plus, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 28 | 1.5 | MULTI Sniper Rifle, Pistol, Shock CCW | — |
| 2 | 26 | 0 | Shock Marksman Rifle; BS Attack (AP) | — |
| 3 | 25 | 0.5 | Thunderbolt, PARA Mine; BS Attack (T2) | — |

### Nisses

**ID 3 · AVA 5 · MI** — `MOV 15-5 | CC 14 | BS 13 | PH 12 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 2`. MSV2, Mimetism (-3), Terrain (Total), Climb 7.5.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 31 | 1.5 | HMG, Boarding Pistol, CCW | Nisses min 1/max 5; WinterFor Beta max 1 |
| 3 | 29 | 1.5 | MULTI Sniper Rifle, Boarding Pistol, CCW | same |
| 5 | 30 | 0.5 | Combi Rifle, Light Shotgun, Boarding Pistol, CCW; Hacking Device | same |
| 6 | 28 | 0 | Combi Rifle, Light Shotgun, Boarding Pistol, CCW; MediKit, Paramedic | same |

### Knight of Justice

**ID 1489 · AVA 2 · HI** — `MOV 15-5 | CC 23 | BS 14 | PH 14 | WIP 13 | ARM 5 | BTS 9 | W 2 | S 2`. Martial Arts L2, Stealth, Religious Troop, Number 2, Terrain (Mountain).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 46 | 1.5 | Missile Launcher (+1SD), Heavy Pistol, DA CCW | Wildcard max 1 |
| 2 | 42 | 1.5 | Spitfire, Heavy Pistol, DA CCW | same |
| 3 | 45 | 0.5 | MULTI Marksman Rifle, Pitcher, D-Charges; Hacking Device | same |
| 4 | 41 | 0 | MULTI Marksman Rifle, Flash Pulse, D-Charges; Forward Observer | same |
| 5 | 42 | 1.5 | Spitfire; Lieutenant | same |
| 6 | 45 | 1.5 | Spitfire, D-Charges; Forward Deployment (+10) | same |
| 9 | 41 | 0 | MULTI Marksman Rifle, Flash Pulse, D-Charges; Lieutenant, Forward Observer | same |

### Captain Uma Sørensen

**ID 1491 · AVA 1 · MI** — `MOV 10-10 | CC 15 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Mimetism (-3), Stealth, Specialist Operative, Climbing Plus, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 27 | 0 | SMG (+1B), E/M Mine, Silenced Pistol (+1B), CCW; Camouflage, Surprise Attack (-3), Forward Deployment (+20) | —; non-FTO |
| 2 | 25 | 0 | **FTO**; Breaker Combi Rifle, Silenced Pistol (+1B), CCW; X-Visor | Wildcard max 1; counts as Fusilier and Nisse |
| 3 | 23 | 0 | **FTO**; SMG (+1B), E/M Mine, Silenced Pistol (+1B), CCW; X-Visor | same |
| 4 | 25 | 0 | **FTO**; Breaker Combi Rifle, Silenced Pistol (+1B), CCW; X-Visor, Lieutenant | same |

### Pathfinder Dronbots

**ID 16 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Remote Presence, Courage, Sensor, Forward Observer, Triangulated Fire, Deactivator.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3) | — |
| 2 | 17 | 0 | Same; Tactical Awareness | — |

### Liang Kai

**ID 1500 · AVA 1 · WB** — `MOV 10-10 | CC 23 | BS 11 | PH 13 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Regular + Impetuous, Martial Arts L4, Berserk, NWI, Super-Jump, Stealth, Mimetism (-3), Forward Deployment (+10), Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | Chain Rifle, Light Shotgun, Flash Pulse, Pistol, EXP CCW | — |

### Blade-Ops

**ID 1751 · AVA 2 · LI** — `MOV 10-10 | CC 16 | BS 13 | PH 10 | WIP 12 | ARM 2 | BTS 3 | W 1 | S 2`. Tactical Awareness, Mimetism (-3), Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 20 | 0 | **BLADE FTO**; Boarding Shotgun, D-Charges, Silenced Pistol, CCW | Fusiliers max 1; counts as Fusilier |
| 2 | 23 | 0 | **BLADE FTO**; AP SMG, D-Charges, Silenced Pistol, CCW; Engineer, GizmoKit | same |
| 3 | 30 | 0 | AP SMG, E/Mitter, D-Charges; Engineer, Forward Deployment (+20), Decoy (2) | —; non-FTO |
| 4 | 30 | 0 | AP SMG, E/Mitter, D-Charges; Engineer, Parachutist, Decoy (2) | —; non-FTO |

### Shona Carano

**ID 1505 · AVA 1 · MI** — `MOV 15-5 | CC 23 | BS 11 | PH 14 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Martial Arts L4, NWI, Super-Jump, Stealth, Frenzy.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 22 | 0 | SMG, Nanopulser (+1B), Flash Pulse, Pistol, AP+EXP CCW | Wildcard max 1 |

### Warcors

**ID 50 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular, Journalist.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor | — |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); Sixth Sense | — |

### ORC Troops WinterFor

**ID 5 · AVA 5 · HI** — `MOV 15-5 | CC 15 | BS 14 | PH 14 | WIP 12 | ARM 4 | BTS 3 | W 2 | S 2`. Terrain (Mountain), Climbing Plus.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 19 | 30 | 0 | MULTI Rifle, Pistol, CCW | Fusiliers max 2; WinterFor Alpha required-choice max 5 |
| 20 | 31 | 0 | MULTI Rifle, TinBot Firewall (-3), Pistol, CCW | same |
| 22 | 28 | 0 | Boarding Shotgun (+1B), TinBot Firewall (-3), Pistol, CCW | same |
| 24 | 36 | 1.5 | HMG, Pistol, CCW | same |
| 25 | 37 | 1.5 | Feuerbach, Pistol, CCW | same |
| 26 | 31 | 0 | MULTI Rifle, TinBot Firewall (-3); Lieutenant | same |
| 27 | 36 | 1 | HMG; Lieutenant | same |

### Fugazi Dronbots

**ID 19 · AVA 3 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Remote Presence, Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) | — |

### Palbots

**ID 37 · AVA 2 · REM peripheral** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Peripheral (Servant), Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | PARA CCW (-3); no Order | — |

### Trauma-Docs

**ID 14 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. Doctor, MediKit.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Pistol, CCW | — |

### Nøkken

**ID 1484 · AVA 4 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Bangbomb (+4), Forward Deployment (+20), Mimetism (-6), Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 1.5 | Spitfire, Pistol, CCW | — |
| 2 | 27 | 0.5 | Combi Rifle, Light Shotgun; Hacking Device | — |
| 3 | 25 | 0 | Combi Rifle, Light Shotgun; Killer Hacking Device | — |
| 4 | 24 | 0.5 | Combi Rifle, Light Shotgun, Shock Mine; Minelayer | — |
| 5 | 22 | 0 | Boarding Shotgun (+1B), Panzerfaust, Flash Pulse; Forward Observer | — |
| 6 | 24 | 0 | Boarding Shotgun (+1B), Panzerfaust; MSV1 | — |

### Mulebots

**ID 38 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 4`. Baggage, Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | Repeater, Deactivator, PARA CCW (-3) | — |
| 2 | 14 | 0.5 | EVO Hacking Device, PARA CCW (-3) | — |
| 3 | 17 | 0 | Combi Rifle, Repeater, PARA CCW (-3); Total Reaction | — |

### Bulleteer Armbots

**ID 35 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Repeater, Remote Presence, Courage, Mimetism (-6).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Heavy Shotgun (+1B), PARA CCW (-3) | Bulleteers Duo min 1/max 2 |
| 2 | 22 | 1 | Spitfire, PARA CCW (-3) | same |

### Vargar Maximum Security Team

**ID 1486 · AVA 5 · MI** — `MOV 15-5 | CC 15 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Albedo (-6), Immunity (Shock), Super-Jump, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 26 | 1.5 | Spitfire, Pistol, CCW | WinterFor Alpha required-choice max 3 |
| 3 | 27 | 0 | Combi Rifle, Heavy Flamethrower, WildParrot; Triangulated Fire, Sensor | same |
| 4 | 26 | 0 | K1 Marksman Rifle, E/M Mine; Minelayer | same |
| 5 | 24 | 0 | Combi Rifle, Heavy Flamethrower, Flash Pulse, Disco Baller; Deactivator, Forward Observer | same |
| 6 | 22 | 1.5 | Heavy Rocket Launcher, Light Shotgun, Flash Pulse; Forward Observer | same |

### Pilot-X Team

**ID 1903 · AVA 1 Pilot-X + 0–2 RacerBots Mk-III**. A Pilot-X Team contains one Pilot-X and zero to two RacerBots Mk-III; RacerBots cannot be taken without Pilot-X, and all members must belong to the same Combat Group.

**Pilot-X** — `MOV 10-10 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 2`. Hacking Device (Upgrade: Zero Pain), RemDriver (+1 BS, +5 CC, BTS=6).

| Element | Pts | SWC | Loadout / differences | FT |
|---|---:|---:|---|---|
| Pilot-X | 21 | 1 | E/Mitter, Flash Pulse, MULTI Pistol, PARA CCW (-3); Hacker | — |
| RacerBot Mk-III | 8 each | 0 | Deployable Repeater, Light Riotstopper, Mine Dispenser (PARA), Stun Pistol, PARA CCW (-6); 360º Visor, Bangbomb (+4), ECM: Hacker (-3), Remote Presence | — |

### Clipper Dronbot

**ID 18 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CCW (-3); BS Attack (Guided) | — |
| 5 | 19 | 1.5 | **CLIPPER DRONBOT FTO**; Missile Launcher (+1B), PARA CCW (-3) | —; no SWF chart row |

### Karhu Special Group

**ID 1485 · AVA 5 · MI** — `MOV 15-5 | CC 14 | BS 13 | PH 11 | WIP 12 | ARM 2 | BTS 3 | W 1 | S 2`. MSV1, Courage, Mimetism (-3), Climbing Plus, Terrain (Total), NCO.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 22 | 0 | MULTI Rifle, Blitzen, AP Mine, Pistol, CCW | Fusiliers max 1; Alpha max 1; Beta required-choice max 3; Bulleteers max 1 |
| 2 | 22 | 0 | MULTI Rifle, E/Marat, AP Mine, Pistol, CCW | same |
| 3 | 34 | 1.5 | Feuerbach (+1B), AP Mine, Pistol, CCW | same |
| 4 | 25 | 0 | MULTI Rifle, Blitzen, D-Charges; Engineer, Deactivator, GizmoKit | same |
| 5 | 24 | 0 | MULTI Rifle, Blitzen, AP Mine; MediKit, Paramedic | same |

### Gunnar Lundmark

**ID 1508 · AVA 1 · MI** — `MOV 10-10 | CC 23 | BS 13 | PH 13 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Martial Arts L2, Berserk, Frenzy, Immunity (Shock), Mimetism (-3), Specialist Operative, Tactical Awareness, Stealth, Climbing Plus, Terrain (Mountain).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 30 | 0 | **GUNNAR FTO**; MULTI Rifle, Chain-colt, Pistol, Trench-Hammer, AP CCW | Wildcard max 1; counts as Fusilier and Karhu |
| 2 | 29 | 0 | Boarding Shotgun (+1B), Chain-colt, Pistol, Trench-Hammer, AP CCW; Forward Deployment (+20), Decoy (2) | —; non-FTO |

### Fusiliers

**ID 1 · AVA T · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 10 | 0 | Combi Rifle, Pistol, CCW | Fusiliers min 1/max 5 |
| 2 | 18 | 1 | HMG, Pistol, CCW | same |
| 4 | 15 | 1.5 | Missile Launcher, Pistol, CCW | same |
| 5 | 16 | 1 | MULTI Sniper Rifle, Pistol, CCW | same |
| 6 | 15 | 0.5 | Combi Rifle; Hacking Device | same |
| 8 | 12 | 0 | Combi Rifle, Flash Pulse; Deployable Repeater, Forward Observer | same |
| 9 | 12 | 0 | Combi Rifle; MediKit, Paramedic | same |
| 10 | 10 | 0 | Combi Rifle; Lieutenant | same |
| 12 | 12 | 0 | Combi Rifle; Commlink (+1), Specialist Operative | same |

### Hannibal

**ID 1345 · AVA 1 · MI** — `MOV 10-10 | CC 15 | BS 13 | PH 11 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. Courage, NWI, Counterintelligence, Sensor, Tactical Awareness, BS Attack (+1SD).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 5 | 24 | 0 | Vulkan Shotgun, Nanopulser (+1B), Flash Pulse, Breaker Pistol, CCW | Wildcard max 1; counts as WinterFor Alpha |
| 6 | 30 | 0 | MULTI Marksman Rifle, Nanopulser (+1B), Breaker Pistol, CCW | same |
| 7 | 27 | 0 | Vulkan Shotgun profile; Strategic Deployment | same |
| 8 | 33 | 0 | MULTI Marksman Rifle profile; Strategic Deployment | same |

### Machinist WinterFor

**ID 15 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`. Engineer, Deactivator, GizmoKit, Mimetism (-3), Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 17 | 0 | Combi Rifle, D-Charges, Pistol, CCW | Wildcard max 1; counts as Nisse |
| 13 | 20 | 0 | Same plus Armed Turret (Combi Rifle) | same |

### Flight Officer Agnes Ferreira

**ID 1504 · AVA 1 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 2`. Courage, Specialist Operative, Sixth Sense, Terrain (Zero-G).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 13 | 0 | SMG, Nanopulser, Pistol, CCW | Wildcard max 1 |
| 2 | 16 | 0 | Same; RemDriver (+1 BS, +5 CC) | same |
| 3 | 18 | 0 | SMG, Nanopulser (+1B), Pistol, CCW; Chain of Command | same |

## Canonical Fireteam chart

Global chart limits: **Core 1 · Haris 2 · Duo unlimited** (`DUO: 256` in the raw Army data).

### FT-SWF-01 — Fusiliers Fireteam

**Types:** Core, Haris

| Member | Unit ID | Min | Max | Required | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Fusilier | 1 | 1 | 5 | No | — | — |
| ORC WinterFor | 5 | 0 | 2 | No | — | — |
| Hawkins | 1586 | 0 | 1 | No | Fusilier | — |
| Blade FTO | 1751 | 0 | 1 | No | Fusilier | options 1/2 only |
| Karhu | 1485 | 0 | 1 | No | — | — |
| Oktavia | 1501 | 0 | 1 | No | — | — |
| Indigo | 1912 | 0 | 1 | No | Spec-Ops | Optional Spec-Ops mode |

At least one Fusilier is required by the explicit source `min: 1`.

### FT-SWF-02 — Nisses Fireteams

**Types:** Core, Haris, Duo

| Member | Unit ID | Min | Max | Required | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Nisse | 3 | 1 | 5 | No | — | — |

A native Nisses Fireteam therefore requires at least one Nisse.

### FT-SWF-03 — WinterFor Alpha Fireteams

**Types:** Core, Haris, Duo

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| ORC WinterFor | 5 | 0 | 5 | Yes | WinterFor Alpha | — |
| Varg | 1486 | 0 | 3 | Yes | WinterFor Alpha | — |
| Karhu | 1485 | 0 | 1 | No | — | — |

ORC WinterFor and Varg are both marked `required: true` in the structured chart; they form the source required-choice set rather than this reference asserting that both unit types must be present simultaneously.

### FT-SWF-04 — WinterFor Beta Fireteams

**Types:** Haris, Duo

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Karhu | 1485 | 0 | 3 | Yes | — | — |
| Knight Hospitaller FTO | 6 | 0 | 3 | Yes | — | FTO options 2/3/4/7/8/10 only |
| Bøyg | 1507 | 0 | 2 | Yes | — | — |
| Nisse | 3 | 0 | 1 | No | — | — |
| Hawkins | 1586 | 0 | 1 | No | Knight Hospitaller | — |

Karhu, Knight Hospitaller FTO, and Bøyg are the structured source required-choice set.

### FT-SWF-05 — Bulleteers Fireteams

**Type:** Duo

| Member | Unit ID | Min | Max | Required | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Bulleteer | 35 | 1 | 2 | No | — | — |
| Karhu | 1485 | 0 | 1 | No | — | — |

The explicit `min: 1` on Bulleteer means a native Bulleteers Duo contains at least one Bulleteer.

### Wildcards

All rows below are in the chart's **Wildcards** row. Parenthetical values are Counts-as labels, not join-scope restrictions.

| Wildcard | Unit ID | Max | Counts as | FTO/profile restriction |
|---|---:|---:|---|---|
| Infirmarer | 1487 | 2 | WinterFor Alpha, Nisse | all |
| Knight of Justice | 1489 | 1 | — | all |
| Machinist WinterFor | 15 | 1 | Nisse | all |
| Quinn | 1490 | 1 | Fusilier | all SWF Quinn loadouts |
| Uma Sørensen | 1491 | 1 | Fusilier, Nisse | FTO options 2/3/4 only |
| Shona Carano | 1505 | 1 | — | all |
| Gunnar FTO | 1508 | 1 | Fusilier, Karhu | option 1 only |
| Agnes | 1504 | 1 | — | all |
| Hannibal | 1345 | 1 | WinterFor Alpha | all |
| Valkyrie | 1343 | 1 | WinterFor Alpha | all |

Wildcard status does not remove the native minimum/required-choice conditions of the Fireteam being joined. Counts-as labels remain relevant to composition.

## Unit → Fireteam access index

| Unit | Fireteam access |
|---|---|
| Peacemaker | — |
| Jotum | — |
| Quinn | Wildcard max 1; counts as Fusilier |
| Tech-Bee | — |
| Beasthunter | —; FTO-labelled option has no SWF chart row |
| Infirmarer | Wildcard max 2; counts as WinterFor Alpha and Nisse |
| Hawkins | FT-SWF-01 max 1/counts as Fusilier; FT-SWF-04 max 1/counts as Knight Hospitaller |
| Oktavia | FT-SWF-01 max 1 |
| Bøyg | FT-SWF-04 required-choice max 2 |
| Knight Hospitaller | FT-SWF-04 required-choice max 3, **FTO options only** |
| Locust | — |
| Sierra | — |
| Valkyrie | Wildcard max 1; counts as WinterFor Alpha |
| Kunai Ninja | — |
| Nisse | FT-SWF-02 min 1/max 5; FT-SWF-04 max 1 |
| Knight of Justice | Wildcard max 1 |
| Uma Sørensen | Wildcard max 1, **FTO options 2/3/4 only**; counts as Fusilier and Nisse |
| Pathfinder | — |
| Liang Kai | — |
| Blade-Ops | FT-SWF-01 max 1, **BLADE FTO options 1/2 only**; counts as Fusilier |
| Shona Carano | Wildcard max 1 |
| Warcor | — |
| ORC WinterFor | FT-SWF-01 max 2; FT-SWF-03 required-choice max 5/counts as WinterFor Alpha |
| Fugazi | — |
| Palbot | — |
| Trauma-Doc | — |
| Nøkken | — |
| Mulebot | — |
| Bulleteer | FT-SWF-05 min 1/max 2 |
| Varg | FT-SWF-03 required-choice max 3/counts as WinterFor Alpha |
| Pilot-X Team | — |
| Clipper | —; FTO-labelled option has no SWF chart row |
| Karhu | FT-SWF-01 max 1; FT-SWF-03 max 1; FT-SWF-04 required-choice max 3; FT-SWF-05 max 1 |
| Gunnar | Wildcard max 1, **GUNNAR FTO option 1 only**; counts as Fusilier and Karhu |
| Fusilier | FT-SWF-01 min 1/max 5 |
| Hannibal | Wildcard max 1; counts as WinterFor Alpha |
| Machinist WinterFor | Wildcard max 1; counts as Nisse |
| Agnes | Wildcard max 1 |
| Indigo Spec-Ops | FT-SWF-01 max 1 when Spec-Ops mode is in use |
| Indigo Team-Ops | — in the ordinary SWF chart |

## Tactical tags

Derived analysis aids, not official characteristics.

| Unit | Tags |
|---|---|
| Jotum | TAG, long-range attack, Tactical Awareness, extreme durability, LT option |
| Fusilier | cheerleader, long-range ARO, hacker, specialist, network projection, link anchor |
| ORC WinterFor | durable attack, long-range attack/ARO, lieutenant option, Climbing Plus, Alpha anchor |
| Varg | mid-range attack, long-range ARO, Sensor, specialist, midfield defense, Super-Jump, Alpha anchor |
| Karhu | NCO, MSV1, long-range attack, Engineer, specialist, AP mine, link utility |
| Nisse | MSV2, Mimetism, long-range attack/ARO, hacker, specialist, link anchor |
| Bøyg | durable long-range attack, Missile ARO, anti-hacker ECM, Beta anchor |
| Knight Hospitaller | durable attack, Doctor, lieutenant option, close assault, Beta anchor |
| Hawkins | close assault, specialist, link support |
| Knight of Justice | durable attack, hacker, network projection, specialist, long-range ARO, Wildcard |
| Infirmarer | Doctor, close assault support, Wildcard, link composition support |
| Quinn | specialist, network projection via Disco Baller, MSV1, Wildcard |
| Uma Sørensen | midfield specialist, camo attack, lieutenant option, Wildcard |
| Gunnar | Tactical Awareness, close assault, specialist, Wildcard |
| Shona Carano | close assault, Wildcard |
| Valkyrie | close assault, Wildcard, WinterFor Alpha composition support |
| Hannibal | Tactical Awareness, Sensor, Counterintelligence, Strategic Deployment, Wildcard |
| Agnes | cheap specialist, Chain of Command option, RemDriver, Wildcard |
| Machinist WinterFor | Engineer, tech-counter, turret option, Wildcard |
| Oktavia | long-range ARO, Albedo, Sixth Sense option, Fusilier link support |
| Blade-Ops | Tactical Awareness, Engineer, airborne option, midfield specialist, Fusilier link support |
| Locust | hidden deployment, midfield specialist, hacker/KHD, Pitcher, deployables |
| Nøkken | midfield defense, hacker/KHD, specialist, Minelayer, MSV1 option |
| Beasthunter | cheap irregular defense, camo midfield defense, AP mines |
| Liang Kai | warband, close assault, Super-Jump, forward deployment |
| Kunai Ninja | hidden deployment, long-range ARO/attack, anti-armor ammunition |
| Peacemaker | midfield defense, forward REM attack, network projection |
| Bulleteer | REM attack, Mimetism (-6), mid-range attack, network projection, native Duo |
| Pathfinder | specialist, Sensor, network projection, Tactical Awareness option |
| Pilot-X Team | hacker, RemDriver, network projection, mine dispenser, fast REM support |
| Fugazi | cheerleader, network projection, flash ARO |
| Mulebot | Baggage, EVO, REM support, cheerleader |
| Sierra | long-range ARO, Total Reaction |
| Clipper | guided missile, long-range ARO |
| Tech-Bee | TAG support, tech-counter, network projection |
| Trauma-Doc | Doctor, recovery support |
| Palbot | Doctor/Engineer projection support |
| Warcor | cheap irregular ARO |

## Validation and maintenance

- Standard roster represented: **38 units**.
- Optional-mode hooks: Indigo Spec-Ops and Indigo Team-Ops.
- Canonical Fireteam rows represented: **Fusiliers, Nisses, WinterFor Alpha, WinterFor Beta, Bulleteers, Wildcards**.
- Limits preserved: `CORE 1`, `HARIS 2`, raw `DUO 256` = InfinityDB `unlimited`.
- Parenthetical source comments are stored as Counts-as/equivalence labels.
- Required-choice sets are preserved directly from the structured source rather than rewritten into a stronger inferred rule.
- FTO restrictions are applied only where the Fireteam row/name explicitly contains an FTO marker.
- No Fireteam access is inferred solely from a loadout having `FTO` in its name.
- Beasthunter FTO and Clipper FTO are deliberately shown with no Fireteam access because neither has an SWF Fireteam-chart row.
- Pathfinder is deliberately shown with no Fireteam access in SWF even though it is a Wildcard in NCA; the SWF chart contains no Pathfinder row.
- Main and Reinforcement Fireteams are not merged.
- Pilot-X/RacerBot dependency is preserved: no RacerBot Mk-III without Pilot-X, and all team members must remain in the same Combat Group.

## Provenance

- Corvus Belli Army-derived source revision: `7.26246.158`.
- Army snapshot commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- Army data changed on / snapshot date: `2026-09-03`.
- InfinityDB semantic cross-check: `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Fireteam source: pinned Army `fireteamChart`, normalized using the same semantics documented in InfinityDB.
- Verified: `2026-10-15`.

## Mission specialist choices — N5.3 cross-game evaluation

**Karhu Engineer/FO or KHD/Specialist variants**, when explicitly listed, provide fighting plus button capability on the same path; compare their premium to **Pathfinder FO/Sensor14** and cheap legal Fusilier/Knight medical specialists. An elite long-range shooter may clear a route but cannot claim a specialist-only Objective unless its *actual selected profile* qualifies. Keep an independent turn-three Specialist while the WinterFor attack team commits.

See [Mission Specialists / Button Pushers apex and value tiers](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). This roster and its Fireteam chart are the final authority for exact options.

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **Nisse HMG31/1.5** is a strong **non-TAG** BS13/MSV2/Mimetism(-3) anti-camo lane clearer in legal team but 1W makes it fragile. **Jotum MULTI HMG82/1.5** sits separately among **TAGs**, punishing ordinary gunfire with BS15/ARM10/BTS9/3W/TacAware; E/M, hacking and CC make its exceptional armor irrelevant if opponents can deliver. **Knight of Justice Spitfire42/1.5** is a cheaper robust **non-TAG** linked midrange/CC alternative when scenario movement matters more than armor wall. [Distinct TAG and non-TAG rankings](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## TAG tactical cross-reference (2026-10-23)

**Jotum (82)** is a hard defensive/attrition anchor against limited AP/E/M threats: ARM10/BTS9, MULTI HMG, HFT and TacAware. Its value drops sharply against AP, E/M or repeaters that bypass the expensive armor advantage; use WinterFor's other troops to remove these threats rather than simply advancing the Jotum first.

Cross-faction **apex vs points-value** comparisons, matchup table, and direct MCP-reviewed podcast/video sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Current profile and Fireteam legality above remain authoritative.

## Hacker and KHD tactical cross-reference (2026-10-23)

**15/0.5 Fusilier HD** is the inexpensive generic anti-heavy Hacker; **Nøkken KHD 25/0 vs HD 27/0.5** adds FD+20 and Mimetism(-6) for objective access and safe network angles. **Locust KHD/Pitcher 27/0 with Firewall(-3)** offers Hidden/counterhacking; HD 29/0.5 trades to Oblivion/Carbonite. **Knight of Justice HD 45/0.5** has BTS9, W2 and BS14 Pitcher but needs a premium gun/link plan to repay its cost. **Why:** a distributed Nøkken/Locust and cheap HD is often safer than staking all network coverage on one 45pt hackable Knight.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

See [Cheerleaders and Order Generators — N5.3 apex, points-value and matchup guide](../../notes/list-building/cheerleaders-and-order-generators.md) for complete comparative tables and verified transcript disagreements. The **current roster above controls** legality, AVA, Training and Fireteams.

- 7pt Fugazi — Flash/Mimetism/Repeater mobile Regular Order, excellent only with a protected S3 slot and available AVA.
- 8pt Mulebot — Baggage/Re­peater Regular Order, excellent if support reloads are useful and S4 bases fit.
- Fusiliers — cheap small-base Regular line, suitable for mandatory Fireteams, Lieutenant uncertainty and guarded rear objectives.
- 9pt RacerBot — mobile Regular Order with adhesive/PARA control, not simply a passive safe S2 soldier.
- Warcor — 3pt Irregular Flash Pulse distraction, not a transferable Regular Order.

**Order audit:** add up only deployed eligible **Regular** Orders in each Combat Group; special LT/Tactical, Irregular and Peripheral activations are not transferable pool Orders. Buy the cheapest protected body that supplies the *second function the list truly needs*; consider large-base DZ crowding, expensive mandatory Fireteam slots, and whether another scoring specialist beats one more cheap Order.


## ARO apex/value cross-reference (2026-10-23)

See [Best ARO Units — N5.3 apex and cost-value tiers](../../notes/list-building/aro-units-apex-and-value.md) for gunfighter vs hidden-trap vs cheap Order-tax comparisons, when each wins, transcript disagreements and counterplay. **The roster, prices/AVA and canonical Fireteam chart above remain authoritative**; a shared unit's permissions do not transfer between armies.

- **Knight of Justice ML** — durable +SD lane anchor; better when real mission approaches must pass its arc
- **Sierra Thunderbolt TR** — 18pt/0SWC multi-arc Regular ARO where profile legal; add Engineer/recovery if its lane matters repeatedly
- **Karhu Feuerbach** — strong AP and visor with Mimetism, but W1 means trade carefully; supports NCO attack role
- **Nisse sniper** — MSV2/Mimetism counters elite visual defence but needs a safe lane and support
- **Warcor Flash Pulse** — 3pt Irregular zero-SWC Order-tax ARO; never count as a generic Regular Order

**Deployment choice:** put the disposable/tax ARO on the approach, preserve a separate hidden/mission-denial gate where legal, and avoid leaving an expensive active-turn gun as your only exposed defence. Test pie-slicing, Smoke/Eclipse/White Noise, hacking, AD entry, recovery access and specialist survival before paying more SWC for a second sniper.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Recovery:** **Jotum** and other REM/TAG investments justify an **Engineer + Palbot** near safe fallback; **Remote Presence token reroll** raises a WIP12 Machinist from 60% to 84% on a failed repair. **Nisse or Knight casualties** instead need **Doctor/Paramedic**, not Engineer. Repair a Jotum only if a single revived STR model can actually return to a useful attack or scoring lane. [Doctor/Engineer apex, points-value, recovery odds and transcript disputes](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## N5.3 DZ defense / anti-alpha-strike tactical choices

**Warcor 360º3/0** guards rear/side landing angles for virtually no points, and **Sierra TR+360º Thunderbolt18/0** gives a Regular repairable multiarc gun; **Fugazi7/0 Flash+Repeater** and **Mulebot8/0 Baggage+Deactivator+Repeater** are dual-purpose **Regular** cheerleaders/limited last-line friction. **Peacemaker 24/.5 Auxbot-3B Minelayer** denies a turn-zero route before the alpha strike but normally wants to defend *midfield-to-DZ access*, not crowd protected rear models. **Counter:** no single long-range ARO stops a safe Combat Jump behind cover or a masked Impersonator; retain close template/mine and disperse vulnerable support.

[Cross-game DZ Defenders — apex/value and transcript-backed disagreement](../../notes/list-building/dz-defenders-alpha-strike-and-impersonation-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Kyle Hawkins32/0 CC23/MA3/2W** is the practical **mobile close-range fighting specialist**, with MULTI Marksman/Pulzar to open an approach. **Hospitaller Knights** and **Knight of Justice** (CC22–23/MA2) bring 2W melee insurance but need legal Fireteam delivery. **Kunai28 Hidden/MA3** lacks Oniwaban Monofilament/Infiltration target execution: primarily an ARO sniper. For **Jotum/expensive WinterFor guns**, screen with ORCs/Karhu and mines rather than asking CC15 ORCs to duel an enemy MA5 assassin. [CC apex/value and reach-versus-lethality comparisons](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## N5.3 network projection — Pitchers, Repeaters, TinBots and disposable delivery

**Fugazi7/0 native Repeater**, **Mulebot8/0 Baggage**, and **Pathfinder FO/Sensor/Repeater** are cheap Regular Order/network foundation; **Peacemaker native Repeater with FD(+20)** brings an already-forward zone plus optional Auxbot/Minelayer. **Nøkken Camo/FD utility** can build further network only on profiles carrying correct Deployable Repeater; **Bulleteer native Repeater** is a gun-platform bonus, not an excuse to sacrifice a 20+pt shooter as a disposable 7pt bot. **Counter:** WinterFor's strong gunfight plan often prefers just Fugazi/Pathfinder rather than spending SWC on a Pitcher team or assuming off-roster tech.

[Whole-game network projection apex/value, transcript disagreements and matchup selection](../../notes/list-building/network-projection-repeaters-pitchers-apex-value.md). Local profile tables and actual Fireteam chart take precedence.

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Beasthunter9 Panzerfaust** (or **15 Camo+FD**), **Nøkken22 Panzerfaust**, **Karhu22 Blitzen or E/Marat**, and **Vargar K1 Marksman+E/M Mine26** offer distinct cheap-to-medium TAG responses: range deterring, short electronic trap and repeatable ARM=0. **ORC Feuerbach37/1.5** provides longer lethal control. A **Jotum** is a high-cost TAG target/opponent rather than the value answer to another Jotum. [Cross-game anti-armor apex/value, E/M, K1 and AP+EXP tiers](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**WinterFor** favors heavyweight **Jotum** high-ARM TAG zone swing and **Knight Hospitaller/Justice** hard midfield when locally roster-legal, but actual Specialist profile/Fireteam determines Supplies eligibility. **Nøkken FO22/0** with marker and FD is excellent initial box retrieval, not invisible after taking box; **Peacemaker23–27/0–.5 + Auxbot** and **Fugazi7/0** guard pickup square while a separate durable specialist retreats. **Sval command/active pieces** that must fight on first turn should not be pinned indefinitely to a console merely because they have high ARM. **Disagreement (2026 overall faction tiers):** WinterFor's fantastic guns struggle to *translate* cleared lanes into scored buttons; plan 2 specialist routes, not only a Jotum.

[Cross-faction zone holding/carrier apex/value and actual transcript disagreements](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Authoritative roster/FT chart above governs profile legality.

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Nisse HMG31/1.5 MSV2 + Mimetism(-3)** is an effective *shoot* answer to revealed Mimetism/ordinary Smoke at the proper range and legal team; **Pathfinder14/0 Sensor/FO** instead cheaply reveals Camouflaged/Hidden threats from ZoC. **Vargar27/0 Sensor+Triangulated Fire** is an active mobile marker hunter; **Vargar24/0 FO+Disco** and **Quinn26 Disco** bypass enemy MSV/Marksmanship without needing to win that FtF. **Opposite tech:** enemy White Noise/Albedo punishes reliance on Nisse MSV2; bring a plain defender and count setup Orders. Do not merge Vargar's Sensor and Disco on one hypothetical profile.

[Anti-tech N5.3 whole-game apex/value and counter-matchups](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## N5.3 peripheral / synchronized / multi-body apex-value update

**Peacemaker HSG+Auxbot23/0** adds an actual second synchronized HFT angle to WinterFor's otherwise gun-heavy long firelanes: FD+20/Repeater/Mim(-3) imposes late corner attack costs. **24/.5 Minelayer** buys prelaid mine for layered DZ/midfield defense; **27/0 BSG+Auxbot** strong active short-range, but **23/0 BSG+1B has NO Auxbot**. **Jotum and other TAG Ancillary Crabbot** are delayed deployable support not 2 Regular Orders. **Opposing analysis:** WinterFor excels killing lanes but can fail button timing; inexpensive Peacemaker+one independent specialist may outscore another expensive reactive HI that doesn't defend the actual interaction square.

[Cross-game N5.3 Peripheral & Multi-Body tiers](../../notes/list-building/peripheral-synchronized-multibody-apex-value.md). Do not substitute another sectorial's AVA, profile or Fireteam access.

## Mission performance — battle-report evidence (2026-11-01)

| Mission(s) | Tested composition / scoring mechanism | Evidence |
|---|---|---|
| **Frostbite** | Nisse/Uma/Karhu plus Doctor/Engineer, heater activators and cold-zone survivors hold the safe approach. | [#098](../../notes/battle-reports/091-100-n5-battle-report-tactical-analysis.md) |
| **Critical Intervention defense** | Knight of Justice, Karhu specialists, Peacemaker mines and turrets defend access after heavy AROs are damaged. | [#182](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md) |

**Limits:** #087's Acquisition final score is not reliably attributable; do not claim a confirmed WinterFor win. Game-era qualitative evidence, not a win-rate or N5.3 Fireteam claim. [Full cross-report mission synthesis](../../notes/battle-reports/cross-report-mission-performance-by-sectorial.md).

## Counterplay — observed N5 battle-report responses (2026-11-02)

| Threat / target | Observed response, timing and consequence | Battle reports |
|---|---|---|
| **Impersonator / room assault** | Peacemaker mine, disposable turrets and small Karhu/REM room workers frustrated Shasvastii Speculo/Sheskiin data-pack extraction after an initial alpha; WinterFor won 9–5. | [#182](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md) |
| **TAG / long guns** | Karhu K1/Paramedic, Nisse/Uma shooting and Machinist offer anti-armor plus repair/mission routes; Shona/Liang Kai mobility counters screen placement at close range. | [#075](../../notes/battle-reports/071-080-n5-battle-report-tactical-analysis.md), [#098](../../notes/battle-reports/091-100-n5-battle-report-tactical-analysis.md) |
| **Counter-counterplay** | Bakunin Custodier White Noise/Repeaters/Guided pressured WinterFor sniper lines, and a Nisse spent 5–6 Orders fighting a Cenobite HRL instead of scoring Supplies. | [#098](../../notes/battle-reports/091-100-n5-battle-report-tactical-analysis.md), [#194](../../notes/battle-reports/191-200-n5-battle-report-tactical-analysis.md) |

**Limit:** A hard ARO must still defend the objective and protected specialists; mission rules/turret activations are episode-specific. These are game-era actions, not current N5.3 profile/Fireteam legality or faction win rates. [Cross-report counterplay analysis](../../notes/battle-reports/n5-cross-report-counterplay-tags-hi-hacking-camo-impersonators-fireteams.md).

---

## Must-have / Go-to / Avoid — source-backed recommendations (2026)

Dated source-backed tactical preferences and miniature purchasing priorities; opinions do not override N5.3 roster, profile or Fireteam data above.

**Original audit title:** PanOceania N5.3 — Must-have, go-to, and avoid picks (transcript-evidenced)

**Review:** 2026-10-23. **Authority:** [pinned PanO sectorial Army/Fireteam references]() (Army 7.26246.158, Sept 2026). The seven [tactical faction notes]() and MO roster research were compared with the direct YouTube/Spotify MCP transcripts linked below. **Only attribute a recommendation to a presenter when they actually say it.** Older footage is opinion and does not overrule N5.3 prices, profiles, AVA or Fireteams.

**How to read:**
- **Must-have** = author **explicitly describes** near-universal pick, or multiple transcripts repeatedly favor it; label **single-reviewer** where unsupported as a consensus. When no unit meets this bar, say **none established**. These are NOT tournament inclusion statistics.
- **Go-to** = explicitly praised as good in broadly relevant roles, though architecture/missions choose the actual loadout.
- **Avoid / near-never** = direct presenter condemnation *of that profile/use*, not a blanket assertion the whole unit is unusable. **Disputed** marks another published view. “No-chart FTO” means **cannot use an implied link**, not that the weapon/model is forbidden.
- Costs are all-in **points/SWC** from pinned local roster when shown.

### Quick decision table

| Army | Credible must-have or closest | Go-to core | Strongest source-backed avoid |
|---|---|---|---|
| **Vanilla PanO** | **None established**; cheap Fugazi infrastructure (7) is closest | Joan/active command, Magistrate, Swiss/Tik/Cutter, Peacemaker | **Clipper Guided** as default attack plan without an actual Targeted engine (Dante/Tristan) |
| **Kestrel** | **Magistrate LT + linked 6pt Jackals** *according to Irregular Order hosts*; Jackal cheap disruption | Fennec FO/Disco/Sensor13, Tik LT, Hetkari, Pathfinder TA17, Banshee | **Fennec LT10** in preference to 19pt Strategos Magistrate or Tik LT (Shepherd); **basic non-command Magistrate** contested low marginal value |
| **Military Orders** | **Foot Montesa FTO Paramedic20** (Shepherd's explicit near-auto-include); not a requirement | Trinitarians, Teutonic19, Santiago KHD31, Commander LT+1 24, De Fersen, Holy Sepulchre | **Knight of Justice Hacker45/.5** in most lists (Shepherd directly rejects) |
| **Neoterra (NCA)** | **None established literally**; Fugazi7 / Auxilia15–18 repeatedly praised as foundation | Blocker Specialist15, Pathfinder TA17, Uhlan70–80, Swiss, Squalos NCO | **Fusilier SWC guns and Hacker** outside specific budget reasons (Shepherd) |
| **Varuna** | **Zulu-Cobra KHD26** (Dante says he starts every list with it) | Foot Montesa26, Helot cheap defense, Kamau / Varuna ORCs | **Clipper** as generic missile buy (Swiss Miss bottom C); **Croc Men over Zulu** disputed (TA vs Swiss Miss) |
| **Shock Army of Acontecimento** | **None established unanimously**; MetaChemistry expects multiple Bagh-Mari, other lists use Regulars/Guarda/TAG | Regular Sensor Minelayer13, Sapper MSR20, foot Montesa FTO20, Pathfinder TA17, Naga utility | **Naga Monofilament Minelayer** considered gimmicky by Swiss Miss; **Clipper FTO** has no link row, and Guided has uncertain payoff |
| **WinterFor / SWF** | **Peacemaker + Auxbot** (Swiss Miss says he would almost always bring one; single-reviewer), Fugazi7 near-default | Karhu Feuerbach34, Vargar FO/Disco24, Blade FTO Engineer23, Hawkins26–32, Locust | **Fusilier HMG / ML / Sniper** (Shepherd says basically never); **Bøyg44** often poorer utility/point than Vargar (disputed) |

### 7. Svalarheima's Winter Force (SWF)

- **Strongest near-auto from one presenter:** [Swiss Miss — WinterFor N5 tier list](https://www.youtube.com/watch?v=-pVR0OSVP4w) says they would **almost always take a Peacemaker with Auxbot**, emphasizing the forward Repeater, mine/flamethrower, nuisance ARO and route denial. **Fugazi7 AVA3** is also called S-tier, but **explicitly not always 3**. This is a documented reviewer preference, not a universal all-player rule.
- **Go-to:** **Karhu Feuerbach34/1.5** (NCO, MSV1+Mimetism for favorable face-to-face shooting), **Karhu Engineer25** (repair/specialist as team partner), **Vargar FO+Disco24 / FO HRL22** (Albedo and mission-compatible screen), **Blade FTO Engineer23** (TacAware and Fusilier-team utility), **Kyle Hawkins Specialist26–32**, **hidden Locust Specialist24**, **Jotum82** as optional TAG bull, not mandatory. [Shepherd WinterFor focus](https://www.youtube.com/watch?v=oHeTzuV9WLY) · [Swiss Miss tier list](https://www.youtube.com/watch?v=-pVR0OSVP4w).
- **Avoid, explicit:** [Shepherd](https://www.youtube.com/watch?v=oHeTzuV9WLY) says **Fusilier HMG, ML and Sniper** are basically *never* the WinterFor purchase: buy Fusilier LT/decoy or occasional Paramedic instead and put serious guns on Karhu/other higher-quality troopers.
- **Low-priority/contested, not never:** [Shepherd](https://www.youtube.com/watch?v=oHeTzuV9WLY) finds **Bøyg44** difficult to justify against significantly cheaper Vargar Albedo+Disco, although he concedes its armor/extra wound and Beta-team potential; [Swiss Miss](https://www.youtube.com/watch?v=-pVR0OSVP4w) finds **unlinked Pathfinder TA17** C-tier, whereas Shepherd calls its Sensor/FO and personal Order useful despite no link access. **Neither is a guaranteed bad purchase.**

### Practical verdict

There are **only four direct source-backed near-universal assertions worth repeating as such**: **MO foot Montesa FTO20** (Shepherd), **Kestrel Magistrate+cheap Jackals** (Irregular Order speakers, with Tik LT exception), **Varuna Zulu KHD26** (Dante), and **SWF Peacemaker+Auxbot** (Swiss Miss). In **Vanilla, NCA and SAA**, the recording evidence supports **a highly efficient *role or package*** much more strongly than any individual compulsory profile.

The strongest no-default profile rejection examples backed by an actual recording are **MO KoJ Hacker45 (Shepherd)**, **NCA Fusilier SWC guns/Hacker (Shepherd)**, **SWF Fusilier premium guns (Shepherd)**, **Kestrel Fennec LT (Shepherd)** and **Varuna Clipper (Swiss Miss; low-tier, not literally unplayable)**. For SAA the negative evidence is **weak/conditional**. Apply each to the named loadout, not every profile sharing its unit name.

### Whole-unit purchasing audit — what can stay off the shopping list? (2026-10-30)

A **whole-unit defer** applies to the *named unit across its usable current profiles* in a particular army, not just a discouraged HMG/ML/Hacker. **No absolute, all-list model ban** is established by the recordings.

| Army | Whole model/unit purchase to defer | Why / when it is worth buying |
|---|---|---|
| **Vanilla PanO** | **Clipper — conditional defer if not building Spotlight/Targeted** | [Dante/Tristan](https://www.youtube.com/watch?v=qp458fqYq_s) do not normally favor generic missile-bot attack here; a deliberate guided network remains a reason to buy. Other cited avoids are not whole-unit judgments. |
| **Kestrel** | **No substantiated full-unit skip** | Fennec **LT** is disfavored but its FO/Sensor/Disco profiles are go-tos. Drummer's expensive controller is criticized, but its cheaper FO + Drumbot and opposing reviewers prevent a unit ban. |
| **Military Orders** | **No** | Knight of Justice **Hacker** is singled out; other KoJ command/combat loadouts must not be rejected on that evidence. |
| **Neoterra** | **No** | Fusilier premium guns/Hacker are criticized; cheap Fusilier LT and decoy bodies still work. |
| **Varuna** | **Clipper — low-priority / conditional**, **not** a proven never-buy | [Swiss Miss](https://www.youtube.com/watch?v=v3hhlSohHzg) rates it bottom C, while a planned linked missile/Guided configuration can still matter. Croc Men have directly opposing reviews, so **do not skip** them on one speaker's advice. |
| **Shock Army of Acontecimento** | **Clipper — defer unless a real missile plan exists** | Weak generic Guided payoff; FTO **does not** have an SAA Fireteam slot. [Swiss Miss](https://www.youtube.com/watch?v=hlmVXGHskS4) is a preference, not proof of zero viable use. Naga's disliked Mono *profile* does not disqualify Naga. |
| **WinterFor** | **Bøyg — optional low-priority buy**, disputed | [Shepherd](https://www.youtube.com/watch?v=oHeTzuV9WLY) often prefers cheaper Vargar utility; Bøyg still offers armor, extra wound and specific Beta-team roles. Fusilier SWC criticism does **not** justify skipping Fusiliers. |

**Collection note:** a Clipper miniature can serve other PanO rosters where the mission/network plan is different. These are **sectorial-specific purchasing priorities**, not sculpt-wide bans. See the [cross-faction shortlist](../../notes/factions/model-purchase-avoid-summary-2026.md).

### Worst-value and rare/circumstantial picks — proxy-before-buy guide (2026-10-30)

**Question answered:** Which *entire miniatures* deserve no immediate purchase, which **specific profiles** should be avoided despite the unit having good uses, and which useful-but-rare units are best represented by an existing model? This expands — and does **not** overturn — the whole-unit purchasing audit above.

**Decision labels (not measured pick rates):**
- **Avoid profile** = sourced criticism of a particular loadout or application; **do not infer that the whole sculpt is bad**.
- **Proxy first** = *inference* from costly/redundant/narrow role, limited list demand or explicit published criticism. Not an assertion that a video presenter called every profile terrible.
- **One is enough** = a duplicate miniature is lower priority than its AVA suggests.
- **Specialist build** = deliberately purchase only for its unique tool or a list actually tested. **Strong / contested** identifies disagreement; never equate a rare pick with an unusable one.

The source judgments below are anchored in the [PanO faction transcript audit above](panoceania.md#1-vanilla-pano--no-verified-universal-locked-unit), [Kestrel](../../notes/factions/kestrel.md), [NCA](../../notes/factions/nca.md), [Varuna](../../notes/factions/varuna.md), [SAA](../../notes/factions/acontecimento.md), [WinterFor](../../notes/factions/svalarheima.md) and the [current MO roster research](military-orders.md). Source labels are **Direct** (recorded reviewer criticism), **Contested** (other reviewers disagree) or **Inference** (purchase-priority conclusion from those reviews and N5.3 roster). The evaluation is for ordinary **300-point N5.3** lists, not narrow custom missions.

#### Svalarheima's Winter Force (WinterFor / SWF)

| Unit / choice | Why it is rarely the best default | Buy or proxy? |
|---|---|---|
| **Bøyg 44pt Mk12/ML** | **Direct/contested:** [Shepherd](https://www.youtube.com/watch?v=oHeTzuV9WLY) prefers much cheaper **Vargar** Albedo/Disco for general utility; Bøyg retains **W2/ARM5**, serious gun and Beta-team advantages. | **Proxy first / lowest-priority named heavy-infantry purchase** unless its survival and specific Beta role matter. |
| **Fusilier HMG, ML, Sniper** | **Direct — Shepherd:** generally weak SWC buys relative to Karhu/Nisse/Vargar/other legal guns. | **Avoid profiles; don't skip basic Fusilier LT/decoy**. One correctly based line-infantry miniature can cover rare weapon variants by declaration. |
| **Clipper FTO or Guided** | **Direct:** poor Guided-network default and **no legal SWF FTO Fireteam row**. | **Proxy first** from Dronbot pool; buy only if actual Targeted plan is tested. |
| **Oktavia Grímsdóttir; Gunnar FTO** | **Direct/contested:** [Swiss Miss](https://www.youtube.com/watch?v=-pVR0OSVP4w) and [Foxbringer](https://www.youtube.com/watch?v=RGInRCx1rRA) question their value versus Vargar / Shona / Valkyrie / other gun/CC utility. They have unique Albedo/Dogged/linked NCO-or-TacAware-related options. | **Proxy first** rather than buy two niche character sculpts; acquire one only after using her/him in a recurring legal Fireteam. |
| **Blade-Ops 30pt Decoy Parachutist/forward deployment** | **Direct — Foxbringer 2026:** pays a lot for mobility without actual Hidden Deployment; **23pt FTO Engineer + Tactical Awareness** is strongly liked by other reviewers. | **Avoid expensive loadout as default; do not skip Blade-Ops**. Proxy alternate Blade profiles as needed. |
| **Unlinked Pathfinder Tactical Awareness17** | **Contested:** Swiss Miss C-tier due to no SWF Fireteam access; Shepherd likes the independent Sensor/FO plus personal activation. | **Proxy/test one**; don't buy a second solely expecting a nonexistent linked activation. |
| **Second Jotum** | **Inference:** first Jotum is a highly rated ARM10 centerpiece; second is a genuine skew, but usually removes Orders, specialists and alternate mission reach. | **Proxy-test the second TAG** before paying for another large kit. **The first Jotum is NOT a worst-unit pick.** |

**Sources:** [Shepherd WinterFor](https://www.youtube.com/watch?v=oHeTzuV9WLY), [Swiss Miss WinterFor](https://www.youtube.com/watch?v=-pVR0OSVP4w), [Foxbringer 2026](https://www.youtube.com/watch?v=RGInRCx1rRA), [SWF tactical guide](../../notes/factions/svalarheima.md). Note that **SWF has no Redeye/VH**; don't proxy an illegal choice simply because another PanO sectorial uses it.
