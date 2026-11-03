---
schema_version: 1
reference_type: faction
status: current
faction_id: 701
faction_slug: aleph
faction_name: ALEPH
rules_baseline: N5.3
army_source_version: "7.26246.159"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Standard Vanilla ALEPH roster, profile/loadout costs and AVA, peripherals/composite entries, Lieutenant/order-control and hacking hooks, optional-mode content, and Reinforcements boundary. Vanilla ALEPH has no normal Fireteam chart."
---

# ALEPH (Vanilla) — N5.3 faction reference

## Overview and provenance

Repository-native reference for **Vanilla ALEPH** (Army faction ID `701`). It is intended to be sufficient for ordinary roster, profile, AVA, points/SWC, Lieutenant, specialist, hacking/network, peripheral, and deployment questions without reopening Army.

Sources used:

- Army-derived ALEPH source revision `7.26246.159` from `massayoshi/infinity-army-backup` commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- Aggregate dataset: `n5/aleph/aleph.json` (blob `c81ab6e036772dd704be69fba83934bfaf6dabba`).
- InfinityDB normalization/semantics at commit `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: N5.3 + N5 FAQ v0.1.

Coverage notes:

- Covers the **52 standard Vanilla ALEPH roster entries** whose Army availability includes faction `701`.
- `Chandra Spec-Ops` and `ALEPH Team-Ops` are optional-mode hooks and are listed separately.
- Generic Soldier-of-Fortune / mercenary-catalog entries whose source faction list is empty are excluded. Named mercenaries explicitly assigned to ALEPH by Army (for example Samsa, Knauf, and John Hawkwood) are included.
- Linked Reinforcement army ID: **799**. Reinforcement profiles are not merged into this base roster.
- **Vanilla ALEPH has no normal Fireteam chart.** `FTO` profile labels are preserved because they are part of Army data, but they do not create Fireteam access in vanilla play.
- AVA is taken from the Vanilla ALEPH source, not from Steel Phalanx or Operations. Cross-faction AVA/profile differences are intentional unless noted otherwise.
- Army encodes **AVA Total** as raw value `255`; this file renders it as `Total`.
- Source spelling/label oddities such as `TARKSIA` option labels are normalized to the unit's canonical `Tarkshya` name while noted where useful.

## Faction summary

| Field | Value |
|---|---|
| Faction | ALEPH (Vanilla) |
| Army ID | 701 |
| Rules baseline | N5.3 + FAQ v0.1 |
| Standard roster entries | 52 |
| Optional-mode entries | Chandra Spec-Ops; ALEPH Team-Ops |
| Reinforcement roster | Army ID `799` |
| Fireteams | **None in normal vanilla play** |

## Standard roster index

| Unit | ID | AVA | Type | Primary hooks |
|---|---:|---:|---|---|
| Maruts | 585 | 1 | TAG | Lt/Strategos, Tactical Awareness, MSV2 |
| Daleth Rebots | 590 | 2 | REM | Sensor, Repeater, FO; TacAware option |
| Thyreos | 1592 | 2 | LI | Camo midfield, mines, FO/Hacker/KHD |
| Yudbots | 192 | 2 | REM | Servant peripheral |
| Deva Functionaries | 109 | 2 | MI | Lt, HD/KHD, Sensor, MSV2, Devabot |
| Yadu | 1129 | 2 | MI | Lt/NCO, Hacker, FO, durable specialist |
| Optimate Agent Maximus | 1862 | 1 | MI | TacAware, Lt + SWC bonus, optional Minimus |
| K2 Auxiliars | 1856 | 1 | HI | cheap E/M/mine support; airborne specialist option |
| Shukra Consultants | 1128 | 1 | LI | Chain of Command, Counterintelligence |
| Penthesilea | 611 | 1 | WB | fast specialist, smoke, CC |
| Ekdromoi | 603 | 1 | MI | Combat Jump hacker/KHD |
| Maximus | 1720 | 1 | TAG | TacAware, Lt option, durable attack TAG |
| Kyra Sharma | 1897 | 1 | HI | TacAware, Paramedic; airborne option |
| Thorakitai | 600 | 2 | MI | cheap line troops, FO/Paramedic/Feuerbach |
| Sharvara HoundBots | 1899 | 1 | REM | FD, Mimetism, E/M/adhesive close assault |
| Arjuna Unit | 1178 | 2 | MI | TacAware, FD, KiranBots, multiple FTO-labelled solos |
| Dikpala Tacbots | 1898 | Total | REM | cheap REM line, Repeater/Commlink/Paramedic |
| Hoplites | 1591 | 1 | HI | Lt, Engineer/Specialist, heavy attack |
| Netrods | 595 | 3 | LI | 6-point Regular order; mandatory Combat Jump deployment |
| Freelance Operator Samsa | 1683 | 1 | MI | Infiltration, Decoy, Mimetism, specialist |
| Riksha Tacbots | 1769 | 5 | REM | cheap Mimetism gunfighters/FO |
| Dawon Tacbots | 1770 | 5 | REM | cheap CC/warband-style REM |
| Zayin Rebots | 591 | 2 | REM | Total Reaction HMG/Thunderbolt |
| Knauf | 939 | 1 | LI | MSV1 sniper, Surprise/Decoy |
| Satrah Unit | 1772 | 2 | MI | MSV2 + Albedo; KHD option |
| Warcors | 50 | 1 | LI | Irregular Flash Pulse ARO |
| Posthumans | 597 | 1 each body | mixed | G: Jumper Proxy Mk.1/2/4/5 |
| Nagas | 59 | 2 | SK | Camo infiltrators, mines/hackers/FO |
| Dasyus | 587 | 2 | SK | Hidden Deployment, Mimetism -6, specialists |
| Parvati | 1534 | 1 | LI | elite Doctor/Engineer |
| Dr. Claire Lazhari | 1894 | 1 | LI | Doctor, MediKit, Albedo, Disco Baller |
| Johnny Kao | 1892 | 1 | MI | Engineer, GizmoKit, mines/turret |
| Apsaras | 1174 | 1 | LI | KHD, Repeater, RemDriver/TAGCom, Lt |
| Danavas Hackers | 950 | 2 | LI | WIP15 HD+, Pitcher |
| Myrmidons | 588 | 4 | WB | smoke, Mimetism -6, CC, Hacker option |
| Probots | 596 | 2 | REM | Baggage, EVO, Repeater/TR option |
| Sophotects | 185 | 2 | MI | Doctor + Engineer, GizmoKit/MediKit, turret options |
| Artalis Unit | 1771 | 2 | LI | NCO, Engineer/Doctor support |
| Garuda Tacbots | 110 | 2 | REM | Combat Jump/Parachutist attack/FO |
| Agêma Marksmen | 602 | 1 | MI | MSV2 long-range ARO/attack |
| Kinnara Scoutbots | 1901 | 2 | REM | Sensor, Eclipse, infiltration/parachutist |
| Lamedh Rebots | 593 | 2 | REM | cheap Repeater/Flash Pulse |
| Samekh Rebots | 592 | 2 | REM | Guided Missile Launcher |
| John Hawkwood | 1556 | 1 | MI | CoC option, long-range option |
| Asuras | 584 | 2 | HI | MSV3, HD+, Lt +1 Order |
| Trisha N33 | 1557 | 1 | LI | Engineer, Jammer |
| Hippolyta | 1471 | 1 | WB | Mimetism -6, smoke, top-tier CC |
| Dart | 1130 | 1 | SK | Camo, MSV1, mines; optional Sharvara K-9 |
| Rudras GunBots | 1197 | 1 | REM | Repeater, durable gunfighter |
| Yaksha Tacbots | 1906 | 2 | REM | Camouflage, FD, mines/MadTraps |
| Tarkshya Interception Wing | 1904 | 1 | VH | aerial heavy gun platform, MSV1 |
| Pilot-X Team | 1903 | 1 Pilot-X | LI + REM | Hacker/RemDriver with 0–2 RacerBots |

## Unit details

### Maruts

**ID 585 · AVA 1 · TAG** — `MOV 15-10 | CC 18 | BS 15 | PH 17 | WIP 15 | ARM 8 | BTS 9 | STR 3 | S 7`. Remote Presence, MSV2, ECM: Guided (-6), Courage, Tactical Awareness, Terrain (Total), strong Dodge/GizmoKit modifiers.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 86 | 1.5 | MULTI HMG, Heavy Flamethrower, Pulzar, AP CCW; includes Karkata |
| 2 | 90 | 2 | As Opt 1; **Lieutenant, Strategos L2**; includes Karkata |

Karkata is the bundled ancillary remote profile.

### Daleth Rebots

**ID 590 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`. Remote Presence, Repeater, Sensor, Forward Observer, Triangulated Fire, Climbing Plus.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 15 | 0 | Combi Rifle, Flash Pulse, PARA CCW |
| 2 | 18 | 0 | As Opt 1; **Tactical Awareness** |

### Thyreos

**ID 1592 · AVA 2 · LI** — `MOV 15-5 | CC 21 | BS 12 | PH 10 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. Camouflage (limited), Mimetism (-3), Forward Deployment (+20), Surprise Attack (-3), Stealth, Natural Born Warrior, Religious Troop.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 22 | 0 | Boarding Shotgun, D-Charges, Shock Mine, Pistol, Monofilament CCW |
| 2 | 21 | 0 | SMG, D-Charges, Shock Mine, Pistol, Monofilament CCW |
| 3 | 22 | 0.5 | As Opt 2; **Minelayer** |
| 4 | 22 | 0 | As Opt 2 + Flash Pulse; **Forward Observer** |
| 5 | 26 | 0.5 | SMG, D-Charges, E/M Mine, Pistol, Monofilament CCW; **Hacking Device** |
| 6 | 25 | 0 | Boarding Shotgun, D-Charges, E/M Mine, Pistol, Monofilament CCW; **Killer Hacking Device** |

### Yudbots

**ID 192 · AVA 2 · REM Peripheral** — `MOV 15-10 | CC 11 | BS 8 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 1`. Peripheral (Servant), Courage, Mimetism (-3).

| Pts | SWC | Loadout |
|---:|---:|---|
| 3 | 0 | PARA CCW; bought as Servant peripheral |

### Deva Functionaries

**ID 109 · AVA 2 · MI** — `MOV 10-10 | CC 15 | BS 12 | PH 11 | WIP 15 | ARM 2 | BTS 3 | W 1 | S 2`. Courage, Number 2, NWI, Immunity (Isolated).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 20 | 0 | Combi Rifle, Nanopulser, Pistol, CCW |
| 2 | 24 | 0 | As Opt 1 + Devabot |
| 3 | 22 | 0 | MULTI Rifle, Nanopulser, Pistol, CCW |
| 4 | 25 | 0.5 | Combi Rifle, Nanopulser, Pistol, CCW; **Hacking Device** |
| 5 | 20 | 0 | Boarding Shotgun, Nanopulser, Pistol, CCW; **KHD** |
| 6 | 21 | 0 | Combi Rifle, Nanopulser, Pistol, CCW; **Sensor, Triangulated Fire** |
| 8 | 21 | 0 | Combi Rifle, Nanopulser, Flash Pulse, Pistol, CCW; **Forward Observer** |
| 9 | 29 | 1 | Spitfire, Nanopulser, Pistol, CCW; **MSV2** |
| 10 | 20 | 0 | Combi package; **Lieutenant** |
| 11 | 24 | 0 | Lieutenant package + Devabot |
| 12 | 21 | 0 | Lieutenant; Sensor/Triangulated Fire package |

### Yadu

**ID 1129 · AVA 2 · MI** — `MOV 15-5 | CC 15 | BS 13 | PH 11 | WIP 14 | ARM 3 | BTS 6 | W 1 | S 2`. Albedo, Courage, NWI, Warhorse, Number 2, Immunity (Shock).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 28 | 0 | MULTI Rifle, E/Marat, Drop Bears, Heavy Pistol, CCW |
| 2 | 26 | 1.5 | HRL, SMG, E/Marat, Heavy Pistol, CCW |
| 5 | 28 | 0 | MULTI Rifle, E/Marat, Disco Baller, Heavy Pistol, CCW; Deactivator |
| 6 | 27 | 0.5 | Boarding Shotgun, E/Marat, Heavy Pistol, CCW; **Hacking Device** |
| 7 | 27 | 0 | MULTI Rifle, E/Marat, Flash Pulse, Heavy Pistol, CCW; **FO** |
| 8 | 34 | 1.5 | HMG, E/Marat, Heavy Pistol, CCW; **NCO** |
| 9 | 28 | 0 | MULTI Rifle/Drop Bears package; **Lieutenant** |

### Optimate Agent Maximus

**ID 1862 · AVA 1 · MI** — `MOV 15-5 | CC 22 | BS 13 | PH 13 | WIP 13 | ARM 3 | BTS 3 | W 1 | S 2`. Tactical Awareness, NWI, Specialist Operative, Number 2, Natural Born Warrior, Albedo, strong Dodge/CC modifiers.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 48 | 1 | AP Thunderbolt, E/M Carbine, Heavy Pistol, AP+DA CCW; includes **Minimus** |
| 2 | 45 | 1 | Same weapons; **FTO label**, TinBot (Repeater); no Minimus |
| 3 | 48 | **+1** | Opt 1; **Lieutenant**; includes Minimus |
| 4 | 45 | **+1** | Opt 2; **Lieutenant**; no Minimus |

**Maximus restriction:** Army notes that there can only be one Maximus in an Army List; this applies when choosing between this entry and the Maximus TAG.

### K2 Auxiliars

**ID 1856 · AVA 1 · HI** — `MOV 10-10 | CC 18 | BS 11 | PH 12 | WIP 13 | ARM 2 | BTS 3 | STR 1 | S 2`. Remote Presence, Courage, NWI.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 11 | 0 | E/Marat, Flash Pulse, Breaker Pistol, PARA CCW; FTO label |
| 2/3 | 12 | 0 | Flash Pulse, Mine Dispenser, Breaker Pistol, PARA CCW; FTO label (duplicate Army rows) |
| 4 | 18 | 0 | E/Marat, Flash Pulse, Breaker Pistol, PARA CCW; GizmoKit, **Parachutist, Specialist Operative** |

### Shukra Consultants

**ID 1128 · AVA 1 · LI** — `MOV 10-10 | CC 16 | BS 12 | PH 11 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Biometric Visor, Counterintelligence, Courage.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 21 | 0 | Boarding Shotgun, Pistol, CCW; **Chain of Command** |
| 2 | 26 | 0 | MULTI Rifle, Nanopulser, Pistol, CCW; **Chain of Command** |

### Penthesilea

**ID 611 · AVA 1 · WB** — `MOV 20-15 | CC 23 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 2 | S 4`. Motorcycle, Impetuous, Mimetism (-3), Specialist Operative, Limited Cover, strong CC/Dodge package.

| Pts | SWC | Loadout |
|---:|---:|---|
| 28 | 0 | AP SMG, Zapper, Smoke Grenade Launcher, Pistol, Monofilament CCW |

### Ekdromoi

**ID 603 · AVA 1 · MI** — `MOV 10-10 | CC 22 | BS 12 | PH 13 | WIP 14 | ARM 2 | BTS 0 | W 1 | S 2`. Martial Arts L3, Combat Jump, Parachutist, Stealth, Super-Jump.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 6 | 23 | 0.5 | Chain Rifle, AP Heavy Pistol, DA CCW; **Hacking Device** |
| 7 | 25 | 0 | SMG, Flash Pulse, AP Heavy Pistol, DA CCW, D-Charges; **KHD** |

### Maximus

**ID 1720 · AVA 1 · TAG** — `MOV 15-10 | CC 24 | BS 14 | PH 13 | WIP 13 | ARM 6 | BTS 6 | STR 4 | S 6`. Tactical Awareness, Natural Born Warrior, heavy Immunity package, Escape System/Transmutation.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 82 | 1.5 | AP HMG, E/M Carbine, Heavy Pistol, AP+DA CCW |
| 2 | 80 | 1 | AP Thunderbolt, E/M Carbine, Heavy Pistol, AP+DA CCW |
| 3 | 82 | 0 | Opt 1; **Lieutenant** |

Only one Maximus may appear in an Army List.

### Kyra Sharma

**ID 1897 · AVA 1 · HI** — `MOV 15-10 | CC 18 | BS 14 | PH 12 | WIP 14 | ARM 3 | BTS 3 | W 2 | S 2`. Tactical Awareness, Regeneration, enhanced Super-Jump, strong Immunity package, MediKit (+1B).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 45 | 0 | MULTI Marksman Rifle, Light Riotstopper, WildParrot, Breaker Pistol, PARA CCW; **Paramedic**; FTO label |
| 2 | 52 | 0 | MULTI Rifle, Light Riotstopper, Akrylat-Kanone, WildParrot, Breaker Pistol, PARA CCW; **Combat Jump, Parachutist, Paramedic** |

### Thorakitai

**ID 600 · AVA 2 · MI** — `MOV 10-10 | CC 16 | BS 12 | PH 11 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 2`.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 12 | 0 | SMG, E/Mitter, Pulzar, Pistol, CCW |
| 2 | 14 | 0 | Combi Rifle, Nanopulser, Pistol, CCW |
| 6 | 13 | 0 | SMG, E/Mitter, Pulzar, Flash Pulse, Pistol, CCW; **FO** |
| 7 | 14 | 0 | SMG, E/Mitter, Pulzar, Pistol, CCW; **Paramedic/MediKit** |
| 9 | 23 | 1.5 | Feuerbach, Nanopulser, Pistol, CCW |

### Sharvara HoundBots

**ID 1899 · AVA 1 · REM** — `MOV 15-15 | CC 22 | BS 11 | PH 12 | WIP 12 | ARM 0 | BTS 3 | STR 1 | S 3`. Remote Presence, Forward Deployment (+10), Mimetism (-3), Stealth, Natural Born Warrior, Super-Jump.

| Opt | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 17 | 0 | Light Shotgun, Heavy Riotstopper, E/Marat, DA CCW, PARA CCW |
| 2 | 19 | 0 | Adhesive Launcher Rifle, Light Shotgun, E/Marat, DA CCW, PARA CCW |
| 3 | 15 | 0 | Adhesive Launcher Rifle, Heavy Riotstopper, E/Marat, DA CCW, PARA CCW |

### Arjuna Unit

**ID 1178 · AVA 2 · MI** — `MOV 15-5 | CC 17 | BS 13 | PH 11 | WIP 14 | ARM 3 | BTS 3 | W 1 | S 2`. Tactical Awareness, Mimetism (-3), Specialist Operative, Religious Troop; many solo profiles add Forward Deployment (+20). KiranBots are optional bundled peripherals.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 21 | 0 | Boarding Shotgun, Flash Pulse, D-Charges, Breaker Pistol, CCW; FTO label |
| 2 | 32 | 0 | Opt 1 + FD (+20) + KiranBot 1 |
| 3 | 25 | 0 | Opt 1 + FD (+20), no bot |
| 7 | 30 | 1.5 | Spitfire, D-Charges, Breaker Pistol, CCW; TinBot: Firewall; FTO label |
| 8 | 42 | 1.5 | Opt 7 + FD (+20) + KiranBot 1 |
| 9 | 35 | 1.5 | Spitfire profile + FD (+20), no bot |
| 10 | 23 | 0 | AP SMG, E/Mitter, D-Charges, Breaker Pistol, CCW; TinBot: Firewall; FTO label |
| 11 | 33 | 0 | Opt 10 package + FD (+20) + KiranBot 1 |
| 12 | 26 | 0 | AP-SMG package + FD (+20), no bot |
| 13 | 32 | 0 | Boarding-Shotgun package + FD (+20) + KiranBot 2 |
| 14 | 33 | 0 | AP-SMG package + FD (+20) + KiranBot 2 |
| 15 | 42 | 1.5 | Spitfire package + FD (+20) + KiranBot 2 |

### Dikpala Tacbots

**ID 1898 · AVA Total · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 2`. Remote Presence, Mimetism (-3), Courage, ECM: Hacker.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 13 | 0 | Combi Rifle, PARA CCW |
| 2 | 21 | 1 | HMG, PARA CCW |
| 3 | 19 | 1 | MULTI Sniper Rifle, PARA CCW |
| 4 | 15 | 0 | Combi Rifle, PARA CCW; **Commlink, Specialist Operative** |
| 5 | 13 | 0 | SMG, Akrylat-Kanone, PARA CCW; **Repeater** |
| 6 | 15 | 0 | Combi Rifle, PARA CCW; **Paramedic/MediKit** |

### Hoplites

**ID 1591 · AVA 1 · HI** — `MOV 15-5 | CC 20 | BS 13 | PH 13 | WIP 13 | ARM 3 | BTS 6 | W 2 | S 2`. Natural Born Warrior, Combat Instinct, Religious Troop, strong CC/Dodge package.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 40 | 1.5 | HMG, Pulzar, AP Heavy Pistol, E/M CCW |
| 2 | 37 | 1 | Red Fury, Pulzar, AP Heavy Pistol, E/M CCW |
| 3 | 36 | 0 | MULTI Rifle, Pulzar, Drop Bears, AP Heavy Pistol, E/M CCW; **Specialist Operative** |
| 4 | 39 | 0 | Opt 3; **Engineer, GizmoKit** |
| 5 | 42 | 0 | Engineer package + Armed Turret (Combi Rifle) |
| 6 | 40 | 1 | HMG package; **Lieutenant** |

### Netrods

**ID 595 · AVA 3 · LI** — `MOV — | CC — | BS — | PH — | WIP — | ARM 0 | BTS 3 | STR 1 | S 2`. Warhorse, Religious Troop.

| Pts | SWC | Loadout / note |
|---:|---:|---|
| 6 | 0 | No weapons. **Must be deployed by Combat Jump during the Deployment Phase.** |

### Freelance Operator Samsa

**ID 1683 · AVA 1 · MI** — `MOV 15-5 | CC 15 | BS 13 | PH 11 | WIP 13 | ARM 3 | BTS 0 | W 1 | S 2`. Infiltration, Mimetism (-3), Decoy, Surprise Attack (-3), Super-Jump, Specialist Operative, Exrah.

| Pts | SWC | Loadout |
|---:|---:|---|
| 26 | 0 | Plasma Rifle, D-Charges, Pistol, CCW |

### Riksha Tacbots

**ID 1769 · AVA 5 · REM** — `MOV 15-5 | CC 13 | BS 13 | PH 10 | WIP 13 | ARM 3 | BTS 3 | STR 1 | S 2`. Remote Presence, Mimetism (-3), Courage, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 18 | 0 | Boarding Shotgun, Chain-colt, PARA CCW |
| 2 | 20 | 1.5 | HRL, Light Shotgun, PARA CCW |
| 3 | 24 | 1 | Red Fury, PARA CCW |
| 4 | 20 | 0 | Combi Rifle, Flash Pulse, PARA CCW; **FO** |

### Dawon Tacbots

**ID 1770 · AVA 5 · REM** — `MOV 15-10 | CC 22 | BS 11 | PH 13 | WIP 12 | ARM 1 | BTS 3 | STR 1 | S 2`. Remote Presence, Martial Arts L2, Dogged, Religious Troop, enhanced Dodge/Immunity.

| Opt | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 20 | 0 | Chain Rifle, Flammenspeer, MULTI Pistol, E/M CCW |
| 2 | 19 | 0 | Pulzar, Blitzen, MULTI Pistol, Shock CCW |
| 3 | 20 | 0 | Boarding Shotgun, MULTI Pistol, Shock CCW |
| 4 | 19 | 0 | Chain Rifle, Flammenspeer, MULTI Pistol, E/M CCW |
| 5 | 18 | 0 | Pulzar, Blitzen, MULTI Pistol, Shock CCW |

Army retains the superficially duplicate rows because option-level differences are source-defined.

### Zayin Rebots

**ID 591 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`. Remote Presence, Total Reaction, 360º Visor, Climbing Plus.

| Opt | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 24 | 1 | HMG, PARA CCW |
| 2 | 19 | 0 | Thunderbolt, PARA CCW |

### Knauf

**ID 939 · AVA 1 · LI** — `MOV 10-10 | CC 21 | BS 13 | PH 11 | WIP 13 | ARM 1 | BTS 0 | W 1 | S 2`. MSV1, Mimetism (-3), Stealth, Terrain (Total), BS Attack bonuses.

| Pts | SWC | Loadout |
|---:|---:|---|
| 31 | 1.5 | MULTI Sniper Rifle, AP Heavy Pistol, CCW; Surprise Attack (-3), Decoy |

### Satrah Unit

**ID 1772 · AVA 2 · MI** — `MOV 10-10 | CC 16 | BS 13 | PH 11 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. MSV2, Albedo, Stealth, Climbing Plus.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 24 | 0 | Thunderbolt, Pulzar, Heavy Pistol, CCW |
| 4 | 24 | 0 | MULTI Marksman Rifle, Pulzar, Heavy Pistol, CCW |
| 5 | 20 | 0 | SMG, Pulzar, Cybermine, Heavy Pistol, CCW; **KHD with Firewall** |

### Warcors

**ID 50 · AVA 1 · LI** — `MOV 10-10 | CC 11 | BS 9 | PH 11 | WIP 13 | ARM 0 | BTS 0 | W 1 | S 2`. Irregular, Journalist.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 3 | 0 | Flash Pulse, Stun Pistol, PARA CCW; 360º Visor |
| 2 | 3 | 0 | Same weapons; Sixth Sense instead of 360º Visor |

### Posthumans

**ID 597 · G: Jumper** — each Proxy body is AVA 1; the unit follows G: Jumper composition rules rather than acting as unrelated troopers.

#### Proxy Mk.1

`MOV 10-10 | CC 13 | BS 13 | PH 11 | WIP 15 | ARM 2 | BTS 3 | W 1 | S 2`. Mimetism (-3), NWI, Courage.

| Opt | Pts | SWC | Loadout / role |
|---:|---:|---:|---|
| 1 | 14 | 0.5 | Combi Rifle, Nanopulser, Pistol, CCW; **Hacking Device** |
| 2 | 13 | 0 | Combi Rifle, Nanopulser, D-Charges, Pistol, CCW; **Engineer**, GizmoKit/Deactivator |
| 3 | 13 | 0 | Combi Rifle, Nanopulser, Pistol, CCW; **Doctor**, MediKit |

#### Proxy Mk.2

`MOV 10-10 | CC 13 | BS 13 | PH 13 | WIP 15 | ARM 1 | BTS 0 | W 1 | S 2`. Camouflage, Infiltration, Mimetism (-6), Stealth, NWI.

| Opt | Pts | SWC | Loadout / role |
|---:|---:|---:|---|
| 1 | 26 | 1.5 | MULTI Sniper Rifle, Pistol, CCW |
| 2 | 22 | 0.5 | Boarding Shotgun, Pistol, CCW; **Hacking Device** |

#### Proxy Mk.4

`MOV 10-10 | CC 13 | BS 14 | PH 14 | WIP 15 | ARM 5 | BTS 6 | W 2 | S 2`.

| Opt | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 30 | 1.5 | HMG, Nanopulser, Pistol, CCW |
| 2 | 26 | 1.5 | HRL, SMG, Nanopulser, Pistol, CCW |

#### Proxy Mk.5

`MOV 10-10 | CC 14 | BS 13 | PH 11 | WIP 15 | ARM 3 | BTS 3 | W 1 | S 2`. Forward Deployment (+10), NWI.

| Opt | Pts | SWC | Loadout / role |
|---:|---:|---:|---|
| 1 | 21 | 0.5 | Mk12, Heavy Pistol, CCW; enhanced BS Attack |
| 2 | 13 | 0.5 | SMG, Flash Pulse, E/M Grenades, Heavy Pistol, CCW; **FO** |

### Nagas

**ID 59 · AVA 2 · SK** — `MOV 10-10 | CC 16 | BS 12 | PH 12 | WIP 14 | ARM 1 | BTS 0 | W 1 | S 2`. Camouflage, Infiltration, Mimetism (-3), Surprise Attack (-3), Stealth, Dogged, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 3 | 29 | 1.5 | MULTI Sniper Rifle, Nanopulser, Pistol, CCW; enhanced BS Attack |
| 4 | 25 | 0.5 | Boarding Shotgun, Nanopulser, Shock Mine, Pistol, CCW; **Minelayer** |
| 5 | 27 | 0 | AP SMG, Nanopulser, D-Charges, E/M Mine, Pistol, CCW; **KHD** |
| 6 | 29 | 0.5 | AP SMG, Nanopulser, D-Charges, Pistol, CCW; **Hacking Device + Deployable Repeater** |
| 7 | 25 | 0 | AP SMG, Nanopulser, Flash Pulse, D-Charges, Pistol, CCW; **FO + Deployable Repeater** |
| 8 | 26 | 0.5 | AP SMG, Nanopulser, Monofilament Mine, Pistol, CCW; **Minelayer** |

### Dasyus

**ID 587 · AVA 2 · SK** — `MOV 15-5 | CC 16 | BS 13 | PH 12 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Camouflage, Hidden Deployment, Infiltration, Mimetism (-6), Surprise Attack (-3), Immunity (Shock), Stealth, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 2 | 28 | 0 | Boarding Shotgun, Pulzar, D-Charges, Silenced Pistol, CCW |
| 3 | 34 | 1.5 | MULTI Sniper Rifle, Pulzar, Silenced Pistol, CCW |
| 4 | 31 | 0 | AP SMG, Pulzar, D-Charges, Silenced Pistol, CCW; **KHD** |
| 5 | 33 | 0.5 | AP SMG, Pulzar, D-Charges, Silenced Pistol, CCW; **Hacking Device** |
| 6 | 29 | 0 | AP SMG, Pulzar, D-Charges, Flash Pulse, Silenced Pistol, CCW; **FO + Deployable Repeater** |
| 8 | 30 | 0.5 | AP SMG, Pulzar, Viral Mine, D-Charges, Silenced Pistol, CCW; **Minelayer** |

### Parvati

**ID 1534 · AVA 1 · LI** — `MOV 15-5 | CC 15 | BS 12 | PH 10 | WIP 15 | ARM 2 | BTS 6 | STR 2 | S 2`. Remote Presence, Doctor, Engineer, Courage, enhanced Dodge/Super-Jump.

| Pts | SWC | Loadout |
|---:|---:|---|
| 36 | 0 | SMG, Flash Pulse, Pistol, CCW; GizmoKit, MediKit |

### Dr. Claire Lazhari

**ID 1894 · AVA 1 · LI** — `MOV 15-5 | CC 16 | BS 13 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. Albedo, NWI, enhanced MediKit/Doctor package.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 33 | 0 | Breaker Combi Rifle, Nanopulser, Viral Pistol, Disco Baller, PARA CCW; **Doctor**, MediKit |
| 2 | 33 | 0 | Same package; FTO-labelled Doctor profile |

### Johnny Kao

**ID 1892 · AVA 1 · MI** — `MOV 15-5 | CC 18 | BS 13 | PH 12 | WIP 14 | ARM 3 | BTS 6 | W 2 | S 2`. Engineer, Mimetism (-3), X-Visor, Deactivator, enhanced GizmoKit.

| Opt | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 36 | 0 | Plasma Carbine, Zapper, Monofilament Mine, D-Charges, MULTI Pistol, CCW |
| 2 | 40 | 0 | MULTI Rifle, Zapper, Drop Bears, D-Charges, MULTI Pistol, CCW |
| 3 | 42 | 0 | MULTI Rifle, Zapper, Monofilament Mine, D-Charges, Armed Turret, MULTI Pistol, CCW |

### Apsaras

**ID 1174 · AVA 1 · LI** — `MOV 10-10 | CC 15 | BS 13 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. KHD, Deployable Repeater.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 17 | 0 | SMG, Zapper, Pistol, CCW; Hacker |
| 2 | 20 | 1 | Same; **RemDriver** |
| 3 | 18 | 0 | Same; **TAGCom** |
| 4 | 20 | 0 | Same; **Lieutenant + RemDriver** |

### Danavas Hackers

**ID 950 · AVA 2 · LI** — `MOV 10-10 | CC 15 | BS 11 | PH 11 | WIP 15 | ARM 1 | BTS 3 | W 1 | S 2`.

| Pts | SWC | Loadout |
|---:|---:|---|
| 22 | 0.5 | Combi Rifle, Pitcher, Breaker Pistol, CCW; **Hacking Device Plus** (Oblivion upgrade), Hacker |

### Myrmidons

**ID 588 · AVA 4 · WB** — `MOV 10-10 | CC 21 | BS 12 | PH 13 | WIP 13 | ARM 2 | BTS 0 | W 1 | S 2`. Frenzy, Martial Arts L3, Mimetism (-6), Stealth, enhanced Dodge.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 23 | 0 | Combi Rifle, Nanopulser, Smoke Grenades, Pistol, AP CCW |
| 2 | 24 | 0 | Combi Rifle, Nanopulser, Smoke Grenades, Pistol, DA CCW |
| 3 | 30 | 1 | Spitfire, Nanopulser, Smoke Grenades, Pistol, DA CCW |
| 4 | 16 | 0 | Chain Rifle, Nanopulser, Smoke Grenades, Pistol, DA CCW |
| 5 | 21 | 0 | Boarding Shotgun, Smoke Grenades, Pistol, DA CCW |
| 6 | 29 | 0.5 | Combi/Nanopulser/Smoke/DA package; **Hacking Device** |

### Probots

**ID 596 · AVA 2 · REM** — `MOV 10-10 | CC 13 | BS 11 | PH 10 | WIP 13 | ARM 2 | BTS 3 | STR 1 | S 4`. Remote Presence, Baggage.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 8 | 0 | PARA CCW; Repeater, Deactivator |
| 2 | 14 | 0.5 | PARA CCW; **EVO Hacking Device** |
| 3 | 17 | 0 | Combi Rifle, PARA CCW; Repeater, **Total Reaction** |

### Sophotects

**ID 185 · AVA 2 · MI** — `MOV 15-10 | CC 13 | BS 11 | PH 11 | WIP 15 | ARM 2 | BTS 3 | W 1 | S 2`. Doctor + Engineer, NWI, Courage, Deployable Cover, MediKit, enhanced GizmoKit.

| Opt | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 25 | 0 | SMG, Pulzar, Flash Pulse, D-Charges, Pistol, CCW |
| 3 | 32 | 0 | Combi Rifle, Pulzar, D-Charges, Armed Turret, Pistol, CCW |
| 4 | 30 | 0 | SMG, Pulzar, D-Charges, Armed Turret, Pistol, CCW |

### Artalis Unit

**ID 1771 · AVA 2 · LI** — `MOV 10-10 | CC 17 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 3 | W 1 | S 2`. NCO, NWI, enhanced BS/Dodge package; Deactivator.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 27 | 0 | Combi Rifle, Light Rocket Launcher, D-Charges, AP Heavy Pistol, CCW; **Engineer**, GizmoKit |
| 2 | 23 | 0 | K1 Combi Rifle, D-Charges, AP Heavy Pistol, CCW; **Engineer**, GizmoKit |
| 3 | 23 | 0 | MULTI Rifle, D-Charges, AP Heavy Pistol, CCW; **Engineer**, GizmoKit |
| 4 | 23 | 0 | K1 Combi Rifle, D-Charges, AP Heavy Pistol, CCW; **Doctor**, MediKit |

### Garuda Tacbots

**ID 110 · AVA 2 · REM** — `MOV 20-5 | CC 13 | BS 12 | PH 11 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 2`. Remote Presence, Mimetism (-3), Combat Jump, Parachutist, Super-Jump.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 3 | 18 | 0 | Boarding Shotgun, Chain-colt, PARA CCW |
| 4 | 25 | 1.5 | Spitfire, PARA CCW |
| 5 | 20 | 0 | Combi Rifle, Flash Pulse, PARA CCW; **FO** |

### Agêma Marksmen

**ID 602 · AVA 1 · MI** — `MOV 10-10 | CC 15 | BS 13 | PH 11 | WIP 13 | ARM 2 | BTS 3 | W 1 | S 2`. MSV2, Courage.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 27 | 1.5 | MULTI Sniper Rifle, Breaker Pistol, CCW; Hidden Deployment, Surprise Attack (-3) |
| 3 | 27 | 1.5 | Missile Launcher, Pulzar, Breaker Pistol, CCW; limited Camouflage + Decoy |

### Kinnara Scoutbots

**ID 1901 · AVA 2 · REM** — `MOV 15-5 | CC 23 | BS 12 | PH 12 | WIP 12 | ARM 1 | BTS 3 | STR 1 | S 2`. Remote Presence, Mimetism (-3), Sensor, Specialist Operative, Decoy, Stealth, Climbing Plus, Terrain (Total).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 25 | 0.5 | Vulkan Shotgun, HFT, D-Charges, E/M Mine, Pistol, Monofilament CCW; **Infiltration, Minelayer** |
| 2 | 24 | 0 | Vulkan Shotgun, HFT, D-Charges, Eclipse Grenades, Pistol, Monofilament CCW; **Parachutist** |
| 3 | 24 | 0 | SMG, E/M Carbine, D-Charges, Eclipse Grenades, Pistol, Monofilament CCW; **Parachutist** |

### Lamedh Rebots

**ID 593 · AVA 2 · REM** — `MOV 15-15 | CC 13 | BS 8 | PH 11 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`. Remote Presence, Mimetism (-3), Repeater.

| Pts | SWC | Loadout |
|---:|---:|---|
| 7 | 0 | Flash Pulse, PARA CCW |

### Samekh Rebots

**ID 592 · AVA 2 · REM** — `MOV 15-10 | CC 13 | BS 12 | PH 10 | WIP 13 | ARM 0 | BTS 3 | STR 1 | S 3`. Remote Presence, Courage.

| Pts | SWC | Loadout |
|---:|---:|---|
| 16 | 1.5 | Missile Launcher, PARA CCW; **BS Attack (Guided)** |

### John Hawkwood

**ID 1556 · AVA 1 · MI** — `MOV 10-10 | CC 22 | BS 13 | PH 11 | WIP 14 | ARM 3 | BTS 6 | W 1 | S 2`. Martial Arts L1, Mimetism (-3), NWI, Stealth, Terrain (Total), Immunity (Shock).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 6 | 35 | 1 | K1 Sniper Rifle, Nanopulser, MULTI Pistol, DA CCW |
| 7 | 40 | 0 | Combi Rifle, Nanopulser, MULTI Pistol, DA CCW; X-Visor, **Chain of Command** |

Army's raw Opt 7 payload contains two weapon-id `0` placeholder rows; they are not treated as named weapons here.

### Asuras

**ID 584 · AVA 2 · HI** — `MOV 15-5 | CC 20 | BS 14 | PH 14 | WIP 15 | ARM 5 | BTS 6 | W 2 | S 2`. MSV3, Courage, NWI, ECM: Hacker.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 2 | 61 | 1.5 | AP Spitfire, Pulzar, MULTI Pistol, AP CCW |
| 3 | 63 | 0.5 | MULTI Marksman Rifle, Pulzar, MULTI Pistol, AP CCW; **Hacking Device Plus** |
| 5 | 65 | 1 | AP Spitfire package; **Lieutenant (+1 Order)** |

### Trisha N33

**ID 1557 · AVA 1 · LI** — `MOV 15-5 | CC 17 | BS 12 | PH 10 | WIP 14 | ARM 2 | BTS 3 | W 1 | S 2`. Engineer, Dogged, Immunity (Shock), enhanced GizmoKit/Deactivator.

| Pts | SWC | Loadout |
|---:|---:|---|
| 24 | 0 | Breaker Combi Rifle, Pulzar, Jammer, D-Charges, Pistol, CCW |

### Hippolyta

**ID 1471 · AVA 1 · WB** — `MOV 15-5 | CC 24 | BS 13 | PH 14 | WIP 14 | ARM 3 | BTS 3 | W 2 | S 2`. Impetuous, Martial Arts L3, Berserk, Mimetism (-6), Stealth, Super-Jump, Limited Cover.

| Pts | SWC | Loadout |
|---:|---:|---|
| 37 | 0 | Breaker Combi Rifle, Nanopulser, Flash Pulse, Smoke Grenades, Pistol, EXP CCW |

### Dart

**ID 1130 · AVA 1 · SK** — `MOV 10-10 | CC 16 | BS 13 | PH 13 | WIP 13 | ARM 1 | BTS 3 | W 1 | S 2`. Camouflage, Mimetism (-3), MSV1, Forward Deployment (+20), Decoy, NWI, Climbing Plus, Specialist Operative.

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 35 | 0 | AP SMG, Viral Tactical Bow, E/M Grenades, Pistol, CCW |
| 2 | 35 | 0 | AP SMG, Viral Tactical Bow, Shock Mine, Pistol, CCW |
| 3 | 36 | 0.5 | Opt 2; **Minelayer** |
| 4 | 42 | 0.5 | Opt 3 + **Sharvara K-9 HoundBot** peripheral |

### Rudras GunBots

**ID 1197 · AVA 1 · REM** — `MOV 15-5 | CC 11 | BS 13 | PH 11 | WIP 12 | ARM 4 | BTS 6 | STR 2 | S 4`. Remote Presence, Repeater, Courage, Immunity (AP), Climbing Plus, Tech-Recovery.

| Opt | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 2 | 35 | 0 | K1 Marksman Rifle, Pulzar, Panzerfaust, Heavy Pistol, PARA CCW; FTO label |
| 3 | 38 | 1 | Red Fury, Pulzar, Panzerfaust, Heavy Pistol, PARA CCW |
| 4 | 37 | 1 | Red Fury package; FTO label |

### Yaksha Tacbots

**ID 1906 · AVA 2 · REM** — `MOV 15-5 | CC 14 | BS 13 | PH 10 | WIP 13 | ARM 4 | BTS 3 | STR 1 | S 2`. Remote Presence, Camouflage (limited), Forward Deployment (+20), Mimetism (-3), Surprise Attack (-3), Terrain (Total).

| Opt | Pts | SWC | Loadout / differences |
|---:|---:|---:|---|
| 1 | 23 | 0 | AP SMG, Light Flamethrower, Mine Dispenser, PARA CCW |
| 2 | 25 | 0.5 | E/M Carbine, Light Flamethrower, MadTraps, PARA CCW; **Minelayer** |
| 3 | 27 | 0 | Boarding Shotgun, Light Flamethrower, Mine Dispenser, PARA CCW; **Specialist Operative** |
| 4 | 31 | 1 | Red Fury, Light Flamethrower, D-Charges, PARA CCW; **Specialist Operative** |

### Tarkshya Interception Wing

**ID 1904 · AVA 1 · VH** — `MOV 20-5 | CC — | BS 13 | PH 12 | WIP 13 | ARM 4 | BTS 6 | STR 3 | S 7`. Remote Presence, Aerial, MSV1, Mimetism (-6), No Cover, Super-Jump, Tech-Recovery, Terrain (Total), Transmutation/Escape operator.

| Opt | Pts | SWC | Loadout |
|---:|---:|---:|---|
| 1 | 41 | 1.5 | MULTI Red Fury, Chain Rifle; bundled Tarkshya Operator |
| 2 | 38 | 0 | MULTI Marksman Rifle, AP SMG; bundled Operator |
| 3 | 34 | 0 | MULTI Marksman Rifle, Chain Rifle; bundled Operator |

Army's option label spells the unit `TARKSIA`; this reference uses the canonical `Tarkshya` name.

### Pilot-X Team

**ID 1903 · AVA 1 Pilot-X + 0–2 RacerBots**.

**Pilot-X** — `MOV 10-10 | CC 17 | BS 12 | PH 10 | WIP 14 | ARM 1 | BTS 6 | W 1 | S 2`. Hacking Device, Immunity (Shock), **RemDriver**.

| Pts | SWC | Loadout |
|---:|---:|---|
| 23 | 0.5 | E/Mitter, Flash Pulse, MULTI Pistol, PARA CCW; Hacker |

**RacerBot Mk-III** — `MOV 20-10 | CC 13 | BS 11 | PH 12 | WIP 11 | ARM 0 | BTS 3 | STR 1 | S 2`. Remote Presence, 360º Visor, No Cover.

| Pts | SWC | Loadout |
|---:|---:|---|
| 8 each | 0 | Light Riotstopper, Mine Dispenser, Stun Pistol, PARA CCW; Deployable Repeater |

Composition note from Army: a Pilot-X Team is **1 Pilot-X and 0–2 RacerBots Mk-III**. A RacerBot cannot be taken without Pilot-X, and all members must belong to the same Combat Group.

## Lieutenant and order-control index

| Unit/profile | Control hook |
|---|---|
| Marut Opt 2 | Lieutenant + Strategos L2 |
| Deva Opts 10–12 | Lieutenant |
| Yadu Opt 9 | Lieutenant |
| Optimate Agent Maximus Opts 3–4 | Lieutenant; **+1 SWC** profile |
| Maximus Opt 3 | Lieutenant |
| Hoplite Opt 6 | Lieutenant |
| Apsara Opt 4 | Lieutenant + RemDriver |
| Asura Opt 5 | Lieutenant **(+1 Order)** |
| Shukra | Chain of Command + Counterintelligence |
| John Hawkwood Opt 7 | Chain of Command |
| Yadu Opt 8 | NCO |
| Artalis | NCO on chassis |
| Marut / Maximus / Optimate Maximus / Kyra / Arjuna | Tactical Awareness (profile/chassis as listed) |
| Apsara | RemDriver or TAGCom options |
| Pilot-X | RemDriver |

## Hacking and network index

### Hacking Devices / KHDs

- **HD+**: Danavas; Asura.
- **HD**: Deva, Yadu, Thyreos, Ekdromos, Myrmidon, Naga, Dasyu, Proxy Mk.1.
- **KHD**: Deva, Thyreos, Ekdromos, Naga, Dasyu, Satrah, Apsara.
- **EVO**: Probot.
- **Pilot-X**: Hacking Device with its source upgrade package and RemDriver.

### Repeater / projection pieces

- Lamedh: Repeater.
- Daleth: Repeater + Sensor/FO.
- Probot: Repeater/Baggage or EVO.
- Rudra: Repeater.
- Dikpala: Repeater option.
- Apsara: Deployable Repeater.
- Naga: Deployable Repeater options.
- Dasyu: Deployable Repeater option.
- Pilot-X RacerBot Mk-III: Deployable Repeater.
- Danavas: Pitcher.
- K2/Arjuna/Yaksha/Kinnara and other deployable-weapon profiles add local area denial around the network.

## Airborne / deployment index

- **Combat Jump / Parachutist:** Ekdromoi, Garuda; Kyra airborne profile; Netrods (mandatory Combat Jump deployment).
- **Parachutist:** K2 airborne specialist; Kinnara options 2–3.
- **Hidden Deployment:** Dasyus; Agêma sniper profile.
- **Camouflage / midfield:** Thyreos, Nagas, Dasyus, Dart, Yaksha; Proxy Mk.2.
- **Forward Deployment:** Samsa/Infiltration, Arjuna solo profiles, Sharvara, Dart, Yaksha, Thyreos, Proxy Mk.5.

## Optional-mode units

| Unit | ID | Mode | Normal vanilla status |
|---|---:|---|---|
| Chandra Spec-Ops | 1922 | Spec-Ops | Optional mode only |
| ALEPH Team-Ops | 1936 | Team-Ops | Optional mode only |

Do not count these as ordinary matched-play Vanilla ALEPH roster entries unless that optional mode is explicitly enabled.

## Reinforcements boundary

Army links Vanilla ALEPH to Reinforcement roster ID **799**. Reinforcement-only profiles and any Reinforcement Fireteam information remain separate from this base-faction reference.

## Source-normalization notes

- `AVA 255` in the raw Dikpala profile is Army's sentinel for **AVA Total**.
- FTO names on Arjuna, K2, Kyra, Rudra, Claire, Optimate Agent Maximus, etc. do **not** create a Fireteam in Vanilla ALEPH.
- Generic `merc-*` catalog objects with an empty `factions` array are not part of the 52-entry standard roster.
- Named mercenaries explicitly carrying faction `701` in Army data are ordinary selectable Vanilla ALEPH entries and are therefore retained.
- Maximus TAG and Optimate Agent Maximus each carry the source restriction that only one Maximus may appear in an Army List.

## Command-unit apex/value cross-reference (2026-10-23)

**Marut LT 90/2** is a true apex **Strategos L2 + Tactical Awareness + MSV2** TAG commander, but it costs an entire supporting specialist package; **Shukra CoC 21/0** with Counterintelligence is cheap insurance that can justify exposing Marut. **Asura LT(+1) 65/1** is a different active-LT plan: its two personal LT Orders need a meaningful outlet or a real linked NCO (where legal). Do not double count Strategos converted Orders as NCO Tactical Orders.

See [cross-game Lieutenant, CoC and Order-economy tiers](../../notes/list-building/command-units-apex-and-value.md). **Current pinned profiles and Fireteam chart above govern legality.**

## Mission specialists — N5.3 apex and value cross-reference (2026-10-23)

**Mission benchmark:** **Posthuman Mk.1 Engineer/Doctor 13 + Mk.5 FO 13/.5** is elite points/slot economy **inside legal 2–3 Proxy G:Jumper**, *not independent Orders*; **Naga FO25 and Dasyu FO29** provide early/hidden scoring. **Sophotect25** is WIP15 Doctor+Engineer/fast, **Parvati36** the durable premium, **Daleth FO15/TA18** cheap Sensor/Repeater. **Asura HD+63** is apex combined hacking/gun/score only if those expensive tools work together. No Vanilla Asura HD+ LT profile.

[Cross-game specialist and button-pusher tiers](../../notes/list-building/mission-specialists-and-button-pushers-apex-value.md). **Current profile options and Fireteam chart in this file remain authoritative.**

## Airborne and enemy-DZ attack choices — N5.3 (2026-10-23)

**Garuda BSG18/0, FO20/0 (MOV20-5, Mimetism−3)** is a premier cheap **Combat Jump or ordinary Parachutist** assault/objective option; **PH11** unsupported Combat Jump gives **55%** delivery, so safe table edge can be wiser. **Ekdromoi HD23/.5 or KHD25/0** combines MA3/CC22 and AD for hacker/close-route tasks. **Kinnara Scoutbot Parachutist24** brings Eclipse/Vulkan/tech attack while its separate **Infiltration25** option trades surprise arrival for predeployed marker threat. **Tarkshya VH34–41** is very mobile aerial **on-table** attacker, **NOT** a Combat Jump troop. Protect mission scorers while spending the primary pool.

See [current cross-game apex/value, landing odds and expected-trade tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **This roster and Fireteam chart control exact loadout/availability.**

## Active-turn gunfighter cross-reference (2026-10-23)

**Active-turn shooting choices:** **Marut MULTI HMG86/1.5** is the heavy **TAG** BS15/MSV2 long-gun answer to enemy Mimetism/Smoke; its expense needs independent specialists and repair. **Asura AP Spitfire61/1.5** is the **non-TAG** MSV3 armored midfield gun, while **HD+ MULTI MMR63/0.5** sacrifices AP range for hacking/utility. **Posthuman Mk.4 HMG30/1.5** is terrific shooting only when the legal multi-Proxy purchase is affordable, **not** an independently fieldable 30pt gun. [Separated TAG versus non-TAG ceiling and value](../../notes/list-building/active-turn-gunfighters-apex-and-value.md).

## TAG tactical cross-reference (2026-10-23)

**Marut (86, 90 Strategos LT)** is an apex shooter against smoke/Mimetism because **MSV2 + BS15 MULTI HMG** matters more than merely paying for armor; it also brings command power but concentrates points/LT risk. **Maximus TAG (80–82)** instead supplies Immunity (ARM), 4 STR, AP/CC/E/M counterassault. Most ordinary scenarios still require inexpensive scoring/anti-hacking bodies alongside either. Maximus Agent and TAG profiles must not be confused.

Across all factions, compare **apex power** separately from **points value**, counterplay and mission fit: [N5.3 TAG guide](../../notes/list-building/tags.md). The current unit profiles and canonical Fireteam chart above take precedence over tactical opinions.

## Vehicle (VH) tactical cross-reference (2026-10-23)

**Tarkshya AVA1** (newer than the October 2025 global flyer ranking): **34/0 MULTI Marksman+Chain Rifle(+1B)** is an excellent low-SWC **MSV1, Mimetism(-6), STR3 Remote Presence** aerial attacker, with **capable Operator after Transmutation**. **38/0 AP SMG** enhances close armored matchups, **41/1.5 MULTI Red Fury** buys range/offensive weight but competes with Marut/other weapons for SWC. Its S apex/S value rank is **provisional 2026 profile analysis**, not an older presenter's assessment. Operator mission utility only applies in the correct state.

See [VH apex/value tier list and matchup guide](../../notes/list-building/vehicles-vh.md). **Current profiles, AVA and canonical Fireteam chart above remain authoritative.**

## Hacker and KHD tactical cross-reference (2026-10-23)

**Best hacker-per-point:** **Danavas HD+ + Oblivion(+1B) 22/0.5 WIP15/Pitcher** combines White Noise/anti-TAG control; **Deva KHD 20/0 WIP15, NWI and Immunity(Isolated)** is cheaper anti-Hacker plus a sturdy scorer. **Asura HD+ 63/0.5 WIP15, ARM5/MSV3/NWI** is the high-end combat specialist, not an economical stationary network node; check *Vanilla* upgrade instead of silently borrowing OSS **Trinity(+1SD)**. **Naga KHD 27/0 vs HD+Deployable Repeater 29/0.5**, **Dasyu KHD 31/0** buy forward concealment. Use affordable remote Repeaters to project Danavas/Deva rather than exposing them; a Marut already strains premium-point budget.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

For cross-faction **apex** and **points-value** rankings, the Order types, situational counterexamples and transcript-backed disagreements, see [Cheerleaders and Order Generators — N5.3](../../notes/list-building/cheerleaders-and-order-generators.md). Roster profiles/AVA/Fireteam legality above take precedence.

- **6pt Netrod**: cheapest Regular pool Order where roster-legal, but its mandatory deployment and stationary non-combat body are a risk
- **9pt RacerBot Mk-I**: mobile Regular Order plus adhesive/PARA disruption; avoid exposing an unnecessary REM

**List-building test:** count *transferable* Regular Orders by Combat Group after deployment; include required link members/command enablers, physical DZ footprint, and the unit's actual ARO/mission contribution. Do not treat Irregular, Tactical, Lieutenant or Peripheral activations as interchangeable generic Orders.


## ARO apex/value cross-reference (2026-10-23)

See [ARO units: N5.3 apex/value tiers, hidden-versus-visible and deployment/matchups](../../notes/list-building/aro-units-apex-and-value.md). The **current profile details here** control exact cost/SWC, Training and Fireteam eligibility; do not import another faction's link or specialist upgrades.

- **Zayin Thunderbolt TR** — 19pt/0SWC reactive volume and regular Order; protected Engineer/Yudbot route makes defeating it a repeat job
- **Riksha HRL** — 20pt/1.5SWC launcher, inexpensive but limited durability; Fireteam source permissions control bonus dice
- **Samekh FTO ML** — linked launcher only when the canonical chart permits this precise profile; Guided version is not automatically a linked ARO
- **Dikpala Mimetism Repeater/akrylat** — backstop/Fireteam troop with reactive control and support, not a generic passive TR piece
- **Posthuman/Proxy screen** — distributed positions and cheap Engineer recovery can outvalue a single static sniper; remember G: Jumper ARO restrictions

**Choose by circumstance:** a hard long gun matters only when the opponent must cross its arc; cheaper mines, Camo markers, templates, Flash, DTWs and hacking force movement or risk without committing an entire attack plan. Budget a second layer and preserved counterattack, check pie-slicing, hidden Order cost, anti-visual bypass and repair routes.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Recovery:** **Sophotect25 WIP15, Doctor+Engineer, MOV15-10, NWI** is an S-value dual network with **Yudbot3** (or two spaced bots), notably for **Marut + Cubed elite VITA**. **Parvati36** has stronger apex **Doctor(2W)** and a mobile Engineer role when both get used. **Posthuman Mk.1 Engineer** is relevant *only within legal 2–3 Proxy/G:Jumper purchase*, never priced as a standalone support Order. [Doctor/Engineer apex, points-value, recovery odds and transcript disputes](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## N5.3 midfield area denial / speed bumps (tactical synthesis)

**Dasyu Viral Minelayer (2) 30/.5** is an apex anti-infantry Hidden deployment trap; **Naga Monofilament Minelayer 26/.5** threatens elite models crossing a chokepoint. **Kinnara infiltrating 25/.5** adds E/M Mine + Decoy(2) + Sensor; **Yaksha 25/.5** offers MadTraps/ARM4/FD(+20), but competing Naga/Dasyu/Dart or inexpensive support REMs can be more efficient. Hidden Dasyu withholds its Order until revealed. The Yaksha 23/0 Mine Dispenser is **not** its zero-Order Minelayer loadout.

[Whole-game midfield area-denial tier guide and transcript disagreements](../../notes/list-building/midfield-area-denial-and-speed-bumps-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Andromeda30/0** (Infiltration, **Guard+MA3+D-Charges**, NWI) is a rare offensive Guard assassination bubble; **LoF+ZoC** is required and Guard does not create Engaged at range. **Myrmidon Chain Rifle16/0** combines **Mimetism−6 + Smoke + MA3 DA** as cheap Regular approach enabler; **Hippolyta37/0** gives a 2W Super-Jump/Berserk/EXP mobile assault when roster-legal. Compare patient target with **NBW** and do not count CC-based criticals as target-kill chance. [Cross-game CC assassin apex/value, Guard and delivery disputes](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## N5.3 network projection — Pitchers, Repeaters, TinBots and disposable delivery

**Danavas HD+/Oblivion(+1B)+Pitcher22/.5** gives WIP15 White Noise plus network but **BS11 Pitcher** is an inconsistent long shot without special die. **Naga FO25/0** or **Dasyu FO29/0** carry deployable Repeaters into forward positions, not prepaid nodes unless selected Minelayer; **Apsaras KHD with Deployable Repeater** is a defensive/support path. **Pilot-X HD23/.5 + RacerBot Mk-III8/0 each**, maximum two, is **31/.5 minimum** (39/.5 two) for MOV20-10 kamikaze Place Deployable; bots **cannot be selected without the Pilot-X**. **Opposing TA OSS 2026:** inexpensive fast bots reduce Danavas pitcher necessity, yet Danavas White Noise/Oblivion retains specialist/hacker value. **Maximus Agent FTO45/1 TinBot Repeater** is a pricey *legal team* Repeater, not Firewall.

[Cross-game apex/value guide, exact delivery cost and transcript disagreements](../../notes/list-building/network-projection-repeaters-pitchers-apex-value.md). Profile and Fireteam tables above remain authoritative.

## Tactical cross-reference — toolbox units (2026-10-23)

**Asura HD+63/.5** is a premium solo shooter/WIP15 hacker/MSV3/specialist with high durability, whereas **AP Spitfire61/1.5** is a non-hacking profile and **AP Spitfire LT65/1** is distinct. **Shikami-style Eclipse** isn't on Asura, and her expensive fair gunfights remain a weakness despite excellent full-suite competency. **Sophotect25 and Parvati36** trade offensive apex for a more efficient Doctor+Engineer/mission toolbox. [Whole-game tier and transcript debate](../../notes/list-building/jack-of-all-trades-toolbox-units-apex-value.md).

## N5.3 rare abilities & unusual combinations — tactical synthesis

**G:Jumper Posthumans** (2–3 Proxies, **one shared Regular Order**) are elite location/role compression: **Mk.1 Engineer/Doctor13/0 + Mk.5 FO13/.5 =26/.5** is a legal cheap specialist pair; add Mk.2 Camo/Infiltration or Mk.4 HMG only if jobs fit budget. **Only one unrestricted reactive ARO among Proxies per enemy Order**; other legal AROs Dodge/Reset. **Apsaras RemDriver20/1** (Vanilla option, versus **20/0 OSS**) gives one eligible REM a free deployment-time printed MOD, and **Pilot-X23/.5 + RacerBot8 each** is a **31/.5 minimum dependent package**, not standalone 8pt units. **Satrah MSV2+Albedo KHD20/0 or gun24/0** counters opponent MSV and camo with independent protections; **Kinnara Parachutist Eclipse+Monofilament24/0** is a rare backline blind-approach specialist, *different* from 25/.5 mine/Infiltration. **Opposing TA OSS:** Pilot-X/racerbot likely ubiquitous versus keeping a simpler Danavas/Mk.1 support budget.

[Cross-faction rare abilities apex/value, mechanics, and MCP source debates](../../notes/list-building/rare-capabilities-and-unique-combinations-apex-value.md). Current roster/Fireteam profile tables above are authoritative.

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**K2 Auxiliary11 E/Marat** (legal FTO variant) and **Thorakitai12 SMG+E/Mitter** are exceptionally cheap *non-hacker* TAG-brick threats. **Sharvara Houndbot15 Adhesive+E/Marat** is versatile short denial; **Thyreos SMG21 Monofilament**, **Artalis K1 Combi Engineer23**, and **Kinnara24 Parachutist Eclipse+Mono / 25 Infiltration Mono+E/M Mine** add actual target access or repeatable ARM=0. **Penthesilea28 Monofilament bike** can reach a flank but isn't a 28pt guaranteed TAG kill. **Maximus** is high-cost gun, separate from cheap control. [Non-hacking anti-TAG/HI apex/value and target matchups](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## Tactical cross-reference — indirect fire (2026-10-23)

**Vanilla ALEPH:** **Samekh Guided ML16/1.5**, with existing Danavas HD+/Dasyu/Daleth FO and Pilot-X/RacerBot network, is an optional high-impact off-angle attack. Targeted also helps **Marut/Asura direct BS fire**; do not sacrifice the primary gun's active Orders unless missile payoff is likely. **FTO Samekh Missile+Flash15/1.5** is a distinct *non-Guided* legal Fireteam variant elsewhere, not an extra free bonus on the vanilla Guided profile. [Indirect tiers/anti-cases](../../notes/list-building/indirect-fire-speculative-guided-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Asura HD+63/.5** has W2+NWI/ARM5/MSV3, WIP15 and hacker counterplay: elite **carry-and-fight** apex, though losing it risks too much list value. **Posthuman Mk.1 Engineer13 + Mk.5 FO13/.5 =26/.5** gives **two location options, one shared Order**; do not count 26VP twice when comparing zones, and non-active Proxies Dodge/Reset. **Marut86/1.5** is huge ARM8/STR3 zone swing, *not normal Supplies carrier*; **Maximus TAG80/1** 4STR is a second raw mass option. **Yadu FO27/0** NWI/Warhorse, **Apsaras/Deva protected score** are cheaper. **Opposing TA OSS/LoL:** luxury Marut/Maximus/Asura screen can win lanes, but the cheap Posthuman/Deva plus independent artillery often scores more reliably.

[Cross-game zone-holder and carrier apex/value guide, rules, and transcript disagreements](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Source roster/FT chart above wins over tactical comparisons.

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Asura HD+63/.5 (MSV3 + WIP15 White Noise)** is an apex *solo* multi-tech answer: visible Camo can be automatically Discovered under MSV3 and enemy MSV/Marksmanship corridors can be blinded via projected White Noise. **Marut86/1.5 MSV2 MULTI HMG** instead *kills* revealed Mimetism/Smoke shooters at very high TAG cost. **Satrah MSV2+Albedo** (KHD20/0 versus gun24/0 are different options) cheaply answers both enemy visor and Mimetism; **Daleth/Pathfinder Sensor FO REM** detects Hidden/Camo behind cover at ZoC and is much more efficient than paying 63pt merely to identify a 15pt marker. **Counter:** White Noise also disables *friendly* visor LoF through the zone; Albedo is matchup-only.

[Anti-Tech N5.3 apex/value tiers, matchup rules and opposing MCP viewpoints](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## Force multipliers — N5.3 role/value cross-reference (2026-10-23)

**Apsaras TAGCom18/0** carries KHD+Deployable Repeater and boosts **same Combat Group TAGs** only by printed Dodge PH+3/GizmoKit PH+1; a **17pt KHD** is cheaper without need. **Probots8/0 Baggage vs14/.5 EVO** depends on live REM/AD Supportware, no native Spotlight. **Shukra Counterintel CoC21 / Strategos LT24** are profile choices; **Arjuna FTO Firewall(-3)23** supports legal Fireteams, while Maximus FTO TinBot(Repeater) is not Firewall. **Samsa/Kinnara/Dart Decoy** buys uncertainty, never extra Orders. [Global tiers](../../notes/list-building/force-multipliers-special-abilities-apex-value.md).

## N5.3 peripheral / synchronized / multi-body apex-value update

**G:Jumper apex:** **Posthuman Mk.1 Engineer13/0 + Mk.5 FO13/.5=26/.5** places specialists in two locations but produces **one** Regular Order, not a two-body synchronized attack. Add **Mk.4 HMG30/1.5** for **56/2** attack+FO+recovery positions; or **Mk.2 Sniper26/1.5** for **52/2** with Mk.1+Mk.5, Camo/Infiltration is **NOT automatically Hidden**. In reactive ARO, only one chosen Proxy has unrestricted reaction when both involved. **Pilot-X23/.5+RacerBot Mk-III8/0 each =31/.5 or39/.5**: 20-10 disposable 360º/Deployable Repeater/PARA bodies, parent RemDriver. Unlike a 7pt free Order bot, **RacerBot Mk-III cannot be selected without Pilot-X**. **Apsaras RemDriver20/1 vanilla** buffs **one** eligible REM, not every synchronized unit. **TA OSS disagreement:** RacerBot activation/Orders vs one hard-to-stop cheap posthuman proxy; need actual other gunfighter/recov target for full benefit.

[Whole-game N5.3 Peripheral & Multi-Body Apex/Value guide](../../notes/list-building/peripheral-synchronized-multibody-apex-value.md). Source profiles, dependency and Fireteam tables above remain authoritative; media are opinions.

## Mission performance — battle-report evidence (2026-11-01)

| Mission(s) | Tested composition / scoring mechanism | Evidence |
|---|---|---|
| **Decapitation** | Maximus heavy gun, Asura and Danavas hacking, Sofotect/Netrods enabled 6–4 vs Corregidor. | [#211](../../notes/battle-reports/211-220-n5-battle-report-tactical-analysis.md) |
| **Hardlock / multi-console counterexample** | Maximus's strong lane cannot replace several protected console operators; Saladin Haqq's cheap specialists achieved more console value. | [#081](../../notes/battle-reports/081-090-n5-battle-report-tactical-analysis.md) |
| **Neutralization / endgame presence** | Maximus suppression and cheap supporting REMs retained board presence after Asura was lost. | [#191](../../notes/battle-reports/191-200-n5-battle-report-tactical-analysis.md) |

**Limits:** The played combination was vanilla ALEPH; do not attribute all its units to OSS or Steel Phalanx. Game-era qualitative evidence, not a win-rate or current Fireteam claim. [Full mission evidence audit](../../notes/battle-reports/cross-report-mission-performance-by-sectorial.md).

## Counterplay — observed N5 battle-report responses (2026-11-02)

| Threat / target | Observed response and limitation | Battle reports |
|---|---|---|
| **Against forward Moran/Jazz network** | Maximus+Asura/Danavas Spotlight+Guided attacked Moran/Koala positions and supported a 6–4 Decapitation result vs Corregidor; maintain backup Specialist routes. | [#211](../../notes/battle-reports/211-220-n5-battle-report-tactical-analysis.md) |
| **Elite defenders / smoke screening** | Maximus and Asura plus tech/Netrods are effective when the shooter is protected from E/M/hidden flank; Saladin Haqq was able to outscore Maximus in Hardlock. | [#081](../../notes/battle-reports/081-090-n5-battle-report-tactical-analysis.md), [#191](../../notes/battle-reports/191-200-n5-battle-report-tactical-analysis.md) |
| **Hero vulnerability** | Vanilla ALEPH's elite investment can be disrupted by multiple hidden short-attack and anti-tech screens; don't treat all-In hero losses as proof another faction generally beats ALEPH. | [#081](../../notes/battle-reports/081-090-n5-battle-report-tactical-analysis.md), [#211](../../notes/battle-reports/211-220-n5-battle-report-tactical-analysis.md) |

**Limit:** #211 was an unusual played vanilla ALEPH roster, not automatically an OSS legal Fireteam. These are historical qualitative interactions, not present N5.3 unit, Fireteam, or win-rate claims. [Full cross-report counterplay analysis](../../notes/battle-reports/n5-cross-report-counterplay-tags-hi-hacking-camo-impersonators-fireteams.md).

---

## Must-have / Go-to / Avoid — source-backed recommendations (2026)

Dated media-backed tactical judgments and miniature purchasing advice. These are qualitative opinions, **not roster/profile/Fireteam authority**; use the canonical N5.3 data above for legality.

**Original audit title:** ALEPH N5.3 — Must-have / Go-to / Avoid (YouTube and podcast evidence)

**Audit:** 23 October 2026. **Armies:** [Vanilla ALEPH](aleph.md), [Operations Subsection (OSS)](operations-subsection.md), and [Steel Phalanx](steel-phalanx.md). Current legality, profile, points, SWC, and Fireteams come from pinned **N5.3 / Army 7.26246.159 (3 September 2026)**, not video captions. Cross-check the detailed [Vanilla guide](../../notes/factions/vanilla-aleph.md), [OSS guide](../../notes/factions/operations-subsection.md), and [Steel guide](../../notes/factions/steel-phalanx.md). Podcast and YouTube statements are **players' assessments**, not measured inclusion rates.

**Method:** Independently retrieved via MCP the [June 2026 Robert Shepherd/Jordan faction-tier transcript](https://www.youtube.com/watch?v=1dW3i9dpI34), [Tactical Awareness S3 E44 OSS YouTube](https://www.youtube.com/watch?v=Jh4jVsFoHN4) and [podcast transcript](https://open.spotify.com/episode/3E6Og0ydRErBokXHYOG6PG), [Tactical Awareness Owen's Adepticon Vanilla ALEPH interview](https://open.spotify.com/episode/0YhA9K7K2xJkiCzqI7PcbV), [MetaChemistry OSS first impressions](https://open.spotify.com/episode/5ynZcV8kOHiVfemyiaOLak), [WIP12 OrderMonkey OSS](https://open.spotify.com/episode/1lx8buKkqrLgCwZB6CaSLZ), [CNN Steel Phalanx N5 deep dive](https://www.youtube.com/watch?v=6RBi4U3t-WQ), and [Robert Shepherd Steel Phalanx N4 focus](https://www.youtube.com/watch?v=764JXbnQ3jQ). The [Yellow Snake/RXron Oct 2025 Steel episode](https://www.youtube.com/watch?v=DcCXt508-CU) **failed direct YouTube transcript retrieval in this audit**; its published example lists and prior guide's notes can corroborate, but are *not* independently transcript-confirmed here. Earlier N4 material describes enduring play patterns only.

**Labels:** **Must / near-must** means a speaker calls it almost automatic or it recurs as a backbone across distinct builds; a strategically coherent omission is still possible. **Go-to** means widely useful, not “take every row.” **Avoid** means a *particular build, profile, or use* is directly criticized by a presenter or defeated by a current rules/profile check. **No confirmed never-take** is better than inventing a dominated whole unit. All three armies need Orders, meaningful attacks, and specialists; not necessarily the same named purchase.

### At a glance

| Roster | Most defensible near-must | General go-to purchases | Source-supported avoidance |
|---|---|---|---|
| **Vanilla ALEPH** | **Posthumans Mk1 Engineer13 + Mk4 HMG30**; 6pt Netrod / 7pt Lamedh cheap-order base; **Apsaras LT20** *when not using a premium LT architecture* | Pilot-X23 + RacerBots8, Tarkshya34/41, Myrmidon Smoke16, Penthesilea28, Marut86/90, Danavas22, Naga FO25, Zayin19 | No universally condemned current unit. Do not pay for vanilla **FTO** solely expecting a Fireteam. Old Dakini recommendations are illegal. |
| **OSS / OperationS** | **Posthumans Mk1 + Mk4**; **Pilot-X + RacerBots** is the clearest *explicit “auto-include” opinion*; cheap Lamedh/Netrod infrastructure | Sharvara15, Dikpala13, Apsaras LT20/TAGCom18, Tarkshya34/41, Asura HD+63/67, Zayin19/24, Riksha20/24, Artalis23, Naga25–29 | **Naga MULTI Sniper29** is *criticized* against Dasyu34 in the May 2026 podcast but **not strictly dominated** after checking full N5.3 profiles; **Samekh FTO** is **not Guided**. No defensible blanket never-take. |
| **Steel Phalanx** | **Netrods6 / Lamedh7** cheap-order shell; **Myrmidon Officer** near-default *when Eclipse/CoC is needed*. **No individual hero** qualifies as universal. | Ajax FTO39, Phoenix, Machaon, Agamemnon63/65, Thorakitai FO13, Dactyl19–20/Acmon, Agêma ML/Atalanta, Scylla32, Eudoros | Avoid **redundant expensive hero bricks** or an unsupported **Scylla FTO** profile taken for its link label; no verified current universally bad whole unit. |

### 1. Vanilla ALEPH

#### Must / near-must

| Choice | Why; qualification | Direct recording |
|---|---|---|
| **Posthumans, especially Mk1 Engineer13 + Mk4 HMG30** | **Highest confidence.** BS14, ARM5 HMG and WIP15 repair in *one G:Jumper combat-group slot*, with optional Mk5 FO13/Mk2 hacker22. Shepherd/Jordan emphatically call Posthumans exceptional slot economy; TA describes cheap support with a premium combat proxy. **Not literally mandatory** in a very specialized list or if the role is supplied elsewhere. Automated captions sometimes call Mk4 “Mk5 HMG”; **Mk4 actually has the HMG**. | [Shepherd/Jordan June 2026, ALEPH/OSS segment ~3:06–3:33](https://www.youtube.com/watch?v=1dW3i9dpI34); [TA S3 E44 ~29–31min](https://open.spotify.com/episode/3E6Og0ydRErBokXHYOG6PG) |
| **Netrod6 + Lamedh7 order shell** | The cheap Regular-order floor gives high-cost attackers enough activations. Owen's actual Adepticon-winning Vanilla list illustrates that this infrastructure (also Probot Baggage8) is part of the engine, not just filler. Exact counts vary: Netrods are Combat Jump in deployment; Lamedh creates a Repeater/Flash Pulse and can expose hackers if carelessly placed. | [TA Adepticon-winning Vanilla ALEPH list (April 2025)](https://open.spotify.com/episode/0YhA9K7K2xJkiCzqI7PcbV); [Shepherd/Jordan 2026](https://www.youtube.com/watch?v=1dW3i9dpI34) |
| **Apsaras LT20 — *near-default, not general must*** | June reviewers explicitly call the new cheap usable LT a transformative removal of Vanilla's former costly-LT bottleneck. KHD/Firewall and RemDriver offer genuine utility. **Skip for a deliberate Marut Strategos, Asura, TAG Maximus or other LT plan**; one-Wound hackable LT can still cause Loss of Lieutenant. | [Shepherd/Jordan 2026 ~3:06–3:30](https://www.youtube.com/watch?v=1dW3i9dpI34) |

#### Go-to (when its role is needed)

| Unit/profile | Why, and when to leave it out | Evidence |
|---|---|---|
| **Pilot-X23/.5 + RacerBot8 ×1–2** | Fast Repeater/PARA pressure and up to three Regular bodies in same Combat Group; strong against exposed HI/TAG and for distributing a network. Full trio **39/.5**, not free bots. Skip if prone to hostile KHD/repeater contamination or points/slots are tight. | [TA S3 E44 ~24–29m](https://open.spotify.com/episode/3E6Og0ydRErBokXHYOG6PG); [Shepherd/Jordan](https://www.youtube.com/watch?v=1dW3i9dpI34) |
| **Tarkshya VH34/0 or 41/1.5** | 3STR aerial MSV1 Mimetism(-6), resilient operator fallback; cheap 34/0 uses angles/Suppressive Fire, 41pt Red Fury is better sustained attacker. **VH No Cover, a large model and hacking remain real weaknesses.** Reviewers rate its aerial package among the best; choose it when flexible attack beats TAG bulk. | [Shepherd/Jordan 2026](https://www.youtube.com/watch?v=1dW3i9dpI34); [TA S3 E44 ~91–96m](https://open.spotify.com/episode/3E6Og0ydRErBokXHYOG6PG) |
| **Myrmidon Smoke16; Penthesilea28** | These are Vanilla's major added dimensions relative to OSS: cheap smoke for Marut/MSV and melee/fast smoke-specialist flanking that avoids a hackable robot's route. Penthesilea can attack and score, not merely taxi smoke. Skip if no practical visual/CC plan. | [Shepherd/Jordan 2026, ALEPH vs OSS discussion](https://www.youtube.com/watch?v=1dW3i9dpI34); [Vanilla research guide](../../notes/factions/vanilla-aleph.md) |
| **Marut86/1.5 or LT90/2** | BS15 MSV2, Tactical Awareness, ARM8/BTS9, plus *Vanilla smoke* makes decisive favorable gunfights; LT offers Strategos L2. Needs orders, repair, hacking protection and optional Shukra CoC. Not a small-game/default purchase. | [TA Vanilla faction guide (N4 strategic principles)](https://www.youtube.com/watch?v=NPlK-e2B1Io); [June 2026 faction comparison](https://www.youtube.com/watch?v=1dW3i9dpI34) |
| **Danavas HD+ Pitcher22/.5; Naga FO25 / Dasyu FO29; Zayin TR19/24** | Diverse repeatable roles: ranged hacking/White Noise; mission infiltrator; repairable Total Reaction lane. Owen demonstrates Danavas+Probot+missile package works, *not* that Guided is always worthwhile. Naga vs Dasyu depends on role, budget and concealment. | [TA Adepticon 2025](https://open.spotify.com/episode/0YhA9K7K2xJkiCzqI7PcbV); [TA S3 E44](https://open.spotify.com/episode/3E6Og0ydRErBokXHYOG6PG) |

#### “Never take” audit

- **No current unit-level universal veto is supported.** Do not promote old Maximus skepticism into a present “never”: the 2026 TAG received substantial AP gun updates. [TA S3 E44](https://open.spotify.com/episode/3E6Og0ydRErBokXHYOG6PG) and [OSS/Vanilla tactical guide](../../notes/factions/vanilla-aleph.md) document the new role.
- **Do not pick FTO Agent Maximus or FTO Rudra specifically for a Vanilla Fireteam bonus**; pinned Vanilla reference has **no ordinary Fireteam**. An FTO profile may still have a viable weapon/cost role without linking.
- **Do not copy a Dakini-centered Vanilla N4/N5.0 list**: Dakini is no longer in current Vanilla roster. This is **unavailable**, not a current inferior unit.

### Cross-army takeaways

1. **The least debatable generic ALEPH value is Posthumans where available, cheap Regular Order infrastructure, and a repair/network plan.** Steel Phalanx substitutes its compact, complementary Myrmidon/Thorakitai architecture for the OSS/Vanilla Posthuman engine.
2. **Most credible explicit “auto-include” claims in retrieved *modern* media:** Pilot-X in the May 2026 [Tactical Awareness OSS episode](https://open.spotify.com/episode/3E6Og0ydRErBokXHYOG6PG); **15pt Sharvara** is emphatically favored around 75m; the June [Shepherd/Jordan](https://www.youtube.com/watch?v=1dW3i9dpI34) review calls Posthumans extraordinary but *does not establish literal 100% tournament usage*.
3. **Profile-specific versus unit-level “never”:** A bad support purchase (EVO without targets, FTO without a legal/useful link, expensive hacker redundant with an Asura, Guided missile without Spotlight), or a duplicate gun, **does not prove the parent unit is universally bad**. Preserve disagreement, especially the Naga sniper/Dasyu sniper comparison.
4. **Current rules beat old voices on legality:** No Dakini in September ALEPH/OSS; Mk4 HMG and Mk5 FO; OSS Asura HD+ LT exists whereas **Vanilla's Asura LT is AP Spitfire**, not HD+; Steel's Agamemnon is its sole standard TAG; current Core member cap and FTO restrictions apply.

### Whole-unit purchasing audit — entire model, not single profile (2026-10-30)

**Result: no defensible all-profile, current-roster whole-unit avoid** in Vanilla ALEPH, Operations Subsection or Steel Phalanx based on the sources above. That is a positive outcome of checking the actual alternatives, **not** a missing category.

| Army | Full-model purchasing decision | Why the apparent “avoid” is not a model ban |
|---|---|---|
| **Vanilla ALEPH** | **No unit to blacklist** | FTO Maximus/Rudra cannot gain a non-existent Vanilla team bonus, but may still have a viable standalone profile. Post-update Maximus has real improved combat options; old Dakini is **unavailable** rather than an avoidable *current* model. |
| **OSS** | **No unit to blacklist** | Naga sniper versus Dasyu is disputed (+1SD versus Hidden/BS); Samekh **FTO** lacks Guided while normal Samekh **has Guided**. Yaksha's cost is contested, not all-profile dominated. |
| **Steel Phalanx** | **No unit to blacklist** | Scylla FTO sacrifices Charybdis, but standard Scylla + Charybdis and supported FTO configurations remain useful. Expensive duplicate hero teams are a **shopping/list architecture** problem, not proof an individual hero sculpt is bad. |

**Practical collection advice:** defer a pricey hero or TAG when you already own another **for the same battlefield job**, but label that as **redundancy**, not “never take” evidence. [Cross-faction buying shortlist](../../notes/factions/model-purchase-avoid-summary-2026.md).

### Worst-value, rarely needed and proxy-first miniature purchases by army (2026-10-30)

This section answers a **miniature-buying** question separately from Army list selection: which **complete units** are low-priority purchases, which **specific profiles** are weak without making their parent unit bad, which **legitimate but mission-dependent models** merit a proxy before buying, and which **extra copies** are not worth purchasing merely because AVA allows them? Cover all three N5.3 armies: **Vanilla ALEPH, Operations Subsection (OSS), Steel Phalanx**. *Rare* means situational or not needed for the source-backed standard list structures—not a measured frequency or tournament pick-rate claim. **No unit in the checked evidence is conclusively worthless across all current profiles**.

**Confidence labels:** **Strong profile avoid** is a direct negative reviewer comparison or a demonstrated profile/Fireteam mismatch; **Defer whole miniature** means its usual niche is less important to an initial collection, not mathematical domination; **Proxy first** is a **reasoned collection recommendation**, not a claimed literal podcast quote; **Contested** explicitly preserves contrary opinion or a post-review update; **Extra-copy defer** means the first model may be excellent. Roster, profile, availability and Fireteam facts use the [September 2026 Vanilla](aleph.md), [OSS](operations-subsection.md) and [Steel](steel-phalanx.md) references; dated commentators provide preferences. The linked [whole-model purchase audit](#whole-unit-purchasing-audit--entire-model-not-single-profile-2026-10-30) continues to apply.

#### 1. Vanilla ALEPH — mostly opportunity-cost, not outright bad whole units

| Unit / loadout / collection plan | Why weak or circumstantial; competing job and evidence | Purchasing decision |
|---|---|---|
| **Agent Maximus FTO or Rudra FTO bought *for a Vanilla Fireteam*** | **Legality warning, not power ranking:** the current Vanilla roster has **no normal Fireteam** for that FTO label. The corresponding solitary profiles can still be efficient for their weapon/role. [Pinned Vanilla](aleph.md). | **Do not purchase for an imaginary link bonus**. Proxy the profile if its *standalone* gun/support benefit is interesting. **Do not skip Maximus or Rudra as complete units**. |
| **A second premium centerpiece when Marut86–90 or TAG Maximus80–82 already carries the list** | **Reasoned:** [Vanilla tactical guide](../../notes/factions/vanilla-aleph.md) describes Marut BS15/MSV2/smoke, updated Maximus AP and support, and fast **Tarkshya34–41 VH** as *different attack investments*. A Marut + Maximus + extra Asura usually leaves too little scoring, Engineer access and safe Order supply. A TAG Maximus and Agent Maximus are **mutually exclusive** where current Army says so. | **Proxy-test another expensive TAG or Asura before buying**, not a veto on its first useful profile. Purchase the *specific* platform regularly fielded; do not buy all expensive chassis for one archetype. |
| **Tarkshya aerial Vehicle used as an unsupported Turn-1 ARO breaker** | **Strong positive model, risky specific job:** the praised 34/0 and 41/1.5 profiles use mobility, MSV1, Mimetism(-6) and 3STR, but a **VH with No Cover and hacking vulnerability** can fail badly when it starts the first face-to-face against defended long lanes. [Shepherd/Jordan 2026](https://www.youtube.com/watch?v=1dW3i9dpI34); [Tactical Awareness OSS](https://open.spotify.com/episode/3E6Og0ydRErBokXHYOG6PG) values the aerial angle. | **Proxy first if the sole reason to buy is “I need another gun.”** Buy if a recurring map/mission permits superior flank/height angles. **Tarkshya is a Vehicle, not a TAG or normal S2 infantry proxy.** |
| **Naga, Dasyu, Dart, Thyreos, Samsa and Yaksha *all* purchased for the same midfield specialist niche** | **Reasoned, not a tier-Z list:** **Naga FO25** is an efficient camo scorer; **Dasyu FO29** brings different Hidden Deployment/Mimetism; **Thyreos FO22** is economical; **Dart42** can include Sharvara K-9; **Samsa26** has Decoy/plasma; **Yaksha23–31** is a debated forward trap platform. Some have mine/CC/anti-armor tasks none of the others duplicate. [Vanilla guide](../../notes/factions/vanilla-aleph.md). | **Proxy the *second, third and rare specialist type*** before buying its dedicated sculpt. **Do not skip a first Naga/Thyreos or Dasyu when that deployment rule wins the mission**; only buy Dart + animal/peripheral package when the selected card actually includes it. |
| **Yaksha as an automatic primary midfield purchase** | **Contested direct review theme:** [Tactical Awareness OSS](https://open.spotify.com/episode/3E6Og0ydRErBokXHYOG6PG) debates its higher cost beside Naga/Dasyu/Dart/Pilot-X; Yaksha's ARM4, Forward Deployment and mine/MadTrap/E/M specialty are genuine defensive answers. Vanilla has similar opportunity cost. | **Defer/Proxy first**, unless your intended list specifically needs a **durable forward one-use-Camo trap**. Not a supported all-profile avoid. |
| **Probot17 Total Reaction, Probot14/.5 EVO, or another Samekh16/1.5 Guided chassis without a support/Targeted plan** | **Role-specific:** **Probot8 Baggage/Repeater** may be worth buying immediately, but **EVO** only matters with real Supportware recipients; high-burst Probot duplicates a genuine **Zayin19/24** defensive job. **Samekh** Guided needs actual Spotlight/FO/repeater reach, Orders and SWC; Danavas/Pilot-X may support it but it is not free. [Vanilla guide](../../notes/factions/vanilla-aleph.md). | **Avoid unsupported *profile/strategy*, not all Probots/Samekhs.** **Proxy missile/EVO variants using appropriately sized existing REM chassis** before buying extra bodies. |
| **Expensive second Doctor/Engineer character** (Parvati, Sophotect, Claire, Johnny Kao, Trisha) | **Reasoned:** **Posthuman Mk1 Engineer13** is exceptionally economical; **Sophotect**, **Parvati**, **Claire**, **Johnny Kao** and **Trisha** have different resilience, doctor/recovery, engineering, mines or support. Paying all those upgrades merely to stand behind the same TAG may overspend compared with independent scoring. | **Proxy-test the *additional* named support figure**, not the first Engineer that keeps a major TAG/REM working. Buy when the **specific Doctor+Engineer, TAG protection or mission** capability is repeatedly needed. |
| **John Hawkwood CoC40 as automatic insurance; Shukra CoC21 for a fully protected cheap LT** | **Reasoned:** Hawkwood adds separate combat/command value but is a very expensive way merely to get CoC; **Shukra CoC21/0** is already an optional hedge, not a universal tax. **Apsaras LT20** and high-cost Marut/Asura LT create very different Loss-of-Lieutenant risks. [Vanilla guide](../../notes/factions/vanilla-aleph.md). | **Proxy named command insurance first** if the list does not actually need that succession plan. **Do not blacklist Hawkwood or Shukra** where a vulnerable elite LT makes CoC valuable. |
| **Posthumans bought as every single Mk1/Mk2/Mk4/Mk5 sculpt for “extra Orders”** | **Very strong underlying unit, wrong physical/accounting assumption:** the **Mk1 Engineer13 and Mk4 HMG30** are source-backed favourites, while **Mk2 hacker / Mk5 FO** expand different roles. **G:Jumper Proxies occupy one troop/slot structure, not one new Regular Order per body**. [Shepherd/Jordan 2026](https://www.youtube.com/watch?v=1dW3i9dpI34), [Tactical Awareness](https://open.spotify.com/episode/3E6Og0ydRErBokXHYOG6PG). | **Prioritize physical Mk1/Mk4 equivalents; proxy the optional Mk2/Mk5 variants initially**. Buy additional bodies only when they are part of your regularly used *legal* Proxy selection. Do **not** call Posthumans a poor purchase. |
| **Legacy Dakini infantry or a “Vanilla Dakini Core”** | **Removed/illegal in this pinned Vanilla roster**, not a legitimate N5.3 avoid rating. Older N4/N5.0 lists are unusable without replacing the unit. [May 2026 roster update](https://infinityuniverse.com/en/news/army-update-mazebreaker). | **Do not buy Dakini *for current standard Vanilla lists***. A Dakini miniature might be an acceptable model proxy for another **legal REM**, subject to base/silhouette and event rules; the proxy doesn't restore removed Army access. |

**Highest-confidence positive purchases to preserve:** a practical **Posthuman Mk1/Mk4 package**, **Netrod6 and Lamedh7** order infrastructure, **Apsaras LT** for the cheap-command architecture, a suitable **Myrmidon Smoke** provider, **Pilot-X + RacerBot(s)** if the network is part of your plan, and *one chosen* premium attack engine. These are recommendations to keep, not extra models to acquire indiscriminately. Evidence: [2026 reviewer discussion](https://www.youtube.com/watch?v=1dW3i9dpI34), [Tactical Awareness OSS/Vanilla](https://open.spotify.com/episode/3E6Og0ydRErBokXHYOG6PG), [Vanilla note](../../notes/factions/vanilla-aleph.md).

#### Cross-ALEPH — good units, rare loadouts and economical proxy substitutions

**Owned-model coverage:** Steel Phalanx counts above come from the checked-in [actual inventory](../../inventory/steel-phalanx.md). No equally authoritative current **Vanilla ALEPH or OSS inventory** was found at the expected paths; thus no ALEPH/OSS owned unit counts are inferred. A suggested **“spare OSS model”** for Hippolyta does **not establish** which OSS models are physically owned.

| Buying opportunity | Better initial proxy or reuse | When a separate miniature becomes sensible |
|---|---|---|
| **Posthuman Mk1/Mk2/Mk4/Mk5 / extra Proxy sculpts** | Use distinct appropriately sized *G:Jumper body* stand-ins, each declared as Mk1 Engineer, Mk2 specialist, Mk4 HMG or Mk5 FO. Their exact silhouettes may differ and are **not one freely interchangeable physical base**. | Buy the exact Proxy Mk bodies that appear **together** in the 2–3-body combination you routinely field; **one proxy selection doesn't make 3 independent Regular Orders**. |
| **Named S2-scale heroes and support characters** (Apsaras, Sophotect, Danavas, Parvati, Claire, Shukra, Thamyris, Hippolyta, Atalanta, Ajax, Phoenix, Machaon, etc.) | Use a *distinct*, correctly based/silhouetted legal Corvus Belli miniature from the same collection, with named identity and profile stated. Check especially **large HI** and any non-S2 Silhouettes rather than assuming all heroes are S2. | When using multiple named characters **simultaneously**, the proxy isn't visually distinct, event demands closer match, or the character becomes a regular purchased favourite. |
| **Common Fireteam gun/scoring variants** (Myrmidon, Officer, Thorakitai, Yadu, Deva, Makhai, Hoplite, Posthuman Mk) | Declare the equipped profile clearly and reuse a correct-size mini **of the same troop family** for an alternate rifle/HMG/Doctor/FO/FTO card where allowed. **Only use troop families actually available in the selected ALEPH roster**; never treat a proxy as granting faction access. | Only buy another exact weapon sculpt when the chosen team needs **different bodies simultaneously**, or the organizer requires greater WYSIWYG clarity. |
| **REM chassis** (Lamedh, Daleth, Zayin, Samekh, Probot, Riksha, Dikpala, Rudra) | Test with spare compatible-size bots: **Steel has two ALEPH Rebots plus four shared PanO Dronbots, and two PanO Mulebots as potential Probot stand-ins**. Specialized support bots **may differ in size** from large combat REMs and tiny RacerBots. | Buy a distinct chassis if its **silhouette/base or simultaneous count** cannot be met, or you play REM-skew lists often. Do not assume every REM uses the same base. |
| **Multi-body teams and peripherals**: Scylla + Charybdis, Pilot-X + RacerBot(s), Arjuna + KiranBot(s), Dart + Sharvara K-9, Agamemnon + Karkata, Engineer/Doctor + Yudbot | Declare/physically represent **each fielded model and its controller**; the main figure cannot “stand for” all extras at once. **RacerBot additional Regular Orders differ from ordinary Servant/KiranBot/Charybdis order accounting**; consult exact current options. | Buy complete partners once you regularly field the combination and lack enough correctly based stand-ins. **Steel Charybdis1 and Yudbots2 already exist; Karkata0 has Crabbot proxy; Arjuna0/KiranBots0**. |
| **Heavy/TAG models**: Marut, Maximus TAG, Agamemnon; **Tarkshya Vehicle** | Proxy/borrow **correct silhouette and base** models to test a TAG-heavy list. **Steel already has Agamemnon1**; it is **not a Marut/Maximus TAG legal listing** and one large model cannot be two separate TAGs simultaneously. Tarkshya is a **Vehicle**, not a TAG. | Buy a new large model when its **specific legal roster, physical size and attack role** recur. A large TAG model with the wrong silhouette isn't a drop-in substitute at an organized event. |
| **Scylla variants / Agent Maximus vs TAG Maximus / Apsaras options / Samekh FTO vs Guided** | Most are **profile choices**, not simultaneously fielded separate named models. **Scylla FTO without Charybdis** is not the same as the **paired** option; **Agent/TAG Maximus** cannot both be selected; **Samekh FTO does not become Guided**. | Buy alternate sculpts only if a second separate legal body is needed concurrently and current event proxy rules require it. Models cannot create missing traits or legal permissions. |
| **Retired Dakini miniatures, extraneous FTO sculpts, Spec-Ops/Team-Ops** | Reuse Dakini **only as a clearly declared legal trooper proxy** with suitable Silhouette/base; optional game modes require explicit event permission. FTO status requires current roster profile and a real **sectorial Fireteam**. | No reason to buy **illegal old Dakini or optional-mode-only minis for current standard ALEPH/OSS**. |
| **Sculpt quantity to AVA** (Steel Myrmidon6, Ekdromoi4, Thorakitai6, etc.) | Start from your **actual 300pt list** and physical **simultaneous model count**. One real Myrmidon Officer represents one trooper; it cannot physically represent two different units deployed simultaneously. | Buy duplicates when proven necessary in repeated, legal list builds, not because a spreadsheet has “missing to AVA.” |

**Proxy safety and legal limits:** announce all substitutes before play; verify selected N5.3 **unit access, exact Fireteam option, Silhouette, base, physically represented secondary figures and troop count**. Check current tournament/ITS/organizer proxy conditions for organized play rather than claiming any old season's blanket rule. A model can be a proxy for another unit when legally represented and accepted; **it cannot lend weapons/skills, faction access, an unavailable Fireteam, extra Orders or missing extra bodies**.

**Bottom line for purchases:** There are **no transcript-proven universal ALEPH whole-model “never buys.”** Best direct **profile-only** skips are **OSS Samekh FTO *if the objective is Guided***, **Steel Scylla FTO *if the expectation is included Charybdis*** and **Vanilla/OSS imaginary FTO Fireteams**; the **Naga sniper vs Dasyu** is *contested*, not a settled Naga verdict. Best **whole-model deferral / proxy-first tests** are **OSS Yaksha when a cheap infiltrator suffices**, **Tarkshya when bought only as an early ARO breaker**, **additional expensive Asura/TAG/hero alternatives**, and **Steel Hippolyta/Arjuna+KiranBot/Sāchā / surplus AVA copies** given the actual inventory. Do **not** convert a weak loadout into advice to skip **Posthumans, Myrmidons, Deva/Yadu, Scylla, Agamemnon or ordinary ALEPH scoring/support REMs**.
