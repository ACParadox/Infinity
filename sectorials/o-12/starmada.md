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

## Validation notes

- Standard roster count checked from source membership: **42 logical units**.
- Optional-mode records excluded from that count: **2** (`Ŝtormo Spec-Ops`, `O-12 Team-Ops`).
- Fireteam limits verified from `fireteamChart.spec`: Core `1`, Haris `1`, Duo `256`.
- All six named normal Fireteam families and the Wildcard block are represented above.
- FTO restrictions were resolved against exact option names/IDs rather than inferred from unit-level availability.
- In particular, Nyoka options `5/6`, Santiago options `3/4`, Vidocq option `4`, and Tian Gǒu options `8/9` do **not** inherit the respective FTO chart access.
- Conversely, the source rows for Ment Agents are plain `MENT`, so Ment option `1` remains legal in Security and Bronzes despite not carrying `FTO` in its profile name.
- Source pinned at Army `7.26246.159`, backup commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`, blob `995037912a4871ef301469d701b9006bbea3371d`, verified 2026-10-15.
