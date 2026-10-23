---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 204
sectorial_slug: invincible-army
sectorial_name: Invincible Army
parent_faction: Yu Jing
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
linked_reinforcement_id: 299
linked_reinforcement_name: Dàebàk Force
coverage: "Standard Invincible Army roster, standard loadouts, canonical main Fireteam chart, reverse Fireteam index, optional Spec-Ops/Team-Ops hooks, and linked Dàebàk Reinforcement roster/Fireteam chart."
---

# Invincible Army

## Overview and provenance

Repository-native reference for **Invincible Army** (Yu Jing sectorial, Army ID `204`) under the schema in `sectorials/REFERENCE_DESIGN.md`.

Sources used:

- Army-derived N5 snapshot `7.26246.158` from `massayoshi/infinity-army-backup`, file `n5/invincible-army/7.26246.158.json`, last changed for N5.3/ITS18 by source commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` on 2026-09-03.
- Linked Reinforcement roster: **Dàebàk Force** (Army ID `299`), source file `n5/daebak-force/7.26246.158.json`.
- InfinityDB semantic/reference baseline pinned at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Repository rules baseline: **N5.3** plus the current N5 FAQ material tracked in this repository.

Coverage notes:

- The ordinary matched-play roster below contains **34 standard Invincible Army units** in Army roster order.
- `GUǏ FĒNG SPEC-OPS` and `YU JING TEAM-OPS` are optional-mode hooks, not ordinary matched-play roster entries.
- Soldier-of-Fortune-only entries exposed by the Army data are not part of the sectorial roster and are intentionally omitted.
- Main-sectorial and Reinforcement Fireteam charts are kept separate. Do not merge Dàebàk rows into the main Invincible Army chart.

## Roster index

| Unit | ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| WÈIBĪNG Yáokòng | 139 | 2 | REM | Regular | — |
| MECH-ENGINEERS (Zhanshi Gōngchéng) | 138 | 2 | LI | Regular | Zhanshi |
| Yáopú PANGGULING | 162 | 2 | REM | Regular | Wildcard (FTO only) |
| Yáoxiè LÙ DUĀN | 160 | 2 | REM | Regular | — |
| MÓWÁNG Troops | 1254 | 3 | HI | Regular | Shock |
| WARCORS | 50 | 1 | LI | Irregular | — |
| CHAĪYÌ Yáokòng | 142 | 2 | REM | Regular | — |
| Zhanshi YĪSHĒNG | 137 | 1 | LI | Regular | Zhanshi |
| Yáoxiè RUI SHI | 159 | 2 | REM | Regular | Invincible |
| YĀN HUǑ Invincibles | 128 | 4 | HI | Regular | Invincible (FTO only) |
| LÉI GŌNG | 1497 | 1 | HI | Regular | Wildcard |
| ZHANSHI | 124 | 5 | LI | Regular | Zhanshi |
| Krit KOKRAM | 1445 | 1 | HI | Regular | Forward (FTO-2); Wildcard (FTO) |
| TAI SHENG | 1263 | 1 | HI | Regular | Wildcard |
| SĀCHĀ, Xenotech Hunters | 1874 | 1 | LI | Irregular | — |
| HǍIDÀO Special Support Group | 1246 | 3 | HI | Regular | Wildcard |
| ZHĒNCHÁ | 1259 | 4 | HI | Regular | — |
| DĀOYĪNG Operative Control Unit | 1244 | 3 | MI | Regular | — |
| HÚLÁNG Shocktroopers | 1257 | 2 | HI | Regular | Forward (FTO-2); Wildcard (FTO) |
| ZÚYǑNG Invincibles | 127 | 5 | HI | Regular | Invincible |
| HAC TAO Special Unit | 131 | 1 | HI | Regular | — |
| BÌXIÉ | 1599 | 1 | HI | Regular | Zhanshi; Invincible |
| Captain QIANG GĀO | 1498 | 1 | HI | Regular | Wildcard |
| SON-BAE Yáokòng | 141 | 1 | REM | Regular | Wildcard (FTO only) |
| LIÚ XĪNG Jump Infantry | 1248 | 4 | HI | Regular | — |
| GŪIJIĂ Squadrons | 133 | 2 | TAG | Regular + Tactical Awareness | Shock |
| Chief Mech-Engineer CHUNG-HEE JEONG | 1539 | 1 | LI | Regular | Wildcard |
| SHÀNG JÍ INVINCIBLES | 150 | 5 | HI | Regular + Tactical Awareness | Invincible; Wildcard |
| HÙSÒNG Yáokòng | 140 | 3 | REM | Regular | — |
| GŪDǍN Troops | 1841 | 2 | LI | Regular | Zhanshi (FTO only) |
| QÍSHÌ, StateEmpire TAG Support Pilots | 1838 | 1 | LI | Regular | Zhanshi |
| LIBERTOS Freedom Fighters | 1275 | 1 | LI | Irregular | — |
| YÁOZĂO | 161 | 4 | REM | Peripheral | — |
| Johnny Kao | 1892 | 1 | MI | Regular | — |

### Optional-mode units

| Unit | ID | Mode | Ordinary roster? | Fireteam hook |
|---|---:|---|---|---|
| GUǏ FĒNG SPEC-OPS | 1914 | Spec-Ops | No | Zhanshi Fireteam, max 1 |
| YU JING TEAM-OPS | 1928 | Team-Ops | No | No ordinary Fireteam-chart row |

## Unit details

### WÈIBĪNG Yáokòng (Guardian Remote)

**ID 139 · AVA 2 · REM · Support Troops · Regular** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`.

Base kit: Deactivator, Repeater; Remote Presence, Courage, Triangulated Fire, Forward Observer, Sensor.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Flash Pulse, PARA CC Weapon (-3) | — |
| 2 | 17 | 0 | As opt 1; **Tactical Awareness** | — |

### MECH-ENGINEERS (Zhanshi Gōngchéng)

**ID 138 · AVA 2 · LI · Support Troops · Regular** — `MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`.

Base kit: Deactivator, GizmoKit; Engineer.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, D-Charges, Pistol, CC Weapon | Zhanshi; counts as Zhanshi |
| 2 | 15 | 0 | As opt 1; Deployable Cover | Zhanshi; counts as Zhanshi |
| 3 | 17 | 0 | Combi Rifle, Armed Turret (Combi Rifle), Pistol, CC Weapon | Zhanshi; counts as Zhanshi |

### Yáopú PANGGULING

**ID 162 · AVA 2 · REM · Support Troops · Regular** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 4`.

Base kit: Baggage; Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | PARA CC Weapon (-3); Deactivator, Repeater | — |
| 2 | 14 | 0.5 | PARA CC Weapon (-3); EVO Hacking Device; Hacker | — |
| 3 | 17 | 0 | Combi Rifle, PARA CC Weapon (-3); Repeater; Total Reaction | — |
| 4 | 12 | 0 | **PANGGULING FTO** — Light Shotgun, PARA CC Weapon (-3); Repeater | Wildcard |

### Yáoxiè LÙ DUĀN

**ID 160 · AVA 2 · REM · Support Troops · Regular** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 4`.

Base kit: Holoprojector, Multispectral Visor L1; Remote Presence, Surprise Attack (-3), Courage, BS Attack (+1B).

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 0 | Mk12, Heavy Flamethrower, E/M Mine, PARA CC Weapon (-3) | — |
| 2 | 20 | 0 | Thunderbolt, E/M Carbine, E/M Mine, PARA CC Weapon (-3) | — |

### MÓWÁNG Troops

**ID 1254 · AVA 3 · HI · Elite Troops · Regular** — `MOV 15-5 | CC 17 | BS 13 | PH 13 | WIP 13 | ARM 5 | BTS 6 | W 2 | S 5`.

Base skills: Courage, Mimetism (-3), Stealth, No Wound Incapacitation, Terrain (Total), Combat Instinct.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 3 | 42 | 1.5 | Spitfire, Flammenspeer, AP Heavy Pistol, CC Weapon (PS=7) | Shock Duo |
| 5 | 44 | 1 | Red Fury, Flammenspeer, Disco Baller, AP Heavy Pistol, CC Weapon (PS=7); NCO | Shock Duo |
| 6 | 44 | 1.5 | Spitfire, Flammenspeer, AP Heavy Pistol, CC Weapon (PS=7); NCO | Shock Duo |
| 9 | 42 | 1 | Spitfire, Flammenspeer, AP Heavy Pistol, CC Weapon (PS=7); Lieutenant | Shock Duo |

### WARCORS, WAR CORRESPONDENTS

**ID 50 · AVA 1 · LI · Mercenary Troops · Irregular** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`.

Base skill: Journalist.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CC Weapon (-3); 360º Visor | — |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CC Weapon (-3); Sixth Sense | — |

### CHAĪYÌ Yáokòng (Messenger Remote)

**ID 142 · AVA 2 · REM · Support Troops · Regular** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`.

Base kit: Repeater; Remote Presence, Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | Flash Pulse, PARA CC Weapon (-3) | — |

### Zhanshi YĪSHĒNG

**ID 137 · AVA 1 · LI · Support Troops · Regular** — `MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`.

Base kit: MediKit; Doctor.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Pistol, CC Weapon | Zhanshi; counts as Zhanshi |

### Yáoxiè RUI SHI

**ID 159 · AVA 2 · REM · Support Troops · Regular** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 6 | W 1 | S 4`.

Base kit: Repeater; Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 1 | Spitfire, PARA CC Weapon (-3); Multispectral Visor L2 | Invincible |
| 2 | 21 | 0.5 | Red Fury, Mine Dispenser (Shock), PARA CC Weapon (-3); Multispectral Visor L1 | Invincible |

### YĀN HUǑ Invincibles, Fire Support Heavy Regiment

**ID 128 · AVA 4 · HI · Line Troops · Regular** — `MOV 10-10 | CC 18 | BS 14 | PH 13 | WIP 13 | ARM 5 | BTS 3 | W 2 | S 5`.

Base skills: Immunity (ARM), Warhorse, Religious Troop.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 45 | 1.5 | **YĀN HUǑ FTO** — MULTI HMG, Heavy Pistol, CC Weapon (PS=7) | Invincible |
| 2 | 47 | 1.5 | HRMC, Heavy Pistol, CC Weapon (PS=7) | — |
| 3 | 41 | 1.5 | **YĀN HUǑ FTO** — Missile Launcher (+1B), Mine Dispenser (Shock), Heavy Pistol, CC Weapon (PS=7) | Invincible |
| 4 | 42 | 1.5 | Missile Launcher, Heavy Pistol, CC Weapon (PS=7); Neurocinetics (+1B) | — |

### LÉI GŌNG, Invincibles Lord of Thunder

**ID 1497 · AVA 1 · HI · Character · Regular** — `MOV 15-5 | CC 18 | BS 13 | PH 12 | WIP 14 | ARM 3 | BTS 6 | W 1 | S 2`.

Base kit: Albedo (-6), Multispectral Visor L1; Courage, Immunity (ARM), No Wound Incapacitation, Super-Jump (source carries both Jet Propulsion and 7.5-distance modifiers).

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 32 | 0 | AP Submachine Gun, E/Mitter, Zapper, Breaker Pistol, CC Weapon; Parachutist | Wildcard; counts as Invincible |
| 2 | 34 | 0 | **FTO** — MULTI Marksman Rifle, Zapper, Blitzen, Breaker Pistol, CC Weapon | Wildcard; counts as Invincible |
| 4 | 29 | 0 | **FTO** — AP Submachine Gun, E/Mitter, Zapper, Breaker Pistol, CC Weapon | Wildcard; counts as Invincible |
| 5 | 34 | 0 | **FTO** — as opt 4; Chain of Command | Wildcard; counts as Invincible |

### ZHANSHI

**ID 124 · AVA 5 · LI · Line Troops · Regular** — `MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 10 | 0 | Combi Rifle, Pistol, CC Weapon | Zhanshi |
| 2 | 18 | 1 | HMG, Pistol, CC Weapon | Zhanshi |
| 4 | 16 | 1 | MULTI Sniper Rifle, Pistol, CC Weapon | Zhanshi |
| 5 | 15 | 1.5 | Missile Launcher, Pistol, CC Weapon | Zhanshi |
| 6 | 15 | 0.5 | Combi Rifle, Pistol, CC Weapon; Hacking Device; Hacker | Zhanshi |
| 8 | 11 | 0 | Combi Rifle, Flash Pulse, Pistol, CC Weapon; Forward Observer | Zhanshi |
| 9 | 12 | 0 | Combi Rifle, Pistol, CC Weapon; MediKit; Paramedic | Zhanshi |
| 10 | 10 | 0 | Combi Rifle, Pistol, CC Weapon; Lieutenant | Zhanshi |
| 11 | 12 | 0 | Combi Rifle, Pistol, CC Weapon; Commlink (+1); Specialist Operative | Zhanshi |

### Krit KOKRAM, Zúyŏng Invincibles Specialist

**ID 1445 · AVA 1 · HI · Character · Regular** — `MOV 15-5 | CC 19 | BS 13 | PH 12 | WIP 14 | ARM 3 | BTS 3 | W 2 | S 2`.

Base kit: Deactivator, GizmoKit; Courage, Dodge (+5), Engineer, NCO.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 37 | 0 | **KOKRAM FTO-2** — Heavy Shotgun, E/Mitter, Chain-colt, E/M Mine, Heavy Pistol (+1B), CC Weapon; Deployable Repeater, Forward Deployment (+20), Minelayer | Forward; Wildcard; counts as Invincible in Wildcard role |
| 2 | 35 | 0 | **KOKRAM FTO** — MULTI Rifle (PS=6), Chain-colt, D-Charges, Heavy Pistol (+1B), CC Weapon | Wildcard; counts as Invincible |
| 3 | 40 | 1.5 | **KOKRAM FTO** — Feuerbach, Chain-colt, D-Charges, Heavy Pistol (+1B), CC Weapon | Wildcard; counts as Invincible |

### TAI SHENG, Zúyŏng Invincibles NCO

**ID 1263 · AVA 1 · HI · Character · Regular** — `MOV 15-5 | CC 18 | BS 14 | PH 12 | WIP 14 | ARM 3 | BTS 6 | W 2 | S 2`.

Base skills: Courage, Dodge (+5), Forward Observer, NCO, Warhorse, Sixth Sense.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 37 | 0 | Breaker Combi Rifle (+1B), Chain-colt, Flash Pulse, Heavy Pistol, CC Weapon; TinBot Firewall (-6) | Wildcard; counts as Invincible |
| 2 | 33 | 0 | Thunderbolt (+1B), Chain-colt, Flash Pulse, Heavy Pistol, CC Weapon | Wildcard; counts as Invincible |
| 3 | 40 | 0 | As opt 1; Chain of Command | Wildcard; counts as Invincible |
| 4 | 36 | 0 | As opt 2; Chain of Command | Wildcard; counts as Invincible |

### SĀCHĀ, Xenotech Hunters

**ID 1874 · AVA 1 · LI · Mercenary Troops · Irregular** — `MOV 10-10 | CC 17 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`.

Base skills: Forward Deployment (+10), Booty, Terrain (Total), Climbing Plus, Specialist Operative.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 6 | 0 | Flash Pulse, E/M Grenades (+1B), Stun Pistol (+1B), CC Weapon | — |

### HǍIDÀO Special Support Group

**ID 1246 · AVA 3 · HI · Spec. Trained Troops · Regular** — `MOV 10-10 | CC 18 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`.

Base skills: Courage, Immunity (Shock), No Wound Incapacitation, Terrain (Zero-G).

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 2 | 24 | 1 | Red Fury, Breaker Pistol, CC Weapon | Wildcard |
| 3 | 24 | 0 | Combi Rifle, D-Charges, Breaker Pistol, CC Weapon; Chain of Command | Wildcard |
| 4 | 22 | 0 | Boarding Shotgun (+1B), Pitcher, D-Charges, Breaker Pistol, CC Weapon; Killer Hacking Device; Hacker | Wildcard |
| 5 | 25 | 0 | MULTI Rifle, D-Charges, Breaker Pistol, CC Weapon; Deactivator, GizmoKit; Engineer | Wildcard |
| 6 | 29 | 1.5 | MULTI Sniper Rifle, Breaker Pistol, CC Weapon; Multispectral Visor L2 | Wildcard |

### ZHĒNCHÁ, Armored Reconnaissance Regiment

**ID 1259 · AVA 4 · HI · Spec. Trained Troops · Regular** — `MOV 10-10 | CC 16 | BS 12 | PH 13 | WIP 13 | ARM 3 | BTS 6 | W 1 | S 2`.

Base skills: Surprise Attack (-3), Camouflage, Courage, Infiltration, Immunity (Shock), Mimetism (-3), Stealth, Terrain (Total), Climbing Plus, No Wound Incapacitation.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 30 | 0 | Boarding Shotgun, Flash Pulse, D-Charges, Silenced Pistol, CC Weapon; Forward Observer | — |
| 2 | 31 | 0 | Submachine Gun, Panzerfaust, Flash Pulse, Shock Mine, Silenced Pistol, CC Weapon; Forward Observer | — |
| 3 | 31 | 0 | Submachine Gun, Panzerfaust, Flash Pulse, Silenced Pistol, CC Weapon; Deployable Repeater; Forward Observer | — |
| 4 | 34 | 0.5 | Boarding Shotgun, D-Charges, Silenced Pistol, CC Weapon; Hacking Device (Upgrade: Trinity); Hacker | — |
| 5 | 32 | 0.5 | Submachine Gun, Panzerfaust, Shock Mine, Silenced Pistol, CC Weapon; Minelayer (2) | — |

### DĀOYĪNG Operative Control Unit

**ID 1244 · AVA 3 · MI · Spec. Trained Troops · Regular** — `MOV 10-10 | CC 17 | BS 12 | PH 11 | WIP 14 | ARM 3 | BTS 3 | W 1 | S 2`.

Base skills: Surprise Attack (-3), Camouflage, Immunity (Shock), Mimetism (-3), Stealth.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 19 | 0 | Boarding Shotgun, Breaker Pistol, CC Weapon | — |
| 2 | 24 | 0.5 | As opt 1; Hacking Device; Hacker | — |
| 3 | 30 | 1.5 | MULTI Sniper Rifle, Shock Mine, Breaker Pistol, CC Weapon; Minelayer | — |
| 4 | 23 | 0 | Boarding Shotgun, Breaker Pistol, CC Weapon; Lieutenant (+1 Order) | — |
| 6 | 28 | 0 | As opt 4; Hacking Device; Hacker | — |
| 7 | 34 | 1 | MULTI Sniper Rifle, Shock Mine, Breaker Pistol, CC Weapon; Lieutenant (+1 Order), Minelayer | — |

### HÚLÁNG Shocktroopers

**ID 1257 · AVA 2 · HI · Veteran Troops · Regular** — `MOV 15-5 | CC 22 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`.

Base skills: Martial Arts L2, Courage, Dodge (+5), Immunity (Shock), Mimetism (-6), Specialist Operative, Stealth, No Wound Incapacitation, Berserk, Combat Instinct.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 38 | 0.5 | **HÚLÁNG FTO-2** — Combi Rifle (+1B), Light Flamethrower, D-Charges, AP Mine, Pistol, Monofilament CC Weapon; Forward Deployment (+20), Minelayer | Forward; Wildcard |
| 2 | 38 | 0 | **HÚLÁNG FTO-2** — Submachine Gun, E/Mitter, D-Charges, CrazyKoala, Pistol, Monofilament CC Weapon; Forward Deployment (+20), Minelayer | Forward; Wildcard |
| 3 | 31 | 0 | **HÚLÁNG FTO** — Submachine Gun, E/Mitter, D-Charges, Disco Baller, Pistol, Monofilament CC Weapon | Wildcard |
| 4 | 33 | 0 | **HÚLÁNG FTO** — Combi Rifle (+1B), Light Flamethrower, D-Charges, Pistol, Monofilament CC Weapon | Wildcard |

### ZÚYǑNG Invincibles, Terra-Cotta Soldiers

**ID 127 · AVA 5 · HI · Line Troops · Regular** — `MOV 15-5 | CC 17 | BS 13 | PH 12 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`.

Base skills: Dodge (+2.5 distance), Number 2.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 2 | 26 | 0 | MULTI Rifle, Breaker Pistol (+1B), CC Weapon; TinBot Firewall (-6) | Invincible; counts as Invincible |
| 3 | 30 | 1.5 | HMG, Breaker Pistol (+1B), CC Weapon | Invincible; counts as Invincible |
| 4 | 22 | 0 | Boarding Shotgun, E/Mitter, Breaker Pistol (+1B), CC Weapon | Invincible; counts as Invincible |
| 5 | 24 | 0 | MULTI Rifle, Breaker Pistol (+1B), CC Weapon | Invincible; counts as Invincible |
| 6 | 31 | 1.5 | Missile Launcher, Light Shotgun, Breaker Pistol (+1B), CC Weapon | Invincible; counts as Invincible |
| 8 | 27 | 0 | Combi Rifle, Breaker Pistol (+1B), CC Weapon; TinBot Firewall (-6); Tactical Awareness | Invincible; counts as Invincible |
| 11 | 26 | 0 | MULTI Rifle, Breaker Pistol (+1B), CC Weapon; MediKit; Paramedic | Invincible; counts as Invincible |
| 12 | 33 | 1.5 | HMG, Breaker Pistol (+1B), CC Weapon; Tactical Awareness | Invincible; counts as Invincible |

### HAC TAO Special Unit

**ID 131 · AVA 1 · HI · Elite Troops · Regular** — `MOV 15-5 | CC 19 | BS 14 | PH 14 | WIP 14 | ARM 5 | BTS 6 | W 2 | S 2`.

Base skills: Surprise Attack (-3), Camouflage, Hidden Deployment, Dodge (+2.5 distance), Mimetism (-6), Stealth.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 4 | 60 | 1.5 | Missile Launcher (+1B), Nanopulser, Pistol, Shock CC Weapon (PS=6) | — |
| 5 | 58 | 0.5 | MULTI Rifle (PS=6), Nanopulser, Pistol, Shock CC Weapon (PS=6); Hacking Device (Upgrade: Trinity); Hacker | — |
| 7 | 59 | 1.5 | HMG, Nanopulser, Pistol, Shock CC Weapon (PS=6); NCO | — |

### BÌXIÉ, The Jade Champion

**ID 1599 · AVA 1 · HI · Character · Regular** — `MOV 15-5 | CC 22 | BS 13 | PH 12 | WIP 13 | ARM 3 | BTS 6 | W 2 | S 2`.

Base kit: Multispectral Visor L1; Martial Arts L3, Courage, Dodge (source carries both +6 and +5-distance modifiers), Forward Observer, Stealth, NCO, Super-Jump, Climbing Plus.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 41 | 0 | MULTI Rifle, Zapper, Flash Pulse, Pistol, E/M CC Weapon (PS=6) | Zhanshi; Invincible (counts as Invincible there) |

### Captain QIANG GĀO, Invincibles Officer

**ID 1498 · AVA 1 · HI · Character · Regular** — `MOV 15-5 | CC 17 | BS 13 | PH 12 | WIP 14 | ARM 5 | BTS 6 | W 2 | S 2`.

Base kit: ECM: Hacker (-3); BS Attack (-3), Dodge (+2.5 distance), Warhorse, Immunity (IMM-B).

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 48 | 1.5 | HMG, Nanopulser, Breaker Pistol (+1B), CC Weapon | Wildcard; counts as Invincible |
| 2 | 48 | 1 | As opt 1; Lieutenant | Wildcard; counts as Invincible |

### SON-BAE Yáokòng

**ID 141 · AVA 1 · REM · Support Troops · Regular** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`.

Base skills: Remote Presence, Courage.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CC Weapon (-3); BS Attack (Guided) | — |
| 2 | 19 | 1.5 | **Yáokòng SON-BAE FTO** — Missile Launcher (+1B), PARA CC Weapon (-3) | Wildcard |

### LIÚ XĪNG Jump Infantry

**ID 1248 · AVA 4 · HI · Veteran Troops · Regular** — `MOV 15-5 | CC 19 | BS 13 | PH 13 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`.

Base skills: Courage, Dodge (+5), Immunity (Shock), Combat Jump (Explosion), Combat Jump (PH=14), Parachutist, No Wound Incapacitation, Super-Jump (Jet Propulsion).

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 0 | Boarding Shotgun, Boarding Pistol, CC Weapon | — |
| 2 | 33 | 1.5 | Spitfire, Boarding Pistol, CC Weapon | — |
| 3 | 30 | 0 | MULTI Rifle, D-Charges, Boarding Pistol, CC Weapon; Specialist Operative | — |
| 4 | 30 | 0.5 | Boarding Shotgun, Boarding Pistol, CC Weapon; Hacking Device (Firewall -6); Hacker | — |

### GŪIJIĂ Squadrons

**ID 133 · AVA 2 · TAG · Mechanized Troops · Regular + Tactical Awareness** — `MOV 15-10 | CC 22 | BS 14 | PH 16 | WIP 13 | ARM 8 | BTS 6 | STR 3 | S 7`.

Base kit: ECM: Guided (-6); Martial Arts L2, Courage, Dodge (PH=11), Tactical Awareness, Super-Jump, GizmoKit (PH=11), BS Attack (SR-1). Includes a SHÀNGDIÀO Ancillary Remote Unit.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 77 | 1.5 | MULTI HMG, Heavy Flamethrower, DA CC Weapon (PS=3) | Shock Duo |
| 2 | 77 | 2 | As opt 1; Lieutenant | Shock Duo |

### Chief Mech-Engineer CHUNG-HEE JEONG

**ID 1539 · AVA 1 · LI · Character · Regular** — `MOV 10-10 | CC 17 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`.

Base kit: Deactivator, GizmoKit, Repeater; BS Attack (+1B), Dodge (+2.5 distance), Immunity (Shock), Engineer (ReRoll -3).

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 31 | 0 | Combi Rifle (AP), E/Mitter, D-Charges, Armed Turret (AP Marksman Rifle), Pistol, CC Weapon | Wildcard; counts as Zhanshi |
| 2 | 27 | 0 | K1 Combi Rifle, AP Mine (PS=5), D-Charges, Pistol, CC Weapon | Wildcard; counts as Zhanshi |

### SHÀNG JÍ INVINCIBLES

**ID 150 · AVA 5 · HI · Line Troops · Regular + Tactical Awareness** — `MOV 15-5 | CC 19 | BS 13 | PH 14 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 2`.

Base skills: BS Attack (Shock), Dodge (+5), Number 2, Terrain (Total), Tactical Awareness, Jump (7.5 distance).

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 2 | 37 | 0 | MULTI Rifle, Boarding Pistol, AP CC Weapon (PS=6); TinBot Firewall (-6) | Invincible; Wildcard; counts as Invincible |
| 7 | 40 | 0.5 | MULTI Rifle, Flash Pulse, D-Charges, Boarding Pistol, AP CC Weapon (PS=6); Hacking Device; Hacker | Invincible; Wildcard; counts as Invincible |
| 10 | 36 | 0 | MULTI Rifle, Flash Pulse, Boarding Pistol, AP CC Weapon (PS=6); Forward Observer | Invincible; Wildcard; counts as Invincible |
| 11 | 45 | 1.5 | AP HMG, Boarding Pistol, AP CC Weapon (PS=6); TinBot Firewall (-6) | Invincible; Wildcard; counts as Invincible |
| 13 | 34 | 1.5 | Heavy Rocket Launcher, Light Shotgun, Boarding Pistol, AP CC Weapon (PS=6) | Invincible; Wildcard; counts as Invincible |
| 16 | 45 | 1 | AP HMG, Boarding Pistol, AP CC Weapon (PS=6); TinBot Firewall (-6); Lieutenant | Invincible; Wildcard; counts as Invincible |

### HÙSÒNG Yáokòng (Escort Remote)

**ID 140 · AVA 3 · REM · Support Troops · Regular** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`.

Base kit: 360º Visor; Remote Presence, Courage, Total Reaction.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 1 | HMG, PARA CC Weapon (-3) | — |
| 2 | 18 | 0 | Thunderbolt (+1B), PARA CC Weapon (-3) | — |

### GŪDǍN Troops

**ID 1841 · AVA 2 · LI · Garrison Troops · Regular** — `MOV 10-10 | CC 15 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`.

Base skills: Warhorse, Terrain (Mountain).

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 11 | 0 | **GŪDǍN FTO** — Light Shotgun, Heavy Flamethrower, Pistol, CC Weapon | Zhanshi; counts as Zhanshi |
| 2 | 11 | 0 | **GŪDǍN FTO** — Submachine Gun, Zapper, Pistol, CC Weapon | Zhanshi; counts as Zhanshi |
| 3 | 13 | 0 | Light Shotgun, Heavy Flamethrower, Shock Mine, Pistol, CC Weapon; Camouflage (1 Use), Forward Deployment (+10) | — |
| 4 | 12 | 0 | Submachine Gun, Zapper, Shock Mine, Pistol, CC Weapon; Camouflage (1 Use), Forward Deployment (+10) | — |

### QÍSHÌ, StateEmpire TAG Support Pilots

**ID 1838 · AVA 1 · LI · Support Troops · Regular** — `MOV 10-10 | CC 21 | BS 11 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 2`.

Base skills: Courage, Specialist Operative, Stealth, TAGCom (Dodge PH+3; GizmoKit PH+1).

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 11 | 0 | **GŪIJIĂ PILOT** — Submachine Gun, Pistol, Shock CC Weapon (PS=7); GizmoKit; Martial Arts L1 | Zhanshi; counts as Zhanshi |

### LIBERTOS Freedom Fighters

**ID 1275 · AVA 1 · LI · Mercenary Troops · Irregular** — `MOV 10-10 | CC 16 | BS 11 | PH 11 | WIP 12 | ARM 0 | BTS 0 | W 1 | S 2`.

Base skills: Camouflage (1 Use), Courage, Forward Deployment (+20), Dodge (+3 and +2.5-distance modifiers in source), Terrain (Aquatic), Dogged, Frenzy.

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | Submachine Gun, Chain-colt, Pistol, CC Weapon | — |
| 4 | 8 | 1 | Light Shotgun, Shock Mine, Pistol, CC Weapon; Minelayer | — |

### YÁOZĂO

**ID 161 · AVA 4 · REM · Support Troops · Peripheral** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`.

Base skills: Peripheral (Servant), Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | PARA CC Weapon (-3); `minis: 0`, no independent Order | — |

### Johnny Kao, Optimate and Technomancer Master

**ID 1892 · AVA 1 · MI · Character · Regular** — `MOV 15-5 | CC 18 | BS 13 | PH 12 | WIP 14 | ARM 3 | BTS 6 | W 2 | S 2`.

Base kit: Cube 2.0, Non Hackable; Deactivator (ReRoll), GizmoKit (+1B), X Visor; Engineer (ReRoll), Mimetism (-3).

| Opt | Pts | SWC | Loadout / role | FT |
|---:|---:|---:|---|---|
| 1 | 36 | 0 | Plasma Carbine, Zapper, Monofilament Mine, D-Charges, MULTI Pistol, CC Weapon | — |
| 2 | 40 | 0 | MULTI Rifle, Zapper, Drop Bears (ARM=0), D-Charges, MULTI Pistol, CC Weapon | — |
| 3 | 42 | 0 | MULTI Rifle, Zapper, Monofilament Mine, D-Charges, Armed Turret (Plasma Carbine), MULTI Pistol, CC Weapon | — |

## Fireteams

This section is **canonical** for the main Invincible Army Fireteam chart. The Unit → Fireteam index below is derivative.

### Chart limits

| Type | Raw source | Meaning |
|---|---:|---|
| Core | 1 | Maximum 1 |
| Haris | 1 | Maximum 1 |
| Duo | 256 | InfinityDB-normalized meaning: unlimited |

### Zhanshi Fireteams

**Types:** Haris, Core.

| Member | Min | Max | Required choice | Counts as | Profile restriction |
|---|---:|---:|---|---|---|
| ZHANSHI | 1 | 5 | No | — | All |
| GŪDǍN FTO | 0 | 2 | No | Zhanshi | Options 1, 2 only |
| Zhanshi YĪSHĒNG | 0 | 1 | No | Zhanshi | All |
| MECH-ENGINEER | 0 | 1 | No | Zhanshi | All |
| BÌXIÉ | 0 | 1 | No | — | All |
| QÍSHÌ | 0 | 1 | No | Zhanshi | All |
| GUǏ FĒNG | 0 | 1 | No | — | Spec-Ops mode only |

### Invincible Fireteams

**Types:** Duo, Haris, Core.

| Member | Min | Max | Required choice | Counts as | Profile restriction |
|---|---:|---:|---|---|---|
| ZÚYǑNG | 0 | 5 | **Yes** | Invincible | All |
| SHÀNG JÍ | 0 | 5 | **Yes** | Invincible | All |
| YĀN HUǑ FTO | 0 | 2 | No | — | Options 1, 3 only |
| BÌXIÉ | 0 | 1 | No | Invincible | All |
| RUI SHI | 0 | 1 | No | — | All |

The Army source marks **both** ZÚYǑNG and SHÀNG JÍ rows `required: true` even though each row has `min: 0`. Preserve those flags literally; do not silently reinterpret or collapse them into a single inferred condition.

### Shock Fireteams

**Type:** Duo.

| Member | Min | Max | Required choice | Counts as | Profile restriction |
|---|---:|---:|---|---|---|
| MÓWÁNG | 0 | 2 | **Yes** | — | All |
| GŪIJIĂ | 0 | 2 | **Yes** | — | All |

The Army source likewise marks **both** MÓWÁNG and GŪIJIĂ rows `required: true` with `min: 0`; preserve the source flags literally.

### Forward Fireteams

**Type:** Duo.  
**Special restriction:** `No Wildcards Special Fireteam`.

| Member | Min | Max | Required choice | Counts as | Profile restriction |
|---|---:|---:|---|---|---|
| HÚLÁNG FTO-2 | 1 | 2 | No | — | Options 1, 2 only |
| KOKRAM FTO-2 | 0 | 1 | No | — | Option 1 only |

Wildcards cannot be added to this special Fireteam.

### Wildcards

| Member | Max | Counts as | Profile restriction |
|---|---:|---|---|
| HǍIDÀO | 3 | — | All |
| SHÀNG JÍ | 2 | Invincible | All |
| HÚLÁNG | 2 | — | FTO / FTO-2 options 1–4 |
| SON-BAE Yaókòng | 1 | — | FTO option 2 only |
| PANGGULING | 1 | — | FTO option 4 only |
| TAI SHENG | 1 | Invincible | All |
| KOKRAM | 1 | Invincible | FTO / FTO-2 options 1–3 |
| CHIEF JEONG | 1 | Zhanshi | All |
| QIANG GĀO | 1 | Invincible | All |
| LÉI GŌNG | 1 | Invincible | All |

Wildcard status does not remove a Fireteam's native minimum, required-choice, type, or profile restrictions. Parenthetical Army-chart comments such as `(Invincible)` and `(Zhanshi)` are preserved here as Counts-as/equivalence labels.

## Unit → Fireteam access index

| Unit | Access |
|---|---|
| WÈIBĪNG Yáokòng | — |
| MECH-ENGINEER | Zhanshi (max 1; counts as Zhanshi) |
| PANGGULING | Wildcard (max 1; option 4 FTO only) |
| LÙ DUĀN | — |
| MÓWÁNG | Shock Duo (source-required row) |
| WARCOR | — |
| CHAĪYÌ | — |
| Zhanshi YĪSHĒNG | Zhanshi (max 1; counts as Zhanshi) |
| RUI SHI | Invincible (max 1) |
| YĀN HUǑ | Invincible (max 2; FTO opts 1,3 only) |
| LÉI GŌNG | Wildcard (max 1; counts as Invincible) |
| ZHANSHI | Zhanshi (min 1, max 5) |
| Krit KOKRAM | Forward Duo (FTO-2 opt 1); Wildcard (max 1 FTO; counts as Invincible) |
| TAI SHENG | Wildcard (max 1; counts as Invincible) |
| SĀCHĀ | — |
| HǍIDÀO | Wildcard (max 3) |
| ZHĒNCHÁ | — |
| DĀOYĪNG | — |
| HÚLÁNG | Forward Duo (FTO-2 opts 1,2); Wildcard (max 2 FTO) |
| ZÚYǑNG | Invincible (max 5; source-required row; counts as Invincible) |
| HAC TAO | — |
| BÌXIÉ | Zhanshi (max 1); Invincible (max 1; counts as Invincible) |
| QIANG GĀO | Wildcard (max 1; counts as Invincible) |
| SON-BAE | Wildcard (max 1; FTO opt 2 only) |
| LIÚ XĪNG | — |
| GŪIJIĂ | Shock Duo (source-required row) |
| CHIEF JEONG | Wildcard (max 1; counts as Zhanshi) |
| SHÀNG JÍ | Invincible (max 5; source-required row; counts as Invincible); Wildcard (max 2; counts as Invincible) |
| HÙSÒNG | — |
| GŪDǍN | Zhanshi (max 2; FTO opts 1,2; counts as Zhanshi) |
| QÍSHÌ | Zhanshi (max 1; counts as Zhanshi) |
| LIBERTOS | — |
| YÁOZĂO | — |
| Johnny Kao | — |
| GUǏ FĒNG SPEC-OPS | Zhanshi (max 1; optional Spec-Ops mode only) |

## Reinforcements — Dàebàk Force

Invincible Army links to Reinforcement roster **299: Dàebàk Force**. This roster and its Fireteam chart are separate from the main Invincible Army roster/chart above.

### Reinforcement roster index

| Unit | ID | AVA | Type | Order |
|---|---:|---:|---|---|
| REINF: YÁOZĂO | 1709 | 2 | REM | Peripheral |
| REINF: HWARANG CORPS | 1711 | 4 | HI | Regular |
| REINF: SULSA WARRIORS | 1712 | 2 | SK | Regular |
| REINF: Yáoxiè RUI SHI | 1718 | 1 | REM | Regular |
| REINF. Chief Mech-Engineer CHUNG-HEE JEONG | 1708 | 1 | LI | Regular |
| Reinf. DOKKAEBI Cyberteam | 1715 | 2 | HI | Regular |
| REINF: SON-BAE Yáokòng | 1717 | 1 | REM | Regular |
| REINF: Naval Operations Group SULYONG | 1714 | 2 | MI | Regular |
| REINF: BÌXIÉ, the Jade Champion | 1719 | 1 | HI | Regular |
| REINF: JUJAK Regiment, Korean Shock Infantry | 1707 | 3 | HI | Regular |
| REINF: WÈIBĪNG Yáokòng | 1716 | 2 | REM | Regular |
| REINF: Sergeant SO-RA KWON, Jujak Regiment | 1710 | 1 | HI | Regular |
| REINF: HAETAE Unit | 1713 | 1 | HI | Regular + Tactical Awareness |

The primary sectorial reference does not duplicate full Dàebàk loadout tables; the canonical Reinforcement roster identity and Fireteam legality data are retained here so main-list and Reinforcement access cannot be conflated.

### Reinforcement Fireteam chart limits

The Dàebàk source stores `CORE: 0`, `HARIS: 0`, and `DUO: 0` in the Reinforcement chart `spec` object. These values are preserved literally and must not be replaced with the main Invincible Army chart limits. The named Reinforcement rows below are the authoritative membership/type data for this linked roster.

### Jujaks Reinforcement Fireteams

**Types:** Duo, Haris, Core.

| Member | Min | Max | Required choice | Counts as | Profile restriction |
|---|---:|---:|---|---|---|
| JUJAK REF. | 1 | 3 | No | — | All Reinforcement Jujak profiles |
| HWARANG REINF. | 0 | 1 | No | — | All |

### Hwarang Reinforcement Fireteams

**Types:** Duo, Haris, Core.

| Member | Min | Max | Required choice | Counts as | Profile restriction |
|---|---:|---:|---|---|---|
| HWARANG REINF. | 1 | 4 | No | — | All |
| SULSA WARRIOR REINF. | 0 | 2 | No | Hwarang | All |
| HAETAE REF. | 0 | 1 | No | — | All |
| BÌXIÉ REINF. | 0 | 1 | No | — | All |

### Reinforcement Wildcards

| Member | Max | Counts as | Profile restriction |
|---|---:|---|---|
| SULYONG REINF. | 2 | — | All |
| Yáokòng WÈIBĪNG REINF. | 2 | — | All |
| Yáokòng SON-BAE REINF. | 1 | — | FTO option 3 only |
| DOKKAEBI REINF. | 1 | — | All |
| CHIEF JEONG REINF. | 1 | — | All |
| SO-RA KWON REINF. | 1 | Jujaks | All |

## Tactical research — Invincible Army N5 (2026-10-22)

> **Interpretive tactics, not authoritative profile data.** Use the N5.3 roster and canonical Fireteam chart above (Army version 7.26246.158, 2026-09-03) whenever a speaker describes older options or values. The dedicated N5 sources below date to Jan–Nov 2025. The Robert Shepherd *Invincible Army* faction-focus video is **N4, June 2024**, not N5, and is retained only as historical dissent. Auto-transcripts sometimes mishear unit names.

### General plan and list-building priorities

**Thesis:** Invincible Army (IA) trades broad cheap board control for **durable multiple-Wound HI, active-turn Order concentration, and flexible specialist/attack Fireteams**. Its challenge is to **win missions after winning gunfights**, particularly when facing hacking/E/M, visual mods, and attacks around its expensive HI. The 2025 CanCon 2nd-/3rd-place IA players (Peter Henry and Jacob Ridley) attribute their success to board-control buffers and mission-specific defensive architecture, not just a giant Fireteam. Tactical Awareness shows both NCO-heavy 10-model lists and broader defensive lists.

1. **Build around the order engine:** A **Dāoyīng Lieutenant (+1 Order)** (23-pt boarding shotgun, 28-pt hacker, or 34-pt sniper/Minelayer) offers two Lieutenant Orders for an **NCO** such as Mówáng, Tai Sheng, Krit, Bìxié or Hac Tao. Hide Dāoyīng until its own shooting, hacking or button-pushing matters. Don't buy every NCO if only one can use the extra orders effectively.
2. **Select the primary problem-solver:** **Shàng Jí AP HMG + TinBot Firewall(-6)** for a protected HI attack; **Mówáng NCO** for independent durable advance; **Yān Huǒ** for long-range attack or denial; **Gūijiă TAG** for heavy shooting, Super-Jump and melee defence. Avoid paying for all four if that leaves no orders and specialists.
3. **Plan a second angle and actual scoring:** **Zhēnchá** camo/infiltration, **Húláng** forward attack, **Liú Xīng** airborne, or **Lù Duān/Rui Shi** as secondary threats; **Gūdǎn** and **Libertos** stop opponents simply running around a predictable HI block. CanCon guests said inexpensive Gūdǎn forward camouflage, Shock Mines and templates materially improved the protection of their main team.
4. **Allocate 10 vs 15 troopers deliberately:** Extra Tactical Awareness and LT→NCO activations allow compact IA builds to act like larger groups, but a low model count concentrates risk and coverage. One 5-man attack squad that cannot cross a hacking network is not efficient, regardless of its theoretical order count.
5. **Protect HI from counter-tech:** EVO Pangguling (Fairy Dust when appropriate), link TinBots, Hǎidào KHD/Pitcher, mines and an Engineer/servant are high-value. Firewall on one Fireteam does not protect independent solo troops automatically. Recovery support must be positioned to reach the expensive piece.
6. **Fireteam legality matters:** Current chart records **Core 1 / Haris 1 / Duo source value 256 (unlimited)**. In **Invincible**, both Zúyǒng and Shàng Jí rows carry required=true with min=0; **Shock Duo** similarly marks both Mówáng and Gūijiă required=true with min=0. The source is ambiguous: don't infer any arbitrary pair works without checking the current Army builder. **Forward Duo** requires Húláng FTO-2, optionally Krit FTO-2 and explicitly bans Wildcards. Only **FTO** Son-Bae/Pangguling profiles have Wildcard access.

### Short unit choices: why / tradeoff

| Unit or team | Why it works | Competing view / limit |
|---|---|---|
| **Dāoyīng LT** | Camo/Mimetism(-3), WIP14, +1 LT Order fuel NCO pressure and keep an LT harder to reach; late hacker/sniper can finish objectives. | An experienced opponent suspects Dāoyīng is LT. The hacker becomes vulnerable when revealed. |
| **Shàng Jí AP HMG / TinBot** | 45 pts, AP HMG, 2W, ARM4/BTS6, Tactical Awareness on every current Shàng Jí profile. A solid primary gun and hacking-protection anchor in an eligible link. | BS13 and no innate Mimetism: a good plan needs angles/counter-vision, not a frontal fight with every Mimetism-6 target. |
| **Zúyǒng** | 26-pt MULTI Rifle Paramedic scores under fire; 27-pt Tactical Awareness with Firewall(-6) adds a cheap HI Order, and HMG TacAware can substitute for a more expensive weapon. Number 2 helps preserve Fireteam value. | Strongest primarily as link glue/specialist, not an excuse to make every member carry heavy weapons. |
| **Hǎidào** | 22-pt **KHD + Pitcher** extends network and fights enemy hackers; 25-pt Engineer repairs; MSV2 MULTI Sniper handles difficult camo ARO lanes. Flexible Wildcard means its role travels with the key team. | You must select among roles. Tactical Awareness especially likes KHD/Pitcher; Swiss Miss emphasizes general link utility. A Hac Tao hacker is a different, much more expensive threat. |
| **Krit / Tai Sheng / Bìxié** | Krit is an NCO Engineer with normal FTO weapons or Forward FTO-2 Minelayer/repeater; Tai Sheng adds NCO + FO + Sixth Sense, optional CoC/TinBot; Bìxié contributes climbing, melee and fast mission play. | All premium Wildcards. CanCon players differ about Tai's efficient ranged pressure vs Krit's repairs vs Bìxié's anti-visor and melee utility. Select the missing capability. |
| **Mówáng** | 42–44 pts, Mimetism(-3), ARM5, BTS6, NWI, Flammenspeer; NCO Red Fury **Disco Baller** gives LoF-denial tools for safe approach; independent attack and Suppressive Fire without a large link. | Tactical Awareness enjoys paired Mówáng; Swiss Miss prefers its standalone value. A second Mówáng competes against objectives/attack diversity. |
| **Yān Huǒ** | BS14, ARM5, Immunity(ARM): **HRMC** is a powerful active-turn cannon; **Neurocinetics(+1B) Missile** is a painful solo ARO; **FTO +1B Missile/Mine Dispenser** belongs in eligible Invincible teams. | S5/slow, BTS3, hacking/E/M and poor hiding. Tactical Awareness tries multi-Yān Huǒ walls; Swiss Miss is favorable on guns but questions points spent on static AROs. |
| **Zhēnchá** | Infiltration, Camo, durable NWI specialist, KHD/Trinity or Minelayer(2): solves missions independently of the main HI link. | Minelayer(2) is not automatically a specialist. A KHD Zhēnchá may do objective/network work more efficiently than a 58-pt Hac Tao hacker, but cannot match Hac Tao long-range durability. |
| **Húláng / Gūdǎn / Libertos** | Húláng forward Mimetism(-6), specialist, Monofilament/D-Charges and E/M or Disco Baller pressures tough defenders; Gūdǎn cheap one-use Camo/Zapper or Heavy Flamethrower and Shock Mine screens HI; Libertos provides cheap disposable Camo/Mine delay. | These are trading/denial tools, not invulnerable assassins. Húláng CC is risky against strong reactive defence. Gūdǎn/Libertos are excellent only when placed where opponents must cross them. |
| **Liú Xīng / Hac Tao** | Liú Xīng explosive Combat Jump (PH14), 24-pt baseline or 30-pt mission/hacker profiles punish exposed objectives/DZ and force deployment respect; EVO Control Jump can help. Hac Tao hidden Mimetism(-6) NCO HMG offers independent long-range surprise. | Some Tactical Awareness speakers prefer cheaper Zhēnchá KHD to Hac Tao hacker; others value Hac Tao's two-Wound/ARM5 threat. Liú Xīng must avoid unsupported drops under layered ARO. |
| **Léi Gōng / Qiang Gāo / Jeong** | Léi Gōng Albedo(-6)/MSV1/Super-Jump answers enemy visors; Qiang's Warhorse, Immunity(IMM-B), ECM(-3) and BS Attack(-3) is specialist anti-hacking/E-M matchup tech; Jeong adds Engineer/turret/repeater zone control. | Swiss Miss doubts the efficiency of these expensive pieces over Shàng Jí/Hǎidào/Krit; Tactical Awareness is more interested in Qiang's unusual immunities and Léi Gōng's mobility. |

### TAG, vehicle and shared Yu Jing REM research

**Source-correct availability:** The main IA roster contains **one TAG family — Gūijiă (AVA 2)** and **no VH-class vehicles**. Sù-Jiàn and Fēiquán appear in other Yu Jing sectorials, **not** this IA roster. Gūijiă's Shàngdiào ancillary is a specialist companion, not a separate TAG. Shared Yu Jing REM profiles should be assessed with IA Fireteam access, not copied wholesale from Vanilla.

| Unit | Best use and why | Weakness / opposing opinion |
|---|---|---|
| **Gūijiă TAG**, 77 pts / BS14 / ARM8 / STR3 / MULTI HMG / Heavy Flamethrower / DA CCW / Super-Jump / TacAware | Heavy-range shooter with AP MULTI-HMG options, an unusually credible CC deterrent (CC22/MA2/DA), and Shàngdiào ancillary specialist. A supported TAG can survive bad rolls and take aggressive close lanes. Include an Engineer and a second independent mission piece. | **Disagreement:** Swiss Miss reports success and calls CC utility underrated; Tactical Awareness hosts question a 77-pt investment when Shàng Jí/Mówáng are cheaper, often Prone-capable, and spread objectives better; Loss of Lieutenant's TAG comparison rates Gūijiă in the middle due to its cost for CC rather than elite gunfighting. **Current Gūijiă has GizmoKit; it does not have Remote Presence.** Shock Duo legality remains subject to the chart's unusual required flags. |
| **Rui Shi** (23-pt MSV2 Spitfire / 21-pt MSV1 Red Fury + Mine Dispenser) | **Can join Invincible Fireteam** unlike many attack REMs; MSV2 pressures Mimetism, EVO Assisted Fire/Marksmanship improves active shooting, and cheaper Red Fury mines force enemies to clear approaches to a Mówáng or objective. CanCon players praised mine control; N5 Bakunin battle report shows EVO-backed Rui Shi. | Fragile ARM1/1 STR. Do not leave it trading prolonged AROs; choose Spitfire for vision-based shooting or Mine Dispenser for area denial. |
| **Lù Duān** (24-pt Mk12/HFT/E-M Mine, 20-pt Thunderbolt/E-M Carbine/Mine) | Holographic echoes/Surprise Attack(-3), +1B and mines: expendable **secondary assault** that can trigger/clear enemy mines or create E/M area denial while the main HI link spends its Orders elsewhere. The CanCon podium review explicitly values this secondary role. | No IA Fireteam access; ARM1/1 STR. Swiss Miss is uncertain whether it outcompetes another cheap specialist, while tournament speakers defend its separate job. |
| **Pangguling** (8-pt Baggage/repeater; 14-pt EVO; 17-pt TR; 12-pt FTO Wildcard) | Cheap Order and **reload** for Flammenspeers, mine dispensers and Disco Ballers; EVO programs can support Rui Shi, Liú Xīng, and HI Firewall via Fairy Dust. | Pick EVO only when the list uses its programs; only **option 4 FTO** is the Wildcard, never assume the plain EVO or 8-pt Baggage is linkable. |
| **Chaīyì / Wèibīng** | 7-pt Chaīyì Flash Pulse Repeater brings cheap Regular order and screen; Wèibīng brings FO, Sensor, Repeater, optional 17-pt TacAware for discovering Camo and establishing Spotlight/mission options. | Wèibīng is **unlinked** in IA. Swiss Miss ranks it below embedded HI specialists; network-oriented lists value its Sensor and FO more. |
| **Hùsòng / Son-Bae** | Hùsòng Total Reaction HMG or 18-pt Thunderbolt(+1B) protects DZ lanes; Son-Bae 16-pt Guided can capitalize on Spotlight, while 19-pt **FTO Missile(+1B)** is a Wildcard for long-range ARO. | Build **overlapping** angles, not a single exposed stationary ARO. Son-Bae guided loadout is not the linked FTO loadout; only **option 2** is Wildcard. |
| **Mech-Engineer / Jeong / Hǎidào Engineer / Krit / Yáozăo / Qíshì** | Choose recoverability that suits your primary piece: embedded Hǎidào/Krit repairs a moving HI team, servants extend repair reach, Jeong/turrets defend approach, and Qíshì TAG-support pilot can accompany a Guijia plan. | A repairer unable to reach the TAG/HI is wasted. Don't over-invest in Engineers instead of having enough Orders and objective specialists. |

**Four concise list skeletons (not verified Army codes):** (A) Dāoyīng + **Shàng Jí AP HMG/TinBot** + **Krit NCO Engineer** + **Hǎidào KHD/Pitcher** + Zúyǒng Paramedic + Gūdǎn; (B) Dāoyīng → **Mówáng NCO Disco Baller** with Rui Shi Mine Dispenser, Zhēnchá specialist, cheap order screens; (C) **Yān Huǒ FTO Missile + Invincible protection**, supporting Hùsòng/Pangguling and a *real* forward specialist; (D) **Gūijiă + Engineer/servant + Shàngdiào/Qíshì** with an independent anti-hacking and midfield mission plan. Confirm Fireteam legality and combat groups before treating any skeleton as an actual list.

### Disagreements worth retaining

- **Strong faction vs predictable HI:** **CanCon 2025 second/third place** demonstrates high-level results with purposeful Gūdǎn, mines, mobile objective play and defensive overlap. Swiss Miss sees broad viable N5 options. Shepherd's explicitly N4 skepticism about being outperformed by Vanilla/White Banner is *historical* and should not replace 2025 evidence.
- **Gūijiă vs smaller HI attackers:** Some like its ARM8, CC and MULTI HMG; others would trade its 77 pts for multiple Shàng Jí/Mówáng, a specialist and a separate angle. Main issue is **single-piece concentration**, not whether the TAG is useless.
- **Link concentration vs distributed NCO/Duos:** One large TacAware link can push a lane hard; smaller threats plus Zhēnchá/Gūdǎn score through different lanes and force less predictable decisions.
- **Yān Huǒ ARO bunker vs mobile scoring:** Multiple ML/HRMC are oppressive on open tables, but low mobility and expensive static pieces can lose objective missions to smoke, hacking, mine bypass and forward scoring.
- **Hac Tao hacker vs Zhēnchá hacker:** N5 podcast guests dispute the price premium: Hidden Deployment and durable BS14 armour are real, but infiltration gives earlier buttons and more affordable Trinity.
- **EVO/repair investment:** Valuable in Rui Shi, Liú Xīng, Gūijiă, firewall-heavy lists; not automatically worth its costs if the list only wants generic heavy infantry guns.

### Sources / transcript audit

| Priority | Video or podcast | What was actually reviewed |
|---|---|---|
| **Best tournament tactics** | [Infinity Dante — Invincible Army Mega-sode: CanCon podium lists](https://www.youtube.com/watch?v=rJJ4PamI-hE) (Feb 2025) | **Full YouTube MCP transcript**: Peter Henry and Jacob Ridley discuss mission-specific lists, Gūdǎn defence, links, secondary Lù Duān, mines, hack protection, and ARO tradeoffs. |
| **Best detailed N5 unit guide** | [Swiss Miss Gaming — N5 Tier List: Invincible Army](https://www.youtube.com/watch?v=SvycUWMYKr4) (Nov 2025) | **Full YouTube MCP transcript**, unit-by-unit reasoning; opinions not source rules. |
| **Best contrasting lists** | [Tactical Awareness S3 Ep20 — Invincible Army](https://open.spotify.com/episode/4uGhKYeMBabBftl1gwXhpS) (19 May 2025) | **Full Podcast MCP transcript**, discussing three+ list approaches, NCO/Mówáng, Yān Huǒ ARO saturation, Hǎidào Pitchers, Fireteam composition, EVO, TAG skepticism. |
| **Best TAG comparison** | [Loss of Lieutenant Ep142 — N5 TAG Tier List](https://open.spotify.com/episode/1h5CJfZC5zBPxdg66o7xIN) (6 Apr 2025) | **Podcast MCP transcript**, direct Gūijiă comparison and price/Remote Presence debate. |
| **Best TAG support fundamentals** | [Loss of Lieutenant Ep141 — Tactical Armored Gear](https://open.spotify.com/episode/6zPRTbn2cilgMyuHtODvf7) (31 Mar 2025) | **Podcast MCP transcript**, tag defensive deployment, hackers, repair, EVO support. |
| **On-table EVO/REM example** | [MiniWarGaming — Invincible Army vs Bakunin](https://www.youtube.com/watch?v=fis91SB7oqA) (22 Jan 2025) | **Full YouTube MCP transcript**, Rui Shi Mine Dispenser/Assisted Fire and Yān Huǒ HRMC. |
| **On-table AD/hacker example** | [MiniWarGaming — Invincible Army vs JSA](https://www.youtube.com/watch?v=FB_Dd43SI-s) (16 Jul 2025) | **Full YouTube MCP transcript**, Zhēnchá KHD, Fairy Dust/Control Jump and Liú Xīng. |
| **Related faction context** | [Robert Shepherd — N5 Yu Jing](https://www.youtube.com/watch?v=mn4yHSNxsnA) (25 Apr 2025) | **YouTube MCP transcript previously reviewed**, common Yu Jing HI/TAG context; Vanilla availability does not imply IA eligibility. |
| **Historical N4 only** | [Robert Shepherd — Faction Focus: Invincible Army](https://www.youtube.com/watch?v=Lco3q6QmezY) (25 Jun 2024) | **YouTube MCP transcript checked**; repository's earlier archive: [Invincible Army.txt](../../rules/Youtube%20factions/Invincible%20Army.txt). Old power-level verdict is not a current N5 opinion. |
| **Reference index** | [Corvus Belli community Yu Jing N5 tacticas](https://forum.corvusbelli.com/threads/n5-recap-yu-jing-tacticas.43474/) / [CanCon results and reviews](https://forum.corvusbelli.com/threads/tournament-cancon-2025-recap-articles-videos.43362/) | External corroboration of dates and guests; not treated as replacement for full transcripts. |

**Future source refresh:** Reconcile new Army data/FAQ with the N5.3 tables **before** revising tactical details. Separate current roster facts, attributed N5 opinions, and N4-era claims.

## Validation and refresh notes

Validation performed for this reference:

- Main roster: **34 ordinary matched-play units**, plus 2 separately identified optional-mode units.
- Main Fireteam chart: 4 named Fireteam families plus the Wildcard table.
- Main chart limits preserved as `Core 1 / Haris 1 / Duo 256`; repository/InfinityDB convention maps raw `256` to unlimited Duo availability.
- All source `min`, `max`, `required`, Counts-as comments, and FTO/FTO-2 restrictions were preserved explicitly.
- The unusual dual-`required` rows in **Invincible** and **Shock** Fireteams were retained literally rather than normalized by inference.
- Forward Fireteams retain the source restriction **No Wildcards Special Fireteam**.
- Dàebàk is retained as a distinct 13-unit Reinforcement roster with its own separate Fireteam chart.
- Stable Army option IDs are used throughout the main-roster loadout tables.

Refresh this file when any of the following changes:

1. Army source version or the Invincible Army / Dàebàk source blobs change.
2. InfinityDB changes Fireteam normalization or Counts-as/FTO semantics.
3. The repository rules baseline moves beyond N5.3 or a new FAQ changes relevant rules.
4. `sectorials/REFERENCE_DESIGN.md` advances to a new schema version.

## TAG tactical cross-reference (2026-10-23)

**Gūijiă** provides a true big-gun/armor alternative to linked HI; prefer it where its 3-STR TAG survivability, firing lane and **Shock** Fireteam access beat spending Orders on yet another HI gun. Count the full companion/Engineer/support cost, and protect it from hacking/E/M rather than relying on high ARM alone.

Across all factions, compare **apex power** separately from **points value**, counterplay and mission fit: [N5.3 TAG guide](../../notes/list-building/tags.md). The current unit profiles and canonical Fireteam chart above take precedence over tactical opinions.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Hǎidào KHD + Pitcher 22/0** is the principal 0-SWC anti-Hacker/scoring support in a **TinBot-protected HI Fireteam**; **Dāoyīng Camouflaged HD/LT** supplies protected command and an alternative anti-HI program package. **Hac Tao Hidden HD+Trinity 58/0.5** is the premium protected killer/anti-heavy ambush but has a steep cost; **Zhēnchá HD+Trinity 34/0.5** supplies forward Camo surprise and a cheaper hybrid. **Liú Xīng HD + Firewall(-6) 30/0.5** can attack distant objectives via Combat Jump; **Shàng Jí HD 40/0.5** comes with a real HI fight/Order economy. **Why:** several hackable HI magnify the payoff from TinBot, KHD, anti-repeater clearance and **one HD with Oblivion**, not just more KHDs.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

See [Cheerleaders and Order Generators — N5.3 apex, points-value and matchup guide](../../notes/list-building/cheerleaders-and-order-generators.md) for complete comparative tables and verified transcript disagreements. The **current roster above controls** legality, AVA, Training and Fireteams.

- 7pt Chaīyì — Flash/Repeater Regular REM when AVA permits; S3 footprint and fragility limit repeats.
- Zhanshi — Regular S2 line with Fireteam/decoy utility; compare actual 7pt Flashbot and specialist upgrades before choosing expensive passive profiles.
- Warcor — 3pt Irregular Flash Pulse distraction, not a transferable Regular Order.

**Order audit:** add up only deployed eligible **Regular** Orders in each Combat Group; special LT/Tactical, Irregular and Peripheral activations are not transferable pool Orders. Buy the cheapest protected body that supplies the *second function the list truly needs*; consider large-base DZ crowding, expensive mandatory Fireteam slots, and whether another scoring specialist beats one more cheap Order.
