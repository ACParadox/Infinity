---
schema_version: 1
reference_type: sectorial
status: current
sectorial_id: 902
sectorial_slug: druze
sectorial_name: Druze Bayram Security
parent_faction: Non-Aligned Armies
rules_baseline: N5.3
army_source_version: "7.26246.159"
army_data_changed_on: 2026-09-03
infinitydb_commit: "4e2662be3f43387fbae42b3790a711b3e98570c4"
verified_on: 2026-10-16
coverage: "Complete standard Druze Bayram Security roster, standard loadouts/profile states and peripherals, canonical Fireteam chart, exact FTO/counts-as restrictions, reverse Fireteam access, optional-mode hooks, source alias reconciliation, and Reinforcements boundary. Generic Soldier of Fortune catalog entries are excluded."
---

# Druze Bayram Security — N5.3 sectorial reference

## Overview and provenance

This file is the repository reference for **Druze Bayram Security** (Army sectorial ID `902`), a sectorial of the **Non-Aligned Armies / NA2** (parent Army ID `901`). It is intended to be sufficient for ordinary roster, AVA, points/SWC, profile, dependency, and Fireteam-legality questions without reopening Army.

Primary data source:

- Corvus Belli Army data snapshot mirrored by `massayoshi/infinity-army-backup`.
- Pinned source commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b` (`army: N5.3 + ITS18`).
- Army dataset: `n5/druze/7.26246.159.json`.
- Source blob: `311c3b0d595ee220d4046b983b8dfb65dceb3b2c`.
- Army version: **7.26246.159**.
- Sectorial ID: **902**.
- Parent Non-Aligned Armies ID: **901**.
- Reinforcements list ID exposed by the dataset: **999**.
- Cross-check/reference model commit: InfinityDB `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Rules baseline: **N5.3 + N5 FAQ v0.1**.

Coverage policy:

- The **35 standard logical roster records** whose faction availability includes Druze Bayram Security are included below.
- Generic Soldier-of-Fortune catalog records present in the aggregate payload with `factions: []` are excluded.
- **Rumbler Spec-Ops** and **NA2 Team-Ops** are optional-mode hooks, not ordinary matched-play roster entries.
- Reinforcements (`army_id: 999`) remain distinct from the normal Druze roster and Fireteam chart.
- Composite states and Peripherals stay under their parent logical unit rather than being counted as separate roster entries.
- Fireteam legality comes from the canonical chart below, not from an `FTO` label alone.
- Where Army marks multiple entries `required: true`, this file follows repository convention and treats those entries as a **required source-choice set** unless the chart specifies otherwise.
- The Fireteam chart names Denma Connolly with the source slug `denma-connolly-caledonian-zellenkrieger`; the roster record uses `denma-connolly`. Both resolve unambiguously to unit ID `1749`, so this file treats them as the same logical unit.

## Sectorial summary

| Field | Value |
|---|---|
| Sectorial | Druze Bayram Security |
| Parent faction | Non-Aligned Armies / NA2 |
| Army ID | 902 |
| Rules baseline | N5.3 + N5 FAQ v0.1 |
| Army source | 7.26246.159 |
| Standard logical roster records | 35 |
| Optional-mode records | 2 |
| Reinforcement roster | yes — Army ID 999 |
| Fireteam chart | yes |

## Fireteam limits and interpretation

| Constraint | Value / wording |
|---|---|
| Core | up to 1 Core |
| Haris | up to 1 Haris |
| Duo | effectively unlimited (`256` in Army source) |
| Fireteam families | Druze Bayram Security; Mechanized; Fast Attack |
| Wildcards | Authorized Bounty Hunters; Diggers; Arslan; Aïda Swanson FTO; Valerya Gromoz; Wolfgang Amadeus Wolff; Clipper Dronbot FTO |
| Main/Reinforcement mixing | Keep normal Druze and Reinforcement charts distinct |

Important profile-level restrictions and equivalences:

- **Zellenkrieger access in Druze Bayram Security Fireteams is FTO-only:** option `3` only. Options `1` and `2` are not Fireteam legal.
- **Aïda Swanson Wildcard access is FTO-only:** option `2` only. She counts as **Druze** in the Fireteam chart. Option `1` is not a Wildcard.
- **Clipper Dronbot Wildcard access is FTO-only:** option `5` only. The Guided Missile Launcher option `1` is not Fireteam legal.
- **Brawlers** count as **Druze** in Druze Bayram Security Fireteams.
- **Táowù** counts as **Druze** in Druze Bayram Security Fireteams.
- **Diggers** and **Arslan** are Wildcards that count as **Druze**.
- **Fiddler option 1 is named `Fiddler FTO`, but Fiddler has no row in the Druze Fireteam chart.** The FTO label alone does not grant Fireteam access.
- The Druze Bayram Security family marks both Druze and Brawlers `required: true`. Under repository required-choice semantics, at least one member must come from that two-row source set; it does not require one of each.
- The Mechanized family marks both Anaconda and Scarface `required: true`. Treat them as a required source-choice set: at least one of those source rows must be present.

## Standard roster index

| Unit ID | Unit | AVA | Type | Classification | Regularity | Fireteam access / notes |
|---:|---|---:|---|---|---|---|
| 16 | Pathfinder Dronbots | 3 | REM | Support Troops | Regular | — |
| 18 | Clipper Dronbots | 1 | REM | Support Troops | Regular | Wildcard, **FTO option 5 only** |
| 333 | Nasmat Remotes | 2 | REM | Support Troops | Peripheral | Servant |
| 310 | Hunzakuts | 2 | SK | Spec. Trained Troops | Irregular | — |
| 36 | Peacemaker Armbots | 1 | REM | Support Troops | Regular | Includes AuxBot variants on selected options |
| 668 | Saito Tōgan | 1 | SK | Character | Regular | — |
| 464 | Valerya Gromoz | 1 | LI | Character | Regular | Wildcard |
| 680 | Armand “Le Muet” | 1 | MI | Character | Regular | Transmutation profile states |
| 986 | Security Chief Arslan | 1 | MI | Character | Regular | Wildcard; counts as Druze |
| 1502 | Kunai Solutions Ninjas | 2 | SK | Mercenary Troops | Regular | — |
| 378 | Yuan Yuan | 4 | WB | Mercenary Troops | Irregular, Impetuous | — |
| 1333 | Monstruckers | 2 | LI | Mercenary Troops | Irregular | Druze Bayram Security |
| 1747 | Zellenkrieger | 1 | WB | Support Troops | Irregular, Impetuous | Druze Bayram Security, **option 3 FTO only** |
| 987 | Brawlers, Mercenary Enforcers | 4 | MI | Spec. Trained Troops | Regular | Druze Bayram Security; Mechanized; counts as Druze in DBS |
| 1568 | Diggers | 2 | HI | Mercenary Troops | Regular, Impetuous | Wildcard; counts as Druze |
| 50 | Warcors | 1 | LI | Mercenary Troops | Irregular | — |
| 1555 | Wolfgang Amadeus Wolff | 1 | WB | Character | Regular | Wildcard |
| 19 | Fugazi Dronbots | 2 | REM | Support Troops | Regular | — |
| 334 | Kameel Remotes | 2 | REM | Support Troops | Regular | — |
| 1565 | Motorized Bounty Hunters | 2 | LI | Mercenary Troops | Irregular, Impetuous | Mechanized; Fast Attack |
| 1748 | Extreme Zellenkrieger | 1 | WB | Support Troops | Irregular, Impetuous | — |
| 1569 | Triphammer | 1 | TAG | Mercenary Troops | Regular | Mechanized; includes Turtlemek Ancillary Remote |
| 1564 | Fiddler | 1 | LI | Character | Regular | No Druze Fireteam access despite option 1 FTO label |
| 379 | Druze Shock Teams | 255 | MI | Veteran Troops | Regular | Druze Bayram Security |
| 1749 | Denma Connolly | 1 | WB | Character | Regular, Impetuous | Druze Bayram Security |
| 300 | Anaconda | 1 | TAG | Mercenary Troops | Regular | Mechanized; embedded Operator state |
| 265 | Wardrivers | 1 | LI | Mercenary Troops | Regular | — |
| 1160 | Aïda Swanson | 1 | LI | Character | Regular | Wildcard, **option 2 FTO only**; counts as Druze |
| 380 | Scarface & Cordelia | 1 | TAG/LI | Character | Regular | Mechanized composite choice; includes Turtlemek |
| 325 | Bashi Bazouks | 4 | LI | Mercenary Troops | Irregular | — |
| 17 | Sierra Dronbots | 1 | REM | Support Troops | Regular | — |
| 49 | Authorized Bounty Hunters | 2 | LI | Mercenary Troops | Regular | Wildcard |
| 1275 | Libertos Freedom Fighters | 1 | LI | Mercenary Troops | Irregular | — |
| 35 | Bulleteer Armbots | 2 | REM | Support Troops | Regular | Fast Attack |
| 1538 | Táowù | 1 | LI | Character | Regular | Druze Bayram Security; counts as Druze |

### Optional-mode entries

| Unit ID | Unit | Mode | Fireteam hook |
|---:|---|---|---|
| 1925 | Rumbler Spec-Ops | Infinity Spec-Ops | Up to 1 in Druze Bayram Security or Mechanized Fireteams |
| 1939 | NA2 Team-Ops | Infinity Team-Ops | Optional-mode only; no normal-roster Fireteam row |

## Unit details

Notation: stats are `MOV CC BS PH WIP ARM BTS VITA/STR S`. Source option IDs are retained because otherwise-similar loadouts and FTO legality can depend on them.

### Pathfinder Dronbots — `pathfinder-dronbot`

**Unit ID:** 16 — AVA 3 — REM, Support Troops.

- **Stats:** `15-10 13 11 10 13 0 3 STR1 3`.
- **Rules/equipment:** Deactivator, Repeater, Remote Presence, Courage, Triangulated Fire, Forward Observer, Sensor.
- **Option 1:** **14 / 0** — Combi Rifle, Flash Pulse, PARA CC Weapon (-3).
- **Option 2:** **17 / 0** — same weapons; Tactical Awareness.

### Clipper Dronbots — `clipper-dronbot`

**Unit ID:** 18 — AVA 1 — REM, Support Troops.

- **Stats:** `15-10 13 12 10 13 0 3 STR1 3`.
- **Rules:** Remote Presence, Courage.
- **Option 1:** **16 / 1.5** — Missile Launcher, PARA CC Weapon (-3); BS Attack (Guided).
- **Option 5 FTO:** **19 / 1.5** — Missile Launcher (+1B), PARA CC Weapon (-3).
- **Fireteam:** Wildcard, **option 5 only**.

### Nasmat Remotes — `nasmat-remotes`

**Unit ID:** 333 — AVA 2 — REM, Support Troops; Peripheral (Servant).

- **Stats:** `15-10 11 8 10 13 0 3 STR1 1`.
- **Rules:** Courage, Mimetism (-3), Peripheral (Servant).
- **Option 1:** **3 / 0** — PARA CC Weapon (-3); no Order of its own.

### Hunzakuts — `hunzakuts`

**Unit ID:** 310 — AVA 2 — SK, Spec. Trained Troops; Irregular.

- **Stats:** `10-10 14 11 12 14 0 0 1 2`.
- **Rules:** Surprise Attack (-3), Camouflage, Infiltration, Mimetism (-3), Stealth, Terrain (Total).
- **Option 1:** **18 / 0.5** — Deployable Repeater; Rifle, Grenade Launcher, Shock Mine, Boarding Pistol, CC Weapon.
- **Option 2:** **18 / 0.5** — Sniper Rifle, Shock Mine, Boarding Pistol, CC Weapon.
- **Option 3:** **19 / 0** — Forward Observer, Deployable Repeater; Rifle, Light Shotgun, Shock Mine, Boarding Pistol, CC Weapon.
- **Option 4:** **15 / 0** — Forward Observer; Boarding Shotgun, D-Charges, Boarding Pistol, CC Weapon.

### Peacemaker Armbots — `armbots-peacemakers`

**Unit ID:** 36 — AVA 1 — REM, Support Troops.

- **Stats:** `15-10 13 12 10 13 1 3 STR1 4`.
- **Rules/equipment:** Repeater, Remote Presence, Courage, Forward Deployment (+20), Mimetism (-3).
- **AuxBot_3 state:** `15-10 13 10 8 11 0 3 STR1 1`; Peripheral (Synchronized), Courage, Forward Deployment (+20), Mimetism (-3).
- **Option 1:** **23 / 0** — Heavy Shotgun, Pulzar, PARA CC Weapon (-3); includes AuxBot_3 with Heavy Flamethrower, Shock Mine, PARA CC Weapon (-3).
- **Option 3:** **24 / 0.5** — Heavy Shotgun, Pulzar, PARA CC Weapon (-3); includes AuxBot_3B with Heavy Flamethrower, Shock Mine, PARA CC Weapon (-3), Minelayer.
- **Option 4:** **23 / 0** — Boarding Shotgun (+1B), Pulzar, PARA CC Weapon (-3); no Peripheral.
- **Option 5:** **27 / 0** — Boarding Shotgun (+1B), Pulzar, PARA CC Weapon (-3); includes AuxBot_3.

### Saito Tōgan — `saito-togan`

**Unit ID:** 668 — AVA 1 — SK, Character.

- **Stats:** `10-10 24 11 13 13 1 0 1 2`.
- **Rules/equipment:** Bangbomb (+4), Martial Arts L4, Surprise Attack (-3), Camouflage, Courage, Hidden Deployment, Dodge (+2.5), Infiltration, Mimetism (-6), Stealth, Terrain (Total).
- **Option 1:** **33 / 0** — T2 Boarding Shotgun, Smoke Grenades, Pistol, EXP CC Weapon (PS=4).
- **Option 2:** **35 / 0** — Specialist Operative; Combi Rifle, D-Charges, Smoke Grenades, Pistol, EXP CC Weapon (PS=4).

### Valerya Gromoz — `valerya-gromoz-mercenary-hacker`

**Unit ID:** 464 — AVA 1 — LI, Character.

- **Stats:** `10-10 15 11 10 14 1 3 1 2`.
- **Rules/equipment:** Hacker, Hacking Device with Total Control (+1B) upgrade.
- **Option 1:** **19 / 0.5** — Combi Rifle, Zapper, Pitcher, Pistol, CC Weapon.
- **Fireteam:** Wildcard, all standard options.

### Armand “Le Muet” — `armand-le-muet-freelance-killer`

**Unit ID:** 680 — AVA 1 — MI, Character.

- **Full-power stats:** `10-10 21 13 12 13 2 3 2 2`.
- **Inactive Symbiont Armor stats:** `10-10 21 13 12 13 0 0 2 2`.
- **Full-power rules:** BS Attack (Shock), Forward Deployment (+10), Natural Born Warrior, Mimetism (-6), Stealth, Transmutation (1).
- **Inactive rules:** BS Attack (Shock), Natural Born Warrior, Stealth.
- **Option 2338:** **33 / 1.5** — MULTI Sniper Rifle, Nanopulser, Shock Mine, Breaker Pistol (+1B), Viral CC Weapon (PS=7); Minelayer.
- **Option 2339:** **34 / 1.5** — Multispectral Visor L1; MULTI Sniper Rifle, Nanopulser, Breaker Pistol (+1B), Viral CC Weapon (PS=7).

### Security Chief Arslan — `security-chief-arslan`

**Unit ID:** 986 — AVA 1 — MI, Character.

- **Stats:** `10-10 17 13 11 13 3 3 1 2`.
- **Rules/equipment:** Multispectral Visor L1, X-Visor, BS Attack (SR-1), Courage, Dodge (+3), Warhorse, No Wound Incapacitation.
- **Option 1:** **35 / 0** — MULTI Rifle, Light Shotgun, Viral Pistol, CC Weapon, Disco Baller.
- **Option 2 Lieutenant:** **35 / 0** — same loadout; Lieutenant.
- **Fireteam:** Wildcard, all options; counts as Druze.

### Kunai Solutions Ninjas — `kunai-solutions-ninjas`

**Unit ID:** 1502 — AVA 2 — SK, Mercenary Troops.

- **Stats:** `10-10 21 12 12 12 1 0 1 2`.
- **Rules:** Martial Arts L3, Surprise Attack (-3), Camouflage, Courage, Hidden Deployment, Dodge (+2.5), Mimetism (-6), Terrain (Total), Climbing Plus, Stealth.
- **Option 1:** **28 / 1.5** — MULTI Sniper Rifle, Pistol, Shock CC Weapon (PS=6).
- **Option 2:** **26 / 0** — Shock Marksman Rifle, Pistol, Shock CC Weapon (PS=6); BS Attack (AP).
- **Option 3:** **25 / 0.5** — Thunderbolt, PARA Mine, Pistol, Shock CC Weapon (PS=6); BS Attack (T2).

### Yuan Yuan — `yuan-yuan`

**Unit ID:** 378 — AVA 4 — WB, Mercenary Troops; Irregular, Impetuous.

- **Stats:** `10-10 22 10 14 13 0 0 1 2`.
- **Rules:** Booty, Parachutist, Combat Jump (PH=11), No Cover, Super-Jump (Jet Propulsion), Impetuous.
- **Option 2:** **6 / 0** — Chain Rifle, Smoke Grenades, Heavy Pistol, AP CC Weapon (PS=6).
- **Option 3:** **7 / 0** — Chain Rifle, Smoke Grenades, Pistol, DA CC Weapon (PS=6).
- **Option 4:** **11 / 0** — Boarding Shotgun, Smoke Grenades, Pistol, AP CC Weapon (PS=6).
- **Option 5:** **11 / 0** — Rifle, Smoke Grenades, Pistol, AP CC Weapon (PS=6).

### Monstruckers — `monstruckers`

**Unit ID:** 1333 — AVA 2 — LI, Mercenary Troops; Irregular.

- **Stats:** `10-10 16 11 12 13 1 0 1 2`.
- **Rules/equipment:** Engineer, Climbing Plus, Deactivator, GizmoKit.
- **Option 1:** **15 / 0** — Boarding Shotgun, Adhesive Launcher Rifle, E/M Grenades, Pistol, CC Weapon.
- **Option 2:** **12 / 0** — Submachine Gun, Chain Rifle, Drop Bears, Pistol, CC Weapon.
- **Option 3:** **15 / 0** — Submachine Gun, Chain Rifle, Drop Bears, Armed Turret (AP Rifle), Pistol, CC Weapon.
- **Option 4:** **16 / 0** — 360º Visor; Rifle, Light Shotgun, Akrylat-Kanone, D-Charges, Pistol, CC Weapon.
- **Fireteam:** Druze Bayram Security, max 2.

### Zellenkrieger — `zellenkrieger`

**Unit ID:** 1747 — AVA 1 — WB, Support Troops; Irregular, Impetuous.

- **Stats:** `10-10 23 10 13 12 1 3 STR1 2`.
- **Rules:** CC Attack (-3), Berserk, Courage, Dodge (+2.5), Natural Born Warrior, MetaChemistry (ReRoll), No Cover, Impetuous.
- **Option 1:** **8 / 0** — Light Shotgun, Smoke Grenades, Heavy Pistol, DA CC Weapon (PS=7).
- **Option 2:** **8 / 0** — Pulzar, Smoke Grenades, Heavy Pistol (+1B), DA CC Weapon (PS=7).
- **Option 3 FTO:** **8 / 0** — Pulzar (+1B), Heavy Pistol (+1B), DA CC Weapon (PS=7).
- **Fireteam:** Druze Bayram Security, **option 3 only**.

### Brawlers, Mercenary Enforcers — `brawlers-mercenary-enforcers`

**Unit ID:** 987 — AVA 4 — MI, Spec. Trained Troops.

- **Stats:** `10-10 17 12 11 12 2 3 1 2`.
- **Rules:** Sixth Sense.
- **Option 1:** **15 / 0** — Rifle, Light Shotgun (+1B), Pistol, CC Weapon.
- **Option 2:** **15 / 1.5** — X-Visor; Heavy Rocket Launcher, Assault Pistol, CC Weapon.
- **Option 3:** **25 / 1.5** — Multispectral Visor L2; MULTI Sniper Rifle, AP Mine, Pistol, CC Weapon.
- **Option 5:** **16 / 0.5** — Hacker, Hacking Device; Submachine Gun, Cybermine, Pistol, CC Weapon.
- **Option 6:** **19 / 0** — Engineer, Deactivator, GizmoKit; Rifle, Light Shotgun (+1B), D-Charges, Pistol, CC Weapon.
- **Option 7:** **19 / 0** — Doctor, MediKit; Rifle, Light Shotgun (+1B), Pistol, CC Weapon.
- **Option 9 Lieutenant:** **15 / 0** — Rifle, Light Shotgun (+1B), Pistol, CC Weapon; Lieutenant.
- **Fireteams:** Druze Bayram Security, max 4 and counts as Druze; Mechanized, max 1.

### Diggers — `diggers-armed-prospectors`

**Unit ID:** 1568 — AVA 2 — HI, Mercenary Troops; Regular, Impetuous.

- **Full-power stats:** `10-10 21 11 13 12 3 0 2 2`.
- **Battle-ravaged stats:** `10-10 21 10 12 12 2 0 2 2`.
- **Full-power rules:** CC Attack (+1B), Booty, Courage, Dodge (+2.5), Natural Born Warrior, Impetuous, Transmutation (1), No Cover.
- **Battle-ravaged rules:** CC Attack (+1B), Booty, Courage, Natural Born Warrior, Impetuous, No Cover.
- **Option 1:** **18 / 0** — Rifle, Light Shotgun, Grenades, Pistol, AP CC Weapon (PS=6).
- **Option 2:** **14 / 0** — Chain Rifle (+1B), Grenades, Pistol, AP CC Weapon (PS=6).
- **Fireteam:** Wildcard, max 2; counts as Druze.

### Warcors — `warcors-war-correspondents`

**Unit ID:** 50 — AVA 1 — LI, Mercenary Troops; Irregular.

- **Stats:** `10-10 11 9 11 13 0 0 1 2`.
- **Rules:** Journalist.
- **Option 1:** **3 / 0** — 360º Visor; Flash Pulse, Stun Pistol, PARA CC Weapon (-3).
- **Option 2:** **3 / 0** — Sixth Sense; Flash Pulse, Stun Pistol, PARA CC Weapon (-3).

### Wolfgang Amadeus Wolff — `wolfgang-amadeus-wolff`

**Unit ID:** 1555 — AVA 1 — WB, Character.

- **Stats:** `15-5 22 12 14 13 3 3 2 2`.
- **Rules:** Martial Arts L3, BS Attack (Continuous Damage), Berserk (+3), Courage, Dodge (+5), Immunity (ARM), Climbing Plus, Terrain (Zero-G), Frenzy, Discover (+6).
- **Option 1:** **33 / 0** — MULTI Rifle (+1SD), Chain-colt, E/M Grenades (+1SD), Heavy Pistol, PARA CC Weapon (-6), DA CC Weapon (PS=4).
- **Fireteam:** Wildcard.

### Fugazi Dronbots — `fugazi-dronbot`

**Unit ID:** 19 — AVA 2 — REM, Support Troops.

- **Stats:** `15-15 13 8 11 13 0 3 STR1 3`.
- **Rules/equipment:** Repeater, Remote Presence, Courage, Mimetism (-3).
- **Option 1:** **7 / 0** — Flash Pulse, PARA CC Weapon (-3).

### Kameel Remotes — `kameel-remotes`

**Unit ID:** 334 — AVA 2 — REM, Support Troops.

- **Stats:** `10-10 13 11 10 13 2 3 STR1 4`.
- **Rules/equipment:** Baggage, Courage, Remote Presence.
- **Option 1:** **8 / 0** — Deactivator, Repeater; PARA CC Weapon (-3).
- **Option 2:** **14 / 0.5** — EVO Hacking Device, Hacker; PARA CC Weapon (-3).
- **Option 3:** **16 / 0** — Repeater, Total Reaction; Rifle, Light Shotgun, PARA CC Weapon (-3).

### Motorized Bounty Hunters — `motorized-bounty-hunters`

**Unit ID:** 1565 — AVA 2 — LI, Mercenary Troops; Irregular, Impetuous.

- **Stats:** `20-15 17 12 10 13 1 3 1 4`.
- **Rules/equipment:** Motorcycle, Booty (ReRoll), Limited Cover, Dodge (+5), Mimetism (-3), Impetuous.
- **Option 1:** **8 / 0** — Boarding Shotgun, Pistol, PARA CC Weapon (-6), Heavy Riotstopper.
- **Option 2:** **9 / 0** — Submachine Gun, Chain-colt (+1B), Pistol, PARA CC Weapon (-6).
- **Option 3:** **16 / 0.5** — Red Fury, Breaker Pistol, PARA CC Weapon (-6).
- **Fireteams:** Mechanized, max 1; Fast Attack, max 1.

### Extreme Zellenkrieger — `extreme-zellenkrieger`

**Unit ID:** 1748 — AVA 1 — WB, Support Troops; Irregular, Impetuous.

- **Stats:** `10-10 23 10 15 12 1 3 STR1 5`.
- **Rules:** CC Attack (-3), Berserk, Courage, Dodge (+5), Natural Born Warrior, Immunity (BTS), No Cover, MetaChemistry (ReRoll), Impetuous.
- **Option 1:** **11 / 0** — Light Shotgun, Smoke Grenades, Heavy Pistol, DA CC Weapon (PS=5).
- **Option 2:** **11 / 0** — Pulzar, Smoke Grenades, Heavy Pistol (+1B), DA CC Weapon (PS=5).

### Triphammer — `triphammers-repurposed-industrial-tags`

**Unit ID:** 1569 — AVA 1 — TAG, Mercenary Troops.

- **Full-power stats:** `15-10 17 13 16 12 7 3 STR3 7`.
- **Battle-ravaged stats:** `10-10 15 12 14 12 4 0 STR3 7`.
- **Full-power rules:** CC Attack (Antimaterial), BS Attack (SR-1), Booty, Dodge (PH=9), GizmoKit (PH=10), Tactical Awareness, Transmutation (2).
- **Battle-ravaged rules:** CC Attack (Antimaterial), BS Attack (SR-1), Booty, Dodge (PH=9), GizmoKit (PH=9), Tactical Awareness.
- **Turtlemek Ancillary Remote:** `15-10 - - 10 12 0 3 STR1 1`; Courage, Dodge (+3), Mimetism (-3), Specialist Operative, Peripheral (Ancillary).
- **Option 2:** **53 / 1.5** — AP Spitfire, Heavy Flamethrower, AP CC Weapon (PS=4); includes Turtlemek.
- **Option 3:** **52 / 1.5** — AP Spitfire, Chain-colt (+1B), AP CC Weapon (PS=4); includes Turtlemek.
- **Option 4:** **52 / 0** — Heavy Shotgun, Thunderbolt (+1B), AP CC Weapon (PS=4); includes Turtlemek.
- **Option 5:** **48 / 0** — Heavy Shotgun, Heavy Rocket Launcher, Panzerfaust (+1B), AP CC Weapon (PS=4); includes Turtlemek.
- **Fireteam:** Mechanized, max 1.

### Fiddler — `fiddler-aristeia-s-ex-toymaker`

**Unit ID:** 1564 — AVA 1 — LI, Character.

- **Stats:** `15-10 18 12 12 14 1 3 STR1 2`.
- **Rules/equipment:** GizmoKit, CC Attack (+1B), Dodge (+3), Dodge (+2.5), Engineer, Immunity (Critical), No Wound Incapacitation.
- **JackBot state:** `15-10 16 11 10 12 0 3 STR1 1`; Peripheral (Synchronized), Courage, Explode, Climbing Plus; Vulkan Shotgun.
- **Option 1 FTO:** **29 / 0** — Super-Jump; Contender (+1B), Drop Bears, D-Charges, Breaker Pistol, PARA CC Weapon (-3).
- **Option 2:** **36 / 0** — Climbing Plus; same weapons; includes 1 JackBot.
- **Option 3:** **43 / 0** — Climbing Plus; same weapons; includes 2 JackBots.
- **Fireteam:** **none in Druze Bayram Security.** The FTO label on option 1 does not create access.

### Druze Shock Teams — `druze-shock-teams`

**Unit ID:** 379 — AVA 255 — MI, Veteran Troops.

- **Stats:** `10-10 16 12 11 13 3 3 1 2`.
- **Rules/equipment:** X-Visor, BS Attack (SR-1), Warhorse.
- **Option 1:** **20 / 0** — Combi Rifle, Chain-colt, Viral Pistol, CC Weapon.
- **Option 2:** **28 / 1.5** — Heavy Machine Gun, Viral Pistol, Chain-colt, CC Weapon.
- **Option 3:** **21 / 0** — Combi Rifle, Chain-colt, Panzerfaust, Viral Pistol, CC Weapon.
- **Option 4:** **24 / 1** — Combi Rifle, Chain-colt, Grenade Launcher, E/M Grenade Launcher, Viral Pistol, CC Weapon.
- **Option 5:** **23 / 0** — Shock Marksman Rifle, Chain-colt, Viral Pistol, CC Weapon.
- **Option 6:** **25 / 0.5** — Hacker, Hacking Device; Combi Rifle, Pitcher, D-Charges, Viral Pistol, CC Weapon.
- **Option 7:** **23 / 0** — Hacker, Killer Hacking Device; Combi Rifle, Pitcher, D-Charges, Viral Pistol, CC Weapon.
- **Option 10:** **27 / 1.5** — Mimetism (-3); MULTI Sniper Rifle, Viral Pistol, Chain-colt, CC Weapon.
- **Option 11:** **22 / 0** — Paramedic, MediKit; Combi Rifle, Chain-colt, Viral Pistol, CC Weapon.
- **Option 12 Lieutenant:** **20 / 0** — Combi Rifle, Chain-colt, Viral Pistol, CC Weapon; Lieutenant.
- **Fireteam:** Druze Bayram Security, max 5; member of the required-source set.

### Denma Connolly — `denma-connolly`

**Unit ID:** 1749 — AVA 1 — WB, Character; Regular, Impetuous.

- **Stats:** `15-5 23 11 14 12 1 3 STR1 2`.
- **Rules:** Martial Arts L1, Berserk, Courage, Dodge (+5), Natural Born Warrior, MetaChemistry (ReRoll), No Cover, Impetuous.
- **Option 1:** **12 / 0** — Chain Rifle (+1B), Smoke Grenades, Heavy Pistol (+1B), AP + DA CC Weapon (PS=6).
- **Fireteam:** Druze Bayram Security, max 1.
- **Source alias:** Fireteam chart slug `denma-connolly-caledonian-zellenkrieger` resolves to this unit ID `1749`; the roster slug is `denma-connolly`.

### Anaconda — `anaconda-merc-tag-squad`

**Unit ID:** 300 — AVA 1 — TAG, Mercenary Troops.

- **TAG stats:** `15-5 21 13 16 13 7 6 STR3 7`.
- **TAG rules/equipment:** ECM: Guided (-6), BS Attack (SR-1), Courage, Dodge (PH=11), GizmoKit (PH=11), Tactical Awareness, Transmutation (Escape System -2), Warhorse, Immunity (AP).
- **Operator stats:** `10-10 13 12 10 13 1 3 3 2`.
- **Operator rules:** Courage, Specialist Operative, Tactical Awareness, Warhorse, Mimetism (-3).
- **Option 1:** **59 / 1.5** — AP Spitfire, Heavy Flamethrower (+1B), Thunderbolt (AP), DA CC Weapon (PS=4).
- **Option 2:** **59 / 1.5** — Heavy Machine Gun, Light Shotgun (+2B), Panzerfaust, DA CC Weapon (PS=4).
- **Embedded Operator:** Spitfire, Smoke Grenade Launcher, Boarding Pistol, CC Weapon.
- **Fireteam:** Mechanized; member of the required-source set.

### Wardrivers — `wardrivers-merc-hackers`

**Unit ID:** 265 — AVA 1 — LI, Mercenary Troops.

- **Stats:** `10-10 13 11 10 13 0 3 1 2`.
- **Rules:** Sixth Sense.
- **Option 4:** **14 / 0** — Hacker with Zero Pain upgrade, Commlink; Boarding Shotgun, Flash Pulse, Cybermine, Pistol, CC Weapon.

### Aïda Swanson — `aida-swanson`

**Unit ID:** 1160 — AVA 1 — LI, Character.

- **Stats:** `10-10 19 12 11 13 1 3 1 2`.
- **Rules:** Martial Arts L2, Courage, Booty, Forward Deployment (+10), Mimetism (-3), Shasvastii, Stealth.
- **Option 1:** **24 / 0.5** — Submachine Gun (+1B), Viral Mine, Viral Pistol, Shock CC Weapon (PS=7); Minelayer, Decoy (2).
- **Option 2 FTO:** **21 / 0** — Submachine Gun, Viral Mine, Viral Pistol, Shock CC Weapon (PS=7); Minelayer.
- **Fireteam:** Wildcard, **option 2 only**; counts as Druze.

### Scarface & Cordelia — `scarface-and-cordelia`

**Unit ID:** 380 — AVA 1 — composite Character choice.

**Scarface TAG state**

- **Stats:** `15-10 22 13 16 13 7 6 STR3 7`.
- **Rules/equipment:** ECM: Guided (-6), ECM: Hacker (-3), CC Attack (-3), BS Attack (SR-1), Berserk (+3), Courage, Dodge (PH=11), GizmoKit (PH=11), Tactical Awareness.

**Cordelia Turner state**

- **Stats:** `10-10 13 11 10 13 1 3 1 2`.
- **Rules/equipment:** Courage, Engineer, Mimetism (-3), Deactivator, GizmoKit.
- **Weapons:** Combi Rifle, D-Charges, PARA Mine, Boarding Pistol, CC Weapon.

**Turtlemek Ancillary Remote**

- **Stats:** `15-10 - - 10 12 0 3 STR1 1`.
- **Rules:** Courage, Dodge (+3), Mimetism (-3), Specialist Operative, Peripheral (Ancillary).

**Composite loadouts**

- **Option 1 — Alpha & Cordelia:** **80 / 1.5** — Scarface Mk12 (+1B), Heavy Rocket Launcher (+1B), DA CC Weapon (PS=4); includes Cordelia and Turtlemek.
- **Option 2 — Beta & Cordelia:** **76 / 1.5** — Scarface AP Heavy Machine Gun, Panzerfaust, DA CC Weapon (PS=4); includes Cordelia and Turtlemek.
- **Option 3 — Gamma & Cordelia:** **76 / 1.5** — Scarface AP Spitfire (+1B), Panzerfaust, DA CC Weapon (PS=4); includes Cordelia and Turtlemek.
- **Fireteam:** Mechanized. The chart exposes separate Scarface and Cordelia member rows, but ordinary roster selection is the composite Scarface & Cordelia choice and must preserve that dependency.

### Bashi Bazouks — `bashi-bazouks`

**Unit ID:** 325 — AVA 4 — LI, Mercenary Troops; Irregular.

- **Stats:** `10-10 16 11 10 12 2 0 1 2`.
- **Rules/equipment:** Holomask, Holoprojector, Surprise Attack (-3), Parachutist, Terrain (Zero-G), Combat Jump (PH=11).
- **Option 1:** **13 / 0** — Contender (+1SD), Boarding Pistol (+1B), CC Weapon.
- **Option 2:** **14 / 0** — T2 Boarding Shotgun, Boarding Pistol (+1B), CC Weapon; BS Attack (AP).
- **Option 3:** **16 / 0** — Specialist Operative; Rifle, Light Shotgun, E/M Mine, Boarding Pistol (+1B), CC Weapon.
- **Option 5:** **14 / 0** — Specialist Operative; Breaker Rifle, Boarding Pistol (+1B), CC Weapon.
- **Option 8:** **12 / 0** — Specialist Operative; Submachine Gun, Boarding Pistol (+1B), CC Weapon.

### Sierra Dronbots — `sierra-dronbot`

**Unit ID:** 17 — AVA 1 — REM, Support Troops.

- **Stats:** `15-10 13 11 10 13 0 3 STR1 3`.
- **Rules/equipment:** 360º Visor, Remote Presence, Courage, Total Reaction.
- **Option 1:** **23 / 1** — Heavy Machine Gun, PARA CC Weapon (-3).
- **Option 2:** **18 / 0** — Thunderbolt (+1B), PARA CC Weapon (-3).

### Authorized Bounty Hunters — `authorized-bounty-hunters`

**Unit ID:** 49 — AVA 2 — LI, Mercenary Troops.

- **Stats:** `10-10 16 12 10 13 1 3 1 2`.
- **Rules:** Booty (ReRoll), Stealth.
- **Option 2:** **12 / 0** — Boarding Shotgun, Pistol, PARA CC Weapon (-6), Heavy Riotstopper.
- **Option 3:** **19 / 0.5** — Sniper Rifle, Breaker Pistol (+1B), PARA CC Weapon (-6).
- **Option 4:** **21 / 1** — Spitfire, Boarding Pistol, PARA CC Weapon (-6).
- **Option 5:** **12 / 0** — Submachine Gun, Akrylat-Kanone, Breaker Pistol, PARA CC Weapon (-6).
- **Fireteam:** Wildcard, max 2.

### Libertos Freedom Fighters — `libertos-freedom-fighters`

**Unit ID:** 1275 — AVA 1 — LI, Mercenary Troops; Irregular.

- **Stats:** `10-10 16 11 11 12 0 0 1 2`.
- **Rules:** Camouflage (1 Use), Courage, Forward Deployment (+20), Dodge (+3), Dodge (+2.5), Terrain (Aquatic), Dogged, Frenzy.
- **Option 1:** **8 / 0** — Submachine Gun, Chain-colt, Pistol, CC Weapon.
- **Option 4:** **8 / 1** — Light Shotgun, Shock Mine, Pistol, CC Weapon; Minelayer.

### Bulleteer Armbots — `armbots-bulleteer`

**Unit ID:** 35 — AVA 2 — REM, Support Troops.

- **Stats:** `15-10 13 12 10 13 1 3 STR1 4`.
- **Rules/equipment:** Repeater, Remote Presence, Courage, Mimetism (-6).
- **Option 1:** **19 / 0** — Heavy Shotgun (+1B), PARA CC Weapon (-3).
- **Option 2:** **22 / 1** — Spitfire, PARA CC Weapon (-3).
- **Fireteam:** Fast Attack, min 1 / max 2.

### Táowù — `taowu-mastermind-and-schemer`

**Unit ID:** 1538 — AVA 1 — LI, Character.

- **Stats:** `10-10 19 12 10 14 1 3 1 2`.
- **Rules/equipment:** Holomask, BS Attack (+1B), Counterintelligence, Dodge (+3), Natural Born Warrior, Immunity (Shock), Specialist Operative, Stealth.
- **Option 1:** **19 / 0** — Light Shotgun, E/Marat, Flash Pulse, Viral Pistol, PARA CC Weapon (-9).
- **Option 2:** **16 / 0** — Contender, Pulzar, Flash Pulse, Viral Pistol, PARA CC Weapon (-9).
- **Option 4:** **21 / 0** — same as option 2; Chain of Command.
- **Fireteam:** Druze Bayram Security, max 1; counts as Druze.

## Optional-mode profile details

### Rumbler Spec-Ops — `rumbler-spec-ops`

**Unit ID:** 1925 — Infinity Spec-Ops only.

- Initial profile: `10-10 17 12 11 13 2 3 1 2`; Infinity Spec-Ops, Immunity (Shock), Sixth Sense, Terrain (Total).
- Enhanced profile: `10-10 17 13 13 13 5 3 2 2`; Sixth Sense, Terrain (Total).
- **Option 1:** **28 / 1** — Heavy Machine Gun, D-Charges, Pistol, CC Weapon.
- **Option 2:** **28 / 1** — AP Spitfire, D-Charges, Pistol, CC Weapon.
- **Option 3:** **23 / 0** — Specialist Operative, GizmoKit; MULTI Rifle, Pistol, CC Weapon.
- **Option 4:** **26 / 0.5** — Hacker, Hacking Device; AP Combi Rifle, D-Charges, Pistol, CC Weapon.
- **Option 5:** **23 / 0** — Forward Observer; MULTI Rifle, Flash Pulse, D-Charges, Pistol, CC Weapon.
- **Option 6:** **23 / 0** — Paramedic, MediKit; AP Combi Rifle, D-Charges, Pistol, CC Weapon.
- **Fireteams:** Optional-mode member of Druze Bayram Security or Mechanized Fireteams, max 1.

### NA2 Team-Ops — `na2-team-ops`

**Unit ID:** 1939 — Infinity Team-Ops only.

This optional-mode record contains Rumbler-1, Rumbler Heavy, and Gort SpecBot Team-Ops profiles. It has **no row in the ordinary Druze Fireteam chart** and is not counted among the 35 standard roster records.

## Fireteams

The tables below are authoritative for Druze Bayram Security Fireteam legality. Profile names such as `FTO` do not grant access by themselves.

### Druze Bayram Security Fireteams

**Types:** Duo, Haris, Core.

The Army source marks both Druze and Brawler rows `required: true`. Treat them as a **required source-choice set**: at least one member must come from one of those two rows.

| Member | Min | Max | Required / equivalence | Profile restriction |
|---|---:|---:|---|---|
| Druze Shock Teams | 0 | 5 | required-source set | all options |
| Brawlers | 0 | 4 | required-source set; counts as Druze | all options |
| Monstruckers | 0 | 2 | — | all options |
| Táowù | 0 | 1 | counts as Druze | all options |
| Zellenkrieger | 0 | 1 | — | **FTO option 3 only** |
| Denma Connolly | 0 | 1 | — | option 1 |
| Rumbler Spec-Ops | 0 | 1 | Spec-Ops mode only | optional-mode record |

Wildcards may join subject to the Wildcard rules below.

### Mechanized Fireteams

**Types:** Duo.

The Army source marks Anaconda and Scarface rows `required: true`. Treat them as a **required source-choice set**: at least one of those source rows must be present.

| Member | Min | Max | Required / equivalence | Profile restriction |
|---|---:|---:|---|---|
| Anaconda | 0 | 1 | required-source set | both standard TAG options |
| Scarface | 0 | 1 | required-source set | Scarface component of the composite roster choice |
| Cordelia Turner | 0 | 1 | — | Cordelia component of the composite roster choice |
| Triphammer | 0 | 1 | — | all options |
| Brawler | 0 | 1 | — | all options |
| Motorized Bounty Hunter | 0 | 1 | — | all options |
| Rumbler Spec-Ops | 0 | 1 | Spec-Ops mode only | optional-mode record |

The standard roster exposes **Scarface & Cordelia** as a composite selection. The Fireteam chart exposes Scarface and Cordelia as separate member rows for composition purposes; roster legality must still preserve the composite source dependency.

Wildcards may join subject to the Wildcard rules below.

### Fast Attack Fireteams

**Types:** Duo.

| Member | Min | Max | Required / equivalence | Profile restriction |
|---|---:|---:|---|---|
| Bulleteer | 1 | 2 | Native required minimum | both options |
| Motorized Bounty Hunter | 0 | 1 | — | all options |

Wildcards may join subject to the Wildcard rules below.

## Wildcards

| Wildcard | Max | Counts as | Profile restriction |
|---|---:|---|---|
| Authorized Bounty Hunter | 2 | — | all options |
| Digger | 2 | Druze | all options |
| Security Chief Arslan | 1 | Druze | both options |
| Aïda Swanson FTO | 1 | Druze | **option 2 only** |
| Valerya Gromoz | 1 | — | option 1 |
| Wolfgang Amadeus Wolff | 1 | — | option 1 |
| Clipper Dronbot FTO | 1 | — | **option 5 only** |

Wildcard means the listed profile may join any otherwise legal Druze Bayram Security Fireteam unless another rule prevents it. `Counts as` labels are preserved separately because they can matter to composition requirements.

## Unit → Fireteam access index

This is a derivative lookup table. If it conflicts with the canonical Fireteam section above, the canonical section wins.

| Unit | Access |
|---|---|
| Anaconda | Mechanized — both standard TAG options; required-source member |
| Authorized Bounty Hunters | Wildcard — all options, max 2 |
| Aïda Swanson | Wildcard — **option 2 FTO only**; counts as Druze |
| Arslan | Wildcard — both options; counts as Druze |
| Brawlers | Druze Bayram Security — all options, max 4, counts as Druze; Mechanized — all options, max 1 |
| Bulleteer | Fast Attack — both options, min 1 / max 2 |
| Clipper Dronbot | Wildcard — **option 5 FTO only** |
| Cordelia Turner | Mechanized — composite Scarface & Cordelia component |
| Denma Connolly | Druze Bayram Security — option 1, max 1 |
| Diggers | Wildcard — all options, max 2; counts as Druze |
| Druze Shock Teams | Druze Bayram Security — all options, max 5; required-source member |
| Monstruckers | Druze Bayram Security — all options, max 2 |
| Motorized Bounty Hunter | Mechanized — all options, max 1; Fast Attack — all options, max 1 |
| Scarface & Cordelia | Mechanized — composite roster choice; Scarface is a required-source member and Cordelia has a separate chart row |
| Táowù | Druze Bayram Security — all options, max 1; counts as Druze |
| Triphammer | Mechanized — all options, max 1 |
| Valerya Gromoz | Wildcard — option 1 |
| Wolfgang Amadeus Wolff | Wildcard — option 1 |
| Zellenkrieger | Druze Bayram Security — **option 3 FTO only**, max 1 |
| Rumbler Spec-Ops | Druze Bayram Security or Mechanized — optional Spec-Ops mode only, max 1 |

Explicit negative lookup notes:

- **Fiddler option 1 (`Fiddler FTO`) has no Druze Fireteam access.**
- **Zellenkrieger options 1 and 2** cannot use the Druze Bayram Security Fireteam row; only option 3 can.
- **Aïda Swanson option 1** cannot use the Wildcard row; only FTO option 2 can.
- **Clipper option 1** cannot use the Wildcard row; only FTO option 5 can.
- No other standard roster unit gains Fireteam access merely from an FTO label, mercenary status, or shared NA2 ancestry.

## Roster dependencies and composite records

The standard Druze source exposes no top-level `relations` restrictions in this snapshot.

Composite and Peripheral handling:

- **Nasmat Remotes** are Servant Peripherals and do not generate Orders independently.
- **Peacemaker** options may include an AuxBot_3 or AuxBot_3B synchronized Peripheral; those AuxBots are not separate roster records.
- **Triphammer** options include one Turtlemek Ancillary Remote; it is not a separate roster record.
- **Fiddler** options 2 and 3 include one or two JackBots respectively; JackBots are not separate roster records.
- **Scarface & Cordelia** are selected as one composite roster record, with embedded Cordelia and Turtlemek components. The Fireteam chart nevertheless exposes Scarface and Cordelia as separate member rows and both facts must be preserved when checking composition.
- Optional Spec-Ops / Team-Ops subprofiles and SpecBots remain inside their optional-mode records.

## Reinforcements boundary

The standard Druze Bayram Security dataset exposes Reinforcements Army ID **999**. It is deliberately not merged into this file's standard roster or canonical Fireteam chart. For ordinary Druze list building, use the 35 standard roster records and Fireteams above; use a separate Reinforcements reference when Reinforcement mode is explicitly involved.

## Validation notes

Validated against Army snapshot `7.26246.159`:

- Standard roster membership was determined from faction availability containing sectorial ID `902`.
- **35** standard logical roster records were identified.
- **2** optional-mode records were separated: Rumbler Spec-Ops (`1925`) and NA2 Team-Ops (`1939`).
- Generic `factions: []` Soldier-of-Fortune catalog entries were excluded.
- Fireteam limits are Core `1`, Haris `1`, Duo `256`.
- Canonical families are Druze Bayram Security, Mechanized, and Fast Attack.
- Wildcards are Authorized Bounty Hunters, Diggers, Arslan, Aïda Swanson FTO, Valerya Gromoz, Wolfgang Amadeus Wolff, and Clipper Dronbot FTO.
- FTO restrictions were reconciled against profile option names: Zellenkrieger `3`; Aïda Swanson `2`; Clipper Dronbot `5`.
- Fiddler FTO was intentionally **not** granted Fireteam access because no canonical chart row grants it.
- Counts-as relationships were preserved separately from ordinary membership.
- Required-source sets were preserved for Druze/Brawler and Anaconda/Scarface.
- Denma Connolly's Fireteam-chart slug alias was resolved to roster unit ID `1749` and documented explicitly.
- Reinforcement Army ID `999` remains distinct.

## Provenance

- Corvus Belli Army source revision: `7.26246.159`.
- Army data changed on: **2026-09-03**.
- Mirrored source commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- Source blob: `311c3b0d595ee220d4046b983b8dfb65dceb3b2c`.
- InfinityDB reference commit: `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Fireteam source: Army snapshot canonical `fireteamChart`, normalized using repository Fireteam conventions.
- Generated/verified: **2026-10-16**.
