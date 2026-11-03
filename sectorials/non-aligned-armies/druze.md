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

## Tactical research — Druze Bayram Security (reviewed 2026-10-23)

**Evidence boundary:** This is a tactical interpretation of videos, podcasts, and reported games—not a replacement for the N5.3 Army profiles and canonical Fireteam chart above. Sources from 2022 (N4) and the December 2024 N5 launch can explain *why* a plan works, but their prices, hacking interactions, Fireteam bonuses, profile availability, and list codes are **not** authoritative in October 2026. The roster above remains verified to Army 7.26246.159 / N5.3.

### Executive decisions: choose the plan before the expensive pieces

| Plan | Starting package | Why / failure mode |
|---|---|---|
| **Network control + optional Guided** | Druze KHD with Pitcher; a second hacking source such as Valerya or Druze HD; Hunzakut FO/repeater; Fugazi/Peacemaker; **unlinked** Clipper Guided *if* investing in missiles | Multiple ways to establish a target or repeater let Druze fight without exposing expensive BS12 one-wound infantry. Do **not** spend orders laying repeaters and Spotlighting if you cannot exploit the marked target; bring direct guns and mission specialists too. [V1, V2, P1] |
| **Compact Fireteams + board denial** | Brawler HRL / MSV2 sniper with useful partner(s), Druze KHD or E/M GL, Diggers/Denma, cheap REMs | Brawler Sixth Sense and low price buy respectable reactive threats; Fireteam bonuses and templates punish opponents for advancing. Prefer a few useful Duos/Haris to an expensive Core built only to amplify one average-BS gun. [V1, V2] |
| **TAG-led direct attack** | Scarface & Cordelia **or** independent Triphammer/Anaconda; engineer support, a Pathfinder or Hunzakut specialist, cheap orders | Heavy armor/AP guns answer targets the light Druze/Bulleteer weapons struggle to remove. Scarface's entire **76–80 point** composite package competes with specialists and order generators; budget for his failure, not just his peak output. [V1, V2, V3, P1] |

**Key asymmetry:** The sectorial has impressive *tools* but relatively few premium face-to-face gunfighters: expensive, one-wound Druze/Brawlers with BS12 can trade sideways well, but do not reliably bully elite TAGs or hard AROs. Use smoke, mines, pitchers, E/M, hacking, AP weapons, and mission angles to create favorable fights rather than treating every linked shooter as a main attack piece. [V1, P1]

### Units and interactions worth building around

- **Druze KHD (23/0) + Pitcher:** Good first hacker because it attacks enemy hackers and deploys the repeater network that enables the rest of the force; the HD (25/0.5) supplies non-killer hacking, so **KHD alone is not a Spotlight plan**. A Druze E/M grenade launcher (24/1) offers a different attack vector against high-value technological targets; spec-fire pressure costs SWC and Orders, so use it when direct attack is worse. [V1, P1]
- **Brawler HRL (15/1.5), hacker (16/0.5), MSV2 sniper (25/1.5):** HRL + native Sixth Sense is a cost-efficient deterrent; the hacker broadens repeater-zone defence; MSV2 has an active smoke-shooting niche but becomes a costly reactive target without good range, cover and lane selection. **Competing views:** V1's guest favors the cheap HRL; its host emphasizes the MSV2 MULTI sniper as an *active* smoke attacker, not a default exposed ARO model.
- **Valerya (19/0.5):** WIP14 HD, Pitcher and Total Control (+1B) make her a lean specialist for hacking and anti-TAG duty. **Counterview:** Druze HD/KHD or Brawler hacker can provide redundancy and other utility; Valerya is not an automatic include if the plan is neither hacking-heavy nor reliant on a Wildcard specialist. [V1, V2]
- **Hunzakut FO/repeater (19/0) or FO/D-Charges (15/0):** Infiltrating Camo midfield mission presence, deployable repeater / FO access and mines make them disproportionately important; most of the rest of this sectorial starts farther from objectives. Their Irregular Orders mean they are not a substitute for the Regular order pool. [V1, P1]
- **Saito, Yuan Yuan, Denma, Diggers:** Saito is a real independent close-attack/midfield threat; cheap Yuan Yuan bring smoke and flank pressure; Denma and Diggers threaten melee trades and can protect a team. **Trade-off:** too many Irregular/Impetuous troops leave too few Regular Orders to operate the network, fireteams, or TAG. [V1, P1]
- **Lieutenant security:** Cheap Brawler LT versus pricier Arslan LT is a real opportunity-cost decision. The Brawler is easier to hide; Arslan supplies a better equipped fighter and Disco Baller but becomes a tempting priority target. Táowù's Chain of Command option (21/0) is a separate insurance choice, not a requirement. [V1, P1]
- **Fiddler:** Strong independent Engineer/mobility/JackBot tool; **FTO option 1 is not Fireteam legal in Druze** despite its name. Monstruckers are cheaper but Irregular Engineers; Cordelia belongs to the mandatory Scarface composite. Match engineer spend to what actually needs repairing.

### TAGs and mechanized units — genuine alternatives and disagreement

| Unit | Best reason to take it | Best reason **not** to | Fireteam reality |
|---|---|---|---|
| **Scarface & Cordelia** (76–80/1.5 total) | Scarface brings ARM7/STR3, Tactical Awareness, ECM and AP HMG/AP Spitfire or Mk12+HRL; Cordelia is an included Engineer; Turtlemek can work on objectives. Strongest overall *supported* TAG pressure choice for many players. [V1, V2, V3] | The mandatory package ties up about a quarter of a 300-point list; Cordelia may not be able to repair him if his assault is overextended. V1's guest would often skip it; V1's host enthusiastically takes it, and V3 rates its NA2 role positively despite average head-on odds against premium TAGs. | Can seed a **Mechanized Duo**, not a TAG Haris. Scarface & Cordelia remain one composite roster choice even though the chart has separate member rows. |
| **Triphammer** (48–53 / 0–1.5) | Cheaper independent TAG with Tactical Awareness, Booty, transmutation and a Turtlemek specialist; AP Spitfire for attacking armor or 0-SWC short/mid-range profiles if preserving SWC. Battle-ravaged state may retain practical board value. [V1, V3] | BS13 with few quality-modifier advantages, BTS3, and difficult matchups into superior shooting TAGs; its low cost is not itself a win condition. V1 is skeptical versus Scarface; V3 sees real value over Anaconda. | **Cannot start a Mechanized Duo by itself**; must have Anaconda or Scarface among its members. May be fielded unlinked. |
| **Anaconda** (59/1.5) | ARM7/BTS6 and Tactical Awareness; cheaper than the full Scarface composite, optional independent operator after escape, HMG or AP Spitfire; use when fitting the *specific* total-point footprint / range / BTS / scenario needs. | V1 and V3 both call it substantially outclassed: less effective armor cracking/dice than Scarface and less independent value than Triphammer; the operator does not compensate for losing the main TAG. This is a **strongly negative consensus**, not evidence it is illegal or impossible to use. | May seed a **Mechanized Duo**. No Mechanized Haris/Core in Druze. |

**Vehicle boundary:** The current Druze **standard roster contains no troop categorized VH**. Its explicit mobile motorcycle unit is **Motorized Bounty Hunter** (8–16 pts, Irregular/Impetuous), which can screen, threaten a flank or accompany a legal Fast Attack/Mechanized Duo. It is **LI with Motorcycle, not a VH**, and it **cannot** create a Fast Attack Duo without a Bulleteer or a Mechanized Duo without Anaconda/Scarface. Avoid importing actual Vehicle/TAG availability or Fireteam entitlements from Qapu Khalqi, Ikari, PanO, StarCo, etc.

### REMs — what the investment buys

| REM | When it earns its slot | Important limitation / contrary view |
|---|---|---|
| **Pathfinder** (14; Tactical Awareness 17) | AVA3, FO + Sensor + Repeater: mobile objectives, Discover/Camo management, direct target acquisition. Tactical Awareness makes one Pathfinder unusually order-efficient. [V1, V2, V4] | **Not Fireteam-linkable in Druze**. Its mobility/base still require a safe lane, and a fragile forward FO must not be the list's only specialist. |
| **Clipper Guided** (16/1.5) | A remote strike option after an actual valid target acquisition; rewards a deliberate Pitcher/FO/hacker shell. [V1, P1] | **NOT a Wildcard and NOT linkable.** It is **option 1**, *not* the FTO option. V1's December 2024 speakers mistakenly describe a linked Guided Clipper benefiting from Fireteam burst; do not copy that combo. |
| **Clipper FTO** (19/1.5) | **Option 5** can Wildcard into legal teams; its Missile Launcher (+1B) is a direct/ARO lane weapon rather than a Guided strike. | **No BS Attack (Guided)** on this option: a player cannot buy both the Guided profile and the FTO Wildcard benefits in one Clipper. |
| **Bulleteer** (19 shotgun / 22 Spitfire) | Mimetism (-6), Repeater, fast attacking; a **Fast Attack Duo of two Bulleteers** is a genuine gunfighting plan, as is Bulleteer + compatible Wildcard. EVO support can improve active shooting. [V1, V2] | Large bases impede cover and movement; conventional shotgun/Spitfire struggles into heavy ARM, even if hit odds are attractive. Opposing emphasis: V1 favors the duo when lanes suit it but warns not to overinvest in two bulky bases. |
| **Peacemaker** (23–27) | Forward Deployment (+20), Mimetism (-3), Repeater and synchronized AuxBot: layered heavy-flamethrower defence or short-range trading. At 24/0.5, **AuxBot_3B** has *Minelayer*, projecting a mine farther from the REM's position. [V1, V2, V4] | The REM itself is **not** the Minelayer. V1's host sees excellent layered denial while its guest had dropped Peacemakers at earlier price levels. Placement and order cost determine whether it outperforms another specialist. |
| **Sierra** (23 HMG / 18 Thunderbolt) | Total Reaction, 360° and EVO-supported shooting make a long-range reactive speed bump; **Thunderbolt saves SWC**, HMG offers a different range/coverage profile. [V1, V4] | A visible TR bot is removable by prepared opponents; consider reserving it as a late-game standing ARO piece rather than exposing it turn 1. |
| **Fugazi** (7) | Cheap Regular Order, Flash Pulse, Mimetism (-3), Repeater; supports the network while filling the pool. [V1, V2] | Alone it is harassment/coverage, not meaningful lethal defense. |
| **Kameel** (8 baggage/repeater; 14 EVO; 16 TR) | Baggage supports ammo economy on a Pitcher/deployable-heavy plan; EVO complements Bulleteer/Sierra and airborne plans; 8-point version is cheap backbone. [V1] | Extra Kameels and other S4/S5 models congest deployment and absorb slots; don't buy EVO without a concrete support target. |
| **Nasmat, Turtlemek, JackBot** | Nasmat extends its Engineer/Doctor's reach; Scarface/Triphammer's Turtlemek brings a specialist; Fiddler's JackBots create independent peripheral tactical reach. | These are Peripherals/composite states, **not extra independent Regular Orders**. Check the relevant parent profile and synchronization type. |

### Disagreements to preserve rather than average away

1. **Guided as central win condition vs optional tool:** WIP12 [P1] (N4) and V1's launch analysis strongly emphasize saturation of Pitchers and missile pressure; some players reject that plan as expensive/uninteractive/fragile, and the later N5.3 chart specifically kills V1's **linked Guided Clipper** assumption. Keep unlinked Guided as one lane, not a universal core.
2. **Scarface investment:** V1's host and the Concilium list-builder like durable AP pressure; V1's veteran Druze guest and WIP12 guest question mandatory Cordelia's cost and how badly the rest of the list thins out. V3 agrees Scarface has useful NA2 role yet notes he's not a premier TAG-vs-TAG duelist.
3. **Fireteam size:** A larger Druze/Brawler team can improve a specific HRL/sniper's performance, but paying multiple medium-infantry models to buff a single BS12 one-wound attacker creates a brittle point concentration. V1 prefers flexible Duos/Haris for many lists; other build styles still legitimately use a larger core when mission/lanes justify it.
4. **Long-range defence:** Cheap Brawler Sixth Sense HRL versus pricier MSV2 MULTI sniper, and Sierra HMG versus 0-SWC Thunderbolt, are *mission and range* selections, not one profile objectively replacing the other.
5. **Old cross-sectorial advice:** PanO's REM-specific support characters and Qapu Khalqi's own TAG/Fireteam permissions **do not transfer** to Druze. Use [V4, V5] for movement, exposure, and target-priority lessons only.

### Curated video / podcast sources and transcript status

**Direct Druze videos**
- **[V1] Infinity the Dante with Druze player Luke Henry, [Druze Bayram Security N5 Initial Reaction — Best Guided in N5???](https://www.youtube.com/watch?v=jmgABxVFU9U)** — **YouTube MCP transcript reviewed**. Best broad profile-by-profile discussion, Fireteam/Guided disagreements, TAG/REM cost-benefit and practical list ideas. **Launch-era / corrected Clipper error above**.
- **[V2] Concilium Watch, [Army Builder Briefing: Druze Bayram Security](https://www.youtube.com/watch?v=pJx--Qj7CQ4)** — **YouTube MCP transcript reviewed**. Best complement for actual packages: Peacemaker forward Repeater, Pathfinder specialists, cheap Fugazi, Valerya/Bulleteer synergy, Scarface all-comers build. Re-check old Army composition.
- **Fast Panda Gaming, [ITS17 Cutthroat: Druze vs Corregidor](https://www.youtube.com/watch?v=ypVn75PRiRs)** — **YouTube MCP transcript reviewed** as a practical battle report featuring multiple TAGs (including Scarface/Anaconda mentions) and repeal/repeater exchanges; use as *one game* rather than a unit ranking.
- **VaulSC, [Druze Bayram Security — The Review](https://www.youtube.com/watch?v=dCRn89I9PQM)** — transcript reviewed but **older edition**; useful for long-running weaknesses and historical opinions, **not N5.3 profiles or Fireteams**.

**Shared TAG / REM cross-faction videos**
- **[V3] Loss of Lieutenant, [Episode 142 — N5 TAG Tier List](https://www.youtube.com/watch?v=dZo_gQWQYSY)** — **YouTube and Podcast MCP transcripts reviewed**; especially Scarface ~2:20, Anaconda/Triphammer comparison ~2:27 (podcast timestamps, hh:mm). Useful *opposed views and tradeoffs*; not the latest Army revision.
- **[V4] Robert Shepherd, [N5 Faction Focus — PanOceania](https://www.youtube.com/watch?v=IqK-RwFt7fw)** — **YouTube MCP transcript reviewed**; shared Pathfinder, Sierra, Peacemaker/AuxBot tactical use. **PanO-only REM enhancements not available here**.
- **[V5] Infinity the Dante, [Qapu Khalqi Faction Focus — The Sky is Falling!](https://www.youtube.com/watch?v=z4kV-SFZ5Uw)** — **YouTube MCP transcript reviewed**; shared Scarface/Triphammer and TAG support comparisons; **QK Fireteam chart is different**.

**Podcasts**
- **[P1] WIP12, [E75 — Druze Bayram Security](https://open.spotify.com/episode/4hppzgYaNybZeMexaNaykO) (2022)** — **Podcast MCP transcript reviewed**. Guest Leomaris: Pitchers/repeater infrastructure (~03:40), Druze KHD (~04:30), Lieutenant/mission constraints and debate on Guided, Scarface cost debate (~30–40 min). **N4-era concepts only**; particularly do not copy old Fireteam bonuses or Guided combo assumptions.
- **[P2] Transmission Matrix, [Episode 13 — Druze Clues](https://open.spotify.com/episode/2zFIdjcX584qQ2hCpsLhHS) (2022)** — listed for Druze vs Ikari competitive/list-building comparison; **Podcast MCP returned no transcript**, so no specific strategy is attributed to its recording.
- **Loss of Lieutenant [Episode 142 — N5 TAG Tier List](https://open.spotify.com/episode/1h5CJfZC5zBPxdg66o7xIN) (2025)** — **Podcast MCP transcript reviewed**; supports [V3]'s Scarface versus Anaconda/Triphammer comparison.

Further community cross-check: [Corvus Belli forum N5 Druze discussion](https://forum.corvusbelli.com/threads/n5-druze.43292/). Treat reported wins and preferences as anecdotes, not rules or population-level win rates.

## Provenance

- Corvus Belli Army source revision: `7.26246.159`.
- Army data changed on: **2026-09-03**.
- Mirrored source commit: `6b79f39a3abbf5cd3d837fb9dc65e411fc35244b`.
- Source blob: `311c3b0d595ee220d4046b983b8dfb65dceb3b2c`.
- InfinityDB reference commit: `4e2662be3f43387fbae42b3790a711b3e98570c4`.
- Fireteam source: Army snapshot canonical `fireteamChart`, normalized using repository Fireteam conventions.
- Generated/verified: **2026-10-16**.

## N5.3 airborne / enemy-DZ profile and value choices (2026-10-23)

**Yuan Yuan Chain Rifle+Smoke6/0 (DA CC7/0)** is one of the whole game's best *pure points-value* rear disruptors: an **Irregular/Impetuous** 6pt model can cost enemy multiple Orders even if it kills no one. Druze's pinned profile explicitly lists **Combat Jump(PH11) or ordinary Parachutist**, so unsupported landing succeeds **55%** and side-edge entry avoids a roll. **Druze Bashi Bazouk** also lists **Combat Jump(PH11)**, unlike Qapu/Dahshat Bashi profiles that list normal Parachutist; don't generalize a same-name model. **Saito Tōgan Hidden/Infiltration33/0** is a much stronger single-hit assassin with greater points at risk. The objective is removing support capability, not necessarily the expensive ARO.

[Cross-game N5.3 airborne/rear-strike apex-value and landing-risk tiers](../../notes/list-building/airborne-and-enemy-dz-attackers-apex-value.md). **Use this roster and canonical Fireteam chart for exact legality.**

## N5.3 cheap warband, template and CC trade decisions

**Yuan Yuan Chain Rifle+Smoke6/0 / DA CC7/0** is a near-bottom priced **Irregular+Impetuous Combat Jump(PH11) or ordinary Parachutist** trade: **55% unsupported jump**, so prefer an open side edge if possible; 6pt may be valuable for just taxing two defending Orders. **Libertos SMG+Chain-colt8/0** has *FD+20/one-use Camo/Dogged*, an alternative safer midfield angle. **Motorized Bounty Hunter8–9** cheap high-speed Riotstopper/Chain-colt. **Saito Togan33 Hidden/EXP** high ceiling, but not an Irregular 6pt warband. **Bashi Bazouk** is Irregular holo/AD, distinct from Yuan; Druze version permits Combat Jump, unlike Qapu/Dahshat.

[Whole-game cheap-trading apex/value, specific targets and Lt/CoC notes](../../notes/list-building/warbands-and-cheap-trading-units-apex-value.md). Current unit loadouts and canonical Fireteam chart remain authoritative.

## TAG tactical cross-reference (2026-10-23)

**Triphammer** is usually the more efficient high-pressure option (budget profiles + TacAware), while **Anaconda** gives AP Spitfire/Thunderbolt and an operator fallback. **Disagreement:** the 2025 TAG tier-list judges Anaconda extremely poorly, but Druze can value a specific role when other gun choices are limited. Both require deliberate Engineer/hacking and mission support; don't assume its TAG Fireteam members from other mercenary factions.

For the two-tier **apex/points-value** comparison, TAG counterplay, matchup matrix and direct transcript sources: [N5.3 TAG field guide](../../notes/list-building/tags.md). Treat current profiles, points/SWC and canonical Fireteam data above as authoritative.

## Hacker and KHD tactical cross-reference (2026-10-23)

**Druze KHD+Pitcher 23/0** is a 0-SWC Hacker-hunter/scorer with native ranged network projection; **Druze HD+Pitcher 25/0.5** instead threatens *ordinary* HI/TAG via Oblivion/Carbonite. **Valerya Gromoz WIP14 HD+Total Control(+1B) 19/0.5** is extraordinarily good value for anti-TAG possession and another Pitcher. **Brawler HD16/0.5** provides cheap redundant Spotlight, while **Kameel EVO14/0.5** only pays if supportware has beneficiaries. **Why:** Druze's own linked X-Visor Pitcher/carrier and multiple Repeaters can make two complementary hackers much stronger than either alone. Beware SWC spent on a guided missile package before buying a true high-Burst attack gun.

See the [cross-game apex/value Hacker/KHD tier guide](../../notes/list-building/hackers-and-killer-hackers.md). **The sectorial's current profiles, AVA and canonical Fireteam chart above remain authoritative; device upgrades are profile-specific.**


## Cheerleader / Order-generation tactical cross-reference (2026-10-23)

The N5.3 [cheerleader/order-generator apex and value guide](../../notes/list-building/cheerleaders-and-order-generators.md) contrasts Orders-per-point, passive utility, matchup dependence, and opposing transcript opinions. **Use this roster for legal AVA, exact profile costs, Training and Fireteam restrictions.**

- 7pt Fugazi — Flash Pulse/Mimetism/Repeater Regular bot: usually prime passive fuel, with S3 footprint and AVA caveats.
- Authorized Bounty Hunters — a cheap Regular, Booty-enabled guard or trade body if the chosen profile is legal; compare its base cost and Team commitment.
- Warcor — a 3pt Irregular Flash ARO speedbump, not a transferable pool Order without actual conversion.
- Peacemaker — pricier Regular REM/peripheral defensive coverage and network projection; not an economical pure cheerleader.
- Pathfinder — more points than 7pt Flashbot but real Sensor/FO/scoring utility; an upgrade only if the mission/network uses it.

**Decision:** first buy enough protected *transferable* Regular Orders for the actual Combat Group attacker/scoring plan, then pay for genuine role compression. Irregular/Impetuous, LT, Tactical Awareness and Peripheral bodies are different resources. Account for a packed S3/S4 deployment zone and mandatory Fireteam members.


## ARO apex/value cross-reference (2026-10-23)

See [Best ARO Units in N5.3 — apex, cost-value, Hidden Deployment, reactive traps, opposed podcast views](../../notes/list-building/aro-units-apex-and-value.md). **Only the legal roster above** establishes options, exact costs/AVA, upgrades and Fireteam permissions in this army.

- **Authorized Bounty Hunter cheap body** — small-base template/Panzerfaust or close ARO if profile equipped, useful only in legal team/roster
- **Ninja hidden/camo** — anti-impersonation or corridor trap if positioned near scoring; may be more valuable unrevealed for own active turn
- **Sierra Thunderbolt TR** — 18pt/0SWC where authorized, all-arc cheap regular ARO and Engineer-restorable lane
- **Fugazi Flashbot** — 7pt Regular cheap Flash/Repeater tax; not substitute for anti-armor hard ARO
- **Druze Fireteam weapon/EM** — durable midlane or utility link option where current source permits; multiple roles beat pure unused sniper SWC

**List test:** a strong ARO consumes enemy Orders by forcing Smoke, rerouting, poor range, discoveries or risky trades. A robust list normally prefers *serial, different* defenders—a cheap visible or marker/template screen, a covered second gate, and a preserved attack/scoring unit—rather than two adjacent visible snipers. Plan for opponent pie-slicing, AD, anti-camo, hacking and recovery; evaluate whether extra SWC is better spent on mission attackers.

## Doctor / Engineer / Recovery cross-reference (2026-10-23)

**Monstrucker12 Engineer (Irregular)** is cheap anti-immobilization/STR rescue for **Anaconda, Triphammer and other technology**, if its Irregular-Order economy and path can actually reach. **Fiddler Engineer** adds mobile combat and objective tools at a higher price; a **Nasmat3** remote support net only applies when attached to a legal Controller. **Scarface & Cordelia** includes the Engineer in a composite TAG purchase. With mostly expendable VITA troopers, a cheap Paramedic or Speedball may outperform buying another premium Doctor. [Recovery support tiers and real success probabilities](../../notes/list-building/doctors-engineers-and-recovery-apex-value.md).

## Close-combat assassins and counter-CC — N5.3 (2026-10-23)

**Druze** is a hacking/Repeater/mine/adhesive and short-range-ambush package, **not** a roster with a 29pt hidden Monofilament specialist. **Libertos8 Camo(1 use), FD+20 and Dogged** is a low-cost *template/trade* unit at **CC16**, not a true assassination duelist. **Scarface** brings **CC22 Berserk(+3)** but as part of a 76–80pt **TAG+Cordelia** composite, with very different melee risk and objective cost. Disable an enemy CC monster using Valerya hacking/E/M, mines and Brawlers before seeking physical contact. [N5.3 melee apex/value and counter-CC guide](../../notes/list-building/dedicated-close-combat-assassins-apex-value.md).

## Anti-TAG / Anti-HI without hacking — N5.3 (2026-10-23)

**Táowù19 E/Marat** is the most economical verified direct *electronic shutdown* in the Druze pinned roster; **Druze21 Panzerfaust** offers affordable AP+EXP lane denial. **Libertos8 Camo+Dogged** is a short-range trade screen, *not* inherently anti-TAG ammo. **Scarface & Cordelia76 AP HMG/Panzerfaust** or **Triphammer48 Panzerfaust(+1B)** are higher-cost TAG categories. Focus an enemy TAG's Engineer/Orders after disabled, rather than overpaying for a second high-price gun without attack modifiers. [Non-hacking anti-armor apex/value, E/M and AP+EXP comparison](../../notes/list-building/anti-tag-anti-heavy-infantry-non-hacking-apex-value.md).

## N5.3 objective holding, zone domination & carried-objective choices

**Brawler Engineer19/0 / Doctor19/0**, each Sixth Sense ARM2, is inexpensive *actual Specialist* for box pickup/protected backline; **Druze HD+Pitcher25/.5** carries a viable hacking counter-layer where chosen but *Druze gunfighter without specialist option is not a box carrier*. **Anaconda59/1.5** (STR3/ARM7/Transmutation) provides zone VP + late-game Specialist Operator possibility **only after valid Escape System state**; not a 59pt ordinary Specialist TAG. **Scarface STR3 TAG + Cordelia Engineer** buys expensive robust repairs and quadrant weight in a **bundled separate-body purchase**, not free independent Orders beyond its printed relation. **Fiddler Engineer36/0 + 1 JackBot or43/0 +2** forces two approach angles but controller and synchronized bots don't generate multiple pooled Orders; **29/0 FTO has no JackBot**. **Opposing:** normal Druze/Brawler Fireteam can lock one room; extra independent 19pt Engineer in total cover may survive to score more reliably than exposed TAG.

[Cross-game holding and carrier apex/value, scenario rules and transcript disagreements](../../notes/list-building/objective-holding-zone-domination-and-carriers-apex-value.md). Use pinned local roster/Fireteam chart.

## Anti-Tech — enemy visors, Mimetism, markers and Impersonation (2026-10-23)

**Pathfinder FO/Sensor14/0 (TacAware17/0)** is the inexpensive **Camo/Hidden** search, scoring, and Repeater piece; it needs to move into ZoC rather than detecting across the table. **Brawler MSV2 MULTI Sniper25/1.5** is for *shooting* revealed Mimetism and contesting ordinary Smoke, often with useful Fireteam support. **Arslan Disco Baller35/0** changes the problem: **Eclipse bypasses enemy MSV/Marksmanship** to deliver a linked scorer without directly defeating the gun. **Choice:** buy Sensor when markers block the mission; pay for Brawler when an ARO must die; Eclipse when the mission can score without that kill. A second expensive sniper is poor value if the opponent can project White Noise.

[Whole-game anti-tech N5.3 apex/value, matchups and opposing MCP transcripts](../../notes/list-building/anti-tech-msv-mimetism-camo-impersonation-apex-value.md).

## N5.3 peripheral / synchronized / multi-body apex-value update

**Fiddler Engineer36/0 + one JackBot; 43/0 + two JackBots** makes 2–3 simultaneous Synchronized bodies, with Vulkan Shotgun/Explode bots and a WIP14 Engineer/Drop Bears Controller; **29/0 FTO has no JackBot** and in Druze **has NO Fireteam access despite the label**. W1+NWI parent remains the risk and must keep Coherency. **Anaconda59/1.5 + Operator** is an Escape-System alternate state, *not two full attackers active from deployment*. **Scarface+Cordelia** is composite TAG plus engineer bought together, not a single synchronous attack pack. **Druze/Brawler Doctors/Engineers + Nasmat3/0** delegate repair to a different flank (1 patient/Order, max one active Servant), not a second pooled Regular Order. **Counter:** 19pt Brawler Engineer + Nasmat gives more real recovery per point than 43pt Fiddler+two bots if enemy isn't exposing flammable close-range targets; Fiddler wins where two independent ARO angles can be threatened on one Order.

[N5.3 Peripheral & Multi-Body apex/value tiers and transcript debates](../../notes/list-building/peripheral-synchronized-multibody-apex-value.md). Pinned source roster/Fireteam restrictions remain authoritative.

## Mission performance — battle-report evidence (2026-11-01)

| Mission(s) | Tested composition / scoring mechanism | Evidence |
|---|---|---|
| **Evacuation / toolbox delivery** | Scarface+Cordelia, Valerya Gromoz/Brawler Hacker, Monstrucker/Fiddler and Bashi/fast objective workers can keep both electronics and civilians moving. | [#202](../../notes/battle-reports/201-210-n5-battle-report-tactical-analysis.md) |
| **Crossing Lines / altered one-TAG format** | Scarface/Fiddler/Kunai/Brawler/Pitcher screened a Cutter; projected Druze 8–0 is **not a full standard ITS result**. | [#226](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) |
| **Cutthroat counterexample** | Anaconda+Scarface+Druze hacker/warband struggled into Corregidor double Gecko/Jazz/Intruder 6–3; spent Orders on unrewarding trades. | [#186](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md) |

**Limits:** #226 has special one-combat-group/one-TAG and forward-deployment restrictions plus unresolved LoF disagreement. No general Druze mission tier inferred. Game-era qualitative evidence, not a win-rate or current Fireteam claim. [Full mission evidence audit](../../notes/battle-reports/cross-report-mission-performance-by-sectorial.md).

## Counterplay — observed N5 battle-report responses (2026-11-02)

| Threat / target | Observed response and limitation | Battle reports |
|---|---|---|
| **Against Cutter / elite linked ARO** | Scarface + Cordelia, Kunai sniper, Brawler MSV and KHD/Pitcher formed layered trap that eliminated exposed Cutter in special-format Crossing Lines; *projected* 8–0, disputed LoF. | [#226](../../notes/battle-reports/221-230-n5-battle-report-tactical-analysis.md) |
| **Counter heavy gun resilience** | Druze Anaconda + Scarface shooting and E/M tools were held off by Corregidor double Gecko, Intruder and Jazz; survive/hack cover instead of repeating failing TAG trade. | [#186](../../notes/battle-reports/181-190-n5-battle-report-tactical-analysis.md) |
| **Forward hacker delivery** | Valerya Gromoz/Monstrucker with Scarface & Bashi Bayouk offer mission route while big TAG opens fire; press CivVac objectives rather than just target enemy heavy. | [#202](../../notes/battle-reports/201-210-n5-battle-report-tactical-analysis.md) |

**Limit:** #226 is one-group/one-TAG with special deployment and projected score, therefore not a clean standard ITS hard-counter example. Game-era tactical evidence, not current N5.3 profile/Fireteam or faction win-rate claims. [Full cross-report counterplay analysis](../../notes/battle-reports/n5-cross-report-counterplay-tags-hi-hacking-camo-impersonators-fireteams.md).

---

## Must-have / Go-to / Avoid — source-backed recommendations (2026)

Dated source-backed tactical preferences and miniature purchasing priorities; opinions do not override N5.3 roster, profile or Fireteam data above.

**Original audit title:** NA2 mercenary sectorials — Must-have / Go-to / Avoid (N5.3)

**Audit date:** 25 October 2026. **Scope:** Druze Bayram Security, Ikari Company, StarCo Free Company of the Star, Dahshat Company, White Company. This companion to the other faction selection audits in this folder evaluates competitive **standard 300-point N5.3** lists. It does not import Reinforcement, optional Spec-Ops/Team-Ops, or a neighboring faction's Fireteam permissions.

**Authority order:** The five repository-native N5.3 sectorial references linked below are authoritative for available troops, particular profiles, AVA, points/SWC, and Fireteams (Army data 7.26246.159, 3 September 2026, verified 16 October). YouTube/podcast transcripts are evidence for **a speaker's opinion**, not a measured tournament inclusion rate or a guarantee of efficiency. Several sources predate N5.3; their strategic observations must be reconciled with the pinned roster. In particular, N5 fireteam changes invalidate some older linked Guided claims.

**Labels used here:**
- **Must / near-must:** An actual presenter's explicit almost-every-list recommendation, or a defensible near-universal list-building package. Near-must does **not** mean compulsory in every mission or list style.
- **Go-to:** Efficient, consistently defensible use of points, SWC, Order slots and a defined tactical job. The alternatives are often mutually exclusive.
- **Avoid / never take:** An **explicit reviewer rejection**, or a specific profile or construction displaced in its intended role by a better same-roster investment. Mark as **contested/conditional** when any credible niche or dissent exists. Do not invent categorical bans when only an older negative opinion is available.
- **Evidence:** **Direct** = explicit recommendation/rejection in a transcript; **Corroborated** = source rationale plus previously transcript-audited repository guide; **Contested** = meaningful opposing speaker's interpretation; **Edition-limited** = interpretation of pre-current Army data.

### Quick comparison

| Sectorial | Most defensible must / near-must | Reliable go-to choices | Strongest sourced avoid | Absolute never-take? |
|---|---|---|---|---|
| **Druze** | Druze **KHD + Pitcher** (direct repeated default) | Brawler HRL, Hunzakut FO, Valerya, Yuan Yuan, Digger, Scarface or Bulleteers | **Anaconda as default TAG** vs Scarface/Triphammer; ordinary Druze HMG value | No: Anaconda has a scenario/total-cost niche |
| **Ikari** | No single compulsory unit; **cheap Keisotsu regular-order base** and **Wú Míng AP HMG** are most convincing defaults | Motorized Yojimbo, Yuan Yuan/Desperado, Tankō, Armand, Druze KHD, Karakuri/Pathfinder | **Security Chief Arslan** as value pick (explicit rejection) | No |
| **StarCo** | **Al Hawwa' KHD**, **Irmandinho** (direct auto-take claims); **Knauf FTO + Uhahu** as a standout package | Brawler/Digger PMC, Bandit Minelayer, Hellcat Paramedic, Mobile Brigada LT, Riot Grrls/Avicenna | **Alguacil premium guns**; **unsupported TAG investment** (Anaconda itself contested) | No |
| **Dahshat** | **Mimetism(-3) Libertos** (direct strong 9-point profile default) | Hunzakut, McMurrough, Zúyŏng + Rui Shi, Valerya, Zhēnchá, Maghariba | Redundant **Al Fasid HMG** or ordinary **Ghulam HMG as main attack** | No |
| **White Company** | No proven single must; **Hǎidào's multi-profile Wildcard role** is a near-default toolbox | Hawkwood K1, Karhu/Kaplan, Laxmee, Varangian/Shona, Guiláng, Tiger, Peacemaker/Sierra | **Fusilier SWC guns as premium shooters**; niche Longarms/Wild Bill | No |

### 1. Druze Bayram Security

**Current profiles and Fireteams:** [Druze N5.3 sectorial reference](druze.md). **Primary direct media:** [D1: Infinity the Dante with experienced Druze player Luke Henry, Druze N5 Initial Reaction](https://www.youtube.com/watch?v=jmgABxVFU9U) (N5 launch, YouTube transcript reviewed); [D2: WIP12 E75, Druze Bayram Security, guest Leomaris](https://open.spotify.com/episode/4hppzgYaNybZeMexaNaykO) (2022/N4, podcast transcript reviewed); [D3: Concilium Watch, Army Builder Briefing Druze](https://www.youtube.com/watch?v=pJx--Qj7CQ4) (previously transcript-reviewed; edition-limited). [Existing Druze N5.3 tactical research](druze.md#tactical-research--druze-bayram-security-reviewed-2026-10-23) preserves source disagreement.

#### Must / near-must

- **Druze Killer Hacker + Pitcher, 23/0 — Direct [D2], reinforced by [D1].** The WIP12 guest explicitly identifies the KHD as the single closest Druze auto-include; Luke Henry says the profile was in every one of his N4 lists and sees that continuing. **Why:** X-Visor lets Pitchers project into deep lanes, KHD removes enemy hackers and Warhorse helps survivability, while the trooper also performs specialist work. **Exception:** a deliberately non-network direct-gun/TAG build. **Important:** KHD does **not** supply ordinary Spotlight; partner an HD, FO or Valerya if using Guided.
- **Not a compulsory guided missile battery.** The cheap network often earns its place even when a Clipper is omitted. [D1,D2] advocate missile potential; the current **Guided Clipper is unlinked**, while the distinct FTO option is a direct Missile Launcher (+1B), **not Guided**. Never repeat early N5 linked-Guided-special-die claims.

#### Go-to

| Unit/profile | Why it is good | Why not universal | Evidence |
|---|---|---|---|
| **Brawler HRL, 15/1.5** | Sixth Sense, long-range area denial and cheap Fireteam ARO; very low point outlay | Uses SWC; MSV2 sniper trades to a different smoke-shooting job | D1 Direct |
| **Brawler Sixth Sense hacker, 16/0.5 / MSV2 MULTI sniper, 25/1.5** | Additional repeater defense, or active smoke-assisted visor shooting | WIP12/BS12 and one wound cannot replace premium attack models | D1,D2 |
| **Hunzakut FO 15/0 or 19/0 repeater** | Camo + Infiltration + FO, optional deployed network; solves weak starting midfield | Irregular Order; do not starve your regular gun/link pool | D1,D2 |
| **Valerya Gromoz, 19/0.5** | WIP14 HD, Pitcher, Total Control (+1B), Wildcard | Other ordinary hackers/FO may already cover the intended network | D1,D3 |
| **Yuan Yuan, Diggers/Denma** | Cheap smoke, close-assault or corner trades, protects medium-infantry links | Irregular/Impetuous pressure; not every model needed in one list | D1,D2 |
| **Bulleteer Spitfire or shotgun / Peacemaker Auxbot** | Mimetism(-6) speed shooting, or FD+20 repeater/templating denial | Large base, hacking exposure, and soft STR1; Bulleteer often needs EVO plan | D1,D3 |
| **Scarface + Cordelia** | AP weapon, ARM/STR and bundled Engineer for heavy armor matchups | **76–80 pts for the entire mandatory composite**, not the isolated TAG chassis; aggressive moves can leave Cordelia out of repair range | D1,D3; opposing opinions |

#### Avoid / never-take candidates

- **Anaconda as a default TAG — Direct strong rejection [D1]; not a mathematical ban.** Both presenters call it poor head-to-head value relative to **Scarface + Cordelia**, and the surviving Operator is not sufficient to close that gap in their view. It can still fill a **59-point independent TAG/BTS or Mechanized Duo** requirement that Scarface's complete composite cannot fit. Mark **strong avoid as default**, not categorically illegal/useless.
- **Ordinary Druze HMG as primary investment — Direct/Corroborated [D1,D2].** Pay near 30 points and SWC for a BS12 one-wound gun that often needs further Fireteam investment; Scarface, linked Bulleteer, Armand or a specialist-heavy setup covers important objectives more efficiently. **Exception:** a compact existing Druze link where the HMG is a useful incremental gun, not an expensive list centerpiece.
- **Arslan LT as cost-neutral substitute for Brawler LT — Conditional [D1,D2].** Higher quality/command options come with conspicuous points and exposure. Can be worthwhile for a specific aggressive LT plan; not supported as a universal hard avoid.
- **Overbuilt 4–5 medium-infantry Core solely to improve a mediocre gun — source-supported construction warning [D1].** Compact Duos/Haris give less single-point-of-failure risk; larger defensive teams remain a legitimate scenario choice.

### Cross-sectorial ranking principles / edition checks

1. **A “must” is a reported list-building default, not tournament telemetry.** Most explicit Druze/StarCo/Dahshat endorsements are a named player's preferences; there is no verified representative inclusion-rate database here.
2. **Do not call every TAG “never take.”** Druze Anaconda has strongly negative direct testimony, whereas **StarCo Anaconda gets a persuasive later rehabilitation in a supported Haris**, and WhiteCo uses a different Kaplan Duo. It is the *same chassis with different team architecture*. The Triphammer's 0-SWC entry can also be right even if it loses raw shootout comparisons.
3. **Do not conflate FTO label and permission:** Druze Guided Clipper differs from Fireteam FTO direct ML; Ikari Guided Clipper similarly does not link; WhiteCo Clipper FTO has no Fireteam row at all; StarCo Stempler FTO likewise has no current StarCo chart row. Always use the exact current Fireteam chart and profile option.
4. **Irregular versus Regular economy is decisive:** Irregular smoke/assault excels individually in Ikari, StarCo and Dahshat, but 15 slots and too few pooled Orders can make even a roster of efficient units dysfunctional. The **Regular** cheap Keisotsu, Fusiliers, Fugazi/Fanous/Transductor and specialist options have systemic value.
5. **Mission scoring and delivery beat theoretical damage:** Druze/Dahshat Hunzakut, Ikari Karakuri/Pathfinder, StarCo Al Hawwa'/Hellcat and WhiteCo Guiláng/Tiger change whether a gun-heavy list can reach a console on time.
6. **No illegal legacy data:** Current N5.3 Army references override early N5/N4 transcripts: old StarCo Alguacil LT SWC tax, old N4 Dahshat Zúyŏng LT, imported Karakuri Fireteams, early linked-Guided Clipper assumptions and other-faction TAG/REM permissions are not reliable.

### Source coverage and limitations

- **Direct full/partial transcripts checked in the immediate research:** Druze N5 Dante, WIP12 Druze E75; StarCo N5 Dante, Loss of Lieutenant E158 StarCo section; WIP12 Ikari E191 sections, Dahshat E165 Libertos sections; WhiteCo N5 Robert Shepherd and tournament report. Remaining linked recordings were **already transcript reviewed in the corresponding existing GitHub tactical files**; do not portray every transcript as newly reviewed in this commit.
- **N4-era sources:** Druze WIP12 E75 (2022), Dahshat WIP12 E165/E166 (2024), WhiteCo WIP12 E160 (2024), Ikari IGL E163 (2024). Their exact points, team bonuses, and equipment are not current evidence. The N5.3 sectorial files take priority for such facts.
- **Dahshat N5 coverage is comparatively thin:** one substantive current N5 battle report plus cross-faction unit reviews; especially avoid inventing consensus “never take” choices. **WhiteCo tournament footage** demonstrates actual successful packages but some event formats/rules and mission requirements differ from standard play.
- **Contrary opinions intentionally retained:** Ikari Daiyōkai/Al Fasid vs cheap Wú Míng; Druze Scarface vs cheaper direct solutions; StarCo Anaconda before/after later podcast; Dahshat Maghariba vs discount swarm; WhiteCo Guiláng vs Nøkken and K2 vs heavier support.

### Whole-unit purchasing audit — can I omit an entire miniature? (2026-10-30)

This section is intentionally **sectorial-specific**: buying the same Anaconda sculpt for *Druze* versus *StarCo* gives materially different Fireteam/support access. **Skip by default** = low purchasing priority in mainstream 300pt builds, **not** a proven prohibition on every list.

| Sectorial | Entire model/unit to defer | Why / decisive exception |
|---|---|---|
| **Druze Bayram Security — Anaconda** | **Skip by default — strong single-source-pair negative** | [D1] presenters favor **Scarface + Cordelia** as the efficient TAG/repair purchase. Anaconda remains valid as a **59pt standalone/Mechanized Duo** role that Scarface's full package cannot duplicate. Do not transfer this verdict to StarCo. |
| **Ikari — Security Chief Arslan (35pt)** | **Skip by default for normal attack/LT plans** | [I1] Copper directly rates his cost inefficient against **Keisotsu/Brawler LT** and **Wú Míng AP HMG** covering those jobs. Buy if specifically leveraging **MSV1, Warhorse, NWI or command/team role**. Not a dismissal of Druze Shock Teams. |
| **StarCo — Anaconda / Triphammer** | **Defer blind standalone TAG purchases; no entire-unit hard skip** | [S1] condemns both; later [S2] argues for Anaconda's **Brawler Engineer + Digger Armored Haris**, while Triphammer buys **0 SWC**. Purchasing one for a supported role can be rational. |
| **Dahshat** | **No source-backed whole-model avoid** | Al Fasid and Ghulam **generic guns** duplicate other attacks, but retain real support/defensive profiles and there is too little current direct evidence to blacklist units. |
| **White Company — Chaksa Longarms** | **Defer as first main gun; low confidence** | [W1,W3] prefer K2, Nisse and ORC for the usual ranged role, but Longarms' legal Duo/Haris and unusual weaponry still create distinct angles. Anaconda can use a Kaplan Duo, unlike Druze/StarCo constructions. |

**Important:** The ordinary Druze HMG, Alguacil SWC, Fusilier SWC, Clockmaker-without-repair-target and Hawkwood CoC criticisms are **profile/usage warnings**, not full model skips. See [all-armies buying shortlist](../../notes/factions/model-purchase-avoid-summary-2026.md).

### Worst-value, rare-use and proxy-first mercenary miniature purchases (2026-10-30)

**Scope and evidence.** This is a **miniature-buying audit**, not a re-ranking of every profile. It covers each current NA2 army separately: [Druze Bayram Security](druze.md), [Ikari Company](../na2/ikari-company.md), [StarCo](starco-free-company-of-the-star.md), [Dahshat Company](../na2/dahshat-company.md), and [White Company](../na2/white-company.md). References are the **pinned N5.3, September 2026 Army 7.26246.159 rosters and Fireteam charts**. **Direct negative** means the speaker actually criticized that use in the earlier [transcript-backed source register](#source-coverage-and-limitations). **Proxy first**, **conditional whole-model deferral**, and **extra-copy defer** are *reasoned buying suggestions*, not claims the media said those literal words. **Rare** means unusual in reviewed all-comers constructions, *not a measured tournament inclusion rate*. When the existing podcast reviews predate current Army, the **current printed profiles** govern. No all-profile universally unplayable unit is established.

**Four distinctions matter:** a **weak gun profile** can belong to a very good unit; a **conditional whole-model deferral** is not a zero-win-rate label; a **rare specialized peripheral/character** can deserve a proxy even when genuinely excellent; and **AVA / alternate weapon sculpts** alone never create a shopping need. Also **one bought model can be reused across different legal sectorials**, not fielded twice simultaneously. No current complete inventory of the five mercenary armies was found at the expected inventory paths; the cross-army proxy examples below **do not assume ownership** of NA2-exclusive models.

#### 1. Druze Bayram Security — strongest all-profile deferral: Anaconda for a default TAG

| Unit / option / purchase | Why it may not earn its model price; legitimate exception | Buy / proxy decision |
|---|---|---|
| **Anaconda59/1.5** as the *first default Druze TAG* | **Direct negative — [Infinity the Dante, experienced Druze player Luke Henry](https://www.youtube.com/watch?v=jmgABxVFU9U)**: prefers **Scarface + Cordelia composite76–80/1.5** for a durable AP attack *with bundled Engineer*. This is a **total 76–80pt multi-body choice**, not a straight 59pt comparison. Anaconda has **Tactical Awareness, Warhorse, AP Immunity, an Escape-System Operator Specialist** and a legitimate **Mechanized team**; its 59pt standalone economy is real. | **Skip the dedicated Anaconda by default / borrow or proxy a correct S7 TAG**, then buy if your own **59pt Mechanized/solo** architecture repeatedly works. **Do not import StarCo's stronger Armored Haris rehabilitation into Druze**. If you already own an Anaconda for StarCo/WhiteCo, reuse it rather than buying another. |
| **Ordinary Druze HMG28/1.5** as the marquee gun | **Direct criticism in [D1](https://www.youtube.com/watch?v=jmgABxVFU9U) and [WIP12 Druze](https://open.spotify.com/episode/4hppzgYaNybZeMexaNaykO)**: BS12/1W SWC gun needs a team and more Orders while **Scarface, Bulleteer, Armand** may present stronger primary attacks. Druze **KHD Pitcher23/0**, ordinary **HD Pitcher25/.5**, and Paramedic22 have more reliable specialist jobs. | **Avoid HMG-as-standalone-investment, not Druze Shock Teams**. **Proxy HMG sculpt** until a particular existing link wants it; prioritize a physical **KHD/Pitcher Druze** first. No need to buy every Druze rifle/GL/ML/sniper sculpt. |
| **Arslan35/0 as automatic Lieutenant/cheap link leader** | **Corroborated conditional warning:** the 35pt BS13/MSV1/Disco/NWI package is much more expensive than a cheap Brawler/Druze LT; the real premium is only justified if **linked MSV1 gun, Warhorse, command/Disco** actually solve an issue. **Do not transfer Ikari's direct Arslan criticism as a categorical Druze ban.** | **Proxy first**, especially if only buying an AVA1 character to satisfy a link photo. Buy for the **actual Wildcard/Disco/LT** role, not for the ordinary Order. |
| **Additional Kunai sniper, Saito, Armand, Bashi Bazouk, Aïda non-FTO** bought to cover every uncommon sneaky attack | **Inference:** **Hunzakut FO15/0** handles economical Camo/Infiltration scoring (Irregular); **Kunai Hidden sniper28/1.5**, **Saito Hidden Smoke+EXP33**, **Armand MSV1/Mimetism(-6) sniper**, **Bashi Bazouk Holoprojector Parachutist**, and **Aïda Decoy/Viral Minelayer24/.5** all do *different* missions. They are **not recorded universally bad**, but paying for all as redundant first specialist slots is poor collection economy. | **Proxy-test the particular rare assassin, alternate sniper or parachutist**, and buy only one whose specialized route recurs. **Aïda FTO21/0** is a distinct team-eligible alternative; don't treat its FTO membership as applying to non-FTO24. |
| **Full Fiddler+JackBot(s)** when the buying goal is only an Engineer or linked Wildcard | **Current Druze profile trap**: **Fiddler FTO29** has **no Druze Fireteam access** despite FTO name; independent **Fiddler36 with one JackBot** and **43 with two JackBots** deploy **separate S1 synchronized** peripherals. A simple **Monstrucker Engineer/other repair** is often enough. Fiddler remains a strong fast specialist and can be worth all three bodies. | **Proxy the complete selected multi-body package** first. **Do not buy FTO hoping to join a Druze Core**; do not buy two JackBots unless selecting their actual profile. |
| **Clipper Guided16/1.5 and FTO19/1.5** bought for the same imaginary linked Guided plan | **Hard current profile distinction**: **Guided ML16 is not linked**; **FTO direct ML(+1B)19 is link-eligible but lacks Guided**. **Druze KHD Pitcher does not cast standard Spotlight**, so a real **Valerya/ordinary HD/FO** target chain must be budgeted to exploit Guided. | **Avoid buying an extra Clipper body for an illegal hybrid profile**. **Proxy the *chosen* ML chassis**, buy a second only if a list can physically field multiple distinct units (here Clipper **AVA1**, so no simultaneous second Clipper in standard Druze). |
| **Full Kameel/Pathfinder/Sierra/Bulleteer/Peacemaker REM collection and redundant large shooters** | **Inference:** **Fugazi7** cheap Regular-order Repeater/Flash Pulse; **Kameel Baggage**, **Pathfinder Sensor/FO**, **Sierra TR**, **Bulleteer Mimetism(-6) Spitfire**, and **Peacemaker+AuxBot** are valuable but require their own separate physical bases. Peacemaker with **AuxBot** creates two figures; a support-heavy list cannot also afford three TAGs. | **Proxy alternate gun and secondary REM chassis** until real lists require them simultaneously. **Buy one preferred attack REM**, cheap Baggage/flash/support and required second AuxBot; avoid pretending one chassis stands for two fielded models. |
| **Extra Yuan Yuan, Zellenkrieger/Extreme Zellenkrieger, Diggers, motorized bounty hunter or Libertos** | **All can have worthwhile smoke/CC/cheap trade roles**, but **many are Irregular/Impetuous**, and Druze is already paying 20–28pt per line trooper. **Zellenkrieger FTO8 has no Smoke**, unlike solo 8pt smoke variants; it **may** fill an eligible Druze team, not automatically throw Smoke. **Motorized Bounty Hunter** needs motorcycle footprint. | **Buy only the first useful actual trade models; proxy additional Irregular warbands/bikes** before collecting AVA. **Don't skip a first Yuan Yuan/Digger** when it is your inexpensive smoke or close-defense answer. |
| **Scarface & Cordelia + Turtlemek, Triphammer + Turtlemek and Anaconda bought all together** | **Reasoned purchase diversity warning:** **Scarface** is a composite **TAG+Cordelia Engineer+Ancillary**, **Triphammer48/52/53** includes a **separate TurtleMek**, and Anaconda's **Operator is an Escape System state**, not an extra selectable TAG. **Scarface Beta76/1.5 AP HMG** and **Triphammer48/0 HRL** can make materially different lists. | **Proxy-test TAG chassis/partners before committing to multiple large models**. A first Scarface kit needs **Scarface, Cordelia, TurtleMek** represented; Anaconda's Operator may require an **S2 representation when it dismounts**. Do not mark one TAG proxy as simultaneously fielding another. |

**Druze priority:** **KHD+Pitcher Druze**, enough **Brawler/other legitimate team bodies**, **one Hunzakut FO**, actual Smoke/cheap defense, and **one** selected efficient main gun or TAG module. **Main default skip**: Anaconda as first TAG versus Scarface *with the full composite price clearly stated*. **Main profile-only avoids**: Druze HMG as generalist and the nonexistent linked Guided Clipper. Sources: [D1](https://www.youtube.com/watch?v=jmgABxVFU9U), [D2](https://open.spotify.com/episode/4hppzgYaNybZeMexaNaykO), [Druze current tactica](druze.md#tactical-research--druze-bayram-security-reviewed-2026-10-23).

#### 6. Cross-mercenary — reuse, proxy rules and multi-body purchase traps

**Inventory note:** no separately verified, complete Druze/Ikari/StarCo/Dahshat/WhiteCo miniature inventories were found. The project *does* contain physical inventories for [Shindenbutai](../../inventory/shindenbutai.md), [Caledonia](../../inventory/caledonia.md), [Kestrel](../../inventory/kestrel.md), [Military Orders](../../inventory/military-orders.md) and [Steel Phalanx](../../inventory/steel-phalanx.md). **Cross-collection re-use is a candidate, not an assumption that the same sculpt is unoccupied in a simultaneous list.** In particular, two Yáoxiè Rui Shi/Lù Duān physical chassis, PanO Dronbot/Mulebot pools and both Yojimbo forms are documented in Shinden; Caledonia Cateran(s) and shared Warcor can be available where current roster allows. Check [inventory rows](../../inventory/shindenbutai.md) before ordering equivalents for an NA2 list.

| Physical category and example models | Recommended test/reuse | Do not overbuy or misrepresent |
|---|---|---|
| **Shared NA2 infantry characters** — Arslan, Valerya, Druze, Brawler, Digger, Aïda, Saito, Wild Bill, Hawkwood, Knauf, Uhahu, Parvati etc. | Use an appropriate, distinctly identified **same-size Corvus Belli infantry proxy** in each legal sectorial; prioritize characters actually in the intended list. One sculpt can represent **non-simultaneous** options across armies, or another legal unit if accepted. | **Do not import faction access.** Druze Arslan differs from Ikari Arslan value; StarCo Knauf cannot be WhiteCo Hawkwood by changing cards without an allowed physical proxy; one model can't be two deployed characters at once. |
| **Alguacil/Fusilier/Keisotsu/Ghulam/Druze/Brawler weapon variants and FTO** | Use existing generic or same-troop properly sized mini to test LT/FO/KHD/Doctor/Engineer/HMG/ML choices; clearly declare the selected loadout. | Buy **extra specific weapon sculptures** when they are actually **different legal simultaneous troopers**, not because a variant appears in Army. FTO status and link membership must be checked by exact sectorial. |
| **TAGs and supporting model counts** — Anaconda S7, Scarface+Cordelia+Turtlemek, Triphammer+Turtlemek, Maghariba S8+Jandab, Gūijiă+Shàngdiào | Borrow a *correct silhouette/base TAG* and **all separately deployed ancillary/Engineer figures** in the actual selected package. A Tag-equivalent S7 base does not automatically stand for an **S8 Maghariba**. Anaconda **Operator** appears on escape; plan an S2 model/representation then. | Scarface composite is **not just a Scarface TAG purchase**; regular physical count includes **Cordelia** and **TurtleMek**. Ancillaries aren't independent Regular Order generators. Buy large sculpts after real mission tests, not for one-time novelty. |
| **Peripherals/Servants** — Fiddler+Jackbot(s), Carmen+Bâtard, Peacemaker+Auxbot, Yáozăo/Nasmat/Zondbot, Yojimbo Koalas, Synchronized companions | Proxy **each fielded partner** with a separate, correctly based body; **equipment markers** (mine, Koala etc.) have their own marker requirements but don't make extra troopers. | Some options do **not** include companions (e.g. Fiddler FTO vs independent Jackbot; specific Peacemaker without Auxbot). Don't buy all option-specific peripherals without selecting their legal profiles. |
| **Shared JSA/Chinese/PanO REM chassis** — Yáoxiè Rui Shi/Lù Duān, Dronbot Pathfinder/Clipper/Sierra/Fugazi, Yáopú/Pangguling/Mulebot, Rafiq/Fanous, Traktor Mul | Reuse documented **2 Yáoxiè chassis**, **4 PanO Dronbots** and **2 PanO Mulebots** as **compatible-sized** temporary replacements, provided current event proxy permissions. **Traktor Mul S4** and **Maghariba S8** must be represented by their own size, not any spare S3 Dronbot. | Buy only chassis that actually **co-deploy in an NA2 list**, or are needed for correct base/size/appearance. The inventory's two Rui Shi/Lù Duān models are **two physical total**, not two of each. |
| **Smoke/Irregular warbands and airborne attackers** — Yuan Yuan, Bashi Bazouk, Hunzakut, Desperado, Libertos, Kum, Irmandinho, McMurrough, Motorized Bounty Hunter, Yojimbo | Proxy a rarely used cheap trader/AD with a **distinct correct-size** infantry/motorcycle/warband in the intended legal roster. The [Shinden inventory](../../inventory/shindenbutai.md) confirms foot+mounted Yojimbo; **motorcycle S4** differs from ordinary S2 smoke infantry. | Don't buy up to AVA automatically. **Hunzakut FO** and **Irmandinho Engineer** are Irregular; too many Irregular trades can starve the main gun of pooled Regular activations. |
| **Medium-heavy specialized silhouettes** — Al Fasid S5, Daiyōkai S5, Karakuri S2, Wú Míng S2, Riot Grrl S2, and vehicle/motorbike models | Use **correct silhouette/base** first and choose models with clearly different identities. **S5** is not an ordinary S2 stand-in; a TAG/Vehicle cannot be represented as common infantry at organized play without organizer permission. | Don't buy an S5 heavyweight simply because you already own a generic S2 HI; verify actual match and legal current unit. |
| **No actual rules on “linked Guided” unless exact profile supports both** | Druze/Ikari Clipper FTO direct ML is **not Guided**, while the Guided profile is **unlinked**; WhiteCo Clipper FTO has **no Fireteam access**; StarCo Stempler FTO likewise not linkable. Test individual **correct unit/profile/network** combinations in Army before purchase. | Do not buy REM artillery boxes for a nonexistent *FTO Guided* bonus. A Guided missile requires actual Targeted source, not merely an expensive KHD with a Pitcher. |
| **Legacy N4/early N5/Spec-Ops/Team-Ops minis** | Reuse sculpts as current legal proxies where sizes and organizer acceptance fit; edition-old fireteam boxes aren't automatically useful whole bundles. | **Do not buy optional-mode-only troops solely for standard play**. A saved N4 TAG/Fireteam roster isn't an N5.3 shopping list. |

**Combined “do not bother buying first” shortlist (not all-profile play bans):** **Druze** Anaconda without a real 59pt plan, HMG-only Druze and full Fiddler multi-bot kit; **Ikari** Arslan and unsupported Al Fasid/S5 or multiple TAGs; **StarCo** solo Anaconda/Triphammer without the relevant Armored plan, expensive optional Alguacil SWC guns, second Engineer/sniper collection; **Dahshat** Al Fasid as redundant gun, optional Ghulam HMG/ML, unproven extra guided/Maghariba TAG and excess Irregular duplicates; **WhiteCo** Chaksa Longarm box and Wild Bill before a specific team, Fusilier heavy weapon sculpts, nonplanned Anaconda and alternate Hawkwood/HD+ kits. **All** deserve re-evaluation if the exact mission, missing collection capability or verified legal Fireteam calls for them.

**Proxy policy/physical limit:** Always declare which legal Army profile each figure represents before playing. Keep its **proper base, silhouette, visibility geometry, different body for each simultaneous trooper, and actual peripheral/Ancillary count**; check current ITS and event organizer proxy policy before organized play. Proxies never change Army availability, AVA, SWC, Fireteam chart, model's real equipment, or independent Order generation.
