---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 504
sectorial_slug: tunguska
sectorial_name: Tunguska
parent_faction: Nomads
rules_baseline: N5.3
army_source_version: "7.26246.158"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Tunguska roster, standard loadouts, canonical Fireteam chart, and reverse Fireteam index. Vortex Spec-Ops and Nomads Team-Ops are optional-mode hooks rather than ordinary matched-play roster entries."
---

# Tunguska

## Overview and provenance

Repository-native reference for **Tunguska** roster, profiles, points/SWC, AVA, and Fireteam access.

For concise transcript-reviewed tactics, Fireteam/list-building roles, **Szalamandra and Anaconda TAGs, Go-Pod VH, REMs** and explicit opposing opinions, see [Tunguska — N5.3 Tactical and List-Building Guide](../../notes/factions/tunguska.md). **This reference remains authoritative** for current profile costs, options, dependency rules and Fireteam legality.

Sources used:

- Army-derived Tunguska source revision `7.26246.158` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- Source blob: `b78b327b90aed6bafba9fa3cccb05ae2cc35dfa0`.
- InfinityDB Fireteam normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **44-unit standard Tunguska roster** and the complete Tunguska `fireteamChart` in the pinned Army source.
- `Vortex Spec-Ops` and `Nomads Team-Ops` are optional game-mode content and are listed separately.
- Soldier of Fortune / generic mercenary-catalog entries whose source faction list is empty are excluded from the base roster.
- Fireteam legality comes from the canonical chart below, not from an `FTO` loadout name by itself.
- Parenthetical Army-chart comments such as `(Securitate)`, `(Spetskorp)`, `(Hollow men)`, `(Bounty Hunters)`, and `(Nayemnik)` are preserved as source equivalence/context labels; they are not silently expanded beyond the chart.
- Structured `required: true` rows in Spetskorp, VATRA, Bounty Hunters, and Nayemnik are preserved as required-choice sets; this reference does not reinterpret every marked row as simultaneously mandatory.
- FTO/profile restrictions are preserved: Switcher access uses FTO profiles only; Fiddler joins Spetskorp/Nayemnik only through the FTO profile; Stempler joins Hollow Men/Nayemnik only through its FTO profile; Vostok and Tsyklon Wildcards are FTO-only; Raoul Spector's Wildcard access is FTO-only and limited to Spetskorp/Nayemnik; Sforza's Wildcard access is FTO-only and tied to the Bounty Hunter context.
- PuppetBots are dependent on the Puppet Master profile group in the source relation table.
- Linked Reinforcement army ID: **599**. Reinforcement Fireteams are not merged into the main chart here.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Tunguska |
| Parent faction | Nomads |
| Army ID | 504 |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster units | 44 |
| Optional-mode units | Vortex Spec-Ops; Nomads Team-Ops |
| Reinforcement roster | Army ID `599` |
| Fireteam limits | Core 1; Haris 1; Duo unlimited |
| Fireteam chart | yes |

## Roster index

`AVA 255` is Army's Total/unlimited sentinel.

| Unit | ID | AVA | Type | Order | Fireteam access |
|---|---:|---:|---|---|---|
| Grenzers | 393 | 5 | MI | Regular | Securitate; Spetskorp; Hollow Men; VATRA; Bounty Hunters |
| Clockmakers | 406 | 2 | LI | Regular | — |
| Hollow Men | 1092 | 5 | HI | Regular | Hollow Men |
| Zondbots | 425 | 2 | REM | Peripheral | — |
| Szalamandra Squadron | 420 | 2 | TAG | Regular | — |
| TAG-Treiber | 1853 | 1 | LI | Regular | Securitate |
| Switchers Gruppa | 1848 | 2 | LI | Regular + Tactical Awareness | Securitate; Spetskorp, FTO profiles only |
| Raoul Spector | 1069 | 1 | LI | Irregular or Regular by profile | Wildcard in Spetskorp/Nayemnik, FTO profile only |
| Warcors | 50 | 1 | LI | Irregular | — |
| Vostok Sputniks | 1544 | 2 | REM | Regular | Wildcard, FTO profiles only |
| Fiddler | 1564 | 1 | LI | Regular | Spetskorp; Nayemnik, FTO profile only |
| Mobile Brigada | 382 | 1 | HI | Regular | Bounty Hunters |
| Father Lucien Sforza | 198 | 1 | MI | Regular | Wildcard in Bounty Hunter context, FTO profiles only |
| Spektrs | 402 | 3 | SK | Regular | — |
| Tunguska Interventors | 407 | 4 | LI | Regular | Securitate |
| Casino Security Rounders | 1762 | 2 | LI | Regular | Securitate |
| Zondnautica | 1091 | 3 | MI + REM | Regular + Impetuous | — |
| Zellenkrieger | 1747 | 2 | WB | Irregular + Impetuous | — |
| Kulak Payback Unit | 1761 | 2 | MI | Regular | Securitate; VATRA |
| Jelena Kovač | 1550 | 1 | LI | Regular + Tactical Awareness | Wildcard; Securitate context |
| Tsyklon Sputniks | 423 | 2 | REM | Regular | Wildcard, FTO profiles only |
| Corregidor Alguaciles | 296 | 2 | LI | Regular | — |
| Transductor Zonds | 412 | 2 | REM | Regular | — |
| Authorized Bounty Hunters | 49 | 3 | LI | Regular | Bounty Hunters |
| Motorized Bounty Hunters | 1565 | 3 | LI | Irregular + Impetuous | Bounty Hunters |
| Go-Pod | 1854 | 1 | VH | Regular | — |
| Kriza Boracs | 954 | 2 | HI | Regular | Hollow Men; VATRA |
| Perseus | 1101 | 1 | WB | Regular | Securitate; Hollow Men; Nayemnik |
| Daktaris | 405 | 1 | LI | Regular | — |
| Vertigo Zonds | 410 | 1 | REM | Regular | — |
| Hecklers | 1095 | 3 | SK | Regular | — |
| Salyut Zonds | 426 | 2 | REM | Regular | — |
| Denma Connolly | 1749 | 1 | WB | Regular + Impetuous | Bounty Hunters |
| Stempler Zonds | 408 | 2 | REM | Regular | Hollow Men; Nayemnik, FTO profile only |
| Tunguska Triggermen | 1855 | 3 | HI | Regular | Wildcard |
| Meteor Zonds | 411 | 1 | REM | Regular | — |
| Puppetactica Company | 1098 | 1 Puppet Master / 3 PuppetBots | LI + REM | Regular / Peripheral | — |
| Tunguska Cheerkillers | 1541 | 5 | LI | Regular | Spetskorp |
| Mary Problems | 1099 | 1 | LI | Regular | — |
| Securitate | 434 | 255 | LI | Regular | Securitate |
| Miranda Ashcroft | 51 | 1 | LI | Regular | Wildcard; Bounty Hunter context |
| Reaktion Zonds | 409 | 1 | REM | Regular | — |
| Anaconda | 300 | 1 | TAG | Regular + Tactical Awareness | VATRA |
| Wolfgang Amadeus Wolff | 1555 | 1 | WB | Regular | Wildcard; Bounty Hunters/Securitate contexts |

Optional-mode units:

| Unit | ID | Mode | Fireteam relevance |
|---|---:|---|---|
| Vortex Spec-Ops | 1917 | Spec-Ops | Securitate Fireteam row, max 1 when Spec-Ops mode is in use |
| Nomads Team-Ops | 1931 | Team-Ops | No ordinary Tunguska Fireteam row |

## Unit details

### Grenzers, Grenz Security Team

**ID 393 · AVA 5 · MI** — `MOV 10-10 | CC 16 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 6 | W 1 | S 2`. MSV1, Courage, Immunity (Shock), Warhorse.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4 | 28 | 1.5 | Missile Launcher, Pistol, Breaker Pistol, CCW | Securitate max 1; Spetskorp required-choice max 5; Hollow Men max 1; VATRA max 1; Bounty Hunters max 1 |
| 5 | 28 | 1 | Red Fury, Pistol, Breaker Pistol, CCW | same |
| 6 | 29 | 0 | Combi Rifle, Light Flamethrower (+1B), Flash Pulse, Pistol, Breaker Pistol, CCW; Forward Observer, Sensor, NCO | same |
| 7 | 28 | 0 | Combi Rifle, Light Flamethrower (+1B), Pistol, Breaker Pistol, CCW; Biometric Visor, Discover (+3) | same |
| 8 | 32 | 1.5 | MULTI Sniper Rifle, Pistol, Breaker Pistol, CCW; Marksmanship | same |
| 9 | 28 | 0 | Combi Rifle, Light Flamethrower (+1B), Pistol, Breaker Pistol, CCW; Biometric Visor, Lieutenant, Discover (+3) | same |

### Clockmakers

**ID 406 · AVA 2 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 15 | ARM 1 | BTS 3 | W 1 | S 2`. Engineer, Deactivator, GizmoKit (+1B).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 18 | 0 | Combi Rifle, D-Charges, Pistol, CCW | — |
| 2 | 19 | 0 | Same; Deployable Cover | — |
| 3 | 21 | 0 | Combi Rifle, D-Charges, Armed Turret (Combi Rifle), Pistol, CCW | — |

### The Hollow Men

**ID 1092 · AVA 5 · HI** — `MOV 15-5 | CC 11 | BS 13 | PH 10 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 2`. Remote Presence, Super-Jump, Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Combi Rifle, Chain-colt, Breaker Pistol, CCW | Hollow Men 1–5 |
| 2 | 26 | 0 | MULTI Rifle, Chain-colt, Pitcher, Breaker Pistol, CCW | same |
| 3 | 28 | 1.5 | Missile Launcher, Chain-colt, Breaker Pistol, CCW | same |
| 4 | 29 | 1.5 | Spitfire, Chain-colt, Breaker Pistol, CCW | same |
| 5 | 24 | 0 | Combi Rifle, Chain-colt, Breaker Pistol, CCW; TinBot Firewall (-3) | same |
| 7 | 29 | 0.5 | Combi Rifle, Chain-colt, Breaker Pistol, CCW; Hacking Device, TinBot Firewall (-3), Hacker | same |
| 8 | 21 | 0 | Boarding Shotgun, Chain-colt, Breaker Pistol, CCW; Specialist Operative | same |

### Zondbots

**ID 425 · AVA 2 · REM** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`. Peripheral (Servant), Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | PARA CCW (-3); Peripheral, no Order | — |

### Szalamandra Squadron

**ID 420 · AVA 2 · TAG** — `MOV 15-10 | CC 17 | BS 14 | PH 16 | WIP 13 | ARM 8 | BTS 9 | W 3 | S 7`. ECM: Guided (-6), BS Attack (SR-1), Dodge (PH=11), GizmoKit (PH=11), NCO; includes a RobbyBot attendant.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 68 | 2 | Hyper-Rapid Magnetic Cannon, Heavy Flamethrower, CCW (PS 5) + RobbyBot | — |

**RobbyBot:** `MOV 15-10 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 1`; Peripheral (Ancillary), Courage, Dodge (+3), Mimetism (-3), Specialist Operative.

### TAG-Treiber, NMF TAG Squadrons Support Pilots

**ID 1853 · AVA 1 · LI** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Specialist Operative, TAGCom (Dodge PH+3 / GizmoKit PH+1).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 3 | 10 | 0 | **SZALAMANDRA PILOT**; Light Shotgun, Cybermine, Pistol, CCW; Killer Hacking Device, Hacker | Securitate max 1 |

### Switchers Gruppa

**ID 1848 · AVA 2 · LI** — base `MOV 10-10 | CC 15 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`; Courage, Transmutation (WIP), Dogged, Tactical Awareness. Enhanced profile: `MOV 15-10 | CC 23 | BS 13 | PH 14 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`; X-Visor, Martial Arts L2, Berserk (+3), Dodge (+5), Immunity (BTS), Dogged, Tactical Awareness.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 25 | 0 | **SWITCHER FTO**; Combi Rifle, E/Mitter, Zapper, Pistol, Viral CCW (PS 5) | Securitate max 1; Spetskorp max 1 |
| 2 | 27 | 0 | **SWITCHER FTO**; Thunderbolt, E/M Carbine, E/M Grenades, Pistol, Viral CCW (PS 5); BS Attack (+1B) | same |
| 3 | 20 | 0 | **SWITCHER FTO**; AP SMG, Flash Pulse (+1B), E/M Grenades, Pistol, Viral CCW (PS 5); Forward Observer | same |
| 4 | 21 | 0 | AP SMG, Flash Pulse (+1B), E/M Grenades, MadTraps, Pistol, Viral CCW (PS 5) | — |

### Raoul Spector, Mercenary Operative

**ID 1069 · AVA 1 · LI** — `MOV 15-5 | CC 22 | BS 12 | PH 13 | WIP 13 | ARM 2 | BTS 3 | W 2 | S 2`. Martial Arts L3, Courage, Mimetism (-6), Specialist Operative, Stealth, Super-Jump (Jet Propulsion), Natural Born Warrior, Dodge (+5), Bangbomb (+4).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 0 | Boarding Shotgun (+1B), Drop Bears (+1SD), Boarding Pistol (PS 6), E/M CCW (PS 6); Parachutist, Combat Jump; Irregular Order | — |
| 3 | 34 | 0 | **SPECTOR FTO**; MULTI Rifle, Drop Bears (+1SD), Boarding Pistol (PS 6), E/M CCW (PS 6); Regular | Wildcard max 1 in Spetskorp/Nayemnik only |

### Warcors

**ID 50 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Journalist.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); 360º Visor | — |
| 2 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW (-3); Sixth Sense | — |

### Vostok Sputniks

**ID 1544 · AVA 2 · REM** — `MOV 15-10 | CC 14 | BS 12 | PH 10 | WIP 13 | ARM 3 | BTS 6 | W 2 | S 4`. Remote Presence, Courage, Immunity (AP), Climbing Plus, Mimetism (-6).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 4 | 38 | 0 | Mk12, Light Shotgun, PARA CCW (-3); Repeater | — |
| 5 | 35 | 0 | **VOSTOK FTO**; Mk12, Light Shotgun, PARA CCW (-3) | Wildcard max 1 |
| 6 | 37 | 1 | Spitfire, PARA CCW (-3); Repeater | — |
| 7 | 34 | 1 | **VOSTOK FTO**; Spitfire, PARA CCW (-3) | Wildcard max 1 |

### Fiddler

**ID 1564 · AVA 1 · LI** — `MOV 15-10 | CC 18 | BS 12 | PH 12 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. GizmoKit, CC Attack (+1B), Dodge (+3), Dodge (+2.5), Engineer, Immunity (Critical), No Wound Incapacitation.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 29 | 0 | **Fiddler FTO**; Contender (+1B), Drop Bears, D-Charges, Breaker Pistol, PARA CCW (-3); Super-Jump | Spetskorp max 1; Nayemnik required-choice max 1 |
| 2 | 36 | 0 | Same weapons; Climbing Plus; includes 1 JackBot | — |
| 3 | 43 | 0 | Same weapons; Climbing Plus; includes 2 JackBots | — |

**JackBot:** `MOV 15-10 | CC 16 | BS 11 | PH 10 | WIP 12 | ARM 0 | BTS 3 | W 1 | S 1`; Vulkan Shotgun, Peripheral (Synchronized), Courage, Explode, Climbing Plus.

### Mobile Brigada

**ID 382 · AVA 1 · HI** — `MOV 15-5 | CC 18 | BS 13 | PH 13 | WIP 13 | ARM 5 | BTS 3 | W 2 | S 2`. 360º Visor, Courage, Jump (7.5).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 0 | MULTI Rifle, Boarding Pistol (+1B), CCW; TinBot Firewall (-6) | Bounty Hunters max 1 |
| 2 | 38 | 1.5 | HMG, Boarding Pistol (+1B), CCW | same |
| 3 | 27 | 0 | Boarding Shotgun, Boarding Pistol (+1B), CCW | same |
| 5 | 35 | 1.5 | Missile Launcher, Boarding Pistol (+1B), CCW | same |
| 9 | 36 | 0.5 | Combi Rifle, D-Charges, Boarding Pistol (+1B), CCW; Hacking Device, TinBot Firewall (-6), Hacker | same |
| 10 | 33 | 0 | MULTI Rifle, Boarding Pistol (+1B), CCW; TinBot Firewall (-6), Lieutenant | same |
| 11 | 27 | 0 | Boarding Shotgun, Boarding Pistol (+1B), CCW; Lieutenant | same |

### Father Lucien Sforza

**ID 198 · AVA 1 · MI** — `MOV 10-10 | CC 19 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. X-Visor, BS Attack (+1SD), Immunity (ARM), Combat Instinct, Stealth, NCO, Dogged, Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 0 | Viral Rifle, Adhesive Launcher Rifle, Nanopulser, Heavy Pistol, PARA CCW (-9); Holoprojector, Surprise Attack (-3), Forward Deployment (+10) | — |
| 2 | 23 | 0 | **SFORZA FTO**; Viral Rifle, Adhesive Launcher Rifle, Nanopulser, Heavy Pistol, PARA CCW (-9) | Wildcard max 1 in Bounty Hunter context |
| 3 | 26 | 0 | **SFORZA FTO**; same weapons; Albedo (-6) | same |

### Spektrs

**ID 402 · AVA 3 · SK** — `MOV 10-10 | CC 13 | BS 12 | PH 12 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Surprise Attack (-3), Camouflage, Hidden Deployment, Infiltration, Mimetism (-6), Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 3 | 32 | 1.5 | MULTI Sniper Rifle, Shock Mine, Silenced Pistol, CCW | — |
| 4 | 28 | 0 | SMG, E/M Mine, Silenced Pistol, CCW; Deployable Repeater | — |
| 5 | 35 | 0.5 | Combi Rifle, D-Charges, Silenced Pistol, CCW; Hacking Device, Hacker | — |
| 6 | 30 | 0 | SMG, Cybermine, D-Charges, Silenced Pistol, CCW; Killer Hacking Device, Hacker | — |
| 7 | 29 | 0 | Boarding Shotgun, Shock Mine, Flash Pulse, Silenced Pistol, CCW; Forward Observer | — |
| 8 | 32 | 0.5 | Boarding Shotgun, D-Charges, Silenced Pistol, CCW; Hacking Device, Hacker | — |
| 9 | 33 | 1 | Combi Rifle, D-Charges, E/M Mine, Shock Mine, Silenced Pistol, CCW; Minelayer | — |

### Tunguska Interventors

**ID 407 · AVA 4 · LI** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 15 | ARM 1 | BTS 9 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0.5 | Combi Rifle, Pistol, CCW; Hacking Device Plus, Hacker | Securitate max 3 |
| 2 | 23 | 0.5 | Same; FastPanda | same |
| 3 | 18 | 0.5 | Boarding Shotgun, Pistol, CCW; Hacking Device Plus, Hacker | same |
| 4 | 20 | 0.5 | Same; FastPanda | same |
| 5 | 21 | 0.5 | Combi Rifle, Pistol, CCW; Hacking Device Plus, Lieutenant, Hacker | same |
| 6 | 23 | 0.5 | Same; FastPanda | same |
| 7 | 18 | 0 | Boarding Shotgun, Pistol, CCW; Killer Hacking Device (Upgrade: Trinity -3), FastPanda, Hacker | same |

### Casino Security Rounders

**ID 1762 · AVA 2 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Biometric Visor, MSV1, Marksmanship, NCO, Terrain (Zero-G).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 17 | 0 | Boarding Shotgun, Boarding Pistol, CCW | Securitate max 1; counts as Securitate |
| 2 | 24 | 0.5 | MULTI Marksman Rifle, Boarding Pistol, CCW | same |
| 3 | 26 | 1 | Red Fury, Boarding Pistol, CCW | same |
| 4 | 21 | 0.5 | SMG, Boarding Pistol, CCW; Hacking Device (Upgrade: Trinity), Hacker | same |

### Zondnautica Rapid Offensive Unit

**ID 1091 · AVA 3 · MI + REM** — mounted Zondnaut: `MOV 20-10 | CC 15 | BS 12 | PH 12 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 4`; AI Motorcycle, Courage, Mimetism (-3), Impetuous, Limited Cover, Transmutation (Auto). Dismounted profile: `MOV 10-10 | PH 11 | ARM 2 | S 2`; includes a ZondMate peripheral.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 25 | 1.5 | **ZONDNAUTICA-A**; mounted Spitfire, Chain Rifle, Smoke Grenade Launcher, Pistol, CCW; dismounted Spitfire; ZondMate | — |
| 2 | 17 | 0 | **ZONDNAUTICA-B**; mounted Boarding Shotgun, Chain Rifle, Smoke Grenade Launcher, Pistol, CCW; dismounted Boarding Shotgun; ZondMate | — |
| 3 | 23 | 0.5 | **ZONDNAUTICA-C**; mounted Combi Rifle, Chain Rifle, Smoke Grenade Launcher, Flash Pulse, Pistol, CCW; dismounted Combi Rifle + Flash Pulse; Hacking Device, Hacker; ZondMate | — |

**ZondMate:** `MOV 20-10 | CC 13 | BS 10 | PH 10 | WIP 11 | ARM 1 | BTS 3 | W 1 | S 5`; Chain Rifle, Smoke Grenade Launcher, PARA CCW (-3), Peripheral (Synchronized), Mimetism (-3), Courage, Transmutation (Auto).

### Zellenkrieger

**ID 1747 · AVA 2 · WB** — `MOV 10-10 | CC 23 | BS 10 | PH 13 | WIP 12 | ARM 1 | BTS 3 | W 1 | S 2`. CC Attack (-3), Berserk, Courage, Dodge (+2.5), Natural Born Warrior, MetaChemistry (ReRoll), No Cover, Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | Light Shotgun, Smoke Grenades, Heavy Pistol, DA CCW (PS 7) | — |
| 2 | 8 | 0 | Pulzar, Smoke Grenades, Heavy Pistol (+1B), DA CCW (PS 7) | — |

### Kulak Payback Unit

**ID 1761 · AVA 2 · MI** — `MOV 10-10 | CC 18 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. BS Attack (Shock), Immunity (Shock), Mimetism (-3), Terrain (Total), Religious Troop.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 20 | 1 | Heavy Rocket Launcher, Pulzar (+1B), MULTI Pistol, CCW | Securitate max 1; VATRA max 1 |
| 3 | 23 | 0 | Boarding Shotgun (+1B), D-Charges, Pistol, CCW; Chain of Command | same |
| 5 | 20 | 0 | AP SMG, D-Charges, Cybermine, Disco Baller, Pistol, CCW; Killer Hacking Device (Upgrade: Carbonite), Hacker | same |
| 6 | 19 | 0 | Boarding Shotgun (+1B), Flash Pulse, D-Charges, Pistol, CCW; Forward Observer | same |
| 7 | 21 | 0 | Combi Rifle (+1B), Pulzar, Pistol, CCW | same |

### Jelena Kovač, Securitate DI

**ID 1550 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. X-Visor, Triangulated Fire, Specialist Operative, Sensor, Tactical Awareness, Warhorse.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | Breaker Combi Rifle, Chain-colt, Pistol, CCW | Wildcard max 1; Securitate context |
| 2 | 21 | 0 | MULTI Rifle, Chain-colt, Pistol, CCW | same |

### Tsyklon Sputniks

**ID 423 · AVA 2 · REM** — `MOV 15-10 | CC 14 | BS 12 | PH 10 | WIP 13 | ARM 3 | BTS 6 | W 1 | S 4`. Repeater, 360º Visor, X-Visor, Remote Presence, Courage, Climbing Plus.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 26 | 1 | **TSYKLON FTO**; Spitfire, Chain Rifle, Pitcher, PARA CCW (-6) | Wildcard max 2 |
| 2 | 29 | 1 | **TSYKLON FTO**; Feuerbach, Chain Rifle, Pitcher, PARA CCW (-6) | same |
| 4 | 31 | 1 | Feuerbach, Chain Rifle, Pitcher, PARA CCW (-6); Forward Deployment (+10) | — |
| 5 | 31 | 1 | Spitfire, Chain Rifle, Pitcher, CrazyKoala, PARA CCW (-6); Forward Deployment (+10), Minelayer (2) | — |

### Corregidor Alguaciles

**ID 296 · AVA 2 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 10 | 0 | Combi Rifle, Pistol, CCW | — |
| 2 | 18 | 1 | HMG, Pistol, CCW | — |
| 5 | 15 | 1.5 | Missile Launcher, Pistol, CCW | — |
| 6 | 15 | 0.5 | Combi Rifle, Pistol, CCW; Hacking Device, Hacker | — |
| 8 | 12 | 0 | Combi Rifle, Flash Pulse, Pistol, CCW; Deployable Repeater, Forward Observer | — |
| 9 | 12 | 0 | Combi Rifle, Pistol, CCW; MediKit, Paramedic | — |
| 10 | 10 | 0 | Combi Rifle, Pistol, CCW; Lieutenant | — |
| 11 | 12 | 0 | Combi Rifle, Pistol, CCW; Commlink (+1), Specialist Operative | — |

### Transductor Zonds

**ID 412 · AVA 2 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Repeater, Remote Presence, Courage, Mimetism (-3).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 7 | 0 | Flash Pulse, PARA CCW (-3) | — |

### Authorized Bounty Hunters

**ID 49 · AVA 3 · LI** — `MOV 10-10 | CC 16 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Booty (ReRoll), Stealth.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 12 | 0 | Boarding Shotgun, Pistol, PARA CCW (-6), Heavy Riotstopper | Bounty Hunters required-choice max 3 |
| 3 | 19 | 0.5 | Sniper Rifle, Breaker Pistol (+1B), PARA CCW (-6) | same |
| 4 | 21 | 1 | Spitfire, Boarding Pistol, PARA CCW (-6) | same |
| 5 | 12 | 0 | SMG, Akrylat-Kanone, Breaker Pistol, PARA CCW (-6) | same |

### Motorized Bounty Hunters

**ID 1565 · AVA 3 · LI** — `MOV 20-15 | CC 17 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 4`. Motorcycle, Booty (ReRoll), Limited Cover, Dodge (+5), Mimetism (-3), Impetuous.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 8 | 0 | Boarding Shotgun, Pistol, PARA CCW (-6), Heavy Riotstopper | Bounty Hunters required-choice max 3 |
| 2 | 9 | 0 | SMG, Chain-colt (+1B), Pistol, PARA CCW (-6) | same |
| 3 | 16 | 0.5 | Red Fury, Breaker Pistol, PARA CCW (-6) | same |

### Go-Pod

**ID 1854 · AVA 1 · VH** — `MOV 20-5 | CC - | BS 13 | PH 13 | WIP 13 | ARM 2 | BTS 6 | W 2 | S 7`. BS Attack (-3), BS Attack (+1B), Aerial, Courage, Dodge (-3), Mimetism (-3), No Cover, Super-Jump (Jet Propulsion), Terrain (Total), Super-Jump (7.5), Tech-recovery; includes a Go-Bot.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 0 | MULTI Rifle, E/Mitter + Go-Bot | — |
| 2 | 32 | 1.5 | Heavy Rocket Launcher, AP SMG; BS Attack (SR-1) + Go-Bot | — |

**Go-Bot:** `MOV 20-5 | BS 5 | PH 11 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`; Flash Pulse, Chain-colt, Peripheral (Synchronized), Mimetism (-3), Courage, No Cover, Aerial, Super-Jump, Tech-recovery.

### Kriza Boracs, Special Crisis Unit

**ID 954 · AVA 2 · HI** — `MOV 10-10 | CC 19 | BS 13 | PH 13 | WIP 13 | ARM 5 | BTS 6 | W 2 | S 5`. BS Attack (+1B), BS Attack (-3), Courage, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 45 | 1.5 | HMG, Heavy Pistol, CCW | Hollow Men max 2; VATRA required-choice max 2 |
| 3 | 48 | 0 | Mk12, SMG, Heavy Pistol, CCW; 360º Visor | same |
| 5 | 45 | 1.5 | HMG, Heavy Pistol, CCW; Lieutenant | same |

### Perseus, Rogue Myrmidon

**ID 1101 · AVA 1 · WB** — `MOV 10-10 | CC 23 | BS 13 | PH 13 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. Frenzy, Martial Arts L3, Courage, Dodge (+2.5), Mimetism (-6), Stealth, No Wound Incapacitation, BS Attack (+1B), Super-Jump.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 34 | 0 | MULTI Rifle, Nanopulser, Smoke Grenades, AP Heavy Pistol, DA CCW (PS 5) | Securitate max 1, counts as Securitate; Hollow Men max 1, counts as Hollow Men; Nayemnik required-choice max 1 |
| 3 | 33 | 0 | Breaker Combi Rifle, Nanopulser, Smoke Grenades, AP Heavy Pistol, DA CCW (PS 5) | same |

### Daktaris

**ID 405 · AVA 1 · LI** — `MOV 10-10 | CC 14 | BS 11 | PH 10 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Doctor, MediKit.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 14 | 0 | Combi Rifle, Pistol, CCW | — |

### Vertigo Zonds

**ID 410 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage, BS Attack (Guided).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 16 | 1.5 | Missile Launcher, PARA CCW (-3) | — |

### Hecklers

**ID 1095 · AVA 3 · SK** — `MOV 10-10 | CC 15 | BS 12 | PH 11 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Surprise Attack (-3), Camouflage (1 Use), Forward Deployment (+10), Mimetism (-3), Stealth, Terrain (Zero-G).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 23 | 0 | Combi Rifle, Jammer, Pistol, CCW; FastPanda | — |
| 2 | 20 | 0 | Boarding Shotgun (+1B), E/Marat, Pistol, CCW | — |
| 3 | 24 | 1 | Red Fury, Pistol, CCW | — |
| 4 | 23 | 0 | Combi Rifle, Cybermine, Assault Pistol, CCW; Killer Hacking Device, Hacker | — |

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
| 1 | 12 | 0 | Chain Rifle (+1B), Smoke Grenades, Heavy Pistol (+1B), AP+DA CCW (PS 6) | Bounty Hunters max 1 |

### Stempler Zonds

**ID 408 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Deactivator, Repeater, Remote Presence, Triangulated Fire, Courage, Forward Observer, Sensor, Climbing Plus.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 15 | 0 | Combi Rifle, Flash Pulse, PARA CCW (-3) | — |
| 2 | 18 | 0 | Same; Tactical Awareness | — |
| 3 | 17 | 0 | **STEMPLER ZOND FTO**; same weapons; Super-Jump | Hollow Men max 2; Nayemnik required-choice max 1 |
| 4 | 22 | 0 | Thunderbolt (+1B), Flash Pulse, PARA CCW (-3); BS 12, Tactical Awareness | — |

### Tunguska Triggermen

**ID 1855 · AVA 3 · HI** — `MOV 15-5 | CC 17 | BS 13 | PH 12 | WIP 13 | ARM 4 | BTS 6 | W 2 | S 4`. 360º Visor, Mimetism (-3), Stealth, CC Attack (+1B), BS Attack (+1SD), Regeneration (PH=14).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 2 | 44 | 1.5 | MULTI Sniper Rifle, E/Marat (+1B), Pulzar (+1B), MULTI Pistol, CCW (-3) | Wildcard max 1 |
| 3 | 43 | 0 | K1 Combi Rifle, E/Marat (+1B), Pulzar (+1B), Drop Bears, MULTI Pistol, Silenced Pistol, CCW (-3); Surprise Attack (-3), Forward Deployment (+10), Decoy (1) | same |
| 4 | 47 | 1.5 | MULTI Sniper Rifle, E/Marat (+1B), Pulzar (+1B), MULTI Pistol, CCW (-3); Neurocinetics | same |

### Meteor Zonds

**ID 411 · AVA 1 · REM** — `MOV 15-10 | CC 14 | BS 11 | PH 12 | WIP 13 | ARM 0 | BTS 6 | W 1 | S 3`. ECM: Hacker (-3), Repeater, Remote Presence, Triangulated Fire, Courage, Forward Observer, Parachutist, Sensor, Combat Jump, Super-Jump (Jet Propulsion).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 21 | 0 | Light Shotgun, E/M Carbine, Flash Pulse, PARA CCW (-6) | — |
| 2 | 19 | 0 | Boarding Shotgun, Flash Pulse, PARA CCW (-6) | — |

### Puppetactica Company

**ID 1098 · AVA 1 Puppet Master / AVA 3 PuppetBots · LI + REM**.

**Puppet Master:** `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`; Counterintelligence.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 11 | 0 | SMG, Shock Mine, Pistol, CCW | — |
| 2 | 13 | 0 | SMG, Shock Mine, Pistol, CCW; Minelayer | — |
| 3 | 16 | 0.5 | SMG, Shock Mine, Pistol, CCW; Hacking Device, Hacker | — |

**PuppetBot Full Power:** `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 2 | S 1`; BS Attack (+1B), Courage, Dodge (+3), Peripheral (Control), Transmutation (1). Battle-ravaged: `BS 11 | ARM 0 | BTS 0`.

| PuppetBot opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 16 | 1.5 | Red Fury, PARA CCW (-3) |
| 2 | 9 | 0 | Boarding Shotgun, Flash Pulse, PARA CCW (-3); Forward Observer |
| 3 | 14 | 0 | AP Marksman Rifle, PARA CCW (-3); BS Attack (Shock) |

**Dependency:** source relation requires the PuppetBot profile group to depend on the Puppet Master profile group (`min: 1`, grouped relation).

### Tunguska Cheerkillers

**ID 1541 · AVA 5 · LI** — `MOV 10-10 | CC 19 | BS 12 | PH 12 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. Martial Arts L1, Dodge (+3), Super-Jump.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 12 | 0 | Light Shotgun, Pulzar, Pistol, Shock CCW | Spetskorp required-choice max 5 |
| 2 | 13 | 0 | SMG, Nanopulser, Pistol, Shock CCW | same |
| 3 | 18 | 0 | AP Rifle, Nanopulser, MULTI Pistol (+1B), Shock CCW | same |
| 4 | 14 | 0 | SMG, Nanopulser, Pistol, Shock CCW; Specialist Operative | same |
| 5 | 24 | 0 | Shock Marksman Rifle, Nanopulser, Pistol, Shock CCW; MSV2 | same |

### Mary Problems, Tactical ÜberHacker

**ID 1099 · AVA 1 · LI** — `MOV 10-10 | CC 14 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 6 | W 1 | S 2`. Hacking Device (Upgrade: Oblivion +1B), Killer Hacking Device (Upgrade: Trinity AP), Forward Deployment (+10), Dodge (+3), Mimetism (-6), Climbing Plus.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 27 | 0.5 | SMG, Zapper, Pitcher, Pistol, CCW; Hacker | — |

### Securitate

**ID 434 · AVA 255 (Total) · LI** — `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Warhorse.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 13 | 0 | Combi Rifle, Pistol, CCW | Securitate 1–5 |
| 2 | 21 | 1 | HMG, Pistol, CCW | same |
| 3 | 22 | 1 | Feuerbach, Pistol, CCW | same |
| 5 | 13 | 0 | Boarding Shotgun, Pistol, CCW; Repeater | same |
| 7 | 18 | 0.5 | Combi Rifle, Pistol, CCW; Hacking Device, Hacker | same |
| 9 | 15 | 0 | Combi Rifle, Pistol, CCW; MediKit, Paramedic | same |
| 10 | 13 | 0 | Combi Rifle, Pistol, CCW; Lieutenant | same |
| 11 | 15 | 0 | Combi Rifle, Pistol, CCW; Commlink (+1), Specialist Operative | same |

### Miranda Ashcroft

**ID 51 · AVA 1 · LI** — `MOV 10-10 | CC 19 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. CC Attack (-6), Mimetism (-6), Specialist Operative, Marksmanship, Stealth.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 27 | 0 | MULTI Rifle, PARA Mine, Boarding Pistol, Monofilament CCW | Wildcard max 1; Bounty Hunter context |
| 2 | 25 | 0 | Boarding Shotgun, PARA Mine, Boarding Pistol, Monofilament CCW | same |
| 3 | 28 | 0 | Combi Rifle, E/Mitter (+1B), PARA Mine, Boarding Pistol, Monofilament CCW | same |

### Reaktion Zonds

**ID 409 · AVA 1 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | W 1 | S 3`. Remote Presence, Courage, Total Reaction, Climbing Plus, 360º Visor.

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 24 | 1 | HMG, PARA CCW (-3) | — |
| 2 | 19 | 0 | Thunderbolt (+1B), PARA CCW (-3) | — |

### Anaconda, Mercenary TAG Squad

**ID 300 · AVA 1 · TAG** — `MOV 15-5 | CC 21 | BS 13 | PH 16 | WIP 13 | ARM 7 | BTS 6 | W 3 | S 7`. ECM: Guided (-6), BS Attack (SR-1), Courage, Dodge (PH=11), GizmoKit (PH=11), Tactical Awareness, Transmutation (Escape System -2), Warhorse, Immunity (AP).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 59 | 1.5 | AP Spitfire, Heavy Flamethrower (+1B), Thunderbolt (AP), DA CCW (PS 4) | VATRA required-choice max 1 |
| 2 | 59 | 1.5 | HMG, Light Shotgun (+2B), Panzerfaust, DA CCW (PS 4) | same |

**Operator:** `MOV 10-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 1 | BTS 3 | W 3 | S 2`; Spitfire, Smoke Grenade Launcher, Boarding Pistol, CCW; Courage, Specialist Operative, Tactical Awareness, Warhorse, Mimetism (-3).

### Wolfgang Amadeus Wolff

**ID 1555 · AVA 1 · WB** — `MOV 15-5 | CC 22 | BS 12 | PH 14 | WIP 13 | ARM 3 | BTS 3 | W 2 | S 2`. Martial Arts L3, BS Attack (Continuous Damage), Berserk (+3), Courage, Dodge (+5/+3), Immunity (ARM), Climbing Plus, Terrain (Zero-G), Frenzy, Discover (+6).

| Opt | Pts | SWC | Loadout / differences | FT |
|---:|---:|---:|---|---|
| 1 | 33 | 0 | MULTI Rifle (+1SD), Chain-colt, E/M Grenades (+1SD), Heavy Pistol, PARA CCW (-6), DA CCW (PS 4) | Wildcard max 1; Bounty Hunters and Securitate contexts |

## Canonical Fireteam chart

Fireteam limits in the pinned source: **Core 1; Haris 1; Duo unlimited** (`DUO: 256` sentinel).

### Securitate Fireteams

**Types:** Haris, Core

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| SECURITATE | 1 | 5 | no | — |
| INTERVENTOR | 0 | 3 | no | — |
| PERSEUS | 0 | 1 | no | Securitate |
| ROUNDER | 0 | 1 | no | Securitate |
| KULAK | 0 | 1 | no | Securitate |
| SWITCHER FTO | 0 | 1 | no | FTO profiles only (Opts 1–3) |
| TAG-TREIBER | 0 | 1 | no | — |
| GRENZER | 0 | 1 | no | — |
| VORTEX | 0 | 1 | no | Spec-Ops mode only |

### Spetskorp (Special Corps) Fireteams

**Types:** Duo, Haris, Core

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| CHEERKILLER | 0 | 5 | yes | Spetskorp |
| GRENZER | 0 | 5 | yes | Spetskorp |
| Fiddler FTO | 0 | 1 | no | Spetskorp; Opt 1 only |
| SWITCHER FTO | 0 | 1 | no | Spetskorp; Opts 1–3 only |

The Cheerkiller and Grenzer `required-choice` rows are a required-choice set from the Army chart; they are not interpreted here as requiring both unit types simultaneously.

### Hollow Men Fireteams

**Types:** Duo, Haris, Core

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| HOLLOW MEN | 1 | 5 | no | — |
| KRIZA BORAC | 0 | 2 | no | — |
| GRENZER | 0 | 1 | no | — |
| STEMPLER ZOND | 0 | 2 | no | FTO profile only (Opt 3) |
| PERSEUS | 0 | 1 | no | Hollow Men |

### VATRA Fireteams

**Types:** Duo

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| KRIZA BORAC | 0 | 2 | yes | — |
| ANACONDA | 0 | 1 | yes | — |
| KULAK | 0 | 1 | no | — |
| GRENZER | 0 | 1 | no | — |

The Kriza Borac and Anaconda `required-choice` rows are a required-choice set from the Army chart; they are not interpreted here as requiring both unit types simultaneously.

### Bounty Hunters Fireteams

**Types:** Duo, Haris

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| BOUNTY HUNTER | 0 | 3 | yes | Bounty Hunters |
| MOTORIZED BOUNTY HUNTER | 0 | 3 | yes | Bounty Hunters |
| GRENZER | 0 | 1 | no | Bounty Hunters |
| MOBILE BRIGADA | 0 | 1 | no | — |
| DENMA CONNOLLY | 0 | 1 | no | — |

The two Bounty Hunter `required-choice` rows are a required-choice set from the Army chart; they are not interpreted here as requiring both unit types simultaneously.

### Nayemnik (Mercenary) Fireteams

**Types:** Haris, Duo

| Entry | Min | Max | Required-choice | Counts as / note |
|---|---:|---:|---|---|
| PERSEUS | 0 | 1 | yes | Nayemnik |
| STEMPLER ZOND | 0 | 1 | yes | FTO profile only (Opt 3); Nayemnik |
| Fiddler FTO | 0 | 1 | yes | Opt 1 only; Nayemnik |

All three rows carry `required: true` in the source. They are preserved as the Army chart's required-choice/formation set rather than being interpreted as requiring all three simultaneously, which would be incompatible with the listed Duo type.

### Wildcards

| Entry | Max | Counts as / profile restriction |
|---|---:|---|
| TSYKLON FTO | 2 | Opts 1 and 2 only |
| VOSTOK | 1 | FTO profiles only (Opts 5 and 7) |
| TRIGGERMEN | 1 | Any standard Triggermen profile |
| SPECTOR | 1 | FTO profile only (Opt 3); Spetskorp and Nayemnik only |
| MIRANDA ASHCROFT | 1 | Bounty Hunter context |
| SFORZA | 1 | FTO profiles only (Opts 2 and 3); Bounty Hunter context |
| JELENA KOVAČ | 1 | Securitate context |
| WOLFGANG AMADEUS | 1 | Bounty Hunters and Securitate contexts |

## Reverse Fireteam index

| Unit | Fireteam access |
|---|---|
| Securitate | Securitate Core/Haris, 1–5 |
| Interventors | Securitate Core/Haris, max 3 |
| Perseus | Securitate Core/Haris max 1, counts as Securitate; Hollow Men Core/Haris/Duo max 1, counts as Hollow Men; Nayemnik Haris/Duo required-choice max 1 |
| Casino Security Rounders | Securitate Core/Haris max 1, counts as Securitate |
| Kulak | Securitate Core/Haris max 1, counts as Securitate; VATRA Duo max 1 |
| Switcher FTO | Securitate Core/Haris max 1; Spetskorp Core/Haris/Duo max 1; Opts 1–3 only |
| TAG-Treiber | Securitate Core/Haris max 1 |
| Grenzer | Securitate Core/Haris max 1; Spetskorp Core/Haris/Duo required-choice max 5; Hollow Men Core/Haris/Duo max 1; VATRA Duo max 1; Bounty Hunters Haris/Duo max 1 |
| Vortex Spec-Ops | Securitate Core/Haris max 1 in Spec-Ops mode |
| Cheerkillers | Spetskorp Core/Haris/Duo required-choice max 5 |
| Fiddler FTO | Spetskorp Core/Haris/Duo max 1; Nayemnik Haris/Duo required-choice max 1; Opt 1 only |
| Hollow Men | Hollow Men Core/Haris/Duo, 1–5 |
| Kriza Boracs | Hollow Men Core/Haris/Duo max 2; VATRA Duo required-choice max 2 |
| Stempler Zond FTO | Hollow Men Core/Haris/Duo max 2; Nayemnik Haris/Duo required-choice max 1; Opt 3 only |
| Anaconda | VATRA Duo required-choice max 1 |
| Authorized Bounty Hunters | Bounty Hunters Haris/Duo required-choice max 3 |
| Motorized Bounty Hunters | Bounty Hunters Haris/Duo required-choice max 3 |
| Mobile Brigada | Bounty Hunters Haris/Duo max 1 |
| Denma Connolly | Bounty Hunters Haris/Duo max 1 |
| Tsyklon FTO | Wildcard max 2; Opts 1 and 2 only |
| Vostok FTO | Wildcard max 1; Opts 5 and 7 only |
| Triggermen | Wildcard max 1 |
| Raoul Spector FTO | Wildcard max 1; Opt 3 only; Spetskorp/Nayemnik contexts only |
| Miranda Ashcroft | Wildcard max 1; Bounty Hunter context |
| Sforza FTO | Wildcard max 1; Opts 2 and 3 only; Bounty Hunter context |
| Jelena Kovač | Wildcard max 1; Securitate context |
| Wolfgang Amadeus Wolff | Wildcard max 1; Bounty Hunters/Securitate contexts |

## Reinforcement linkage

The pinned Tunguska Army data links Reinforcement roster **599**. This reference deliberately keeps Reinforcement roster entries and Reinforcement-specific Fireteams separate from the standard Tunguska chart.

## Source pinning

- Army source version: `7.26246.158`
- Army data changed on: `2026-09-03`
- Army backup commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`
- Army source blob: `b78b327b90aed6bafba9fa3cccb05ae2cc35dfa0`
- InfinityDB commit: `4e2662be3f43387fbae42b3790a711b3e98570c4`
- Rules baseline: N5.3 + N5 FAQ v0.1
- Verified/generated: `2026-10-15`

## Validation notes

- Standard roster count: 44 logical units, excluding Vortex Spec-Ops and Nomads Team-Ops optional modes and excluding generic mercenary-catalog entries with an empty source-faction list.
- All standard Army loadouts are represented, including composite/Peripheral profiles for Szalamandra, Fiddler, Zondnautica, Go-Pod, Puppetactica, and Anaconda.
- Canonical Fireteam chart reproduces the pinned Army min/max/required flags and profile-level FTO restrictions.
- Required rows with zero minimums are preserved as source required-choice sets rather than expanded into contradictory simultaneous requirements.
- Puppetactica's PuppetBot dependency on a Puppet Master is recorded from the source relation table.

## Command-unit apex/value cross-reference (2026-10-23)

**Kulak CoC 23/0** is a practical attack-capable safety net when an aggressive Tunguska Lieutenant/Hacker risks the next turn's pooled Orders. Safe backline command/NCO may require less insurance if the LT is rarely exposed. **Shifta CoC 21/0 belongs to Vanilla Nomads**, not automatically Tunguska; do not import the parent's availability.

See [cross-game Lieutenant, CoC and Order-economy tiers](../../notes/list-building/command-units-apex-and-value.md). **Refer to this pinned roster/Fireteam chart for profile legality.**

## Mission specialist / button-pusher choices (N5.3)

**Interventor HD+18–23/.5 WIP15 BTS9** is spectacular low-cost network/button eligibility from safety, but is **not a midfield console runner** by itself. Build a real repeater/recon unit and a second forward Objective specialist to reach buttons; **Mary Problems** trades extra points for a Mimetism(-6) forward KHD/Pitcher hybrid. **Kulak CoC** gives command insurance when chosen profile and mission recognize it. Compare hacker duel value separately from actual physical objective access.

[Cross-game apex and value specialist tier guide](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). The unit profiles/Fireteams above control exact legality.

## N5.3 airborne / backline-strike archetypes and trades (2026-10-23)

**Meteor Zond19/0 or21/0** provides true AD **Repeater + Sensor + FO** at the enemy backline: the payoff comes from **Interventor/WIP15 hacker and guided/Trinity network** rather than its own weak BS11 gun. **Go-Pod VH** attacks across rooftops with aerial mobility but can be very exposed (No Cover) and is not Combat Jump; choose only when supported LoF/exit path exists. **Spektr Hidden/Infiltration** is a more controllable delayed attacker into risky Combat Jump sites. Never import **Corregidor Hellcats/Surface Bearcats** without current Tunguska roster permission.

[Full N5.3 apex/value and delivery-probability tier guide](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). Current roster/profile restrictions and canonical Fireteam chart above govern legal choices.

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn gunfighter choice:** **Kriza HMG45/1.5 (LT same 45)** is the high-Burst/HMG direct gun with BS Attack(-3) and +1B; its protected *non-LT* variant generally suits aggressive repeated trading better unless CoC is planned. **Szalamandra HRMC68/2** adds much higher ARM/range/AP for a visible 3STR centerpiece, **NCO** profitable only when the special LT Order is available. **Grenzer Red Fury28/1** / **MSR32/1.5 Marksmanship** solve respectively mobile close fighting and visible long ARO; neither is a cheap Kriza HMG replacement against high-ARM TAGs. [Cross-game gunfighter and LT/CoC decision guide](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## Warbands and inexpensive trading roles — N5.3

**Denma Connolly Chain(+1B)+Smoke/AP+DA12/0** is a high-value active/defensive speedbump with 15-5, CC23, Berserk and MetaChemistry(ReRoll) inside legal **Bounty Hunters team** context if selected; it is **not a Morlock6** and does not grant team-wide smoke otherwise. **Motorized Bounty Hunters8/0 shotgun+Riotstopper or9/0 SMG+Chain-colt** are faster cheap template/control flank traders, but 1W/Impetuous motorbikes can be eliminated by mines/side ARO. Strong Tunguska hackers can often immobilize a TAG without attempting an unprotected CC dive. Do not import Vanilla Nomads Morlocks unless listed.

[Cross-game warband/cheap-trader apex and value tiers, targets and command packages](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). Profile-specific sectorial legality/Fireteams above control all selections.

## TAG tactical cross-reference (2026-10-23)

**Szalamandra (68)** is the obvious HRMC long-range centerpiece and the current Tunguska profile gives **NCO**; it needs help navigating Hackers, Camo and close flanks. **Anaconda (59)** trades ceiling for an AP Spitfire/Thunderbolt and operator fallback, but is usually a more conditional investment. Do not copy Tunguska NCO into another faction's profile without checking.

Cross-faction **apex vs points-value** comparisons, matchup table, and direct MCP-reviewed podcast/video sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Current profile and Fireteam legality above remain authoritative.

## Vehicle (VH) tactical cross-reference (2026-10-23)

**Go-Pod AVA1:** **33/0 MULTI Rifle/E/Mitter+Go-Bot** preserves Szalamandra/Hollow-Men SWC; **32/1.5 HRL+AP SMG** buys a bigger attack. After those guns and the hacking network remove threats, its Jet Propulsion and Go-Bot create unusually deep flanks. **Robert Shepherd's detailed Tunguska review** strongly opposes treating it as a default opener: S7/ARM2/No Cover and Mimetism(-3) are hard to hide or maintain under MSV/warhorse/repeater opposition. It is not a Fireteam member.

See [VH apex/value tier list and matchup guide](../../notes/list-building/vehicles-vh.md). **This sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative.**

## Hacker and KHD tactical cross-reference (2026-10-23)

**Interventor HD+ 18–23/0.5 WIP15/BTS9**, alongside **KHD 18/0**, are premium cyber capability for near-budget prices. Use **Hollow-Men Pitcher/linked gun** and FastPandas to give them a real network; **Spektr KHD 30/0** supplies Hidden/Infiltration scoring. **Mary Problems 27/0.5** combines HD/KHD + FD/Mimetism(-6), but Shepherd's detailed faction review argues **two Interventors** better sustain a protected backfield net unless Mary must personally deploy forward. **Rounder HD+Trinity 21/0.5** and **Kulak KHD+Carbonite 20/0** make cheap hybrids. **Hollow Man HD 29/0.5 TinBot** needs legitimate link protection; do not confuse high BTS with hacking immunity.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

See the N5.3 [cross-game apex/value rankings and transcript-backed competing assessments](../../notes/list-building/cheerleaders-and-order-generators.md). The current roster and official Fireteam definitions above remain authoritative; unit access/cost may differ from vanilla.

- 7pt Transductor — cheap Regular Repeater/Flash REM (not a dedicated gunfighter); its S3 footprint and AVA constrain spam.
- 8pt Salyut — Baggage/Repeater Regular Order; reload support and deployment-zone density determine marginal value.
- 10pt Alguacil — inexpensive S2 Regular and Fireteam/LT material; upgrade only for a credible second job.
- 11pt Puppet Master — one Regular Order plus Counterintelligence; PuppetBots do not add Orders.
- 13pt Securitate — Warhorse/WIP14 Repeater and link option; much worse pure pts/Order than a 7pt Transductor.

**Selection rule:** Count deployed, transferable Regular Orders per Combat Group, not total models or restricted bonus Orders; choose the lowest-cost protected Regular profile that *also* contributes a relevant Repeater, Baggage, Fireteam, template, ARO or Specialist job. Check Group slots and DZ hiding space before buying a third large-base REM or replacing a needed scoring piece.


## ARO apex/value cross-reference (2026-10-23)

The [N5.3 cross-faction ARO apex/value and matchup study](../../notes/list-building/aro-units-apex-and-value.md) compares hidden missile traps, Neurocinetics/TR, cheap templates/mines, DZ guards and conflicting creator opinions. Consult the **roster and Fireteam chart above** for legally available profiles, SWC, Training and AVA.

- **Reaktion 0SWC Thunderbolt TR** — 19pt recoverable midrange guard, complements a separate expensive gun/hidden layer
- **Triggerman Neurocinetics Sniper** — high-reactive-ceiling durable 47pt investment, but disputed versus cheaper TR + mine/hidden layers
- **PuppetBots + Master** — Flash/forward presence, Counterintelligence and activation compression; PuppetBots do not generate separate orders
- **Tsyklon Feuerbach/Pitcher FTO** — ranged defense and forward repeater pressure; only link when chart authorizes FTO
- **Warcor Flash** — 3pt Irregular ARO tax/late-game Stun attempt, not a Regular Order

**Practical deployment:** put cheap disposable/Flash/DTW or mine pressure on the approach; retain a separate unseen or recoverable threat for the decisive square; avoid exposing a premium active attacker and check opponent Smoke, MSV, hacking, AD and pie-slicing. No automatic order from an off-table Hidden model; Irregular ARO units do not supply generic Regular Orders.
