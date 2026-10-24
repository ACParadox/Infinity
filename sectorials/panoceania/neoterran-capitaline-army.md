---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 104
sectorial_slug: neoterran-capitaline-army
sectorial_name: Neoterran Capitaline Army
parent_faction: PanOceania
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Neoterran Capitaline Army roster, standard loadouts, canonical Fireteam chart, and reverse Fireteam index. Indigo Spec-Ops and Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# Neoterran Capitaline Army

## Overview and provenance

Repository-native reference for **Neoterran Capitaline Army (NCA)** roster, profiles, points/SWC, AVA, and Fireteam access.

For **video/transcript-backed tactical guidance** (listbuilding, LT/CoC packages, threat redundancy, efficient Auxilia objective play, Fireteam and TAG architecture), see [`notes/factions/nca.md`](../../notes/factions/nca.md). The tactical note includes an October 2026 vidIQ transcript review of Robert Shepherd and Gravitypool, with rules/profile corrections. **This reference file remains the authoritative source for current roster facts; video opinions do not change Fireteam legality or profile data.**

Sources used:

- Army-derived NCA source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **36-unit standard NCA roster** and the complete NCA `fireteamChart` in the pinned Army source.
- Soldier of Fortune entries whose source faction list is empty are excluded from the base roster.
- `Indigo Spec-Ops` and `Indigo Team-Ops` are optional game-mode content and are listed separately.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name by itself. Clipper Dronbot and Aïda Swanson both have FTO-labelled options but no NCA Fireteam-chart row.
- Parenthetical Army-chart comments such as `(Fusilier)`, `(Bolts)`, `(CSU)`, and `(Orc Troops)` are Counts-as / equivalence labels, not join-scope restrictions.
- Aquila, Blade-Ops, and Uma Sørensen are profile-restricted Wildcards because their Wildcard rows explicitly carry an FTO marker. Agent Maximus is not FTO-restricted by the Wildcard chart row.
- Only one Maximus may be selected between **Optimate Agent Maximus** and **Maximus, Optimate and HexaDome Legend**.
- Linked Reinforcement section: **Code: Capital** (`army_id: 199`). No Reinforcement Fireteam rows are merged into the main chart here.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Neoterran Capitaline Army |
| Parent faction | PanOceania |
| Army ID | 104 |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 36 |
| Optional-mode units | Indigo Spec-Ops; Indigo Team-Ops |
| Reinforcement roster | Code: Capital (`199`) |
| Fireteam chart | yes |

## Roster index

| Unit | ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| Clipper Dronbot | 18 | 2 | REM | Regular | —; FTO-labelled option has no NCA chart row |
| Palbots | 37 | 2 | REM | Peripheral | — |
| Richard Quinn | 1490 | 1 | LI | Regular | Wildcard; counts as Fusilier / Bolt |
| Fusiliers | 1 | 5 | LI | Regular | Fusiliers |
| Captain Uma Sørensen | 1491 | 1 | MI | Regular | Wildcard, FTO profiles only; counts as Fusilier / Bolt |
| Neoterra Bolts | 4 | T | MI | Regular | Neoterra required-choice |
| Squalos Mk-II | 1651 | 2 | TAG | Regular | Ultima Ratio required-choice |
| PanOceanian Black Friar | 771 | 1 | MI | Regular | Wildcard |
| Blade-Ops | 1751 | 3 | LI | Regular | Wildcard, FTO profiles only; counts as Fusilier / Bolt |
| Bulleteer Armbots | 35 | 2 | REM | Regular | Wildcard |
| Sierra Dronbots | 17 | 2 | REM | Regular | — |
| Peacemaker Armbots | 36 | 2 | REM | Regular | — |
| Aquila Guard | 8 | 3 | HI | Regular | Wildcard, FTO profiles only |
| Redeye Close Air Support Squad | 1816 | 2 | VH | Regular | — |
| Machinist NCA | 15 | 1 | LI | Regular | Neoterra; counts as Bolt |
| ORC Troops | 5 | 5 | HI | Regular | Fusiliers; Neoterra; Ultima Ratio |
| Blockers | 1750 | 2 | LI | Regular | Fusiliers; Neoterra; CSU |
| Fugazi Dronbots | 19 | 3 | REM | Regular | — |
| Trauma-Docs | 14 | 1 | LI | Regular | — |
| Auxilia | 22 | T | LI | Regular | — |
| Clausewitz Uhlans | 32 | 2 | TAG | Regular | — |
| Aïda Swanson | 1160 | 1 | LI | Regular | —; FTO-labelled option has no NCA chart row |
| Warcors | 50 | 1 | LI | Irregular | — |
| Optimate Agent Maximus | 1862 | 1 | MI | Regular | Wildcard; counts as ORC |
| Garuda Tacbots | 110 | 1 | REM | Regular | — |
| Pathfinder Dronbots | 16 | 2 | REM | Regular | Wildcard |
| Mulebots | 38 | 2 | REM | Regular | — |
| Swiss Guard | 9 | 2 | HI | Regular | — |
| Hexas | 23 | 3 | LI | Regular | — |
| Hannibal, Neoterran Mercenary Team Leader | 1875 | 1 | MI | Regular | Wildcard; counts as ORC / Bolt |
| Tech-Bees | 935 | 1 | LI | Regular | — |
| Shona Carano | 1505 | 1 | MI | Regular | Wildcard |
| Deva Functionaries | 109 | 2 | MI | Regular | CSU |
| Maximus, Optimate and HexaDome Legend | 1720 | 1 | TAG | Regular | Ultima Ratio required-choice |
| Locust | 769 | 3 | SK | Regular | — |
| CSU | 122 | 2 | LI | Regular | Fusiliers; CSU |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Indigo Spec-Ops | 1912 | Spec-Ops | Fusiliers Fireteam row, max 1 when Spec-Ops mode is in use |
| Indigo Team-Ops | 1926 | Team-Ops | No ordinary NCA Fireteam row |

## Unit details

### Clipper Dronbot

**ID 18 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CCW (-3); BS Attack (Guided) | — |
| 5 | 19 | 1.5 | **CLIPPER DRONBOT FTO**; Missile Launcher (+1B), PARA CCW (-3) | —; no NCA chart row |

### Palbots

**ID 37 · AVA 2 · REM peripheral** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Peripheral (Servant), Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | PARA CCW (-3); no Order | — |

### Fusilier Indigo Richard Quinn

**ID 1490 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 13 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. MSV1, Warhorse, Immunity (ARM).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 0 | MULTI Marksman Rifle, Flash Pulse, D-Charges, Boarding Pistol (+1B), CCW; Forward Observer | Wildcard max 1; counts as Fusilier and Bolt |
| 2 | 24 | 0 | SMG, E/Mitter, Flash Pulse, D-Charges, Boarding Pistol (+1B), CCW; Chain of Command | same |
| 3 | 26 | 0 | MULTI Rifle, Flash Pulse, D-Charges, Disco Baller, Boarding Pistol (+1B), CCW; Forward Observer | same |

### Fusiliers

**ID 1 · AVA 5 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 10 | 0 | Combi Rifle, Pistol, CCW | Fusiliers min 1/max 5 |
| 2 | 18 | 1 | HMG, Pistol, CCW | same |
| 4 | 15 | 1.5 | Missile Launcher, Pistol, CCW | same |
| 5 | 16 | 1 | MULTI Sniper Rifle, Pistol, CCW | same |
| 6 | 15 | 0.5 | Combi Rifle; Hacking Device, Hacker | same |
| 8 | 12 | 0 | Combi Rifle, Flash Pulse; Deployable Repeater, Forward Observer | same |
| 9 | 12 | 0 | Combi Rifle; MediKit, Paramedic | same |
| 10 | 10 | 0 | Lieutenant; Combi Rifle | same |
| 12 | 12 | 0 | Combi Rifle; Commlink (+1), Specialist Operative | same |

### Captain Uma Sørensen

**ID 1491 · AVA 1 · MI** — `MOV 10-10 | CC 15 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Immunity (Shock), Combat Instinct, Mimetism (-3), Specialist Operative, Stealth, Terrain (Total), Climbing Plus.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 27 | 0 | SMG (+1B), E/M Mine, Silenced Pistol (+1B), CCW; Camouflage, Surprise Attack (-3), Forward Deployment (+20) | — |
| 2 | 25 | 0 | **UMA SØRENSEN FTO**; Breaker Combi Rifle, Silenced Pistol (+1B), CCW; X Visor | Wildcard max 1; counts as Fusilier and Bolt |
| 3 | 23 | 0 | **UMA SØRENSEN FTO**; SMG (+1B), E/M Mine, Silenced Pistol (+1B), CCW; X Visor | same |
| 4 | 25 | 0 | **UMA SØRENSEN FTO Lieutenant**; Breaker Combi Rifle, Silenced Pistol (+1B), CCW; X Visor | same |

### Neoterra Bolts

**ID 4 · AVA T · MI** — `MOV 10-10 | CC 16 | BS 13 | PH 11 | WIP 12 | ARM 2 | BTS 6 | W 1 | S 2`. Warhorse, Immunity (Shock), Marksmanship, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 21 | 0 | Combi Rifle, Light Shotgun, Drop Bears, Pistol, CCW | Neoterra required-choice max 5 |
| 3 | 19 | 0 | Boarding Shotgun (+1B), Drop Bears, Pistol, CCW | same |
| 4 | 24 | 1.5 | Missile Launcher, Pistol, CCW | same |
| 5 | 25 | 1.5 | Spitfire, Pistol, CCW | same |
| 6 | 26 | 0 | Combi Rifle, Light Shotgun, Drop Bears; Chain of Command | same |
| 7 | 24 | 0.5 | Boarding Shotgun (+1B), E/M Mine; Hacking Device, Hacker | same |
| 8 | 22 | 0 | Boarding Shotgun (+1B), E/M Mine; Killer Hacking Device, Hacker | same |
| 9 | 23 | 0 | Combi Rifle, Light Shotgun, Drop Bears; MediKit, Paramedic | same |
| 10 | 26 | 1.5 | MULTI Sniper Rifle; MSV1 | same |
| 11 | 21 | 0 | Lieutenant; Combi Rifle, Light Shotgun, Drop Bears | same |

### Squalos Mk-II

**ID 1651 · AVA 2 · TAG** — `MOV 15-10 | CC 18 | BS 15 | PH 15 | WIP 13 | ARM 6 | BTS 6 | W 3 | S 6`. ECM: Guided (-6), Remote Presence, Courage, Combat Instinct, Tactical Awareness, enhanced Dodge/GizmoKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 55 | 1 | MULTI Marksman Rifle, MULTI Pistol (+1B), CCW; Crabbot | Ultima Ratio required-choice max 2 |
| 2 | 62 | 1.5 | HMG, Grenade Launcher, MULTI Pistol (+1B), CCW; Crabbot | same |
| 3 | 66 | 1.5 | MULTI HMG, MULTI Pistol (+1B), CCW; NCO; Crabbot | same |

### PanOceanian Black Friar

**ID 771 · AVA 1 · MI** — `MOV 10-10 | CC 19 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. MSV2, Albedo (-6), Combat Instinct, Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 24 | 0 | Thunderbolt (+1B), Nanopulser, Pistol, CCW | Wildcard max 1 |
| 3 | 27 | 0 | MULTI Rifle, Nanopulser, Drop Bears, Pistol, CCW; Biometric Visor; Discover (+3) | same |
| 4 | 22 | 1.5 | Heavy Rocket Launcher, Nanopulser, MULTI Pistol (+1B), CCW | same |

### Blade-Ops

**ID 1751 · AVA 3 · LI** — `MOV 10-10 | CC 16 | BS 13 | PH 10 | WIP 12 | ARM 2 | BTS 3 | W 1 | S 2`. BS Attack (SR-1), Immunity (Shock), Mimetism (-3), Stealth, Terrain (Total), Tactical Awareness.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 20 | 0 | **BLADE FTO**; Boarding Shotgun, D-Charges, Silenced Pistol, CCW | Wildcard max 2; counts as Fusilier and Bolt |
| 2 | 23 | 0 | **BLADE FTO**; AP SMG, D-Charges, Silenced Pistol, CCW; Engineer, GizmoKit | same |
| 3 | 30 | 0 | AP SMG, E/Mitter, D-Charges, Silenced Pistol, CCW; Engineer, Forward Deployment (+20), Decoy (2) | — |
| 4 | 30 | 0 | AP SMG, E/Mitter, D-Charges, Silenced Pistol, CCW; Engineer, Parachutist, Decoy (2) | — |

### Bulleteer Armbots

**ID 35 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Repeater, Remote Presence, Courage, Mimetism (-6).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Heavy Shotgun (+1B), PARA CCW (-3) | Wildcard max 2 |
| 2 | 22 | 1 | Spitfire, PARA CCW (-3) | same |

### Sierra Dronbots

**ID 17 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage, Total Reaction, 360º Visor.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 1 | HMG, PARA CCW (-3) | — |
| 2 | 18 | 0 | Thunderbolt (+1B), PARA CCW (-3) | — |

### Peacemaker Armbots

**ID 36 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Repeater, Remote Presence, Courage, Forward Deployment (+20), Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Heavy Shotgun, Pulzar, PARA CCW (-3); Auxbot_3 | — |
| 3 | 24 | 0.5 | Heavy Shotgun, Pulzar, PARA CCW (-3); Auxbot_3B | — |
| 4 | 23 | 0 | Boarding Shotgun, Pulzar, PARA CCW (-3); BS Attack (+1B) | — |
| 5 | 27 | 0 | Boarding Shotgun, Pulzar, PARA CCW (-3); BS Attack (+1B); Auxbot_3 | — |

### Aquila Guard

**ID 8 · AVA 3 · HI** — `MOV 15-5 | CC 15 | BS 15 | PH 14 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 2`. MSV3, ECM: Hacker (-3), Deactivator, Courage, enhanced Jump.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 3 | 52 | 1.5 | HMG, MULTI Pistol, Shock CCW | — |
| 5 | 49 | 0 | **AQUILA FTO**; MULTI Marksman Rifle, Disco Baller, MULTI Pistol, Shock CCW; Specialist Operative | Wildcard max 3 |
| 7 | 49 | 0 | **AQUILA FTO Lieutenant**; same as 5 | same |
| 8 | 52 | +1 | **AQUILA FTO Lieutenant**; same as 5; Strategos L1 | same |

### Redeye Close Air Support Squad

**ID 1816 · AVA 2 · VH** — `MOV 20-5 | CC — | BS 14 | PH 13 | WIP 13 | ARM 6 | BTS 6 | W 2 | S 7`. Aerial, Courage, Mimetism (-6), Remote Presence, Sensor, No Cover, Super-Jump (Jet Propulsion), Tech-Recovery, Terrain (Total), enhanced Dodge/GizmoKit.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 37 | 1.5 | Spitfire, Chain Rifle, Blitzen | — |
| 2 | 38 | 1.5 | Spitfire, Chain Rifle, Grenade Launcher (Continuous Damage) | — |

### Machinist NCA

**ID 15 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`. Engineer, Deactivator, GizmoKit; NCA profiles also have Warhorse, Immunity (Shock), Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4 | 17 | 0 | Combi Rifle, D-Charges, Pistol, CCW | Neoterra max 1; counts as Bolt |
| 17 | 18 | 0 | As 4 + Deployable Cover | same |
| 18 | 20 | 0 | Combi Rifle, D-Charges, Armed Turret (Combi Rifle), Pistol, CCW | same |

### ORC Troops

**ID 5 · AVA 5 · HI** — `MOV 15-5 | CC 15 | BS 14 | PH 14 | WIP 12 | ARM 4 | BTS 3 | W 2 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 28 | 0 | MULTI Rifle, Pistol, CCW | Fusiliers max 2; Neoterra required-choice max 5; Ultima Ratio max 1 |
| 2 | 29 | 0 | MULTI Rifle; TinBot: Firewall (-3) | same |
| 3 | 34 | 1.5 | HMG | same |
| 4 | 26 | 0 | Boarding Shotgun (+1B) | same |
| 6 | 33 | 0.5 | MULTI Rifle; Hacking Device, Hacker | same |
| 7 | 28 | 0 | Lieutenant; MULTI Rifle | same |
| 8 | 34 | 1 | Lieutenant; HMG | same |
| 10 | 35 | 1.5 | Feuerbach | same |
| 11 | 27 | 0 | Boarding Shotgun (+1B); TinBot: Firewall (-3) | same |

### Blockers

**ID 1750 · AVA 2 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Biometric Visor, X Visor, BS Attack (+1B), Sensor, Discover (ReRoll).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 15 | 0 | Adhesive Launcher Rifle, Pitcher, Pulzar, Flash Pulse, MULTI Pistol, PARA CCW (-6); Specialist Operative | Fusiliers max 2/counts as Fusilier; Neoterra max 2; CSU max 2/counts as CSU |
| 2 | 19 | 0.5 | Adhesive Launcher Rifle, Pulzar, Flash Pulse, MULTI Pistol, PARA CCW (-6); Hacking Device (Firewall -3), Hacker | same |

### Fugazi Dronbots

**ID 19 · AVA 3 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Remote Presence, Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) | — |

### Trauma-Docs

**ID 14 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. Doctor, MediKit.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Pistol, CCW | — |

### Auxilia

**ID 22 · AVA T · LI** — `MOV 10-10 | CC 16 | BS 11 | PH 10 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 15 | 0 | Combi Rifle, Nanopulser (+1B), Pistol, CCW; Auxbot_1 | — |
| 2 | 18 | 0 | Combi Rifle, Flash Pulse, Nanopulser (+1B), Pistol, CCW; Forward Observer; Auxbot_2 | — |
| 3 | 15 | 0 | SMG, Flash Pulse, Pistol, CCW; Deployable Repeater, Forward Observer; Auxbot_2 | — |
| 4 | 15 | 0 | Lieutenant; Combi Rifle, Nanopulser (+1B), Pistol, CCW; Auxbot_1 | — |

### Clausewitz Uhlans

**ID 32 · AVA 2 · TAG** — `MOV 15-10 | CC 15 | BS 15 | PH 15 | WIP 12 | ARM 6 | BTS 6 | W 3 | S 6`. ECM: Guided (-6), Camouflage, Mimetism (-3), Surprise Attack (-3), Remote Presence, Courage, Tactical Awareness, Warhorse, enhanced Dodge/GizmoKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 80 | 1.5 | Spitfire, Heavy Rocket Launcher (+1B), AP CCW; BS Attack (AP); Crabbot | — |
| 2 | 70 | 1.5 | Feuerbach, Panzerfaust, Blitzen, MULTI Pistol, AP CCW; BS Attack (+1B); Crabbot | — |

### Aïda Swanson

**ID 1160 · AVA 1 · LI** — `MOV 10-10 | CC 19 | BS 12 | PH 11 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Martial Arts L2, Courage, Booty, Mimetism (-3), Stealth, Shasvastii.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 0.5 | SMG (+1B), Viral Mine, Viral Pistol, Shock CCW; Forward Deployment (+10), Minelayer, Decoy (2) | — |
| 2 | 21 | 0 | **AÏDA SWANSON FTO**; SMG, Viral Mine, Viral Pistol, Shock CCW; Minelayer | —; no NCA chart row |

### Warcors

**ID 50 · AVA 1 · LI · Irregular** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Journalist.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor | — |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); Sixth Sense | — |

### Optimate Agent Maximus

**ID 1862 · AVA 1 · MI** — `MOV 15-5 | CC 22 | BS 13 | PH 13 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Albedo (-3), Courage, Natural Born Warrior, Immunity (ARM), Number 2, Specialist Operative, Tactical Awareness, NWI, enhanced CC/Dodge.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 48 | 1 | **MAXIMUS AGENT**; AP Thunderbolt (+2B), E/M Carbine, Heavy Pistol, AP+DA CCW; Minimus Peripheral | Wildcard max 1; counts as ORC |
| 2 | 45 | 1 | **MAXIMUS AGENT FTO**; same main weapons; TinBot (Repeater) | same |
| 5 | 47 | +1 | **MAXIMUS AGENT FTO Lieutenant**; same; TinBot (Repeater), Inspiring Leadership | same |

Only one Maximus may be selected between this unit and Maximus TAG (ID 1720).

### Garuda Tacbots

**ID 110 · AVA 1 · REM** — `MOV 20-5 | CC 13 | BS 12 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`. Remote Presence, Courage, Mimetism (-3), Parachutist, Combat Jump, Super-Jump (Jet Propulsion).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 3 | 18 | 0 | Boarding Shotgun, Chain-colt, PARA CCW (-3) | — |
| 4 | 25 | 1.5 | Spitfire, PARA CCW (-3) | — |
| 5 | 20 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3); Forward Observer | — |

### Pathfinder Dronbots

**ID 16 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Deactivator, Remote Presence, Courage, Triangulated Fire, Forward Observer, Sensor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3) | Wildcard max 2 |
| 2 | 17 | 0 | As 1 + Tactical Awareness | same |

### Mulebots

**ID 38 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 4`. Baggage, Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | Deactivator, Repeater, PARA CCW (-3) | — |
| 2 | 14 | 0.5 | EVO Hacking Device; Hacker; PARA CCW (-3) | — |
| 3 | 17 | 0 | Combi Rifle, Repeater, PARA CCW (-3); Total Reaction | — |

### Swiss Guard

**ID 9 · AVA 2 · HI** — `MOV 10-10 | CC 15 | BS 15 | PH 14 | WIP 13 | ARM 5 | BTS 6 | W 2 | S 2`. Camouflage, Hidden Deployment, Mimetism (-6), Surprise Attack (-3), Stealth.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 56 | 1.5 | HMG, Pulzar, Heavy Pistol, AP CCW | — |
| 3 | 60 | 1.5 | Missile Launcher (+1SD), Light Shotgun, Pulzar, Heavy Pistol, AP CCW | — |
| 4 | 56 | 0.5 | MULTI Rifle, Pulzar, Flammenspeer, Heavy Pistol, AP CCW; Hacking Device, Hacker, X Visor | — |
| 5 | 44 | 0 | AP SMG, Pulzar, Flammenspeer, Heavy Pistol, AP CCW; TinBot: Firewall (-3), Martial Arts L1, CC=21, Forward Deployment (+10) | — |
| 6 | 47 | 0 | As 5 + Killer Hacking Device, Hacker | — |

### Hexas

**ID 23 · AVA 3 · LI** — `MOV 10-10 | CC 17 | BS 13 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Counterintelligence, Camouflage, Hidden Deployment, Mimetism (-6), Surprise Attack (-3), Courage, Stealth, Immunity (Shock).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 31 | 1.5 | Spitfire, E/Marat, Silenced Pistol (+1B), PARA CCW (-3); X Visor | — |
| 3 | 30 | 1.5 | MULTI Sniper Rifle, Silenced Pistol (+1B), PARA CCW (-3) | — |
| 4 | 30 | 0.5 | Combi Rifle, Panzerfaust, D-Charges, Silenced Pistol (+1B), PARA CCW (-3); Hacking Device, Hacker | — |
| 5 | 27 | 0 | Combi Rifle, E/Marat, D-Charges, Silenced Pistol (+1B), PARA CCW (-3); Killer Hacking Device, Hacker | — |

### Hannibal, Neoterran Mercenary Team Leader

**ID 1875 · AVA 1 · MI** — `MOV 10-10 | CC 15 | BS 13 | PH 11 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. BS Attack (+1SD), Courage, enhanced Dodge, Immunity (Shock), Sensor, Tactical Awareness, NWI.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Vulkan Shotgun, Nanopulser (+1B), Flash Pulse, Breaker Pistol, CCW | Wildcard max 1; counts as ORC and Bolt |
| 2 | 29 | 0 | MULTI Marksman Rifle, Nanopulser (+1B), Breaker Pistol, CCW | same |
| 3 | 26 | 0 | As 1 + Strategic Deployment | same |
| 4 | 32 | +1 | As 2 + Strategic Deployment | same |

### Tech-Bees

**ID 935 · AVA 1 · LI** — `MOV 10-10 | CC 12 | BS 11 | PH 10 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 2`. Specialist Operative, TAGCom, Deactivator, GizmoKit.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 2 | 9 | 0 | Adhesive Launcher Rifle, Flash Pulse, Pistol, PARA CCW (-3); Deployable Repeater | — |

### Shona Carano

**ID 1505 · AVA 1 · MI** — `MOV 15-5 | CC 23 | BS 11 | PH 14 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Martial Arts L4, Courage, Frenzy, Stealth, NWI, Super-Jump, Immunity (Shock), enhanced Dodge.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 22 | 0 | SMG, Nanopulser (+1B), Flash Pulse, Pistol, AP+EXP CCW | Wildcard max 1 |

### Deva Functionaries

**ID 109 · AVA 2 · MI** — `MOV 10-10 | CC 15 | BS 12 | PH 11 | WIP 15 | ARM 2 | BTS 3 | W 1 | S 2`. Courage, Number 2, NWI, Immunity (Isolated).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 20 | 0 | Combi Rifle, Nanopulser, Pistol, CCW | CSU max 1 |
| 2 | 24 | 0 | As 1 + Devabot | same |
| 3 | 22 | 0 | MULTI Rifle, Nanopulser, Pistol, CCW | same |
| 4 | 25 | 0.5 | Combi Rifle, Nanopulser; Hacking Device, Hacker | same |
| 5 | 20 | 0 | Boarding Shotgun; Killer Hacking Device, Hacker | same |
| 6 | 21 | 0 | Combi Rifle, Nanopulser; Triangulated Fire, Sensor | same |
| 8 | 21 | 0 | Combi Rifle, Nanopulser, Flash Pulse; Forward Observer | same |
| 9 | 29 | 1 | Spitfire, Nanopulser; MSV2 | same |

### Maximus, Optimate and HexaDome Legend

**ID 1720 · AVA 1 · TAG** — `MOV 15-10 | CC 24 | BS 14 | PH 13 | WIP 13 | ARM 6 | BTS 6 | W 4 | S 6`. ECM: Guided (-6), Courage, Natural Born Warrior, Immunity (ARM, POS), Tactical Awareness, Transmutation / Escape System, enhanced CC/Dodge.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 82 | 1.5 | AP HMG, E/M Carbine, Heavy Pistol, AP+DA CCW | Ultima Ratio required-choice max 1 |
| 2 | 80 | 1 | AP Thunderbolt (+2B), E/M Carbine, Heavy Pistol, AP+DA CCW | same |
| 4 | 84 | 0 | Lieutenant; AP HMG, E/M Carbine, Heavy Pistol, AP+DA CCW; Inspiring Leadership | same |

Only one Maximus may be selected between this unit and Optimate Agent Maximus (ID 1862).

### Locust, Clandestine Action Team

**ID 769 · AVA 3 · SK** — `MOV 10-10 | CC 16 | BS 12 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Bangbomb, Hidden Deployment, Mimetism (-6), Surprise Attack (-3), Forward Deployment (+20), Stealth, Terrain (Total), enhanced Climb.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 3 | 24 | 0 | Boarding Shotgun, Grenades, Drop Bears, Boarding Pistol, CCW; Specialist Operative | — |
| 4 | 27 | 0 | MULTI Marksman Rifle, Boarding Pistol, CCW | — |
| 5 | 21 | 0 | SMG, D-Charges, WildParrot, Boarding Pistol, CCW | — |
| 6 | 29 | 0.5 | Breaker Combi Rifle, Pitcher, D-Charges, Boarding Pistol, CCW; Hacking Device (Firewall -3), Hacker | — |
| 7 | 27 | 0 | Breaker Combi Rifle, Pitcher, D-Charges, Boarding Pistol, CCW; Killer Hacking Device (Firewall -3), Hacker | — |
| 8 | 31 | 0.5 | Breaker Combi Rifle, Flash Pulse, D-Charges, Boarding Pistol, CCW; Hacking Device (Firewall -3), Hacker; Camouflage (1 Use) | — |

### CSU, Corporate Security Unit

**ID 122 · AVA 2 · LI** — `MOV 10-10 | CC 16 | BS 12 | PH 10 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 2`. MetaChemistry, Sixth Sense.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 10 | 0 | Breaker Rifle, Nanopulser (+1B), MULTI Pistol, PARA CCW (-6) | Fusiliers max 2/counts as Fusilier; CSU min 1/max 2 |
| 2 | 11 | 0 | Combi Rifle, Nanopulser (+1B), MULTI Pistol, PARA CCW (-6) | same |
| 3 | 11 | 0 | Boarding Shotgun, Adhesive Launcher Rifle (+1B), MULTI Pistol, PARA CCW (-6) | same |
| 4 | 11 | 0 | Rifle, Light Shotgun, Nanopulser (+1B), MULTI Pistol, PARA CCW (-6); Specialist Operative | same |
| 5 | 13 | 0 | Breaker Combi Rifle, Nanopulser (+1B), MULTI Pistol, PARA CCW (-6); Specialist Operative | same |

## Fireteams

This section is **canonical**. The Unit → Fireteam access index below is derivative.

### Chart limits

| Type | Raw source | Meaning |
|---|---:|---|
| Core | 1 | Maximum 1 |
| Haris | 1 | Maximum 1 |
| Duo | 256 | InfinityDB-normalized meaning: unlimited |

### FT-NCA-01 — Fusiliers Fireteams

**Types:** Core, Haris

| Member | Unit ID | Min | Max | Required | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Fusilier | 1 | 1 | 5 | No | — | — |
| ORC | 5 | 0 | 2 | No | — | — |
| CSU | 122 | 0 | 2 | No | Fusilier | — |
| Blocker | 1750 | 0 | 2 | No | Fusilier | — |
| Indigo | 1912 | 0 | 1 | No | Spec-Ops | Optional Spec-Ops mode |

At least one Fusilier is required by the explicit source `min: 1`.

### FT-NCA-02 — Neoterra Fireteams

**Types:** Core, Haris, Duo

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| ORC | 5 | 0 | 5 | Yes | — | — |
| Bolt | 4 | 0 | 5 | Yes | — | — |
| Machinist NCA | 15 | 0 | 1 | No | Bolt | — |
| Blocker | 1750 | 0 | 2 | No | — | — |

ORC and Bolt are both marked `required: true` in the structured chart; they form the source required-choice set rather than requiring both unit types simultaneously.

### FT-NCA-03 — Ultima Ratio Fireteams

**Type:** Duo

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| Squalos Mk-II | 1651 | 0 | 2 | Yes | — | — |
| Maximus Optimate TAG | 1720 | 0 | 1 | Yes | — | — |
| ORC | 5 | 0 | 1 | No | — | — |

Squalos Mk-II and Maximus Optimate are the source required-choice set.

### FT-NCA-04 — CSU Fireteams

**Type:** Duo

| Member | Unit ID | Min | Max | Required | Counts as | FTO restriction |
|---|---:|---:|---:|---|---|---|
| CSU | 122 | 1 | 2 | No | — | — |
| Blocker | 1750 | 0 | 2 | No | CSU | — |
| Deva | 109 | 0 | 1 | No | — | — |

The structured source places an explicit `min: 1` on the CSU row. The Blocker carries a separate `CSU` equivalence label; this file preserves both facts rather than inferring a different minimum rule.

### Wildcards

All rows below are in the chart's **Wildcards** row. Parenthetical values are Counts-as labels, not join-scope restrictions.

| Wildcard | Unit ID | Max | Counts as | FTO/profile restriction |
|---|---:|---:|---|---|
| Aquila | 8 | 3 | — | FTO options 5, 7, 8 only |
| Blade FTO | 1751 | 2 | Fusilier, Bolt | FTO options 1, 2 only |
| Bulleteer | 35 | 2 | — | all |
| Pathfinder Dronbot | 16 | 2 | — | all |
| Black Friar | 771 | 1 | — | all |
| Quinn | 1490 | 1 | Fusilier, Bolt | all |
| Uma Sørensen | 1491 | 1 | Fusilier, Bolt | FTO options 2, 3, 4 only |
| Shona Carano | 1505 | 1 | — | all |
| Hannibal | 1875 | 1 | ORC, Bolt | all |
| Maximus Agent | 1862 | 1 | ORC | all Agent loadouts; chart row is not FTO-restricted |

Wildcard status does not remove the native minimum/required-choice conditions of the Fireteam being joined. Counts-as labels remain relevant to composition.

## Unit → Fireteam access index

| Unit | Fireteam access |
|---|---|
| Clipper | —; FTO-labelled option has no NCA chart row |
| Palbot | — |
| Quinn | Wildcard max 1; counts as Fusilier and Bolt |
| Fusilier | FT-NCA-01 min 1/max 5 |
| Uma Sørensen | Wildcard max 1, **FTO options 2/3/4 only**; counts as Fusilier and Bolt |
| Bolt | FT-NCA-02 required-choice max 5 |
| Squalos Mk-II | FT-NCA-03 required-choice max 2 |
| Black Friar | Wildcard max 1 |
| Blade-Ops | Wildcard max 2, **FTO options 1/2 only**; counts as Fusilier and Bolt |
| Bulleteer | Wildcard max 2 |
| Sierra | — |
| Peacemaker | — |
| Aquila | Wildcard max 3, **FTO options 5/7/8 only** |
| Redeye | — |
| Machinist NCA | FT-NCA-02 max 1; counts as Bolt |
| ORC | FT-NCA-01 max 2; FT-NCA-02 required-choice max 5; FT-NCA-03 max 1 |
| Blocker | FT-NCA-01 max 2/counts as Fusilier; FT-NCA-02 max 2; FT-NCA-04 max 2/counts as CSU |
| Fugazi | — |
| Trauma-Doc | — |
| Auxilia | — |
| Uhlan | — |
| Aïda Swanson | —; FTO-labelled option has no NCA chart row |
| Warcor | — |
| Optimate Agent Maximus | Wildcard max 1; counts as ORC; all Agent loadouts allowed by chart row |
| Garuda | — |
| Pathfinder | Wildcard max 2 |
| Mulebot | — |
| Swiss Guard | — |
| Hexa | — |
| Hannibal | Wildcard max 1; counts as ORC and Bolt |
| Tech-Bee | — |
| Shona Carano | Wildcard max 1 |
| Deva | FT-NCA-04 max 1 |
| Maximus TAG | FT-NCA-03 required-choice max 1 |
| Locust | — |
| CSU | FT-NCA-01 max 2/counts as Fusilier; FT-NCA-04 min 1/max 2 |
| Indigo Spec-Ops | FT-NCA-01 max 1 when Spec-Ops mode is in use |
| Indigo Team-Ops | — in the ordinary NCA chart |

## Tactical tags

Derived analysis aids, not official characteristics.

| Unit | Tags |
|---|---|
| Fusilier | cheerleader, long-range ARO, hacker, specialist, network projection, link anchor |
| Quinn | specialist, Chain of Command, mid-range attack, network projection, Wildcard |
| Uma Sørensen | midfield specialist, camo attack, lieutenant option, Wildcard |
| Bolt | mid-range attack, long-range ARO, hacker, KHD, specialist, Chain of Command, link anchor |
| ORC | durable attack, hacker, long-range attack, link anchor |
| Machinist NCA | Engineer, tech-counter, deployable support, link support |
| CSU | cheap link member, close defense, specialist |
| Blocker | network projection, hacker, Sensor, tech-counter, specialist, link support |
| Aquila | MSV3, anti-camo, mid/long-range attack, specialist, Strategos LT option, Wildcard |
| Black Friar | MSV2, anti-camo, long-range ARO, Wildcard |
| Blade-Ops | Tactical Awareness, Engineer, airborne option, midfield specialist, Wildcard |
| Hannibal | Tactical Awareness, Sensor, mid-range attack, Strategic Deployment, Wildcard |
| Shona Carano | close assault, Wildcard |
| Agent Maximus | Tactical Awareness, close/mid-range attack, specialist, LT option, Wildcard |
| Squalos Mk-II | TAG, Tactical Awareness, long-range attack, NCO option, Ultima Ratio |
| Maximus TAG | TAG, Tactical Awareness, close assault, long-range attack, LT option, Ultima Ratio |
| Uhlan | TAG, Camouflage, Tactical Awareness, long-range attack |
| Swiss Guard | hidden deployment, long-range attack, hacker, KHD, midfield attack option |
| Hexa | hidden deployment, long-range attack/ARO, hacker, KHD, Counterintelligence |
| Locust | hidden deployment, midfield specialist, network projection, hacker, KHD |
| Aïda Swanson | midfield defense, Minelayer, deception |
| Auxilia | DZ defense, specialist option, network projection option |
| Peacemaker | midfield defense, forward REM attack, network projection |
| Bulleteer | REM attack, Mimetism (-6), mid-range attack, network projection, Wildcard |
| Pathfinder | specialist, Sensor, network projection, Tactical Awareness option, Wildcard |
| Fugazi | cheerleader, network projection, flash ARO |
| Mulebot | Baggage, EVO, REM support, cheerleader |
| Sierra | long-range ARO, Total Reaction |
| Clipper | guided missile, long-range ARO |
| Redeye | fast attack, Sensor, tech-counter |
| Garuda | airborne, enemy-DZ attacker, specialist option |
| Trauma-Doc | Doctor, recovery support |
| Palbot | Doctor/Engineer projection support |
| Tech-Bee | TAG support, tech-counter, network projection |
| Deva | hacker, KHD, Sensor, MSV2, specialist, CSU link support |
| Warcor | cheap irregular ARO |

## Validation and maintenance

- Standard roster represented: **36 units**.
- Optional-mode hooks: Indigo Spec-Ops and Indigo Team-Ops.
- Canonical Fireteam rows represented: **Fusiliers, Neoterra, Ultima Ratio, CSU, Wildcards**.
- Limits preserved: `CORE 1`, `HARIS 1`, raw `DUO 256` = InfinityDB `unlimited`.
- Parenthetical source comments are stored as Counts-as/equivalence labels.
- Wildcard FTO restrictions are applied only where the Wildcard row explicitly carries an FTO marker.
- No Fireteam access is inferred solely from a loadout having `FTO` in its name.
- Clipper option 5 and Aïda option 2 are deliberately shown with no Fireteam access because neither unit has an NCA Fireteam-chart row.
- Agent Maximus is deliberately treated as an unrestricted Wildcard row because the chart says `MAXIMUS AGENT (Orc Troops)` without an FTO marker.
- Agent Maximus and Maximus TAG mutual exclusion is preserved.
- Main and Reinforcement Fireteams are not merged.

## Provenance

- Corvus Belli Army-derived source revision: `7.26246.158`.
- Army snapshot commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- Army data changed on / snapshot date: `2026-09-03`.
- InfinityDB semantic cross-check: `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Fireteam source: pinned Army `fireteamChart`, normalized using the same semantics documented in InfinityDB.
- Verified: `2026-10-15`.

## Mission specialist choices — N5.3 cross-game evaluation

**Auxilia** brings a cheap Specialist with an **Auxbot synchronized ARO/attack fork** where the chosen option qualifies; **Deva KHD20/FO21** is WIP15 NWI but uses different loadouts; **Pathfinder FO/Sensor14/TA17** gives independent repeater/anti-Camo access if roster-legal. A **Swiss Guard** or premier TAG clears lanes, **not necessarily the Console**; leave real late-stage mission scoring models alive. Only currently eligible FTO/team rows permit shared moves.

See [Mission Specialists / Button Pushers apex and value tiers](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). This roster and its Fireteam chart are the final authority for exact options.

## N5.3 airborne / enemy-DZ profile and value choices (2026-10-23)

**Garuda BSG18/0 or FO20/0** delivers MOV20-5/Mimetism(-3) through **Combat Jump(PH11 = 55% before modifiers)** or reliable normal Parachutist side entry. **Blade-Ops Engineer/Parachutist30/0 + Tactical Awareness and Decoy(2)** is a sustained technical backline fork, while **Blade Engineer FD+20 30/0** and **linked FTO Engineer23/0** are other mutually exclusive profiles. **Swiss Guard / Hexas Hidden** can threaten a line from concealment, but neither gets enemy-DZ Infiltration by default. A Redeye is an on-table aerial VH, not Combat Jump.

[Cross-game N5.3 airborne/rear-strike apex-value and landing-risk tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **Use this roster and canonical Fireteam chart for exact legality.**

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **Squalos Mk-II MMR55/1** is the economical **TAG** when a Pathfinder can also score/sense; **HMG62/1.5** instead clears long lanes. **Uhlan Feuerbach70/1.5** buys Camo/Surprise and armor-threatening long shots; **Spitfire80/1.5** prefers a closer approach. **WIP12 E201 disagreement:** repeatable visible Squalos attack versus Uhlan surprise; neither Uhlan profile receives automatic Ultima Ratio team access. [Gunfighter apex/value with separate TAG category](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## TAG tactical cross-reference (2026-10-23)

**Uhlan Feuerbach (70)** is a camouflaged +1B standoff/ARO piece; **Uhlan Spitfire+AP HRL (80)** is an advancing attacker. **Squalos NCO MULTI HMG (66) + tactical Pathfinder** makes a purposeful Ultima Ratio Duo (gun + Sensor/FO + movement Order); **Maximus TAG** is a very different close-assault/Immunity investment. Uhlan does **not** inherit Squalos Fireteam rights. See [NCA tactical analysis](../../notes/factions/nca.md).

Cross-faction **apex vs points-value** comparisons, matchup table, and direct MCP-reviewed podcast/video sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Current profile and Fireteam legality above remain authoritative.

## Vehicle (VH) tactical cross-reference (2026-10-23)

**Redeye AVA2:** **37/1.5 Blitzen** deters heavy targets; **38/1.5 GL** can reach prone/hidden defenders without frontal LoF. **WIP12 #201 NCA (Mar 2026)** values its BS14/Sensor/Aerial angles and a **Parachutist Blade Engineer** for distant ranged GizmoKit recovery. **Against:** No Cover, Hackable, SWC tax and need for Uhlan/Swiss/Squalos to suppress hard ARO first; no Redeye Fireteam rights.

See [VH apex/value tier list and matchup guide](../../notes/list-building/vehicles-vh.md). **This sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative.**

## Hacker and KHD tactical cross-reference (2026-10-23)

**19/0.5 Blocker HD + Firewall(-3)** is a cheap backline defensive anchor; **20/0 Deva KHD** combines WIP15/NWI/Immunity(Isolated) for better anti-Hacker and mission resilience. **Hexa HD 30/0.5 vs KHD 27/0**, **Locust KHD/Pitcher 27/0** exploit Hidden/Camo positioning, while **Bolt KHD 22/0** is cheaper Warhorse protection. **Fusilier HD 15/0.5** is the budget general HD; a **Swiss Guard 47/0 KHD or 56/0.5 HD** should be bought for Hidden Deployment attack/scoring, *not* as a backfield hacker. Use existing fast REM/FO projection; current NCA Fireteam chart does not automatically let those skirmishers join.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

The N5.3 [cheerleader/order-generator apex and value guide](../../notes/list-building/cheerleaders-and-order-generators.md) contrasts Orders-per-point, passive utility, matchup dependence, and opposing transcript opinions. **Use this roster for legal AVA, exact profile costs, Training and Fireteam restrictions.**

- 7pt Fugazi — Flash Pulse/Mimetism/Repeater Regular bot: usually prime passive fuel, with S3 footprint and AVA caveats.
- 8pt Mulebot — Baggage/Repeater Regular support; reload and a protected DZ slot increase its value.
- Fusilier/Fennec — about 10pt small-base Regular line material where legal; costs more than a Flashbot but helps meet link, LT, defensive and scoring requirements.
- Warcor — a 3pt Irregular Flash ARO speedbump, not a transferable pool Order without actual conversion.
- Peacemaker — pricier Regular REM/peripheral defensive coverage and network projection; not an economical pure cheerleader.

**Decision:** first buy enough protected *transferable* Regular Orders for the actual Combat Group attacker/scoring plan, then pay for genuine role compression. Irregular/Impetuous, LT, Tactical Awareness and Peripheral bodies are different resources. Account for a packed S3/S4 deployment zone and mandatory Fireteam members.


## ARO apex/value cross-reference (2026-10-23)

See [Best ARO Units — N5.3 apex and cost-value tiers](../../notes/list-building/aro-units-apex-and-value.md) for gunfighter vs hidden-trap vs cheap Order-tax comparisons, when each wins, transcript disagreements and counterplay. **The roster, prices/AVA and canonical Fireteam chart above remain authoritative**; a shared unit's permissions do not transfer between armies.

- **Swiss Guard ML** — apex hidden missile ambush; 60pt buys +SD and durable reveal, but hidden/undeployed contributes no normal early Order
- **Sierra Thunderbolt TR** — 18pt/0SWC multi-arc Regular ARO where profile legal; add Engineer/recovery if its lane matters repeatedly
- **Warcor Flash Pulse** — 3pt Irregular zero-SWC Order-tax ARO; never count as a generic Regular Order
- **Fugazi Flash/Repeater** — 7pt Regular cheap secondary ARO and hacking net; not a main gun
- **Peacemaker/Auxbot screen** — template and multi-body route denial; protect arrival corners rather than expose controller

**Deployment choice:** put the disposable/tax ARO on the approach, preserve a separate hidden/mission-denial gate where legal, and avoid leaving an expensive active-turn gun as your only exposed defence. Test pie-slicing, Smoke/Eclipse/White Noise, hacking, AD entry, recovery access and specialist survival before paying more SWC for a second sniper.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Recovery:** **Blade Engineer** offers **Parachutist/Decoy** repair access to forward Redeye/REM routes (WIP12+GizmoKit where legal), as discussed in WIP12 E201; this beats rear support only if safe entry exists. **Machinist17 WIP12 + Palbot3** is the simpler long-term Remote Presence net; token reroll makes 60% become **84%** if legal. **Trauma-Doc14** is similarly cheap VITA-only support. [Doctor/Engineer apex, points-value, recovery odds and transcript disputes](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## N5.3 DZ defense / anti-alpha-strike tactical choices

**Auxilia + synchronized Auxbot 15/0** (or **FO+Auxbot 15/0** alternate option) is the reusable *close-corner* answer to a Hellcat/Fiday racing at cheerleaders: two bodies threaten an overlapping advance while the controller still supplies one Regular Order and, on FO option, a specialist. **Warcor 360º 3/0** is a separate rear-facing Flash tax; **Sierra 18/0 360º/TR** covers the outer/vertical angle. **Counterpoint (WIP12 #201):** proactive **Peacemaker 27/0 +1B/Auxbot** can outperform a 24/.5 Minelayer when its active assault is valuable. Do not count an Auxbot as a second independently generated Regular Order, or a merely carried mine as turn-zero Minelayer.

[Whole-game DZ-defender apex/value tiers and media disagreements](../../notes/list-building/dz-defenders-alpha-strike-and-impersonation-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**NCA has no rostered Oniwaban/Fiday-style dedicated CC assassin.** **Aquila Guard52/1.5** is a BS15/MSV3 gunfighter with **CC15**, not a sword specialist; **Blade-Ops20** (CC16) and Bolts (CC16) solve corners with shotguns/mines rather than serious melee. **Counter-CC:** screen valuable Aquila/Swiss/REM with cheap bodies, mines and layered AROs; kill incoming markers at range or by Discover/Sensor rather than rolling against MA4/Monofilament at base contact. [CC apex/value and reach-versus-lethality comparisons](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## N5.3 network projection — Pitchers, Repeaters, TinBots and disposable delivery

**Blocker Specialist Operative Pitcher15/0** is one of the cheapest **projectors who can join actual Fusilier/CSU teams**; range reliability improves with legal FT bonuses. **Locust KHD/Pitcher27/0 or HD/Pitcher29/.5** brings a tougher infiltrated projector/mission piece; **Auxilia FO+Deployable Repeater15/0** controls a corner by activation alongside synchronized bot. **Peacemaker native Repeater FD(+20)** and **Fugazi7/0** are the physical options; **Maximus Agent FTO45/1 TinBot(Repeater)** extends a legal Fireteam, not an independent Repeater. **Opposing WIP12 NCA:** 27pt active +1B Peacemaker often beats 24/.5 Minelayer for fighting, but passive network/T0 mine is valuable going second.

[Whole-game network projection apex/value, transcript disagreements and matchup selection](../../notes/list-building/network-projection-repeaters-pitchers-apex-value.md). Local profile tables and actual Fireteam chart take precedence.

## N5.3 rare abilities & unusual combinations — tactical synthesis

**Black Friar24/0 MSV2+Albedo(-6)+Combat Instinct** is a compact anti-MSV/anti-camo gun; **27/0 Biometric+Drop Bears** helps against enemy impersonators instead. **Apsaras/RemDriver not part of NCA by implication**: evaluate only the actual source roster. **Auxilia FO+Auxbot15/0** is a strong two-body close assault/mission package but the **Auxbot is NOT automatically Forward Observer**; controller supplies one Order. **Maximus Agent FTO45/1 TinBot(Repeater)** uses actual legal teams, not a free repeater token. **When**: Friar for enemy visor/camo, Auxilia for close choke, Pathfinder for cheaper FO/Sensor; too many unusual support roles weaken NCA's proper premium gun.

[Whole-game rare capability apex/value, rules, matchups and opposing MCP transcripts](../../notes/list-building/rare-capabilities-and-unique-combinations-apex-value.md). Use current profile and Fireteam chart above.

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Fusilier Missile Launcher15/1.5** is inexpensive but low-Burst and exposed; **Bolts ML24/1.5**, **Quinn24 E/Mitter+Chain of Command**, **Blade-Ops Engineer30 E/Mitter (FD+20 or Parachutist)** and **ORC Feuerbach35/1.5** buy different reliability/roles. **Swiss Guard ML** is high-end hidden ARO, **Uhlan Feuerbach+Blitzen** a TAG priced separately. Cheap E/Mtter can disable on failed BTS Saves, but needs a winning FTF and the Engineer may restore function. [Cross-game anti-armor apex/value, E/M, K1 and AP+EXP tiers](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Squalos Mk-II MULTI MMR55/1** is outstanding affordable **3STR/TA quadrant-flip TAG**, compared with **Maximus TAG80/1** STR4 and **Swiss Guard44/0 Hidden/FD** that can delay/reveal as heavy physical guard but *not standard Supplies Specialist* absent Hacker/KHD profile. **Auxilia FO+Auxbot15/0** scores and defends by double-angle synchronized template on 1 Order, but Auxbot is not FO and no independent Order; **Auxilia FO+Deployable Repeater15/0** is a **different loadout**. **Peacemaker+Auxbot23/0** is an FD+20 physical wall. **NCA available Hexa KHD27/0** has Hidden/Mimetism(-6) and Specialist, excellent *pickup* but cannot keep marker while holding. **Opposing WIP12 NCA:** cheaper Auxilia/Peacemaker holds entry path more efficiently than 55–80pt TAG garrison if opponent goes around, leaving guns free to attack another zone.

[Cross-faction zone holding/carrier apex/value and actual transcript disagreements](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Authoritative roster/FT chart above governs profile legality.

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Aquila Guard52/1.5 MSV3 BS15** is the **apex direct** anti-Camo/Mimetism shooter: automatic successful Discover on eligible visible Camo and active-turn marker shot are distinct from Sensor. **Black Friar24/0 MSV2+Albedo(-6)** instead efficiently attacks opposing MSV/Marksmanship; its **Biometric 27/0** option answers Impersonation. **Blocker Sensor/Biometric** or **Pathfinder14 Sensor/FO** is much cheaper to *identify* a marker, including Sensor around total cover. **Counter:** 52pt Aquila can be blinded by White Noise; non-MSV Squalos/other guns and independent Sensor need to survive.

[Full N5.3 anti-tech apex/value, rules, matchups and transcript disagreements](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).
