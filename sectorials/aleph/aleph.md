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
