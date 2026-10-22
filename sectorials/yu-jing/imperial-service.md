---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 202
sectorial_slug: imperial-service
sectorial_name: Imperial Service
parent_faction: Yu Jing
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Imperial Service roster, standard loadouts, canonical main Fireteam chart, reverse Fireteam index, and linked Daebak Force Reinforcement roster/Fireteam chart. Spec-Ops and Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# Imperial Service

## Overview and provenance

Repository-native reference for **Imperial Service (ISS)** roster, profiles, points/SWC, AVA, and Fireteam access.

Sources used:

- Army-derived Imperial Service source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `d4329bb596ffea5d568eb2435f74366c305a7630`.
- Army-derived linked Reinforcement force **Daebak Force** (`army_id: 299`) from the same pinned revision/commit.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **43-unit standard Imperial Service roster** and the complete ISS `fireteamChart` in the pinned Army source.
- Soldier of Fortune entries with empty faction lists are excluded from the base roster.
- `Guǐ Fēng Spec-Ops` and `Yu Jing Team-Ops` are optional game-mode content and are listed separately.
- Fireteam legality comes from the canonical chart in this file, not from an `FTO` loadout name by itself.
- Parenthetical Army-chart comments such as `(Celestial Guard)`, `(Hsien)`, `(Zhian)`, and `(Bounty Hunter)` are treated as **Counts-as / equivalence labels**.
- Linked Reinforcement section: **Daebak Force** (`army_id: 299`). Its distinct Reinforcement roster and Fireteam chart are recorded separately below; Main and Reinforcement troopers are not merged.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Imperial Service |
| Parent faction | Yu Jing |
| Army ID | 202 |
| Rules baseline | N5.3 |
| Main roster units | 43 |
| Linked Reinforcement roster | Daebak Force (Army ID 299) |
| Main Fireteam chart | yes |
| Reinforcement Fireteam chart | yes |

## Fireteam chart limits and sectorial-level restrictions

| Constraint | Value / wording |
|---|---|
| Core | raw source `1`: maximum 1 |
| Haris | raw source `2`: maximum 2 |
| Duo | raw source `256`: InfinityDB-normalized as unlimited |
| Kuang Shi | Fireteam is automatically Cancelled if the Celestial Guard Monitor leaves the Fireteam |
| Main/Reinforcement mixing | no source exception recorded; charts are kept separate |

## Roster index

| Unit | ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| Sun Tze | 143 | 1 | HI | Regular | — |
| Dragon Lords, Imperial Service Judges | 1868 | 1 | LI | Irregular | Celestial Guard max 1 |
| Imperial Vanguard Qiánfēng | 1871 | 2 | MI | Regular | — |
| Bayara Palace Guard | 1866 | 2 | LI | Regular | — |
| Kuang Shi | 146 | 8 | LI | Regular, Impetuous | KUANG SHI Core |
| Deva Functionaries | 109 | 3 | MI | Regular | ALEPH Support |
| Ninjas | 135 | 1 | SK | Regular | — |
| Major Lunah | 947 | 1 | LI | Regular | — |
| Lóngwáng | 1839 | 1 | TAG | Regular | Fast Attack Duo required-choice |
| Bào Troops | 166 | 5 | LI | Regular | Zhian required-choice; counts as Zhian |
| Kǎnrèn | 766 | 3 | SK | Regular | — |
| Koga Ninjas | 1867 | 2 | LI | Regular | — |
| Imperial Agents, Pheasant Rank | 148 | 3 | MI | Regular | Celestial Guard; Wu Míng; Zhian required-choice |
| Yáozăo | 161 | 2 | REM | Peripheral | — |
| Wú Míng | 129 | 5 | HI | Regular | Wú Míng native |
| Imperial Agents, Crane Rank | 151 | 3 | HI | Regular | Celestial Guard; Wú Míng; Zhian required-choice |
| Táowù | 1538 | 1 | LI | Regular | Celestial Guard max 1 |
| Miranda Ashcroft | 51 | 1 | LI | Regular | Zhian max 1; counts as Bounty Hunter |
| Sù-Jiàn | 155 | 3 | HI | Regular | Fast Attack Duo required-choice |
| Fēiquán | 1842 | 1 | VH | Regular | — |
| Hsien | 132 | 2 | HI | Regular | Zhian required-choice |
| Adil Mehmut, Crane Rank Armor | 1540 | 1 | HI | Regular | Wildcard max 1; counts as Crane Rank/Bounty Hunter |
| Xi Zhuang | 847 | 1 | LI | Regular | Wildcard max 1; counts as Celestial Guard/CSU |
| CSU | 122 | 2 | LI | Regular | Zhian required-choice |
| Wèibīng | 139 | 2 | REM | Regular | — |
| Son-Bae | 141 | 1 | REM | Regular | Wildcard max 1, FTO only |
| Hùsòng | 140 | 3 | REM | Regular | — |
| Kunai Solutions Ninjas | 1502 | 1 | SK | Regular | — |
| Authorized Bounty Hunters | 49 | 2 | LI | Regular | Zhian required-choice |
| Qíshì TAG Support Pilots | 1838 | 1 | LI | Regular | Celestial Guard max 1 |
| Rui Shi | 159 | 2 | REM | Regular | — |
| Lù Duān | 160 | 2 | REM | Regular | — |
| Shénjī Yíng | 1869 | 2 | MI | Regular | Wildcard max 2; counts as Hsien |
| Jìnwèi | 1870 | 3 | HI | Regular | Celestial Guard max 2; Zhian max 1 |
| Dikpala Tacbots | 1898 | 3 | REM | Regular | ALEPH Support required-choice |
| Chaīyì | 142 | 1 | REM | Regular | — |
| Pangguling | 162 | 2 | REM | Regular | Wildcard max 1, FTO only |
| Motorized Bounty Hunters | 1565 | 2 | LI | Irregular, Impetuous | Fast Attack Duo required-choice |
| Celestial Guard | 145 | 255 | LI | Regular | Celestial Guard native; Kuang Shi Monitor profile |
| Jīnyào Drop Unit | 1865 | 3 | REM | Regular | — |
| Warcors | 50 | 1 | LI | Irregular | — |
| Zhànyīng | 125 | 4 | LI | Regular | Wú Míng; Zhian required-choice |
| Father Lucien Sforza | 198 | 1 | MI | Regular | Zhian max 1, FTO only; counts as Bounty Hunter |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Guǐ Fēng Spec-Ops | 1914 | Spec-Ops | Celestial Guard max 1 when Spec-Ops mode is in use |
| Yu Jing Team-Ops | 1928 | Team-Ops | No ordinary ISS Fireteam row |

## Unit details

### Sun Tze

**ID 143 · AVA 1 · HI** — `MOV 15-5 | CC 16 | BS 12 | PH 12 | WIP 17 | ARM 4 | BTS 6 | W 2 | S 2`. ECM: Hacker (-3), BS Attack (+1B), Counterintelligence, Immunity (Enhanced), Mimetism (-3), Decoy (2), NWI, Strategos L2.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 3 | 53 | 0 | Vulkan Shotgun, Pulzar, Flash Pulse, Breaker Pistol, CCW; Lieutenant (+1 Command Token) | — |
| 4 | 53 | 0 | Thunderbolt, Light Shotgun, Pulzar, Breaker Pistol, CCW; Lieutenant (+1 Command Token) | — |
| 5 | 53 | 0 | Vulkan Shotgun, Pulzar, Flash Pulse, Breaker Pistol, CCW; Lieutenant (+1 Order) | — |

### Dragon Lords, Imperial Service Judges

**ID 1868 · AVA 1 · LI · Irregular** — `MOV 10-10 | CC 18 | BS 10 | PH 10 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Martial Arts L1, Specialist Operative, Stealth.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 5 | 0 | Nanopulser, Flash Pulse, Silenced Pistol, Monofilament CCW | Celestial Guard max 1 |

### Imperial Vanguard Qiánfēng

**ID 1871 · AVA 2 · MI** — `MOV 10-10 | CC 18 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 6 | W 1 | S 2`. BS Attack (+1B), Dodge (+2.5 cm), Mimetism (-3), Specialist Operative, Stealth, Terrain (Total), Religious Troop.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 25 | 0 | Boarding Shotgun, Heavy Flamethrower, D-Charges, Silenced Pistol, PARA CCW (-6); Parachutist | — |
| 2 | 24 | 0 | SMG, E/Marat, D-Charges, Silenced Pistol, PARA CCW (-6); KHD, Firewall (-3), Parachutist | — |
| 3 | 26 | 0 | SMG, E/Marat, D-Charges, Silenced Pistol, PARA CCW (-6); Hacking Device, Firewall (-3), Parachutist | — |
| 4 | 27 | 0 | Light Shotgun, E/M Carbine, D-Charges, Silenced Pistol, PARA CCW (-6); Surprise Attack (-3), Hidden Deployment, Infiltration | — |
| 5 | 28 | 0 | Boarding Shotgun, Heavy Flamethrower, D-Charges, Silenced Pistol, PARA CCW (-6); Surprise Attack (-3), Hidden Deployment, Infiltration | — |
| 6 | 26 | 0 | SMG, E/Marat, Flash Pulse, D-Charges, Silenced Pistol, PARA CCW (-6); Surprise Attack (-3), Hidden Deployment, Infiltration, Forward Observer | — |

### Bayara Palace Guard

**ID 1866 · AVA 2 · LI** — `MOV 10-10 | CC 22 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 4`. 360º Visor, Biometric Visor, MSV1, Discover (ReRoll), Guard, Religious Troop.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 18 | 0 | Light Shotgun, Heavy Flamethrower, Disco Baller, Kobra Pistol (PS 6), PARA CCW (-9) | — |
| 2 | 19 | 0 | Light Shotgun, Heavy Flamethrower, Shock Mine, Kobra Pistol, PARA CCW (-9); Minelayer | — |
| 3 | 20 | 0 | SMG, E/Marat, Shock Mine, Kobra Pistol, PARA CCW (-9); Minelayer | — |

### Kuang Shi

**ID 146 · AVA 8 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Impetuous, Dodge (+3), No Cover, Religious Troop, Explode.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 6 | 0 | Chain Rifle, Pistol, CCW | KUANG SHI Core |
| 2 | 8 | 0 | Boarding Shotgun, Pistol, CCW | KUANG SHI Core |

**Celestial Guard Monitor group** — `MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`; Dodge (+2.5 cm), Fireteam Master (Kuang Shi).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 13 | 0.5 | Combi Rifle, Smoke Grenade Launcher, Pistol, CCW | KUANG SHI Core; exactly 1 Monitor required |

A Kuang Shi Unit is one Monitor plus up to four Kuang Shi in the same Combat Group. The Fireteam is automatically Cancelled if the Monitor leaves it.

### Deva Functionaries

**ID 109 · AVA 3 · MI** — `MOV 10-10 | CC 15 | BS 12 | PH 11 | WIP 15 | ARM 2 | BTS 3 | W 1 | S 2`. Courage, Number 2, NWI, Immunity (Isolated).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 20 | 0 | Combi Rifle, Nanopulser, Pistol, CCW | ALEPH Support required-choice |
| 2 | 24 | 0 | Combi Rifle, Nanopulser, Pistol, CCW; Devabot | ALEPH Support required-choice |
| 3 | 22 | 0 | MULTI Rifle, Nanopulser, Pistol, CCW | ALEPH Support required-choice |
| 4 | 25 | 0.5 | Combi Rifle, Nanopulser, Pistol, CCW; Hacking Device | ALEPH Support required-choice |
| 5 | 20 | 0 | Boarding Shotgun, Pistol, CCW; Killer Hacking Device | ALEPH Support required-choice |
| 6 | 21 | 0 | Combi Rifle, Nanopulser, Pistol, CCW; Triangulated Fire, Sensor | ALEPH Support required-choice |
| 8 | 21 | 0 | Combi Rifle, Nanopulser, Flash Pulse, Pistol, CCW; Forward Observer | ALEPH Support required-choice |
| 9 | 29 | 1 | Spitfire, Nanopulser, Pistol, CCW; MSV2 | ALEPH Support required-choice |

**Devabot peripheral:** `MOV 15-10 | CC 13 | BS 10 | PH 10 | WIP 11 | ARM 0 | BTS 3 | W 1 | S 2`; Courage, Peripheral (Synchronized); Heavy Flamethrower, PARA CCW (-3).

### Ninjas

**ID 135 · AVA 1 · SK** — `MOV 10-10 | CC 23 | BS 11 | PH 12 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Martial Arts L3, Surprise Attack (-3), Camouflage, Courage, Hidden Deployment, Dodge (+2.5 cm), Infiltration, Mimetism (-6), Stealth, Terrain (Total), Climbing Plus.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 0 | Tactical Bow (+1SD), Shock Mine, Pistol, DA CCW (PS 6) | — |
| 4 | 27 | 0 | SMG, Pistol, DA CCW (PS 6) | — |
| 6 | 33 | 0.5 | SMG, Pistol, DA CCW (PS 6); Hacking Device | — |
| 7 | 26 | 0 | Tactical Bow (+1SD), Shock Mine, Pistol, DA CCW (PS 6); Killer Hacking Device | — |
| 9 | 30 | 0.5 | Boarding Shotgun, Flash Pulse, Pistol, DA CCW (PS 6); Forward Observer | — |

### Major Lunah

**ID 947 · AVA 1 · LI** — `MOV 10-10 | CC 16 | BS 13 | PH 10 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. MSV1, Triangulated Fire, Camouflage (1 Use), Immunity (Shock), Mimetism (-3), Stealth, Terrain (Total), Religious Troop, Surprise Attack (-3), BS Attack (SR-1).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 29 | 1.5 | Viral Sniper Rifle (+1SD), Boarding Pistol, CCW | — |

### Lóngwáng

**ID 1839 · AVA 1 · TAG** — `MOV 15-10 | CC 18 | BS 14 | PH 14 | WIP 13 | ARM 7 | BTS 6 | W 3 | S 6`. ECM: Guided (-6), Biometric Visor, Courage, Tactical Awareness; TAG remote-presence support rules from source.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 70 | 1.5 | AP HMG, Adhesive Launcher Rifle, Light Riotstopper (+1B), PARA CCW (-6); Shàngdiào ancillary | Fast Attack required-choice max 1 |
| 2 | 68 | 1 | Mk12, Adhesive Launcher Rifle, Light Riotstopper, PARA CCW (-6); BS Attack (+1B); Shàngdiào ancillary | Fast Attack required-choice max 1 |
| 3 | 72 | 1.5 | AP HMG, Adhesive Launcher Rifle, Light Riotstopper (+1B), PARA CCW (-6); NCO; Shàngdiào ancillary | Fast Attack required-choice max 1 |

**Shàngdiào ancillary:** `MOV 15-10 | PH 10 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 1`; Courage, Dodge (+3), Mimetism (-3), Specialist Operative, Peripheral (Ancillary).

### Bào Troops

**ID 166 · AVA 5 · LI** — `MOV 10-10 | CC 16 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 6 | W 1 | S 2`. Albedo (-3), Biometric Visor, MSV2, Discover (+3), Religious Troop.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 3 | 27 | 1.5 | MULTI Sniper Rifle, Flash Pulse, Pistol, CCW | Zhian required-choice max 3; counts as Zhian |
| 7 | 16 | 0 | Light Shotgun, Heavy Riotstopper, Flash Pulse, Pistol, CCW | Zhian required-choice max 3; counts as Zhian |
| 8 | 17 | 0 | SMG, Heavy Riotstopper, Flash Pulse, Pistol, CCW | Zhian required-choice max 3; counts as Zhian |
| 9 | 23 | 0 | Thunderbolt, Flash Pulse, Pistol, CCW; BS Attack (+1B) | Zhian required-choice max 3; counts as Zhian |

### Kǎnrèn

**ID 766 · AVA 3 · SK** — `MOV 10-10 | CC 18 | BS 13 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Surprise Attack (-3), Forward Deployment (+20), Dodge (+2.5 cm), Stealth, Terrain (Total), Mimetism (-6), Decoy (2).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 2 | 27 | 0 | Combi Rifle, D-Charges, Boarding Pistol, CCW; Killer Hacking Device | — |
| 3 | 25 | 0.5 | SMG, D-Charges, Boarding Pistol, CCW; Hacking Device, Cybermask upgrade | — |
| 4 | 26 | 0.5 | Boarding Shotgun (+1B), Shock Mine, Boarding Pistol, CCW; Minelayer | — |
| 5 | 22 | 0.5 | SMG, MadTraps, Boarding Pistol, CCW; Minelayer | — |
| 6 | 25 | 0 | Boarding Shotgun (+1B), Flash Pulse, Boarding Pistol, CCW; Forward Observer | — |

### Koga Ninjas

**ID 1867 · AVA 2 · LI** — `MOV 15-5 | CC 23 | BS 12 | PH 12 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Bangbomb (+4), Martial Arts L3, Surprise Attack (-3), Courage, Dodge (+2.5 cm), Mimetism (-3), Specialist Operative, Decoy (1), Stealth, Climbing Plus.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 27 | 0 | E/M Carbine (+1B), Pulzar, Tactical Bow, Pistol, E/M CCW (PS 6); Camouflage, Forward Deployment (+20) | — |
| 2 | 28 | 0.5 | E/M Carbine (+1B), Pulzar, E/M Mine, Pistol, E/M CCW (PS 6); Camouflage, Forward Deployment (+20), Minelayer | — |
| 3 | 30 | 0 | E/M Carbine (+1B), Pulzar, Pistol, E/M CCW (PS 6); KHD (Carbonite), Deployable Repeater, Camouflage, Forward Deployment (+20) | — |
| 4 | 28 | 0 | E/M Carbine (+1B), Contender, Tactical Bow, Pistol, E/M CCW (PS 6); Parachutist | — |
| 5 | 25 | 0 | E/M Carbine (+1B), Pulzar, E/M Mine, Pistol, E/M CCW (PS 6); Parachutist | — |

### Imperial Agents, Pheasant Rank

**ID 148 · AVA 3 · MI** — `MOV 10-10 | CC 17 | BS 12 | PH 11 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. Chain of Command, Strategic Deployment, Dodge (+2.5 cm), Immunity (Shock), Stealth.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 2 | 28 | 0.5 | Combi Rifle, E/Mitter, Breaker Pistol, PARA CCW (-6); Hacking Device | Celestial Guard max 1; Wú Míng max 1; Zhian required-choice max 3 |
| 3 | 26 | 0 | Combi Rifle, E/Mitter, Breaker Pistol, PARA CCW (-6); Killer Hacking Device | same |
| 4 | 27 | 0 | Combi Rifle, E/Mitter, Breaker Pistol, PARA CCW (-6); Doctor, MediKit | same |
| 5 | 23 | 0 | Boarding Shotgun, E/Mitter, MadTraps, Breaker Pistol, PARA CCW (-6); Minelayer | same |
| 6 | 28 | 1 | Red Fury, Breaker Pistol, PARA CCW (-6); Tactical Awareness | same |

### Yáozăo

**ID 161 · AVA 2 · REM · Peripheral** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Peripheral (Servant), Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | PARA CCW (-3); peripheral/no Order | — |

### Wú Míng

**ID 129 · AVA 5 · HI** — `MOV 10-10 | CC 17 | BS 13 | PH 12 | WIP 12 | ARM 4 | BTS 3 | W 2 | S 2`. Dodge (+2.5 cm).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 2 | 27 | 0 | MULTI Rifle, Grenade Launcher, E/M Grenade Launcher, Boarding Pistol, CCW | Wú Míng native |
| 3 | 22 | 0 | Boarding Shotgun, Boarding Pistol, CCW; TinBot Firewall (-6) | Wú Míng native |
| 4 | 33 | 1.5 | AP HMG, Boarding Pistol, CCW | Wú Míng native |
| 5 | 19 | 0 | AP SMG, E/Marat, Boarding Pistol, CCW | Wú Míng native |
| 6 | 23 | 1.5 | Heavy Rocket Launcher, E/M Carbine, Boarding Pistol, CCW | Wú Míng native |
| 9 | 22 | 0 | AP SMG, E/Mitter, Boarding Pistol, CCW | Wú Míng native |

### Imperial Agents, Crane Rank

**ID 151 · AVA 3 · HI** — `MOV 15-5 | CC 24 | BS 13 | PH 13 | WIP 14 | ARM 4 | BTS 6 | W 2 | S 2`. X Visor, Martial Arts L3, Courage, Dodge, Combat Instinct, Stealth.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 49 | 1.5 | AP HMG, Pulzar (+1B), MULTI Pistol, DA CCW (PS 5) | Celestial Guard max 1; Wú Míng max 1; Zhian required-choice max 3 |
| 2 | 47 | 1 | AP Spitfire, Pulzar (+1B), MULTI Pistol, DA CCW (PS 5) | same |
| 3 | 41 | 0 | MULTI Rifle, Pulzar (+1B), MULTI Pistol, DA CCW (PS 5); Triangulated Fire, Sensor | same |
| 4 | 45 | 0.5 | MULTI Rifle, Pulzar (+1B), MULTI Pistol, DA CCW (PS 5); Hacking Device | same |
| 5 | 49 | 1 | AP HMG, Pulzar (+1B), MULTI Pistol, DA CCW (PS 5); Lieutenant | same |
| 6 | 47 | 0 | AP Spitfire, Pulzar (+1B), MULTI Pistol, DA CCW (PS 5); Lieutenant | same |
| 7 | 41 | +1.5 | MULTI Rifle, Pulzar (+1B), MULTI Pistol, DA CCW (PS 5); Lieutenant, Triangulated Fire, Sensor | same |

### Táowù

**ID 1538 · AVA 1 · LI** — `MOV 10-10 | CC 19 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Holomask, BS Attack (+1B), Counterintelligence, Dodge (+3), Natural Born Warrior, Immunity (Shock), Specialist Operative, Stealth.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Light Shotgun, E/Marat, Flash Pulse, Viral Pistol, PARA CCW (-9) | Celestial Guard max 1 |
| 2 | 16 | 0 | Contender, Pulzar, Flash Pulse, Viral Pistol, PARA CCW (-9) | Celestial Guard max 1 |
| 3 | 21 | 0.5 | Contender, Pulzar, Flash Pulse, Viral Pistol, PARA CCW (-9); Chain of Command | Celestial Guard max 1 |

### Miranda Ashcroft

**ID 51 · AVA 1 · LI** — `MOV 10-10 | CC 19 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. CC Attack (-6), Mimetism (-6), Specialist Operative, Marksmanship, Stealth.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 27 | 0 | MULTI Rifle, PARA Mine, Boarding Pistol, Monofilament CCW | Zhian max 1; counts as Bounty Hunter |
| 2 | 25 | 0 | Boarding Shotgun, PARA Mine, Boarding Pistol, Monofilament CCW | same |
| 3 | 28 | 0 | Combi Rifle, E/Mitter (+1B), PARA Mine, Boarding Pistol, Monofilament CCW | same |

### Sù-Jiàn

**ID 155 · AVA 3 · HI** — two Transmutation forms.

**High Mobility Form:** `MOV 20-5 | CC 9 | BS 12 | PH 14 | WIP 13 | ARM 5 | BTS 6 | W 2 | S 3`. Courage, Dodge (+5), NWI, Terrain (Total), Climbing Plus, Remote Presence, Transmutation.

**Combat Form:** `MOV 10-10 | CC 17 | BS 14 | PH 14 | WIP 13 | ARM 5 | BTS 6 | W 2 | S 5`. Courage, NWI, Remote Presence, Transmutation, BS Attack (SR-1).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 554 | 50 | 1.5 | Spitfire, Light Flamethrower, Panzerfaust, Heavy Pistol, CCW | Fast Attack required-choice max 2 |
| 2674 | 46 | 0 | Heavy Shotgun (+1B), Light Flamethrower (+1B), Thunderbolt, Heavy Pistol, CCW | Fast Attack required-choice max 2 |

### Fēiquán

**ID 1842 · AVA 1 · VH** — `MOV 20-5 | CC — | BS 13 | PH 12 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 7`. Aerial, Courage, Mimetism (-6), No Cover, Sensor, Super-Jump (Jet Propulsion), Terrain (Total), Tech-recovery, GizmoKit interaction from source.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 28 | 0 | E/M Carbine (+1B), Flash Pulse, Akrylat-Kanone, Pitcher; BS Attack (+1SD) | — |
| 2 | 27 | 0 | MULTI Rifle (+1B), Akrylat-Kanone, Blitzen; X Visor | — |

### Hsien

**ID 132 · AVA 2 · HI** — `MOV 15-5 | CC 21 | BS 14 | PH 14 | WIP 14 | ARM 4 | BTS 6 | W 2 | S 2`. MSV2, Martial Arts L1, Courage, Dodge (+2.5 cm).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 20 | 47 | 0 | MULTI Marksman Rifle, Nanopulser (+1B), Pistol, DA CCW (PS 6); TinBot Firewall (-6) | Zhian required-choice max 2 |
| 30 | 49 | 1.5 | HMG, Nanopulser (+1B), Pistol, DA CCW (PS 6) | same |
| 40 | 44 | +1 | MULTI Rifle, Nanopulser (+1B), Pistol, DA CCW (PS 6); Specialist Operative | same |
| 50 | 47 | +1 | MULTI Marksman Rifle, Nanopulser (+1B), Pistol, DA CCW (PS 6); Lieutenant | same |
| 700 | 49 | 1 | HMG, Nanopulser (+1B), Pistol, DA CCW (PS 6); Lieutenant | same |
| 701 | 51 | +1 | MULTI Marksman Rifle, Nanopulser (+1B), Pistol, DA CCW (PS 6); Lieutenant (+1 Order) | same |
| 702 | 48 | +1 | MULTI Rifle, Nanopulser (+1B), Pistol, DA CCW (PS 6); Lieutenant (+1 Order), Specialist Operative | same |

### Adil Mehmut, Crane Rank Armor

**ID 1540 · AVA 1 · HI** — `MOV 15-5 | CC 23 | BS 13 | PH 13 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 2`. Deactivator, X Visor, Martial Arts L3, BS Attack (Continuous Damage), Courage, Dodge (+5), Warhorse, Number 2, Specialist Operative, Sensor, Stealth.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 49 | 1.5 | AP Spitfire, Nanopulser, Disco Baller, Heavy Pistol, Monofilament CCW, PARA CCW (-6) | Wildcard max 1; counts as Crane Rank/Bounty Hunter |
| 2 | 49 | 1.5 | Same; Lieutenant | same |

### Xi Zhuang

**ID 847 · AVA 1 · LI** — `MOV 10-10 | CC 16 | BS 12 | PH 10 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. Dodge (+2.5 cm), Immunity (Shock), Number 2, Forward Observer, Discover (ReRoll).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | SMG, Flash Pulse, MadTraps, Disco Baller, Heavy Pistol, PARA CCW (-6); BS Attack (+1B) | Wildcard max 1; counts as Celestial Guard/CSU |
| 2 | 21 | 0 | Combi Rifle, Light Flamethrower (+1B), Flash Pulse, MadTraps, Heavy Pistol, PARA CCW (-6); Minelayer | same |

### CSU

**ID 122 · AVA 2 · LI** — `MOV 10-10 | CC 16 | BS 12 | PH 10 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 2`. MetaChemistry, Sixth Sense.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 10 | 0 | Breaker Rifle, Nanopulser (+1B), MULTI Pistol, PARA CCW (-6) | Zhian required-choice max 2 |
| 2 | 11 | 0 | Combi Rifle, Nanopulser (+1B), MULTI Pistol, PARA CCW (-6) | same |
| 3 | 11 | 0 | Boarding Shotgun, Adhesive Launcher Rifle (+1B), MULTI Pistol, PARA CCW (-6) | same |
| 4 | 11 | 0 | Rifle, Light Shotgun, Nanopulser (+1B), MULTI Pistol, PARA CCW (-6); Specialist Operative | same |
| 5 | 13 | 0 | Breaker Combi Rifle, Nanopulser (+1B), MULTI Pistol, PARA CCW (-6); Specialist Operative | same |

### Wèibīng

**ID 139 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Deactivator, Repeater, Remote Presence, Courage, Triangulated Fire, Forward Observer, Sensor.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3) | — |
| 2 | 17 | 0 | Same; Tactical Awareness | — |

### Son-Bae

**ID 141 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CCW (-3); BS Attack (Guided) | — |
| 2 | 19 | 1.5 | **Yáokòng SON-BAE FTO**; Missile Launcher (+1B), PARA CCW (-3) | Wildcard max 1 |

### Hùsòng

**ID 140 · AVA 3 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. 360º Visor, Remote Presence, Courage, Total Reaction.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 1 | HMG, PARA CCW (-3) | — |
| 2 | 18 | 0 | Thunderbolt (+1B), PARA CCW (-3) | — |

### Kunai Solutions Ninjas

**ID 1502 · AVA 1 · SK** — `MOV 10-10 | CC 21 | BS 12 | PH 12 | WIP 12 | ARM 1 | BTS 0 | W 1 | S 2`. Martial Arts L3, Surprise Attack (-3), Camouflage, Courage, Hidden Deployment, Dodge (+2.5 cm), Mimetism (-6), Terrain (Total), Climbing Plus, Stealth.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 28 | 1.5 | MULTI Sniper Rifle, Pistol, Shock CCW (PS 6) | — |
| 2 | 26 | 0 | Shock Marksman Rifle, Pistol, Shock CCW (PS 6); BS Attack (AP) | — |
| 3 | 25 | 0.5 | Thunderbolt, PARA Mine, Pistol, Shock CCW (PS 6); BS Attack (T2) | — |

### Authorized Bounty Hunters

**ID 49 · AVA 2 · LI** — `MOV 10-10 | CC 16 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Booty (ReRoll), Stealth.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 2 | 12 | 0 | Boarding Shotgun, Heavy Riotstopper, Pistol, PARA CCW (-6) | Zhian required-choice max 2 |
| 3 | 19 | 0.5 | Sniper Rifle, Breaker Pistol (+1B), PARA CCW (-6) | same |
| 4 | 21 | 1 | Spitfire, Boarding Pistol, PARA CCW (-6) | same |
| 5 | 12 | 0 | SMG, Akrylat-Kanone, Breaker Pistol, PARA CCW (-6) | same |

### Qíshì TAG Support Pilots

**ID 1838 · AVA 1 · LI** — `MOV 10-10 | CC 21 | BS 11 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`. Courage, Specialist Operative, Stealth, TAGCom.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 3 | 10 | 0 | **LÓNGWÁNG PILOT**; Adhesive Launcher Rifle, Assault Pistol, PARA CCW (-6); GizmoKit, CC Attack (+3) | Celestial Guard max 1 |

### Rui Shi

**ID 159 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 4`. Repeater, Remote Presence, Courage.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 1 | Spitfire, PARA CCW (-3); MSV2 | — |
| 2 | 21 | 0.5 | Red Fury, Mine Dispenser (Shock), PARA CCW (-3); MSV1 | — |

### Lù Duān

**ID 160 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 4`. Holoprojector, MSV1, Remote Presence, Surprise Attack (-3), Courage, BS Attack (+1B).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 0 | Mk12, Heavy Flamethrower, E/M Mine, PARA CCW (-3) | — |
| 2 | 20 | 0 | Thunderbolt, E/M Carbine, E/M Mine, PARA CCW (-3) | — |

### Shénjī Yíng

**ID 1869 · AVA 2 · MI** — `MOV 10-10 | CC 16 | BS 12 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Deactivator, GizmoKit, Engineer (WIP 14).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 18 | 0 | Combi Rifle, Akrylat-Kanone, D-Charges (PS 5), Pistol, PARA CCW (-3) | Wildcard max 2; counts as Hsien |
| 2 | 19 | 0 | Thunderbolt (AP), Light Shotgun, D-Charges (PS 5), Pistol, PARA CCW (-3) | same |
| 3 | 20 | 0 | Same as 2; Deployable Cover | same |
| 4 | 21 | 0 | Combi Rifle, Akrylat-Kanone, D-Charges (PS 5), Armed Turret (E/Mitter), Pistol, PARA CCW (-3) | same |
| 5 | 21 | 0 | Combi Rifle, Akrylat-Kanone, D-Charges (PS 5), Armed Turret (Adhesive Launcher Rifle +1B), Pistol, PARA CCW (-3) | same |

### Jìnwèi

**ID 1870 · AVA 3 · HI** — `MOV 10-10 | CC 18 | BS 12 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 2 | S 2`. BS Attack (+1B), Immunity (BTS), Sensor, Sixth Sense, Religious Troop, Remote Presence.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 18 | 0 | Adhesive Launcher Rifle, Heavy Riotstopper, Heavy Pistol, PARA CCW (-3) | Celestial Guard max 2; counts as Celestial Guard; Zhian max 1, counts as Hsien |
| 2 | 19 | 0 | Same + Akrylat-Kanone | same |
| 3 | 19 | 0 | Adhesive Launcher Rifle, Heavy Riotstopper, Heavy Pistol, PARA CCW (-3); TinBot Firewall (-3) | same |
| 4 | 23 | 0 | E/Mitter, Heavy Riotstopper, Heavy Pistol, PARA CCW (-3); Triangulated Fire | same |

### Dikpala Tacbots

**ID 1898 · AVA 3 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`. ECM: Hacker (-3), Remote Presence, Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 13 | 0 | Combi Rifle, PARA CCW (-3) | ALEPH Support required-choice max 3 |
| 2 | 21 | 1 | HMG, PARA CCW (-3) | same |
| 3 | 19 | 1 | MULTI Sniper Rifle, PARA CCW (-3) | same |
| 5 | 13 | 0 | SMG, Akrylat-Kanone, PARA CCW (-3); Repeater | same |
| 6 | 15 | 0 | Combi Rifle, PARA CCW (-3); MediKit, Paramedic | same |

### Chaīyì

**ID 142 · AVA 1 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Remote Presence, Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) | — |

### Pangguling

**ID 162 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 4`. Baggage, Remote Presence, Courage.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | PARA CCW (-3); Deactivator, Repeater | — |
| 2 | 14 | 0.5 | PARA CCW (-3); EVO Hacking Device | — |
| 3 | 17 | 0 | Combi Rifle, PARA CCW (-3); Repeater, Total Reaction | — |
| 4 | 12 | 0 | **PANGGULING FTO**; Light Shotgun, PARA CCW (-3); Repeater | Wildcard max 1 |

### Motorized Bounty Hunters

**ID 1565 · AVA 2 · LI · Irregular, Impetuous** — `MOV 20-15 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Motorcycle, Booty (ReRoll), Limited Cover, Dodge (+5), Mimetism (-3).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | Boarding Shotgun, Heavy Riotstopper, Pistol, PARA CCW (-6) | Fast Attack required-choice max 2 |
| 2 | 9 | 0 | SMG, Chain-colt (+1B), Pistol, PARA CCW (-6) | same |
| 3 | 16 | 0.5 | Red Fury, Breaker Pistol, PARA CCW (-6) | same |

### Celestial Guard

**ID 145 · AVA 255 · LI** — `MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Dodge (+2.5 cm).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 13 | 0 | Combi Rifle, Light Riotstopper, Pistol, CCW | Celestial Guard native |
| 8 | 14 | 0.5 | SMG, Light Riotstopper, Pistol, CCW; Hacking Device | Celestial Guard native |
| 9 | 14 | 0 | Combi Rifle, Light Riotstopper, Flash Pulse, Pistol, CCW; Forward Observer | Celestial Guard native |
| 10 | 13 | 0 | Combi Rifle, Light Riotstopper, Pistol, CCW; Lieutenant | Celestial Guard native |
| 12 | 15 | 0 | Combi Rifle, Light Riotstopper, Pistol, CCW; Commlink (+1), Specialist Operative | Celestial Guard native |
| 13 | 13 | 0.5 | Combi Rifle, Smoke Grenade Launcher, Pistol, CCW | Celestial Guard native |
| 14 | 17 | 0 | MULTI Marksman Rifle, Pistol, CCW | Celestial Guard native |

The separate **Monitor** profile used by the Kuang Shi Unit/Fireteam is recorded under Kuang Shi above.

### Jīnyào Drop Unit

**ID 1865 · AVA 3 · REM** — `MOV 15-5 | CC 12 | BS 12 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Albedo (-3), Remote Presence, Courage, Parachutist, Combat Jump (PH 13), Super-Jump (Jet Propulsion).

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 17 | 0 | Boarding Shotgun, Heavy Riotstopper, PARA Mine, PARA CCW (-3) | — |
| 2 | 24 | 1 | Red Fury, Heavy Riotstopper, PARA CCW (-3) | — |
| 3 | 18 | 0 | SMG, Adhesive Launcher Rifle, Heavy Riotstopper, PARA CCW (-3); Deployable Repeater | — |
| 4 | 19 | 0 | Same; MediKit, Paramedic | — |

### Warcors

**ID 50 · AVA 1 · LI · Irregular** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Journalist.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor | — |
| 2 | 3 | 0 | Same; Sixth Sense | — |

### Zhànyīng

**ID 125 · AVA 4 · LI** — `MOV 10-10 | CC 18 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 2`. Dodge (+2.5 cm), Immunity (BTS), Sixth Sense.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 1 | HMG, Boarding Pistol, PARA CCW (-6) | Wú Míng max 3; counts as Wu Míng; Zhian required-choice max 3, counts as Zhian |
| 2 | 23 | 1.5 | Missile Launcher, Boarding Pistol, PARA CCW (-6) | same |
| 3 | 24 | 0.5 | Breaker Combi Rifle, Pitcher, D-Charges, Boarding Pistol, PARA CCW (-6); Hacking Device (Zero Pain) | same |
| 4 | 20 | 0 | Breaker Combi Rifle, D-Charges, Flash Pulse, Boarding Pistol, PARA CCW (-6); Forward Observer | same |
| 7 | 23 | 0 | Breaker Combi Rifle, MadTraps, Boarding Pistol, PARA CCW (-6); Triangulated Fire, Minelayer, Sensor | same |
| 9 | 23 | 0 | Same weapons; Lieutenant, Triangulated Fire, Minelayer, Sensor | same |

### Father Lucien Sforza

**ID 198 · AVA 1 · MI** — `MOV 10-10 | CC 19 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. X Visor, BS Attack (+1SD), Immunity (ARM), Combat Instinct, Stealth, NCO, Dogged, Religious Troop.

| Opt | Pts | SWC | Loadout | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 0 | Viral Rifle, Adhesive Launcher Rifle, Nanopulser, Heavy Pistol, PARA CCW (-9); Holoprojector, Surprise Attack (-3), Forward Deployment (+10) | — |
| 2 | 23 | 0 | **SFORZA FTO**; same weapons | Zhian max 1; counts as Bounty Hunter |
| 3 | 26 | 0 | **SFORZA FTO**; same weapons; Albedo (-6) | Zhian max 1; counts as Bounty Hunter |

## Optional-mode unit details

### Guǐ Fēng Spec-Ops

**ID 1914 · optional Spec-Ops mode.** The Army document exposes both initial and enhanced Spec-Ops profile states. Its Fireteam chart row is `GUǏ FĒNG (Spec-Ops)`, max 1 in Celestial Guard Fireteams.

Standard option IDs in the pinned source: `2, 3, 4, 5, 6, 7`. Do not treat Guǐ Fēng as ordinary matched-play roster content unless Spec-Ops mode is active.

### Yu Jing Team-Ops

**ID 1928 · optional Team-Ops mode.** No ordinary Imperial Service Fireteam chart row.

## Fireteams

This section is **canonical**. The Unit → Fireteam index below is derivative.

### Chart limits

| Type | Raw source | Meaning |
|---|---:|---|
| Core | 1 | Maximum 1 |
| Haris | 2 | Maximum 2 |
| Duo | 256 | InfinityDB-normalized meaning: unlimited |

### FT-01 — Celestial Guard Fireteams

**Types:** Core, Haris

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction | Allowed loadout IDs |
|---|---:|---:|---:|---|---|---|---|
| Celestial Guard | 145 | 1 | 5 | No | — | — | all standard CG profiles |
| Jìnwèi | 1870 | 0 | 2 | No | Celestial Guard | — | all |
| Crane Agent | 151 | 0 | 1 | No | — | — | all |
| Pheasant Imperial Agent | 148 | 0 | 1 | No | — | — | all |
| Qíshì | 1838 | 0 | 1 | No | — | — | all available ISS profile |
| Dragon Lord | 1868 | 0 | 1 | No | — | — | all |
| Táowù | 1538 | 0 | 1 | No | — | — | all |
| Guǐ Fēng | 1914 | 0 | 1 | No | Spec-Ops | Spec-Ops mode | Spec-Ops options only |

At least one Celestial Guard is required by explicit `min: 1`.

### FT-02 — Kuang Shi Fireteam

**Type:** Core  
**Observation:** “The Fireteam is automatically Cancelled if the Celestial Guard Monitor leaves the Fireteam.”

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction | Allowed loadout IDs |
|---|---:|---:|---:|---|---|---|---|
| Kuang Shi | 146 | 2 | 4 | No | — | — | Kuang Shi 1, 2 |
| Celestial Guard Monitor | 146 | 1 | 1 | No | Kuang Shi | Monitor | Monitor 1 |

### FT-03 — ALEPH Support Fireteams

**Types:** Duo, Haris

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction | Allowed loadout IDs |
|---|---:|---:|---:|---|---|---|---|
| Dikpala | 1898 | 0 | 3 | Yes | — | — | all |
| Deva | 109 | 0 | 3 | Yes | Dikpala | — | all |

The `required: true` rows form the required-choice set recorded by the source projection: a legal team needs an eligible required-choice member; it does not require both unit types simultaneously.

### FT-04 — Wu Míng Fireteams

**Types:** Duo, Haris, Core

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction | Allowed loadout IDs |
|---|---:|---:|---:|---|---|---|---|
| Wú Míng | 129 | 1 | 5 | No | — | — | all |
| Zhànyīng | 125 | 0 | 3 | No | Wu Míng | — | all |
| Pheasant Imperial Agent | 148 | 0 | 1 | No | — | — | all |
| Crane Agent | 151 | 0 | 1 | No | — | — | all |

At least one Wú Míng is required by explicit `min: 1`.

### FT-05 — Zhian (Law&Order) Fireteams

**Types:** Duo, Haris

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction | Allowed loadout IDs |
|---|---:|---:|---:|---|---|---|---|
| Bào Troop | 166 | 0 | 3 | Yes | Zhian | — | all |
| Pheasant Imperial Agent | 148 | 0 | 3 | Yes | Zhian | — | all |
| Crane Agent | 151 | 0 | 3 | Yes | Zhian | — | all |
| Bounty Hunter | 49 | 0 | 2 | Yes | — | — | all |
| Zhànyīng | 125 | 0 | 3 | Yes | Zhian | — | all |
| CSU | 122 | 0 | 2 | Yes | — | — | all |
| Hsien | 132 | 0 | 2 | Yes | — | — | all |
| Jìnwèi | 1870 | 0 | 1 | No | Hsien | — | all |
| Sforza | 198 | 0 | 1 | No | Bounty Hunter | FTO | 2, 3 |
| Miranda Ashcroft | 51 | 0 | 1 | No | Bounty Hunter | — | all |

The `required: true` rows form the source required-choice set. Jìnwèi, Sforza, and Miranda are optional additions and do not by themselves satisfy that required-choice set.

### FT-06 — Fast Attack Fireteams

**Type:** Duo

| Member | Unit ID | Min | Max | Required choice | Counts as | FTO restriction | Allowed loadout IDs |
|---|---:|---:|---:|---|---|---|---|
| Sù-Jiàn | 155 | 0 | 2 | Yes | — | — | all |
| Motorized Bounty Hunter | 1565 | 0 | 2 | Yes | — | — | all |
| Lóngwáng | 1839 | 0 | 1 | Yes | — | — | all |

All three rows are in the source required-choice set; a legal Duo needs eligible required-choice members from this set.

### Wildcards

All rows below are in the chart's **Wildcards** row. Parenthetical values are Counts-as/equivalence labels.

| Wildcard | Unit ID | Max | Counts as | FTO restriction | Allowed loadout IDs |
|---|---:|---:|---|---|---|
| Shénjī | 1869 | 2 | Hsien | — | all |
| Xi Zhuang | 847 | 1 | Celestial Guard, CSU | — | all |
| Adil Mehmut | 1540 | 1 | Imperial Agent Crane Rank, Bounty Hunter | — | all |
| Son-Bae Yáokòng | 141 | 1 | — | FTO | 2 |
| Pangguling | 162 | 1 | — | FTO | 4 |

Wildcard status does not remove a Fireteam's native minimum/required-choice conditions.

## Unit → Fireteam access index

| Unit | Access |
|---|---|
| Sun Tze | — |
| Dragon Lords | Celestial Guard Core/Haris max 1 |
| Qiánfēng | — |
| Bayara Palace Guard | — |
| Kuang Shi | Kuang Shi Core, 2–4 plus exactly one Monitor |
| Deva | ALEPH Support Duo/Haris required-choice; counts as Dikpala |
| Ninja | — |
| Major Lunah | — |
| Lóngwáng | Fast Attack Duo required-choice max 1 |
| Bào | Zhian Duo/Haris required-choice max 3; counts as Zhian |
| Kǎnrèn | — |
| Koga Ninja | — |
| Pheasant Agent | Celestial Guard max 1; Wú Míng max 1; Zhian required-choice max 3, counts as Zhian there |
| Yáozăo | — |
| Wú Míng | Wú Míng Duo/Haris/Core native, min 1/max 5 |
| Crane Agent | Celestial Guard max 1; Wú Míng max 1; Zhian required-choice max 3, counts as Zhian there |
| Táowù | Celestial Guard max 1 |
| Miranda Ashcroft | Zhian max 1; counts as Bounty Hunter |
| Sù-Jiàn | Fast Attack Duo required-choice max 2 |
| Fēiquán | — |
| Hsien | Zhian required-choice max 2 |
| Adil Mehmut | Wildcard max 1; counts as Crane Rank/Bounty Hunter |
| Xi Zhuang | Wildcard max 1; counts as Celestial Guard/CSU |
| CSU | Zhian required-choice max 2 |
| Wèibīng | — |
| Son-Bae | Wildcard max 1, option 2 FTO only |
| Hùsòng | — |
| Kunai Ninja | — |
| Authorized Bounty Hunter | Zhian required-choice max 2 |
| Qíshì | Celestial Guard max 1 |
| Rui Shi | — |
| Lù Duān | — |
| Shénjī | Wildcard max 2; counts as Hsien |
| Jìnwèi | Celestial Guard max 2, counts as Celestial Guard; Zhian max 1, counts as Hsien |
| Dikpala | ALEPH Support Duo/Haris required-choice max 3 |
| Chaīyì | — |
| Pangguling | Wildcard max 1, option 4 FTO only |
| Motorized Bounty Hunter | Fast Attack Duo required-choice max 2 |
| Celestial Guard | Celestial Guard Core/Haris native, min 1/max 5; Monitor profile in Kuang Shi Core |
| Jīnyào | — |
| Warcor | — |
| Zhànyīng | Wú Míng max 3, counts as Wu Míng; Zhian required-choice max 3, counts as Zhian |
| Sforza | Zhian max 1, options 2/3 FTO only; counts as Bounty Hunter |
| Guǐ Fēng Spec-Ops | Celestial Guard max 1 when Spec-Ops mode is active |
| Yu Jing Team-Ops | — in ordinary ISS chart |

## Reinforcements — Daebak Force

Linked Army ID: **299**. The pinned Daebak document has a distinct Reinforcement roster and Fireteam chart. It is not merged into the main ISS chart.

### Reinforcement roster membership

| Unit | ID | AVA | Type |
|---|---:|---:|---|
| Reinf. Yáozăo | 1709 | 2 | REM |
| Reinf. Hwarang Corps | 1711 | 4 | HI |
| Reinf. Sulsa Warriors | 1712 | 2 | SK |
| Reinf. Yáoxiè Rui Shi | 1718 | 1 | REM |
| Reinf. Chief Mech-Engineer Chung-Hee Jeong | 1708 | 1 | LI |
| Reinf. Dokkaebi Cyberteam | 1715 | 2 | HI |
| Reinf. Son-Bae Yáokòng | 1717 | 1 | REM |
| Reinf. Naval Operations Group Sulyong | 1714 | 2 | MI |
| Reinf. Bìxié, the Jade Champion | 1719 | 1 | HI |
| Reinf. Jujak Regiment | 1707 | 3 | HI |
| Reinf. Wèibīng Yáokòng | 1716 | 2 | REM |
| Reinf. Sergeant So-ra Kwon | 1710 | 1 | HI |
| Reinf. Haetae Unit | 1713 | 1 | HI |

### Reinforcement Fireteam chart limits

The Daebak source `spec` block records `CORE: 0`, `HARIS: 0`, `DUO: 0`; the named Reinforcement Fireteam rows below define the available formations.

### RF-01 — Jujaks Reinforcement Fireteams

**Types:** Duo, Haris, Core

| Member | Unit ID | Min | Max | Counts as | Restriction |
|---|---:|---:|---:|---|---|
| Jujak REF. | 1707 | 1 | 3 | — | native minimum 1 |
| Hwarang REF. | 1711 | 0 | 1 | — | — |

### RF-02 — Hwarang Reinforcement Fireteams

**Types:** Duo, Haris, Core

| Member | Unit ID | Min | Max | Counts as | Restriction |
|---|---:|---:|---:|---|---|
| Hwarang REF. | 1711 | 1 | 4 | — | native minimum 1 |
| Sulsa Warrior REF. | 1712 | 0 | 2 | Hwarang | — |
| Haetae REF. | 1713 | 0 | 1 | — | — |
| Bìxié REF. | 1719 | 0 | 1 | — | — |

### Reinforcement Wildcards

| Wildcard | Unit ID | Max | Counts as | FTO restriction |
|---|---:|---:|---|---|
| Sulyong REF. | 1714 | 2 | — | — |
| Wèibīng Yáokòng REF. | 1716 | 2 | — | — |
| Son-Bae Yáokòng REF. | 1717 | 1 | — | FTO; option 3 |
| Dokkaebi REF. | 1715 | 1 | — | — |
| Chief Jeong REF. | 1708 | 1 | — | — |
| So-ra Kwon REF. | 1710 | 1 | Jujaks | — |

### Reinforcement units without chart access

- Reinf. Yáozăo — servant peripheral; no Fireteam row.
- Reinf. Yáoxiè Rui Shi — no Fireteam row.

## Tactical tags

Derived analysis aids, not official characteristics.

| Unit | Tags |
|---|---|
| Sun Tze | Strategos Lieutenant, Counterintelligence, durable command piece |
| Celestial Guard | cheap orders, Lieutenant, hacker, FO, smoke, long-range gun, link anchor |
| Kuang Shi | cheap Impetuous orders, disposable attack/defense, dedicated Monitor Core |
| Dragon Lord | ultra-cheap irregular specialist, monofilament, Celestial Guard filler |
| Crane Agent | premium HI assault, sensor, hacker, Lieutenant, flexible link member |
| Pheasant Agent | Chain of Command, Strategic Deployment, hacker/KHD/Doctor, TacAware gunfighter |
| Hsien | MSV2 HI gunfighter, Lieutenant options, specialist option, Zhian anchor |
| Wú Míng | durable HI Core/Haris, AP HMG, HRL, E/M, TinBot |
| Zhànyīng | missile/HMG, hacker with Pitcher, FO, sensor/minelayer, Lieutenant, link glue |
| Jìnwèi | cheap durable HI, Sensor, Sixth Sense, Fireteam counts-as bridge |
| Shénjī | Engineer, deployable turrets/cover, Wildcard counts as Hsien |
| Sù-Jiàn | very fast durable attack piece, climbing mobility, Fast Attack Duo |
| Lóngwáng | TAG, TacAware, NCO option, E/M/adhesive control, Fast Attack Duo |
| Fēiquán | aerial Mimetism (-6), Sensor, Pitcher, E/M attack |
| Qiánfēng | airborne or hidden/infiltrating specialist/hacker, strong close-range attack |
| Koga Ninja | midfield/airborne E/M attack, KHD/repeater option |
| Kǎnrèn | forward-deployed Mimetism (-6), decoy, hacker/KHD, mines/MadTraps |
| Ninja | hidden-deployment infiltration, KHD/hacker/FO, strong CC |
| Jīnyào | airborne REM attack/specialist, deployable repeater option |
| Rui Shi | MSV attack REM, Repeater, mine-dispenser option |
| Lù Duān | Holoprojector attack REM, MSV1, E/M mines |
| Wèibīng | Sensor/FO Repeater, TacAware option |
| Pangguling | Baggage, EVO, Repeater, TR option, FTO Wildcard |
| Son-Bae | guided missile option; FTO Wildcard missile profile |
| Dikpala | Mimetism REM gun platform, repeater/paramedic options, ALEPH Support link |
| Deva | NWI specialist/gunfighter, HD/KHD, Sensor, MSV2 option, ALEPH Support link |
| Bào | MSV2/Albedo gunfighter, Riotstopper, Zhian link |
| Bayara | MSV1/Biometric Visor, Guard, Disco Baller/mines |
| Táowù | Holomask, Counterintelligence, specialist, CoC option |
| Xi Zhuang | FO, MadTraps, Disco Baller/flamethrower, Wildcard |
| Adil | premium CC/specialist/Sensor, Wildcard |
| Sforza | NCO, viral/adhesive attack, FTO Zhian member |

## Tactical research — Imperial Service N5 (2026-10-22)

> **Status:** Interpretive list-building notes, **not** Army data. Use the N5.3 roster, loadouts, and canonical Fireteam chart above for legal profiles and costs. Most dedicated faction commentary below dates to the March–May 2025 rework; the September 2026 Army snapshot in this file takes precedence where rules, costs, or equipment have changed. Podcast transcripts are automated and sometimes mishear unit names. Opinions are attributed rather than presented as universal rankings.

### Identity, list-building and priorities

**Thesis:** ISS wins through *interlocking complementary tools*, not a single mandatory death star: inexpensive Regular orders; smoke + MSV / Albedo; flexible Duo/Haris packages; credible mobile HI/TAGs; and an unusually wide supply of E/M, adhesive, PARA, mines, hacking and repeaters. Robert Shepherd's pre-play review is optimistic about breadth and warns that a list which merely crams in every gimmick can lose focus. Tactical Awareness's game-informed reviews show viable but very different ISS builds (Sun Tze/TAG, Hsien/bounty-hunter teams, or network-control packages), yet the hosts disagree on the faction's overall efficiency.

1. **Choose one primary attack plan and its answer to armour:** Hsien/Bào visibility control; Lóngwáng with repairs and orders; fast Sù-Jiàn; Wu Míng HI trading; or hidden/airborne E/M and hacking. A secondary attack vector prevents one counter or lost gun from ending the turn.
2. **Buy only the Kuang Shi you need.** A Monitor + two Kuang Shi is a compact, linked smoke/Core and three Regular-order package; more cheap bodies can fuel a costly threat, but using the sole Core for this denies a Wu Míng/Celestial alternative. Kuang Shi lost Dogged in N5: treat them as disposable trading pieces, not guaranteed survivors.
3. **Cheap hacking is unusually efficient.** The 14-point, WIP 14 Celestial Guard hacker (0.5 SWC) pairs well with Wèibīng, Rui Shi, Pangguling, Jīnyào deployable repeaters and Zhànyīng Pitchers. Consider a Jìnwèi for Firewall/Sensor and as tougher link glue. **An ordinary Celestial Guard Duo is *not* on the current chart:** use a legal Core/Haris, e.g. a third eligible member, or keep them separate.
4. **Solve Lieutenant safety explicitly.** Sun Tze's Strategos L2, Decoys, Counterintelligence and Lieutenant (+1 Order) option are excellent but cost 53 points; a cheap Celestial Guard LT preserves more attackers but is easier to identify/attack. Pheasant Chain of Command and Táowù's CoC option buy insurance at real opportunity cost.
5. **Use immobilization to gain tempo, not automatically a kill.** E/M, Adhesive, PARA and Carbonite can stop an advance or expose a target to follow-up AP/viral/normal damage. Opponents may Reset, engineer, or use recovery rules, so specify *who will finish the target* or whether a turn of denial already wins the mission.

### Fast unit decisions: why, counters and competing opinions

| Unit / package | Pick it because… | Reservations / alternative opinion |
|---|---|---|
| **Celestial Guard hacker + smoke** | WIP 14 hacker is cheap; smoke launcher enables MSV shooting and obscures movement; a small Haris can support a separate aggressive Duo. | Ordinary rifle/MMR Guards are less attractive than specialists; smoke is scarce. CG-only Duo is not legal under the chart. |
| **Kuang Shi + Monitor Core** | Cheap Regular orders and reliable linked Smoke Grenade Launcher help Hsien, Bào and approach paths. | Takes the sole Core; lost Dogged; full-size spam may crowd out quality specialists and second-wave attackers. |
| **Hsien / Bào Zhian team** | Hsien's MSV2 HI gun combines with smoke; Bào add MSV2, Albedo and strong Discover, pressing camo/visor-dependent opponents. Named bounty hunters/Miranda/Sforza create alternative utility and ranged threats. | Expensive if every member must fight; inspect the **required-choice**, counts-as and FTO restrictions. A flexible Zhian cannot become a Core merely by filling slots. |
| **Wu Míng + Pheasant / Crane / Zhànyīng** | A 19-point AP-SMG Wu Míng or TinBot body can anchor an affordable ARM 4/2-Wound HI team; AP HMG/HRL cover attack/ARO, while Pheasant CoC and Zhànyīng hacking/Pitcher supply mission tools. | A full HI Core ties up the only Core and can be slowed by hacking or E/M; multiple small teams and cheap orders may cover more missions. |
| **Koga Ninja** | Camouflage, forward-deployed E/M Minelayer or KHD + Carbonite/repeater create hidden anti-HI pressure; Parachutist options react to where the enemy leaves exposed targets. | Tactical Awareness's speakers disagree whether to use forward mine/KHD or off-table flanking; Koga costs more than simpler objective Ninjas and cannot solve everything with E/M. |
| **Qiánfēng** | BS 13, BS Attack (+1B), D-Charges and specialist status make hidden/infiltrating or Parachutist builds credible **kill-after-disable** pieces; KHD/HD versions add Firewall. | Some prefer Koga's camouflage/mines and deployment ambiguity; Parachutist Qiánfēng gives up the immediate midfield trap. |
| **Kǎnrèn / Ninja** | Kǎnrèn provides Decoy, forward deployment, mines/MadTraps, or cheap hacking; Ninja Hidden Deployment offers a true late objective reveal. | Less direct gunfighting than Qiánfēng and less broad E/M coverage than Koga; select for mission and deployment shell game. |
| **Jìnwèi** | Remote Presence, Sensor, Sixth Sense, optional Firewall and counts-as links produce tough, efficient hacking support and close defence. | ARM 2 and limited shooting mean it isn't a solo replacement for a heavy attack piece. |
| **Dragon Lord / Qíshì Pilot** | Cheap 5-point irregular Dragon Lord specialist fills a Celestial Guard team and offers a nanopulser/Flash Pulse; 10-point Qíshì similarly fills specialist/link requirements. | Robert doubts Dragon Lord will ever consistently reach/use Monofilament; Tactical Awareness enjoys its unlikely TAG-kill upside. Buy it for cheap utility, not an expected assassination. |
| **Bayara Palace Guard** | 360°/Biometric/MSV1, Minelayer or Disco Baller, and PARA/Guard make a good backfield anti-AD and camo/disruption sentinel. | Robert's early review called it underwhelming for cost and conspicuous S4; Tactical Awareness likes the mine/disco layering. Niche defensive role, not an automatic inclusion. |
| **Adil vs Crane** | Adil's Wildcard, specialist, Sensor, multispectral close-range attacks and melee are flexible. Crane supplies robust HI weapons/CC, Triangulated Fire/Sensor, hacker or LT SWC package. | Tactical Awareness questions paying for Crane when Adil can accomplish similar close-range jobs; Crane still earns a place when its **specific weapon, LT or Fireteam role** is needed. |
| **Deva / Dikpala ALEPH support** | Deva WIP15/Immune Isolated specialist, hacker, MSV2 Spitfire; Dikpala give cheap Mimetism(-3) HMG/MSR ARO and repeater/paramedic loadouts in Duo/Haris. | Opportunity cost: Deva competes against cheap native hackers; basic Dikpala are fragile. Verify a required Deva/Dikpala member and Wildcard conditions. |

### Vehicle, TAG, Remote Presence HI, and REMs

**Actual ISS category coverage:** **Lóngwáng** is the roster's TAG; **Fēiquán** is its vehicle (VH); **Sù-Jiàn** is a Remote Presence **HI, not a TAG/REM unit type**. Standard Yu Jing REMs and Jīnyào/Dikpala provide the rest. Shared profiles were also discussed in Vanilla Yu Jing and general N5 TAG/REM coverage; don't copy unavailable Vanilla tools (e.g. Blue Wolf) into ISS.

| Platform | Best employment and the “why” | Tradeoff / support |
|---|---|---|
| **Lóngwáng TAG** (68–72 pts; BS14 ARM7, W3, S6, Tactical Awareness) | Durable primary active-turn shooter with AP HMG for hard targets, Mk12 (+1B) for midrange volume, adhesive/riotstopper for suppression of threats, and a Shàngdiào *ancillary specialist* to work objectives while the TAG attacks. NCO AP HMG option benefits from spare LT-order access. Eligible for **Fast Attack Duo**, subject to its actual required-choice restrictions. | Needs a protected Engineer/repair path and a plan against enemy hackers, AP and melee. Mk12 lacks AP HMG's armour punch; nonlethal adhesive alone doesn't score the kill. **Older 2025 commentary described ordinary HMG + BS Attack(-3); do not apply that historical profile to this N5.3 roster**, which records AP HMG or Mk12 options. |
| **Fēiquán vehicle** (27–28 pts; Mimetism -6, Aerial, Sensor, Super-Jump) | E/M Carbine (+1B) + Pitcher + Akrylat-Kanone profile projects hacking and nonlethal anti-TAG pressure across difficult angles; the MULTI Rifle (+1B) alternative helps *finish* targets disabled by a teammate. | Large S7 body, **No Cover**, positional exposure and limited lethal finish on E/M loadout. Tactical Awareness values E/M control highly; other analysis argues it needs a second shooter because disabled TAGs may be repaired. Sensor + Tech-recovery and fast movement are utility, not invulnerability. |
| **Sù-Jiàn** (46-pt heavy shotgun or 50-pt Spitfire; HI) | High-Mobility Form's MOV 20-5/Climbing Plus gets unexpected flanks; Combat Form BS14/ARM5 with NWI and Remote Presence converts the angle into repeated short-range attacks. Heavy Shotgun (+1B) is efficient close assault; Spitfire supplies a longer lane. **Fast Attack Duo** can combine with Lóngwáng or Motorized Bounty Hunter when chart restrictions are satisfied. | Hacking/E/M exposure and transmutation positioning matter. It is an HI with Remote Presence, **not** a second TAG and not a normal support REM; if forced to cross open long fire lanes, TAG or Hsien may work better. |
| **Jīnyào airborne REM** (17–24 pts) | Parachutist/Combat Jump, Jet Propulsion and Albedo allow flank damage or a **deployable repeater** where a regular Pitcher cannot reach. 18-point adhesive/SMG + repeater is a powerful low-cost network extender; 19-point paramedic can complete objectives; Red Fury is a more committed gunfighter. | BS12 and single Structure make it a delivery/trade piece, not an independent main attack. Older podcast opinions range from near-automatic repeater choice to taking only one for a specific mission. |
| **Rui Shi / Lù Duān attack REMs** | Rui Shi 23-point MSV2 Spitfire converts smoke/visors into anti-camo attack and carries a Repeater; its 21-point Red Fury/Mine Dispenser trades MSV strength for deployable pressure. Lù Duān's Holoprojector, Mimetism-independent Surprise Attack(-3), +1B, E/M Mines and Mk12/flamethrower can force poor decisions in close lanes. | Fragile ARM1; poor unsupported AROs. Rui Shi's weapon/visor and Lù Duān's holoprojector are different jobs rather than an automatic winner. |
| **Dikpala / Wèibīng / Hùsòng / Son-Bae** | Dikpala linkable HMG/MSR (+ Mimetism-3) and 13-point repeater/akrylat option; Wèibīng is Sensor + FO + Repeater, optional Tactical Awareness; Hùsòng Total Reaction protects a lane; Son-Bae guided missile punishes previously Spotlighted targets. | Keep the network viable, and do not mistake *availability* of guided missiles for reliable Spotlight coverage. Hùsòng and MSR bots can be bypassed/flanked; Son-Bae FTO Wildcard is **loadout-limited**. |
| **Pangguling / Shénjī / Yáozăo** | 8-point Baggage Pangguling is a useful Regular-order/repeater/reload support; EVO, Total Reaction and 12-point FTO Wildcard versions each fill a distinct job. Shénjī Engineer (WIP14), turret/deployable cover and Counts-as Hsien Wildcard helps repair TAG/REM/VH plans while adding area denial. Yáozăo 3-point servant extends repair reach. | Regular Pangguling is not automatically a Wildcard: only **FTO option 4** is. The Shénjī is an Engineer, not free healing; place it where it survives and can reach damaged assets. |

**Practical combined-arms packages (illustrations, not ready-made legal lists):** (a) **Kuang Shi Monitor smoke Core → Hsien/MSV assault**, plus inexpensive hacker and repeater; (b) **Lóngwáng + Shénjī Engineer + Pangguling Baggage**, with a separate objective specialist; (c) **Jīnyào/Wèibīng repeater → Celestial/Zhànyīng hackers → Son-Bae guided** with a close-range Sù-Jiàn/Qiánfēng finisher; (d) **Fēiquán E/M → mobile lethal gun**, using the vehicle to disable or reveal—not to replace a main gun. Validate Fireteam composition and combat-group Orders against the tables above.

### Where reviewers genuinely disagree

- **Is ISS top-tier or merely versatile?** Shepherd's rework appraisal is broadly positive, even against Vanilla; Tactical Awareness hosts describe both strong combinations and awkward/overpriced pieces. Their game lists support **flexible but demanding** rather than an automatic power ranking.
- **E/M saturation vs lethal efficiency:** Dan (Tactical Awareness) leans into Fēiquán + Koga/Qiánfēng/Jīnyào immobilization; Shepherd emphasizes N5 recovery/Engineer counterplay and the need to finish an enemy. Both agree disruption can purchase time.
- **Forward trap vs reserve flank:** Some Tactical Awareness hosts favor Koga Minelayer/KHD on the table, others Qiánfēng/Koga Parachutists for reactions to enemy deployment; the choice follows mission and expected armour.
- **Bayara/Dragon Lord:** Early Shepherd coverage is sceptical of standalone return; Tactical Awareness emphasizes defensive mines/disco/Guard for Bayara and bargain utility for Dragon Lord. Neither requires expecting a reliable Monofilament assassination.
- **TAG-centered vs multi-HI/MSV:** Lóngwáng produces efficient BS14 ARM7 pressure with Tactical Awareness, but the same cost buys redundant specialists and mobile threats (Sù-Jiàn, Hsien/Wu Míng, infiltrators). Match the primary threat to lanes, hacking density, and objectives.
- **Deva/Crane vs cheaper alternatives:** Deva specialists or Crane weapons can be excellent *for their precise job*; if only a WIP14 hacker, cheap gun, or close assault is needed, Celestial Guard, Dikpala or Adil may free enough points for a second threat.

### Sources and transcript audit

**Full transcripts checked through connected YouTube/Podcast MCP unless otherwise specified.** Early rework sources are dated March–June **2025**, before the pinned **2026-09-03 N5.3** snapshot.

| Priority | Resource | Distinct value / evidence level |
|---|---|---|
| **Start here: faction overview** | [Robert Shepherd — Infinity N5 Faction Focus: Imperial Service (22 Mar 2025)](https://www.youtube.com/watch?v=Yskl69PVzWA) | **YouTube transcript reviewed**; already archived in this repository at [rules/Youtube factions/Imperial Service.txt](../../rules/Youtube%20factions/Imperial%20Service.txt). Broad unit-by-unit list building; author discloses this is **theory-first**, not extensive play experience. |
| **Start here: faction after games** | [Tactical Awareness — Imperial Service UPDATE (24 Mar 2025)](https://open.spotify.com/episode/0v98BsWGJMA6gbkNUQWja8) | **Podcast transcript reviewed.** New profiles, actual early games, opposing takes on Koga/Qiánfēng, Bayara, Jìnwèi, Jīnyào, Lóngwáng. |
| **Strongest list examples** | [Tactical Awareness — S3 Ep19 Imperial Service (12 May 2025)](https://open.spotify.com/episode/0nIc1Ub4zoXpKxb1PyTJl3) | **Podcast transcript reviewed.** Three opposing build philosophies, Hsien/Bounty Hunters, Sun Tze/Lóngwáng, Fēiquán E/M, Jīnyào repeaters; hosts dispute individual efficiency. |
| **Cross-faction TAG/VH context** | [Tactical Awareness — S3 Ep22 Prime Yu Jing (3 Jun 2025)](https://open.spotify.com/episode/6SExmNQGYYnzbf8vsodN0A) | **Podcast transcript reviewed.** Shared Lóngwáng/Fēiquán TAG+vehicle discussion, immobilize-and-finish, LT order use, Engineers. **Blue Wolf is Vanilla context, not ISS eligibility.** |
| **Cross-faction video** | [Robert Shepherd — N5 Faction Focus: Yu Jing (25 Apr 2025)](https://www.youtube.com/watch?v=mn4yHSNxsnA) | **YouTube transcript reviewed.** Contrast Yu Jing's HI identity and Vanilla broad threat access with ISS-specific Fireteams. |
| **TAG fundamentals** | [Loss of Lieutenant — Ep141 Tactical Armored Gear (31 Mar 2025)](https://open.spotify.com/episode/6zPRTbn2cilgMyuHtODvf7) | **Podcast transcript reviewed.** TAG mission roles, why BS14/ARM7 remain valuable, repairs, E/M counterplay, Lóngwáng's niche. |
| **TAG comparative opinions** | [Loss of Lieutenant — Ep142 N5 TAG Tier List (6 Apr 2025)](https://open.spotify.com/episode/1h5CJfZC5zBPxdg66o7xIN) | **Podcast transcript retrieved; comparative tier discussion sampled.** Broad TAG tradeoffs and disagreement; don't copy old profile rankings as current N5.3 verdicts. |
| **Independent written dissent** | [Thanqol Decadion — Infinity Faction Focus: Imperial Service (25 Mar 2025)](https://www.tabletopbattles.com/infinity-faction-focus-imperial-service-2) | **Article reviewed, not MCP audio.** Compares ISS vs Vanilla, E/M positioning, Koga/Qiánfēng, Lóngwáng and Fēiquán. |
| **Additional videos index** | [Bureau Aegis N5 Imperial Service resource roundup](https://www.bureau-aegis.org/forum/index.php?topic=17850.0) | **Index checked; linked individual transcripts not all obtained.** Includes The Dice Gods War Gaming's **2 Apr 2025 Imperial Service Bundle** breakdown, Dante's **29 Mar 2025 Imperial Service Initial Reaction**, and faction-era change dates. These are further viewing, **not** claimed transcript-reviewed. |

**Version guardrails:** Do not copy old comments claiming a Lóngwáng *normal* HMG or BS Attack(-3), 2025 Fireteam limits, or pre-rework unit availability into authoritative fields. Verify against the roster/Fireteam tables in this document. Similarly, pilots/ancillaries and Yu Jing shared REMs do **not** imply that all Vanilla Yu Jing TAGs are accessible in ISS.

## Validation and maintenance

- Standard ISS roster represented: **43 units**.
- Optional-mode hooks: **Guǐ Fēng Spec-Ops** and **Yu Jing Team-Ops**.
- Canonical main Fireteam rows represented: **Celestial Guard, Kuang Shi, ALEPH Support, Wu Míng, Zhian (Law&Order), Fast Attack, Wildcards**.
- Main limits preserved: `CORE 1`, `HARIS 2`, raw `DUO 256` = InfinityDB `unlimited`.
- Parenthetical source comments are stored as Counts-as/equivalence labels.
- FTO restrictions are applied only where the Fireteam member/Wildcard row contains an FTO marker.
- Sforza is restricted to options **2/3** in Zhian because the source row is `FTO (Bounty Hunter)`.
- Son-Bae Wildcard access is restricted to option **2** (`Yáokòng SON-BAE FTO`).
- Pangguling Wildcard access is restricted to option **4** (`PANGGULING FTO`).
- Linked Reinforcement force **Daebak Force** is represented separately with its distinct roster and Fireteam chart.
- Reinforcement chart rows represented: **Jujaks Reinforcement, Hwarang Reinforcement, Reinforcement Wildcards**.
- Main and Reinforcement Fireteams are deliberately not merged.

### Refresh rule

When a newer Army source revision or InfinityDB normalization supersedes the provenance above, set `status: stale` until roster/profile/Fireteam changes are reconciled. Do not silently mix newer live values into this file without updating the provenance block.
