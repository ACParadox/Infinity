---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 1003
sectorial_slug: torchlight-brigade
sectorial_name: Torchlight Brigade
parent_faction: O-12
rules_baseline: N5.3
army_source_version: "7.26246.159"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-15
coverage: "Complete standard Torchlight Brigade roster, standard loadouts/profile states and peripherals, canonical Fireteam chart, exact FTO/context restrictions, reverse Fireteam access, optional-mode hooks, and Reinforcements boundary. Generic Soldier of Fortune catalog entries are excluded."
---

# Torchlight Brigade — N5.3 sectorial reference

## Overview and provenance

This file is the repository reference for **Torchlight Brigade** (Army sectorial ID `1003`). It is intended to be sufficient for ordinary roster, AVA, points/SWC, profile, dependency, and Fireteam-legality questions without reopening Army.

Primary data source:

- Corvus Belli Army data snapshot mirrored by `massayoshi/infinity-army-backup`.
- Pinned source commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` (`army: N5.3 + ITS18`).
- Army dataset: `n5/torchlight-brigade/7.26246.159.json`.
- Source blob: `9ea237fbfcfb5ea46a9466b35593f16fe9f4c75d`.
- Army version: **7.26246.159**.
- Sectorial ID: **1003**.
- Parent O-12 ID: **1001**.
- Reinforcements list ID exposed by the dataset: **1099**.
- Cross-check/reference model commit: InfinityDB `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: **N5.3 + N5 FAQ v0.1**.

Coverage policy:

- The **36 standard logical roster entries** whose faction availability includes Torchlight Brigade are included below.
- Generic Soldier-of-Fortune catalog records present in the aggregate payload with `factions: []` are excluded.
- **Ŝtormo Spec-Ops** and **O-12 Team-Ops** are optional-mode hooks, not ordinary matched-play roster entries.
- Reinforcements (`army_id: 1099`) remain distinct from the normal Torchlight roster and Fireteam chart.
- Composite states and Peripherals stay under their parent logical unit rather than being counted as separate roster entries.
- Fireteam legality comes from the canonical chart below, not from an `FTO` label alone.
- Where Army marks multiple rows `required: true`, this file treats them as a **required source-choice set**: a legal Fireteam needs a member from that required set; every marked row is not simultaneously mandatory.
- Army relates **Jamie Arantes, Netroid Handler** and **Jamie Arantes, Netroid Rover** as alternate versions; do not field both versions in the same normal roster.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Torchlight Brigade |
| Parent faction | O-12 |
| Army ID | 1003 |
| Rules baseline | N5.3 + N5 FAQ v0.1 |
| Army source | 7.26246.159 |
| Standard logical roster units | 36 |
| Optional-mode records | 2 |
| Reinforcement roster | yes — Army ID 1099 |
| Fireteam chart | yes |

## Fireteam limits and interpretation

| Constraint | Value / wording |
|---|---|
| Core | up to 1 Core |
| Haris | up to 1 Haris |
| Duo | effectively unlimited (`256` in Army source) |
| Fireteam families | Silverstars; Mobility; Wreckers |
| Wildcards | PSI-COps; StormBots FTO; Jackboot; Vidocq FTO; Ment; Hippolyta (restricted); Sonya (restricted); Jamie Rover FTO (restricted) |
| Main/Reinforcement mixing | Keep normal Torchlight and Reinforcement charts distinct |

Important profile-level and context restrictions:

- **StormBot Wildcard access is FTO-only**: options `2` and `3`. Option `1` is not FTO and does not receive Wildcard access.
- **Vidocq Wildcard access is FTO-only**: options `1`, `2`, and `3`. Option `4` is not FTO.
- **Jamie Rover Wildcard access is `JAMIE ROVER FTO` and Silverstars-only**: options `1` and `3`. Option `2` is not FTO.
- **Hippolyta** is a Wildcard only in **Silverstars** and **Mobility** Fireteams.
- **Sonya Lacroix** is a Wildcard only in **Silverstars** Fireteams.
- The Wildcard row says **MENT**, not `MENT FTO`; all Torchlight Ment options are legal as Wildcards.
- Mobility lists **NIMROD**, not `NIMROD FTO`; all Nimrod options are legal in Mobility Fireteams.
- **Beasthunter FTO** and **Kyra Sharma FTO** have FTO labels in their profiles but no Torchlight Fireteam-chart access.
- `FTO` in a profile name does not create Fireteam access unless the chart grants it.

## Standard roster index

| Unit ID | Unit | AVA | Troop type | Classification | Regularity | Fireteam access / notes |
|---:|---|---:|---|---|---|---|
| 1785 | StormBots | 2 | REM | Support Troops | Regular | Wildcard, **FTO options 2/3 only** |
| 1774 | Nightshades | 1 | SK | Elite Troops | Regular | — |
| 1781 | Striders, Scouting Forward Unit | 2 | HI | Veteran Troops | Regular | — |
| 1783 | Wreckers, Fire Recon Armored Squadron | 2 | TAG | Mechanized Troops | Regular | Wreckers |
| 1467 | Kyttä Copperbots | 1 | REM | Support Troops | Regular | — |
| 1469 | FuzzBots | 2 | REM | Support Troops | Regular | — |
| 1784 | Moonrakers, Forward Remote Devices | 2 | REM | Support Troops | Regular | — |
| 1463 | Specialized Support Unit Lambda | 2 | LI | Support Troops | Regular | — |
| 1767 | Jackboots | 1 | MI | Veteran Troops | Regular | Wildcard |
| 192 | Yudbots | 2 | REM | Support Troops | Peripheral | Servant support unit |
| 1570 | Beasthunters Free Guild | 1 | SK | Mercenary Troops | Irregular | FTO profile has **no Torchlight Fireteam access** |
| 1786 | Jamie Arantes, Netroid Handler | 1 | HI | Character | Regular | Alternate Jamie version; no Fireteam access |
| 1776 | Hellblazers, CQB Spec. Unit | 3 | HI | Line Troops | Regular, Impetuous | Silverstars; counts as Silverstar source |
| 1568 | Diggers, Armed Prospectors | 1 | HI | Mercenary Troops | Regular, Impetuous | — |
| 1588 | Raveneye Officers | 2 | LI | Support Troops | Regular | Silverstars |
| 1465 | Peeler Copperbots | 1 | REM | Support Troops | Regular | — |
| 1777 | Waveriders Cybercombat Team | 2 | MI | Spec. Trained Troops | Regular | Silverstars |
| 1778 | Kludgers Resolution Team | 3 | MI | Veteran Troops | Regular | Silverstars; Mobility; Wreckers |
| 1872 | Tinkers, Maintenance Support Company | 1 | LI | Support Troops | Regular | — |
| 1447 | Kappa Unit | 1 | LI | Line Troops | Regular | Silverstars |
| 1857 | Firebat Attack Wing | 1 | VH | Elite Troops | Regular | — |
| 1775 | Silverstar Rovers | 5 | HI | Line Troops | Regular | Silverstars; counts as Silverstar source |
| 1782 | Silverstar Prime | 2 | HI | Headquarters Troops | Regular | — |
| 1471 | Hippolyta, Amazon Officer | 1 | WB | Character | Regular, Impetuous | Wildcard: **Silverstars + Mobility only** |
| 1874 | Sāchā, Xenotech Hunters | 1 | LI | Mercenary Troops | Irregular | — |
| 1464 | Oko Copperbots | 2 | REM | Support Troops | Regular | — |
| 1768 | Ment Agents | 1 | LI | Spec. Trained Troops | Regular | Wildcard; **all options** |
| 1787 | Sonya Lacroix, Glo-Pol Marshall | 1 | MI | Character | Regular | Wildcard: **Silverstars only** |
| 1466 | Millicent Copperbots | 1 | REM | Support Troops | Regular | — |
| 1511 | PSI-Cops | 2 | LI | Veteran Troops | Regular | Wildcard |
| 1773 | Vidocq | 1 | LI | Spec. Trained Troops | Regular | Wildcard, **FTO options 1/2/3 only** |
| 1779 | Nimrods Wetworks Detachment | 2 | MI | Elite Troops | Regular | Mobility; **all options** |
| 1780 | Yellowjackets Transorbital Team | 2 | HI | Veteran Troops | Regular | — |
| 1864 | Jamie Arantes, Netroid Rover | 1 | HI | Character | Regular | Silverstars Wildcard, **FTO options 1/3 only**; alternate Jamie version |
| 50 | Warcors | 1 | LI | Mercenary Troops | Irregular | — |
| 1897 | Kyra Sharma, Iron Maiden of the Optimates | 1 | HI | Character | Regular | FTO profile has **no Torchlight Fireteam access** |

### Optional-mode entries

| Unit ID | Unit | Mode | Fireteam hook |
|---:|---|---|---|
| 1923 | Ŝtormo Spec-Ops | Infinity Spec-Ops | Up to 1 in Silverstars Fireteams |
| 1937 | O-12 Team-Ops | Infinity Team-Ops | Optional-mode only; no normal-roster Fireteam row |

## Unit details

Notation: stats are `MOV CC BS PH WIP ARM BTS VITA/STR S`. Source option IDs are retained because FTO legality and otherwise-similar loadouts can depend on them.

### StormBots — `stormbots`

**Unit ID:** 1785 — AVA 2 — REM, Support Troops.

- **Stats:** `15-10 13 13 10 13 3 6 STR2 4`.
- **Rules/equipment:** BS Attack (SR-1), Courage, Remote Presence; Repeater.
- **Option 1:** **31 / 1.5** — Heavy Rocket Launcher (+1B), Pulzar, PARA CC Weapon (-3). Not FTO.
- **Option 2 — STORMBOT FTO:** **29 / 1.5** — Heavy Rocket Launcher, Pulzar, E/M Mine, PARA CC Weapon (-3). **Wildcard legal.**
- **Option 3 — STORMBOT FTO:** **33 / 0** — Combi Rifle (+1B), Pulzar, PARA CC Weapon (-3). **Wildcard legal.**

### Nightshades — `nightshades`

**Unit ID:** 1774 — AVA 1 — SK, Elite Troops.

- **Stats:** `10-10 22 12 12 13 2 0 1 2`.
- **Rules/equipment:** Martial Arts L3, Camouflage, Courage, Forward Deployment (+20), Mimetism (-6), Stealth, Super-Jump, Terrain (Total), Surprise Attack (-3), Hidden Deployment; Bangbomb (+4).
- **Option 1:** **32 / 0** — Boarding Shotgun, Shock Mine, Pistol, E/M CC Weapon (PS=6), PARA CC Weapon (-6).
- **Option 2:** **31 / 0** — Submachine Gun, Drop Bears, D-Charges, Pistol, E/M CC Weapon (PS=6), PARA CC Weapon (-6).
- **Option 3 KHD:** **34 / 0** — option-2 weapons; Killer Hacking Device, Hacker.
- **Option 4 Minelayer:** **32 / 0.5** — Submachine Gun, D-Charges, Shock Mine, Pistol, E/M CC Weapon (PS=6), PARA CC Weapon (-6); Minelayer.

### Striders, Scouting Forward Unit — `striders-scouting-forward-unit`

**Unit ID:** 1781 — AVA 2 — HI, Veteran Troops.

- **Stats:** `10-10 16 12 11 13 3 6 1 2`.
- **Rules:** Camouflage, Forward Deployment (+20), Immunity (Shock), Mimetism (-3), NWI, Stealth, NCO, Terrain (Total), Surprise Attack (-3).
- **Option 1:** **34 / 1** — Red Fury, Pistol, CC Weapon.
- **Option 2 FO:** **29 / 0** — Light Shotgun (+1B), Flash Pulse, Shock Mine, D-Charges, Pistol, CC Weapon; Forward Observer.
- **Option 3 Specialist:** **27 / 0** — Submachine Gun, Shock Mine, D-Charges, Pistol, CC Weapon; Specialist Operative.
- **Option 4 Minelayer:** **28 / 0.5** — option-3 weapons; Minelayer, Specialist Operative.
- **Option 5 Minelayer:** **28 / 0.5** — Submachine Gun, D-Charges, Pistol, CC Weapon; Deployable Repeater; Minelayer, Specialist Operative.

### Wreckers, Fire Recon Armored Squadron — `wreckers-fire-recon-armored-squadron`

**Unit ID:** 1783 — AVA 2 — TAG, Mechanized Troops.

- **Stats:** `15-10 18 13 15 13 6 9 STR3 6`.
- **Rules/equipment:** BS Attack (SR-1), BS Attack (AP), Courage, Dodge (PH=11), Remote Presence, Tactical Awareness, Terrain (Total), GizmoKit (PH=11); ECM: Guided (-6).
- **Option 1:** **57 / 1.5** — HMG, Chain Rifle (+1B), CC Weapon (PS=6); includes ZetBot Ancillary Remote.
- **Option 2:** **55 / 1.5** — Spitfire, Chain Rifle (+1B), CC Weapon (PS=6); includes ZetBot.
- **Option 3:** **51 / 1.5** — Heavy Rocket Launcher, Chain Rifle, CC Weapon (PS=6); BS Attack (+1B); includes ZetBot.
- **ZetBot Ancillary Remote:** `10-10 — — 10 13 0 3 STR1 1`; Courage, Dodge (+3), Mimetism (-3), Specialist Operative, Terrain (Total), Peripheral (Ancillary).

### Kyttä Copperbots — `kyttae-copperbots`

**Unit ID:** 1467 — AVA 1 — REM, Support Troops.

- **Stats:** `15-15 13 8 11 13 0 3 STR1 3`.
- **Rules/equipment:** Remote Presence, Courage, Mimetism (-3); Repeater.
- **Option 1:** **7 / 0** — Flash Pulse, PARA CC Weapon (-3).

### FuzzBots — `fuzzbots`

**Unit ID:** 1469 — AVA 2 — REM, Support Troops.

- **Stats:** `10-10 13 11 10 13 2 3 STR1 4`.
- **Rules/equipment:** Remote Presence, Courage; Baggage.
- **Option 1:** **8 / 0** — PARA CC Weapon (-3); Deactivator, Repeater.
- **Option 2 EVO:** **14 / 0.5** — PARA CC Weapon (-3); EVO Hacking Device, Hacker.
- **Option 3 Total Reaction:** **17 / 0** — Combi Rifle, PARA CC Weapon (-3); Repeater, Total Reaction.

### Moonrakers, Forward Remote Devices — `moonrakers-forward-remote-devices`

**Unit ID:** 1784 — AVA 2 — REM, Support Troops.

- **Stats:** `10-10 14 11 10 12 0 6 STR1 2`.
- **Rules:** Camouflage (1 Use), Courage, Forward Deployment (+20), Mimetism (-3), Remote Presence, Surprise Attack (-3).
- **Option 1:** **14 / 0** — Heavy Shotgun, Adhesive Launcher Rifle, Shock Mine, PARA CC Weapon (-3).
- **Option 2 Minelayer:** **15 / 0.5** — same weapons; Minelayer.

### Specialized Support Unit Lambda — `specialized-support-unit-lambda`

**Unit ID:** 1463 — AVA 2 — LI, Support Troops.

- **Stats:** `10-10 14 11 10 14 1 3 1 2`.
- **Option 1 Engineer:** **16 / 0** — Combi Rifle, Pistol, CC Weapon, D-Charges; Engineer, Deactivator, GizmoKit.
- **Option 2 Engineer:** **17 / 0** — Combi Rifle, D-Charges, Pistol, CC Weapon; Engineer, Deactivator, GizmoKit, Deployable Cover.
- **Option 3 Engineer:** **19 / 0** — Combi Rifle, D-Charges, Armed Turret (Adhesive Launcher Rifle, +1B), Pistol, CC Weapon; Engineer, Deactivator, GizmoKit.
- **Option 4 Doctor:** **16 / 0** — Combi Rifle, Pistol, CC Weapon; MediKit, Doctor.

### Jackboots — `jackboots`

**Unit ID:** 1767 — AVA 1 — MI, Veteran Troops.

- **Stats:** `10-10 15 13 11 13 3 3 1 2`.
- **Rules:** BS Attack (SR-1), Warhorse, Immunity (Enhanced), Combat Instinct, Religious Troop.
- **Option 4 FO:** **26 / 0** — Thunderbolt (+1B), E/M Carbine, Flash Pulse, Pistol, CC Weapon; Forward Observer. **Wildcard.**
- **Option 5 Paramedic:** **21 / 0** — AP Submachine Gun, Light Riotstopper, Panzerfaust, Pistol, CC Weapon; MediKit, Paramedic. **Wildcard.**
- **Option 6 NCO:** **29 / 1** — HMG, Light Riotstopper, Pistol, CC Weapon; NCO. **Wildcard.**

### Yudbots — `yudbots`

**Unit ID:** 192 — AVA 2 — REM, Support Troops.

- **Stats:** `15-10 11 8 10 13 0 3 STR1 1`.
- **Rules:** Peripheral (Servant), Courage, Mimetism (-3).
- **Option 1:** **3 / 0** — PARA CC Weapon (-3). No Order; attach per Servant rules.

### Beasthunters Free Guild — `beasthunters-free-guild`

**Unit ID:** 1570 — AVA 1 — SK, Mercenary Troops; Irregular.

- **Stats:** `10-10 21 11 13 12 0 0 1 2`.
- **Base rules:** Mimetism (-3), Stealth, Super-Jump, Terrain (Total), Religious Troop.
- **Option 1 — BEASTHUNTER FTO:** **9 / 0** — Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CC Weapon (PS=5). **No Torchlight Fireteam chart access despite FTO label.**
- **Option 2:** **15 / 0** — Heavy Flamethrower, Tactical Bow, AP Mine, Pistol, DA CC Weapon (PS=5); Surprise Attack (-3), Camouflage, Forward Deployment (+20).
- **Option 3:** **15 / 0** — Heavy Flamethrower, Panzerfaust, AP Mine, Pistol, DA CC Weapon (PS=5); Surprise Attack (-3), Camouflage, Forward Deployment (+20).

### Jamie Arantes, Netroid Handler — `jamie-arantes-netroid-handler`

**Unit ID:** 1786 — AVA 1 — HI, Character.

- **Stats:** `15-5 22 13 14 14 4 9 2 4`.
- **Rules:** Martial Arts L1, Courage, Forward Deployment (+20), Dodge (+5), Guard, Mimetism (-3), Decoy (1), Terrain (Total), Stealth, NCO, Jump (+7.5).
- **Option 1:** **49 / 0** — Plasma Rifle, Akrylat-Kanone, Nanopulser, Silenced Pistol, AP CC Weapon (PS=5).
- **Option 2:** **52 / 0** — option-1 weapons plus Armed Turret (Combi Rifle).
- **Option 3 Lieutenant (+1 Order):** **49 / 0** — option-1 weapons; Lieutenant (+1 Order).
- **Roster relation:** alternate Jamie version with Jamie Rover; do not field both.

### Hellblazers, CQB Spec. Unit — `hellblazers-cqb-spec-unit`

**Unit ID:** 1776 — AVA 3 — HI, Line Troops; Regular, Impetuous.

- **Stats:** `15-5 22 12 13 13 3 6 2 2`.
- **Rules:** Martial Arts L2, Courage, Dodge (+5), Stealth, Impetuous, Limited Cover, Jump (+7.5).
- **Option 1:** **18 / 0** — Light Shotgun, Flammenspeer, Pistol, EXP CC Weapon (PS=6).
- **Option 2:** **19 / 0** — Submachine Gun, Blitzen, Pistol, EXP CC Weapon (PS=6).
- **Option 3:** **19 / 0** — Boarding Shotgun, Akrylat-Kanone, Pistol, EXP CC Weapon (PS=6).
- **Fireteam:** native Silverstars member; counts toward the required Silverstar/Hellblazer source-choice set.

### Diggers, Armed Prospectors — `diggers-armed-prospectors`

**Unit ID:** 1568 — AVA 1 — HI, Mercenary Troops; Regular, Impetuous.

- **Full-Power stats:** `10-10 21 11 13 12 3 0 2 2`.
- **Battle-Ravaged stats:** `10-10 21 10 12 12 2 0 2 2`.
- **Rules:** CC Attack (+1B), Booty, Courage, Natural Born Warrior, Impetuous, No Cover; Full-Power state also has Dodge (+2.5) and Transmutation (1).
- **Option 1:** **18 / 0** — Rifle, Light Shotgun, Grenades, Pistol, AP CC Weapon (PS=6).
- **Option 2:** **14 / 0** — Chain Rifle (+1B), Grenades, Pistol, AP CC Weapon (PS=6).

### Raveneye Officers — `raveneye-officers`

**Unit ID:** 1588 — AVA 2 — LI, Support Troops.

- **Stats:** `10-10 15 11 10 13 1 3 1 2`.
- **Rules/equipment:** Immunity (Shock), Minelayer, Forward Observer; Deactivator.
- **Option 1:** **12 / 0** — Submachine Gun, E/Marat, Flash Pulse, E/M Mine, Pistol, CC Weapon.
- **Option 2:** **12 / 0** — Submachine Gun, E/Marat, Flash Pulse, Cybermine, Pistol, CC Weapon.
- **Option 4 Chain of Command:** **18 / 0** — option-1 weapons; Holomask, Chain of Command.
- **Option 5 Lieutenant (+1 Order):** **17 / 0** — option-1 weapons; Holomask, Lieutenant (+1 Order).
- **Fireteam:** Silverstars.

### Peeler Copperbots — `peeler-copperbots`

**Unit ID:** 1465 — AVA 1 — REM, Support Troops.

- **Stats:** `15-10 13 11 10 13 0 3 STR1 3`.
- **Rules/equipment:** Remote Presence, Courage, Total Reaction, Climbing Plus; 360º Visor.
- **Option 1:** **24 / 1** — HMG, PARA CC Weapon (-3).
- **Option 2:** **19 / 0** — Thunderbolt (+1B), PARA CC Weapon (-3).

### Waveriders Cybercombat Team — `waveriders-cybercombat-team`

**Unit ID:** 1777 — AVA 2 — MI, Spec. Trained Troops.

- **Stats:** `15-5 18 12 11 13 3 6 1 2`.
- **Rules:** Mimetism (-3), Stealth, Terrain (Total).
- **Option 1 Hacker:** **23 / 0.5** — Boarding Shotgun, Pitcher, D-Charges, Pistol, CC Weapon; Hacking Device with Oblivion (+1B), Hacker.
- **Option 2 Hacker:** **22 / 0.5** — Submachine Gun, Pitcher, D-Charges, Pistol, CC Weapon; Hacking Device with Oblivion (+1B), Hacker.
- **Option 3 KHD:** **20 / 0** — Submachine Gun, Pitcher, D-Charges, Pistol, CC Weapon; Killer Hacking Device with Trinity (SR-1), Hacker.
- **Fireteam:** Silverstars.

### Kludgers Resolution Team — `kludgers-resolution-team`

**Unit ID:** 1778 — AVA 3 — MI, Veteran Troops.

- **Stats:** `15-5 16 13 11 14 2 6 1 2`.
- **Rules:** Immunity (Shock), Mimetism (-3), Super-Jump, Terrain (Total), Warhorse.
- **Option 1 Engineer:** **23 / 0** — Boarding Shotgun, Panzerfaust, D-Charges, Pistol, CC Weapon; Engineer, Deactivator, GizmoKit.
- **Option 2 Engineer:** **23 / 0** — Submachine Gun, Panzerfaust, D-Charges, Disco Baller, Pistol, CC Weapon; Engineer, Deactivator, GizmoKit.
- **Option 3 Doctor:** **23 / 0** — Submachine Gun, Adhesive Launcher Rifle, Pistol, CC Weapon; MediKit, Doctor.
- **Fireteams:** Silverstars; required source unit for Mobility; may join Wreckers.

### Tinkers, Maintenance Support Company — `tinkers-maintenance-support-company`

**Unit ID:** 1872 — AVA 1 — LI, Support Troops.

- **Stats:** `10-10 12 11 10 13 0 3 1 2`.
- **Rules/equipment:** Specialist Operative; Deactivator, GizmoKit, Repeater.
- **Option 1:** **11 / 0** — Adhesive Launcher Rifle, Flash Pulse (PS=6 source modifier), Stun Pistol, PARA CC Weapon (-3).

### Kappa Unit — `kappa-unit`

**Unit ID:** 1447 — AVA 1 — LI, Line Troops.

- **Stats:** `10-10 14 12 10 13 1 0 1 2`.
- **Rules:** Immunity (Shock).
- **Option 1:** **12 / 0** — Combi Rifle, Pistol, CC Weapon.
- **Option 5 Hacker:** **13 / 0.5** — Submachine Gun, Pistol, CC Weapon; Hacking Device, Hacker.
- **Option 6 FO:** **14 / 0** — Combi Rifle, Flash Pulse, Pistol, CC Weapon; Deployable Repeater, Forward Observer.
- **Option 7 Paramedic:** **14 / 0** — Combi Rifle, Pistol, CC Weapon; MediKit, Paramedic.
- **Option 10 Commlink:** **14 / 0** — Combi Rifle, Pistol, CC Weapon; Commlink (+1), Specialist Operative.
- **Fireteam:** Silverstars, maximum 1.

### Firebat Attack Wing — `firebat-attack-wing`

**Unit ID:** 1857 — AVA 1 — VH, Elite Troops.

- **Stats:** `20-5 — 13 12 13 4 6 STR2 7`.
- **Rules:** Aerial, Courage, Dodge (-3), GizmoKit (PH=13), Mimetism (-6), No Cover, Super-Jump (Jet Propulsion), Terrain (Total), Super-Jump (+7.5), BS Attack (+1SD), NCO, Tech-Recovery.
- **Option 1:** **36 / 0** — AP Submachine Gun, Thunderbolt, Light Rocket Launcher (PS=6).
- **Option 2:** **35 / 0** — MULTI Rifle, Heavy Riotstopper, Akrylat-Kanone, Blitzen.

### Silverstar Rovers — `silverstar-rovers`

**Unit ID:** 1775 — AVA 5 — HI, Line Troops.

- **Stats:** `15-5 16 13 12 13 3 6 2 2`.
- **Rules:** Courage, Dodge (+2.5), Specialist Operative, Jump (+7.5).
- **Option 1:** **27 / 0** — Combi Rifle, Light Riotstopper, Heavy Pistol (+1B), CC Weapon; TinBot: Firewall (-3).
- **Option 2:** **28 / 0** — MULTI Rifle, Light Riotstopper, Heavy Pistol (+1B), CC Weapon.
- **Option 3 FO:** **27 / 0** — Combi Rifle, Light Riotstopper, Flash Pulse, D-Charges, Heavy Pistol (+1B), CC Weapon; Forward Observer.
- **Option 4 Paramedic:** **28 / 0** — Combi Rifle, Light Riotstopper, Heavy Pistol (+1B), CC Weapon; MediKit, Paramedic.
- **Option 5 HMG Tactical Awareness:** **37 / 1.5** — HMG, Heavy Pistol (+1B), CC Weapon; Tactical Awareness.
- **Option 6 Tactical Awareness:** **30 / 0** — Combi Rifle, Light Riotstopper, Heavy Pistol (+1B), CC Weapon; TinBot: Firewall (-3), Tactical Awareness.
- **Option 7 Missile Launcher Tactical Awareness:** **31 / 1.5** — Missile Launcher, Heavy Pistol (+1B), CC Weapon; Tactical Awareness.
- **Option 8 Lieutenant:** **28 / 0** — MULTI Rifle, Light Riotstopper, Heavy Pistol (+1B), CC Weapon; Lieutenant.
- **Fireteam:** native Silverstars member; counts toward required Silverstar/Hellblazer source-choice set.

### Silverstar Prime — `silverstar-prime`

**Unit ID:** 1782 — AVA 2 — HI, Headquarters Troops.

- **Stats:** `15-5 18 14 13 13 5 9 2 5`.
- **Rules/equipment:** BS Attack (-3 source modifier), Courage, Tactical Awareness; Multispectral Visor L1.
- **Option 1:** **53 / 1.5** — HMG (PS=4 source modifier), Heavy Riotstopper, Heavy Pistol, Shock CC Weapon (PS=6); Tactical Awareness.
- **Option 2 Lieutenant:** **53 / 1** — same weapons; Tactical Awareness, Lieutenant.
- **Fireteam:** none in the current Torchlight chart despite the Silverstar name.

### Hippolyta, Amazon Officer — `hippolyta-amazon-officer`

**Unit ID:** 1471 — AVA 1 — WB, Character; Regular, Impetuous.

- **Stats:** `15-5 24 13 14 14 3 3 2 2`.
- **Rules:** Impetuous, Martial Arts L3, Berserk, Courage, Dodge (+2.5), Mimetism (-6), Stealth, Super-Jump, Limited Cover.
- **Option 1:** **37 / 0** — Breaker Combi Rifle, Nanopulser, Flash Pulse, Smoke Grenades, Pistol, EXP CC Weapon (PS=4).
- **Wildcard restriction:** Silverstars and Mobility Fireteams only.

### Sāchā, Xenotech Hunters — `sacha-xenotech-hunters`

**Unit ID:** 1874 — AVA 1 — LI, Mercenary Troops; Irregular.

- **Stats:** `10-10 17 11 12 13 0 3 1 2`.
- **Rules:** Forward Deployment (+10), Booty, Terrain (Total), Climbing Plus, Specialist Operative.
- **Option 1:** **6 / 0** — Flash Pulse, E/M Grenades (+1B), Stun Pistol (+1B), CC Weapon.

### Oko Copperbots — `oko-copperbots`

**Unit ID:** 1464 — AVA 2 — REM, Support Troops.

- **Stats:** `15-10 13 11 10 13 0 3 STR1 3`.
- **Rules/equipment:** Remote Presence, Triangulated Fire, Courage, Forward Observer, Sensor, Climbing Plus; Deactivator, Repeater.
- **Option 1:** **15 / 0** — Combi Rifle, Flash Pulse, PARA CC Weapon (-3).
- **Option 2 Tactical Awareness:** **18 / 0** — same weapons; Tactical Awareness.

### Ment Agents — `ment-agents`

**Unit ID:** 1768 — AVA 1 — LI, Spec. Trained Troops.

- **Stats:** `10-10 17 12 10 13 1 3 1 2`.
- **Rules/equipment:** Chain of Command, Stealth, Number 2; Biometric Visor.
- **Option 1 — MENT:** **15 / 0** — Heavy Riotstopper (+2B), Assault Pistol, PARA CC Weapon (-3). **Wildcard legal.**
- **Option 2 — MENT FTO:** **15 / 0** — Light Shotgun, Pistol, PARA CC Weapon (-3). **Wildcard legal.**
- **Option 3 — MENT FTO:** **14 / 0** — Heavy Riotstopper (+1B), Assault Pistol, PARA CC Weapon (-3). **Wildcard legal.**
- **Option 4 — MENT FTO Hacker:** **20 / 0.5** — Light Shotgun, Pistol, PARA CC Weapon (-3); Hacking Device, Hacker. **Wildcard legal.**

### Sonya Lacroix, Glo-Pol Marshall — `sonya-lacroix-glo-pol-marshall`

**Unit ID:** 1787 — AVA 1 — MI, Character.

- **Stats:** `15-5 22 13 12 13 2 6 1 2`.
- **Rules/equipment:** Martial Arts L2, Courage, Immunity (Shock), Stealth, Terrain (Total), Combat Instinct, Specialist Operative; Albedo (-6), X Visor.
- **Option 1:** **28 / 0** — MULTI Rifle, E/Mitter, MULTI Pistol, Shock CC Weapon (PS=6).
- **Option 2 NCO:** **28 / 0** — MULTI Rifle, E/Marat, MULTI Pistol, Shock CC Weapon (PS=6); NCO.
- **Option 3 Lieutenant:** **28 / +1 SWC** — MULTI Rifle, E/Mitter, MULTI Pistol, Shock CC Weapon (PS=6); Lieutenant.
- **Wildcard restriction:** Silverstars only.

### Millicent Copperbots — `millicent-copperbots`

**Unit ID:** 1466 — AVA 1 — REM, Support Troops.

- **Stats:** `15-10 13 12 10 13 0 3 STR1 3`.
- **Rules:** Remote Presence, BS Attack (Guided), Courage.
- **Option 1:** **16 / 1.5** — Missile Launcher, PARA CC Weapon (-3).

### PSI-Cops — `psi-cops`

**Unit ID:** 1511 — AVA 2 — LI, Veteran Troops.

- **Stats:** `10-10 15 13 10 13 1 6 1 2`.
- **Rules/equipment:** Immunity (Shock), Mimetism (-3), Specialist Operative, Combat Instinct; X Visor.
- **Option 3:** **26 / 0** — MULTI Marksman Rifle, Nanopulser (+1B), Heavy Pistol, CC Weapon; Biometric Visor, Discover (+3). **Wildcard.**
- **Option 4 Hacker:** **24 / 0.5** — Combi Rifle, Nanopulser (+1B), Heavy Pistol, CC Weapon; Hacking Device, Hacker. **Wildcard.**
- **Option 5 KHD:** **23 / 0** — Combi Rifle, Nanopulser (+1B), Heavy Pistol, Disco Baller, CC Weapon; Killer Hacking Device, Hacker. **Wildcard.**
- **Option 7 MSV1:** **27 / 0** — MULTI Marksman Rifle, Nanopulser (+1B), Heavy Pistol, CC Weapon; Multispectral Visor L1. **Wildcard.**
- **Option 8 MSV1 turret:** **30 / 0** — option-7 weapons plus Armed Turret (Thunderbolt); Multispectral Visor L1. **Wildcard.**

### Vidocq — `vidocq`

**Unit ID:** 1773 — AVA 1 — LI, Spec. Trained Troops.

- **Stats:** `10-10 16 13 10 13 1 3 1 2`.
- **Rules:** Mimetism (-3), Stealth, NCO, Terrain (Total).
- **Option 1 — VIDOCQ FTO:** **15 / 0** — Boarding Shotgun, Boarding Pistol, CC Weapon. **Wildcard legal.**
- **Option 2 — VIDOCQ FTO Doctor:** **19 / 0** — option-1 weapons; MediKit, Doctor. **Wildcard legal.**
- **Option 3 — VIDOCQ FTO:** **26 / 1.5** — MULTI Sniper Rifle, Breaker Pistol, CC Weapon; Multispectral Visor L1. **Wildcard legal.**
- **Option 4:** **30 / 1.5** — same weapons as option 3; Multispectral Visor L1, Surprise Attack (-3), Camouflage. Not FTO.

### Nimrods Wetworks Detachment — `nimrods-wetworks-det`

**Unit ID:** 1779 — AVA 2 — MI, Elite Troops.

- **Stats:** `15-5 16 13 11 13 2 6 1 2`.
- **Rules/equipment:** Immunity (Shock), Mimetism (-3), Stealth, Super-Jump, Terrain (Total), BS Attack (Shock); Multispectral Visor L2.
- **Option 1:** **27 / 0** — AP Submachine Gun, Flash Pulse, Shock Mine, Pistol, CC Weapon; Surprise Attack (-3), Forward Deployment (+20), Hidden Deployment.
- **Option 2 — NIMROD FTO:** **29 / 0.5** — AP Marksman Rifle, E/M Carbine, Pistol, CC Weapon.
- **Option 3 — NIMROD FTO:** **28 / 0.5** — Thunderbolt (+1B), Light Shotgun, Pistol, CC Weapon.
- **Fireteam:** Mobility row is `NIMROD`, so **all three options** qualify.

### Yellowjackets Transorbital Team — `yellowjackets-transorbital-team`

**Unit ID:** 1780 — AVA 2 — HI, Veteran Troops.

- **Stats:** `10-10 15 12 12 13 3 6 1 2`.
- **Rules:** Dodge (+5), Immunity (Shock), Mimetism (-3), Parachutist, Combat Jump, NWI, Stealth, Super-Jump (Jet Propulsion).
- **Option 1:** **25 / 0** — Boarding Shotgun, D-Charges, Boarding Pistol, CC Weapon.
- **Option 2:** **29 / 0** — Combi Rifle, Light Riotstopper, Boarding Pistol, CC Weapon.
- **Option 3 Specialist:** **25 / 0** — Submachine Gun, D-Charges, Boarding Pistol, CC Weapon; Specialist Operative.
- **Option 4 Hacker:** **29 / 0.5** — option-3 weapons; Hacking Device, Hacker.

### Jamie Arantes, Netroid Rover — `jamie-arantes-netroid-rover`

**Unit ID:** 1864 — AVA 1 — HI, Character.

- **Stats:** `15-5 22 13 14 14 4 9 2 2`.
- **Rules:** Martial Arts L1, Courage, Dodge (+5), Mimetism (-3), Jump (+7.5), Stealth, NCO, Terrain (Total).
- **Option 1 — JAMIE ROVER FTO:** **47 / 0** — Plasma Rifle, Akrylat-Kanone, Nanopulser, Silenced Pistol, AP CC Weapon (PS=5); X Visor. **Silverstars Wildcard legal.**
- **Option 2 — JAMIE ROVER:** **53 / 0** — Plasma Rifle, Akrylat-Kanone, Nanopulser, Armed Turret (Combi Rifle), Silenced Pistol, AP CC Weapon (PS=5); Parachutist, Decoy (1). Not FTO.
- **Option 3 — JAMIE ROVER FTO Lieutenant (+1 Order):** **49 / 0** — option-1 weapons; X Visor, Lieutenant (+1 Order). **Silverstars Wildcard legal.**
- **Roster relation:** alternate Jamie version with Jamie Handler; do not field both.

### Warcors — `warcors-war-correspondents`

**Unit ID:** 50 — AVA 1 — LI, Mercenary Troops; Irregular.

- **Stats:** `10-10 11 9 11 13 0 0 1 2`.
- **Rules:** Journalist.
- **Option 1:** **3 / 0** — Flash Pulse, Stun Pistol, PARA CC Weapon (-3); 360º Visor.
- **Option 2:** **3 / 0** — same weapons; Sixth Sense.

### Kyra Sharma, Iron Maiden of the Optimates — `kyra-sharma-the-iron-maiden-of-the-optimates`

**Unit ID:** 1897 — AVA 1 — HI, Character.

- **Stats:** `15-10 18 14 12 14 3 3 2 2`.
- **Rules/equipment:** BS Attack (SR-1), Courage, Dodge (+5), Immunity (ARM), Immunity (Critical), Regeneration, Tactical Awareness, Super-Jump (+7.5), Super-Jump (Jet Propulsion); MediKit (+1B).
- **Option 1 — KYRA SHARMA FTO:** **45 / 0** — MULTI Marksman Rifle, Light Riotstopper (+1B), WildParrot, Breaker Pistol (+1SD), PARA CC Weapon (-6); Paramedic.
- **Fireteam:** **none in the current Torchlight chart despite the FTO label.**

## Fireteams

The following section is canonical for Torchlight Fireteam legality. The reverse index below is derivative.

### FT-01 — Silverstars Fireteams

**Types:** Duo, Haris, Core  
**Wildcard team:** no  
**Required-source semantics:** at least one member from the `SILVERSTAR` / `HELLBLAZER` required set.

| Member | Unit ID | Required-source set | Min | Max | Counts as / chart comment | FTO restriction | Allowed option IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Silverstar Rovers | 1775 | yes | 0 | 5 | Silverstar | — | all | Native source unit |
| Hellblazers | 1776 | yes | 0 | 3 | Silverstar | — | all | Native source unit |
| Waveriders | 1777 | no | 0 | 2 | Silverstar | — | all | — |
| Kappa Unit | 1447 | no | 0 | 1 | — | — | all | — |
| Raveneye Officers | 1588 | no | 0 | 1 | — | — | all | — |
| Kludgers | 1778 | no | 0 | 1 | — | — | all | — |
| Ŝtormo Spec-Ops | 1923 | no | 0 | 1 | Spec-Ops | optional mode | optional-mode only | Not standard matched-play roster |

Effective Wildcards that may join Silverstars are listed under **Wildcards** below.

### FT-02 — Mobility Fireteams

**Types:** Duo, Haris  
**Wildcard team:** no  
**Required-source semantics:** at least one Kludger.

| Member | Unit ID | Required | Min | Max | Counts as / chart comment | FTO restriction | Allowed option IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Kludgers | 1778 | yes | 0 | 3 | Mobility | — | all | Required source unit |
| Nimrods | 1779 | no | 0 | 1 | — | **none** | all | Chart says `NIMROD`, so non-FTO option 1 also qualifies |

Effective Wildcards for Mobility exclude Sonya and Jamie Rover but include Hippolyta.

### FT-03 — Wreckers Fireteams

**Types:** Duo  
**Wildcard team:** no

| Member | Unit ID | Required | Min | Max | Counts as | FTO restriction | Allowed option IDs | Notes |
|---|---:|---|---:|---:|---|---|---|---|
| Wreckers | 1783 | no | 1 | 2 | — | — | all | At least one Wrecker |
| Kludgers | 1778 | no | 0 | 1 | — | — | all | — |

### Wildcards

| Unit | Unit ID | Max | Counts as / context | FTO/profile restriction | Effective access |
|---|---:|---:|---|---|---|
| PSI-Cops | 1511 | 2 | — | none | Silverstars, Mobility, Wreckers |
| StormBots | 1785 | 2 | FTO | **options 2, 3 only** | Silverstars, Mobility, Wreckers |
| Jackboots | 1767 | 1 | — | none | Silverstars, Mobility, Wreckers |
| Vidocq | 1773 | 1 | — | **FTO options 1, 2, 3 only** | Silverstars, Mobility, Wreckers |
| Ment Agents | 1768 | 1 | — | chart says `MENT`; **all options** | Silverstars, Mobility, Wreckers |
| Hippolyta | 1471 | 1 | Silverstar & Mobility | none | **Silverstars, Mobility only** |
| Sonya Lacroix | 1787 | 1 | Silverstar | none | **Silverstars only** |
| Jamie Rover | 1864 | 1 | Silverstar | **FTO options 1, 3 only** | **Silverstars only** |

## Unit → Fireteam access index

| Unit | Effective Fireteam access |
|---|---|
| StormBots | Wildcard in Silverstars / Mobility / Wreckers, **options 2/3 only** |
| Nightshades | none |
| Striders | none |
| Wreckers | Wreckers Duo |
| Kyttä | none |
| FuzzBots | none |
| Moonrakers | none |
| Lambda | none |
| Jackboots | Wildcard in Silverstars / Mobility / Wreckers |
| Yudbots | none |
| Beasthunters | none; FTO label alone grants nothing |
| Jamie Handler | none |
| Hellblazers | Silverstars Duo / Haris / Core; required-source set |
| Diggers | none |
| Raveneye | Silverstars Duo / Haris / Core |
| Peeler | none |
| Waveriders | Silverstars Duo / Haris / Core |
| Kludgers | Silverstars Duo / Haris / Core; Mobility Duo / Haris; Wreckers Duo |
| Tinkers | none |
| Kappa | Silverstars Duo / Haris / Core |
| Firebat | none |
| Silverstar Rovers | Silverstars Duo / Haris / Core; required-source set |
| Silverstar Prime | none |
| Hippolyta | Wildcard in **Silverstars and Mobility only** |
| Sāchā | none |
| Oko | none |
| Ment Agents | Wildcard in Silverstars / Mobility / Wreckers; **all options** |
| Sonya Lacroix | Wildcard in **Silverstars only** |
| Millicent | none |
| PSI-Cops | Wildcard in Silverstars / Mobility / Wreckers |
| Vidocq | Wildcard in Silverstars / Mobility / Wreckers, **options 1/2/3 only** |
| Nimrods | Mobility Duo / Haris, **all options** |
| Yellowjackets | none |
| Jamie Rover | Wildcard in **Silverstars only**, **options 1/3 only** |
| Warcors | none |
| Kyra Sharma | none; FTO label alone grants nothing |
| Ŝtormo Spec-Ops | Silverstars optional-mode row only |
| O-12 Team-Ops | optional mode; no normal Fireteam access |

## Composite / dependency notes

- **Wreckers** include a ZetBot Ancillary Remote in each standard Wrecker option.
- **Jamie Handler** and **Jamie Rover** are alternate Jamie Arantes roster versions linked by Army; do not field both in one normal list.
- **Yudbots** are Servant Peripherals and do not generate Orders of their own.
- **Ŝtormo Spec-Ops** and **O-12 Team-Ops** belong to optional game modes and are not counted among the 36 standard logical units.
- The generic Soldier-of-Fortune catalog entries in the source payload are not standard Torchlight roster entries and are intentionally excluded.

## Validation notes

- Verified against Army snapshot **7.26246.159**, source blob `9ea237fbfcfb5ea46a9466b35593f16fe9f4c75d`, mirrored in backup commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` dated **2026-09-03**.
- Fireteam chart source limits: `CORE: 1`, `HARIS: 1`, `DUO: 256`.
- Canonical Fireteam families found in the source: **Silverstars**, **Mobility**, **Wreckers**, plus Wildcards.
- FTO labels were not treated as permissions. Chart context was applied explicitly to StormBots, Vidocq, Jamie Rover, Beasthunters, Kyra Sharma, and Nimrods.
- The canonical **Fireteams** section takes precedence over the reverse access index if an inconsistency is ever introduced during later edits.
