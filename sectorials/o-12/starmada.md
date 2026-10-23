---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 1002
sectorial_slug: starmada
sectorial_name: Starmada
parent_faction: O-12
rules_baseline: N5.3
army_source_version: "7.26246.159"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Complete standard Starmada roster, standard loadouts/profile states and peripherals, canonical Fireteam chart, exact FTO restrictions, reverse Fireteam access, optional-mode hooks, and Reinforcements boundary. Generic Soldier of Fortune catalog entries are excluded."
---

# Starmada — N5.3 sectorial reference

## Overview and provenance

This file is the repository reference for **Starmada, Bureau Aegis Naval Police Department** (Army sectorial ID `1002`). It is intended to be sufficient for ordinary roster, AVA, points/SWC, profile, dependency, and Fireteam-legality questions without reopening Army.

Primary data source:

- Corvus Belli Army data snapshot mirrored by `massayoshi/infinity-army-backup`.
- Pinned source commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` (`army: N5.3 + ITS18`).
- Army dataset: `n5/starmada/7.26246.159.json`.
- Source blob: `995037912a4871ef301469d701b9006bbea3371d`.
- Army version: **7.26246.159**.
- Sectorial ID: **1002**.
- Parent O-12 ID: **1001**.
- Reinforcements list ID exposed by the dataset: **1099**.
- Cross-check/reference model commit: InfinityDB `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: **N5.3 + N5 FAQ v0.1**.

Coverage policy:

- The **42 standard logical roster entries** whose faction availability includes Starmada are included below.
- Generic Soldier-of-Fortune catalog records present in the aggregate payload with `factions: []` are excluded.
- **Ŝtormo Spec-Ops** and **O-12 Team-Ops** are optional-mode hooks, not ordinary matched-play roster entries.
- Reinforcements (`army_id: 1099`) remain distinct from the normal Starmada roster and Fireteam chart.
- Composite states and Peripherals stay under their parent logical unit rather than being counted as separate roster entries.
- Fireteam legality comes from the canonical chart below, not from an `FTO` label alone.
- Where Army marks multiple rows `required: true`, this file follows the repository convention and treats them as a **required source-choice set**: a legal Fireteam needs a member from that required set; every marked row is not simultaneously mandatory.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Starmada |
| Parent faction | O-12 |
| Army ID | 1002 |
| Rules baseline | N5.3 + N5 FAQ v0.1 |
| Army source | 7.26246.159 |
| Standard logical roster units | 42 |
| Optional-mode records | 2 |
| Reinforcement roster | yes — Army ID 1099 |
| Fireteam chart | yes |

## Fireteam limits and interpretation

| Constraint | Value / wording |
|---|---|
| Core | up to 1 Core |
| Haris | up to 1 Haris |
| Duo | effectively unlimited (`256` in Army source) |
| Fireteam families | Security; Nyokas; Betatroopers; Bronzes; Varangian Guards; Road |
| Wildcards | PSI-COps; Shona Carano; Parvati; Tian Gǒu FTO |
| Main/Reinforcement mixing | Keep normal Starmada and Reinforcement charts distinct |

Important profile-level restrictions:

- **Nyoka Fireteam row is `NYOKA FTO`**: only Nyoka options `3` and `4` may use that Fireteam access. Options `5` and `6` are not FTO.
- **Knight of Santiago access in Bronzes is `KNIGHT OF SANTIAGO FTO`**: options `1`, `2`, `5`, and `6` only. The unit source explicitly states that Combat Jump options cannot be part of a Fireteam; options `3` and `4` are therefore excluded.
- **Vidocq access in Security and Bronzes is `VIDOCQ FTO`**: options `1`, `2`, and `3` only; option `4` is not FTO.
- **Tian Gǒu Wildcard access is `TIAN GǑU FTO`**: options `1`, `3`, `4`, and `6` only.
- The Security/Bronze rows say **`MENT`**, not `MENT FTO`; all Starmada Ment options are legal in those chart rows.
- `FTO` in a profile name does not create Fireteam access unless the chart grants it.

## Standard roster index

| Unit ID | Unit | AVA | Troop type | Classification | Regularity | Fireteam access / notes |
|---:|---|---:|---|---|---|---|
| 1465 | Peeler Copperbots | 1 | REM | Support Troops | Regular | — |
| 1872 | Tinkers, Maintenance Support Company | 1 | LI | Support Troops | Regular | — |
| 1536 | Tian Gǒu, Orbital Activity Squad | 1 | LI | Spec. Trained Troops | Regular | Wildcard, **FTO options 1/3/4/6 only** |
| 1505 | Shona Carano | 1 | MI | Character | Regular | Wildcard |
| 1529 | Bluecoats | 4 | LI | Line Troops | Regular | Security |
| 1857 | Firebat Attack Wing | 1 | VH | Elite Troops | Regular | — |
| 27 | Knights of Santiago | 1 | HI | Elite Troops | Regular | Bronzes, **FTO options 1/2/5/6 only** |
| 1462 | Cyberghosts | 1 | LI | Support Troops | Regular | — |
| 1456 | Betatroopers | 5 | HI | Veteran Troops | Regular | Betatroopers |
| 1610 | Ŝarko | 2 | SK | Spec. Trained Troops | Regular | — |
| 1611 | Sekudroids | 2 | REM | Spec. Trained Troops | Regular | Security; Betatroopers; Bronzes |
| 1517 | Ensign Katherine Cho | 1 | LI | Character | Regular | Security |
| 1609 | RoadBots Highway Patrol | 2 | REM | Spec. Trained Troops | Regular | Road |
| 1461 | Varangian Guard | 2 | WB | Mercenary Troops | Regular, Impetuous | Varangian Guards |
| 754 | Hector | 1 | HI | Character | Regular | Nyokas; Betatroopers |
| 788 | Andromeda | 1 | MI | Character | Regular | — |
| 1588 | Raveneye Officers | 2 | LI | Support Troops | Regular | Security |
| 1530 | Lawkeepers | 2 | LI | Spec. Trained Troops | Regular, Impetuous | Road |
| 1773 | Vidocq | 2 | LI | Spec. Trained Troops | Regular | Security; Bronzes, **FTO options 1/2/3 only** |
| 192 | Yudbots | 2 | REM | Support Troops | Peripheral | Servant support unit |
| 1535 | Saladin, Naval Liaison Officer | 1 | MI | Character | Regular | — |
| 1533 | Raptor Boarding Squad | 4 | HI | Veteran Troops | Regular | Includes Devabot |
| 1458 | Zeta Unit | 1 | TAG | Mechanized Troops | Regular | Includes ZetBot |
| 1464 | Oko Copperbots | 2 | REM | Support Troops | Regular | Road; counts as Lawkeepers |
| 1463 | Specialized Support Unit Lambda | 2 | LI | Support Troops | Regular | — |
| 1467 | Kyttä Copperbots | 1 | REM | Support Troops | Regular | — |
| 1511 | PSI-Cops | 2 | LI | Veteran Troops | Regular | Wildcard; counts as Security |
| 1469 | FuzzBots | 2 | REM | Support Troops | Regular | — |
| 1454 | Epsilon Unit | 2 | MI | Elite Troops | Regular | Nyokas; Betatroopers |
| 50 | Warcors | 1 | LI | Mercenary Troops | Irregular | — |
| 1534 | Parvati | 1 | LI | Character | Regular | Wildcard |
| 1531 | Nyoka Assault Troops | 5 | LI | Spec. Trained Troops | Regular | Nyokas, **FTO options 3/4 only** |
| 1512 | Crushers | 3 | MI | Veteran Troops | Regular | — |
| 1483 | Casanova | 1 | LI | Character | Regular | — |
| 1768 | Ment Agents | 1 | LI | Spec. Trained Troops | Regular | Security; Bronzes; all options |
| 1466 | Millicent Copperbots | 1 | REM | Support Troops | Regular | — |
| 1532 | Bronzes | 3 | HI | Veteran Troops | Regular | Security; Nyokas; Bronzes |
| 1767 | Jackboots | 2 | MI | Veteran Troops | Regular | Security |
| 1774 | Nightshades | 1 | SK | Elite Troops | Regular | — |
| 1447 | Kappa Unit | 5 | LI | Line Troops | Regular | Security |
| 1599 | Bìxié, the Jade Champion | 1 | HI | Character | Regular | Betatroopers |
| 1940 | Ioann Bann, Varangian Dog-Warrior | 1 | WB | Character | Irregular, Impetuous | Varangian Guards; counts as Varangian |

### Optional-mode entries

| Unit ID | Unit | Mode | Fireteam hook |
|---:|---|---|---|
| 1923 | Ŝtormo Spec-Ops | Infinity Spec-Ops | Up to 1 in Security Fireteams |
| 1937 | O-12 Team-Ops | Infinity Team-Ops | Optional-mode only; no normal-roster Fireteam row |

## Unit details

Notation: stats are `MOV CC BS PH WIP ARM BTS VITA/STR S`. Source option IDs are retained because FTO legality and otherwise-similar loadouts can depend on them.

### Peeler Copperbots — `peeler-copperbots`

**Unit ID:** 1465 — AVA 1 — REM, Support Troops.

- **Stats:** `15-10 13 11 10 13 0 3 STR1 3`.
- **Rules/equipment:** Remote Presence, Courage, Total Reaction, Climbing Plus; 360º Visor.
- **Option 1:** **24 / 1** — HMG, PARA CC Weapon (-3).
- **Option 2:** **19 / 0** — Thunderbolt (+1B), PARA CC Weapon (-3).

### Tinkers, Maintenance Support Company — `tinkers-maintenance-support-company`

**Unit ID:** 1872 — AVA 1 — LI, Support Troops.

- **Stats:** `10-10 12 11 10 13 0 3 1 2`.
- **Rules/equipment:** Specialist Operative; Deactivator, GizmoKit, Repeater.
- **Option 1:** **11 / 0** — Adhesive Launcher Rifle, Flash Pulse, Stun Pistol, PARA CC Weapon (-3).

### Tian Gǒu, Orbital Activity Squad — `tian-g-u-orbital-activity-squad`

**Unit ID:** 1536 — AVA 1 — LI, Spec. Trained Troops.

- **Stats:** `10-10 16 12 10 14 2 3 1 2`.
- **Rules/equipment:** Warhorse, Terrain (Zero-G); 360º Visor.
- **Option 1 — TIAN GǑU FTO:** **22 / 0** — Combi Rifle, Jammer, Boarding Pistol, CC Weapon; Holomask. **Wildcard legal.**
- **Option 3 — TIAN GǑU FTO:** **20 / 0** — Boarding Shotgun, Grenades, Jammer, Boarding Pistol, CC Weapon; Holomask. **Wildcard legal.**
- **Option 4 — TIAN GǑU FTO:** **24 / 0** — Thunderbolt (+1B), E/M Carbine, Boarding Pistol, CC Weapon; Holomask. **Wildcard legal.**
- **Option 6 — TIAN GǑU FTO:** **22 / 0** — Combi Rifle, Boarding Pistol, CC Weapon; Killer Hacking Device, Hacker. **Wildcard legal.**
- **Option 8:** **26 / 0** — Thunderbolt (+1B), E/M Carbine, Boarding Pistol, CC Weapon; Holoprojector, Holomask, Surprise Attack (-3). Not FTO.
- **Option 9:** **27 / 0** — Combi Rifle, MadTraps, Boarding Pistol, CC Weapon; Killer Hacking Device, Holoprojector, Surprise Attack (-3), Minelayer, Hacker. Not FTO.

### Shona Carano — `shona-carano`

**Unit ID:** 1505 — AVA 1 — MI, Character.

- **Stats:** `15-5 23 11 14 13 2 3 1 2`.
- **Rules:** Martial Arts L4, Courage, Dodge modifiers, Frenzy, Stealth, No Wound Incapacitation, Super-Jump, Immunity (Shock).
- **Option 1:** **22 / 0** — Submachine Gun, Nanopulser (+1B), Flash Pulse, Pistol, AP + EXP CC Weapon. **Wildcard.**

### Bluecoats — `bluecoats`

**Unit ID:** 1529 — AVA 4 — LI, Line Troops.

- **Stats:** `10-10 20 12 10 13 1 3 1 2`.
- **Rules/equipment:** Courage, Natural Born Warrior, Sixth Sense, Discover (+6); Biometric Visor.
- **Option 1:** **16 / 0** — Submachine Gun, Heavy Riotstopper (+1B), Flash Pulse (+1B), Kobra Pistol, PARA CC Weapon (-6).
- **Option 2:** **17 / 0** — Boarding Shotgun, Heavy Riotstopper (+1B), Flash Pulse (+1B), Kobra Pistol, PARA CC Weapon (-6).
- **Option 3:** **13 / 0** — Adhesive Launcher Rifle, Heavy Riotstopper (+1B), Kobra Pistol, PARA CC Weapon (-6).
- **Option 4:** **16 / 0** — Adhesive Launcher Rifle, Heavy Riotstopper (+1B), Disco Baller, Kobra Pistol, PARA CC Weapon (-6).
- **Option 5:** **25 / 1** — Red Fury, Heavy Riotstopper (+1B), Kobra Pistol, PARA CC Weapon (-6).
- **Option 7 Lieutenant:** **16 / 0** — option-1 weapons; Lieutenant.

### Firebat Attack Wing — `firebat-attack-wing`

**Unit ID:** 1857 — AVA 1 — VH, Elite Troops.

- **Stats:** `20-5 — 13 12 13 4 6 STR2 7`.
- **Rules:** Aerial, Courage, Dodge (-3 source modifier), GizmoKit (PH=13), Mimetism (-6), No Cover, Super-Jump (Jet Propulsion), Terrain (Total), Super-Jump (+7.5), BS Attack (+1SD), NCO, Tech-Recovery.
- **Option 1:** **36 / 0** — AP Submachine Gun, Thunderbolt, Light Rocket Launcher.
- **Option 2:** **35 / 0** — MULTI Rifle, Heavy Riotstopper, Akrylat-Kanone, Blitzen.

### Knights of Santiago — `knights-of-santiago`

**Unit ID:** 27 — AVA 1 — HI, Elite Troops.

- **Stats:** `15-5 23 14 13 13 4 3 2 2`.
- **Rules/equipment:** Frenzy, Martial Arts L1, Dodge (+2.5), Specialist Operative, Stealth, Terrain (Zero-G), Religious Troop; 360º Visor.
- **Source note:** options with Combat Jump cannot be part of a Fireteam.
- **Option 1 — KNIGHT OF SANTIAGO FTO:** **33 / 1.5** — Spitfire, E/M Grenades, D-Charges, Boarding Pistol, DA CC Weapon. **Bronzes Fireteam legal.**
- **Option 2 — KNIGHT OF SANTIAGO FTO:** **31 / 0** — MULTI Rifle, D-Charges, Boarding Pistol, DA CC Weapon; Killer Hacking Device, TinBot Firewall (-3), Hacker. **Bronzes Fireteam legal.**
- **Option 3:** **38 / 0** — Boarding Shotgun (+1B), Flash Pulse, D-Charges, Shock Mine, Boarding Pistol, DA CC Weapon; Combat Jump, Super-Jump (Jet Propulsion), Killer Hacking Device. **Not Fireteam legal.**
- **Option 4:** **36 / 0** — option-3 weapons; Combat Jump, Super-Jump (Jet Propulsion). **Not Fireteam legal.**
- **Option 5 — KNIGHT OF SANTIAGO FTO Lieutenant:** **33 / 0** — Spitfire, E/M Grenades, D-Charges, Boarding Pistol, DA CC Weapon; Lieutenant. **Bronzes Fireteam legal.**
- **Option 6 — KNIGHT OF SANTIAGO FTO Lieutenant:** **31 / 0** — MULTI Rifle, D-Charges, Boarding Pistol, DA CC Weapon; Killer Hacking Device, TinBot Firewall (-3), Lieutenant. **Bronzes Fireteam legal.**

### Cyberghosts — `cyberghosts`

**Unit ID:** 1462 — AVA 1 — LI, Support Troops.

- **Stats:** `10-10 14 11 10 14 1 6 1 2`.
- **Rules:** Stealth.
- **Option 1:** **21 / 0.5** — Combi Rifle, Pitcher, Breaker Pistol, PARA CC Weapon (-3); Hacking Device Plus, Hacker.
- **Option 2:** **18 / 0** — same weapons; Killer Hacking Device, Hacker.

### Betatroopers — `betatroopers`

**Unit ID:** 1456 — AVA 5 — HI, Veteran Troops.

- **Stats:** `15-5 16 13 12 13 3 3 STR2 2`.
- **Rules:** Remote Presence, Courage, Dodge (+3), Mimetism (-3), Climbing Plus.
- **Option 1:** **32 / 0** — MULTI Rifle, Nanopulser (+1B), Pistol, CC Weapon; TinBot Firewall (-3).
- **Option 2:** **35 / 1.5** — Spitfire, Nanopulser (+1B), Pistol, CC Weapon.
- **Option 3:** **36 / 1.5** — option-2 weapons; TinBot Firewall (-3).
- **Option 4:** **25 / 0** — Submachine Gun, Nanopulser (+1B), Pistol, CC Weapon; Killer Hacking Device, Hacker.
- **Option 5 Doctor:** **27 / 0** — Boarding Shotgun, Nanopulser (+1B), Pistol, CC Weapon; Doctor, MediKit.
- **Option 6 Specialist:** **32 / 0** — MULTI Rifle, Nanopulser (+1B), D-Charges, Pistol, CC Weapon; Specialist Operative.

### Ŝarko — `arko`

**Unit ID:** 1610 — AVA 2 — SK, Spec. Trained Troops.

- **Stats:** `10-10 18 11 12 13 1 3 1 2`.
- **Rules:** Surprise Attack (-3), Camouflage, Infiltration, Mimetism (-3), Stealth, Terrain (Total), Climbing Plus.
- **Option 1:** **24 / 0** — Boarding Shotgun, Shock Mine, D-Charges, Pistol, CC Weapon; Killer Hacking Device, Hacker.
- **Option 2:** **22 / 0.5** — Boarding Shotgun, Shock Mine, D-Charges, Pistol, CC Weapon; Minelayer.
- **Option 3:** **22 / 0** — Submachine Gun, Flash Pulse, D-Charges, WildParrot, Pistol, CC Weapon; Forward Observer.
- **Option 4:** **22 / 0** — Boarding Shotgun, Flash Pulse, Shock Mine, D-Charges, Pistol, CC Weapon; Forward Observer.

### Sekudroids — `sekudroids`

**Unit ID:** 1611 — AVA 2 — REM, Spec. Trained Troops.

- **Stats:** `15-5 17 11 10 13 2 6 STR2 2`.
- **Rules/equipment:** Remote Presence, Courage, Mimetism (-3), Climbing Plus; 360º Visor.
- **Option 1:** **19 / 0** — Adhesive Launcher Rifle, Flash Pulse (+1B), Heavy Pistol, PARA CC Weapon (-9).
- **Option 2:** **18 / 0** — Akrylat-Kanone, Flash Pulse (+1B), Heavy Pistol, PARA CC Weapon (-9).

### Ensign Katherine Cho — `ensign-katherine-cho-psi-unit`

**Unit ID:** 1517 — AVA 1 — LI, Character.

- **Stats:** `10-10 13 11 10 14 1 3 1 2`.
- **Rules/equipment:** Immunity (Shock); Holomask.
- **Option 1:** **20 / 0** — MULTI Rifle, Nanopulser, Pistol, CC Weapon; Chain of Command.
- **Option 2 Lieutenant:** **15 / 0** — same weapons; Lieutenant.

### RoadBots Highway Patrol — `roadbots-highway-patrol`

**Unit ID:** 1609 — AVA 2 — REM, Spec. Trained Troops.

#### High Mobility Form

- **Stats:** `20-10 10 11 11 12 2 3 STR1 3`.
- **Rules:** Remote Presence, Courage, Dodge modifiers, Mimetism (-3), No Wound Incapacitation, Terrain (Total), Climbing Plus, Transmutation (Auto).

#### Combat Form

- **Stats:** `10-10 18 12 11 12 2 3 STR1 5`.
- **Rules:** Remote Presence, Courage, Mimetism (-3), No Wound Incapacitation, Transmutation (Auto).

#### Loadouts

- **Option 1:** **26 / 0** — Marksman Rifle, Light Shotgun (+1B), Pistol, PARA CC Weapon (-3).
- **Option 2:** **27 / 1** — Red Fury, Pistol, PARA CC Weapon (-3).
- **Option 3:** **31 / 1** — option-2 weapons; includes SideBot.
- **Option 4 Paramedic:** **22 / 0** — Submachine Gun, Panzerfaust, Drop Bears, Pistol, PARA CC Weapon (-3); MediKit, Paramedic.
- **Option 5 Paramedic:** **20 / 0** — Submachine Gun, Panzerfaust, Heavy Riotstopper, Pistol, PARA CC Weapon (-3); MediKit, Paramedic.
- **Option 6 Paramedic:** **24 / 0** — option-5 weapons; includes SideBot.
- **SideBot included profile:** `20-15 13 10 11 11 0 3 STR1 1`; Peripheral (Synchronized), Courage, Mimetism (-3); Heavy Riotstopper, PARA CC Weapon (-3). Internal source cost 4; not independently selected through this unit.

### Varangian Guard — `varangian-guard`

**Unit ID:** 1461 — AVA 2 — WB, Mercenary Troops.

- **Stats:** `10-10 23 10 14 13 2 0 1 2`.
- **Rules:** Berserk (+3), Impetuous, No Cover, Dogged, Religious Troop.
- **Option 3:** **13 / 0** — Boarding Shotgun, Smoke Grenades, Heavy Pistol, AP CC Weapon.
- **Option 4:** **12 / 0** — Submachine Gun, Chain Rifle, Smoke Grenades, Heavy Pistol, AP CC Weapon.
- **Option 5:** **13 / 0** — Submachine Gun, Chain-colt (+1B), Smoke Grenades, Heavy Pistol, AP CC Weapon.
- **Option 6:** **13 / 0** — Submachine Gun, Chain Rifle, Smoke Grenades, Heavy Pistol, Trench-Hammer, AP CC Weapon.

### Hector, Homeridae's Champion — `hector-homerid-champion`

**Unit ID:** 754 — AVA 1 — HI, Character.

- **Stats:** `10-10 24 13 14 15 5 6 2 2`.
- **Rules/equipment:** Martial Arts L4, Courage, Dodge (+5), Stealth, No Wound Incapacitation, Strategos L1, X-Visor; TinBot Firewall (-3).
- **Option 1:** **61 / 0** — Plasma Rifle, Nanopulser, E/M Grenades, Heavy Pistol, EXP CC Weapon.
- **Option 2:** **60 / 1.5** — Spitfire, Nanopulser, E/M Grenades, Heavy Pistol, EXP CC Weapon.
- **Option 3 Lieutenant:** **65 / 0** — option-1 weapons; Lieutenant (+1 Order), generating two Lieutenant orders in the source.
- **Option 4 Lieutenant:** **64 / 0.5** — option-2 weapons; Lieutenant (+1 Order), generating two Lieutenant orders in the source.

### Andromeda — `andromeda`

**Unit ID:** 788 — AVA 1 — MI, Character.

- **Stats:** `15-5 21 12 12 13 2 3 1 4`.
- **Rules:** Martial Arts L3, Courage, Dodge (+5), Guard, Immunity (Shock), Mimetism (-3), Specialist Operative, Stealth, No Wound Incapacitation, Infiltration (PH=15).
- **Option 5:** **30 / 0** — Submachine Gun, Zapper, Flash Pulse, D-Charges, Breaker Pistol, DA CC Weapon.
- **Option 6:** **33 / 0** — Boarding Shotgun (+1B), Zapper, Flash Pulse, D-Charges, Breaker Pistol, DA CC Weapon.

### Raveneye Officers — `raveneye-officers`

**Unit ID:** 1588 — AVA 2 — LI, Support Troops.

- **Stats:** `10-10 15 11 10 13 1 3 1 2`.
- **Rules/equipment:** Immunity (Shock), Minelayer, Forward Observer; Deactivator.
- **Option 1:** **12 / 0** — Submachine Gun, E/Marat, Flash Pulse, E/M Mine, Pistol, CC Weapon.
- **Option 2:** **12 / 0** — Submachine Gun, E/Marat, Flash Pulse, Cybermine, Pistol, CC Weapon.
- **Option 3 Lieutenant:** **12 / 0** — option-1 weapons; Lieutenant.

### Lawkeepers, Badlands Patrol — `lawkeepers-badlands-patrol`

**Unit ID:** 1530 — AVA 2 — LI, Spec. Trained Troops.

- **Stats:** `20-15 18 12 11 13 2 3 1 4` (mounted).
- **Rules/equipment:** BS Attack (SR-1), Courage, Dodge modifiers, Mimetism (-3), Impetuous, Limited Cover, Specialist Operative; Motorcycle.
- **Option 1:** **18 / 0** — Boarding Shotgun, Chain Rifle, MULTI Pistol, PARA CC Weapon (-3).
- **Option 2:** **25 / 1** — Red Fury, Chain Rifle, MULTI Pistol, PARA CC Weapon (-3).
- **Option 3:** **29 / 1** — option-2 weapons; includes SideBot.
- **Option 4:** **20 / 0** — Combi Rifle, Chain Rifle, MULTI Pistol, PARA CC Weapon (-3).
- **Option 5:** **24 / 0** — option-4 weapons; includes SideBot.
- **Option 6:** **33 / 1** — option-2 weapons; includes two SideBots.
- **Option 7:** **28 / 0** — option-4 weapons; includes two SideBots.
- **SideBot:** same support profile used by RoadBots: `20-15 13 10 11 11 0 3 STR1 1`, Peripheral (Synchronized), Courage, Mimetism (-3), Heavy Riotstopper, PARA CC Weapon (-3).

### Vidocq, Multipurpose Security Brigade — `vidocq`

**Unit ID:** 1773 — AVA 2 — LI, Spec. Trained Troops.

- **Stats:** `10-10 16 13 10 13 1 3 1 2`.
- **Rules:** Mimetism (-3), Stealth, NCO, Terrain (Total).
- **Option 1 — VIDOCQ FTO:** **15 / 0** — Boarding Shotgun, Boarding Pistol, CC Weapon. **Security/Bronzes legal.**
- **Option 2 — VIDOCQ FTO Doctor:** **19 / 0** — option-1 weapons; Doctor, MediKit. **Security/Bronzes legal.**
- **Option 3 — VIDOCQ FTO:** **26 / 1.5** — MULTI Sniper Rifle, Breaker Pistol, CC Weapon; MSV1. **Security/Bronzes legal.**
- **Option 4:** **30 / 1.5** — MULTI Sniper Rifle, Breaker Pistol, CC Weapon; MSV1, Surprise Attack (-3), Camouflage. Not FTO.

### Yudbots — `yudbots`

**Unit ID:** 192 — AVA 2 — REM, Support Troops / Peripheral.

- **Stats:** `15-10 11 8 10 13 0 3 STR1 1`.
- **Rules:** Peripheral (Servant), Courage, Mimetism (-3).
- **Option 1:** **3 / 0** — PARA CC Weapon (-3); support Peripheral with no Order of its own (`minis: 0` in source selection semantics).

### Saladin, Naval Liaison Officer — `saladin-naval-liaison-officer`

**Unit ID:** 1535 — AVA 1 — MI, Character.

- **Stats:** `10-10 17 13 12 16 3 3 1 2`.
- **Rules/equipment:** Courage, Immunity (Shock), No Wound Incapacitation, Counterintelligence, Decoy (2), Minelayer (2); Deployable Repeater.
- **Option 1:** **33 / 0** — Thunderbolt, E/M Carbine, Nanopulser, Pistol, Shock CC Weapon; Chain of Command.
- **Option 2 Lieutenant:** **34 / 0** — same weapons; Lieutenant (+1 Command Token), Strategos L1.

### Raptor Boarding Squad — `raptor-boarding-squad`

**Unit ID:** 1533 — AVA 4 — HI, Veteran Troops.

- **Stats:** `15-5 16 14 12 13 3 3 2 2`.
- **Rules/equipment:** Courage, NCO, Terrain (Zero-G); 360º Visor.
- **Option 2:** **32 / 0** — Heavy Shotgun, Panzerfaust, Boarding Pistol, CC Weapon; includes Devabot.
- **Option 3 FO:** **39 / 0** — MULTI Rifle, E/M Carbine, Flash Pulse, Boarding Pistol, CC Weapon; Forward Observer; includes Devabot.
- **Option 4 Hacker:** **41 / 0** — MULTI Rifle, E/Mitter, Boarding Pistol, CC Weapon; Killer Hacking Device; includes Devabot.
- **Option 5:** **39 / 1.5** — Spitfire, Boarding Pistol, CC Weapon; includes Devabot.
- **Devabot included profile:** `15-10 13 10 10 11 0 3 STR1 2`; Peripheral (Synchronized), Courage, Terrain (Zero-G); 360º Visor; Heavy Flamethrower, Heavy Pistol, PARA CC Weapon (-3). Internal source cost 5.

### Zeta Unit — `zeta-unit`

**Unit ID:** 1458 — AVA 1 — TAG, Mechanized Troops.

- **Stats:** `15-10 17 14 16 13 8 6 STR3 7`.
- **Rules/equipment:** Remote Presence, Dodge (PH=11), Climbing Plus, Courage, GizmoKit (PH=13), BS Attack (SR-1); ECM Guided (-8).
- **Option 2:** **73 / 2** — Hyper-Rapid Magnetic Cannon, Heavy Riotstopper, AP CC Weapon; NCO; includes ZetBot.
- **Option 3 Lieutenant:** **70 / 2** — same weapons; Lieutenant; includes ZetBot.
- **ZetBot included profile:** `15-10 — — 10 12 0 3 STR1 1`; Courage, Dodge (+3), Mimetism (-3), Specialist Operative, Climbing Plus, Peripheral (Ancillary). Internal source cost 3.

### Oko Copperbots — `oko-copperbots`

**Unit ID:** 1464 — AVA 2 — REM, Support Troops.

- **Stats:** `15-10 13 11 10 13 0 3 STR1 3`.
- **Rules/equipment:** Remote Presence, Triangulated Fire, Courage, Forward Observer, Sensor, Climbing Plus; Deactivator, Repeater.
- **Option 1:** **15 / 0** — Combi Rifle, Flash Pulse, PARA CC Weapon (-3).
- **Option 2:** **18 / 0** — same weapons; Tactical Awareness.

### Specialized Support Unit Lambda — `specialized-support-unit-lambda`

**Unit ID:** 1463 — AVA 2 — LI, Support Troops.

- **Stats:** `10-10 14 11 10 14 1 3 1 2`.
- **Option 1 Engineer:** **16 / 0** — Combi Rifle, D-Charges, Pistol, CC Weapon; Deactivator, GizmoKit.
- **Option 2 Engineer:** **17 / 0** — same weapons; Deactivator, GizmoKit, Deployable Cover.
- **Option 3 Engineer:** **19 / 0** — Combi Rifle, D-Charges, Armed Turret (Adhesive Launcher Rifle), Pistol, CC Weapon; Deactivator, GizmoKit.
- **Option 4 Doctor:** **16 / 0** — Combi Rifle, Pistol, CC Weapon; Doctor, MediKit.

### Kyttä Copperbots — `kyttae-copperbots`

**Unit ID:** 1467 — AVA 1 — REM, Support Troops.

- **Stats:** `15-15 13 8 11 13 0 3 STR1 3`.
- **Rules/equipment:** Remote Presence, Courage, Mimetism (-3); Repeater.
- **Option 1:** **7 / 0** — Flash Pulse, PARA CC Weapon (-3).

### PSI-Cops — `psi-cops`

**Unit ID:** 1511 — AVA 2 — LI, Veteran Troops.

- **Stats:** `10-10 15 13 10 13 1 6 1 2`.
- **Rules/equipment:** Immunity (Shock), Mimetism (-3), Specialist Operative, Combat Instinct; X-Visor.
- **Option 3:** **26 / 0** — MULTI Marksman Rifle, Nanopulser (+1B), Heavy Pistol, CC Weapon; Biometric Visor, Discover (+3).
- **Option 4 Hacker:** **24 / 0.5** — Combi Rifle, Nanopulser (+1B), Heavy Pistol, CC Weapon; Hacking Device.
- **Option 5 Hacker:** **23 / 0** — Combi Rifle, Nanopulser (+1B), Heavy Pistol, CC Weapon, Disco Baller; Killer Hacking Device.
- **Option 7:** **27 / 0** — MULTI Marksman Rifle, Nanopulser (+1B), Heavy Pistol, CC Weapon; MSV1.
- **Option 8:** **30 / 0** — option-7 weapons; MSV1, Armed Turret (Thunderbolt).
- **Fireteam:** Wildcard; counts as Security.

### FuzzBots — `fuzzbots`

**Unit ID:** 1469 — AVA 2 — REM, Support Troops.

- **Stats:** `10-10 13 11 10 13 2 3 STR1 4`.
- **Rules/equipment:** Remote Presence, Courage; Baggage.
- **Option 1:** **8 / 0** — PARA CC Weapon (-3); Deactivator, Repeater.
- **Option 2:** **14 / 0.5** — PARA CC Weapon (-3); EVO Hacking Device, Hacker.
- **Option 3:** **17 / 0** — Combi Rifle, PARA CC Weapon (-3); Repeater, Total Reaction.

### Epsilon Unit — `epsilon-unit`

**Unit ID:** 1454 — AVA 2 — MI, Elite Troops.

- **Stats:** `10-10 16 13 11 13 3 3 1 2`.
- **Rules/equipment:** Mimetism (-3), Immunity (Shock), Climbing Plus; MSV2.
- **Option 1:** **34 / 1.5** — HMG, Nanopulser, Pistol, CC Weapon.
- **Option 2:** **32 / 1.5** — MULTI Sniper Rifle, Nanopulser, Pistol, CC Weapon.
- **Option 3:** **29 / 0.5** — Shock Marksman Rifle, Nanopulser, Pistol, CC Weapon.

### Warcors — `warcors-war-correspondents`

**Unit ID:** 50 — AVA 1 — LI, Mercenary Troops; Irregular.

- **Stats:** `10-10 11 9 11 13 0 0 1 2`.
- **Rules:** Journalist.
- **Option 1:** **3 / 0** — Flash Pulse, Stun Pistol, PARA CC Weapon (-3); 360º Visor.
- **Option 2:** **3 / 0** — same weapons; Sixth Sense.

### Parvati, Circle League star — `parvati-circle-league-star`

**Unit ID:** 1534 — AVA 1 — LI, Character.

- **Stats:** `15-5 15 12 10 15 2 6 STR2 2`.
- **Rules/equipment:** Remote Presence, Courage, Doctor (2W), Engineer (+3), Dodge (+3), Super-Jump; Deactivator, GizmoKit, MediKit.
- **Option 1:** **36 / 0** — Submachine Gun (+1B), Flash Pulse, Pistol, CC Weapon. **Wildcard.**

### Nyoka Assault Troops — `nyoka-assault-troops`

**Unit ID:** 1531 — AVA 5 — LI, Spec. Trained Troops.

- **Stats:** `10-10 19 12 11 13 1 3 1 2`.
- **Rules:** BS Attack (SR-1), Courage, Immunity (Shock), Terrain (Zero-G), Climbing Plus.
- **Option 3 — NYOKA FTO:** **18 / 1** — Heavy Rocket Launcher, Chain-colt, Heavy Pistol (+1B), Shock CC Weapon. **Nyoka Fireteam legal.**
- **Option 4 — NYOKA FTO:** **22 / 0** — MULTI Rifle, Chain-colt, Pistol, Shock CC Weapon; Forward Observer. **Nyoka Fireteam legal.**
- **Option 5:** **27 / 0** — MULTI Rifle, Chain-colt, Pistol, Shock CC Weapon; Forward Observer, Parachutist. Not FTO.
- **Option 6:** **29 / 1** — Red Fury, Chain-colt, Pistol, Shock CC Weapon; Parachutist. Not FTO.

### Crushers, Special Naval Demolition Team — `crushers`

**Unit ID:** 1512 — AVA 3 — MI, Veteran Troops.

- **Stats:** `10-10 17 13 12 13 2 3 1 2`.
- **Rules:** Courage, Immunity (Shock), Mimetism (-3), Forward Observer, No Wound Incapacitation, Terrain (Zero-G).
- **Option 1:** **31 / 0** — MULTI Rifle, Flash Pulse, D-Charges, Boarding Pistol, E/M CC Weapon; Forward Deployment (+20).
- **Option 2:** **25 / 0** — Submachine Gun, Flash Pulse, D-Charges, Boarding Pistol, E/M CC Weapon; Forward Deployment (+20).
- **Option 3:** **31 / 0.5** — Submachine Gun, Light Rocket Launcher, Flash Pulse, D-Charges, Boarding Pistol, E/M CC Weapon; Forward Deployment (+20).
- **Option 4:** **27 / 0** — Boarding Shotgun, Panzerfaust, D-Charges, Boarding Pistol, E/M CC Weapon; Combat Jump, Super-Jump (Jet Propulsion), Parachutist.

### Casanova, NOC Operative — `casanova-noc-operative`

**Unit ID:** 1483 — AVA 1 — LI, Character.

- **Stats:** `10-10 22 13 11 13 1 6 1 2`.
- **Rules:** Martial Arts L2, Courage, Dodge (+3), Immunity (Shock), Mimetism (-6), Specialist Operative, Stealth, No Wound Incapacitation, Decoy (1).
- **Option 1:** **31 / 0** — Submachine Gun, Nanopulser (+1B), E/M Mine, Silenced Pistol, Monofilament CC Weapon; Forward Deployment (+20), Minelayer.
- **Option 2:** **31 / 0** — as option 1 but Shock Mine instead of E/M Mine; Forward Deployment (+20), Minelayer.
- **Option 3:** **32 / 0** — Submachine Gun, Nanopulser (+1B), E/M Mine, Silenced Pistol, Monofilament CC Weapon; Infiltration (PH=15).

### Ment Agents, PSID — `ment-agents`

**Unit ID:** 1768 — AVA 1 — LI, Spec. Trained Troops.

- **Stats:** `10-10 17 12 10 13 1 3 1 2`.
- **Rules/equipment:** Chain of Command, Stealth, Number 2; Biometric Visor.
- **Option 1 — MENT:** **15 / 0** — Heavy Riotstopper (+2B), Assault Pistol, PARA CC Weapon (-3).
- **Option 2 — MENT FTO:** **15 / 0** — Light Shotgun, Pistol, PARA CC Weapon (-3).
- **Option 3 — MENT FTO:** **14 / 0** — Heavy Riotstopper (+1B), Assault Pistol, PARA CC Weapon (-3).
- **Option 4 — MENT FTO Hacker:** **20 / 0.5** — Light Shotgun, Pistol, PARA CC Weapon (-3); Hacking Device, Hacker.
- **Fireteam note:** the canonical Security and Bronzes chart rows name `MENT`, not `MENT FTO`; therefore **all four options** are legal there.

### Millicent Copperbots — `millicent-copperbots`

**Unit ID:** 1466 — AVA 1 — REM, Support Troops.

- **Stats:** `15-10 13 12 10 13 0 3 STR1 3`.
- **Rules:** Remote Presence, BS Attack (Guided), Courage.
- **Option 1:** **16 / 1.5** — Missile Launcher, PARA CC Weapon (-3).

### Bronzes, Deep Space Peacemaker Corps — `bronzes`

**Unit ID:** 1532 — AVA 3 — HI, Veteran Troops.

- **Stats:** `15-5 20 13 13 13 4 6 2 2`.
- **Rules/equipment:** Martial Arts L1, Courage, Terrain (Zero-G), Climbing Plus, Dodge (+2.5), Immunity (Enhanced); 360º Visor.
- **Option 3:** **47 / 1** — Red Fury, Pistol, E/M CC Weapon, PARA CC Weapon (-6).
- **Option 4 Paramedic:** **41 / 0** — Heavy Shotgun, Akrylat-Kanone, Pistol, E/M CC Weapon, PARA CC Weapon (-6); MediKit, Paramedic.
- **Option 5 Specialist:** **43 / 0** — MULTI Rifle, Heavy Riotstopper, Pistol, E/M CC Weapon, PARA CC Weapon (-6); Specialist Operative.
- **Option 6:** **48 / 1.5** — HMG, Pistol, E/M CC Weapon, PARA CC Weapon (-6).

### Jackboots — `jackboots`

**Unit ID:** 1767 — AVA 2 — MI, Veteran Troops.

- **Stats:** `10-10 15 13 11 13 3 3 1 2`.
- **Rules:** BS Attack (SR-1), Warhorse, Immunity (Enhanced), Combat Instinct, Religious Troop.
- **Option 1:** **23 / 1.5** — Heavy Rocket Launcher, Light Shotgun, Pistol, CC Weapon.
- **Option 2 Engineer:** **25 / 0** — AP Submachine Gun, E/Mitter, D-Charges, Pistol, CC Weapon; Engineer, GizmoKit.
- **Option 3 Engineer:** **28 / 0** — option-2 weapons plus Armed Turret (Thunderbolt AP); Engineer, GizmoKit.
- **Option 4 FO:** **26 / 0** — Thunderbolt (+1B), E/M Carbine, Flash Pulse, Pistol, CC Weapon; Forward Observer.
- **Option 5 Paramedic:** **21 / 0** — AP Submachine Gun, Light Riotstopper, Panzerfaust, Pistol, CC Weapon; MediKit, Paramedic.
- **Option 6 NCO:** **29 / 1** — HMG, Light Riotstopper, Pistol, CC Weapon; NCO.

### Nightshades — `nightshades`

**Unit ID:** 1774 — AVA 1 — SK, Elite Troops.

- **Stats:** `10-10 22 12 12 13 2 0 1 2`.
- **Rules/equipment:** Martial Arts L3, Camouflage, Courage, Forward Deployment (+20), Mimetism (-6), Stealth, Super-Jump, Terrain (Total), Surprise Attack (-3), Hidden Deployment; Bangbomb (+4).
- **Option 1:** **32 / 0** — Boarding Shotgun, Shock Mine, Pistol, E/M CC Weapon, PARA CC Weapon (-6).
- **Option 2:** **31 / 0** — Submachine Gun, Drop Bears, D-Charges, Pistol, E/M CC Weapon, PARA CC Weapon (-6).
- **Option 3 Hacker:** **34 / 0** — option-2 weapons; Killer Hacking Device, Hacker.
- **Option 4:** **32 / 0.5** — Submachine Gun, D-Charges, Shock Mine, Pistol, E/M CC Weapon, PARA CC Weapon (-6); Minelayer.

### Kappa Unit — `kappa-unit`

**Unit ID:** 1447 — AVA 5 — LI, Line Troops.

- **Stats:** `10-10 14 12 10 13 1 0 1 2`.
- **Rules:** Immunity (Shock).
- **Option 1:** **12 / 0** — Combi Rifle, Pistol, CC Weapon.
- **Option 2:** **20 / 1** — HMG, Pistol, CC Weapon.
- **Option 3:** **18 / 1** — MULTI Sniper Rifle, Pistol, CC Weapon.
- **Option 4:** **17 / 1.5** — Missile Launcher, Pistol, CC Weapon.
- **Option 5 Hacker:** **13 / 0.5** — Submachine Gun, Pistol, CC Weapon; Hacking Device.
- **Option 6 FO:** **14 / 0** — Combi Rifle, Flash Pulse, Pistol, CC Weapon; Deployable Repeater, Forward Observer.
- **Option 7 Paramedic:** **14 / 0** — Combi Rifle, Pistol, CC Weapon; MediKit, Paramedic.
- **Option 8 Lieutenant:** **12 / 1** — Combi Rifle, Pistol, CC Weapon; Lieutenant.
- **Option 10 Specialist:** **14 / 0** — Combi Rifle, Pistol, CC Weapon; Commlink (+1), Specialist Operative.

### Bìxié, the Jade Champion — `bixie`

**Unit ID:** 1599 — AVA 1 — HI, Character.

- **Stats:** `15-5 22 13 12 13 3 6 2 2`.
- **Rules/equipment:** Martial Arts L3, Courage, Dodge modifiers, Forward Observer, Stealth, NCO, Super-Jump, Climbing Plus; MSV1.
- **Option 1:** **41 / 0** — MULTI Rifle, Zapper, Flash Pulse, Pistol, E/M CC Weapon.

### Ioann Bann, Varangian Dog-Warrior — `ioann-bann-varangian-dog-warrior`

**Unit ID:** 1940 — AVA 1 — WB, Character; Irregular, Impetuous.

#### Dogface Form

- **Stats:** `15-10 22 11 14 13 2 3 3 2`.

#### Dog-Warrior Form

- **Stats:** `15-10 23 11 16 13 4 6 3 6`.

- **Rules across source states:** Martial Arts L3, BS Attack (-3), Berserk, Dodge (+5), Immunity (ARM), No Cover, Super-Jump, Transmutation, Religious Troop, Impetuous.
- **Option 1:** **32 / 0** — Chain Rifle (+1B), Viral Tactical Bow (+1SD), Smoke Grenades, AP Heavy Pistol (+1B), AP + T2 CC Weapon; Irregular.

## Optional-mode profile hooks

### Ŝtormo Spec-Ops — `tormo-spec-ops`

**Unit ID:** 1923 — Infinity Spec-Ops; not part of the ordinary 42-unit matched-play roster.

- **Initial profile:** `10-10 14 13 11 13 2 3 1 2`.
- **Enhanced profile:** `15-5 16 13 12 13 3 6 2 2`.
- **Option 1:** **27 / 1** — HMG, Light Riotstopper, D-Charges, Pistol, PARA CC Weapon (-6).
- **Option 2:** **25 / 1.5** — MULTI Sniper Rifle, Light Riotstopper, D-Charges, Pistol, PARA CC Weapon (-6).
- **Option 3 Specialist:** **22 / 0** — MULTI Rifle, Light Riotstopper, D-Charges, Pistol, PARA CC Weapon (-6); GizmoKit, Specialist Operative.
- **Option 4 Hacker:** **21 / 0.5** — AP Submachine Gun, Light Riotstopper, Akrylat-Kanone, D-Charges, Pistol, PARA CC Weapon (-6); Hacking Device.
- **Option 5 FO:** **22 / 0** — MULTI Rifle, Light Riotstopper, Flash Pulse, D-Charges, Pistol, PARA CC Weapon (-6); Forward Observer.
- **Option 6 Paramedic:** **18 / 0** — AP Submachine Gun, Light Riotstopper, Flash Pulse, D-Charges, Pistol, PARA CC Weapon (-6); MediKit, Paramedic.
- **Fireteam hook:** up to one in Security Fireteams when the Spec-Ops mode is in use.
- The source also carries internal Kolego SpecBot options for Spec-Ops construction; they are not normal roster entries.

### O-12 Team-Ops — `o12-team-ops`

**Unit ID:** 1937 — Infinity Team-Ops optional-mode record. It contains Ŝtormo-1, Ŝtormo Heavy, and Kolego SpecBot construction profiles and is not part of the ordinary Starmada roster or canonical normal Fireteam chart.

## Fireteams

This section is authoritative for Starmada Fireteam legality. The reverse index below is derivative.

### FT-01 — Security Fireteams

**Types:** Haris, Core  
**Required-source set:** at least one legal member from the `KAPPA (Security)` / `BLUECOAT (Security)` required rows.

| Member | Unit ID | Required set | Min | Max | Counts as | FTO restriction | Allowed option IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Kappa Unit | 1447 | yes | 0 | 5 | Security | — | all | required-choice source |
| Bluecoats | 1529 | yes | 0 | 4 | Security | — | all | required-choice alternative |
| Raveneye Officers | 1588 | no | 0 | 2 | Security | — | all | — |
| Sekudroids | 1611 | no | 0 | 1 | Security | — | all | — |
| Bronzes | 1532 | no | 0 | 1 | — | — | all | — |
| Ensign Katherine Cho | 1517 | no | 0 | 1 | Security | — | all | — |
| Jackboots | 1767 | no | 0 | 2 | — | — | all | — |
| Vidocq | 1773 | no | 0 | 1 | — | **FTO** | `1,2,3` | option 4 excluded |
| Ment Agents | 1768 | no | 0 | 1 | — | **none** | `1,2,3,4` | chart says `MENT`, so non-FTO option 1 is legal |
| Ŝtormo Spec-Ops | 1923 | no | 0 | 1 | — | optional mode | Spec-Ops options | Spec-Ops only |

### FT-02 — Nyokas Fireteams

**Types:** Duo, Haris, Core

| Member | Unit ID | Required | Min | Max | Counts as | FTO restriction | Allowed option IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Nyoka Assault Troops | 1531 | no | 1 | 5 | — | **FTO** | `3,4` | at least 1 Nyoka FTO |
| Bronzes | 1532 | no | 0 | 1 | Nyoka | — | all | — |
| Hector | 754 | no | 0 | 1 | — | — | all | — |
| Epsilon Unit | 1454 | no | 0 | 1 | — | — | all | — |

### FT-03 — Betatroopers Fireteams

**Types:** Duo, Haris, Core

| Member | Unit ID | Required | Min | Max | Counts as | FTO restriction | Allowed option IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Betatroopers | 1456 | no | 1 | 5 | — | — | all | at least 1 Betatrooper |
| Epsilon Unit | 1454 | no | 0 | 1 | Betatrooper | — | all | — |
| Sekudroids | 1611 | no | 0 | 1 | Betatrooper | — | all | — |
| Hector | 754 | no | 0 | 1 | — | — | all | — |
| Bìxié | 1599 | no | 0 | 1 | — | — | all | — |

### FT-04 — Bronzes Fireteams

**Types:** Duo, Haris

| Member | Unit ID | Required | Min | Max | Counts as | FTO restriction | Allowed option IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Bronzes | 1532 | no | 1 | 2 | — | — | all | at least 1 Bronze |
| Knights of Santiago | 27 | no | 0 | 1 | — | **FTO** | `1,2,5,6` | Combat Jump options 3/4 excluded by source note |
| Sekudroids | 1611 | no | 0 | 1 | — | — | all | — |
| Vidocq | 1773 | no | 0 | 1 | — | **FTO** | `1,2,3` | option 4 excluded |
| Ment Agents | 1768 | no | 0 | 1 | — | **none** | `1,2,3,4` | chart says `MENT` |

### FT-05 — Varangian Guards Fireteams

**Type:** Duo

| Member | Unit ID | Required | Min | Max | Counts as | FTO restriction | Allowed option IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Varangian Guard | 1461 | no | 1 | 2 | — | — | all | at least 1 Varangian |
| Ioann Bann | 1940 | no | 0 | 1 | Varangian | — | all | — |

### FT-06 — Road Fireteams

**Type:** Duo  
**Required-source set:** at least one legal member from the `LAWKEEPER` / `ROADBOT (Lawkeepers)` required rows.

| Member | Unit ID | Required set | Min | Max | Counts as | FTO restriction | Allowed option IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Lawkeepers | 1530 | yes | 0 | 2 | — | — | all | required-choice source |
| RoadBots | 1609 | yes | 0 | 2 | Lawkeepers | — | all | required-choice alternative |
| Oko Copperbots | 1464 | no | 0 | 1 | Lawkeepers | — | all | — |

### Wildcards

| Unit | Unit ID | Counts as | FTO/profile restriction | Max | Notes |
|---|---:|---|---|---:|---|
| PSI-Cops | 1511 | Security | none; all options | 2 | Wildcard |
| Shona Carano | 1505 | — | all | 1 | Wildcard |
| Parvati | 1534 | — | all | 1 | Wildcard |
| Tian Gǒu | 1536 | — | **FTO options `1,3,4,6` only** | 1 | Wildcard |

## Unit → Fireteam access index

This index is generated from the canonical chart above. If it ever conflicts with `## Fireteams`, the canonical chart wins.

| Unit | Effective Fireteam access |
|---|---|
| Peeler Copperbots | — |
| Tinkers | — |
| Tian Gǒu | Wildcard; options **1,3,4,6 only** |
| Shona Carano | Wildcard; all options |
| Bluecoats | Security Haris/Core; all options; counts as Security |
| Firebat Attack Wing | — |
| Knights of Santiago | Bronzes Duo/Haris; **options 1,2,5,6 only** |
| Cyberghosts | — |
| Betatroopers | Betatroopers Duo/Haris/Core; all options |
| Ŝarko | — |
| Sekudroids | Security Haris/Core; Betatroopers Duo/Haris/Core; Bronzes Duo/Haris; all options |
| Ensign Katherine Cho | Security Haris/Core; all options; counts as Security |
| RoadBots | Road Duo; all options; counts as Lawkeepers |
| Varangian Guard | Varangian Guards Duo; all options |
| Hector | Nyokas Duo/Haris/Core; Betatroopers Duo/Haris/Core; all options |
| Andromeda | — |
| Raveneye Officers | Security Haris/Core; all options; counts as Security |
| Lawkeepers | Road Duo; all options |
| Vidocq | Security Haris/Core; Bronzes Duo/Haris; **options 1,2,3 only** |
| Yudbots | — |
| Saladin | — |
| Raptor Boarding Squad | — |
| Zeta Unit | — |
| Oko Copperbots | Road Duo; all options; counts as Lawkeepers |
| Lambda | — |
| Kyttä Copperbots | — |
| PSI-Cops | Wildcard; all options; counts as Security |
| FuzzBots | — |
| Epsilon Unit | Nyokas Duo/Haris/Core; Betatroopers Duo/Haris/Core; all options |
| Warcors | — |
| Parvati | Wildcard; all options |
| Nyoka Assault Troops | Nyokas Duo/Haris/Core; **options 3,4 only** |
| Crushers | — |
| Casanova | — |
| Ment Agents | Security Haris/Core; Bronzes Duo/Haris; **all options 1–4** |
| Millicent Copperbots | — |
| Bronzes | Security Haris/Core; Nyokas Duo/Haris/Core (counts as Nyoka); Bronzes Duo/Haris; all options |
| Jackboots | Security Haris/Core; all options |
| Nightshades | — |
| Kappa Unit | Security Haris/Core; all options; counts as Security |
| Bìxié | Betatroopers Duo/Haris/Core; all options |
| Ioann Bann | Varangian Guards Duo; all options; counts as Varangian |
| Ŝtormo Spec-Ops | Security Haris/Core in Spec-Ops mode only |
| O-12 Team-Ops | Optional mode only; no ordinary Fireteam access row |

## Dependencies, alternate states, and roster boundaries

- **RoadBots** options `3` and `6` include one SideBot; **Lawkeepers** options `3` and `5` include one SideBot and options `6` and `7` include two. SideBots are internal Synchronized Peripherals, not independent logical roster entries.
- **Raptor Boarding Squad** options include a Devabot Synchronized Peripheral.
- **Zeta Unit** options include a ZetBot Ancillary Remote Unit.
- **Yudbots** are Servant Peripherals and do not generate an Order of their own.
- **RoadBot** High Mobility / Combat forms and **Ioann Bann** Dogface / Dog-Warrior forms are alternate states of one logical trooper, not additional roster entries.
- The Army source contains relation records involving Starmada units and counterpart records outside this normal roster. Those do not merge Reinforcement-only or alternate army records into the 42-unit standard roster.
- Generic Soldier-of-Fortune catalog records with `factions: []` are not Starmada roster entries merely because they appear in the aggregate source payload.

## Community tactics — Starmada N5.3 (transcripts reviewed 2026-10-23)

**Interpretation, not Army data.** Use the profile/Fireteam tables above for N5.3 costs, AVA, FTO, Orders and eligibility. The discussion sources include N5-launch (2024), 2025, 2026 and historical N4 material; do **not** copy historical profiles, generic O-12 units or former Fireteam combinations into current Starmada. Relative grades quoted below are **speakers' subjective assessments**, not faction-wide facts.

### Starmada in five decisions (the "why")

1. **Start with the link's job, then buy its members.** Starmada trades Vanilla O-12's Gamma/Omega/Wrecker/Moonraker options for a **Security Core**, Betatroopers, Bronzes, Nyokas, Road Duos and distinctive command/CC tools. Its good but relatively expensive 20–40+ point models can leave too few Orders if you buy every toolbox. Decide first whether the list's main plan is **Bronze/Security fighting**, **Betatrooper mobility**, **Hector/Nyoka combined arms**, or a **Zeta-centric TAG**.
2. **Security is the adjustable economy/defense Core.** A legal Security Haris/Core needs **at least one Kappa or Bluecoat**. Cheap Kappas, Bluecoats' Sixth Sense/Discover/glue, Raveneye mines and optional PSI-Cop/Vidocq/Jackboot/Bronze/Parvati pieces create defensive depth without committing five expensive HI. Retain the right Kappa/Bluecoat source member after casualties; do not infer access from Wildcard/FTO alone.
3. **Put *mobility* where it saves Orders.** Betatroopers and Sekudroids share **Climbing Plus + Remote Presence**; Betatrooper+Sekudroid or Betatrooper+Epsilon teams get a dangerous rifle/specialist to the right angle while the second model contributes adhesion/ARO/repairable structure. Separately, the **RoadBot/Oko Duo** makes a 20–24pt fast Paramedic plus a 15/18pt Sensor/FO/Repeater a small objective package. Route around towers/walls, not into an opponent's prepared ARO lane.
4. **Nonlethal control creates the attack.** Bluecoat Heavy Riotstopper/adhesive, Sekudroid adhesive, a Bronze's E/M/para CC, Raveneye E/M mines, Cyberghost's Pitcher/HD+ White Noise, Shona/Varangian smoke, and Šarko mines/WildParrot can **force Dodges, Resets and movement** before a premium weapon commits. Stacking several complementary threats is stronger than repeating a single gun at every defensive piece.
5. **Protect mission capacity after the fighting piece falls.** Starmada has useful specialist options but limited very cheap Regular bodies and lacks Vanilla's Moonraker mine layer. Budget a backup scoring lane (Oko, RoadBot, Šarko, cheap Kappa/PSI-Cop) and defenses rather than relying on one 60–73pt hero/TAG. The 2026 comparative review's chief objection is exactly this *opportunity cost*.

### Practical Fireteam packages (verify exact source restrictions above)

| Package | Why it earns Orders | Cost / tactical trap |
|---|---|---|
| **Security Core** — Kappa or Bluecoat anchor, Raveneye, PSI-Cop, Vidocq, optional Bronze/Jackboot/Parvati | Mission-flexible home defense; Bluecoat discovers and arrests up close, Raveneye's mines delay DZ attacks, PSI-Cop provides a specialist/MSV/hacker; one powerful guest can fire without buying a five-HI Core. | A Security Core **must** include a Kappa/Bluecoat source, not just Wildcards. Be clear about which named troopers count as Security and the FTO restriction on Vidocq. |
| **Bronze + Ment / Vidocq / Santiago / Sekudroid Haris** | Bronze HMG/Red Fury anchors a durable push, 360° helps cover flanks, Climbing Plus changes routes, Enhanced Immunity and E/M/PARA CC punish approaches; Ment/Vidocq can add recovery or complementary gun; Sekudroid provides a cheap glue/Flash-Pulse body. | 41–48pt Bronzes are a major investment with hacking/template exposure. No Core in the *Bronzes family*; Santiago **Combat Jump** options cannot join it. |
| **Bronze + Parvati in a legal Fireteam** | Parvati is a **Wildcard**, Doctor (2W) and Engineer (+3); she can restore expensive Bronzes/remote troops and score, turning an otherwise unaffordable loss into recoverable pressure. | Parvati costs 36 and must reach the casualty safely; do not force her into an exposed attack path or assume revival is guaranteed. |
| **Betatrooper Spitfire / KHD / Doctor + Sekudroid or Epsilon** | Betatroopers bring Mimetism (-3), 2 STR/Remote Presence, Climbing Plus and specialist options; Sekudroid adds **glue, Flash Pulse (+1B), 360° and two STR** for 18–19pt; Epsilon is a linked MSV2 gun for smoke/Mimetism problems. | Every additional Beta increases investment; a compact Duo/Haris often does the movement job cheaper than a five-body HI Core. A Sekudroid is **max one** in this family. |
| **Nyoka FTO HRL/FO + Epsilon/Hector/Bronze (legal FT-II)** | The 18pt FTO Heavy Rocket Launcher is an economical template/ARO source; an Epsilon solves visor fights and a Hector Lt can supply command plus a threatening gun/CC counterattack. A single **Bronze counts as Nyoka** here. | **Only Nyoka FTO options 3/4** link; parachutist Nyoka 5/6 do not. Hector is 60–65pt before partners: do not build a full premium Core just for theoretical bonuses. |
| **Road Duo: RoadBot / Lawkeeper + Oko or second RoadBot** | A RoadBot 20/22pt Paramedic + **Oko 18pt Tactical Awareness** advances two objective pieces efficiently; Oko contributes Sensor, FO and Repeater; an alternative Lawkeeper adds bike speed and SideBot tricks. | Need **at least one Lawkeeper or RoadBot**; Oko cannot form Road Duo alone. Split up when opposing AROs/area threats make shared movement unsafe. |
| **Varangian Duo; with Shona as legal Wildcard option** | Low-point smoke and template/CC pressure can screen the advance or attack an isolated defender; Shona's cheap, dangerous AP+EXP close combat adds a real finishing threat. | Impetuous exposure, Natural Born Warrior and gun range still matter. Wildcard legality is distinct from the base chart's native Varangian/Ioann entries. |

### Independent units: strengths with limits

| Pick | Use because… | Avoid / reconsider when… |
|---|---|---|
| **Šarko (22–24)** | Infiltration + Camo + Climbing Plus give Starmada its own midfield marker-state scorer; KHD, FO/WildParrot or Minelayer can set a short-range trap and pressure TAGs/hackers in a repeater/adhesive fork. | BS11, one Wound, short guns and ~22pt are a steep tax for what Robert Shepherd calls a *costly Zero-like* specialist (June 2026). Budget as a button/trap first, not a premium attacker. |
| **Nightshade (31–34)** | Hidden Deployment, Mimetism (-6), FD, KHD or mines and strong CC can delay high-value specialists or ambush isolated enemies. | Expensive one-Wound investment; hold to a credible ambush/mission route rather than expose it just to threaten. |
| **Shona / Bìxié / Varangians** | Shona 22pt Wildcard (AP+EXP CC, Super-Jump) is an efficient short-range trade; Bìxié offers a higher-cost durable specialist/attack variant in Betatroopers; 12–13pt Varangians offer Regular smoke and cheap countercharge. | Different matchups: Shona fears Natural Born Warrior, templates and poor approach; Bìxié adds expense/hacking exposure; Varangian risks Impetuous movement. |
| **Hector versus Saladin versus Raveneye Lt** | **Hector Lt** gives two Lt Orders and a dangerous plasma/spitfire/CC presence plus Strategos; **Saladin Lt** brings WIP16, Strategos, Counterintelligence, +1 Command Token, Decoy (2)/Minelayer (2) for protected reserve play; **Raveneye Lt 12pt** preserves army points and adds DZ mines. | Hector's ~64–65pt competes with your main attacker; Saladin ~34pt pays heavily for command not guns; Raveneye is cheaper but must be disguised/protected. Ment/Cho CoC can insure exposed Lt choices. |
| **Cyberghost HD+ with coverage** | 21pt WIP14/BTS6 Pitcher + White Noise helps Bronze/Zeta/Epsilon teammates deal with enemy visors and builds a useful hacking threat from Kyttä/Oko/Fuzz/Sekudroid-adjacent positions (Sekudroid itself is **not** a Repeater). | AVA **1** Starmada: choosing the HD+ excludes its 18pt KHD alternative. Keep separate KHD or other defensive answers as needed; avoid White Noise impairing your own MSV user. |
| **Raptor KHD + Devabot** | NCO, BS14, 2W, 360°, Cybermask option and synchronized heavy flamethrower make an effective enemy-backfield fork: protect against hacking while the Devabot forces template decisions. | 41pt KHD or 32–39pt other profiles is not a disposable drop trooper; stay alert to templates and enemy KHD/networks. |
| **Casanova / Andromeda / Crushers / Santiago AD** | Can create unexpected midfield or backline threats; Santiago Combat Jump KHD provides a different reach from a linked FTO Santiago. | Speakers disagree on reliability and price, particularly Casanova and Andromeda; a failed infiltration roll or unfavorable arrival can burn a lot of points. **Santiago options 3/4 cannot link** while using their Combat Jump profiles. |

### TAG, Vehicle and *all* REMs in Starmada

**Roster boundary:** Starmada has the **Zeta TAG** and **Firebat Vehicle**, but **not** the Wrecker TAG, StormBot, Moonraker or Gamma from other O-12 lists. Shared O-12 commentaries on the Zeta/Firebat/Oko/RoadBot/Peeler still apply tactically; parent-faction/other-sectorial AVA and Fireteams **do not**.

| Platform (current Starmada profile) | Why / operating role | Tradeoff and support |
|---|---|---|
| **Zeta TAG** — **70 Lt / 73 NCO, 2 SWC** | HMC + BS14, ARM8/STR3, Climbing Plus, ECM Guided (-8), Remote Presence and an included **ZetBot Ancillary specialist** make a powerful long-range and scoring anchor. Take only with a full target/escape/recovery plan. | **No Tactical Awareness**: the 2025 Tactical Awareness panel argues it lacks the extra Orders to justify its cost *in Starmada*, unlike the very enthusiastic **S-tier parent O-12** rating from Loss of Lieutenant's TAG panel. Lt version saves points but needs CoC/anti-hack protection. |
| **Firebat VH (not TAG/REM)** — **35–36, 0 SWC** | Aerial/20-5 movement, Super-Jump, Mimetism (-6), NCO, Tech-Recovery and E/M/rocket/adhesive weapons allow unusual flanking angles and a Lt-Order recipient; 0 SWC helps SWC-constrained builds. | **No Cover, STR2, ARM4**. June 2026 Robert Shepherd/Jordan tier review calls it arguably the weakest flyer for price: at 35–36 it must do decisive work, unlike a cheaper flyer that can trade. Use with a planned route and backup, not as default. |
| **RoadBot (REM)** — **20–31; Paramedic 20/22/24** | High-Mobility 20-10 + Climbing Plus, Combat-form NWI, Drop Bears / Heavy Riotstopper / Panzerfaust, optional **SideBot** and Road Duo eligibility make it a swift button-pusher/flanker. | WIP12/BS11–12 and fragile on an exposed lane; its form changes alter silhouette/movement/abilities. Cheap 20/22pt Paramedic often provides more mission value than a costly Red Fury attacker when the list already has Bronze/Zeta. |
| **Oko Copperbot (REM)** — **15, or 18 with Tactical Awareness** | Mission all-rounder: **FO + Sensor + Repeater + Climbing Plus** and, for +3pts, an Order to reposition/scan/objective-run without consuming the main pool. Road Duo can escort it to a button. | BS11/ARM0, cannot force its way through a live ARO. Take the TA version when it will actually act; otherwise 15pt is a legitimate saving. |
| **Sekudroid (REM)** — **18–19** | **2 STR, Mimetism (-3), 360°, Climbing Plus, adhesive/Akrylat and Flash Pulse (+1B)**; uniquely **legal team glue/body** in Security, Betatroopers and Bronzes. Its relative low price makes a powerful HI team less all-in. | AVA2 but only **one per respective Fireteam**. Still BS11, not a primary shooter, and its sticky ARO is weaker once opponents choose favorable range/angles. Pair with Betatrooper repairs or a mission-specific threat. |
| **Peeler Copperbot (REM)** — **19 Thunderbolt (+1B), 0 SWC** or **24 HMG, 1 SWC** | Total Reaction + 360° + Climbing Plus: good low-maintenance backfield ARO. Thunderbolt variant is easy to fit when the SWC budget is tight. | ARM0/BS11 and one STR; a capable active-turn attacker will eventually dismantle an overexposed static turret. Make it part of layered defense with Bluecoat/Raveneye, not the only speed bump. |
| **Kyttä Copperbot (REM)** — **7, 0 SWC** | Cheap Regular Repeater/Flash Pulse (Mimetism -3, 15-15 MOV) to extend Cyberghost's network and consume enemy Orders. | BS8; it's a network/ARO nuisance, not an active attack plan. **AVA1** Starmada. |
| **FuzzBot (REM)** — **8 Baggage/Repeater**, **14 EVO**, or **17 TR combi** | The 8pt Baggage bot supplies a cheap Regular Order, network area and Pitcher reload; EVO supports a chosen hacking/Remote-Presence plan; TR version defends close approaches. | The **17pt Total Reaction combi** is debated versus the 19pt Thunderbolt Peeler: trading 2pts for much worse range is rarely worthwhile *unless* the Repeater/Baggage benefits are central. EVO consumes 0.5 SWC and needs purpose. |
| **Millicent Copperbot (REM)** — **16, 1.5 SWC** | Guided Missile Launcher creates a second attack vector if **Cyberghost/other hackers establish Targeted** and the order/network geometry is sound; forces TAGs to respect Spotlight. | Without a reliable Targeted pipeline it is a 16pt/1.5SWC passive piece; don't assume guided fire ignores mission timing or reactive counterplay. |
| **Yudbot servant REM** — **3** | Extend Lambda/Parvati's Doctor/Engineer access so expensive Bronze/Beta/Zeta/ZetBot casualties can be recovered from safer positions. | Servant Peripheral: no independent Order, cannot repair without its linked specialist and a legal route; don't confuse with Zeta's separate **Ancillary ZetBot**. |

**Practical platform shells:**
- **Zeta shell:** Zeta Lt/NCO + Ment/Cho CoC when appropriate + Lambda/Parvati/Yudbot engineering + cheap Road/Oko scorer + denial pieces. Challenge: too many points in support for one TAG; do the Order math first.
- **Mobility shell:** Beta Spitfire/KHD + **one Sekudroid** (or linked Epsilon for MSV problem) and a separate RoadBot/Oko Duo; obstacles become alternate routes, not dead ends.
- **Network shell:** Cyberghost HD+ Pitcher + 7pt Kyttä / 15–18pt Oko / 8pt FuzzBot Baggage + separate hacker/KHD cover and optional Millicent. Challenge: the network only matters if a Spotlight/White Noise/Oblivion route is valuable for the mission.
- **Cheap defense shell:** 13–17pt Bluecoats and 12pt Raveneyes near objectives + 19pt Peeler; avoid standing a 40+pt Bronze in an easy long-range ARO unless that trade is intentional.

### Real disagreements, with reasons

| Question | View A | View B / counterargument | Use-case distinction |
|---|---|---|---|
| **Zeta: excellent or inefficient?** | [Loss of Lieutenant N5 TAG panel](https://www.youtube.com/watch?v=dZo_gQWQYSY) argues **S-tier** for O-12: HMC, Climbing Plus, high resilience and ZetBot make it a flagship, with O-12's Lt support. Historic WIP12 Starmada players also built Zeta-focused lists. | [Tactical Awareness Starmada N5](https://www.youtube.com/watch?v=1DKpabLoqyE) is unusually negative: **no Tactical Awareness**, 70–73pts and few cheap Orders make it much worse value *specifically in Starmada*. | Parent-faction TAG grade ≠ Starmada-specific list efficiency. Compare scoring/Orders to a Bronze/Betatrooper core. |
| **Are Bronzes the faction's signature or a trap?** | Tactical Awareness N5 enthusiasts field Bronze HMG/Red Fury/Paramedic backed by Ment and Parvati: durability, CC control, high BTS, recovery and multiple legal teams create a robust push. | Infinity the Dante guest and 2026 Shepherd/Jordan critique highlight **expense**: two Bronzes or a stacked premium Haris can cost as much as a second independent attack group and sacrifice midfield presence. | Start with **one** Bronze and cheap support; add a second only if the mission rewards that much resilience. |
| **Šarko: essential midfield or overpriced?** | Tactical Awareness and Infinity the Dante say Šarko's new Camouflage/Infiltration/WildParrot fills a historic Starmada weakness; it can threaten objectives with KHD/FO. | June 2026 Robert Shepherd/Jordan call it a **costly Zero-like 22–24pt troop** with BS11 and short guns; not a strong value-per-point attacker. | Useful for a planned classified/objective/trap; weak as generic gunfighting filler. |
| **Firebat: tactical flyer or wasteful luxury?** | Aerial Mimetism(-6), NCO and E/M/adhesive toolkit can create angles most grounded pieces cannot. | The June 2026 pair rate its **35–36pt/no-Cover cost** very poorly relative to other factions' flyers; mobility alone does not earn its points. | Only pay for it when there is a specified first-turn route and NCO plan. |
| **Casanova / Andromeda high-variance aggression** | Some hosts like decoys, marker pressure and aggressive infiltration as ways to force defense reactions unavailable to passive Security links. | Tactical Awareness N5 hosts call Casanova **too expensive/too unreliable**, and Andromeda's risk/fragility hard to justify; a credible camo specialist/cheap smoke screen can do more predictable work. | Choose based on deployment zone, mission and failure tolerance; do not build the list assuming a high-risk infiltration success. |
| **Big Betatrooper/Epsilon Core or small team?** | Strong Betatrooper/linked Epsilon gunfighter; a Doctor plus Sekudroid protects expensive assets and reaches difficult angles. | WIP12's experienced Starmada guest dislikes committing a **heavy-HI Core** ("eggs in one basket"), preferring flexible Haris/Duos; later reviewers also note Beta and Epsilon still cost real points. | A Duo/Haris preserves more independent Orders/backup scoring; a Core is justified when its sustained push is the central win condition. |
| **Oko/RoadBot game-breaking?** | Tactical Awareness and historic WIP12 praise rapid objective access, multiple climbing routes and efficient Duo repositioning. | June 2026 comparison calls it a **sensible, modest** Duo rather than dominant: fragile WIP12/13 button presses still lose to control and good ARO positioning. | Strong *scoring infrastructure*, not a replacement for your main attack/defense. |

### Source shortlist (actual MCP transcript review)

**Tier 1: N5 Starmada.** Prefer these for list-building, but apply N5.3 changes from the reference above:

| Resource | What to extract |
|---|---|
| [**Tactical Awareness S3 Ep27 — Starmada (YouTube)**](https://www.youtube.com/watch?v=1DKpabLoqyE) · [Spotify episode](https://open.spotify.com/episode/4gwxsTu15Mc2Tp3wAsuLHr) — **2025-07-14** | **Best focused N5 list laboratory.** Full YouTube and podcast MCP transcripts checked: Beta+Sekudroid, RoadBot+Oko, Saladin/Security Core, Bronze+Ment/Parvati, smoke/CC, Zeta skepticism, Firebat/REM comparisons. |
| [**Infinity the Dante + Tristan (Loss of Lieutenant) — Starmada N5 Initial Reaction**](https://www.youtube.com/watch?v=PKP5G5iEPbg) — **N5 launch** | Full YouTube MCP transcript checked: flexible Security keyword Core, command choices, linked Epsilon, Bronze/Betatrooper cost, Šarko, Shona, Raptor and Starmada-specific tradeoffs. **Early-edition opinions, not current costs.** |
| [**Robert Shepherd + Jordan (Loss of Lieutenant) — June 2026 N5 factions tier list**](https://www.youtube.com/watch?v=1dW3i9dpI34) — **2026-06** | Full YouTube MCP transcript checked: **key skeptical counterweight** on Starmada's expensive midfield, low-end Order economy, Firebat, Beta and RoadBot/Oko. Relative faction grade is opinion. |
| [**GMG/TA battle report — Starmada vs Neoterra, Hardlock**](https://www.youtube.com/watch?v=DJmXoX260Vw) — **ITS17/N5** | Full YouTube MCP transcript checked: concrete layered defense with Bronze/Nyoka, Cyberghost, FuzzBot, Oko Tactical Awareness, RoadBot and smoke/CC. **One game illustrates lines of play; it does not prove a unit's average power.** |

**Tier 2: shared O-12 machines and historical context.**

| Resource | What transfers / caveat |
|---|---|
| [**Loss of Lieutenant Ep142 — N5 TAG Tier List**](https://www.youtube.com/watch?v=dZo_gQWQYSY) · [Spotify](https://open.spotify.com/episode/1h5CJfZC5zBPxdg66o7xIN) — **2025-04** | Full YouTube MCP transcript checked: **pro-Zeta** TAG view; also covers Wrecker, which is **not in Starmada**. |
| [**Tactical Awareness S3 Ep29 — Vanilla O-12**](https://www.youtube.com/watch?v=aGCxiKFBvVY) · [Spotify](https://open.spotify.com/episode/630rsGHb33HMTOrGmx3sIS) — **2025-07** | Previously reviewed MCP transcripts: cross-faction **Oko TA**, Cyberghost and REM network. **Vanilla Fireteams/Gamma/Moonraker/Wrecker are not Starmada legal.** |
| [**Counterintelligence Ep1 — O-12 role-by-role](https://www.youtube.com/watch?v=Vrn9U320eSs) — **N5** | Previously reviewed YouTube MCP transcript: unit-by-unit Zeta, RoadBot, Firebat, Peeler, Kyttä/FuzzBot, Oko and Wrecker. Hosts openly disagree on TAG/bike evaluations; Vanilla-specific comparisons. |
| [**WIP12 Ep120 — Starmada Revisited, Lobo**](https://open.spotify.com/episode/6y9QzLldApsH1fz3K6xTju) — **2023-08; N4** | Podcast MCP transcript checked: tournament-experienced reasoning about **compact Beta/Sekudroid-style Fireteams, road objectives, smoke, Zeta and hacker forks**. **Historical only**; current Fireteam chart outranks old examples. |
| [**WIP12 Ep52 — Starmada (Old)**](https://open.spotify.com/episode/0jezN3bdz1UFdz0MOQ8pyN) — **2022-04; N4** | Podcast MCP transcript checked: early Bronze/Epsilon/Raptor and Fireteam debate, including post-N4 chart addendum. **Do not carry profile prices or formerly legal links into N5.3.** |
| [**Robert Shepherd N4 Starmada Faction Focus**](https://www.youtube.com/watch?v=MtYNqULwLvs) | YouTube MCP transcript checked; useful for historical faction identity, **not** current roster, links, costs or standings. |

**Not counted as reviewed transcripts:** WIP12's *Episode 36: Talking Starmada with Jordan* (2024) was located, but the Podcast MCP returned *no transcript*. It was not used for specific tactical claims.

**Priority when sources conflict:** N5.3 Starmada **Fireteams and profile data in this file** > newer N5 opinion supported by those profiles > older N5 opinion > N4 history. Different authors' assessments stay explicitly side by side.

## Validation notes

- Standard roster count checked from source membership: **42 logical units**.
- Optional-mode records excluded from that count: **2** (`Ŝtormo Spec-Ops`, `O-12 Team-Ops`).
- Fireteam limits verified from `fireteamChart.spec`: Core `1`, Haris `1`, Duo `256`.
- All six named normal Fireteam families and the Wildcard block are represented above.
- FTO restrictions were resolved against exact option names/IDs rather than inferred from unit-level availability.
- In particular, Nyoka options `5/6`, Santiago options `3/4`, Vidocq option `4`, and Tian Gǒu options `8/9` do **not** inherit the respective FTO chart access.
- Conversely, the source rows for Ment Agents are plain `MENT`, so Ment option `1` remains legal in Security and Bronzes despite not carrying `FTO` in its profile name.
- Source pinned at Army `7.26246.159`, backup commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`, blob `995037912a4871ef301469d701b9006bbea3371d`, verified 2026-10-15.

## TAG tactical cross-reference (2026-10-23)

**Zeta** is the S7 HRMC centerpiece for high-powered ranged engagements and vertical routes (Climbing Plus); it needs dedicated hacker-screening and mission scorers, not just another gun. Compare NCO/lieutenant choices *only if this sectorial's current profile actually offers them*. When missions require many distributed specialists, reserve enough points for the excellent Starmada objective network.

For the two-tier **apex/points-value** comparison, TAG counterplay, matchup matrix and direct transcript sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Treat current profiles, points/SWC and canonical Fireteam data above as authoritative.

## Vehicle (VH) tactical cross-reference (2026-10-23)

**Firebat AVA1:** **36/0 AP SMG/Thunderbolt/LRL** provides 0-SWC opportunistic ranged flanks; **35/0 MULTI Rifle/Riotstopper/Akrylat/Blitzen** controls dangerous enemy troopers. **NCO** converts usable LT Orders into attack/retreat/Suppression and **+1 Special Die/Mimetism(-6)** improve FtF quality, but BS13/S7/No Cover still require hard AROs cleared first. This is a **VH**, unlike Starmada's **Zeta TAG** and RoadBot REM; no Fireteam permission.

See [VH apex/value tier list and matchup guide](../../notes/list-building/vehicles-vh.md). **Current profiles, AVA and canonical Fireteam chart above remain authoritative.**

## Hacker and KHD tactical cross-reference (2026-10-23)

**Cyberghost HD+ 21/0.5** projects White Noise/Oblivion via Pitcher, whereas **KHD18/0** protects the same network with Trinity; **Kappa HD13/0.5** supplies cheap general HD. **Knight Santiago FTO KHD+TinBot Firewall(-3) 31/0** is a resilient **Bronzes** team counterhacker; the **Combat Jump KHD38/0** is *not* the linked FTO profile. **PSI-Cop KHD23/0** adds mission/Disco Baller flexibility; **Raptor KHD41/0 + Devabot** buys a strong attack/peripheral fork, not cheap backline cyber coverage. **Why:** White Noise helps Zeta/Bronze clear MSV, and TinBot/KHD helps resist enemy Trinities. Opposing Starmada commentary favors mission-first Cyberghost/TinBot combinations over paying for duplicate isolated hackers.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

The N5.3 [cheerleader/order-generator apex and value guide](../../notes/list-building/cheerleaders-and-order-generators.md) contrasts Orders-per-point, passive utility, matchup dependence, and opposing transcript opinions. **Use this roster for legal AVA, exact profile costs, Training and Fireteam restrictions.**

- 7pt Kyttä — cheap mobile Flash/Repeater/Mimetism Regular Order; check local AVA and deployment safety.
- 8pt FuzzBot — Baggage/Repeater plus Regular Order, excellent if the S4 footprint can be concealed.
- 12pt Kappa — S2 baseline Regular Order, with modest Specialist/Commlink upgrades; compare their actual mission utility against cheaper REMs.
- Warcor — a 3pt Irregular Flash ARO speedbump, not a transferable pool Order without actual conversion.

**Decision:** first buy enough protected *transferable* Regular Orders for the actual Combat Group attacker/scoring plan, then pay for genuine role compression. Irregular/Impetuous, LT, Tactical Awareness and Peripheral bodies are different resources. Account for a packed S3/S4 deployment zone and mandatory Fireteam members.


## ARO apex/value cross-reference (2026-10-23)

[Best ARO units across N5.3 — absolute apex vs points-value](../../notes/list-building/aro-units-apex-and-value.md) compares hidden reactive fire, TR/Neurocinetics, Flash/DTW/expendable defenders and why competing creators disagree. The **roster here** is authoritative for actual costs, Training, AVA and Fireteam construction.

- **Bluecoat Riotstopper/Adhesive** — ~13pt close defence/board-control unit with Sixth Sense; guard objectives and AD entry, not 32-inch gun lanes
- **FuzzBot TR** — 17pt/0SWC Regular cheap Repeater/Combi deterrent; compare stronger but dearer StormBot
- **Kyttä Flashbot** — 7pt Repeater/Flash secondary ARO and cheap Order; insufficient alone against assault gun
- **Warcor 3pt Flash** — disposable Irregular Stun/Orders tax, not a generic Regular cheerleader
- **Total Reaction support** — use recoverable remote for routine lanes, rather than expose primary active gun

**Best circumstance:** long exposed lanes justify a real sniper/missile/linked gun; dense tables, DZ landings and mission rooms favor E/M, mine, Shotgun, Riotstopper and hidden traps. Cover the destination/approach, layer serial threats rather than two pie-sliceable visible guns, and preserve scoring units for the active turn.
