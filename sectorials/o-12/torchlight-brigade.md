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

## Community tactics and transcript synthesis — Torchlight Brigade (2026-10-23)

**Community interpretation, not new Army data.** Read the N5.3 unit options, costs, availability, and especially the canonical Fireteam chart **above** before applying these conclusions. This is a concise synthesis of the linked **YouTube and podcast MCP transcripts**. It preserves disagreements, including the difference between the enthusiastic 2024 tournament experience, the 2025 list-building guides, and the more skeptical June 2026 comparative assessment. N4 results and pre-N5.3 examples are never authoritative for current profiles.

### Why Torchlight succeeds — and why it disappoints

1. **Pay for an attack plan, not for all the heavy infantry.** Torchlight has outstanding *individual* tools (Silverstar Prime, Wrecker, Waverider, Moonraker, Hippolyta, Kludger) but only a thin supply of truly cheap Regular Orders. A stack of Silverstar Rovers, Jamie, Prime and Wrecker may look intimidating and still be outactivated. Begin with **one reliable long-range gun**, one compact supporting team, a midfield scoring plan and enough surviving Orders to finish missions.
2. **The faction's distinct identity is a layered middle, not a five-HI Core.** Two 14–15pt Moonrakers, one or two 27–29pt Striders, Raveneye mines, a 9/15pt Beasthunter and hacking repeaters can **pre-place uncertainty and delay**. The expensive attack piece then shoots a hole; the remaining midfield units score after the enemy spends Orders clearing mines and Camo. This is the positive *why* behind the 2024 tournament-winning construction.
3. **Treat an efficient Silverstars team as an assembled toolkit.** A **Hellblazer (18–19)** supplies the compulsory native source cheaply, a **Waverider (20–23)** supplies Pitcher/hacking, and a **Vidoc FTO MSV1 sniper (26)** or **PSI-Cop (26–30)** supplies actual gunfighting. This uses the sectorial's Fireteam access without buying several expensive Silverstar Rovers just to make the same link.
4. **Spend the extra Lieutenant Orders purposefully.** Raveneye **17pt Lt (+1 Order)**, Jamie Handler/Rover Lt (+1 Order) and NCO recipients (Strider, Vidoc, Jackboot, Sonya, Firebat, Jamie) can make an apparently smaller pool play bigger. Include **Ment CoC (14–20)** when the Lt is exposed: a lost Lt can undo the entire economy advantage. NCO orders are not an excuse to spend all Orders on gunfighting rather than objectives.
5. **Hackers enable difficult approaches, but do not magically fix the army's shooting costs.** Waverider **Pitcher + upgraded Oblivion/Trinity**, Kappa/PSI-Cop/Ment hackers, Kyttä/Oko/Fuzz repeaters and StormBot's Repeater force armor and hacker decisions; the **Disco Baller** on a Kludger engineer or PSI-Cop KHD offers visibility control. However, unlike Vanilla O-12, **Torchlight lacks the Cyberghost HD+ White Noise/Pitcher package**. Do not silently borrow Vanilla's hacking coverage.
6. **Two competing overall assessments matter.** Tactical Awareness S3 Ep28 emphasizes how much control, hacking, defensive geometry, and mission coverage Torchlight can combine. [Robert Shepherd's June 2025 dedicated review](https://www.youtube.com/watch?v=PZKCQAupCMs) and his [June 2026 review with Jordan](https://www.youtube.com/watch?v=1dW3i9dpI34) argue the roster has too many merely *fairly priced* units, with expensive Silverstars/Yellowjackets and fragile attack plans. **Both** are plausible: competent list filtering makes the sectorial more competitive than buying its most thematic models indiscriminately.

### Fireteam modules (all checked against the *current* N5.3 chart)

| Module | Reason to take it | Critical restrictions / when not to |
|---|---|---|
| **Silverstars Core or Haris:** Hellblazer + Waverider HD/KHD + Vidoc FTO MSV1 sniper, PSI-Cop or other legal Wildcard | Gives an **18–19pt Core/Haris source**, linked Pitcher and a credible long-range/MSV gun; Waverider's BTS6, Stealth and Mimetism help contest enemy hackers while Hellblazer threatens CC, Flammenspeer/Blitzen/Akrylat. Flexible enough to take a mission-specialist replacement. | A Silverstars team needs **at least one Silverstar Rover or Hellblazer**. Kappa (max one), Raveneye (max one), Kludger, Waverider and Wildcards **do not independently satisfy that source set**. Only **one Core and one Haris** across the army. |
| **Silverstar Rover as deliberate specialist/TA gun:** 27–37pt | Unlike a pure filler model, Rover has **2 Wounds, BTS6, Specialist Operative**, TinBot/FO/Paramedic choices, and **31pt TA Missile Launcher / 37pt TA HMG**. A Rover can lead a fireteam when needing resilient objectives or a specific TA ARO. | It is **BS13, ARM3, no Mimetism**, with built-in extras that cost points. Robert Shepherd recommends often taking *zero*: buy one only when its specific TinBot, Tactical Awareness, gun or specialist role is worth more than a cheaper Hellblazer anchor. |
| **Mobility Duo/Haris:** Kludger Doctor or Engineer + Hippolyta; optionally Nimrod | Kludger **23pt WIP14 Doctor/Engineer** fixes key units and moves/super-jumps with **Hippolyta's Mimetism(-6), smoke, Breaker rifle and strong CC**. A **Nimrod MSV2** adds an actual shooting answer through smoke, plus AP Marksman/E/M or Thunderbolt threat. | The native **required member is a Kludger**; Nimrod alone/Hippolyta alone cannot found Mobility. Nimrod **options 1–3** are chart-legal (the row says plain NIMROD). A 3-model assault group costs considerably more than a basic Kludger/Hippolyta Duo. |
| **Wrecker TAG Duo:** Wrecker 51pt HRL + **Kludger Engineer 23pt** | Tactical Awareness supplies a TAG Order, **AP HRL/BS Attack (+1B)** threatens grouped/heavy targets, and Kludger can **repair its Remote Presence/3 STR** and do objectives. The TAG's included **ZetBot Ancillary specialist** scores without exposing the expensive chassis. | Kludger is a valid Wreckers-team member; other Wildcards obey the chart. Kludger must have an actual repair route. Wrecker is BS13 and does not bring a visor/Mimetism, so don't make it fight every FtF ARO. |
| **Double Wrecker Duo:** two 51pt HRLs (102pt/3SWC), or mixed weapon options | A thematic **two-attack-vector**, two-**Tactical Awareness** shell: an AP heavy rocket threat on each body, mutually supportive reactive deterrence, plus durable scoring Ancillaries. TA/Robert suggest it can be genuinely dangerous. | 102pts before support; if both are exposed to a superior linked MSV gun/hacking network, a third of the army is endangered. Lower points flexibility and fewer support pieces make it a deliberate skew, not default list-building. |
| **Small Silverstars / reactive link:** Hellblazer + Waverider + Vidoc/PSI/StormBot FTO | Can split defense across the table; Rocket ARO, Pitcher coverage and specialist order income without requiring a full 5-model HI Core. | StormBot Wildcard is **options 2/3 only**; option 1 HRL(+1B) **cannot** join. Vidoc Wildcard **options 1/2/3**, Jamie Rover **options 1/3 and Silverstars-only**, Sonya **Silverstars-only**; Hippolyta **Silverstars/Mobility only**. |
| **Solo Silverstar Prime with separate small link** | **53pt BS14, ARM5/BTS9, MSV1, HMG, Tactical Awareness** is more reliable at *winning* FtF rolls than Wrecker; it clears sightlines for cheaper linked hackers/specialists. Can take the Lt variant when defense/CoC makes sense. | **Prime has NO Fireteam access in current Torchlight**, notwithstanding its name and **older N4 discussions**. Do not rely on linked extra Burst/BS or transplant a pre-N5 build. |

**Commander option comparison:** Raveneye Lt (+1 Order) with Ment CoC turns **Strider NCO** and/or **Vidoc NCO** into strong specialists/shooters; Jamie Lt (+1 Order) costs 49 and can spend Orders aggressively but puts 49pts and command in harm's way; Prime Lt 53 is a hard gunfighter **without Lt (+1 Order)**; Sonya Lt 28 offers **+1 SWC, not an extra Lt Order**. Select based on which Lt Orders your list can actually exploit; NCO stops being useful if its recipient dies/gets disabled or its command source fails.

### Standalone mission and support pieces

| Unit | Why it works | Limit / competition |
|---|---|---|
| **Moonraker** — 14 / 15 Minelayer | **Forward Deployment (+20), one-use Camo, Mimetism, Shock Mine and Adhesive Launcher Rifle** put a mine/possible-glue fork on an approach before spending active Orders. Opponents must discover, avoid or risk a cheap Regular model; two Minelayers anchor much of the faction's defensive economy. | BS11/WIP12/1 STR; usually a **predeployed trade/denial piece**, not a dependable gunfighter. At 15pts/0.5SWC, take it only when mine placement actually covers a contested route; cannot borrow a Vanilla-only Camo alternative. |
| **Strider** — FO 29; specialist 27; Minelayer 28 | **FD(+20), Camo, NWI, Mimetism(-3), NCO, WIP13** create a durable objective/marker-state operator that can spend extra Lt Orders. FO light shotgun(+1B) trades brutally at close range; 28pt Repeater/Minelayer or Shock Mine options make a Camo fork. | BS12 and (for Red Fury) 34pt/1SWC limit value as long-range attacker. The 2024 event winner spent **Lt Orders on a Strider after the Prime had opened the table**; the June 2026 panel calls some Strider profiles too expensive for a BS12 NWI specialist. |
| **Waverider** — HD 22/23, KHD 20 | BTS6/Mimetism(-3)/Stealth, **Pitcher**, **Oblivion(+1B)** or **Trinity(SR-1)** plus link access let it establish a network or suppress opposing hackers before TAG/HI advances. Often combine at least one KHD and one standard Hacking Device somewhere in the army. | WIP13 is adequate, not overwhelming; a vulnerable Pitcher line can cost several Orders; **Moonraker is not a Repeater**. Linked hacking still obeys normal Fireteam/action restrictions. |
| **Hippolyta** — 37 | **Mimetism(-6), smoke, BS13 Breaker rifle, melee ability, 2 Wounds and Super-Jump** create a non-hackable assault vector/visibility screen that hard-target gunfighters cannot provide. Mobility with Kludger and/or Nimrod is a serious alternative to a second TAG/Prime. | Limited Cover and Impetuous exposure; 37pts is a lot for a short-range attacker. **Current N5.3 equipment says Smoke Grenades**, not the historical **Eclipse Grenades** repeatedly mentioned in N4 2024 podcast transcripts. Do not import old smoke semantics. |
| **Kludger** — 23 Doctor/Engineer | **WIP14, Mimetism(-3), Super-Jump**, D-Charges/Panzerfaust/adhesive; its engineer-with-Disco-Baller can *repair Wrecker/Prime-support network* and counter sightlines, while the Doctor can restore HI. Unusually eligible in **all three** team families. | AVA3, but not three automatic purchases: competing specialist coverage and expensive linkmates strain Orders. A 23pt Kludger needs actual work and a safe route to do it. |
| **Hellblazer** — 18/19 | Regular/Impetuous **2-Wound** HI with CC22 MA2, EXP CC weapon and Flammenspeer/Blitzen/Akrylat. Cheapest qualifying **Silverstars source**, giving efficient aggression and a cheap Team slot. | Limited Cover, exposed Impetuous rush and hacking susceptibility. Treat as a close-range trader/anchor, not as a premium gun on a tower. |
| **Nightshade** — 31–34 | Hidden Deployment, FD, Mimetism(-6), KHD/Minelayer, Super-Jump and E/M/PARA CC can trap a key enemy or fill specialist pressure missing from a gun-led plan. | One-Wound, 30+pt ambush: brittle when opponent sweeps templates/Sensor and can lose to cheap close defenders; should not substitute for cheap Moonraker screen. |
| **Nimrod** — 27–29 | MSV2 + Mimetism(-3) + Super-Jump, E/M Carbine/AP Marksman or Thunderbolt(+1B); with **Hippolyta smoke** it contests otherwise severe visual modifiers and can disable rather than only wound a TAG. | No durable second wound; 28–29pt gun is not as high-damage as Prime/Wrecker. **Hidden Deployment option 1** also counts as a legal Mobility option in the current chart, but deploying hidden may complicate forming/using the link. |
| **Yellowjacket** — 25/29 | Combat Jump/Parachutist + Mimetism(-3), NWI, 1-Wound HI; **25pt Specialist SMG/D-Charges** can threaten a poorly screened objective, kill isolated targets or achieve a classified. | Strong dissent from TA 2025 and Robert/Jordan 2026: **BS12 and no serious long-range gun**, costing close to reliable midfield choices, makes it a poor general-purpose attack drop. Use a defined landing/mission plan, not as an automatic alpha-striker. |
| **Jamie Handler vs Rover** — 49/52, 47/49/53 | Plasma+Akrylat pressure, NCO or Lt(+1 Order), BTS9; **Rover FTO 47/49** can join Silverstars, while **Handler** FD(+20)/Decoy can threaten midfield as a solo. Tactical Awareness likes high-BTS NCO Rover/command aggression; the 2024 winner found Jamie too expensive/large for his safer Prime-Hippolyta plan. | **Mutually exclusive alternate versions.** Rover option 2 parachutist is **not FTO**; Handler cannot Fireteam. Taking one competes with Prime/Wrecker for a major ~50pt role. |
| **Sonya / Kyra / Sāchā / Beasthunter** | **Sonya** 28pt Albedo and NCO/Emitter can ambush visor pieces, is a **Silverstars-only Wildcard**; **Kyra** 45pt TA/Regeneration, Paramedic and WildParrot offers a self-driven close mission push; **Sāchā** 6pt Irregular FD specialist helps certain missions; **Beasthunter** 9pt expendable DZ deterrent or 15pt Camo attack/minelayer threat. | Sonya's Albedo is situational and can be an expensive 1-Wound niche; Kyra costs premium points and **FTO name grants no Fireteam**; Sāchā's Irregular Order is not free Regular pool fuel; Beasthunter's FTO also has **no chart access**. The 2026 review dislikes paying for luxury options over another reliable gun. |
| **Ment / Raveneye / Vidoc / Jackboot / PSI-Cop** | **Ment CoC + Number 2** cheaply insures bold command; **Raveneye** mine+FO and Lt(+1 Order) are mission/Order infrastructure; **Vidoc** 26pt MSV1 MULTI Sniper/NCO provides linked range; **Jackboot** 21pt Paramedic, 26pt FO Thunderbolt or 29pt NCO HMG gives independent tech; **PSI-Cop** can bring MSV1, a Disco Baller KHD or another legal Wildcard specialist. | All compete for points/limited Wildcard slots. **Torchlight has no Jackboot Engineer** (only profiles 4/5/6); avoid importing the superior Vanilla Engineer loadout. Vidoc options 1/2/3 only are Wildcard. |

### TAG / Vehicle / REM quick decisions — Torchlight **only**

**Roster boundary:** **Wrecker** is the Torchlight TAG (AVA2, may Duo), **Firebat is a Vehicle (VH), not TAG or REM**, and the rest below are remotes or peripherals. **Zeta, RoadBot, Sekudroid and other O-12 machines available in Vanilla and/or Starmada are NOT in the current Torchlight roster**. Vanilla O-12 and Starmada opinions inform *performance*, not these sectorials' availability or Fireteams.

| Platform, exact N5.3 cost | What the platform does and *why* | Role / trade |
|---|---|---|
| **Wrecker TAG — HRL 51/1.5, Spitfire 55/1.5, HMG 57/1.5** | **BS13, ARM6/BTS9/STR3, Tactical Awareness, Remote Presence**, AP on shots and included **ZetBot Ancillary specialist**. **HRL BS Attack(+1B)** makes 51pt profile a cost-efficient burst/template threat to clustered enemies/armor; 55/57 trade for more traditional solo gun range/burst. | Wrecker is best at **punishing a successful hit**, not necessarily winning every opposing roll; lacks Prime's BS14/MSV1. Repair with Kludger/Yudbot/Lambda; avoid unfavorable Mimetism/cover duels. **A-tier opinion** from Loss of Lieutenant TAG panel; Robert Shepherd prefers Prime *first*, then Wrecker for damage/second gun. |
| **Firebat Attack Wing VH — 35–36/0** | **S7 Aerial, very fast movement, Super-Jump, Mimetism(-6), NCO, Tech-Recovery**, 0 SWC and AP SMG/Thunderbolt/rocket vs MULTI Rifle/Heavy Riotstopper/Akrylat/Blitzen loadouts. Unique high-angle close/flank attack and Lt-Order use. | **No Cover, ARM4, STR2**; may be exposed despite -6 Mimetism. Robert Shepherd (2025), Counterintelligence and Shepherd/Jordan (2026) disagree on its exact niche but trend **skeptical for 35–36pts** compared with cheaper flyer alternatives. Do not plan to use it like a normal covering unit or objective sitter. |
| **StormBot REM — 31/1.5 HRL(+1B) non-FTO; 29/1.5 HRL+E/M Mine FTO; 33/0 Combi(+1B) FTO** | **ARM3/BTS6/STR2, BS13, Repeater, Remote Presence**. Rocket mode can support a backfield overwatch plan; E/M Mine creates local denial; **FTO 2/3** can join Silverstars/Mobility/Wreckers and add a tough repeater/TinBot-adjacent threat. | Contrast: the non-FTO 31pt extra-burst rocket is **not linkable**, and the linkable 29pt rocket gives up that inherent +1B. TA 2025 didn't select one in sample lists; N4 TA liked boosted StormBot defense, but its buffs/Fireteams are historical. At 29–33pts, only buy with credible target lanes and repeater coverage. |
| **Moonraker REM — 14/0, 15/0.5 Minelayer (AVA2)** | **Camo(1 Use), FD(+20), Mimetism(-3), Heavy Shotgun, Adhesive Launcher Rifle, Shock Mine**; excellent deploy-first protection for costly HI/TAG and midfield mission positions. | Fragile BS11/WIP12/STR1; not a Repeater, not a linked REM. Threatens *time* as well as casualties; take two for board-control density when table geometry permits. |
| **Oko Copperbot REM — 15/0 or 18/0 Tactical Awareness (AVA2)** | **Sensor, FO, Repeater, Climbing Plus, Triangulated Fire**: inexpensive independent specialist, detection and hacking area projection. **TA for +3pts** when Oko will spend Orders uncovering markers/pressing buttons. | BS11/ARM0 and cannot shoot through serious defense; **unlike Starmada, no RoadBot/Oko Road Duo**. This is a support/mission unit, not a gunfighter. |
| **Peeler Copperbot REM — Thunderbolt(+1B) 19/0 or HMG 24/1 (AVA1)** | **Total Reaction, 360° Visor, Climbing Plus**; cheap static ARO, especially 0SWC Thunderbolt when HRLs and Prime already consume SWC. Forces enemy to allocate an Order to clear a lane. | ARM0/STR1, BS11; expect dedicated attackers/smoke to beat it. Compare the cheaper 19pt Thunderbolt to FuzzBot TR rather than assuming 24pt HMG is always required. |
| **Kyttä Copperbot REM — 7/0 (AVA1)** | 15-15 Move, **Flash Pulse, Mimetism(-3), Repeater** for a cheap Regular Order and network/flash nuisance. | BS8/STR1, its job is to enable Waveriders or tax enemy movement, not to actively remove ARO. |
| **FuzzBot REM — 8/0 Repeater/Baggage; 14/0.5 EVO; 17/0 TR Combi (AVA2)** | 8pt **Baggage** supplies cheap Regular Order, repairs ammo economy by reloading compatible deployables/Pitchers and adds a Repeater. 14pt EVO is for an actual remote/hacking support plan; 17pt TR Combi adds local defense. | EVO/Hacking requires a specific plan. **17pt TR Combi vs 19pt Peeler TR Thunderbolt**: Peeler usually wins the *longer-ranged* ARO question; FuzzBot wins only if Baggage/Repeater or shorter-range network protection is more relevant. |
| **Millicent Copperbot REM — 16/1.5 (AVA1)** | Guided Missile Launcher punishes **Targeted** opponents produced through Waverider/Kappa/PSI hacking, adding a secondary lane when direct shooting is costly. | 16pt + 1.5SWC + Spotlight/Pitcher/Orders is a **system**, not a free answer. Robert Shepherd (2025) included it only because he had spare resources; the WIP12 **2024 tournament winner specifically omitted** it because a Prime, Vidoc, and midfield scorers solved his problems more cheaply. |
| **Yudbot servant REM — 3/0 (AVA2)** | Extends **Lambda/Kludger/other compatible Doctor-Engineer support** across the table where permitted; keeps repair/rescue specialists behind the front and lets TAG/HI investment recover. | **Peripheral (Servant), not an independent Order**. Do not confuse it with the Wrecker's included **ZetBot Ancillary** (a separate scoring tool tied to the TAG). |

**Model-independent machine packages:**
- **Ranged attack + scoring:** **Prime (53)** *or* **Wrecker HRL (51)** + two Moonrakers + Strider NCO + cheap backup scorer. Select Prime when facing strong Mimetism/visors/ARO FtF; Wrecker when AP template and the ZetBot's specialist reach solve the mission.
- **TAG rescue:** Wrecker + Kludger Engineer **Wreckers Duo** + 8pt FuzzBot + Yudbot/Lambda where support-legal. Don't spend a second full repair suite automatically; test whether the TAG's route actually benefits from one.
- **Camo/hacking net:** two Moonrakers / one Strider Minelayer or repeater / Kyttä / Oko + Waverider HD/KHD Pitcher + possibly StormBot Repeater and a FuzzBot Baggage supply. **Moonrakers aren't repeaters**; a Camo screen and a hacking screen complement rather than duplicate each other.
- **Defensive cheap screen:** 12pt Raveneye E/M Mine + 14–15pt Moonraker(s) + 19pt Peeler and a legal Silverstars cheap anchor. Opponent cannot remove one firing lane without committing to mines, Cyber/EM control and possible glue.
- **Airborne disruption:** Yellowjacket specialist after the main shooter opens a landing lane; prefer a clearly identified classified/backfield objective over attempting to shoot down long-range defenses with its SMG.

### Contested judgments — *both* views and decisive circumstances

| Question | Optimistic assessment — why | Skeptical assessment — why | Practical test |
|---|---|---|---|
| **Torchlight strong or disappointing?** | [Tactical Awareness S3 Ep28](https://www.youtube.com/watch?v=86n0kQ5xBgY) shows lists mixing Wrecker, Moonrakers, Waverider hacking, Super-Jump mobility and strong command tools; the 2024 [WIP12 CyberBaltic-winning player](https://open.spotify.com/episode/72TMCTByFqldzNPtvz8gta) describes how Camo mine screens + Prime/Hippolyta/Strider sequenced attacks and scoring. | [Robert Shepherd 2025](https://www.youtube.com/watch?v=PZKCQAupCMs) and [Shepherd/Jordan 2026](https://www.youtube.com/watch?v=1dW3i9dpI34) see inflated costs, no Prime Fireteam, too few cheap Regular Orders, mediocre Silverstar Rovers and weak Yellowjacket guns; the sum is less than its paper stats. | Count Orders after adding the expensive team, and test objective backup after losing Prime or Wrecker. 2024 successes were under **N4**, not current points/rules. |
| **Silverstar Rovers vs cheap Hellblazer source** | Rovers **all specialists**, BTS6/2W and TA HMG/ML can form a durable linked main plan, supply TinBot firewall and score even after fighting. Early N4 players leaned heavily on these teams. | Shepherd suggests **0 Rovers in many N5 lists**: too much money for built-in specialist/dodge/jump/rio stopper when a Hellblazer plus a Waverider/Vidoc achieves the key roles. | Need the 31pt TA missile or a specific resilient objective holder? Rover. Need just a Fireteam source? Hellblazer. |
| **Prime or Wrecker as first gun?** | Wrecker HRL **51pts** with TA, AP blast, BTS9/STR3, ZetBot is disproportionately punishing on a connected hit; [Loss of Lieutenant TAG panel](https://www.youtube.com/watch?v=dZo_gQWQYSY) rates it highly, and TA explores **dual HRLs**. | Shepherd explicitly prefers **Prime 53** for first attacker: BS14/MSV1 wins FtF against Mimetism and other AROs more reliably; Wrecker BS13 can fail while taking hits and is poor against favorable enemy range/mim penalties. | Choose Prime for **clearing ARO**; Wrecker for **AP template, durability and scoring**. Two together is viable but sacrifices list economy. |
| **StormBot strong ARO or expensive unused REM?** | 2STR, ARM3/BTS6, Repeater and rocket + E/M mines make a resilient remote-gate; **29pt FTO HRL** can support Fireteam Defense. N4 Tactical Awareness praised combinations with buffs. | N5 TA 2025 largely **left it out**: high cost, mediocre defense compared with 19pt Peeler + dispersed mines; can't simultaneously choose non-FTO +1B rocket and link it. | Pay for FTO when its **specific linked rocket/network position** is better than Peeler + cheap Order. |
| **Firebat valuable or poor value?** | 0SWC, NCO, S7 aerial mobility, Mimetism(-6) and high-angle rockets/adhesive allow an unusual flanking route and targeted victim. | Robert 2025 and June 2026 call its **35–36pts/No Cover** poor opportunity cost; Counterintelligence hosts also place it low because good enemies hunt an exposed huge S7 silhouette. | Define a first-turn attack route, retreat space, and Lt Order recipient plan before buying it. |
| **Strider superb midfield or bloated?** | WIP12 tournament winner 2024 specifically used **Strider NCO** to spend Lt Orders **after** Prime/Hippolyta removed enemies, so a small second group could still score. Camo/FD/NWI/FO/shotgun is genuinely multifunctional. | 2026 Shepherd/Jordan say BS12 27–34pt NWI troops are expensive relative to other factions' midfield and cannot independently crack ARO defenses. | Cost-effective **button/control** piece, not an independent primary gun. Avoid 34pt Red Fury absent clear target lanes. |
| **Yellowjacket drop worth 25–29?** | Camouflage is absent but Combat Jump/Parachutist + Mimetism(-3), NWI, D-Charges and specialist access force backfield screening and can score from unexpected angles. | TA 2025 and Shepherd/Jordan 2026 find **BS12 short-range-only guns** too weak to buy as serious AD attack investment. | Pick when insertion creates a mission-winning interaction, not when you need your second long gun. |
| **Millicent guided plan or unnecessary tax?** | Waverider Pitcher, repeaters, Standard HD Spotlight and 16pt launcher can crack a dug-in unit without exposing Prime. | WIP12's 2024 winner says a **good Prime/Hippolyta attack + Strider** is preferable to 16pt/1.5SWC guided expenditure; Shepherd says he takes it as spare-points luxury, not faction identity. | Take when reliable Targeted/setup and spare SWC already exist; otherwise buy a second mission threat. |
| **Jamie worth his cost?** | Tactical Awareness 2025 argues a **BTS9 NCO/Plasma Rifle** in a legal Rover FTO Silverstars role or as a solo Lt can turn otherwise spare Lt Orders into a catastrophic assault; specialist/CC support from allies. | CyberBaltic 2024 winner dislikes a **~50pt large silhouette** and extra required activations; Shepherd 2025 calls him a fun expensive luxury in a faction already short on economy. | Choose based on a real Plasma/NCO path and Lt protection. Never field Handler and Rover simultaneously or assume all Rover profiles are linkable. |

### Best video/podcast source trail (MCP verification)

**N5 sources (prioritize these for opinions; confirm current N5.3 profiles in this file):**

| Source | MCP evidence, focus |
|---|---|
| [**Tactical Awareness S3 Ep28 — Torchlight Brigade** (YouTube)](https://www.youtube.com/watch?v=86n0kQ5xBgY), **2025-07-21** | Full **YouTube MCP transcript checked**. Closest all-roster N5 dedicated discussion: multiple example lists, Silverstar Prime no-link correction, Moonrakers, Wrecker HRL Duo/Ancillary, Waveriders, Jamie, Striders, StormBot/Yellowjacket/Firebat disagreements. |
| [**Robert Shepherd — N5 Torchlight Faction Focus**](https://www.youtube.com/watch?v=PZKCQAupCMs), **2025-06-14** | Full **YouTube MCP transcript checked**. Best contrasting *list-building* critique: Rover trap, efficient Hellblazer+Waverider+Vidoc/PSI links, Hippolyta/Kludger/Nimrod, affordable Moonrakers, Prime vs Wrecker, hesitant Vehicle judgment. |
| [**Robert Shepherd + Jordan — June 2026 N5 all-factions comparative review**](https://www.youtube.com/watch?v=1dW3i9dpI34), **2026-06** | Full **YouTube MCP transcript checked**. Latest sampled opinion on the **post-N5 balance**: disappointed by costly Rovers/Striders, unlinked Prime, Yellowjacket and over-fair profiles; Moonrakers stay a positive. |
| [**Loss of Lieutenant Ep142 — N5 TAG tier list**](https://www.youtube.com/watch?v=dZo_gQWQYSY) · [Spotify](https://open.spotify.com/episode/1h5CJfZC5zBPxdg66o7xIN), **2025-04** | Full **YouTube MCP transcript checked**: **Wrecker A-tier** pro case, 51pt HRL/Tactical Awareness/BTS9/Ancillary, when to use Prime as a secondary gun and how to budget a TAG. Also reviews **Zeta**, which is not available in Torchlight. |
| [**Counterintelligence — O-12 role-by-role N5**](https://www.youtube.com/watch?v=Vrn9U320eSs) · [Tactical Awareness S3 Ep29 — Vanilla O-12](https://www.youtube.com/watch?v=aGCxiKFBvVY) | Full **YouTube MCP transcripts checked**: Wrecker/Firebat/Peeler/Oko/REM tradeoffs plus cross-faction support. **Vanilla AVA, Gamma/Omega/Zeta/Fireteam choices are not Torchlight legality**. |
| [**MiniWarGaming — Torchlight vs Steel Phalanx (N5 battle report)**](https://www.youtube.com/watch?v=Tn6_u2OH4Tw), **2025** | Full **YouTube MCP transcript checked**: example of a played table/mission and turn sequencing; a single game is not proof of broad win rates. |
| [**Infinity the Dante + Loss of Lieutenant guest — O-12 N5 initial reaction**](https://www.youtube.com/watch?v=48clEYqxRsA), **2024 N5 launch** | Full **YouTube MCP transcript checked**: Wrecker and Firebat early judgments and shared O-12 unit tradeoffs. Note focus is **Vanilla**, not current Torchlight. |

**Historical N4 podcasts (transcripts checked, with strict edition caveat):**

| Source | Transferable insight; what must *not* be transplanted |
|---|---|
| [**WIP12 Ep161 — 2024 CyberBaltic satellite champion on Torchlight**](https://open.spotify.com/episode/72TMCTByFqldzNPtvz8gta), **2024-06** | Full **Podcast MCP transcript checked**. **Most useful tournament case study**: Prime/Hippolyta/Vidoc open a lane; Strider NCO spends reserve Lt Orders to score; Moonraker/Strider/Beasthunter mine layers protect expensive pieces. He omits Millicent and Jamie for mission economy. *N4 roster/Prime link/smoke information is obsolete*. |
| [**WIP12 Ep149 — Torchlight Brigade with Dr D**](https://open.spotify.com/episode/29VGwPXG8hoCcnvrK9ebCV), **2024-04** | Full **Podcast MCP transcript checked**. Early strength of budget Wrecker TAG, dispersed Camo with Moonrakers, Waverider/Wildcard construction and reservations about some Sonya/Silverstar investments. **Early release N4**; roster, costs, FTO and Fireteams differ. |
| [**Tactical Awareness S2 Ep16 — Torchlight Brigade (ITS15)**](https://open.spotify.com/episode/3ctvxknSzkDi3RoTll8pFy), **2024-03** | Full **Podcast MCP transcript checked**. N4 exploratory discussion of Prime, StormBot buffs, Moonraker mines and alpha-defense layering; useful strategic precedent but **Prime was discussed as linkable and Hippolyta had different historical smoke**. Never treat as N5.3. |

**Found but not transcript-backed:** [*Spotlight #9 — Torchlight Brigade First Impressions*](https://open.spotify.com/episode/55zHRE0pZePskqp6DOl2Im) (2024-03) was located via Podcast MCP, but its transcript request returned **no transcript**; no detailed tactical claims here rely on it.

**Evidence priority:** this repository's **Army 7.26246.159 / N5.3** profiles and Fireteam chart > post-N5 tactics reconciled against those profiles > early N5 commentary > N4 anecdotes. In particular, **Prime cannot link**, **Hippolyta currently has Smoke Grenades**, Torchlight has **1 Core + 1 Haris**, and a podcast example with two simultaneous Haris teams or former mixed Fireteams is **not** current-legal just because the hosts proposed it.

## Validation notes

- Verified against Army snapshot **7.26246.159**, source blob `9ea237fbfcfb5ea46a9466b35593f16fe9f4c75d`, mirrored in backup commit `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` dated **2026-09-03**.
- Fireteam chart source limits: `CORE: 1`, `HARIS: 1`, `DUO: 256`.
- Canonical Fireteam families found in the source: **Silverstars**, **Mobility**, **Wreckers**, plus Wildcards.
- FTO labels were not treated as permissions. Chart context was applied explicitly to StormBots, Vidocq, Jamie Rover, Beasthunters, Kyra Sharma, and Nimrods.
- The canonical **Fireteams** section takes precedence over the reverse access index if an inconsistency is ever introduced during later edits.

## Command-unit apex/value cross-reference (2026-10-23)

**Raveneye LT(+1) 17/0** is a premier low-cost Holomask, FO, Minelayer two-Order commander when **Strider/Vidoc or another legal NCO** can spend those Orders; **Raveneye CoC 18/0** is a different legal profile that supplies hidden succession. **Jamie Arantes LT(+1) 49/0** is for actually spending command Orders on the fighter, but adds substantial risk. **Ment CoC** is another backup option. Keep successor away from active LT attack and do not count personal Tactical Awareness as global Orders.

See [cross-game Lieutenant, Chain of Command and Order-package tiers](../../notes/list-building/command-units-apex-and-value.md). **Use this roster/Fireteam chart above for exact legality.**

## TAG tactical cross-reference (2026-10-23)

**Wrecker** is unusually high **value**: **51-point HRL+1B** punishes bunching and hard targets, while Spitfire/HMG versions switch to more conventional direct attacks. TacAware helps fund aggression without reducing your specialists. It is not an HRMC/Zeta replacement—use TLB's other threats to open the lane and a Wrecker to exploit and hold it. In the 2025 TAG transcript, hosts highlight the lethality of the HRL's attack modes.

For the two-tier **apex/points-value** comparison, TAG counterplay, matchup matrix and direct transcript sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Treat current profiles, points/SWC and canonical Fireteam data above as authoritative.

## Vehicle (VH) tactical cross-reference (2026-10-23)

**Firebat AVA1:** **36/0 AP SMG+Thunderbolt+LRL** adds 0-SWC short-to-long coverage, or **35/0 MULTI Rifle/Riotstopper/Akrylat/Blitzen** provides nonlethal attacks. **NCO** makes an available Raveneye LT(+1 Order) valuable for aerial repositioning or defensive Suppression; Mimetism(-6)/+1 Special Die make active engagements reliable against weak units. It is **not** Wrecker TAG, and at BS13 cannot replace the primary heavy-gun/ground-scoring architecture. Older Shepherd analysis rates its value and Suppression option higher than pure raw power.

See [VH apex/value tier list and matchup guide](../../notes/list-building/vehicles-vh.md). **Current profiles, AVA and canonical Fireteam chart above remain authoritative.**

## Hacker and KHD tactical cross-reference (2026-10-23)

**Waverider HD + Oblivion(+1B) 22/0.5 or KHD 20/0**, both with Pitcher, combines **15–5 MOV, Mimetism(-3), BTS6** and legal **Silverstars** access: the HD attacks HI/TAG, the KHD counters hacker networks. **Kappa HD13/0.5** provides a very cheap second control specialist; **Ment FTO HD20/0.5** and **PSI-Cop HD24/0.5 vs KHD23/0** provide team/mission alternatives. **Nightshade KHD34/0** pays for Hidden Deployment and close-range physical kill potential rather than pure hacking power. **Why:** a Waverider can project an accurate Pitcher while moving with a relevant team, but **TinBot/team legality** must follow the canonical Silverstars row. Upgrade **Oblivion(+1B)** matters in active anti-HI/TAG turns, unlike a plain KHD.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

The N5.3 [cheerleader/order-generator apex and value guide](../../notes/list-building/cheerleaders-and-order-generators.md) contrasts Orders-per-point, passive utility, matchup dependence, and opposing transcript opinions. **Use this roster for legal AVA, exact profile costs, Training and Fireteam restrictions.**

- 7pt Kyttä — cheap mobile Flash/Repeater/Mimetism Regular Order; check local AVA and deployment safety.
- 8pt FuzzBot — Baggage/Repeater plus Regular Order, excellent if the S4 footprint can be concealed.
- 12pt Kappa — S2 baseline Regular Order, with modest Specialist/Commlink upgrades; compare their actual mission utility against cheaper REMs.
- Waverider — fast forward network/multi-role piece rather than pure passive Order filler; invest for actual hacking and scoring payoff.
- Warcor — a 3pt Irregular Flash ARO speedbump, not a transferable pool Order without actual conversion.

**Decision:** first buy enough protected *transferable* Regular Orders for the actual Combat Group attacker/scoring plan, then pay for genuine role compression. Irregular/Impetuous, LT, Tactical Awareness and Peripheral bodies are different resources. Account for a packed S3/S4 deployment zone and mandatory Fireteam members.


## ARO apex/value cross-reference (2026-10-23)

[Best ARO units across N5.3 — absolute apex vs points-value](../../notes/list-building/aro-units-apex-and-value.md) compares hidden reactive fire, TR/Neurocinetics, Flash/DTW/expendable defenders and why competing creators disagree. The **roster here** is authoritative for actual costs, Training, AVA and Fireteam construction.

- **StormBot HRL** — two-structure mobile shooter with durable reactive potential; FTO/non-FTO costs and legal link matter
- **FuzzBot TR** — 17pt/0SWC Regular cheap Repeater/Combi deterrent; compare stronger but dearer StormBot
- **Kyttä Flashbot** — 7pt Repeater/Flash secondary ARO and cheap Order; insufficient alone against assault gun
- **Warcor 3pt Flash** — disposable Irregular Stun/Orders tax, not a generic Regular cheerleader
- **Total Reaction support** — use recoverable remote for routine lanes, rather than expose primary active gun

**Best circumstance:** long exposed lanes justify a real sniper/missile/linked gun; dense tables, DZ landings and mission rooms favor E/M, mine, Shotgun, Riotstopper and hidden traps. Cover the destination/approach, layer serial threats rather than two pie-sliceable visible guns, and preserve scoring units for the active turn.
